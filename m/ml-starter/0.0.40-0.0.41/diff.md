# Comparing `tmp/ml-starter-0.0.40.tar.gz` & `tmp/ml-starter-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.40.tar", last modified: Sun May 14 11:20:28 2023, max compression
+gzip compressed data, was "ml-starter-0.0.41.tar", last modified: Sat May 20 07:38:31 2023, max compression
```

## Comparing `ml-starter-0.0.40.tar` & `ml-starter-0.0.41.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 11:20:16.000000 ml-starter-0.0.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-14 11:20:16.000000 ml-starter-0.0.40/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 11:20:28.961558 ml-starter-0.0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-14 11:20:16.000000 ml-starter-0.0.40/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.945558 ml-starter-0.0.40/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.949558 ml-starter-0.0.40/ml/models/pretrained/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41249 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/hubert.py
--rw-r--r--   0 runner    (1001) docker     (123)    22211 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)    60772 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/models/pretrained/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.953559 ml-starter-0.0.40/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.957558 ml-starter-0.0.40/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-14 11:20:16.000000 ml-starter-0.0.40/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 11:20:28.961558 ml-starter-0.0.40/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-14 11:20:28.000000 ml-starter-0.0.40/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-14 11:20:16.000000 ml-starter-0.0.40/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 11:20:16.000000 ml-starter-0.0.40/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 11:20:28.961558 ml-starter-0.0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-14 11:20:16.000000 ml-starter-0.0.40/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.974888 ml-starter-0.0.41/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-20 07:38:18.000000 ml-starter-0.0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-20 07:38:18.000000 ml-starter-0.0.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-20 07:38:31.974888 ml-starter-0.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-20 07:38:18.000000 ml-starter-0.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.942887 ml-starter-0.0.41/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.942887 ml-starter-0.0.41/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25200 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.946887 ml-starter-0.0.41/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10045 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44643 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.950887 ml-starter-0.0.41/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25205 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/models/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26671 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22197 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60788 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/models/pretrained/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.954887 ml-starter-0.0.41/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.958887 ml-starter-0.0.41/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18535 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.962887 ml-starter-0.0.41/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.966888 ml-starter-0.0.41/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9190 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.970888 ml-starter-0.0.41/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.970888 ml-starter-0.0.41/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-05-20 07:38:18.000000 ml-starter-0.0.41/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 07:38:31.974888 ml-starter-0.0.41/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-20 07:38:31.000000 ml-starter-0.0.41/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-20 07:38:18.000000 ml-starter-0.0.41/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 07:38:18.000000 ml-starter-0.0.41/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 07:38:31.974888 ml-starter-0.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-20 07:38:18.000000 ml-starter-0.0.41/setup.py
```

### Comparing `ml-starter-0.0.40/LICENSE` & `ml-starter-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/PKG-INFO` & `ml-starter-0.0.41/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.40
+Version: 0.0.41
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.40/README.md` & `ml-starter-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/api.py` & `ml-starter-0.0.41/ml/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,21 +113,25 @@
     "Output",
     "pad_all",
     "pad_sequence",
     "parallel_group_info",
     "ParallelEmbedding",
     "parallelism_is_initialized",
     "Phase",
+    "pretrained_blip",
     "pretrained_clip",
     "pretrained_hubert",
     "pretrained_llama",
+    "pretrained_rwkv",
     "pretrained_sam",
+    "PretrainedBlipKey",
     "PretrainedClipSize",
     "PretrainedHubertSize",
     "PretrainedLlamaKey",
+    "PretrainedRwkvKey",
     "PretrainedSamSize",
     "project_dir_paths",
     "read_gif",
     "read_video",
     "reduce",
     "register_logger",
     "register_lr_scheduler",
@@ -206,17 +210,19 @@
     cast_embedding_kind,
     get_positional_embeddings,
 )
 from ml.models.init import InitializationType, cast_init_type, init_
 from ml.models.lora import LoraConv1d, LoraConv2d, LoraEmbedding, LoraLinear, lora
 from ml.models.norms import NormType, cast_norm_type, get_norm_1d, get_norm_2d, get_norm_3d, get_norm_linear
 from ml.models.parallel import ColumnParallelLinear, ParallelEmbedding, RowParallelLinear
