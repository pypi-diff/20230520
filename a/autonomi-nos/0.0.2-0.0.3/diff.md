# Comparing `tmp/autonomi_nos-0.0.2-py3-none-any.whl.zip` & `tmp/autonomi_nos-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,49 +1,51 @@
-Zip file size: 40865 bytes, number of entries: 47
+Zip file size: 42344 bytes, number of entries: 49
 -rw-rw-r--  2.0 unx      119 b- defN 23-Apr-23 00:49 nos/__init__.py
 -rw-rw-r--  2.0 unx      561 b- defN 23-May-16 21:17 nos/constants.py
 -rw-rw-r--  2.0 unx       93 b- defN 23-May-01 21:40 nos/exceptions.py
 -rw-rw-r--  2.0 unx      940 b- defN 23-May-01 21:40 nos/logging.py
--rw-rw-r--  2.0 unx     2716 b- defN 23-May-16 21:17 nos/protoc.py
--rw-rw-r--  2.0 unx       22 b- defN 23-May-17 22:26 nos/version.py
+-rw-rw-r--  2.0 unx     2778 b- defN 23-May-19 23:50 nos/protoc.py
+-rw-rw-r--  2.0 unx       22 b- defN 23-May-19 23:53 nos/version.py
 -rw-rw-r--  2.0 unx      110 b- defN 23-Apr-23 00:49 nos/cli/benchmark.py
 -rw-rw-r--  2.0 unx      455 b- defN 23-May-16 21:17 nos/cli/cli.py
 -rw-rw-r--  2.0 unx     1983 b- defN 23-May-16 21:17 nos/cli/docker.py
 -rw-rw-r--  2.0 unx     1294 b- defN 23-Apr-23 00:49 nos/cli/hub.py
--rw-rw-r--  2.0 unx     6244 b- defN 23-May-16 21:17 nos/cli/serve_grpc.py
+-rw-rw-r--  2.0 unx     6094 b- defN 23-May-19 20:10 nos/cli/serve_grpc.py
 -rw-rw-r--  2.0 unx     5962 b- defN 23-May-16 21:17 nos/cli/serve_http.py
 -rw-rw-r--  2.0 unx     3479 b- defN 23-May-16 21:17 nos/cli/system.py
 -rw-rw-r--  2.0 unx      425 b- defN 23-May-05 01:05 nos/cli/utils.py
--rw-rw-r--  2.0 unx      148 b- defN 23-May-16 21:17 nos/client/__init__.py
+-rw-rw-r--  2.0 unx      141 b- defN 23-May-18 22:36 nos/client/__init__.py
 -rw-rw-r--  2.0 unx       92 b- defN 23-May-12 23:31 nos/client/exceptions.py
--rw-rw-r--  2.0 unx     6048 b- defN 23-May-16 21:17 nos/client/grpc/client.py
--rw-rw-r--  2.0 unx     7153 b- defN 23-May-17 22:02 nos/executors/ray.py
--rw-rw-r--  2.0 unx     2087 b- defN 23-May-15 21:54 nos/hub/__init__.py
--rw-rw-r--  2.0 unx     1812 b- defN 23-May-15 21:54 nos/hub/config.py
+-rw-rw-r--  2.0 unx     7307 b- defN 23-May-19 20:10 nos/client/grpc.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-18 22:36 nos/executors/__init__.py
+-rw-rw-r--  2.0 unx     6237 b- defN 23-May-19 22:34 nos/executors/ray.py
+-rw-rw-r--  2.0 unx     2985 b- defN 23-May-19 20:10 nos/hub/__init__.py
+-rw-rw-r--  2.0 unx     2195 b- defN 23-May-19 20:10 nos/hub/config.py
 -rw-rw-r--  2.0 unx      902 b- defN 23-May-12 23:31 nos/hub/spec.py
 -rw-rw-r--  2.0 unx      242 b- defN 23-May-15 21:54 nos/models/__init__.py
 -rw-rw-r--  2.0 unx     2370 b- defN 23-May-10 21:27 nos/models/clip.py
 -rw-rw-r--  2.0 unx     2028 b- defN 23-May-12 23:31 nos/models/faster_rcnn.py
 -rw-rw-r--  2.0 unx     2651 b- defN 23-May-01 21:36 nos/models/stable_diffusion.py
 -rw-rw-r--  2.0 unx       66 b- defN 23-May-13 02:32 nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py
 -rw-rw-r--  2.0 unx     2589 b- defN 23-May-13 02:01 nos/models/openmmlab/mmdetection/mmdetection.py
 -rw-rw-r--  2.0 unx      370 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py
 -rw-rw-r--  2.0 unx     3187 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py
 -rw-rw-r--  2.0 unx     1765 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py
 -rw-rw-r--  2.0 unx     3828 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py
 -rw-rw-r--  2.0 unx      304 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py
 -rw-rw-r--  2.0 unx     5340 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
 -rw-rw-r--  2.0 unx      177 b- defN 23-May-15 21:54 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
+-rw-rw-r--  2.0 unx     1409 b- defN 23-May-19 20:10 nos/proto/nos_service.proto
 -rw-rw-r--  2.0 unx      156 b- defN 23-May-16 21:17 nos/server/__init__.py
