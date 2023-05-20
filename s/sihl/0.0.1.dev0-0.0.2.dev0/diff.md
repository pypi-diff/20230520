# Comparing `tmp/sihl-0.0.1.dev0.tar.gz` & `tmp/sihl-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sihl-0.0.1.dev0.tar", max compression
+gzip compressed data, was "sihl-0.0.2.dev0.tar", max compression
```

## Comparing `sihl-0.0.1.dev0.tar` & `sihl-0.0.2.dev0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0      836 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     1310 2023-05-06 18:19:45.998105 sihl-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      229 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/heads/__init__.py
--rw-r--r--   0        0        0     2274 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/heads/binary_classification.py
--rw-r--r--   0        0        0     2861 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/heads/multiclass_classification.py
--rw-r--r--   0        0        0     2659 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/heads/multilabel_classification.py
--rw-r--r--   0        0        0     3283 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/lightning_module.py
--rw-r--r--   0        0        0     6338 2023-05-06 18:19:33.737782 sihl-0.0.1.dev0/src/sihl/torchvision_backbone.py
--rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 sihl-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-20 16:08:12.727536 sihl-0.0.2.dev0/LICENSE
+-rw-r--r--   0        0        0      897 2023-05-20 16:08:25.023681 sihl-0.0.2.dev0/README.md
+-rw-r--r--   0        0        0     1334 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0      233 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/__init__.py
+-rw-r--r--   0        0        0     2237 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/binary_classification.py
+-rw-r--r--   0        0        0     2832 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/multiclass_classification.py
+-rw-r--r--   0        0        0     2630 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/heads/multilabel_classification.py
+-rw-r--r--   0        0        0     2936 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/lightning_module.py
+-rw-r--r--   0        0        0     6170 2023-05-20 16:08:25.027681 sihl-0.0.2.dev0/src/sihl/torchvision_backbone.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 sihl-0.0.2.dev0/PKG-INFO
```

### Comparing `sihl-0.0.1.dev0/LICENSE` & `sihl-0.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sihl-0.0.1.dev0/pyproject.toml` & `sihl-0.0.2.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sihl"
-version = "0.0.1-dev"
+version = "0.0.2-dev"
 description = "Simple Image Heads and Layers"
 authors = ["jonregef <jon.regef@pm.me>"]
 readme = "README.md"
 license = "MIT"
 # homepage = "https://github.com/sihlAI/sihl"
 # repository = "https://github.com/sihlAI/sihl"
 
@@ -24,14 +24,15 @@
 pre-commit = "^3.3.1"
 pre-commit-hooks = "^4.4.0"
 isort = "^5.12.0"
 pyupgrade = "^3.3.2"
 kaggle = "^1.5.13"
 torchinfo = "^1.7.2"
 lightning = "^2.0.2"
+tensorboard = "^2.13.0"
 
 [tool.poetry.extras]
 lightning = ["lightning"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sihl-0.0.1.dev0/src/sihl/heads/binary_classification.py` & `sihl-0.0.2.dev0/src/sihl/heads/multiclass_classification.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,76 @@
-from __future__ import annotations  # noqa: D100
+from __future__ import annotations
 
 import torch
-import torchmetrics
 from torch import Tensor
 from torch import nn
+from torchmetrics.classification import MulticlassAccuracy
+from torchmetrics.classification import MulticlassPrecision
+from torchmetrics.classification import MulticlassRecall
 
 
-class BinaryClassification(nn.Module):  # noqa: D101
-    def __init__(self, in_channels: int) -> None:  # noqa: D107
+class MulticlassClassification(nn.Module):
+    def __init__(
+        self,
+        in_channels: int,
+        num_classes: int,
+        level: int = -1,
+        label_weights: list[float] | None = None,
+        label_smoothing: float = 0.0,
+    ) -> None:
         super().__init__()
+        self.num_classes = num_classes
+        self.level = level
+        self.label_weights = torch.tensor(label_weights) if label_weights else None
+        self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
-            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, 1)
+            nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, num_classes)
         )
 
-    def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:  # noqa: D102
-        scores = torch.sigmoid(self.net(inputs[-1])).squeeze(-1)
-        return scores, scores > 0.5
+    def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
+        scores, classes = torch.max(
+            torch.nn.functional.softmax(self.net(inputs[self.level]), dim=1), dim=1
+        )
+        return scores, classes
 