+from ml.models.pretrained.blip import PretrainedBlipKey, pretrained_blip
 from ml.models.pretrained.clip import PretrainedClipSize, pretrained_clip
 from ml.models.pretrained.hubert import PretrainedHubertSize, pretrained_hubert
 from ml.models.pretrained.llama import PretrainedLlamaKey, pretrained_llama
+from ml.models.pretrained.rwkv import PretrainedRwkvKey, pretrained_rwkv
 from ml.models.pretrained.sam import PretrainedSamSize, pretrained_sam
 from ml.optimizers.base import BaseOptimizer, BaseOptimizerConfig
 from ml.tasks.base import BaseTask, BaseTaskConfig
 from ml.tasks.datasets import transforms
 from ml.tasks.datasets.async_iterable import AsyncIterableDataset
 from ml.tasks.datasets.clippify import ClippifyDataset
 from ml.tasks.datasets.collate import CollateMode, collate, collate_non_null, pad_all, pad_sequence
```

### Comparing `ml-starter-0.0.40/ml/core/common_types.py` & `ml-starter-0.0.41/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/core/config.py` & `ml-starter-0.0.41/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/core/env.py` & `ml-starter-0.0.41/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/core/registry.py` & `ml-starter-0.0.41/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/core/state.py` & `ml-starter-0.0.41/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/launchers/base.py` & `ml-starter-0.0.41/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/launchers/mp.py` & `ml-starter-0.0.41/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/launchers/slurm.py` & `ml-starter-0.0.41/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/launchers/torchrun.py` & `ml-starter-0.0.41/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/loggers/base.py` & `ml-starter-0.0.41/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/loggers/meter.py` & `ml-starter-0.0.41/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/loggers/multi.py` & `ml-starter-0.0.41/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/loggers/stdout.py` & `ml-starter-0.0.41/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/loggers/tensorboard.py` & `ml-starter-0.0.41/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/base.py` & `ml-starter-0.0.41/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/constant.py` & `ml-starter-0.0.41/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.41/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.41/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/linear.py` & `ml-starter-0.0.41/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.41/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.41/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/activations.py` & `ml-starter-0.0.41/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/base.py` & `ml-starter-0.0.41/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/embeddings.py` & `ml-starter-0.0.41/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/init.py` & `ml-starter-0.0.41/ml/models/init.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     "normal",
     "biased_normal",
     "uniform",
     "kaiming_uniform",
     "kaiming_normal",
     "xavier_uniform",
     "xavier_normal",
+    "trunc_normal",
+    "dirac",
+    "constant",
     "zeros",
     "ones",
 ]
 
 
 def cast_init_type(s: str) -> InitializationType:
     args = get_args(InitializationType)
@@ -57,32 +60,42 @@
         nn.init.zeros_(bias)
     else:
         bound = 1 / math.sqrt(fan_in)
         nn.init.uniform_(bias, -bound, bound)
     return bias
 
 
