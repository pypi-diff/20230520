# Comparing `tmp/JaqalPaw-1.1.1.tar.gz` & `tmp/JaqalPaw-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/jaqalpaw/dist/.tmp-8pt8lojc/JaqalPaw-1.1.1.tar", last modified: Wed Mar 29 16:24:11 2023, max compression
+gzip compressed data, was "/tmp/build-jaqal/jaqalpaw/dist/.tmp-4zgtcu7n/JaqalPaw-1.2.0a1.tar", last modified: Fri May 19 23:36:05 2023, max compression
```

## Comparing `JaqalPaw-1.1.1.tar` & `JaqalPaw-1.2.0a1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       81 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      197 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1364 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      486 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/
--rw-rw-r--   0 root         (0) root         (0)       49 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex14.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1341 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex14.py
--rw-rw-r--   0 root         (0) root         (0)     3072 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex14.wvf
--rw-rw-r--   0 root         (0) root         (0)       55 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex3.jaqal
--rw-rw-r--   0 root         (0) root         (0)      508 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex3.py
--rw-rw-r--   0 root         (0) root         (0)     2816 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex3.wvf
--rw-rw-r--   0 root         (0) root         (0)      109 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex4.jaqal
--rw-rw-r--   0 root         (0) root         (0)      602 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex4.py
--rw-rw-r--   0 root         (0) root         (0)     9440 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/ex4.wvf
--rw-rw-r--   0 root         (0) root         (0)       87 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_a.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1335 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_a.py
--rw-rw-r--   0 root         (0) root         (0)     7552 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_a.wvf
--rw-rw-r--   0 root         (0) root         (0)       94 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_b.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1296 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_b.py
--rw-rw-r--   0 root         (0) root         (0)     8832 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_b.wvf
--rw-rw-r--   0 root         (0) root         (0)       83 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iv.jaqal
--rw-rw-r--   0 root         (0) root         (0)      554 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iv.py
--rw-rw-r--   0 root         (0) root         (0)     2816 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iv.wvf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/examples/MSGateFrameRotations/
--rw-rw-r--   0 root         (0) root         (0)      270 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.jaqal
--rw-rw-r--   0 root         (0) root         (0)     5703 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py
--rw-rw-r--   0 root         (0) root         (0)     9792 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/examples/ModulatedMS/
--rw-rw-r--   0 root         (0) root         (0)      331 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS.jaqal
--rw-rw-r--   0 root         (0) root         (0)    10232 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS.py
--rw-rw-r--   0 root         (0) root         (0)     9824 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf
--rw-rw-r--   0 root         (0) root         (0)      518 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/test_sk1.jaqal
--rw-rw-r--   0 root         (0) root         (0)     8000 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/test_sk1.wvf
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/test_std.jaqal
--rw-rw-r--   0 root         (0) root         (0)     7680 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/examples/test_std.wvf
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     2859 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1364 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2876 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/JaqalPaw.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/
--rw-rw-r--   0 root         (0) root         (0)       22 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2346 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/_cli.py
--rw-rw-r--   0 root         (0) root         (0)      410 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2005 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/binary_conversion.py
--rw-rw-r--   0 root         (0) root         (0)     7209 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/encoding_parameters.py
--rw-rw-r--   0 root         (0) root         (0)     6839 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/lut_programming.py
--rw-rw-r--   0 root         (0) root         (0)    18094 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/pulse_binarization.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/bytecode/spline_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/compiler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/compiler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    33383 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/compiler/jaqal_compiler.py
--rw-rw-r--   0 root         (0) root         (0)     2888 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/compiler/time_ordering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9387 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/arbiters.py
--rw-rw-r--   0 root         (0) root         (0)     9795 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/byte_decoding.py
--rw-rw-r--   0 root         (0) root         (0)    19023 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/firmware_emulator.py
--rw-rw-r--   0 root         (0) root         (0)      554 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/pdq_spline.py
--rw-rw-r--   0 root         (0) root         (0)     1928 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/emulator/uram.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3462 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/ast_utilities.py
--rw-rw-r--   0 root         (0) root         (0)     4730 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/circuit_constructor.py
--rw-rw-r--   0 root         (0) root         (0)     7647 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/circuit_constructor_visitor.py
--rw-rw-r--   0 root         (0) root         (0)     6914 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/gate_slice.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/padding.py
--rw-rw-r--   0 root         (0) root         (0)     8614 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/ir/pulse_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/datatypes.py
--rw-rw-r--   0 root         (0) root         (0)      144 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1541 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/helper_functions.py
--rw-rw-r--   0 root         (0) root         (0)      103 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/jaqalpaw/utilities/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/qscout/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/qscout/v1/
--rw-rw-r--   0 root         (0) root         (0)    18055 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/qscout/v1/QSCOUTBuiltins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/qscout/v1/sk1/
--rw-rw-r--   0 root         (0) root         (0)      440 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/qscout/v1/sk1/jaqal_pulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/src/qscout/v1/std/
--rw-rw-r--   0 root         (0) root         (0)      404 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/src/qscout/v1/std/jaqal_pulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/tests/
--rw-rw-r--   0 root         (0) root         (0)      119 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/backcompat.jaqal
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:24:11.000000 JaqalPaw-1.1.1/tests/benchmark/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/benchmark/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1887 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/benchmark/benchmark.py
--rw-rw-r--   0 root         (0) root         (0)    12982 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/run_benchmarks.py
--rw-rw-r--   0 root         (0) root         (0)     1651 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/test_backcompat.py
--rw-rw-r--   0 root         (0) root         (0)      956 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/test_repro.py
--rw-rw-r--   0 root         (0) root         (0)     1159 2023-03-29 16:01:48.000000 JaqalPaw-1.1.1/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      486 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/
+-rw-rw-r--   0 root         (0) root         (0)       49 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1341 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.py
+-rw-rw-r--   0 root         (0) root         (0)     3072 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.wvf
+-rw-rw-r--   0 root         (0) root         (0)       55 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      508 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.py
+-rw-rw-r--   0 root         (0) root         (0)     2816 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.wvf
+-rw-rw-r--   0 root         (0) root         (0)      109 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      602 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.py
+-rw-rw-r--   0 root         (0) root         (0)     9440 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.wvf
+-rw-rw-r--   0 root         (0) root         (0)       87 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1335 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.py
+-rw-rw-r--   0 root         (0) root         (0)     7552 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.wvf
+-rw-rw-r--   0 root         (0) root         (0)       94 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1296 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.py
+-rw-rw-r--   0 root         (0) root         (0)     8832 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.wvf
+-rw-rw-r--   0 root         (0) root         (0)       83 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      554 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.py
+-rw-rw-r--   0 root         (0) root         (0)     2816 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.wvf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/
+-rw-rw-r--   0 root         (0) root         (0)      270 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     5703 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py
+-rw-rw-r--   0 root         (0) root         (0)     9792 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/
+-rw-rw-r--   0 root         (0) root         (0)      331 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.jaqal
+-rw-rw-r--   0 root         (0) root         (0)    10232 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py
+-rw-rw-r--   0 root         (0) root         (0)     9824 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf
+-rw-rw-r--   0 root         (0) root         (0)      518 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_sk1.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     8000 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_sk1.wvf
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_std.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     7680 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/examples/test_std.wvf
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     2863 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2346 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/_cli.py
+-rw-rw-r--   0 root         (0) root         (0)      410 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2005 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/binary_conversion.py
+-rw-rw-r--   0 root         (0) root         (0)     7209 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/encoding_parameters.py
+-rw-rw-r--   0 root         (0) root         (0)     6839 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/lut_programming.py
+-rw-rw-r--   0 root         (0) root         (0)    18094 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/pulse_binarization.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/spline_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    33383 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/jaqal_compiler.py
+-rw-rw-r--   0 root         (0) root         (0)     2888 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/time_ordering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9387 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/arbiters.py
+-rw-rw-r--   0 root         (0) root         (0)     9795 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/byte_decoding.py
+-rw-rw-r--   0 root         (0) root         (0)    19023 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/firmware_emulator.py
+-rw-rw-r--   0 root         (0) root         (0)      554 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/pdq_spline.py
+-rw-rw-r--   0 root         (0) root         (0)     1928 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/uram.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3462 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/ast_utilities.py
+-rw-rw-r--   0 root         (0) root         (0)     4730 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor.py
+-rw-rw-r--   0 root         (0) root         (0)     7647 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py
+-rw-rw-r--   0 root         (0) root         (0)     6914 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/gate_slice.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/padding.py
+-rw-rw-r--   0 root         (0) root         (0)     8614 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/ir/pulse_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1274 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/datatypes.py
+-rw-rw-r--   0 root         (0) root         (0)      144 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1541 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/helper_functions.py
+-rw-rw-r--   0 root         (0) root         (0)      103 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/
+-rw-rw-r--   0 root         (0) root         (0)    18055 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/QSCOUTBuiltins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/sk1/
+-rw-rw-r--   0 root         (0) root         (0)      440 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/sk1/jaqal_pulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/src/qscout/v1/std/
+-rw-rw-r--   0 root         (0) root         (0)      404 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/src/qscout/v1/std/jaqal_pulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/tests/
+-rw-rw-r--   0 root         (0) root         (0)      119 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/backcompat.jaqal
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:36:05.000000 JaqalPaw-1.2.0a1/tests/benchmark/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/benchmark/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1887 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/benchmark/benchmark.py
+-rw-rw-r--   0 root         (0) root         (0)    12982 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/run_benchmarks.py
+-rw-rw-r--   0 root         (0) root         (0)     1651 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_backcompat.py
+-rw-rw-r--   0 root         (0) root         (0)      956 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_repro.py
+-rw-rw-r--   0 root         (0) root         (0)     1159 2023-05-19 20:12:56.000000 JaqalPaw-1.2.0a1/tests/test_smoke.py
```

### Comparing `JaqalPaw-1.1.1/LICENSE` & `JaqalPaw-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/PKG-INFO` & `JaqalPaw-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaw
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Just Another Quantum Assembly Language Pulses and Waveform Specification
 Home-page: https://qscout.sandia.gov
 Author: Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/ex14.py` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/ex14.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex14.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/ex3.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex3.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/ex4.py` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/ex4.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/ex4.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_a.py` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_a.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_a.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_b.py` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iii_b.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iii_b.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iv.py` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/DocumentationSamples/examples_iv.wvf` & `JaqalPaw-1.2.0a1/examples/DocumentationSamples/examples_iv.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py` & `JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf` & `JaqalPaw-1.2.0a1/examples/MSGateFrameRotations/Exemplar_MSGateFrameRotations.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS.py` & `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf` & `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt` & `JaqalPaw-1.2.0a1/examples/ModulatedMS/Exemplar_ModulatedMS_Config.txt`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/test_sk1.wvf` & `JaqalPaw-1.2.0a1/examples/test_sk1.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/examples/test_std.wvf` & `JaqalPaw-1.2.0a1/examples/test_std.wvf`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/setup.cfg` & `JaqalPaw-1.2.0a1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = JaqalPaw
 author = Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 author_email = qscout@sandia.gov
 description = Just Another Quantum Assembly Language Pulses and Waveform Specification
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.1.1
+version = 1.2.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,15 +18,15 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = numpy; scipy; jaqalpaq>=1.1.1
+install_requires = numpy; scipy; jaqalpaq>=1.2.0a1
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	jaqalpaw
 	jaqalpaw.*
```

