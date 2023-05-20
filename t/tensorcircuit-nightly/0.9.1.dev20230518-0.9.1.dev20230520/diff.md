# Comparing `tmp/tensorcircuit-nightly-0.9.1.dev20230518.tar.gz` & `tmp/tensorcircuit-nightly-0.9.1.dev20230520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230518.tar", last modified: Thu May 18 12:41:11 2023, max compression
+gzip compressed data, was "tensorcircuit-nightly-0.9.1.dev20230520.tar", last modified: Sat May 20 12:48:01 2023, max compression
```

## Comparing `tensorcircuit-nightly-0.9.1.dev20230518.tar` & `tensorcircuit-nightly-0.9.1.dev20230520.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/
--rw-r--r--   0 runner    (1001) docker     (122)    25020 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    18675 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/README_cn.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.021173 tensorcircuit-nightly-0.9.1.dev20230518/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.025173 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/advance.rst
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/cnconf.py
--rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/contribution.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/generate_rst.py
--rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/infras.rst
--rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst.backup
--rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/sharpbits.rst
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/textbooktoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc.rst
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc_cn.rst
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-18 12:41:04.000000 tensorcircuit-nightly-0.9.1.dev20230518/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.029173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-18 12:41:04.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2901 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/about.py
--rw-r--r--   0 runner    (1001) docker     (122)    42135 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.029173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/dqas.py
--rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vags.py
--rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/van.py
--rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vqes.py
--rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/asciiart.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    31112 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/basecircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/apis.py
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/local.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)    14222 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/simple_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cons.py
--rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/densitymatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/gates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/keras.py
--rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mps_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    34350 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/quantum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.033173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/counts.py
--rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/simplify.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.037173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/blocks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/chems.py
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/graphs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/measurements.py
--rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/translation.py
--rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.037173 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-18 12:41:10.000000 tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-18 12:41:11.041173 tensorcircuit-nightly-0.9.1.dev20230518/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_calibrating.py
--rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (122)    47235 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_cloud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_dmcircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_miscs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_mpscircuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_noisemodel.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_qaoa.py
--rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum_attr.py
--rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_torchnn.py
--rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-18 12:16:18.000000 tensorcircuit-nightly-0.9.1.dev20230518/tests/test_van.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.981461 tensorcircuit-nightly-0.9.1.dev20230520/
+-rw-r--r--   0 runner    (1001) docker     (122)    25154 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-20 12:48:01.981461 tensorcircuit-nightly-0.9.1.dev20230520/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18675 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6097 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/README_cn.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.957461 tensorcircuit-nightly-0.9.1.dev20230520/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.961461 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     6332 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/advance.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/cnconf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/contribution.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10971 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/generate_rst.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3326 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10071 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/infras.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      680 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4334 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/modules.rst.backup
+-rw-r--r--   0 runner    (1001) docker     (122)    27533 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/sharpbits.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/textbooktoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/tutorial_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/whitepapertoc.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/docs/source/whitepapertoc_cn.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-20 12:48:01.981461 tensorcircuit-nightly-0.9.1.dev20230520/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-20 12:47:53.000000 tensorcircuit-nightly-0.9.1.dev20230520/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.965461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-20 12:47:52.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/about.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42135 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.965461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34460 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15348 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18124 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14032 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36391 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/vags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15117 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/van.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23416 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8235 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/asciiart.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.969462 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57621 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1713 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14928 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24925 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4024 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24148 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3825 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35980 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34020 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/basecircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28637 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36220 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.969462 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14582 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17866 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2252 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14222 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3622 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10737 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.973461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6032 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9595 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29573 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cons.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13806 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29016 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/gates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.973461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10364 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5117 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10126 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15270 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/mps_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11861 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82850 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/quantum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.973461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       89 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31362 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9413 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/simplify.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.973461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6158 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/chems.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5811 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10942 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4621 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27335 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7060 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12195 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.977461 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21081 2023-05-20 12:48:01.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3561 2023-05-20 12:48:01.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-20 12:48:01.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-05-20 12:48:01.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-20 12:48:01.000000 tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-20 12:48:01.981461 tensorcircuit-nightly-0.9.1.dev20230520/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33735 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3805 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_calibrating.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11237 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47235 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5445 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17232 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_dmcircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13220 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6639 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_miscs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10552 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_mpscircuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5637 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_noisemodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16823 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_quantum_attr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11050 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2823 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_torchnn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3163 2023-05-20 12:14:59.000000 tensorcircuit-nightly-0.9.1.dev20230520/tests/test_van.py
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/CHANGELOG.md` & `tensorcircuit-nightly-0.9.1.dev20230520/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 
 ### Added
 
 - `c.measure_instruction(*qubits)` now supports multiple ints specified at the same time
 
 - `c.expectation_ps()` now also supports `ps` argument directly (pauli structures)
 