--rw-rw-r--  2.0 unx     6235 b- defN 23-May-16 21:17 nos/server/docker.py
--rw-rw-r--  2.0 unx     3004 b- defN 23-May-17 22:02 nos/server/runtime.py
--rw-rw-r--  2.0 unx     8470 b- defN 23-May-17 22:02 nos/server/service.py
+-rw-rw-r--  2.0 unx     6229 b- defN 23-May-19 20:10 nos/server/docker.py
+-rw-rw-r--  2.0 unx     3004 b- defN 23-May-18 22:36 nos/server/runtime.py
+-rw-rw-r--  2.0 unx     8880 b- defN 23-May-19 22:34 nos/server/service.py
 -rw-rw-r--  2.0 unx      373 b- defN 23-Apr-23 00:49 nos/test/benchmark.py
--rw-rw-r--  2.0 unx      378 b- defN 23-May-17 22:02 nos/test/conftest.py
--rw-rw-r--  2.0 unx     1324 b- defN 23-May-17 22:02 nos/test/utils.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6038 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       86 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        4 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     4109 b- defN 23-May-17 22:26 autonomi_nos-0.0.2.dist-info/RECORD
-47 files, 98899 bytes uncompressed, 34243 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx     1317 b- defN 23-May-19 22:34 nos/test/conftest.py
+-rw-rw-r--  2.0 unx     1324 b- defN 23-May-18 22:36 nos/test/utils.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5917 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       86 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        4 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     4266 b- defN 23-May-19 23:53 autonomi_nos-0.0.3.dist-info/RECORD
+49 files, 103216 bytes uncompressed, 35480 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -42,15 +42,18 @@
 
 Filename: nos/client/__init__.py
 Comment: 
 
 Filename: nos/client/exceptions.py
 Comment: 
 
-Filename: nos/client/grpc/client.py
+Filename: nos/client/grpc.py
+Comment: 
+
+Filename: nos/executors/__init__.py
 Comment: 
 
 Filename: nos/executors/ray.py
 Comment: 
 
 Filename: nos/hub/__init__.py
 Comment: 
@@ -96,14 +99,17 @@
 
 Filename: nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py
 Comment: 
 
 Filename: nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py
 Comment: 
 
+Filename: nos/proto/nos_service.proto
+Comment: 
+
 Filename: nos/server/__init__.py
 Comment: 
 
 Filename: nos/server/docker.py
 Comment: 
 
 Filename: nos/server/runtime.py
@@ -117,26 +123,26 @@
 
 Filename: nos/test/conftest.py
 Comment: 
 
 Filename: nos/test/utils.py
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/LICENSE
+Filename: autonomi_nos-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/METADATA
+Filename: autonomi_nos-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/WHEEL
+Filename: autonomi_nos-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/entry_points.txt
+Filename: autonomi_nos-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/top_level.txt
+Filename: autonomi_nos-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: autonomi_nos-0.0.2.dist-info/RECORD
+Filename: autonomi_nos-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nos/protoc.py

```diff
@@ -25,14 +25,15 @@
     def __init__(self) -> None:
         self.cache_dir.mkdir(parents=True, exist_ok=True)
 
         # Add cache dir to sys.path
         sys.path.append(str(self.cache_dir))
 
         # Compile all proto files from all paths
+        logger.debug(f"Compiling protos from: {PROTO_PATHS}")
         for path in itertools.chain.from_iterable(Path(path).glob("*.proto") for path in PROTO_PATHS):
             logger.debug(f"Compiling {path}")
             self.compile(str(path))
         logger.debug(f"Compiled modules: {self.list_modules()}")
 
     @classmethod
     def get(cls: "DynamicProtobufCompiler") -> "DynamicProtobufCompiler":
```

## nos/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## nos/cli/serve_grpc.py

```diff
@@ -15,20 +15,16 @@
 import rich.console
 import rich.status
 import rich.table
 import typer
 
 from nos.client import InferenceClient
 from nos.client.exceptions import NosClientException
-from nos.protoc import import_module
 
 
-nos_service_pb2 = import_module("nos_service_pb2")
-nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
-
 serve_grpc_cli = typer.Typer(name="serve-grpc", help="NOS gRPC Serve CLI.", no_args_is_help=True)
 console = rich.console.Console()
 
 
 @dataclass
 class gRPCConfig:
     """Common gRPC options"""
```

## nos/client/__init__.py

```diff
@@ -1,3 +1,3 @@
 from nos.client.exceptions import NosClientException
-from nos.client.grpc.client import InferenceClient
+from nos.client.grpc import InferenceClient
 from nos.constants import DEFAULT_GRPC_PORT
```

## nos/executors/ray.py