### Comparing `JaqalPaw-1.1.1/src/JaqalPaw.egg-info/PKG-INFO` & `JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaw
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Just Another Quantum Assembly Language Pulses and Waveform Specification
 Home-page: https://qscout.sandia.gov
 Author: Daniel Lobser, Benjamin C. A. Morrison, Kenneth Rudinger, Antonio Russo, Jay Wesley Van Der Wall
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaw-1.1.1/src/JaqalPaw.egg-info/SOURCES.txt` & `JaqalPaw-1.2.0a1/src/JaqalPaw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/_cli.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/_cli.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/bytecode/binary_conversion.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/binary_conversion.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/bytecode/encoding_parameters.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/encoding_parameters.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/bytecode/lut_programming.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/lut_programming.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/bytecode/pulse_binarization.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/pulse_binarization.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/bytecode/spline_mapping.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/bytecode/spline_mapping.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/compiler/jaqal_compiler.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/jaqal_compiler.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/compiler/time_ordering.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/compiler/time_ordering.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/emulator/arbiters.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/arbiters.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/emulator/byte_decoding.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/byte_decoding.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/emulator/firmware_emulator.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/firmware_emulator.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/emulator/pdq_spline.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/pdq_spline.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/emulator/uram.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/emulator/uram.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/ast_utilities.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/ast_utilities.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/circuit_constructor.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/circuit_constructor_visitor.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/circuit_constructor_visitor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/gate_slice.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/gate_slice.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/padding.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/padding.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/ir/pulse_data.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/ir/pulse_data.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/utilities/datatypes.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/datatypes.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/jaqalpaw/utilities/helper_functions.py` & `JaqalPaw-1.2.0a1/src/jaqalpaw/utilities/helper_functions.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/src/qscout/v1/QSCOUTBuiltins.py` & `JaqalPaw-1.2.0a1/src/qscout/v1/QSCOUTBuiltins.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/tests/benchmark/benchmark.py` & `JaqalPaw-1.2.0a1/tests/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/tests/run_benchmarks.py` & `JaqalPaw-1.2.0a1/tests/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/tests/test_backcompat.py` & `JaqalPaw-1.2.0a1/tests/test_backcompat.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/tests/test_repro.py` & `JaqalPaw-1.2.0a1/tests/test_repro.py`

 * *Files identical despite different names*

### Comparing `JaqalPaw-1.1.1/tests/test_smoke.py` & `JaqalPaw-1.2.0a1/tests/test_smoke.py`

 * *Files identical despite different names*