+def _zeros(t: Tensor | None) -> Tensor | None:
+    return None if t is None else nn.init.zeros_(t)
+
+
 def init_(
     weight: Tensor,
     bias: Tensor | None,
     init: InitializationType,
     *,
-    normal_std: float = 0.01,
-    uniform_scale: float = 0.02,
+    mean: float = 0.0,
+    std: float = 0.01,
+    scale: float = 0.02,
+    groups: int = 1,
+    trunc_clip: tuple[float, float] = (-2.0, 2.0),
 ) -> tuple[Tensor, Tensor | None]:
     """Initializes the weight and bias in-place, using an initialization key.
 
     The weight and bias are from a convolution or linear layer.
 
     Args:
         weight: The weight tensor
         bias: The bias tensor
         init: The initialization type to use
-        normal_std: The standard deviation for normal initialization
-        uniform_scale: The scale amount for uniform initialization
+        mean: The mean for normal initialization
+        std: The standard deviation for normal initialization
+        scale: The scale amount for uniform or constant initialization
+        groups: The number of groups, if argument is necessary
+        trunc_clip: The min and max values for trunc_normal initialization
 
     Returns:
         The initialized weight and bias (which can be discarded, since the
         initialization happens in-place).
 
     Raises:
         NotImplementedError: If the initialization mode isn't implemented
@@ -92,36 +105,43 @@
         return weight, bias
     if isinstance(weight, nn.Parameter):
         weight = weight.data
     if isinstance(bias, nn.Parameter):
         bias = bias.data
     match init:
         case "orthogonal":
-            if weight.dtype == torch.float16:
+            if weight.dtype in (torch.float16, torch.bfloat16):
                 return (
                     weight.copy_(nn.init.orthogonal_(weight.float(), gain=0.01).to(weight)),
-                    None if bias is None else nn.init.zeros_(bias),
+                    _zeros(bias),
                 )
-            return nn.init.orthogonal_(weight), None if bias is None else nn.init.zeros_(bias)
+            return nn.init.orthogonal_(weight), _zeros(bias)
         case "normal":
-            return nn.init.normal_(weight, std=normal_std), None if bias is None else nn.init.zeros_(bias)
+            return nn.init.normal_(weight, mean=mean, std=std), _zeros(bias)
         case "biased_normal":
             return (
-                nn.init.normal_(weight, std=normal_std),
-                None if bias is None else nn.init.normal_(bias, std=normal_std),
+                nn.init.normal_(weight, mean=mean, std=std),
+                None if bias is None else nn.init.normal_(bias, mean=mean, std=std),
             )
         case "uniform":
-            return nn.init.uniform_(weight, b=uniform_scale), None if bias is None else nn.init.zeros_(bias)
+            return nn.init.uniform_(weight, b=scale), _zeros(bias)
         case "kaiming_uniform":
             return nn.init.kaiming_uniform_(weight), _uniform_bias(weight, bias)
         case "kaiming_normal":
             return nn.init.kaiming_normal_(weight), _uniform_bias(weight, bias)
         case "xavier_uniform":
             return nn.init.xavier_uniform_(weight), _uniform_bias(weight, bias)
         case "xavier_normal":
             return nn.init.xavier_normal_(weight), _uniform_bias(weight, bias)
+        case "trunc_normal":
+            a, b = trunc_clip
+            return nn.init.trunc_normal_(weight, mean=mean, std=std, a=a, b=b), _zeros(bias)
+        case "dirac":
+            return nn.init.dirac_(weight, groups=groups), _zeros(bias)
+        case "constant":
+            return nn.init.constant_(weight, scale), _zeros(bias)
         case "zeros":
-            return nn.init.zeros_(weight), None if bias is None else nn.init.zeros_(bias)
+            return nn.init.zeros_(weight), _zeros(bias)
         case "ones":
-            return nn.init.ones_(weight), None if bias is None else nn.init.zeros_(bias)
+            return nn.init.ones_(weight), _zeros(bias)
         case _:
             raise NotImplementedError(f"Unexpected initialization: {init}")
```

### Comparing `ml-starter-0.0.40/ml/models/lora.py` & `ml-starter-0.0.41/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/norms.py` & `ml-starter-0.0.41/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/parallel.py` & `ml-starter-0.0.41/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/models/pretrained/clip.py` & `ml-starter-0.0.41/ml/models/pretrained/clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+# mypy: disable-error-code="import"
 """Defines a simple API for using OpenAI's pretrained CLIP model.
 
 .. highlight:: python
 .. code-block:: python
 
     from ml.models.pretrained.clip import pretrained_clip
 
     full_model = pretrained_clip("RN50", mode="all")
     visual_model = pretrained_clip("RN50", mode="visual")
     linguistic_model = pretrained_clip("RN50", mode="linguistic")
 
-    image = PIL.Image.open(url_path)
+    image = PIL.Image.open(image_path)
     image_tensorizer = visual_model.get_preprocess()
     image_tensor = image_tensorizer(image)  # (3, 224, 224)
 
     tokenizer = linguistic_model.get_tokenizer()
     token_tensor = tokenizer.tokenizer(["A photo of a cat", "A photo of a dog"])
 
     visual_model.encode_image(imgs)  # (N, C)