-    def training_step(  # noqa: D102
-        self, inputs: list[Tensor], categories: Tensor
+    def training_step(
+        self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[-1]).squeeze(-1)
-        targets = categories.to(logits.dtype).to(logits.device)
-        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
+        logits = self.net(inputs[self.level])
+        loss = torch.nn.functional.cross_entropy(
+            logits,
+            labels,
+            weight=self.label_weights,
+            label_smoothing=self.label_smoothing,
+        )
         return loss, {}
 
-    def on_validation_start(self) -> None:  # noqa: D102
-        self.accuracy_computer = torchmetrics.classification.BinaryAccuracy()
-        self.precision_computer = torchmetrics.classification.BinaryPrecision()
-        self.recall_computer = torchmetrics.classification.BinaryRecall()
+    def on_validation_start(self) -> None:
+        self.accuracy_computer = MulticlassAccuracy(num_classes=self.num_classes)
+        self.precision_computer = MulticlassPrecision(num_classes=self.num_classes)
+        self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
 
-    def validation_step(  # noqa: D102
-        self, inputs: list[Tensor], categories: Tensor
+    def validation_step(
+        self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        self.accuracy_computer = self.accuracy_computer.to(inputs[-1].device)
-        self.precision_computer = self.precision_computer.to(inputs[-1].device)
-        self.recall_computer = self.recall_computer.to(inputs[-1].device)
-        logits = self.net(inputs[-1]).squeeze(-1)
-        targets = categories.to(logits.dtype).to(logits.device)
-        loss = torch.nn.functional.binary_cross_entropy_with_logits(logits, targets)
-        self.accuracy_computer.update(logits, targets)
-        self.precision_computer.update(logits, targets)
-        self.recall_computer.update(logits, targets)
+        input = inputs[self.level]
+        self.accuracy_computer = self.accuracy_computer.to(input.device)
+        self.precision_computer = self.precision_computer.to(input.device)
+        self.recall_computer = self.recall_computer.to(input.device)
+        logits = self.net(input)
+        loss = torch.nn.functional.cross_entropy(
+            logits,
+            labels,
+            weight=self.label_weights,
+            label_smoothing=self.label_smoothing,
+        )
+        self.accuracy_computer.update(logits, labels)
+        self.precision_computer.update(logits, labels)
+        self.recall_computer.update(logits, labels)
         return loss, {}
 
-    def on_validation_end(self) -> dict[str, float]:  # noqa: D102
+    def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
```

### Comparing `sihl-0.0.1.dev0/src/sihl/heads/multiclass_classification.py` & `sihl-0.0.2.dev0/src/sihl/heads/multilabel_classification.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,68 @@
-from __future__ import annotations  # noqa: D100
+from __future__ import annotations
 
 import torch
 from torch import Tensor
 from torch import nn
-from torchmetrics.classification import MulticlassAccuracy
-from torchmetrics.classification import MulticlassPrecision
-from torchmetrics.classification import MulticlassRecall
+from torchmetrics.classification import MultilabelAccuracy
+from torchmetrics.classification import MultilabelPrecision
+from torchmetrics.classification import MultilabelRecall
 
 
-class MulticlassClassification(nn.Module):  # noqa: D101
-    def __init__(  # noqa: D107
+class MultilabelClassification(nn.Module):
+    def __init__(
         self,
         in_channels: int,
         num_classes: int,
+        level: int = -1,
         label_weights: list[float] | None = None,
-        label_smoothing: float = 0.0,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
+        self.level = level
         self.label_weights = torch.tensor(label_weights) if label_weights else None
-        self.label_smoothing = label_smoothing
         self.net = nn.Sequential(
             nn.AdaptiveAvgPool2d(1), nn.Flatten(), nn.Linear(in_channels, num_classes)
         )
 
-    def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:  # noqa: D102
-        scores, classes = torch.max(
-            torch.nn.functional.softmax(self.net(inputs[-1]), dim=1), dim=1
+    def forward(self, inputs: list[Tensor]) -> tuple[Tensor, Tensor]:
+        scores, classes = torch.sort(
+            torch.sigmoid(self.net(inputs[self.level])), descending=True
         )
         return scores, classes
 
-    def training_step(  # noqa: D102
+    def training_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        logits = self.net(inputs[-1])
-        loss = torch.nn.functional.cross_entropy(
-            logits,
-            labels,
-            weight=self.label_weights,
-            label_smoothing=self.label_smoothing,
+        logits = self.net(inputs[self.level])
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(
+            logits, labels, pos_weight=self.label_weights
         )
         return loss, {}
 
-    def on_validation_start(self) -> None:  # noqa: D102
-        self.accuracy_computer = MulticlassAccuracy(num_classes=self.num_classes)
-        self.precision_computer = MulticlassPrecision(num_classes=self.num_classes)
-        self.recall_computer = MulticlassRecall(num_classes=self.num_classes)
+    def on_validation_start(self) -> None:
+        self.accuracy_computer = MultilabelAccuracy(num_labels=self.num_classes)
+        self.precision_computer = MultilabelPrecision(num_labels=self.num_classes)
+        self.recall_computer = MultilabelRecall(num_labels=self.num_classes)
 
-    def validation_step(  # noqa: D102
+    def validation_step(
         self, inputs: list[Tensor], labels: Tensor
     ) -> tuple[Tensor, dict[str, float]]:
-        self.accuracy_computer = self.accuracy_computer.to(inputs[-1].device)
-        self.precision_computer = self.precision_computer.to(inputs[-1].device)
-        self.recall_computer = self.recall_computer.to(inputs[-1].device)
-        logits = self.net(inputs[-1])
-        loss = torch.nn.functional.cross_entropy(
-            logits,
-            labels,
-            weight=self.label_weights,
-            label_smoothing=self.label_smoothing,
+        input = inputs[self.level]
+        self.accuracy_computer = self.accuracy_computer.to(input.device)
+        self.precision_computer = self.precision_computer.to(input.device)
+        self.recall_computer = self.recall_computer.to(input.device)
+        logits = self.net(input)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(
+            logits, labels, pos_weight=self.label_weights
         )
         self.accuracy_computer.update(logits, labels)
         self.precision_computer.update(logits, labels)
         self.recall_computer.update(logits, labels)
         return loss, {}
 
-    def on_validation_end(self) -> dict[str, float]:  # noqa: D102
+    def on_validation_end(self) -> dict[str, float]:
         return {
             "accuracy": self.accuracy_computer.compute().item(),
             "precision": self.precision_computer.compute().item(),
             "recall": self.recall_computer.compute().item(),
         }
```

### Comparing `sihl-0.0.1.dev0/src/sihl/lightning_module.py` & `sihl-0.0.2.dev0/src/sihl/lightning_module.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,89 +1,80 @@
-from __future__ import annotations  # noqa: D100
+from __future__ import annotations
 
 import logging
 from typing import Any
 
 import lightning.pytorch as pl
 import torch
 from torch import Tensor
 from torch import nn
+from torch.optim import Optimizer
+from torch.optim.lr_scheduler import _LRScheduler as Scheduler
 
 
-class LightningModule(pl.LightningModule):  # type: ignore
-    """Lightning module wrapper for conveniently training SIHL models."""
+class LightningModule(pl.LightningModule):  # type:ignore
+    """Lightning module wrapper for conveniently training Sihl models."""
 
-    def __init__(  # noqa: D107
+    def __init__(
         self,
         backbone: nn.Module,
         neck: nn.Module | None,
         head: nn.Module,
-        optimizer: type[torch.optim.Optimizer] = torch.optim.AdamW,
+        optimizer: type[Optimizer] = torch.optim.AdamW,
         optimizer_kwargs: dict[str, Any] | None = None,
-        scheduler: type[torch.optim.lr_scheduler._LRScheduler] | None = None,
+        scheduler: type[Scheduler] | None = None,
         scheduler_kwargs: dict[str, Any] | None = None,
     ):
         super().__init__()
         self.optimizer = optimizer
         self.optimizer_kwargs = optimizer_kwargs or {}
         self.scheduler = scheduler
         self.scheduler_kwargs = scheduler_kwargs or {}
         self.backbone = backbone
         self.neck = neck or nn.Identity()
         self.head = head
 
-    def forward(self, input: Tensor) -> tuple[Tensor, ...]:  # noqa: D102
-        return self.head(self.neck(self.backbone(input)))  # type: ignore
+    def forward(self, input: Tensor) -> tuple[Tensor, ...]:
+        return self.head(self.neck(self.backbone(input)))  # type:ignore
 
-    def training_step(  # noqa: D102
-        self, batch: tuple[Tensor, Any], batch_idx: int
-    ) -> Tensor:
+    def training_step(self, batch: tuple[Tensor, Any], batch_idx: int) -> Tensor:
         x, *y = batch
         head_inputs = self.neck(self.backbone(x))
-        loss, metrics = self.head.training_step(head_inputs, *y)  # type: ignore
+        loss, metrics = self.head.training_step(head_inputs, *y)  # type:ignore
         self.log("train/loss", loss, on_epoch=False, on_step=True, prog_bar=True)
         self.log_dict(metrics, on_epoch=False, on_step=True, prog_bar=True)
         scheduler = self.lr_schedulers()
         if scheduler:
             scheduler.step()
             lr = scheduler.get_last_lr()[0]
             self.log("lr", lr, on_epoch=False, on_step=True, prog_bar=True)
-        return loss  # type: ignore
+        return loss  # type:ignore
 
-    def validation_step(  # noqa: D102
-        self, batch: tuple[Tensor, Any], batch_idx: int
-    ) -> Tensor:
+    def validation_step(self, batch: tuple[Tensor, Any], batch_idx: int) -> Tensor:
         x, *y = batch
         head_inputs = self.neck(self.backbone(x))
-        loss, metrics = self.head.validation_step(head_inputs, *y)  # type: ignore
-        self.log("valid/loss", loss, on_epoch=False, on_step=True, prog_bar=True)
-        self.log_dict(metrics, on_epoch=False, on_step=True, prog_bar=True)
-        return loss  # type: ignore
+        loss, metrics = self.head.validation_step(head_inputs, *y)  # type:ignore
+        return loss  # type:ignore
 
-    def configure_optimizers(  # noqa: D102
+    def configure_optimizers(
         self,
-    ) -> (
-        torch.optim.Optimizer
-        | tuple[
-            list[torch.optim.Optimizer], list[torch.optim.lr_scheduler._LRScheduler]
-        ]
-    ):
+    ) -> Optimizer | tuple[list[Optimizer], list[Scheduler]]:
         optimizer = self.optimizer(self.parameters(), **self.optimizer_kwargs)
         if self.scheduler:
             scheduler = self.scheduler(optimizer, **self.scheduler_kwargs)
             return [optimizer], [scheduler]
         return optimizer
 
-    def on_validation_start(self) -> None:  # noqa: D102
+    def on_validation_start(self) -> None:
         try:
-            self.head.on_validation_start()  # type: ignore
+            self.head.on_validation_start()  # type:ignore
         except Exception as e:
             logging.warn(e)
             pass
 
-    def on_validation_epoch_end(self) -> None:  # noqa: D102
+    def on_validation_epoch_end(self) -> None:
         try:
-            val_metrics = self.head.on_validation_end()  # type: ignore
+            val_metrics = self.head.on_validation_end()  # type:ignore
             self.log_dict(val_metrics, on_epoch=True, on_step=False, prog_bar=True)
         except Exception as e:
             logging.warn(e)
             pass
```

### Comparing `sihl-0.0.1.dev0/src/sihl/torchvision_backbone.py` & `sihl-0.0.2.dev0/src/sihl/torchvision_backbone.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from __future__ import annotations  # noqa: D100
+from __future__ import annotations
 
 from typing import Final
 
 import torch
 import torchvision
 from torch import Tensor
 from torch import fx
@@ -12,16 +12,16 @@
 from torchvision.models.feature_extraction import create_feature_extractor
 
 
 __all__ = ["TorchvisionBackbone"]
 
 
 @torch.no_grad()
-def update_input_channels(  # noqa: D103
-    fx_module: fx.GraphModule, in_channels: int  # type: ignore
+def update_input_channels(
+    fx_module: fx.GraphModule, in_channels: int  # type:ignore
 ) -> None:
     modules = dict(fx_module.named_modules())
     first_conv_node = next(
         node
         for node in fx_module.graph.nodes
         if matches_module_pattern([nn.Conv2d], node, modules)
     )
@@ -42,27 +42,25 @@
         new_conv.weight[:, channel_idx] = weight[:, channel_idx % 3]
     replace_node_module(first_conv_node.args[0], modules, new_conv)
     first_conv_node.replace_all_uses_with(first_conv_node.args[0])
     fx_module.graph.erase_node(first_conv_node)
     fx_module.recompile()
 
 
-class Normalize(nn.Module):  # noqa: D101
-    def __init__(  # noqa: D107
-        self, mean: tuple[float, ...], std: tuple[float, ...]
-    ) -> None:
+class Normalize(nn.Module):
+    def __init__(self, mean: tuple[float, ...], std: tuple[float, ...]) -> None:
         super().__init__()
         self.register_buffer("mean", torch.tensor(mean).reshape(1, -1, 1, 1))
         self.register_buffer("std", torch.tensor(std).reshape(1, -1, 1, 1))
 
-    def forward(self, x: Tensor) -> Tensor:  # noqa: D102
+    def forward(self, x: Tensor) -> Tensor:
         return (x - self.mean) / self.std
 
 
-class TorchvisionBackbone(nn.Module):  # noqa: D101
+class TorchvisionBackbone(nn.Module):
     all_level_names: Final[dict[str, list[str]]] = {
         "efficientnet_b0": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b1": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b2": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b3": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b4": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
         "efficientnet_b5": [f"features.{_}" for _ in (1, 2, 3, 5, 8)],
@@ -81,31 +79,29 @@
         "resnet101": ["relu"] + [f"layer{_}" for _ in [1, 2, 3, 4]],
         "resnet152": ["relu"] + [f"layer{_}" for _ in [1, 2, 3, 4]],
         "resnet18": ["relu"] + [f"layer{_}" for _ in [1, 2, 3, 4]],
         "resnet34": ["relu"] + [f"layer{_}" for _ in [1, 2, 3, 4]],
         "resnet50": ["relu"] + [f"layer{_}" for _ in [1, 2, 3, 4]],
         "regnet_x_16gf": ["stem"] + [f"trunk_output.block{_}" for _ in [1, 2, 3, 4]],
     }
-    min_level: Final[int] = 1
-    max_level: Final[int] = 5
 
-    def __init__(  # noqa: D107, C901
+    def __init__(
         self,
         name: str,
         pretrained: bool = False,
         input_channels: int = 3,
         frozen_levels: int = 0,
     ) -> None:
         super().__init__()
         self.name = name
         try:
             level_names = self.all_level_names[name]
         except KeyError as error:
             raise KeyError(
-                f"Architecture {name} is not supported. "  # noqa: S608
+                f"Architecture {name} is not supported. "
                 f"Select from {list(self.all_level_names.keys())}"
             ) from error
         self.normalize = (
             Normalize(mean=(0.485, 0.456, 0.406), std=(0.229, 0.224, 0.225))
             if pretrained and input_channels == 3
             else Normalize(mean=(0.5,), std=(0.5,))
         )
@@ -132,13 +128,14 @@
                     last_level_reached = True
                 if last_level_reached and last_frozen_name not in module_name:
                     freezing = False
                 for param in torchvision_model.get_submodule(module_name).parameters():
                     param.requires_grad = not freezing
         setattr(self, name, torchvision_model)
         self.dummy_input = torch.empty((1, input_channels, 64, 64))
-        self.output_channels = [
+        self.output_channels = [input_channels] + [
             _.shape[1] for _ in getattr(self, name)(self.dummy_input).values()
         ]
 
-    def forward(self, x: Tensor) -> list[Tensor]:  # noqa: D102
-        return list(getattr(self, self.name)(self.normalize(x)).values())
+    def forward(self, x: Tensor) -> list[Tensor]:
+        x = self.normalize(x)
+        return [x] + list(getattr(self, self.name)(x).values())
```

### Comparing `sihl-0.0.1.dev0/PKG-INFO` & `sihl-0.0.2.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sihl
-Version: 0.0.1.dev0
+Version: 0.0.2.dev0
 Summary: Simple Image Heads and Layers
 License: MIT
 Author: jonregef
 Author-email: jon.regef@pm.me
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,27 +18,27 @@
 Requires-Dist: torchvision (>=0.15.1,<0.16.0)
 Description-Content-Type: text/markdown
 
 # Simple Image Heads and Layers
 
 [![PyPI](https://img.shields.io/pypi/v/sihl.svg)][pypi_]
 [![python versions](https://img.shields.io/pypi/pyversions/sihl)][python version]
-[![codecov](https://codecov.io/gh/sihlAI/sihl/branch/main/graph/badge.svg?token=RZE0XM6J5O)][codecov]
+[![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jonregef/c203d6bce2a485ab49d1814ff3218a06/raw/covbadge.json)][coverage]
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/sihl/
 [python version]: https://pypi.org/project/sihl
-[codecov]: https://codecov.io/gh/sihlAI/sihl
+[coverage]: https://coverage.readthedocs.io/en/7.2.5/
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Installation
 
 ```console
-$ pip install sihl
+pip install sihl
 ```
 
 <!-- github-only -->
 
 [license]: https://github.com/sihlAI/sihl/blob/main/LICENSE
```