```diff
@@ -3,42 +3,35 @@
 This module provides a Ray executor for NOS. The Ray executor is a singleton
 instance that can be used to start a Ray head, connect to an existing Ray
 cluster, and submit tasks to Ray. We use Ray as a backend for distributed
 computation and containerize them in docker to isolate the environment.
 """
 import logging
 import os
-import subprocess
 import time
 from dataclasses import dataclass
 from typing import Optional
 
 import psutil
 import ray
 import rich.console
 import rich.panel
 import rich.status
 
-from nos.constants import NOS_TMP_DIR
 from nos.logging import LOGGING_LEVEL
 
 
 logger = logging.getLogger(__name__)
 
-
-NOS_RAY_ADDRESS = os.environ.get("NOS_RAY_ADDRESS", "auto")
-NOS_RAY_GCS_PORT = os.environ.get("NOS_RAY_GCS_PORT", 6379)
 NOS_RAY_NS = os.getenv("NOS_RAY_NS", "nos-dev")
 NOS_RAY_RUNTIME_ENV = os.getenv("NOS_RAY_ENV", None)
 
 
 @dataclass
 class RayRuntimeSpec:
-    address: str = NOS_RAY_ADDRESS
-    """Address of Ray head."""
     namespace: str = NOS_RAY_NS
     """Namespace for Ray runtime."""
     runtime_env: str = NOS_RAY_RUNTIME_ENV
     """Runtime environment for Ray runtime."""
 
 
 @dataclass
@@ -58,118 +51,110 @@
         return cls._instance
 
     def is_initialized(self) -> bool:
         """Check if Ray is initialized."""
         return ray.is_initialized()
 
     def init(self, max_attempts: int = 5, timeout: int = 60, retry_interval: int = 5) -> None:
-        """Initialize Ray exector (as a daemon).
+        """Initialize Ray exector.
+
+        This implementation forces Ray to start a new cluster instance via
+        `ray.init(address="local")` and then connecting to the
+        server via `ray.init(address="auto")`. The first call to
+        `ray.init(address="auto")` raises a `ConnectionError` and proceeds to
+        force-start a new ray cluster instance, followed by a second call to
+        `ray.init(address="auto")` which successfully connects to the server.
 
-        Currently, this method will first attempt to connect to an existing
-        Ray cluster (address="auto"). If it fails, it will start a Ray head
-        as a daemon, attempt to re-connect (upto a maximum of 5
-        attempts, or if timeout of 60 seconds is reached).
+        In the case of a Ray cluster already running, the first call to
+        `ray.init(address="auto")` will successfully connect to the server.
 
         Args:
             max_attempts: Number of retries to attempt to connect to an existing
             timeout: Time to wait for Ray to start. Defaults to 60 seconds.
             retry_interval: Time to wait between retries. Defaults to 5 seconds.
         """
         level = getattr(logging, LOGGING_LEVEL)
 
+        # Ignore predefined RAY_ADDRESS environment variable.
+        if "RAY_ADDRESS" in os.environ:
+            del os.environ["RAY_ADDRESS"]
+
         st = time.time()
         attempt = 0
 
         # Attempt to connect to an existing ray cluster.
         # Allow upto 5 attempts, or if timeout of 60 seconds is reached.
         console = rich.console.Console()
         while time.time() - st <= timeout and attempt < max_attempts:
             # Attempt to connect to an existing ray cluster in the background.
             try:
                 with console.status(
-                    f"[bold green] {self.__class__.__name__} :: Connecting to backend ... [/bold green]"
+                    "[bold green] InferenceExecutor :: Connecting to backend ... [/bold green]"
                 ) as status:
                     ray.init(
-                        address=self.spec.address,
+                        address="auto",
                         namespace=self.spec.namespace,
                         runtime_env=self.spec.runtime_env,
                         ignore_reinit_error=True,
                         configure_logging=True,
                         logging_level=logging.ERROR,
                         log_to_driver=level <= logging.ERROR,
                     )
                     status.stop()
-                    console.print(
-                        f"[bold green] ✓ {self.__class__.__name__} :: Connected to backend. (address={self.spec.address}) [/bold green]"
-                    )
+                    console.print("[bold green] ✓ InferenceExecutor :: Connected to backend. [/bold green]")
                 return True
-            except ConnectionError:
+            except ConnectionError as exc:
                 # If Ray head is not running (this results in a ConnectionError),
                 # start it in a background subprocess.
+                if attempt > 0:
+                    logger.error(
+                        f"Failed to connect to InferenceExecutor.\n"
+                        f"{exc}\n"
+                        f"Retrying {attempt}/{max_attempts} after {retry_interval}s..."
+                    )
                 self.start()
                 attempt += 1
-                logger.info(
-                    f"Failed to connect to Ray head. Retrying {attempt}/{max_attempts} after {retry_interval}s..."
-                )
+
                 time.sleep(retry_interval)
         return False
 
-    def start(self, wait: int = 5) -> Optional[int]:
-        """Start Ray head as daemon.
+    def start(self) -> None:
+        """Force-start a local instance of Ray head."""
+        level = getattr(logging, LOGGING_LEVEL)
 
-        Args:
-            wait: Time to wait for Ray to start. Defaults to 5 seconds.
-        """
         console = rich.console.Console()
         with console.status(
-            f"[bold green] {self.__class__.__name__} :: Starting ray head (as daemon) ... [/bold green]"
+            "[bold green] InferenceExecutor :: Backend initializing (as daemon) ... [/bold green]"
         ) as status:
-            # Check if Ray head is already running
-            if self.pid:
-                status.stop()
-                console.print(
-                    f"[bold yellow] {self.__class__.__name__} :: Ray head is already running. [/bold yellow]"
+            try:
+                ray.init(
+                    _node_name="nos-executor",
+                    address="local",
+                    namespace=self.spec.namespace,
+                    runtime_env=self.spec.runtime_env,
+                    ignore_reinit_error=False,
+                    include_dashboard=False,
+                    configure_logging=True,
+                    logging_level=logging.ERROR,
+                    log_to_driver=level <= logging.ERROR,
                 )
-                return self.pid
-            # Start Ray head if not running
-            RAY_TMP_DIR = NOS_TMP_DIR / "ray"
-            RAY_TMP_DIR.mkdir(parents=True, exist_ok=True)
-            cmd = f"ray start --head --node-ip-address localhost --port={NOS_RAY_GCS_PORT} --storage {RAY_TMP_DIR} --no-monitor"
-            proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            time.sleep(wait)
-            if proc.poll() != 0:
-                # Get the process output
-                stdout, stderr = proc.communicate()
-                raise RuntimeError(f"Failed to start Ray stdout={stdout}, stderr={stderr}.")
-            status.stop()
-            console.print(f"[bold green] ✓ {self.__class__.__name__} :: Ray head started. [/bold green]")
-            return self.pid
+                status.stop()
+            except ConnectionError as exc:
+                raise RuntimeError(f"Failed to start executor: exc={exc}.")
+            console.print("[bold green] ✓ InferenceExecutor :: Backend initialized. [/bold green]")
 
-    def stop(self, wait: int = 5) -> Optional[int]:
+    def stop(self) -> None:
         """Stop Ray head."""
         console = rich.console.Console()
-        attempt, max_attempts = 0, 5
-        while attempt < max_attempts:
-            with console.status(f"[bold green] {self.__class__.__name__} :: Stopping ray head ... [/bold green]"):
-                # Check if Ray head is running
-                if not self.pid:
-                    console.print("[bold yellow] Ray head is not running.[/bold yellow]")
-                    return
-                # Stop Ray head if pid is valid
-                cmd = "ray stop -f"
-                proc = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-                time.sleep(wait)
-                if proc.poll() == 0:
-                    console.print(f"[bold green] ✓ {self.__class__.__name__} :: Ray head stopped. [/bold green]")
-                    return self.pid
-            attempt += 1
-            console.print(
-                f"[bold yellow] {self.__class__.__name__} :: Failed to stop Ray head. Retrying {attempt}/{max_attempts} after {wait}s ... [/bold yellow]"
-            )
-        raise RuntimeError("Failed to stop Ray.")
+        with console.status("[bold green] InferenceExecutor :: Backend stopping ... [/bold green]"):
+            try:
+                ray.shutdown()
+            except Exception as exc:
+                raise RuntimeError(f"Failed to stop executor: exc={exc}.")
+            console.print("[bold green] ✓ InferenceExecutor :: Backend stopped. [/bold green]")
 
     @property
     def pid(self) -> Optional[int]:
         """Get PID of Ray head."""
         for proc in psutil.process_iter(attrs=["pid", "name"]):
             if proc.name() == "raylet":
                 return proc.pid
```