@@ -164,15 +165,15 @@
         prev_char = char
     return pairs
 
 
 @functools.lru_cache()
 def test_clean_func(lower: bool = True) -> Callable[[str], str]:
     try:
-        import ftfy  # type: ignore[import]
+        import ftfy
 
     except ImportError:
         logger.warning("Please install ftfy: pip install ftfy")
         ftfy = None
 
     def _clean(text: str) -> str:
         if ftfy is not None:
@@ -1065,19 +1066,19 @@
     parser.add_argument("key", type=str, choices=get_args(PretrainedClipSize))
     args = parser.parse_args()
 
     configure_logging()
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
-    url_path = Path("/tmp/peach.jpg")
-    if not url_path.exists():
-        download_url(peach_url, "/tmp", filename="peach.jpg")
+    img_path = Path("/tmp/peach.jpg")
+    if not img_path.exists():
+        download_url(peach_url, str(img_path.parent), filename=img_path.name)
 
-    peach_img = PIL.Image.open(url_path)
+    peach_img = PIL.Image.open(img_path)
     pos_desc = "A picture of an Autumn Red peach"
     neg_desc = "An Instagram photo of a cute puppy"
 
     # Loads the JIT'd model and the regular model.
     auto_device = AutoDevice.detect_device()
     jit_model = cast(Clip, torch.jit.load(get_pretrained_path(cast(PretrainedClipSize, args.key)), map_location="cpu"))
     model = pretrained_clip(jit_model, "all")
```

### Comparing `ml-starter-0.0.40/ml/models/pretrained/llama.py` & `ml-starter-0.0.41/ml/models/pretrained/llama.py`

 * *Files 0% similar despite different names*

```diff
@@ -532,15 +532,15 @@
     # Logs model summary.
     total_params = sum(p.numel() for p in model.parameters())
     logger.info("Model %s has %s parameters", key, f"{total_params:,}")
 
     # Build the transformer and loads the checkpoint.
     with Timer("loading state dict", spinner=True):
         model._apply(meta_to_empty_func(torch.device("cuda"), torch.half))