+- Add tc version print in `tc.about()` method
+
 ### Fixed
 
 - `tc.results.counts.plot_histogram` now can dispatch kws to corresponding qiskit method
 
 - New implementation for `c.inverse()` to partially avoid unrecognized gate name issue
 
 - Fixed bug for `batch_expectation_ps` for jax backend
 
+- Partially fix the SVD numerical stability bug on tf backend when using `MPSCircuit`
+
 ## 0.9.1
 
 ### Added
 
 - Add `tc.TorchHardwarLayer` for shortcut layer construction of quantum hardware experiments
 
 - Add cotengra contractor setup shortcut
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/HISTORY.md` & `tensorcircuit-nightly-0.9.1.dev20230520/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/LICENSE` & `tensorcircuit-nightly-0.9.1.dev20230520/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230520/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230518
+Version: 0.9.1.dev20230520
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/README.md` & `tensorcircuit-nightly-0.9.1.dev20230520/README.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/README_cn.md` & `tensorcircuit-nightly-0.9.1.dev20230520/README_cn.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/advance.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/cnconf.py` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/conf.py` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/contribution.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/faq.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/generate_rst.py` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/index.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/infras.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/infras.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/modules.rst.backup` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/quickstart.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/sharpbits.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/tutorial_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-nightly-0.9.1.dev20230520/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/setup.py` & `tensorcircuit-nightly-0.9.1.dev20230520/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.1.dev20230518"
+__version__ = "0.9.1.dev20230520"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/about.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/about.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,20 @@
         import tensornetwork as tn
 
         print(f"TensorNetwork version: {tn.__version__}")
     except ModuleNotFoundError:
         print(f"TensorNetwork is not installed")
 
     try:
-        import cotengra as _
+        import cotengra
 
-        print(f"Cotengra: installed")
+        try:
+            print(f"Cotengra version: {cotengra.__version__}")
+        except AttributeError:
+            print(f"Cotengra: installed")
     except ModuleNotFoundError:
         print(f"Cotengra is not installed")
 
     try:
         import tensorflow as tf
 
         print(f"TensorFlow version: {tf.__version__}")
@@ -103,10 +106,14 @@
     try:
         import cirq
 
         print(f"Cirq version: {cirq.__version__}")
     except ModuleNotFoundError:
         print(f"Cirq is not installed")
 