## nos/hub/__init__.py

```diff
@@ -11,43 +11,75 @@
     _instance: Optional["Hub"] = None
     """Singleton instance."""
     _registry: Dict[str, ModelSpec] = {}
     """Model specifications lookup for all models registered."""
 
     @classmethod
     def get(cls: "Hub") -> "Hub":
-        """Get the singleton instance."""
+        """Get the singleton instance.
+
+        Returns:
+            Hub: Singleton instance.
+        """
         if cls._instance is None:
             cls._instance = cls()
         return cls._instance
 
     @classmethod
     def list(cls, private: bool = False) -> List[Dict[str, Any]]:
-        """List models in the registry."""
+        """List models in the registry.
+
+        Args:
+            private (bool): Whether to include private models.
+
+        Returns:
+            List[Dict[str, Any]]: List of model specifications.
+        """
         if private:
             raise NotImplementedError("Private models not supported.")
         return [v.name for v in cls.get()._registry.values()]
 
     @classmethod
     def load_spec(cls, model_name: str) -> ModelSpec:
-        """Load model spec from the registry."""
+        """Load model spec from the registry.
+
+        Args:
+            model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
+
+        Returns:
+            ModelSpec: Model specification.
+        """
         try:
             return cls.get()._registry[model_name]
         except KeyError:
             raise KeyError(f"Unavailable model (name={model_name}).")
 
     @classmethod
     def load(cls, model_name: str) -> Any:
-        """Instantiate model from the registry."""
+        """Instantiate model from the registry.
+
+        Args:
+            model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
+
+        Returns:
+            Any: Instantiated model.
+        """
         spec: ModelSpec = cls.load_spec(model_name)
         return spec.cls(*spec.args, **spec.kwargs)
 
     @classmethod
-    def register(cls, model_name: str, method: str, model_cls: Type[Any], *args, **kwargs) -> Any:
-        """Model registry decorator."""
+    def register(cls, model_name: str, method: str, model_cls: Type[Any], *args, **kwargs) -> None:
+        """Model registry decorator.
+
+        Args:
+            model_name (str): Model identifier (e.g. `openai/clip-vit-base-patch32`).
+            method (str): Method to use for prediction (one of `MethodType.TXT2VEC`, `MethodType.IMG2VEC`,
+                `MethodType.IMG2BBOX`, `MethodType.TXT2IMG`).
+            model_cls (Type[Any]): Model class.
+        """
         cls.get()._registry[model_name] = ModelSpec(
             name=model_name,
             method=MethodType[method.upper()],
             cls=model_cls,
             args=kwargs.pop("args", ()),
             kwargs=kwargs.pop("kwargs", {}),
         )
```

## nos/hub/config.py

```diff
@@ -34,29 +34,45 @@
     """Model name (e.g. bert-base-uncased)."""
     checkpoint: str = None
     """Checkpoint name (e.g. bert-base-uncased-pytorch_model.bin)."""
 
 
 @dataclass(frozen=True)
 class MMLabConfig:
+    """OpenMMlab configuration."""
+
     config: str
+    """Model configuration file."""
+
     checkpoint: str
+    """Model checkpoint file."""
 
     def validate(self):
+        """Validate the configuration."""
         if not Path(self.config).exists():
             raise IOError(f"Failed to load config={self.config}.")
         if not Path(self.checkpoint).exists():
             raise IOError(f"Failed to load checkpoint={self.checkpoint}.")
         return self
 
     @property
-    def model_name(self):
+    def model_name(self) -> str:
+        """Model name.
+
+        Returns:
+            str: Model name.
+        """
         return Path(self.config).stem
 
-    def cached_checkpoint(self):
+    def cached_checkpoint(self) -> str:
+        """Download the checkpoint and return the local path.
+
+        Returns:
+            str: Local path to the checkpoint.
+        """
         from torchvision.datasets.utils import download_url
 
         # Download the checkpoint and place it in the model directory (with the same filename)
         directory = Path(NOS_MODELS_DIR) / self.model_name
         download_url(self.checkpoint, str(directory))
         filename = directory / Path(self.checkpoint).name
```