-        model.load_state_dict(checkpoint, strict=False)
+        model.load_state_dict(checkpoint)
 
     return model
 
 
 def worker(
     key: PretrainedLlamaKey,
     prompt: str,
```

### Comparing `ml-starter-0.0.40/ml/models/pretrained/sam.py` & `ml-starter-0.0.41/ml/models/pretrained/sam.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 .. code-block:: python
 
     from ml.models.pretrained.sam import pretrained_sam
 
     model = pretrained_sam("ViT-B")
     predictor = model.predictor()
 
-    image = PIL.Image.open(url_path)
+    image = PIL.Image.open(img_path)
     predictor.set_image(np.array(image))
 
     predictions, _, _ = predictor.predict()
     single_mask = predictions[0]  # Same shape as the original image.
 
 The choices for the model key are:
 
@@ -1560,22 +1560,22 @@
     parser.add_argument("key", type=str, choices=get_args(PretrainedSamSize))
     args = parser.parse_args()
 
     configure_logging()
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
-    url_path = Path("/tmp/peach.jpg")
-    if not url_path.exists():
-        download_url(peach_url, "/tmp", filename="peach.jpg")
+    img_path = Path("/tmp/peach.jpg")
+    if not img_path.exists():
+        download_url(peach_url, str(img_path.parent), filename=img_path.name)
 
     model = pretrained_sam(cast(PretrainedSamSize, args.key))
     predictor = model.predictor()
 
-    peach_img = PIL.Image.open(url_path)
+    peach_img = PIL.Image.open(img_path)
     predictor.set_image(np.array(peach_img))
 
     predictions, _, _ = predictor.predict()
     single_mask = predictions[0]
     mask = PIL.Image.fromarray(single_mask.astype(np.uint8) * 255)
 
     # Overlays the mask on the original image.
```

### Comparing `ml-starter-0.0.40/ml/optimizers/adam.py` & `ml-starter-0.0.41/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/optimizers/adamw.py` & `ml-starter-0.0.41/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/optimizers/adan.py` & `ml-starter-0.0.41/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/optimizers/base.py` & `ml-starter-0.0.41/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/optimizers/sgd.py` & `ml-starter-0.0.41/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/optimizers/shampoo.py` & `ml-starter-0.0.41/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/scripts/cli.py` & `ml-starter-0.0.41/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/scripts/stage.py` & `ml-starter-0.0.41/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/scripts/train.py` & `ml-starter-0.0.41/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/base.py` & `ml-starter-0.0.41/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.41/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.41/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/collate.py` & `ml-starter-0.0.41/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.41/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.41/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.41/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.41/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.41/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/utils.py` & `ml-starter-0.0.41/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.41/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/environments/base.py` & `ml-starter-0.0.41/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/environments/utils.py` & `ml-starter-0.0.41/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/environments/worker.py` & `ml-starter-0.0.41/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/losses/reduce.py` & `ml-starter-0.0.41/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/rl/base.py` & `ml-starter-0.0.41/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/rl/replay.py` & `ml-starter-0.0.41/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/tasks/sl/base.py` & `ml-starter-0.0.41/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/base.py` & `ml-starter-0.0.41/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/compile.py` & `ml-starter-0.0.41/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.41/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.0.41/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.41/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.41/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.41/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.41/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.41/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.41/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.41/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/rl.py` & `ml-starter-0.0.41/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/sl.py` & `ml-starter-0.0.41/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/trainers/vanilla.py` & `ml-starter-0.0.41/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/argparse.py` & `ml-starter-0.0.41/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/atomic.py` & `ml-starter-0.0.41/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/augmentation.py` & `ml-starter-0.0.41/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/caching.py` & `ml-starter-0.0.41/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/checkpoint.py` & `ml-starter-0.0.41/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/cli.py` & `ml-starter-0.0.41/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/colors.py` & `ml-starter-0.0.41/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/config.py` & `ml-starter-0.0.41/ml/utils/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/data.py` & `ml-starter-0.0.41/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/datetime.py` & `ml-starter-0.0.41/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/device/auto.py` & `ml-starter-0.0.41/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/device/base.py` & `ml-starter-0.0.41/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/device/cpu.py` & `ml-starter-0.0.41/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/device/gpu.py` & `ml-starter-0.0.41/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/device/metal.py` & `ml-starter-0.0.41/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/distributed.py` & `ml-starter-0.0.41/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/image.py` & `ml-starter-0.0.41/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/large_models.py` & `ml-starter-0.0.41/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/logging.py` & `ml-starter-0.0.41/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/meter.py` & `ml-starter-0.0.41/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/parallel.py` & `ml-starter-0.0.41/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/staging.py` & `ml-starter-0.0.41/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/timer.py` & `ml-starter-0.0.41/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/torch_distributed.py` & `ml-starter-0.0.41/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml/utils/video.py` & `ml-starter-0.0.41/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.41/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.40
+Version: 0.0.41
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.40/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.41/ml_starter.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,19 @@
 ml/models/base.py
 ml/models/embeddings.py
 ml/models/init.py
 ml/models/lora.py
 ml/models/norms.py
 ml/models/parallel.py
 ml/models/pretrained/__init__.py
+ml/models/pretrained/blip.py
 ml/models/pretrained/clip.py
 ml/models/pretrained/hubert.py
 ml/models/pretrained/llama.py
+ml/models/pretrained/rwkv.py
 ml/models/pretrained/sam.py
 ml/optimizers/__init__.py
 ml/optimizers/adam.py
 ml/optimizers/adamw.py
 ml/optimizers/adan.py
 ml/optimizers/base.py
 ml/optimizers/sgd.py
```

### Comparing `ml-starter-0.0.40/pyproject.toml` & `ml-starter-0.0.41/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.40/setup.py` & `ml-starter-0.0.41/setup.py`

 * *Files identical despite different names*