+    from tensorcircuit import __version__
+
+    print(f"TensorCircuit version {__version__}")
+
 
 if __name__ == "__main__":
     about()
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/abstractcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/dqas.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/graphdata.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/layers.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vags.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/van.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/applications/vqes.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/applications/vqes.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/asciiart.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/jax_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/tensorflow_backend.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Backend magic inherited from tensornetwork: tensorflow backend
 """
 # pylint: disable=invalid-name
 
+import os
 from functools import reduce, partial
 from operator import mul
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 from scipy.sparse import coo_matrix
 import tensornetwork
 from tensornetwork.backends.tensorflow import tensorflow_backend
@@ -221,14 +222,128 @@
     )  # M=r*q at this point
     center_dim = tf.shape(r)[1]
     r = tf.reshape(r, tf.concat([left_dims, [center_dim]], axis=-1))
     q = tf.reshape(q, tf.concat([[center_dim], right_dims], axis=-1))
     return r, q
 
 
+def _svd_tf(
+    self: Any,
+    tensor: Tensor,
+    pivot_axis: int = -1,
+    max_singular_values: Optional[int] = None,
+    max_truncation_error: Optional[float] = None,
+    relative: Optional[bool] = False,
+) -> Tuple[Tensor, Tensor, Tensor, Tensor]:
+    """Computes the singular value decomposition (SVD) of a tensor.
+
+    The SVD is performed by treating the tensor as a matrix, with an effective
+    left (row) index resulting from combining the axes `tensor.shape[:pivot_axis]`
+    and an effective right (column) index resulting from combining the axes
+    `tensor.shape[pivot_axis:]`.
+
+    For example, if `tensor` had a shape (2, 3, 4, 5) and `pivot_axis` was 2, then
+    `u` would have shape (2, 3, 6), `s` would have shape (6), and `vh` would
+    have shape (6, 4, 5).
+
+    If `max_singular_values` is set to an integer, the SVD is truncated to keep
+    at most this many singular values.
+
+    If `max_truncation_error > 0`, as many singular values will be truncated as
+    possible, so that the truncation error (the norm of discarded singular
+    values) is at most `max_truncation_error`.
+    If `relative` is set `True` then `max_truncation_err` is understood
+    relative to the largest singular value.
+
+    If both `max_singular_values` snd `max_truncation_error` are specified, the
+    number of retained singular values will be
+    `min(max_singular_values, nsv_auto_trunc)`, where `nsv_auto_trunc` is the
+    number of singular values that must be kept to maintain a truncation error
+    smaller than `max_truncation_error`.
+
+    The output consists of three tensors `u, s, vh` such that:
+    ```python
+    u[i1,...,iN, j] * s[j] * vh[j, k1,...,kM] == tensor[i1,...,iN, k1,...,kM]
+    ```
+    Note that the output ordering matches numpy.linalg.svd rather than tf.svd.
+
+    Args:
+    tf: The tensorflow module.
+    tensor: A tensor to be decomposed.
+    pivot_axis: Where to split the tensor's axes before flattening into a
+        matrix.
+    max_singular_values: The number of singular values to keep, or `None` to
+        keep them all.
+    max_truncation_error: The maximum allowed truncation error or `None` to not
+        do any truncation.
+    relative: Multiply `max_truncation_err` with the largest singular value.
+
+    Returns:
+    u: Left tensor factor.
+    s: Vector of ordered singular values from largest to smallest.
+    vh: Right tensor factor.
+    s_rest: Vector of discarded singular values (length zero if no
+            truncation).
+    """
+    left_dims = tf.shape(tensor)[:pivot_axis]
+    right_dims = tf.shape(tensor)[pivot_axis:]
+
+    tensor = tf.reshape(tensor, [tf.reduce_prod(left_dims), tf.reduce_prod(right_dims)])
+
+    eps = os.environ.get("TC_BACKENDS_TENSORFLOW_BACKEND__SVD_TF_EPS")
+    if eps is not None:
+        eps = 10 ** (-int(eps))
+        tensor += eps * tf.ones(tensor.shape, dtype=tensor.dtype)
+        # for numerical stability at least in tf+cpu
+    s, u, v = tf.linalg.svd(tensor)
+
+    if max_singular_values is None:
+        max_singular_values = tf.size(s, out_type=tf.int64)
+    else:
+        max_singular_values = tf.constant(max_singular_values, dtype=tf.int64)
+
+    if max_truncation_error is not None:
+        # Cumulative norms of singular values in ascending order.
+        trunc_errs = tf.sqrt(tf.cumsum(tf.square(s), reverse=True))
+        # If relative is true, rescale max_truncation error with the largest
+        # singular value to yield the absolute maximal truncation error.
+        if relative:
+            abs_max_truncation_error = max_truncation_error * s[0]
+        else:
+            abs_max_truncation_error = max_truncation_error
+        # We must keep at least this many singular values to ensure the
+        # truncation error is <= abs_max_truncation_error.
+        num_sing_vals_err = tf.math.count_nonzero(
+            tf.cast(trunc_errs > abs_max_truncation_error, dtype=tf.int32)
+        )
+    else:
+        num_sing_vals_err = max_singular_values
+
+    num_sing_vals_keep = tf.minimum(max_singular_values, num_sing_vals_err)
+
+    # tf.svd() always returns the singular values as a vector of float{32,64}.
+    # since tf.math_ops.real is automatically applied to s. This causes
+    # s to possibly not be the same dtype as the original tensor, which can cause
+    # issues for later contractions. To fix it, we recast to the original dtype.
+    s = tf.cast(s, tensor.dtype)
+
+    s_rest = s[num_sing_vals_keep:]
+    s = s[:num_sing_vals_keep]
+    u = u[:, :num_sing_vals_keep]
+    v = v[:, :num_sing_vals_keep]
+
+    vh = tf.linalg.adjoint(v)
+
+    dim_s = tf.shape(s)[0]  # must use tf.shape (not s.shape) to compile
+    u = tf.reshape(u, tf.concat([left_dims, [dim_s]], axis=-1))
+    vh = tf.reshape(vh, tf.concat([[dim_s], right_dims], axis=-1))
+
+    return u, s, vh, s_rest
+
+
 # temporary hot replace until new version of tensorflow is released,
 # see issue: https://github.com/google/TensorNetwork/issues/940
 # avoid buggy tensordot2 in tensornetwork
 
 tensornetwork.backends.tensorflow.tensorflow_backend.TensorFlowBackend.tensordot = (
     _tensordot_tf
 )
@@ -236,14 +351,15 @@
     _outer_product_tf
 )
 tensornetwork.backends.tensorflow.tensorflow_backend.TensorFlowBackend.matmul = (
     _matmul_tf
 )
 tensornetwork.backends.tensorflow.tensorflow_backend.TensorFlowBackend.qr = _qr_tf
 tensornetwork.backends.tensorflow.tensorflow_backend.TensorFlowBackend.rq = _rq_tf
+tensornetwork.backends.tensorflow.tensorflow_backend.TensorFlowBackend.svd = _svd_tf
 
 
 class TensorFlowBackend(tensorflow_backend.TensorFlowBackend, ExtendedBackend):  # type: ignore
     """
     See the original backend API at `tensorflow backend
     <https://github.com/google/TensorNetwork/blob/master/tensornetwork/backends/tensorflow/tensorflow_backend.py>`_
     """
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/basecircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/channels.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/apis.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/apis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/local.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/tencent.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/tencent.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cloud/wrapper.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cloud/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/composed_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/compiler/simple_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/compiler/simple_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/cons.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/cons.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/densitymatrix.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/experimental.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/gates.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/__init__.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/interfaces/torch.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/keras.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mps_base.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/mps_base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -123,23 +123,23 @@
                     assert site in (site1, site2)
                     self.center_position = site
                 else:
                     self.center_position = None
 
         if center_position is None:
             center_position = site1
-
         if use_svd:
             U, S, V, tw = self.backend.svd(
                 tensor,
                 pivot_axis=2,
                 max_singular_values=max_singular_values,
                 max_truncation_error=max_truncation_err,
                 relative=relative,
             )
+
             # Note: fix the center position bug here
             if center_position == site2:
                 left_tensor = U
                 right_tensor = ncon.ncon(
                     [self.backend.diagflat(S), V],
                     [[-1, 1], [1, -2, -3]],
                     backend=self.backend,
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/mpscircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
     else:
         if center_left:
             return backend.rq(tensor)  # type: ignore
         else:
             return backend.qr(tensor)  # type: ignore
 
 
+# TODO(@refraction-ray): AD + MPS can lead to numerical stability issue
+# E ./tensorflow/core/kernels/linalg/svd_op_impl.h:110] Eigen::BDCSVD failed with error code 3
+
+
 class MPSCircuit(AbstractCircuit):
     """
     ``MPSCircuit`` class.
     Simple usage demo below.
 
     .. code-block:: python
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/counts.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/blocks.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/chems.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/dataset.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/graphs.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/templates/measurements.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/translation.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/utils.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit/vis.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/PKG-INFO` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit-nightly
-Version: 0.9.1.dev20230518
+Version: 0.9.1.dev20230520
 Summary: nightly release for tensorcircuit
 Home-page: https://github.com/refraction-ray/tensorcircuit-dev
 Author: TensorCircuit Authors
 Author-email: znfesnpbh.tc@gmail.com
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
```

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tensorcircuit_nightly.egg-info/SOURCES.txt` & `tensorcircuit-nightly-0.9.1.dev20230520/tensorcircuit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/conftest.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_backends.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_calibrating.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_channels.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_circuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_cloud.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_cloud.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_compiler.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_dmcircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_ensemble.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_gates.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_interfaces.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_keras.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_miscs.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_mpscircuit.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_noisemodel.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_qaoa.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_quantum_attr.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_results.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_simplify.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_templates.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_torchnn.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_torchnn.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-nightly-0.9.1.dev20230518/tests/test_van.py` & `tensorcircuit-nightly-0.9.1.dev20230520/tests/test_van.py`

 * *Files identical despite different names*