## nos/server/docker.py

```diff
@@ -61,15 +61,15 @@
         if cls._instance is None:
             cls._instance = cls()
         return cls._instance
 
     def start(
         self,
         image: str,
-        container_name: List[str],
+        container_name: str,
         ports: Optional[Dict[int, int]] = None,
         command: Optional[List[str]] = None,
         environment: Optional[Dict[str, str]] = None,
         volumes: Optional[Dict[str, str]] = None,
         detach: bool = True,
         shm_size: str = "4g",
         **kwargs: Any,
```

## nos/server/service.py

```diff
@@ -21,16 +21,19 @@
 from nos.protoc import import_module
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
-class FixedLengthDict(OrderedDict):
-    """Fixed length dictionary."""
+class FixedLengthFIFODict(OrderedDict):
+    """Fixed length FIFO dictionary.
+
+    Note: Needs to be refactored to be more generic with FIFO/LRU options.
+    """
 
     def __init__(self, *args, **kwargs):
         self._maxlen = kwargs.pop("_maxlen", None)
         super().__init__(*args, **kwargs)
 
     def __setitem__(self, key, value):
         if len(self.keys()) >= self._maxlen:
@@ -59,20 +62,21 @@
     This service is used to serve models over gRPC.
 
     Refer to the bring-your-own-schema section:
     https://docs.ray.io/en/master/serve/direct-ingress.html?highlight=grpc#bring-your-own-schema
     """
 
     def __init__(self):
-        self.model_handle = FixedLengthDict(_maxlen=4)
+        self.model_handle = FixedLengthFIFODict(_maxlen=4)
         self.executor = RayExecutor.get()
         try:
             self.executor.init()
         except Exception as e:
-            logger.error(f"Failed to initialize executor: {e}")
+            logger.info(f"Failed to initialize executor: {e}")
+            raise RuntimeError(f"Failed to initialize executor: {e}")
 
     def init_model(self, model_name: str):
         """Initialize the model."""
         assert model_name not in self.model_handle, f"Model already initialized: {model_name}"
 
         # Load the model spec
         try:
@@ -129,14 +133,20 @@
     def DeleteModel(
         self, request: nos_service_pb2.DeleteModelRequest, context: grpc.ServicerContext
     ) -> nos_service_pb2.DeleteModelResponse:
         """Delete the model."""
         self.delete_model(request.model_name)
         return nos_service_pb2.DeleteModelResponse(result="ok")
 
+    def GetModelInfo(
+        self, request: nos_service_pb2.ModelInfoRequest, context: grpc.ServicerContext
+    ) -> nos_service_pb2.ModelInfoResponse:
+        """Get model information."""
+        raise NotImplementedError()
+
     def Predict(
         self, request: nos_service_pb2.InferenceRequest, context: grpc.ServicerContext
     ) -> nos_service_pb2.InferenceResponse:
         """Main model prediction interface."""
         logger.debug(f"Received request: {request.method}, {request.model_name}")
         if request.model_name not in self.model_handle:
             self.init_model(request.model_name)
@@ -196,15 +206,15 @@
     nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceService(), server)
     server.add_insecure_port(address)
 
     console = rich.console.Console()
     with console.status(f"[bold green] Starting server on {address}[/bold green]") as status:
         server.start()
         console.print(
-            f"[bold green] ✓ Deployment complete [/bold green]",  # noqa
+            f"[bold green] ✓ InferenceService :: Deployment complete [/bold green]",  # noqa
         )
         status.stop()
         server.wait_for_termination()
         console.print("Server stopped")
 
 
 def main():
```

## nos/test/conftest.py

```diff
@@ -1,21 +1,48 @@
+from concurrent import futures
+
+import grpc
 import pytest
 
+from nos.client import DEFAULT_GRPC_PORT, InferenceClient
 from nos.executors.ray import RayExecutor
-from nos.server.docker import DockerRuntime
+from nos.protoc import import_module
+from nos.server import InferenceService
 
 
-@pytest.fixture(scope="session")
-def docker_runtime():
-    runtime = DockerRuntime.get()
-    yield runtime
-    runtime.stop()
+GRPC_TEST_PORT = DEFAULT_GRPC_PORT + 1
+
+nos_service_pb2 = import_module("nos_service_pb2")
+nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
 @pytest.fixture(scope="session")
 def ray_executor():
     executor = RayExecutor.get()
     executor.init()
 
     yield executor
 
     executor.stop()
+
+
+@pytest.fixture(scope="session")
+def test_grpc_server():
+    from loguru import logger
+
+    logger.info(f"Starting gRPC test server on port: {GRPC_TEST_PORT}")
+    options = [
+        ("grpc.max_message_length", 512 * 1024 * 1024),
+        ("grpc.max_send_message_length", 512 * 1024 * 1024),
+        ("grpc.max_receive_message_length", 512 * 1024 * 1024),
+    ]
+    server = grpc.server(futures.ThreadPoolExecutor(max_workers=1), options=options)
+    nos_service_pb2_grpc.add_InferenceServiceServicer_to_server(InferenceService(), server)
+    server.add_insecure_port(f"[::]:{GRPC_TEST_PORT}")
+    server.start()
+    yield server
+    server.stop(grace=None)
+
+
+@pytest.fixture(scope="function")
+def test_grpc_client():
+    yield InferenceClient(f"localhost:{GRPC_TEST_PORT}")
```

## Comparing `nos/client/grpc/client.py` & `nos/client/grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-"""
-Simple gRPC client for NOS service.
-
-Used for testing purposes and in conjunction with the NOS gRPC server (grpc_server.py).
-"""
+"""gRPC client for NOS service."""
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import List, Union
 
 import cloudpickle
 import grpc
 import numpy as np
@@ -20,16 +16,25 @@
 
 
 nos_service_pb2 = import_module("nos_service_pb2")
 nos_service_pb2_grpc = import_module("nos_service_pb2_grpc")
 
 
 @contextmanager
-def InferenceSession(stub, model_name: str, num_replicas: int = 1):
-    """Remote model context manager."""
+def InferenceSession(stub: nos_service_pb2_grpc.InferenceServiceStub, model_name: str, num_replicas: int = 1):
+    """Remote model context manager.
+
+    Args:
+        stub (nos_service_pb2_grpc.InferenceServiceStub): gRPC stub.
+        model_name (str): Name of the model to init.
+        num_replicas (int): Number of replicas to init.
+
+    Yields:
+        None (NoneType): Nothing.
+    """
     # Create inference stub and init model
     request = nos_service_pb2.InitModelRequest(model_name=model_name, num_replicas=num_replicas)
     response: nos_service_pb2.InitModelResponse = stub.InitModel(request)
     logger.info(f"Init Model response: {response}")
     # Yield so that the model inference can be done
     yield
     # Delete model
@@ -42,50 +47,68 @@
 class InferenceClientState:
     """State of the client for serialization purposes."""
 
     address: str
     """Address for the gRPC server."""
 
 
-@dataclass
 class InferenceClient:
-    """Simple gRPC client for NOS service.
+    """Main gRPC client for NOS inference service.
+
+    Parameters:
+        address (str): Address for the gRPC server.
 
     Usage:
+        ```py
         # Create client
         >>> client = InferenceClient(address="localhost:50051")
 
         # List all models registered with the server
-        >>> models client.ListModels()
-        ['openai/clip-vit-base-patch32', ...]
+        # models = ['openai/clip-vit-base-patch32', ...]
+        >>> models = models client.ListModels()
 
         # Encode "Hello world!" with the CLIP text encoder
         >>> client.Predict(method=MethodType.TXT2VEC, model_name="openai/clip-vit-base-patch32", text="Hello world!")
 
         # Encode img with the CLIP visual encoder
         >>> client.Predict(method=MethodType.IMG2VEC, model_name="openai/clip-vit-base-patch32", text="Hello world!")
 
         # Predict bounding-boxes from with FastRCNN
         >>> img = Image.open("test.jpg")
         >>> client.Predict(method=MethodType.IMG2BBOX, model_name="torchvision/fasterrcnn_mobilenet_v3_large_320_fpn", img=img)
+        ```
     """
 
-    address: str = f"[::]:{DEFAULT_GRPC_PORT}"
-    """Default address for the gRPC server."""
-    _channel: grpc.Channel = None
-    """gRPC channel."""
-    _stub: nos_service_pb2_grpc.InferenceServiceStub = None
-    """gRPC stub."""
+    def __init__(self, address: str = f"[::]:{DEFAULT_GRPC_PORT}"):
+        """Initializes the gRPC client.
+
+        Args:
+            address (str): Address for the gRPC server. Defaults to f"[::]:{DEFAULT_GRPC_PORT}".
+        """
+        self.address: str = address
+        self._channel: grpc.Channel = None
+        self._stub: nos_service_pb2_grpc.InferenceServiceStub = None
 
     def __getstate__(self) -> InferenceClientState:
-        """Returns the state of the client for serialization purposes."""
+        """Returns the state of the client for serialization purposes.
+
+        Returns:
+            InferenceClientState: State of the client.
+        """
         return InferenceClientState(address=self.address)
 
     def __setstate__(self, state: InferenceClientState) -> None:
-        """Sets the state of the client for de-serialization purposes."""
+        """Sets the state of the client for de-serialization purposes.
+
+        Args:
+            state (InferenceClientState): State of the client.
+
+        Returns:
+            None (NoneType): Nothing.
+        """
         self.address = state.address
         self._channel = None
         self._stub = None
 
     @property
     def stub(self) -> nos_service_pb2_grpc.InferenceServiceStub:
         """Returns the gRPC stub.
@@ -101,22 +124,37 @@
             self._channel = grpc.insecure_channel(self.address)
             self._stub = nos_service_pb2_grpc.InferenceServiceStub(self._channel)
         assert self._channel
         assert self._stub
         return self._stub
 
     def ListModels(self) -> List[str]:
-        """List all models."""
+        """List all models.
+
+        Returns:
+            List[str]: List of model names.
+        """
         try:
             response: nos_service_pb2.ModelListResponse = self.stub.ListModels(empty_pb2.Empty())
             logger.debug(response.models)
-            return response.models
+            return list(response.models)
         except grpc.RpcError as e:
             logger.error(f"Failed to list models ({e})")
 
+    def GetModelInfo(self, model_name: str):
+        """Get the relevant model information from the model name.
+
+        Note: This may be possible only after initialization, as we need to inspect the
+        HW to understand the configurable image resolutions, batch sizes etc.
+
+        Args:
+            model_name (str): Model identifier (e.g. openai/clip-vit-base-patch32).
+        """
+        raise NotImplementedError()
+
     def Predict(
         self,
         method: str,
         model_name: str,
         img: Union[Image.Image, np.ndarray, List[Image.Image], List[np.ndarray]] = None,
         text: str = None,
     ) -> nos_service_pb2.InferenceResponse:
@@ -127,14 +165,17 @@
                 Method to use for prediction (one of MethodType.TXT2VEC, MethodType.IMG2VEC,
                 MethodType.IMG2BBOX, MethodType.TXT2IMG).
             model_name (str):
                 Model identifier (e.g. openai/clip-vit-base-patch32).
             img (Union[Image.Image, np.ndarray, List[Image.Image], List[np.ndarray]]):
                 Image or text to predict on.
             text (str): Prompt text to use for text-generation or embedding.
+
+        Returns:
+            nos_service_pb2.InferenceResponse: Inference response.
         """
         if method not in ("txt2vec", "img2vec", "img2bbox", "txt2img"):
             raise NosClientException(f"Invalid method {method}")
 
         try:
             if method in ("txt2vec", "txt2img"):
                 response = self.stub.Predict(
```

## Comparing `autonomi_nos-0.0.2.dist-info/LICENSE` & `autonomi_nos-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `autonomi_nos-0.0.2.dist-info/RECORD` & `autonomi_nos-0.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 nos/__init__.py,sha256=ON7r9-nhUByFaRhC-pr-NcTHa2zdd4fuJUsWwTVQiB0,119
 nos/constants.py,sha256=j-nz48q31rE7eclMqkZH6xFJ0eGmtx2Jt5yr_wQA_1Y,561
 nos/exceptions.py,sha256=ocRCxTbzT_Q8WTobAbkbo4jl5a6F3xC_D2N7rtzfWeg,93
 nos/logging.py,sha256=D0QDNFGmAYshfnSC-ctEDSIeBO6TnLPz1babUmJGRSA,940
-nos/protoc.py,sha256=zC26J8H6ojuSSU8bpcScNSCenpmsAwTKBaK0ZjmZwIU,2716
-nos/version.py,sha256=QvlVh4JTl3JL7jQAja76yKtT-IvF4631ASjWY1wS6AQ,22
+nos/protoc.py,sha256=xUck1U30UqUEnTaFuWMGWagyDcIrjmcQo8xozqbypmI,2778
+nos/version.py,sha256=4GZKi13lDTD25YBkGakhZyEQZWTER_OWQMNPoH_UM2c,22
 nos/cli/benchmark.py,sha256=p-EGzEUDMFFv2hpB9Nn8-Xk1zW-hrYDaUzyNvWmSgzk,110
 nos/cli/cli.py,sha256=nO0Eg_zp7L6xt5ST0QteypNHky8TIms8JSOLsvtHhjY,455
 nos/cli/docker.py,sha256=uPGrLe8FlvwSNFGUqp-vw5VAZhCeyvrfUfwJZdqXypk,1983
 nos/cli/hub.py,sha256=USdzVgaZlPZABrrIZzCA7ySwXg1iseEk7GJ7iwanXIg,1294
-nos/cli/serve_grpc.py,sha256=3n-4M-FSlQuSMMUJb5g1URLUD8m8L_JCdJI77DjeQlw,6244
+nos/cli/serve_grpc.py,sha256=XUxyCcyLkRg9psbhcydCq45V7WgOG7oUH-vF9EEipGE,6094
 nos/cli/serve_http.py,sha256=xMwSE46-_uHLgif1gnJCRoLbBE3ttC2zkm2JXVooWg0,5962
 nos/cli/system.py,sha256=gFm8ngxyxcPThhjkgB8S8ZBmtYBcqLdSo4unaWTl0N8,3479
 nos/cli/utils.py,sha256=uR1lGZyyDEuflNvxKuAmVUP-DTE55PzZL5c0c3l2h4U,425
-nos/client/__init__.py,sha256=XWZl4NSAfDiKPjgDn2L0ohBzBAz93AuFD3Dwcb1yxK8,148
+nos/client/__init__.py,sha256=u-xpiMdEMYNPzarLAbjDx2KlLCq4XaqpkhqzcMdKTcU,141
 nos/client/exceptions.py,sha256=Lqqeu_6oNSZgOUipXHFx20yeASJi9bEewpG1UYuy1gk,92
-nos/client/grpc/client.py,sha256=UAVfrnluIbeYUZl6EW9Yd3RmZK5ke76pC74UpjCUtS8,6048
-nos/executors/ray.py,sha256=BaRnMjZqyWsEpc-Ov7JVxOUp3r-ZNVgSAzYz7_k8ZE8,7153
-nos/hub/__init__.py,sha256=5UDQXTn5ZP-jlfofNBDod490PFklhsmvc95E1coUQjM,2087
-nos/hub/config.py,sha256=BTGPITkECUfLBd7w0NXiG94VuzvWmd4t_mYMmfRGn7o,1812
+nos/client/grpc.py,sha256=3A-3vpk4FFx3kUi9aGzJP_Mn_sAbPQkaM6yRgbtDK3g,7307
+nos/executors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+nos/executors/ray.py,sha256=wxbKvIMinQODTVm0zUlKpCcmj9TkGxNpmlAL3k7vvoE,6237
+nos/hub/__init__.py,sha256=1gZVEGB5dD-QfDTKB1hGiYMBDEa5kmbfiYOcOUYd4hM,2985
+nos/hub/config.py,sha256=DK0t6xrB6Sgf71YWnX_htNbbU4H2Bcdu9b7ujiA6QKY,2195
 nos/hub/spec.py,sha256=vC6DDYo0F1PVX9EYGMdnhFDKH7emRBX-Z0JJm54Slwc,902
 nos/models/__init__.py,sha256=FMoBv4glDtKz1eCIvqOy0RDqWM6w0fP7fdT_NJR8Q3k,242
 nos/models/clip.py,sha256=TVeCvHOe-1KfQI0e7CZu0SLIGQusMEI6EM7Z9IgVDDg,2370
 nos/models/faster_rcnn.py,sha256=Wnjdq-B5qZqqgMu3PzHCR2ga8LPGKR5FqaaQYs5MCJw,2028
 nos/models/stable_diffusion.py,sha256=pDc_3PJr7k5rOJuelcGD7i5zCcurQ02lkpfc0TaaUqw,2651
 nos/models/openmmlab/mmdetection/detection_tensorrt_dynamic-320x320-1344x1344.py,sha256=YFx2dzUKL2MkS5mIqw6gDO1TxLkwLIWEFVOxwHIhnYg,66
 nos/models/openmmlab/mmdetection/mmdetection.py,sha256=BFyy-H6EwP3ZvuOgpiEmmn8R0p-sSOdfBIDHMY6Kbms,2589
 nos/models/openmmlab/mmdetection/configs/_base_/default_runtime.py,sha256=tAbybUUg9TtBy_dqiXD5Zgl0kSs39JX7TiTeIYZrOUo,370
 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_detection.py,sha256=MxNi_Sf1m8CNkR64vZWaFN2O2P2LBI1-EexpLr166YU,3187
 nos/models/openmmlab/mmdetection/configs/_base_/datasets/coco_instance.py,sha256=DVkj2zskGrXxiF6hVQ1ofsOsqQGHsdjAh5sXRkaxjiw,1765
 nos/models/openmmlab/mmdetection/configs/_base_/models/faster-rcnn_r50_fpn.py,sha256=Al2qpY2P-MzsfBCod5pjB6HrH7ZzFvQxICc1CVmpnRY,3828
 nos/models/openmmlab/mmdetection/configs/_base_/schedules/schedule_1x.py,sha256=G8gXisLhM7mBRlxrhTOLCsWD17zCyH7kBvVi7J4BICI,304
 nos/models/openmmlab/mmdetection/configs/efficientdet/efficientdet_effb3_bifpn_8xb16-crop896-300e_coco.py,sha256=RSkd9o1IO-YkWhIwnXU83tRyGeySiR1IMlSk14dTw9s,5340
 nos/models/openmmlab/mmdetection/configs/faster-rcnn/faster-rcnn_r50_fpn_1x_coco.py,sha256=Cm8lyQ3wOT5I9KR0m1TfTsPAGybs-buILRPLDZKzOPQ,177
+nos/proto/nos_service.proto,sha256=akx6q6f7aYjsIvwINPZR93SBjncHapG__ibQHYgwyTA,1409
 nos/server/__init__.py,sha256=kdNIS7NMSFz_ooJC3ZXzTjjS2VHb0me5SiPPFSrOu4U,156
-nos/server/docker.py,sha256=5wb0XGZuLewa3qDQb18IcZAk67zCWz4m-eCyowSUNXc,6235
+nos/server/docker.py,sha256=Wbob_pkHXKdMWliD2VTWw1U7R7dojBImYWZTeSNDfLY,6229
 nos/server/runtime.py,sha256=nW2oAYfySqxVcH7B1Np0JZHqkqKFG6SjtMdtfEZOVbo,3004
-nos/server/service.py,sha256=Fc0NjzP6KtH9vvvtGnkQltRBS29X8Lo1f_7ONGl_Elg,8470
+nos/server/service.py,sha256=GweoeaDgHY8RLIMSa8HrpqIjdbGJfnRDolEU815slfQ,8880
 nos/test/benchmark.py,sha256=b_QMHfStY5iRjHGPZwaY7VrXzy_VeFKfjld9UEVbn-g,373
-nos/test/conftest.py,sha256=7Nbz2zvNdZyzhGN4FEQNqurIOz02DfVJxXp2g0C5FBY,378
+nos/test/conftest.py,sha256=psIsMxzB9g8jgUokP_q6sJ-SZuTYTZSxBtfyYb0hSc8,1317
 nos/test/utils.py,sha256=qZbEN85EhUNBF3BAUTW_dStMCsPwrdosSRlkQp-ShX0,1324
-autonomi_nos-0.0.2.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
-autonomi_nos-0.0.2.dist-info/METADATA,sha256=1jVZmGdhTy_bujudlMwa4cSOs89wfN3azTwLThGsA2A,6038
-autonomi_nos-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-autonomi_nos-0.0.2.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
-autonomi_nos-0.0.2.dist-info/top_level.txt,sha256=Tgqk49XI1nXvi6W_Ryy7_YwQ7iFU-mAlIsbNMR1HS6s,4
-autonomi_nos-0.0.2.dist-info/RECORD,,
+autonomi_nos-0.0.3.dist-info/LICENSE,sha256=9TQFxQ2AkXOQuIHy9GueB_a18hayRXT7pDt9fJv9WLo,1068
+autonomi_nos-0.0.3.dist-info/METADATA,sha256=a12iqcMfV1vlmTUyyKgPndkj_GXdn0ScgN-GwRMrUu4,5917
+autonomi_nos-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+autonomi_nos-0.0.3.dist-info/entry_points.txt,sha256=UYtJAmFT3RPWmlKM11MMZvZPRHTeKyIh1BbZ3QpbsJs,86
+autonomi_nos-0.0.3.dist-info/top_level.txt,sha256=Tgqk49XI1nXvi6W_Ryy7_YwQ7iFU-mAlIsbNMR1HS6s,4
+autonomi_nos-0.0.3.dist-info/RECORD,,
```

