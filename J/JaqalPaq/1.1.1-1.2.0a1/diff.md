# Comparing `tmp/JaqalPaq-1.1.1.tar.gz` & `tmp/JaqalPaq-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/jaqalpaq/dist/.tmp-y78_v1mo/JaqalPaq-1.1.1.tar", last modified: Wed Mar 29 16:23:29 2023, max compression
+gzip compressed data, was "/tmp/build-jaqal/jaqalpaq/dist/.tmp-xx3uijcb/JaqalPaq-1.2.0a1.tar", last modified: Fri May 19 23:35:22 2023, max compression
```

## Comparing `JaqalPaq-1.1.1.tar` & `JaqalPaq-1.2.0a1.tar`

### file list

```diff
@@ -1,202 +1,214 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       52 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      197 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     7716 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6818 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/H2 (Molecular Hydrogen)/
--rw-rw-r--   0 root         (0) root         (0)    86609 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/H2 (Molecular Hydrogen)/JaqalPaq_H2_Exemplar.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/HeH+ (Helium Hydride)/
--rw-rw-r--   0 root         (0) root         (0)    89927 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Tapered_Exemplar.ipynb
--rw-rw-r--   0 root         (0) root         (0)    90735 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Untapered_Exemplar.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/LiH (Lithium Hydride)/
--rw-rw-r--   0 root         (0) root         (0)    88809 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/LiH (Lithium Hydride)/JaqalPaq_LiH_Exemplar.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/Tutorials/
--rw-rw-r--   0 root         (0) root         (0)   117694 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/Tutorials/Emulator_Demo.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/jaqal/
--rw-rw-r--   0 root         (0) root         (0)       85 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/Sxx_circuit.jaqal
--rw-rw-r--   0 root         (0) root         (0)      184 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/Sxx_circuit_q.py
--rw-rw-r--   0 root         (0) root         (0)     1201 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/bell_prep.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1433 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/bell_prep.py
--rw-rw-r--   0 root         (0) root         (0)      891 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/bell_prep_q.py
--rw-rw-r--   0 root         (0) root         (0)      719 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/bell_prep_spec.jaqal
--rw-rw-r--   0 root         (0) root         (0)      179 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      180 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_loop_outside_subcircuit.jaqal
--rw-rw-r--   0 root         (0) root         (0)      199 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_loop_q.py
--rw-rw-r--   0 root         (0) root         (0)      198 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_parallel.jaqal
--rw-rw-r--   0 root         (0) root         (0)      205 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_parallel_q.py
--rw-rw-r--   0 root         (0) root         (0)       46 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_prog.jaqal
--rw-rw-r--   0 root         (0) root         (0)      170 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/empty_prog_q.py
--rw-rw-r--   0 root         (0) root         (0)      309 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/idle_padding.jaqal
--rw-rw-r--   0 root         (0) root         (0)      240 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/idle_padding_q.py
--rw-rw-r--   0 root         (0) root         (0)      406 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/molmer-sorensen-rotations.jaqal
--rw-rw-r--   0 root         (0) root         (0)      294 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/molmer-sorensen-rotations_q.py
--rw-rw-r--   0 root         (0) root         (0)     8937 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/nested_bit_flips.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1072 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/nested_bit_flips_q.py
--rw-rw-r--   0 root         (0) root         (0)       59 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/no_measure.jaqal
--rw-rw-r--   0 root         (0) root         (0)      146 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/no_prepare.jaqal
--rw-rw-r--   0 root         (0) root         (0)      172 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/nonempty_zero_loop_outside_subcircuit.jaqal
--rw-rw-r--   0 root         (0) root         (0)     1036 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/one-qubit-rotations.jaqal
--rw-rw-r--   0 root         (0) root         (0)      740 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/one-qubit-rotations_q.py
--rw-rw-r--   0 root         (0) root         (0)      224 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/only_idles.jaqal
--rw-rw-r--   0 root         (0) root         (0)      211 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/only_idles_q.py
--rw-rw-r--   0 root         (0) root         (0)      159 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_block_in_parallel_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      279 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_block_in_sequential_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      289 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_block_in_sequential_loop_q.py
--rw-rw-r--   0 root         (0) root         (0)      201 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_gate_collision.jaqal
--rw-rw-r--   0 root         (0) root         (0)       90 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_idle.jaqal
--rw-rw-r--   0 root         (0) root         (0)      213 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_idle_q.py
--rw-rw-r--   0 root         (0) root         (0)      278 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      425 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/parallel_prep-parallel_measure.jaqal
--rw-rw-r--   0 root         (0) root         (0)      606 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/pi_fracs.jaqal
--rw-rw-r--   0 root         (0) root         (0)      540 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/pi_fracs_q.py
--rw-rw-r--   0 root         (0) root         (0)      385 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/prepare-measure-equiv.jaqal
--rw-rw-r--   0 root         (0) root         (0)      325 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/prepare-measure-equiv_q.py
--rw-rw-r--   0 root         (0) root         (0)      235 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/prepare-measure.jaqal
--rw-rw-r--   0 root         (0) root         (0)      280 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/sequential_block_in_parallel_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      153 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/sequential_loop_in_parallel.jaqal
--rw-rw-r--   0 root         (0) root         (0)      239 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/sequential_loop_in_parallel_q.py
--rw-rw-r--   0 root         (0) root         (0)     1751 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst.jaqal
--rw-rw-r--   0 root         (0) root         (0)     4164 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst.py
--rw-rw-r--   0 root         (0) root         (0)     1717 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst_q.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/
--rw-rw-r--   0 root         (0) root         (0)       78 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/bell.jaqal
--rw-rw-r--   0 root         (0) root         (0)      241 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/blocks.jaqal
--rw-rw-r--   0 root         (0) root         (0)      330 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/compile.jaqal
--rw-rw-r--   0 root         (0) root         (0)       49 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/constants.jaqal
--rw-rw-r--   0 root         (0) root         (0)      464 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/crz.jaqal
--rw-rw-r--   0 root         (0) root         (0)       67 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)       71 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/macro.jaqal
--rw-rw-r--   0 root         (0) root         (0)      125 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/output.jaqal
--rw-rw-r--   0 root         (0) root         (0)       43 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/registers.jaqal
--rw-rw-r--   0 root         (0) root         (0)       34 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/slice.jaqal
--rw-rw-r--   0 root         (0) root         (0)       47 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/spec_samples/two_qubit_gate.jaqal
--rw-rw-r--   0 root         (0) root         (0)      273 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/two-qubit-nonadjacent.jaqal
--rw-rw-r--   0 root         (0) root         (0)      207 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/two-qubit-nonadjacent_q.py
--rw-rw-r--   0 root         (0) root         (0)      186 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/zero_loop.jaqal
--rw-rw-r--   0 root         (0) root         (0)      203 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/jaqal/zero_loop_q.py
--rw-rw-r--   0 root         (0) root         (0)      423 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/examples/usage_example.py
--rw-rw-r--   0 root         (0) root         (0)      111 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     6003 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7716 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5900 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      265 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/JaqalPaq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/
--rw-rw-r--   0 root         (0) root         (0)     7106 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/_cli.py
--rw-rw-r--   0 root         (0) root         (0)     3983 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/
--rw-rw-r--   0 root         (0) root         (0)     1050 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/
--rw-rw-r--   0 root         (0) root         (0)      604 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5242 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/expand_macros.py
--rw-rw-r--   0 root         (0) root         (0)     3328 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/expand_subcircuits.py
--rw-rw-r--   0 root         (0) root         (0)     6230 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/fill_in_let.py
--rw-rw-r--   0 root         (0) root         (0)     3935 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/fill_in_map.py
--rw-rw-r--   0 root         (0) root         (0)     4479 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/unit_timing.py
--rw-rw-r--   0 root         (0) root         (0)     4575 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/used_qubit_visitor.py
--rw-rw-r--   0 root         (0) root         (0)     3308 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/visitor.py
--rw-rw-r--   0 root         (0) root         (0)     7660 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/walkers.py
--rw-rw-r--   0 root         (0) root         (0)     4829 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/block.py
--rw-rw-r--   0 root         (0) root         (0)     3142 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/branch.py
--rw-rw-r--   0 root         (0) root         (0)     5005 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/circuit.py
--rw-rw-r--   0 root         (0) root         (0)    35567 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/circuitbuilder.py
--rw-rw-r--   0 root         (0) root         (0)     2272 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/constant.py
--rw-rw-r--   0 root         (0) root         (0)     2389 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/gate.py
--rw-rw-r--   0 root         (0) root         (0)     8378 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/gatedef.py
--rw-rw-r--   0 root         (0) root         (0)      610 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/identifier.py
--rw-rw-r--   0 root         (0) root         (0)     1427 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/macro.py
--rw-rw-r--   0 root         (0) root         (0)     7753 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/parameter.py
--rw-rw-r--   0 root         (0) root         (0)    14122 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/register.py
--rw-rw-r--   0 root         (0) root         (0)    11340 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/result.py
--rw-rw-r--   0 root         (0) root         (0)     2205 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/stretch.py
--rw-rw-r--   0 root         (0) root         (0)     2524 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/core/usepulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/
--rw-rw-r--   0 root         (0) root         (0)      393 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7521 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/_validator.py
--rw-rw-r--   0 root         (0) root         (0)     7238 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/backend.py
--rw-rw-r--   0 root         (0) root         (0)      366 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/
--rw-rw-r--   0 root         (0) root         (0)       24 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3722 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/backends.py
--rw-rw-r--   0 root         (0) root         (0)     7630 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/circuit.py
--rw-rw-r--   0 root         (0) root         (0)    12828 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/model.py
--rw-rw-r--   0 root         (0) root         (0)     6006 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/emulator/unitary.py
--rw-rw-r--   0 root         (0) root         (0)      489 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/generator/
--rw-rw-r--   0 root         (0) root         (0)      287 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/generator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5492 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/generator/generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/ipc/
--rw-rw-r--   0 root         (0) root         (0)      203 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/ipc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4636 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/ipc/ipc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/parser/
--rw-rw-r--   0 root         (0) root         (0)      409 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/parser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1141 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/parser/identifier.py
--rw-rw-r--   0 root         (0) root         (0)     7375 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/parser/parser.py
--rw-rw-r--   0 root         (0) root         (0)    15508 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/parser/slyparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/
--rw-rw-r--   0 root         (0) root         (0)      263 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3450 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/compile.py
--rw-rw-r--   0 root         (0) root         (0)    19877 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/qsyntax.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/src/jaqalpaq/run/
--rw-rw-r--   0 root         (0) root         (0)      359 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/run/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4103 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/run/run.py
--rw-rw-r--   0 root         (0) root         (0)      453 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/src/jaqalpaq/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/core/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6799 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/abstractgate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/core/algorithm/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3892 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_expand_macros.py
--rw-rw-r--   0 root         (0) root         (0)     6040 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_expand_subcircuits.py
--rw-rw-r--   0 root         (0) root         (0)     5348 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_fill_in_let.py
--rw-rw-r--   0 root         (0) root         (0)     1785 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_unit_timing.py
--rw-rw-r--   0 root         (0) root         (0)     4504 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_used_qubits.py
--rw-rw-r--   0 root         (0) root         (0)     1289 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/algorithm/test_visitor.py
--rw-rw-r--   0 root         (0) root         (0)    11819 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/common.py
--rw-rw-r--   0 root         (0) root         (0)      192 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/gpf1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/core/gpf2/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/gpf2/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      209 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/gpf2/jaqal_gates.py
--rw-rw-r--   0 root         (0) root         (0)     2195 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/randomize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/core/reload/
--rw-rw-r--   0 root         (0) root         (0)      200 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/reload/gpf1.py
--rw-rw-r--   0 root         (0) root         (0)     1353 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_block.py
--rw-rw-r--   0 root         (0) root         (0)     2286 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_branch.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_circuit.py
--rw-rw-r--   0 root         (0) root         (0)    21056 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_circuitbuilder.py
--rw-rw-r--   0 root         (0) root         (0)     2042 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_constant.py
--rw-rw-r--   0 root         (0) root         (0)      853 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_gate.py
--rw-rw-r--   0 root         (0) root         (0)      381 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_gatedef.py
--rw-rw-r--   0 root         (0) root         (0)     1220 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_loop.py
--rw-rw-r--   0 root         (0) root         (0)      660 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_macro.py
--rw-rw-r--   0 root         (0) root         (0)     6183 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_named_qubit.py
--rw-rw-r--   0 root         (0) root         (0)     5517 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_parameter.py
--rw-rw-r--   0 root         (0) root         (0)     8687 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_register.py
--rw-rw-r--   0 root         (0) root         (0)     4004 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/core/test_usepulses.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/emulator/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/emulator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18015 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/emulator/test_forward_simulation.py
--rw-rw-r--   0 root         (0) root         (0)     2280 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/emulator/test_jaqal_files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/generator/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/generator/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3613 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/generator/test_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/ipc/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/ipc/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1045 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/ipc/_mock_server.py
--rw-rw-r--   0 root         (0) root         (0)     1209 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/ipc/test_ipc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/jaqalparser/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/jaqalparser/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1306 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/jaqalparser/test_examples.py
--rw-rw-r--   0 root         (0) root         (0)    24509 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/jaqalparser/test_jaqalpup_parser.py
--rw-rw-r--   0 root         (0) root         (0)    16772 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/jaqalparser/test_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 16:23:29.000000 JaqalPaq-1.1.1/tests/qsyntax/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/qsyntax/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5074 2023-03-29 16:04:49.000000 JaqalPaq-1.1.1/tests/qsyntax/test_qsyntax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6818 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/H2 (Molecular Hydrogen)/
+-rw-rw-r--   0 root         (0) root         (0)    86609 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/H2 (Molecular Hydrogen)/JaqalPaq_H2_Exemplar.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/HeH+ (Helium Hydride)/
+-rw-rw-r--   0 root         (0) root         (0)    89927 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Tapered_Exemplar.ipynb
+-rw-rw-r--   0 root         (0) root         (0)    90735 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Untapered_Exemplar.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/LiH (Lithium Hydride)/
+-rw-rw-r--   0 root         (0) root         (0)    88809 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/LiH (Lithium Hydride)/JaqalPaq_LiH_Exemplar.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/Tutorials/
+-rw-rw-r--   0 root         (0) root         (0)   228827 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/Tutorials/BatchingExamples.ipynb
+-rw-rw-r--   0 root         (0) root         (0)   117750 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/Tutorials/Emulator_Demo.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/jaqal/
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/Sxx_circuit.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      184 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/Sxx_circuit_q.py
+-rw-rw-r--   0 root         (0) root         (0)     1201 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/bell_prep.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1433 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/bell_prep.py
+-rw-rw-r--   0 root         (0) root         (0)      891 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/bell_prep_q.py
+-rw-rw-r--   0 root         (0) root         (0)      719 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/bell_prep_spec.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1208 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/bell_prep_subcircuit.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      179 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      180 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_loop_outside_subcircuit.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      199 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_loop_q.py
+-rw-rw-r--   0 root         (0) root         (0)      198 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_parallel.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_parallel_q.py
+-rw-rw-r--   0 root         (0) root         (0)       46 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_prog.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      170 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/empty_prog_q.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/idle_padding.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/idle_padding_q.py
+-rw-rw-r--   0 root         (0) root         (0)      406 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/molmer-sorensen-rotations.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      294 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/molmer-sorensen-rotations_q.py
+-rw-rw-r--   0 root         (0) root         (0)     8937 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/nested_bit_flips.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/nested_bit_flips_q.py
+-rw-rw-r--   0 root         (0) root         (0)      131 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/no_measure.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/no_prepare.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      172 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/nonempty_zero_loop_outside_subcircuit.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     1036 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/one-qubit-rotations.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      740 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/one-qubit-rotations_q.py
+-rw-rw-r--   0 root         (0) root         (0)      224 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/only_idles.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      211 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/only_idles_q.py
+-rw-rw-r--   0 root         (0) root         (0)      159 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_block_in_parallel_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      279 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_block_in_sequential_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      289 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_block_in_sequential_loop_q.py
+-rw-rw-r--   0 root         (0) root         (0)      201 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_gate_collision.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       90 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_idle.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      213 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_idle_q.py
+-rw-rw-r--   0 root         (0) root         (0)      278 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      425 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/parallel_prep-parallel_measure.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      606 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/pi_fracs.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      540 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/pi_fracs_q.py
+-rw-rw-r--   0 root         (0) root         (0)      385 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/prepare-measure-equiv.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      325 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/prepare-measure-equiv_q.py
+-rw-rw-r--   0 root         (0) root         (0)      235 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/prepare-measure.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/sequential_block_in_parallel_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      153 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/sequential_loop_in_parallel.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      239 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/sequential_loop_in_parallel_q.py
+-rw-rw-r--   0 root         (0) root         (0)     1751 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst.jaqal
+-rw-rw-r--   0 root         (0) root         (0)     4164 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst.py
+-rw-rw-r--   0 root         (0) root         (0)     1717 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst_q.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/
+-rw-rw-r--   0 root         (0) root         (0)       78 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/bell.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      241 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/blocks.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      330 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/compile.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       49 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/constants.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      464 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/crz.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/macro.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      125 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/output.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       43 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/registers.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       34 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/slice.jaqal
+-rw-rw-r--   0 root         (0) root         (0)       47 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/spec_samples/two_qubit_gate.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      159 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/subcircuit.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      273 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/two-qubit-nonadjacent.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      207 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/two-qubit-nonadjacent_q.py
+-rw-rw-r--   0 root         (0) root         (0)      186 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/zero_loop.jaqal
+-rw-rw-r--   0 root         (0) root         (0)      203 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/jaqal/zero_loop_q.py
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/examples/usage_example.py
+-rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     6211 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6257 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/
+-rw-rw-r--   0 root         (0) root         (0)     7106 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/_cli.py
+-rw-rw-r--   0 root         (0) root         (0)     4005 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/
+-rw-rw-r--   0 root         (0) root         (0)     1050 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/
+-rw-rw-r--   0 root         (0) root         (0)      604 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5638 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/expand_macros.py
+-rw-rw-r--   0 root         (0) root         (0)     3384 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/expand_subcircuits.py
+-rw-rw-r--   0 root         (0) root         (0)     6393 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/fill_in_let.py
+-rw-rw-r--   0 root         (0) root         (0)     4025 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/fill_in_map.py
+-rw-rw-r--   0 root         (0) root         (0)     4479 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/unit_timing.py
+-rw-rw-r--   0 root         (0) root         (0)     4575 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/used_qubit_visitor.py
+-rw-rw-r--   0 root         (0) root         (0)     3361 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/visitor.py
+-rw-rw-r--   0 root         (0) root         (0)     9429 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/walkers.py
+-rw-rw-r--   0 root         (0) root         (0)     4829 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/block.py
+-rw-rw-r--   0 root         (0) root         (0)     3142 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/branch.py
+-rw-rw-r--   0 root         (0) root         (0)     5542 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/circuit.py
+-rw-rw-r--   0 root         (0) root         (0)    35547 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/circuitbuilder.py
+-rw-rw-r--   0 root         (0) root         (0)     2272 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/constant.py
+-rw-rw-r--   0 root         (0) root         (0)     2389 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/gate.py
+-rw-rw-r--   0 root         (0) root         (0)     9705 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/gatedef.py
+-rw-rw-r--   0 root         (0) root         (0)      610 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/identifier.py
+-rw-rw-r--   0 root         (0) root         (0)     2940 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/locus.py
+-rw-rw-r--   0 root         (0) root         (0)     1877 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/macro.py
+-rw-rw-r--   0 root         (0) root         (0)     7753 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/parameter.py
+-rw-rw-r--   0 root         (0) root         (0)    14122 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/register.py
+-rw-rw-r--   0 root         (0) root         (0)     3620 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/stretch.py
+-rw-rw-r--   0 root         (0) root         (0)     2524 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/core/usepulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/
+-rw-rw-r--   0 root         (0) root         (0)      450 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      435 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/_import.py
+-rw-rw-r--   0 root         (0) root         (0)     7677 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/_validator.py
+-rw-rw-r--   0 root         (0) root         (0)     5685 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3500 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/backends.py
+-rw-rw-r--   0 root         (0) root         (0)     7630 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/circuit.py
+-rw-rw-r--   0 root         (0) root         (0)    13118 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/model.py
+-rw-rw-r--   0 root         (0) root         (0)     6047 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/unitary.py
+-rw-rw-r--   0 root         (0) root         (0)      489 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/generator/
+-rw-rw-r--   0 root         (0) root         (0)      287 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/generator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5492 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/generator/generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/ipc/
+-rw-rw-r--   0 root         (0) root         (0)      203 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/ipc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3578 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/ipc/client.py
+-rw-rw-r--   0 root         (0) root         (0)     3844 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/ipc/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/parser/
+-rw-rw-r--   0 root         (0) root         (0)      409 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/parser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1141 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/parser/identifier.py
+-rw-rw-r--   0 root         (0) root         (0)     7657 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/parser/parser.py
+-rw-rw-r--   0 root         (0) root         (0)    15539 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/parser/slyparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3466 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/compile.py
+-rw-rw-r--   0 root         (0) root         (0)    19877 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/qsyntax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/
+-rw-rw-r--   0 root         (0) root         (0)      964 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3699 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/_view.py
+-rw-rw-r--   0 root         (0) root         (0)     2111 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/backend.py
+-rw-rw-r--   0 root         (0) root         (0)     9530 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/classical_cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     5985 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/cursor.py
+-rw-rw-r--   0 root         (0) root         (0)     4211 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/frontend.py
+-rw-rw-r--   0 root         (0) root         (0)    32197 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/run/result.py
+-rw-rw-r--   0 root         (0) root         (0)      453 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/src/jaqalpaq/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/core/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6754 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/abstractgate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3892 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_expand_macros.py
+-rw-rw-r--   0 root         (0) root         (0)     6040 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_expand_subcircuits.py
+-rw-rw-r--   0 root         (0) root         (0)     5348 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_fill_in_let.py
+-rw-rw-r--   0 root         (0) root         (0)     1785 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_unit_timing.py
+-rw-rw-r--   0 root         (0) root         (0)     4504 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_used_qubits.py
+-rw-rw-r--   0 root         (0) root         (0)     1289 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/algorithm/test_visitor.py
+-rw-rw-r--   0 root         (0) root         (0)    11819 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/common.py
+-rw-rw-r--   0 root         (0) root         (0)      192 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/gpf1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/core/gpf2/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/gpf2/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      209 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/gpf2/jaqal_gates.py
+-rw-rw-r--   0 root         (0) root         (0)     2195 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/randomize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/core/reload/
+-rw-rw-r--   0 root         (0) root         (0)      200 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/reload/gpf1.py
+-rw-rw-r--   0 root         (0) root         (0)     1353 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_block.py
+-rw-rw-r--   0 root         (0) root         (0)     2286 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_branch.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_circuit.py
+-rw-rw-r--   0 root         (0) root         (0)    21056 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_circuitbuilder.py
+-rw-rw-r--   0 root         (0) root         (0)     2042 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_constant.py
+-rw-rw-r--   0 root         (0) root         (0)      853 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_gate.py
+-rw-rw-r--   0 root         (0) root         (0)      381 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_gatedef.py
+-rw-rw-r--   0 root         (0) root         (0)     1220 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_loop.py
+-rw-rw-r--   0 root         (0) root         (0)      660 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_macro.py
+-rw-rw-r--   0 root         (0) root         (0)     6183 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_named_qubit.py
+-rw-rw-r--   0 root         (0) root         (0)     5517 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_parameter.py
+-rw-rw-r--   0 root         (0) root         (0)     8687 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_register.py
+-rw-rw-r--   0 root         (0) root         (0)     4004 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/core/test_usepulses.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/emulator/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/emulator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21828 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/emulator/test_forward_simulation.py
+-rw-rw-r--   0 root         (0) root         (0)     2219 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/emulator/test_jaqal_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/generator/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/generator/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3613 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/generator/test_generator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/ipc/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/ipc/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4425 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/ipc/test_ipc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/jaqalparser/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/jaqalparser/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1306 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/jaqalparser/test_examples.py
+-rw-rw-r--   0 root         (0) root         (0)    24509 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/jaqalparser/test_jaqalpup_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    16772 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/jaqalparser/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/qsyntax/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/qsyntax/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5074 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/qsyntax/test_qsyntax.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:22.000000 JaqalPaq-1.2.0a1/tests/run/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/run/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     8583 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/run/batching_reference.py
+-rw-rw-r--   0 root         (0) root         (0)     6934 2023-05-19 23:28:10.000000 JaqalPaq-1.2.0a1/tests/run/test_classical_cursor.py
```

### Comparing `JaqalPaq-1.1.1/LICENSE` & `JaqalPaq-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/PKG-INFO` & `JaqalPaq-1.2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaq
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Python tools for Jaqal
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaq-1.1.1/README.md` & `JaqalPaq-1.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/H2 (Molecular Hydrogen)/JaqalPaq_H2_Exemplar.ipynb` & `JaqalPaq-1.2.0a1/examples/H2 (Molecular Hydrogen)/JaqalPaq_H2_Exemplar.ipynb`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Tapered_Exemplar.ipynb` & `JaqalPaq-1.2.0a1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Tapered_Exemplar.ipynb`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Untapered_Exemplar.ipynb` & `JaqalPaq-1.2.0a1/examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Untapered_Exemplar.ipynb`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/LiH (Lithium Hydride)/JaqalPaq_LiH_Exemplar.ipynb` & `JaqalPaq-1.2.0a1/examples/LiH (Lithium Hydride)/JaqalPaq_LiH_Exemplar.ipynb`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/Tutorials/Emulator_Demo.ipynb` & `JaqalPaq-1.2.0a1/examples/Tutorials/Emulator_Demo.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997958453848088%*

 * *Differences: {"'cells'": '{2: {\'source\': {insert: [(30, \'""", name_hint=\\\'familiar_circuit\\\') # Give the '*

 * *            "circuit a name for a nicer repr')], delete: [30]}}, 5: {'outputs': {0: {'data': "*

 * *            "{'text/plain': ['<ExecutionResult@1970-01-01T00:00:00.000000Z of <Circuit (expanded) "*

 * *            "familiar_circuit>>']}}}}, 6: {'outputs': {0: {'data': {'text/plain': "*

 * *            "['[<SubcircuitView 0@Locus<(0,)> of <Circuit (expanded) familiar_circuit>>,\\n', ' "*

 * *            "<SubcircuitView 1@Loc […]*

```diff
@@ -65,15 +65,15 @@
                 "\n",
                 "subcircuit {\n",
                 " hadamard q[0]\n",
                 " cnot q[0] q[1]\n",
                 " Px q[0]\n",
                 "}\n",
                 "\n",
-                "\"\"\")"
+                "\"\"\", name_hint='familiar_circuit') # Give the circuit a name for a nicer repr"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Unitary Emulation"
@@ -108,15 +108,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<jaqalpaq.core.result.ExecutionResult at 0x85aa69c9ca30>"
+                            "<ExecutionResult@1970-01-01T00:00:00.000000Z of <Circuit (expanded) familiar_circuit>>"
                         ]
                     },
                     "execution_count": 4,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -136,15 +136,16 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "[<EmulatorSubcircuit 0@[7]>, <EmulatorSubcircuit 1@[16]>]"
+                            "[<SubcircuitView 0@Locus<(0,)> of <Circuit (expanded) familiar_circuit>>,\n",
+                            " <SubcircuitView 1@Locus<(1,)> of <Circuit (expanded) familiar_circuit>>]"
                         ]
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -164,15 +165,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([5.00000000e-01, 1.54074396e-32, 6.16297582e-33, 5.00000000e-01])"
+                            "array([0.5, 0. , 0. , 0.5])"
                         ]
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -192,15 +193,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([7.08490623e-33, 5.00000000e-01, 5.00000000e-01, 8.03767555e-33])"
+                            "array([0. , 0.5, 0.5, 0. ])"
                         ]
                     },
                     "execution_count": 7,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -220,15 +221,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([5.00000000e-01, 1.54074396e-32, 6.16297582e-33, 5.00000000e-01])"
+                            "array([0.5, 0. , 0. , 0.5])"
                         ]
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -379,15 +380,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<jaqalpaq.core.result.ExecutionResult at 0x85aa69c9ca30>"
+                            "<ExecutionResult@1970-01-01T00:00:00.000000Z of <Circuit (expanded) familiar_circuit>>"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -407,15 +408,15 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "array([0.01231296, 0.48720558, 0.48672233, 0.01375913])"
+                            "array([0.01701459, 0.4825135 , 0.4820207 , 0.01845121])"
                         ]
                     },
                     "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -462,15 +463,15 @@
                     "shell.execute_reply": "1970-01-01T00:00:00.000000Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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MzNnztS3336rb7/9Vh999JHatm2rJ554QsuXL7fNWbZsmYKCgtShQwelp6fbHuHh4fL399fatWtvOkeDBg20detWPf744zpw4ICmT5+uLl26KDg4WO+9955D27BarfLwuPRnLDc3VydOnJC/v7/q1q2r5OTk666/detW7d69W7169dKJEyds7zMrK0vt27fX999/r7y8vOtu56mnnrL9TP/6qF+/vm2On5+f5s+frx07dujvf/+7VqxYobfeektVq1bNt73IyEiFh4fblqtWraoHH3xQq1atUm5urgzD0GeffabOnTvLMAy731FMTIwyMjLyvf8+ffrI19f3uu9FurRH7NFHH7Ut161bV6VKlVK9evUUERFhG7/873379knSDeWKjY2123t4eY/q5W0CcA6HYoHbTMuWLe0unujZs6eaNWumwYMH6/7775e3t7d2796tjIwMu3Pd/spVFzfUqVNHH374oXJzc/X777/r3//+tyZNmqSnnnpK1atXV3R09DXXz8vL0/Tp0/Xuu+9q//79ys3NtT1XtmzZ677+7t27JV0qPVeTkZGh0qVLX3M7tWvXvm5WSWrdurWeeeYZzZw5UzExMerXr99Vt3elOnXq6Ny5czp+/Lg8PDx0+vRpzZkzR3PmzClwG1f+jqpXr37dfJdVqVJFFovFbiwoKEihoaH5xiTZzrs8fvy407muLLaXf9auOpcTuN1Q7IDbnIeHh9q2bavp06dr9+7datCggfLy8lShQgUtWrSowHXKly/v0gyenp5q1KiRGjVqpMjISLVt21aLFi26bll6/fXXNWbMGPXr10/jx49XmTJl5OHhoWHDhjm0p+3ynMmTJ1/1NiiuPJ8rOzvbdqHC3r17de7cOfn5+Tm9ncu5H3/88auW0saNG9stO7q3Trr0+3Bm3DCMG851vW0CcA7FDoD+/PNPSdLZs2clSTVr1tSaNWvUunVrpwqBK1zem5iSkmIbu3Lv0WWffvqp2rZtqw8++MBu/PTp0ypXrtx1169Zs6YkKTAw0KE9bjcrPj5eO3bs0JtvvqkXX3xRI0eO1Ntvv51v3uU9iX+1a9cu+fn52Up1QECAcnNziyS3o8qXL18oua72+wOQH+fYAbe5ixcvavXq1fL29la9evUkSd27d1dubq7Gjx+fb/6ff/6p06dP3/Tr/vDDD7p48WK+8a+//lrS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DgAAwCQodgAAACZBsQMAADCJmy52mZmZ+uKLL7Rjxw5X5AEAAMANcrrYde/eXTNmzJAknT9/Xi1atFD37t3VuHFjffbZZy4PCAAAAMc4Xey+//573X333ZKkzz//XIZh6PTp03r77bf12muvuTwgAAAAHON0scvIyFCZMmUkSStXrtRDDz0kPz8/derUSbt373Z5QAAAADjG6WIXGhqqpKQkZWVlaeXKlerYsaMk6dSpU/Lx8XF5QAAAADimhLMrDBs2TI899pj8/f1VrVo1tWnTRtKlQ7SNGjVydT4AAAA4yOliN3DgQEVEROjQoUPq0KGDPDwu7fSrUaOGJkyY4PKAAAAAcIzTh2JfffVV1atXT127dpW/v79tvF27dlqzZo1LwwEAAMBxFsMwDGdW8PT0VEpKiipUqGA3fuLECVWoUEG5ubkuDehqmZmZCgoKUkZGhgIDA90dBwAA4Jqc6S5O77EzDEMWiyXf+C+//GK7WhYAAABFz+Fz7EqXLi2LxSKLxaI6derYlbvc3FydPXtWAwYMKJSQAAAAuD6Hi920adNkGIb69euncePGKSgoyPact7e3wsLCFBkZWSghAQAAcH0OF7s+ffpIkqpXr65WrVrJy8ur0EIBAADAeU7f7iQqKkp5eXnatWuXjh07pry8PLvn//73v7ssHAAAABzndLH7z3/+o169eungwYO68oJai8VS7K+KBQAAMCuni92AAQPUokULrVixQhUrVizwClkAAAAUPaeL3e7du/Xpp5+qVq1ahZEHAAAAN8jp+9hFRERoz549hZEFAAAAN8HpPXbPPvusnnvuOaWmpqpRo0b5ro5t3Lixy8IBAADAcU5/pZiHR/6dfBaLxfaNFMX94gm+UgwAANxKnOkuTu+x279//w0HAwAAQOFxuthVq1atMHIAAADgJjld7BYuXHjN53v37n3DYQAAAHDjnD7HrnTp0nbLFy9e1Llz5+Tt7S0/Pz+dPHnSpQFdjXPsAADArcSZ7uL07U5OnTpl9zh79qz++OMP3XXXXfr4449vODQAAABujtPFriC1a9fWG2+8oaFDh7picwAAALgBLil2klSiRAkdPXrUVZsDAACAk5wudv/617/sHl9++aVmz56txx9/XK1bt3Y6wMyZMxUWFiYfHx9FRETo559/vub806dPa9CgQapYsaKsVqvq1Kmjr7/+2unXBQAAMBunr4rt0qWL3bLFYlH58uXVrl07TZkyxaltLVmyRHFxcZo9e7YiIiI0bdo0xcTE6I8//lCFChXyzc/JyVGHDh1UoUIFffrpp6pcubIOHjyoUqVKOfs2AAAATMfpq2JdKSIiQnfeeadmzJghScrLy1NoaKieffZZjRw5Mt/82bNna/Lkydq5c2e+rzJzFFfFAgCAW0mhXhX7V4Zh6EZ7YU5OjjZv3qzo6Oj/hfHwUHR0tJKSkgpc51//+pciIyM1aNAgBQcHq2HDhnr99dev+TVm2dnZyszMtHsAAACY0Q0Vu4ULF6pRo0by9fWVr6+vGjdurA8//NCpbaSnpys3N1fBwcF248HBwUpNTS1wnX379unTTz9Vbm6uvv76a40ZM0ZTpkzRa6+9dtXXSUhIUFBQkO0RGhrqVE4AAIBbhdPn2E2dOlVjxozR4MGDbRdL/N///Z8GDBig9PR0DR8+3OUhL8vLy1OFChU0Z84ceXp6Kjw8XEeOHNHkyZMVHx9f4DqjRo1SXFycbTkzM5NyBwAATMnpYvfOO+9o1qxZdl8d9sADD6hBgwZ65ZVXHC525cqVk6enp9LS0uzG09LSFBISUuA6FStWlJeXlzw9PW1j9erVU2pqqnJycuTt7Z1vHavVKqvV6lAmAACAW5nTh2JTUlLUqlWrfOOtWrVSSkqKw9vx9vZWeHi4EhMTbWN5eXlKTExUZGRkgeu0bt1ae/bsUV5enm1s165dqlixYoGlDgAA4HbidLGrVauWli5dmm98yZIlql27tlPbiouL03vvvacFCxZox44deuaZZ5SVlaXY2FhJUu/evTVq1Cjb/GeeeUYnT57U0KFDtWvXLq1YsUKvv/66Bg0a5OzbAAAAMB2nD8WOGzdOPXr00Pfff287x27Dhg1KTEwssPBdS48ePXT8+HGNHTtWqampatq0qVauXGm7oOLQoUPy8Phf9wwNDdWqVas0fPhwNW7cWJUrV9bQoUP14osvOvs2AAAATOeG7mO3efNmvfXWW9qxY4ekS+e5Pffcc2rWrJnLA7oa97EDAAC3Eme6i1tvUOwOFDsAAHArKZQbFB89elQjRowo8Aa/GRkZev755/Nd4QoAAICi43Cxmzp1qjIzMwtsikFBQTpz5oymTp3q0nAAAABwnMPFbuXKlXb3rrtS79699e9//9sloQAAAOA8h4vd/v37VbVq1as+X6VKFR04cMAVmQAAAHADHC52vr6+1yxuBw4ckK+vrysyAQAA4AY4XOwiIiL04YcfXvX5hQsXqmXLli4JBQAAAOc5fIPiESNGqEOHDgoKCtLzzz9vu4lwWlqaJk2apPnz52v16tWFFhQAAADX5tR97P75z39q6NChunjxogIDA2WxWJSRkSEvLy+99dZbeuaZZwozq0twHzsAAHArKdQbFB85ckRLly7Vnj17ZBiG6tSpo4cfflhVqlS5qdBFhWIHAABuJXzzxDVQ7AAAwK2kUL55AgAAAMUbxQ4AAMAkKHYAAAAmQbEDAAAwiZsqdtnZ2a7KAQAAgJvkVLH75ptv1KdPH9WoUUNeXl7y8/NTYGCgoqKiNGHCBB09erSwcgIAAOA6HCp2n3/+uerUqaN+/fqpRIkSevHFF7V8+XKtWrVK77//vqKiorRmzRrVqFFDAwYM0PHjxws7NwAAAK7g0H3sIiMjNXr0aN17773y8Lh6Fzxy5IjeeecdBQcHa/jw4S4N6ircxw4AANxKuEHxNVDsAADArYQbFAMAANyGSjgyKS4uzuENTp069YbDAAAA4MY5VOy2bNlit5ycnKw///xTdevWlSTt2rVLnp6eCg8Pd31CAAAAOMShYrd27Vrbv6dOnaqAgAAtWLBApUuXliSdOnVKsbGxuvvuuwsnJQAAAK7L6YsnKleurNWrV6tBgwZ249u3b1fHjh2L/b3suHgCAADcSgr14onMzMwC71N3/PhxnTlzxtnNAQAAwEWcLnZdu3ZVbGysli9frv/+97/673//q88++0z9+/dXt27dCiMjAAAAHODQOXZ/NXv2bI0YMUK9evXSxYsXL22kRAn1799fkydPdnlAAAAAOOaGb1CclZWlvXv3SpJq1qypkiVLujRYYeEcOwAAcCspkhsUp6SkKCUlRbVr11bJkiV1m32BBQAAQLHjdLE7ceKE2rdvrzp16ui+++5TSkqKJKl///567rnnXB4QAAAAjnG62A0fPlxeXl46dOiQ/Pz8bOM9evTQypUrXRoOAAAAjnP64onVq1dr1apVqlKlit147dq1dfDgQZcFAwAAgHOc3mOXlZVlt6fuspMnT8pqtbokFAAAAJzndLG7++67tXDhQtuyxWJRXl6eJk2apLZt27o0HAAAABzn9KHYSZMmqX379tq0aZNycnL0wgsv6LffftPJkye1YcOGwsgIAAAABzhd7Bo2bKhdu3ZpxowZCggI0NmzZ9WtWzcNGjRIFStWLIyMgGmEjVzh7ghw0IE3Ork7AgA4zeliJ0lBQUF6+eWXXZ0FAG5LFP5bB4UfxZ3T59jVqFFDsbGxys7OthtPT09XjRo1XBYMAAAAznG62B04cEAbNmzQ3XffrdTUVNt4bm4utzsBAABwI6eLncVi0cqVK1WlShWFh4dr48aNhZELAAAATnK62BmGIX9/fy1fvly9e/dWVFSUPvroo8LIBgAAACc4ffGExWKx/TshIUENGjTQk08+qZ49e7o0GAAAAJzjdLEzDMNu+fHHH1fNmjXVtWtXl4UCAACA85wudnl5efnGIiMj9csvv2jnzp0uCQUAAADn3dB97AoSHBys4OBgV20OAAAATnKo2DVv3lyJiYkqXbq0mjVrZnee3ZWSk5NdFg4AAACOc6jYPfjgg7JarZKkLl26FGYeAAAA3CCHil18fHyB/wYAAEDx4fR97AAAAFA8ObTHrnTp0tc8r+6vTp48eVOBAAAAcGMcKnbTpk0r5BgAAAC4WQ4Vuz59+hR2DgAAANykm7qP3YULF5STk2M3FhgYeFOBAAAAcGOcvngiKytLgwcPVoUKFVSyZEmVLl3a7gEAAAD3cLrYvfDCC/ruu+80a9YsWa1Wvf/++xo3bpwqVaqkhQsXFkZGAAAAOMDpQ7FfffWVFi5cqDZt2ig2NlZ33323atWqpWrVqmnRokV67LHHCiMnAAAArsPpPXYnT55UjRo1JF06n+7y7U3uuusuff/9965NBwAAAIc5Xexq1Kih/fv3S5LuuOMOLV26VNKlPXmlSpVyaTgAAAA4zuliFxsbq19++UWSNHLkSM2cOVM+Pj4aPny4nn/+eZcHBAAAgGOcPsdu+PDhtn9HR0dr586d2rx5s2rVqqXGjRu7NBwAAAAcd1P3sZOkatWqqVq1aq7IAgAAgJtwQ8Vu48aNWrt2rY4dO6a8vDy756ZOneqSYAAAAHCO08Xu9ddf1+jRo1W3bl0FBwfLYrHYnvvrvwEAAFC0nC5206dP19y5c9W3b99CiAMAAIAb5fRVsR4eHmrdurVLQ8ycOVNhYWHy8fFRRESEfv75Z4fW++STT2SxWNSlSxeX5gEAALgVOV3shg8frpkzZ7oswJIlSxQXF6f4+HglJyerSZMmiomJ0bFjx6653oEDBzRixAjdfffdLssCAABwK3P6UOyIESPUqVMn1axZU/Xr15eXl5fd88uXL3dqe1OnTtWTTz6p2NhYSdLs2bO1YsUKzZ07VyNHjixwndzcXD322GMaN26cfvjhB50+fdrZtwEAAGA6Tu+xGzJkiNauXas6deqobNmyCgoKsns4IycnR5s3b1Z0dPT/Anl4KDo6WklJSVdd79VXX1WFChXUv39/Z+MDAACYltN77BYsWKDPPvtMnTp1uukXT09PV25uroKDg+3Gg4ODtXPnzgLX+b//+z998MEH2rp1q0OvkZ2drezsbNtyZmbmDecFAAAozpzeY1emTBnVrFmzMLJc15kzZ/SPf/xD7733nsqVK+fQOgkJCXZ7FENDQws5JQAAgHs4XexeeeUVxcfH69y5czf94uXKlZOnp6fS0tLsxtPS0hQSEpJv/t69e3XgwAF17txZJUqUUIkSJbRw4UL961//UokSJbR3795864waNUoZGRm2x+HDh286NwAAQHHk9KHYt99+W3v37lVwcLDCwsLyXTyRnJzs8La8vb0VHh6uxMRE2y1L8vLylJiYqMGDB+ebf8cdd2jbtm12Y6NHj9aZM2c0ffr0AvfGWa1WWa1WhzMBAADcqpwudq6+Z1xcXJz69OmjFi1aqGXLlpo2bZqysrJsV8n27t1blStXVkJCgnx8fNSwYUO79UuVKiVJ+cYBAABuN04Vuz///FMWi0X9+vVTlSpVXBKgR48eOn78uMaOHavU1FQ1bdpUK1eutF1QcejQIXl4OH3EGAAA4LZjMQzDcGaFgIAAbdu2TWFhYYUUqXBlZmYqKChIGRkZCgwMdHcc3GbCRq5wdwQ46MAbN3/lv6P4XNw6ivJzAVzmTHdxeldYu3bttH79+hsOBwAAgMLh9Dl29957r0aOHKlt27YpPDxcJUuWtHv+gQcecFk4AAAAOM7pYjdw4EBJl74K7EoWi0W5ubk3nwoAAABOc7rY5eXlFUYOAAAA3CQuNwUAADCJGyp269evV+fOnVWrVi3VqlVLDzzwgH744QdXZwMAAIATnC52H330kaKjo+Xn56chQ4ZoyJAh8vX1Vfv27bV48eLCyAgAAAAHOH2O3YQJEzRp0iQNHz7cNjZkyBBNnTpV48ePV69evVwaEAAAAI5xeo/dvn371Llz53zjDzzwgPbv3++SUAAAAHCe08UuNDRUiYmJ+cbXrFmj0NBQl4QCAACA85w+FPvcc89pyJAh2rp1q1q1aiVJ2rBhg+bPn6/p06e7PCAAAAAc43Sxe+aZZxQSEqIpU6Zo6dKlkqR69eppyZIlevDBB10eEAAAAI5xuthJUteuXdW1a1dXZwEAAMBNuKFiJ0k5OTk6duxYvm+iqFq16k2HAgAAgPOcLna7d+9Wv3799OOPP9qNG4bBd8UCAAC4kdPFrm/fvipRooT+/e9/q2LFirJYLIWRCwAAAE5yutht3bpVmzdv1h133FEYeQAAAHCDnL6PXf369ZWenl4YWQAAAHATnC52EydO1AsvvKB169bpxIkTyszMtHsAAADAPZw+FBsdHS1Jat++vd04F08AAAC4l9PFbu3atYWRAwAAADfJ6WIXFRVVGDkAAABwkxw6x+7QoUNObfTIkSM3FAYAAAA3zqFid+edd+rpp5/Wxo0brzonIyND7733nho2bKjPPvvMZQEBAADgGIcOxf7++++aMGGCOnToIB8fH4WHh6tSpUry8fHRqVOn9Pvvv+u3335T8+bNNWnSJN13332FnRsAAABXcGiPXdmyZTV16lSlpKRoxowZql27ttLT07V7925J0mOPPabNmzcrKSmJUgcAAOAmTl084evrq4cfflgPP/xwYeUBAADADXL6BsUAAAAonih2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACTKBbFbubMmQoLC5OPj48iIiL0888/X3Xue++9p7vvvlulS5dW6dKlFR0dfc35AAAAtwu3F7slS5YoLi5O8fHxSk5OVpMmTRQTE6Njx44VOH/dunXq2bOn1q5dq6SkJIWGhqpjx446cuRIEScHAAAoXtxe7KZOnaonn3xSsbGxql+/vmbPni0/Pz/NnTu3wPmLFi3SwIED1bRpU91xxx16//33lZeXp8TExCJODgAAULy4tdjl5ORo8+bNio6Oto15eHgoOjpaSUlJDm3j3LlzunjxosqUKVNYMQEAAG4JJdz54unp6crNzVVwcLDdeHBwsHbu3OnQNl588UVVqlTJrhz+VXZ2trKzs23LmZmZNx4YAACgGHP7odib8cYbb+iTTz7R559/Lh8fnwLnJCQkKCgoyPYIDQ0t4pQAAABFw63Frly5cvL09FRaWprdeFpamkJCQq657ptvvqk33nhDq1evVuPGja86b9SoUcrIyLA9Dh8+7JLsAAAAxY1bi523t7fCw8PtLny4fCFEZGTkVdebNGmSxo8fr5UrV6pFixbXfA2r1arAwEC7BwAAgBm59Rw7SYqLi1OfPn3UokULtWzZUtOmTVNWVpZiY2MlSb1791blypWVkJAgSZo4caLGjh2rxYsXKywsTKmpqZIkf39/+fv7u+19AAAAuJvbi12PHj10/PhxjR07VqmpqWratKlWrlxpu6Di0KFD8vD4347FWbNmKScnRw8//LDdduLj4/XKK68UZXQAAIBixe3FTpIGDx6swYMHF/jcunXr7JYPHDhQ+IEAAABuQbf0VbEAAAD4H4odAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDAAAwiRLuDgAAAPILG7nC3RHgoANvdHJ3BJtiUexmzpypyZMnKzU1VU2aNNE777yjli1bXnX+smXLNGbMGB04cEC1a9fWxIkTdd999xVhYsfwH+Wtozj9RwkAwI1y+6HYJUuWKC4uTvHx8UpOTlaTJk0UExOjY8eOFTj/xx9/VM+ePdW/f39t2bJFXbp0UZcuXbR9+/YiTg4AAFC8uL3YTZ06VU8++aRiY2NVv359zZ49W35+fpo7d26B86dPn6577rlHzz//vOrVq6fx48erefPmmjFjRhEnBwAAKF7cWuxycnK0efNmRUdH28Y8PDwUHR2tpKSkAtdJSkqymy9JMTExV50PAABwu3DrOXbp6enKzc1VcHCw3XhwcLB27txZ4DqpqakFzk9NTS1wfnZ2trKzs23LGRkZkqTMzMybie6QvOxzhf4acI2i+DxIfCZuJUX1mZD4XNxK+FygIIX9ubi8fcMwrju3WFw8UZgSEhI0bty4fOOhoaFuSIPiKmiauxOguOEzgYLwuUBBiupzcebMGQUFBV1zjluLXbly5eTp6am0tDS78bS0NIWEhBS4TkhIiFPzR40apbi4ONtyXl6eTp48qbJly8pisdzkO7i9ZGZmKjQ0VIcPH1ZgYKC746CY4HOBK/GZQEH4XNw4wzB05swZVapU6bpz3VrsvL29FR4ersTERHXp0kXSpeKVmJiowYMHF7hOZGSkEhMTNWzYMNvYt99+q8jIyALnW61WWa1Wu7FSpUq5Iv5tKzAwkP8okQ+fC1yJzwQKwufixlxvT91lbj8UGxcXpz59+qhFixZq2bKlpk2bpqysLMXGxkqSevfurcqVKyshIUGSNHToUEVFRWnKlCnq1KmTPvnkE23atElz5sxx59sAAABwO7cXux49euj48eMaO3asUlNT1bRpU61cudJ2gcShQ4fk4fG/i3dbtWqlxYsXa/To0XrppZdUu3ZtffHFF2rYsKG73gIAAECx4PZiJ0mDBw++6qHXdevW5Rt75JFH9MgjjxRyKlzJarUqPj4+36Ft3N74XOBKfCZQED4XRcNiOHLtLAAAAIo9t3/zBAAAAFyDYgcAAGASFDsAAACToNihQDNnzlRYWJh8fHwUERGhn3/+2fbchQsXNGjQIJUtW1b+/v566KGH8t00Gubz/fffq3PnzqpUqZIsFou++OILu+cNw9DYsWNVsWJF+fr6Kjo6Wrt373ZPWBSpa/29mDNnjtq0aaPAwEBZLBadPn3afUFRJK73t2L58uXq2LGj7YsCtm7d6pacZkWxQz5LlixRXFyc4uPjlZycrCZNmigmJkbHjh2TJA0fPlxfffWVli1bpvXr1+vo0aPq1q2bm1OjsGVlZalJkyaaOXNmgc9PmjRJb7/9tmbPnq2ffvpJJUuWVExMjC5cuFDESVGUrvf34ty5c7rnnnv00ksvuTkpisr1/lZkZWXprrvu0sSJE4s42W3CAK7QsmVLY9CgQbbl3Nxco1KlSkZCQoJx+vRpw8vLy1i2bJnt+R07dhiSjKSkJHfEhRtIMj7//HPbcl5enhESEmJMnjzZNnb69GnDarUaH3/8sRsSoqhc6+/FX61du9aQZJw6daqIE8Kdrvxb8Vf79+83JBlbtmwp0kxmxx472MnJydHmzZsVHR1tG/Pw8FB0dLSSkpK0efNmXbx40e75O+64Q1WrVlVSUpI7IqMY2L9/v1JTU+0+F0FBQYqIiOBzYWLX+3sBoOhR7GAnPT1dubm5tm/+uCw4OFipqalKTU2Vt7d3vu/bvfw8bk+Xf/dX+9zAnK739wJA0aPYAQAAmATFDnbKlSsnT0/PfFe5pqWlKSQkRCEhIcrJycl3Zdvl53F7uvy7v9rnBuZ0vb8XAIoexQ52vL29FR4ersTERNtYXl6eEhMTFRkZqfDwcHl5edk9/8cff+jQoUOKjIx0R2QUA9WrV1dISIjd5yIzM1M//fQTnwsTu97fCwBFr4S7A6D4iYuLU58+fdSiRQu1bNlS06ZNU1ZWlmJjYxUUFKT+/fsrLi5OZcqUUWBgoJ599llFRkbqb3/7m7ujoxCdPXtWe/bssS3v379fW7duVZkyZVS1alUNGzZMr732mmrXrq3q1atrzJgxqlSpkrp06eK+0Ch01/p7Icl2bu7lz862bdsUEBCgqlWrqkyZMu6MjkJyvb8VJ0+e1KFDh3T06FFJl3YOSLIdFcJNcvdluSie3nnnHaNq1aqGt7e30bJlS+M///mP7bnz588bAwcONEqXLm34+fkZXbt2NVJSUtyYFkXh8u0qrnz06dPHMIxLtzwZM2aMERwcbFitVqN9+/bGH3/84d7QKBLX+nsRHx9f4Odm3rx57guMQnW9vxXz5s0r8Pn4+Hi35jYLi2EYRtFWSQAAABQGzrEDAAAwCYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDABdp06aNhg0bdtPbCQsL07Rp0256O444cOCALBaLtm7dWiSvB6BwUewAuEzfvn1lsVg0YMCAfM8NGjRIFotFffv2LfpgxcT8+fNlsVhsD39/f4WHh2v58uV28zZu3KinnnrKtmyxWPTFF1849TqlSpVyaG5oaKhSUlLUsGFDh7cPoPii2AFwqdDQUH3yySc6f/68bezChQtavHixqlat6sZkjsnJySnU7QcGBiolJUUpKSnasmWLYmJi1L17d9sXoUtS+fLl5efnV6g5pEvv1dPTUyEhISpRokShvx6AwkexA+BSzZs3V2hoqN1eqOXLl6tq1apq1qyZ3dy8vDwlJCSoevXq8vX1VZMmTfTpp5/ans/NzVX//v1tz9etW1fTp0+328a6devUsmVLlSxZUqVKlVLr1q118OBBSZf2IHbp0sVu/rBhw9SmTRvbcps2bTR48GANGzZM5cqVU0xMjCRp+/btuvfee+Xv76/g4GD94x//UHp6um29rKws9e7dW/7+/qpYsaKmTJni0M/HYrEoJCREISEhql27tl577TV5eHjo119/tc3566HYsLAwSVLXrl1lsVhsy7/88ovatm2rgIAABQYGKjw8XJs2bdK6desUGxurjIwM257BV155xbat8ePHq3fv3goMDNRTTz2V71DsunXrZLFYlJiYqBYtWsjPz0+tWrWyK56S9Nprr6lChQoKCAjQE088oZEjR6pp06YO/QwAFB6KHQCX69evn+bNm2dbnjt3rmJjY/PNS0hI0MKFCzV79mz99ttvGj58uB5//HGtX79e0qXiV6VKFS1btky///67xo4dq5deeklLly6VJP3555/q0qWLoqKi9OuvvyopKUlPPfWULBaLU3kXLFggb29vbdiwQbNnz9bp06fVrl07NWvWTJs2bdLKlSuVlpam7t2729Z5/vnntX79en355ZdavXq11q1bp+TkZKdeNzc3VwsWLJB0qRAXZOPGjZKkefPmKSUlxbb82GOPqUqVKtq4caM2b96skSNHysvLS61atdK0adPs9gyOGDHCtr0333xTTZo00ZYtWzRmzJirZnv55Zc1ZcoUbdq0SSVKlFC/fv1szy1atEgTJkzQxIkTtXnzZlWtWlWzZs1y6r0DKCQGALhInz59jAcffNA4duyYYbVajQMHDhgHDhwwfHx8jOPHjxsPPvig0adPH8MwDOPChQuGn5+f8eOPP9pto3///kbPnj2v+hqDBg0yHnroIcMwDOPEiROGJGPdunXXzPNXQ4cONaKiomzLUVFRRrNmzezmjB8/3ujYsaPd2OHDhw1Jxh9//GGcOXPG8Pb2NpYuXWp7/sSJE4avr68xdOjQq2afN2+eIckoWbKkUbJkScPDw8OwWq3GvHnz7OZVq1bNeOutt2zLkozPP//cbk5AQIAxf/78q75OUFBQvvFq1aoZXbp0sRvbv3+/IcnYsmWLYRiGsXbtWkOSsWbNGtucFStWGJKM8+fPG4ZhGBEREcagQYPsttO6dWujSZMmV33vAIoGJ1UAcLny5curU6dOmj9/vgzDUKdOnVSuXDm7OXv27NG5c+fUoUMHu/GcnBy7Q7YzZ87U3LlzdejQIZ0/f145OTm2Q35lypRR3759FRMTow4dOig6Olrdu3dXxYoVncobHh5ut/zLL79o7dq18vf3zzd37969thwRERG28TJlyqhu3brXfa2AgADbnr1z585pzZo1GjBggMqWLavOnTs7nDkuLk5PPPGEPvzwQ0VHR+uRRx5RzZo1r7teixYtHNp+48aNbf++/PM8duyYqlatqj/++EMDBw60m9+yZUt99913DucHUDgodgAKRb9+/TR48GBJl8rZlc6ePStJWrFihSpXrmz3nNVqlSR98sknGjFihKZMmaLIyEgFBARo8uTJ+umnn2xz582bpyFDhmjlypVasmSJRo8erW+//VZ/+9vf5OHhIcMw7LZ98eLFfFlKliyZL1vnzp01ceLEfHMrVqyoPXv2OPIjKJCHh4dq1aplW27cuLFWr16tiRMnOlXsXnnlFfXq1UsrVqzQN998o/j4eH3yySfq2rXrNde78r1ejZeXl+3flw9t5+XlOZwPgHtwjh2AQnHPPfcoJydHFy9etF2Q8Ff169eX1WrVoUOHVKtWLbtHaGioJGnDhg1q1aqVBg4cqGbNmqlWrVrau3dvvm01a9ZMo0aN0o8//qiGDRtq8eLFki7tOUxJSbGb68j92po3b67ffvtNYWFh+bKVLFlSNWvWlJeXl13BPHXqlHbt2uXMj8jG09PT7iriK3l5eSk3NzffeJ06dTR8+HCtXr1a3bp1s53X6O3tXeB8V6lbt67tXL/LrlwG4B4UOwCFwtPTUzt27NDvv/8uT0/PfM8HBARoxIgRGj58uBYsWKC9e/cqOTlZ77zzju2Cgtq1a2vTpk1atWqVdu3apTFjxtgViP3792vUqFFKSkrSwYMHtXr1au3evVv16tWTJLVr106bNm3SwoULtXv3bsXHx2v79u3XzT5o0CCdPHlSPXv21MaNG7V3716tWrVKsbGxys3Nlb+/v/r376/nn39e3333nbZv366+ffvKw+P6f1INw1BqaqpSU1O1f/9+zZkzR6tWrdKDDz541XXCwsKUmJio1NRUnTp1SufPn9fgwYO1bt06HTx4UBs2bNDGjRtt7zssLExnz55VYmKi0tPTde7cuevmcsazzz6rDz74QAsWLNDu3bv12muv6ddff3X6ohUArsehWACFJjAw8JrPjx8/XuXLl1dCQoL27dunUqVKqXnz5nrppZckSU8//bS2bNmiHj16yGKxqGfPnho4cKC++eYbSZKfn5927typBQsW6MSJE6pYsaIGDRqkp59+WpIUExOjMWPG6IUXXtCFCxfUr18/9e7dW9u2bbtmrkqVKmnDhg168cUX1bFjR2VnZ6tatWq65557bOVt8uTJtkO2AQEBeu6555SRkXHdn0lmZqbtnDWr1apq1arp1Vdf1YsvvnjVdaZMmaK4uDi99957qly5snbt2qUTJ06od+/eSktLU7ly5dStWzeNGzdOktSqVSsNGDBAPXr00IkTJxQfH2+75YkrPPbYY9q3b59GjBihCxcuqHv37urbt69+/vlnl70GgBtjMa48AQUAACd16NBBISEh+vDDD90dBbitsccOAOCUc+fOafbs2YqJiZGnp6c+/vhjrVmzRt9++627owG3PfbYAQCccv78eXXu3FlbtmzRhQsXVLduXY0ePVrdunVzdzTgtkexAwAAMAmuigUAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADCJ/wfzLvVasueAXAAAAABJRU5ErkJggg==\n",
+                        "image/png": "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LHCbmTlzpr7//nt9//33+vjjj9WuXTs98cQTWr58ubXPsmXLFBgYqI4dOyo9Pd36CgsLk5+fn9auXXvTdTRo0EDJycl6/PHHdeDAAc2YMUNdu3ZVUFCQ3n//fbv24eXlJTe3Sx9jubm5OnHihPz8/FS3bl0lJSVdd/vk5GTt3r1bvXv31okTJ6zvMysrSx06dNCPP/6ovLy86+7nqaeesv5O//6qX7++tY+vr6/mz5+vHTt26O6779aKFSv01ltvqWrVqvn2FxERobCwMOty1apV9eCDD2rVqlXKzc2VYRj6/PPP1aVLFxmGYfM3io6OVkZGRr7337dvX/n4+Fz3vUiXrog9+uij1uW6deuqVKlSqlevnsLDw63tl3/et2+fJN1QXTExMTZXDy9fUb28TwCO4VYscJtp2bKlzeCJXr16qVmzZhoyZIjuv/9+eXp6avfu3crIyLB51u3vnDW4oU6dOvroo4+Um5urP/74Q//+9781efJkPfXUU6pevbqioqKuuX1eXp5mzJih9957T/v371dubq51XdmyZa97/N27d0u6FHquJiMjQ6VLl77mfmrXrn3dWiWpdevWeuaZZzRz5kxFR0erf//+V93flerUqaNz587p+PHjcnNz0+nTpzVnzhzNmTOnwH1c+TeqXr36deu7rEqVKrJYLDZtgYGBCgkJydcmyfrc5fHjxx2u68pge/l37axnOYHbDcEOuM25ubmpXbt2mjFjhnbv3q0GDRooLy9PFSpU0KJFiwrcpnz58k6twd3dXY0aNVKjRo0UERGhdu3aadGiRdcNS6+//rrGjh2r/v37a8KECSpTpozc3Nw0fPhwu660Xe4zZcqUq06D4sznubKzs60DFfbu3atz587J19fX4f1crvvxxx+/aiht3LixzbK9V+ukS38PR9oNw7jhuq63TwCOIdgB0F9//SVJOnv2rCSpZs2aWrNmjVq3bu1QIHCGy1cTU1JSrG1XXj267LPPPlO7du304Ycf2rSfPn1a5cqVu+72NWvWlCQFBATYdcXtZsXFxWnHjh1688039eKLL2rUqFF6++238/W7fCXx73bt2iVfX19rqPb391dubm6R1G2v8uXLF0pdV/v7AciPZ+yA29zFixe1evVqeXp6ql69epKkHj16KDc3VxMmTMjX/6+//tLp06dv+rg//fSTLl68mK/922+/lXTpua7LSpYsWeAx3d3d813ZWbZsmY4cOWLTVrJkSUnKt4+wsDDVrFlTb775pjXU/t3x48ftei/2+OWXX/Tmm29q+PDheu655/T888/r3Xff1fr16/P1TUxMtHkW7fDhw/rqq6/UqVMnubu7y93dXQ899JA+//xzbd++vVDrdkRh1VWyZEllZGTcbHnAbYErdsBt5rvvvtPOnTslXXreafHixdq9e7dGjRqlgIAASVJkZKSefvppxcfHKzk5WZ06dZKHh4d2796tZcuWacaMGXr44Ydvqo5JkyZpy5Yt6t69u/X2XFJSkhYuXKgyZcrYTIsRFhamWbNm6bXXXlOtWrVUoUIFtW/fXvfff79effVVxcTEqFWrVtq2bZsWLVqkGjVq2ByrZs2aKlWqlGbPni1/f3+VLFlS4eHhql69uj744APde++9atCggWJiYlS5cmUdOXJEa9euVUBAgL755pvrvpekpCR9/PHH+dpr1qypiIgIXbhwQX379lXt2rU1ceJESdL48eP1zTffKCYmRtu2bbOGT0lq2LChoqOjbaY7ubzNZW+88YbWrl2r8PBwPfnkk6pfv75OnjyppKQkrVmzRidPnrT/j+FEhVFXWFiYlixZotjYWN15553y8/NTly5dCqF6wARcOCIXQBEqaLoTb29vo2nTpsasWbNspvu4bM6cOUZYWJjh4+Nj+Pv7G40aNTJeeOEF4+jRo9Y+NzrdyYYNG4zBgwcbDRs2NAIDAw0PDw+jatWqRr9+/Yy9e/fa9E1NTTU6d+5s+Pv7G5Ksx7tw4YLx3HPPGRUrVjR8fHyM1q1bG4mJiflqMgzD+Oqrr4z69esbJUqUyFff1q1bje7duxtly5Y1vLy8jGrVqhk9evQwEhISrvkerjfdSd++fQ3DMIwRI0YY7u7uxi+//GKz/ebNm40SJUoYzzzzjLVNkjF48GDj448/NmrXrm14eXkZzZo1s5mS5LK0tDRj8ODBRkhIiOHh4WEEBwcbHTp0MObMmWPtc3lakWXLluXb/mrTnTRo0CBf32rVqhmdO3fO1365XmfVVdD5c/bsWaN3795GqVKlDElMfQJcg8UweEIVAIoLi8WiwYMH691333V1KQBuQTxjBwAAYBIEOwAAAJMg2AEAAJiES4Pdjz/+qC5duqhSpUqyWCz68ssvr7vNunXr1Lx5c3l5ealWrVqaP39+odcJAEXFMAyerwNww1wa7LKystSkSRPNnDnTrv779+9X586d1a5dOyUnJ2v48OF64okntGrVqkKuFAAAoPgrNqNiLRaLvvjiC3Xt2vWqfV588UWtWLHCZuLLRx99VKdPn9bKlSuLoEoAAIDi65aaoDgxMTHf19RER0fbTGR6pezsbGVnZ1uX8/LydPLkSZUtW5avqQEAAMWeYRg6c+aMKlWqJDe3a99svaWCXWpqqoKCgmzagoKClJmZqfPnzxf4nZbx8fE2s7UDAADcig4fPqwqVapcs88tFexuxOjRoxUbG2tdzsjIUNWqVXX48GHr1ycBAAAUV5mZmQoJCZG/v/91+95SwS44OFhpaWk2bWlpaQoICCjwap0keXl5ycvLK197QEAAwQ4AANwy7HmE7Jaaxy4iIkIJCQk2bd9//70iIiJcVBEAAEDx4dJgd/bsWSUnJys5OVnSpelMkpOTdejQIUmXbqP26dPH2n/gwIHat2+fXnjhBe3cuVPvvfeeli5dqhEjRriifAAAgGLFpcFu8+bNatasmZo1ayZJio2NVbNmzTRu3DhJUkpKijXkSVL16tW1YsUKff/992rSpImmTp2qDz74QNHR0S6pHwAAoDgpNvPYFZXMzEwFBgYqIyODZ+wAAECx50h2uaWesQMAAMDVEewAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMwuXBbubMmQoNDZW3t7fCw8O1cePGa/afPn266tatKx8fH4WEhGjEiBG6cOFCEVULAABQfLk02C1ZskSxsbGKi4tTUlKSmjRpoujoaB07dqzA/osXL9aoUaMUFxenHTt26MMPP9SSJUv00ksvFXHlAAAAxY9Lg920adP05JNPKiYmRvXr19fs2bPl6+uruXPnFtj/559/VuvWrdW7d2+FhoaqU6dO6tWr13Wv8gEAANwOXBbscnJytGXLFkVFRf2vGDc3RUVFKTExscBtWrVqpS1btliD3L59+/Ttt9/qvvvuu+pxsrOzlZmZafMCAAAwoxKuOnB6erpyc3MVFBRk0x4UFKSdO3cWuE3v3r2Vnp6uu+66S4Zh6K+//tLAgQOveSs2Pj5e48ePd2rtAAAAxZHLB084Yt26dXr99df13nvvKSkpScuXL9eKFSs0YcKEq24zevRoZWRkWF+HDx8uwooBAACKjsuu2JUrV07u7u5KS0uzaU9LS1NwcHCB24wdO1b//Oc/9cQTT0iSGjVqpKysLD311FN6+eWX5eaWP6d6eXnJy8vL+W8AAACgmHHZFTtPT0+FhYUpISHB2paXl6eEhARFREQUuM25c+fyhTd3d3dJkmEYhVcsAADALcBlV+wkKTY2Vn379lWLFi3UsmVLTZ8+XVlZWYqJiZEk9enTR5UrV1Z8fLwkqUuXLpo2bZqaNWum8PBw7dmzR2PHjlWXLl2sAQ8AAOB25dJg17NnTx0/flzjxo1TamqqmjZtqpUrV1oHVBw6dMjmCt2YMWNksVg0ZswYHTlyROXLl1eXLl00ceJEV70FAACAYsNi3Gb3MDMzMxUYGKiMjAwFBAS4uhwAAIBrciS73FKjYgEAAHB1BDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEncdLDLzMzUl19+qR07djijHgAAANwgh4Ndjx499O6770qSzp8/rxYtWqhHjx5q3LixPv/8c6cXCAAAAPs4HOx+/PFHtWnTRpL0xRdfyDAMnT59Wm+//bZee+01pxcIAAAA+zgc7DIyMlSmTBlJ0sqVK/XQQw/J19dXnTt31u7du51eIAAAAOzjcLALCQlRYmKisrKytHLlSnXq1EmSdOrUKXl7ezu9QAAAANinhKMbDB8+XI899pj8/PxUrVo1tW3bVtKlW7SNGjVydn0AAACwk8PBbtCgQQoPD9ehQ4fUsWNHublduuhXo0YNTZw40ekFAgAAwD4O34p99dVXVa9ePXXr1k1+fn7W9vbt22vNmjVOLQ4AAAD2sxiGYTiygbu7u1JSUlShQgWb9hMnTqhChQrKzc11aoHOlpmZqcDAQGVkZCggIMDV5QAAAFyTI9nF4St2hmHIYrHka//111+to2UBAABQ9Ox+xq506dKyWCyyWCyqU6eOTbjLzc3V2bNnNXDgwEIpEgAAANdnd7CbPn26DMNQ//79NX78eAUGBlrXeXp6KjQ0VBEREYVSJAAAAK7P7mDXt29fSVL16tXVqlUreXh4FFpRAAAAcJzD051ERkYqLy9Pu3bt0rFjx5SXl2ez/u6773ZacQAAALCfw8HuP//5j3r37q2DBw/qygG1Foul2I+KBQAAMCuHg93AgQPVokULrVixQhUrVixwhCwAAACKnsPBbvfu3frss89Uq1atwqgHAAAAN8jheezCw8O1Z8+ewqgFAAAAN8HhK3bPPvusnnvuOaWmpqpRo0b5Rsc2btzYacUBAADAfg5/pZibW/6LfBaLxfqNFMV98ARfKQYAAG4ljmQXh6/Y7d+//4YLAwAAQOFxONhVq1atMOoAAADATXI42C1cuPCa6/v06XPDxQAAAODGOfyMXenSpW2WL168qHPnzsnT01O+vr46efKkUwt0Np6xAwAAtxJHsovD052cOnXK5nX27Fn9+eefuuuuu/TJJ5/ccNEAAAC4OQ4Hu4LUrl1bb7zxhoYNG+aM3QEAAOAGOCXYSVKJEiV09OhRZ+0OAAAADnI42H399dc2r6+++kqzZ8/W448/rtatWztcwMyZMxUaGipvb2+Fh4dr48aN1+x/+vRpDR48WBUrVpSXl5fq1Kmjb7/91uHjAgAAmI3Do2K7du1qs2yxWFS+fHm1b99eU6dOdWhfS5YsUWxsrGbPnq3w8HBNnz5d0dHR+vPPP1WhQoV8/XNyctSxY0dVqFBBn332mSpXrqyDBw+qVKlSjr4NAAAA03F4VKwzhYeH684779S7774rScrLy1NISIieffZZjRo1Kl//2bNna8qUKdq5c2e+rzKzF6NiAQDAraRQR8X+nWEYutFcmJOToy1btigqKup/xbi5KSoqSomJiQVu8/XXXysiIkKDBw9WUFCQGjZsqNdff/2aX2OWnZ2tzMxMmxcAAIAZ3VCwW7hwoRo1aiQfHx/5+PiocePG+uijjxzaR3p6unJzcxUUFGTTHhQUpNTU1AK32bdvnz777DPl5ubq22+/1dixYzV16lS99tprVz1OfHy8AgMDra+QkBCH6gQAALhVOPyM3bRp0zR27FgNGTLEOlji//7v/zRw4EClp6drxIgRTi/ysry8PFWoUEFz5syRu7u7wsLCdOTIEU2ZMkVxcXEFbjN69GjFxsZalzMzMwl3AADAlBwOdu+8845mzZpl89VhDzzwgBo0aKBXXnnF7mBXrlw5ubu7Ky0tzaY9LS1NwcHBBW5TsWJFeXh4yN3d3dpWr149paamKicnR56envm28fLykpeXl101AQAA3MocvhWbkpKiVq1a5Wtv1aqVUlJS7N6Pp6enwsLClJCQYG3Ly8tTQkKCIiIiCtymdevW2rNnj/Ly8qxtu3btUsWKFQsMdQAAALcTh4NdrVq1tHTp0nztS5YsUe3atR3aV2xsrN5//30tWLBAO3bs0DPPPKOsrCzFxMRIkvr06aPRo0db+z/zzDM6efKkhg0bpl27dmnFihV6/fXXNXjwYEffBgAAgOk4fCt2/Pjx6tmzp3788UfrM3YbNmxQQkJCgYHvWnr27Knjx49r3LhxSk1NVdOmTbVy5UrrgIpDhw7Jze1/2TMkJESrVq3SiBEj1LhxY1WuXFnDhg3Tiy++6OjbAAAAMJ0bmsduy5Yteuutt7Rjxw5Jl55ze+6559SsWTOnF+hszGMHAABuJY5kF5dOUOwKBDsAAHArKZQJio8ePaqRI0cWOMFvRkaGnn/++XwjXAEAAFB07A5206ZNU2ZmZoFJMTAwUGfOnNG0adOcWhwAAADsZ3ewW7lypc3cdVfq06eP/v3vfzulKAAAADjO7mC3f/9+Va1a9arrq1SpogMHDjijJgAAANwAu4Odj4/PNYPbgQMH5OPj44yaAAAAcAPsDnbh4eH66KOPrrp+4cKFatmypVOKAgAAgOPsnqB45MiR6tixowIDA/X8889bJxFOS0vT5MmTNX/+fK1evbrQCgUAAMC1OTSP3b/+9S8NGzZMFy9eVEBAgCwWizIyMuTh4aG33npLzzzzTGHW6hTMYwcAAG4lhTpB8ZEjR7R06VLt2bNHhmGoTp06evjhh1WlSpWbKrqoEOwAAMCthG+euAaCHQAAuJUUyjdPAAAAoHgj2AEAAJgEwQ4AAMAkCHYAAAAmcVPBLjs721l1AAAA4CY5FOy+++479e3bVzVq1JCHh4d8fX0VEBCgyMhITZw4UUePHi2sOgEAAHAddgW7L774QnXq1FH//v1VokQJvfjii1q+fLlWrVqlDz74QJGRkVqzZo1q1KihgQMH6vjx44VdNwAAAK5g1zx2ERERGjNmjO699165uV09Cx45ckTvvPOOgoKCNGLECKcW6izMYwcAAG4lTFB8DQQ7AABwK2GCYgAAgNtQCXs6xcbG2r3DadOm3XAxAAAAuHF2BbutW7faLCclJemvv/5S3bp1JUm7du2Su7u7wsLCnF8hAAAA7GJXsFu7dq3152nTpsnf318LFixQ6dKlJUmnTp1STEyM2rRpUzhVAgAA4LocHjxRuXJlrV69Wg0aNLBp3759uzp16lTs57Jj8AQAALiVFOrgiczMzALnqTt+/LjOnDnj6O4AAADgJA4Hu27duikmJkbLly/Xf//7X/33v//V559/rgEDBqh79+6FUSMAAADsYNczdn83e/ZsjRw5Ur1799bFixcv7aRECQ0YMEBTpkxxeoEAAACwzw1PUJyVlaW9e/dKkmrWrKmSJUs6tbDCwjN2AADgVlIkExSnpKQoJSVFtWvXVsmSJXWbfYEFAABAseNwsDtx4oQ6dOigOnXq6L777lNKSookacCAAXruueecXiAAAADs43CwGzFihDw8PHTo0CH5+vpa23v27KmVK1c6tTgAAADYz+HBE6tXr9aqVatUpUoVm/batWvr4MGDTisMAAAAjnH4il1WVpbNlbrLTp48KS8vL6cUBQAAAMc5HOzatGmjhQsXWpctFovy8vI0efJktWvXzqnFAQAAwH4O34qdPHmyOnTooM2bNysnJ0cvvPCCfv/9d508eVIbNmwojBoBAABgB4ev2DVs2FC7du3SXXfdpQcffFBZWVnq3r27tm7dqpo1axZGjQAAALDDDU9QfKtigmIAAHArcSS7OHwrtkaNGoqMjNTs2bNtBkukp6erZcuW2rdvn+MVA7eJ0FErXF0C7HTgjc5FdizOi1tHUZ4XwI1w+FbsgQMHtGHDBrVp00apqanW9tzcXKY7AQAAcCGHg53FYtHKlStVpUoVhYWFadOmTYVRFwAAABzkcLAzDEN+fn5avny5+vTpo8jISH388ceFURsAAAAc4PAzdhaLxfpzfHy8GjRooCeffFK9evVyamEAAABwjMPB7spBtI8//rhq1qypbt26Oa0oAAAAOM7hYJeXl5evLSIiQr/++qt27tzplKIAAADgOIeD3dUEBQUpKCjIWbsDAACAg+wKds2bN1dCQoJKly6tZs2a2Txnd6WkpCSnFQcAAAD72RXsHnzwQetkxF27di3MegAAAHCD7Ap2cXFxBf4MAACA4sPheewAAABQPNl1xa506dLXfK7u706ePHlTBQEAAODG2BXspk+fXshlAAAA4GbZFez69u1b2HUAAADgJt3UPHYXLlxQTk6OTVtAQMBNFQQAAIAb4/DgiaysLA0ZMkQVKlRQyZIlVbp0aZsXAAAAXMPhYPfCCy/ohx9+0KxZs+Tl5aUPPvhA48ePV6VKlbRw4cLCqBEAAAB2cPhW7DfffKOFCxeqbdu2iomJUZs2bVSrVi1Vq1ZNixYt0mOPPVYYdQIAAOA6HL5id/LkSdWoUUPSpefpLk9vctddd+nHH390bnUAAACwm8PBrkaNGtq/f78k6Y477tDSpUslXbqSV6pUKacWBwAAAPs5HOxiYmL066+/SpJGjRqlmTNnytvbWyNGjNDzzz/v9AIBAABgH4efsRsxYoT156ioKO3cuVNbtmxRrVq11LhxY6cWBwAAAPvd1Dx2klStWjVVq1bNGbUAAADgJtxQsNu0aZPWrl2rY8eOKS8vz2bdtGnTnFIYAAAAHONwsHv99dc1ZswY1a1bV0FBQbJYLNZ1f/8ZAAAARcvhYDdjxgzNnTtX/fr1K4RyAAAAcKMcHhXr5uam1q1bO7WImTNnKjQ0VN7e3goPD9fGjRvt2u7TTz+VxWJR165dnVoPAADArcjhYDdixAjNnDnTaQUsWbJEsbGxiouLU1JSkpo0aaLo6GgdO3bsmtsdOHBAI0eOVJs2bZxWCwAAwK3M4VuxI0eOVOfOnVWzZk3Vr19fHh4eNuuXL1/u0P6mTZumJ598UjExMZKk2bNna8WKFZo7d65GjRpV4Da5ubl67LHHNH78eP300086ffq0o28DAADAdBy+Yjd06FCtXbtWderUUdmyZRUYGGjzckROTo62bNmiqKio/xXk5qaoqCglJiZedbtXX31VFSpU0IABAxwtHwAAwLQcvmK3YMECff755+rcufNNHzw9PV25ubkKCgqyaQ8KCtLOnTsL3Ob//u//9OGHHyo5OdmuY2RnZys7O9u6nJmZecP1AgAAFGcOX7ErU6aMatasWRi1XNeZM2f0z3/+U++//77KlStn1zbx8fE2VxRDQkIKuUoAAADXcDjYvfLKK4qLi9O5c+du+uDlypWTu7u70tLSbNrT0tIUHBycr//evXt14MABdenSRSVKlFCJEiW0cOFCff311ypRooT27t2bb5vRo0crIyPD+jp8+PBN1w0AAFAcOXwr9u2339bevXsVFBSk0NDQfIMnkpKS7N6Xp6enwsLClJCQYJ2yJC8vTwkJCRoyZEi+/nfccYe2bdtm0zZmzBidOXNGM2bMKPBqnJeXl7y8vOyuCQAA4FblcLBz9pxxsbGx6tu3r1q0aKGWLVtq+vTpysrKso6S7dOnjypXrqz4+Hh5e3urYcOGNtuXKlVKkvK1AwAA3G4cCnZ//fWXLBaL+vfvrypVqjilgJ49e+r48eMaN26cUlNT1bRpU61cudI6oOLQoUNyc3P4jjEAAMBtx2IYhuHIBv7+/tq2bZtCQ0MLqaTClZmZqcDAQGVkZCggIMDV5eA2EzpqhatLgJ0OvHHzI//txXlx6yjK8wK4zJHs4vClsPbt22v9+vU3XBwAAAAKh8PP2N17770aNWqUtm3bprCwMJUsWdJm/QMPPOC04gAAAGA/h4PdoEGDJF36KrArWSwW5ebm3nxVAAAAcJjDwS4vL68w6gAAAMBNYrgpAACASdxQsFu/fr26dOmiWrVqqVatWnrggQf0008/Obs2AAAAOMDhYPfxxx8rKipKvr6+Gjp0qIYOHSofHx916NBBixcvLowaAQAAYAeHn7GbOHGiJk+erBEjRljbhg4dqmnTpmnChAnq3bu3UwsEAACAfRy+Yrdv3z516dIlX/sDDzyg/fv3O6UoAAAAOM7hYBcSEqKEhIR87WvWrFFISIhTigIAAIDjHL4V+9xzz2no0KFKTk5Wq1atJEkbNmzQ/PnzNWPGDKcXCAAAAPs4HOyeeeYZBQcHa+rUqVq6dKkkqV69elqyZIkefPBBpxcIAAAA+zgc7CSpW7du6tatm7NrAQAAwE24oWAnSTk5OTp27Fi+b6KoWrXqTRcFAAAAxzkc7Hbv3q3+/fvr559/tmk3DIPvigUAAHAhh4Ndv379VKJECf373/9WxYoVZbFYCqMuAAAAOMjhYJecnKwtW7bojjvuKIx6AAAAcIMcnseufv36Sk9PL4xaAAAAcBMcDnaTJk3SCy+8oHXr1unEiRPKzMy0eQEAAMA1HL4VGxUVJUnq0KGDTTuDJwAAAFzL4WC3du3awqgDAAAAN8nhYBcZGVkYdQAAAOAm2fWM3aFDhxza6ZEjR26oGAAAANw4u4LdnXfeqaefflqbNm26ap+MjAy9//77atiwoT7//HOnFQgAAAD72HUr9o8//tDEiRPVsWNHeXt7KywsTJUqVZK3t7dOnTqlP/74Q7///ruaN2+uyZMn67777ivsugEAAHAFu67YlS1bVtOmTVNKSoreffdd1a5dW+np6dq9e7ck6bHHHtOWLVuUmJhIqAMAAHARhwZP+Pj46OGHH9bDDz9cWPUAAADgBjk8QTEAAACKJ4IdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkikWwmzlzpkJDQ+Xt7a3w8HBt3Ljxqn3ff/99tWnTRqVLl1bp0qUVFRV1zf4AAAC3C5cHuyVLlig2NlZxcXFKSkpSkyZNFB0drWPHjhXYf926derVq5fWrl2rxMREhYSEqFOnTjpy5EgRVw4AAFC8uDzYTZs2TU8++aRiYmJUv359zZ49W76+vpo7d26B/RctWqRBgwapadOmuuOOO/TBBx8oLy9PCQkJRVw5AABA8eLSYJeTk6MtW7YoKirK2ubm5qaoqCglJibatY9z587p4sWLKlOmTGGVCQAAcEso4cqDp6enKzc3V0FBQTbtQUFB2rlzp137ePHFF1WpUiWbcPh32dnZys7Oti5nZmbeeMEAAADFmMtvxd6MN954Q59++qm++OILeXt7F9gnPj5egYGB1ldISEgRVwkAAFA0XBrsypUrJ3d3d6Wlpdm0p6WlKTg4+Jrbvvnmm3rjjTe0evVqNW7c+Kr9Ro8erYyMDOvr8OHDTqkdAACguHFpsPP09FRYWJjNwIfLAyEiIiKuut3kyZM1YcIErVy5Ui1atLjmMby8vBQQEGDzAgAAMCOXPmMnSbGxserbt69atGihli1bavr06crKylJMTIwkqU+fPqpcubLi4+MlSZMmTdK4ceO0ePFihYaGKjU1VZLk5+cnPz8/l70PAAAAV3N5sOvZs6eOHz+ucePGKTU1VU2bNtXKlSutAyoOHTokN7f/XVicNWuWcnJy9PDDD9vsJy4uTq+88kpRlg4AAFCsuDzYSdKQIUM0ZMiQAtetW7fOZvnAgQOFXxAAAMAt6JYeFQsAAID/IdgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASJVxdgJmFjlrh6hJgpwNvdHZ1CQBgg39Dbh3F6d8QrtgBAACYRLEIdjNnzlRoaKi8vb0VHh6ujRs3XrP/smXLdMcdd8jb21uNGjXSt99+W0SVAgAAFF8uD3ZLlixRbGys4uLilJSUpCZNmig6OlrHjh0rsP/PP/+sXr16acCAAdq6dau6du2qrl27avv27UVcOQAAQPHi8mA3bdo0Pfnkk4qJiVH9+vU1e/Zs+fr6au7cuQX2nzFjhu655x49//zzqlevniZMmKDmzZvr3XffLeLKAQAAiheXBrucnBxt2bJFUVFR1jY3NzdFRUUpMTGxwG0SExNt+ktSdHT0VfsDAADcLlw6KjY9PV25ubkKCgqyaQ8KCtLOnTsL3CY1NbXA/qmpqQX2z87OVnZ2tnU5IyNDkpSZmXkzpdslL/tcoR8DzlEU54PEOXErKapzQuK8uJVwXqAghX1eXN6/YRjX7Wv66U7i4+M1fvz4fO0hISEuqAbFVeB0V1eA4oZzAgXhvEBBiuq8OHPmjAIDA6/Zx6XBrly5cnJ3d1daWppNe1pamoKDgwvcJjg42KH+o0ePVmxsrHU5Ly9PJ0+eVNmyZWWxWG7yHdxeMjMzFRISosOHDysgIMDV5aCY4LzAlTgnUBDOixtnGIbOnDmjSpUqXbevS4Odp6enwsLClJCQoK5du0q6FLwSEhI0ZMiQAreJiIhQQkKChg8fbm37/vvvFRERUWB/Ly8veXl52bSVKlXKGeXftgICAviPEvlwXuBKnBMoCOfFjbnelbrLXH4rNjY2Vn379lWLFi3UsmVLTZ8+XVlZWYqJiZEk9enTR5UrV1Z8fLwkadiwYYqMjNTUqVPVuXNnffrpp9q8ebPmzJnjyrcBAADgci4Pdj179tTx48c1btw4paamqmnTplq5cqV1gMShQ4fk5va/wbutWrXS4sWLNWbMGL300kuqXbu2vvzySzVs2NBVbwEAAKBYcHmwk6QhQ4Zc9dbrunXr8rU98sgjeuSRRwq5KlzJy8tLcXFx+W5t4/bGeYErcU6gIJwXRcNi2DN2FgAAAMWey795AgAAAM5BsAMAADAJgh0AAIBJEOxQoJkzZyo0NFTe3t4KDw/Xxo0bresuXLigwYMHq2zZsvLz89NDDz2Ub9JomM+PP/6oLl26qFKlSrJYLPryyy9t1huGoXHjxqlixYry8fFRVFSUdu/e7ZpiUaSu9XkxZ84ctW3bVgEBAbJYLDp9+rTrCkWRuN5nxfLly9WpUyfrFwUkJye7pE6zItghnyVLlig2NlZxcXFKSkpSkyZNFB0drWPHjkmSRowYoW+++UbLli3T+vXrdfToUXXv3t3FVaOwZWVlqUmTJpo5c2aB6ydPnqy3335bs2fP1i+//KKSJUsqOjpaFy5cKOJKUZSu93lx7tw53XPPPXrppZdcXCmKyvU+K7KysnTXXXdp0qRJRVzZbcIArtCyZUtj8ODB1uXc3FyjUqVKRnx8vHH69GnDw8PDWLZsmXX9jh07DElGYmKiK8qFC0gyvvjiC+tyXl6eERwcbEyZMsXadvr0acPLy8v45JNPXFAhisq1Pi/+bu3atYYk49SpU0VcIVzpys+Kv9u/f78hydi6dWuR1mR2XLGDjZycHG3ZskVRUVHWNjc3N0VFRSkxMVFbtmzRxYsXbdbfcccdqlq1qhITE11RMoqB/fv3KzU11ea8CAwMVHh4OOeFiV3v8wJA0SPYwUZ6erpyc3Ot3/xxWVBQkFJTU5WamipPT89837d7eT1uT5f/9lc7b2BO1/u8AFD0CHYAAAAmQbCDjXLlysnd3T3fKNe0tDQFBwcrODhYOTk5+Ua2XV6P29Plv/3VzhuY0/U+LwAUPYIdbHh6eiosLEwJCQnWtry8PCUkJCgiIkJhYWHy8PCwWf/nn3/q0KFDioiIcEXJKAaqV6+u4OBgm/MiMzNTv/zyC+eFiV3v8wJA0Svh6gJQ/MTGxqpv375q0aKFWrZsqenTpysrK0sxMTEKDAzUgAEDFBsbqzJlyiggIEDPPvusIiIi9I9//MPVpaMQnT17Vnv27LEu79+/X8nJySpTpoyqVq2q4cOH67XXXlPt2rVVvXp1jR07VpUqVVLXrl1dVzQK3bU+LyRZn829fO5s27ZN/v7+qlq1qsqUKePK0lFIrvdZcfLkSR06dEhHjx6VdOnigCTrXSHcJFcPy0Xx9M477xhVq1Y1PD09jZYtWxr/+c9/rOvOnz9vDBo0yChdurTh6+trdOvWzUhJSXFhtSgKl6eruPLVt29fwzAuTXkyduxYIygoyPDy8jI6dOhg/Pnnn64tGkXiWp8XcXFxBZ438+bNc13BKFTX+6yYN29egevj4uJcWrdZWAzDMIo2SgIAAKAw8IwdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdADhJ27ZtNXz48JveT2hoqKZPn37T+7HHgQMHZLFYlJycXCTHA1C4CHYAnKZfv36yWCwaOHBgvnWDBw+WxWJRv379ir6wYmL+/PmyWCzWl5+fn8LCwrR8+XKbfps2bdJTTz1lXbZYLPryyy8dOk6pUqXs6hsSEqKUlBQ1bNjQ7v0DKL4IdgCcKiQkRJ9++qnOnz9vbbtw4YIWL16sqlWrurAy++Tk5BTq/gMCApSSkqKUlBRt3bpV0dHR6tGjh/WL0CWpfPny8vX1LdQ6pEvv1d3dXcHBwSpRokShHw9A4SPYAXCq5s2bKyQkxOYq1PLly1W1alU1a9bMpm9eXp7i4+NVvXp1+fj4qEmTJvrss8+s63NzczVgwADr+rp162rGjBk2+1i3bp1atmypkiVLqlSpUmrdurUOHjwo6dIVxK5du9r0Hz58uNq2bWtdbtu2rYYMGaLhw4erXLlyio6OliRt375d9957r/z8/BQUFKR//vOfSk9Pt26XlZWlPn36yM/PTxUrVtTUqVPt+v1YLBYFBwcrODhYtWvX1muvvSY3Nzf99ttv1j5/vxUbGhoqSerWrZssFot1+ddff1W7du3k7++vgIAAhYWFafPmzVq3bp1iYmKUkZFhvTL4yiuvWPc1YcIE9enTRwEBAXrqqafy3Ypdt26dLBaLEhIS1KJFC/n6+qpVq1Y2wVOSXnvtNVWoUEH+/v564oknNGrUKDVt2tSu3wGAwkOwA+B0/fv317x586zLc+fOVUxMTL5+8fHxWrhwoWbPnq3ff/9dI0aM0OOPP67169dLuhT8qlSpomXLlumPP/7QuHHj9NJLL2np0qWSpL/++ktdu3ZVZGSkfvvtNyUmJuqpp56SxWJxqN4FCxbI09NTGzZs0OzZs3X69Gm1b99ezZo10+bNm7Vy5UqlpaWpR48e1m2ef/55rV+/Xl999ZVWr16tdevWKSkpyaHj5ubmasGCBZIuBeKCbNq0SZI0b948paSkWJcfe+wxValSRZs2bdKWLVs0atQoeXh4qFWrVpo+fbrNlcGRI0da9/fmm2+qSZMm2rp1q8aOHXvV2l5++WVNnTpVmzdvVokSJdS/f3/rukWLFmnixImaNGmStmzZoqpVq2rWrFkOvXcAhcQAACfp27ev8eCDDxrHjh0zvLy8jAMHDhgHDhwwvL29jePHjxsPPvig0bdvX8MwDOPChQuGr6+v8fPPP9vsY8CAAUavXr2ueozBgwcbDz30kGEYhnHixAlDkrFu3bpr1vN3w4YNMyIjI63LkZGRRrNmzWz6TJgwwejUqZNN2+HDhw1Jxp9//mmcOXPG8PT0NJYuXWpdf+LECcPHx8cYNmzYVWufN2+eIckoWbKkUbJkScPNzc3w8vIy5s2bZ9OvWrVqxltvvWVdlmR88cUXNn38/f2N+fPnX/U4gYGB+dqrVatmdO3a1aZt//79hiRj69athmEYxtq1aw1Jxpo1a6x9VqxYYUgyzp8/bxiGYYSHhxuDBw+22U/r1q2NJk2aXPW9AygaPFQBwOnKly+vzp07a/78+TIMQ507d1a5cuVs+uzZs0fnzp1Tx44dbdpzcnJsbtnOnDlTc+fO1aFDh3T+/Hnl5ORYb/mVKVNG/fr1U3R0tDp27KioqCj16NFDFStWdKjesLAwm+Vff/1Va9eulZ+fX76+e/futdYRHh5ubS9Tpozq1q173WP5+/tbr+ydO3dOa9as0cCBA1W2bFl16dLF7ppjY2P1xBNP6KOPPlJUVJQeeeQR1axZ87rbtWjRwq79N27c2Prz5d/nsWPHVLVqVf35558aNGiQTf+WLVvqhx9+sLt+AIWDYAegUPTv319DhgyRdCmcXens2bOSpBUrVqhy5co267y8vCRJn376qUaOHKmpU6cqIiJC/v7+mjJlin755Rdr33nz5mno0KFauXKllixZojFjxuj777/XP/7xD7m5uckwDJt9X7x4MV8tJUuWzFdbly5dNGnSpHx9K1asqD179tjzKyiQm5ubatWqZV1u3LixVq9erUmTJjkU7F555RX17t1bK1as0Hfffae4uDh9+umn6tat2zW3u/K9Xo2Hh4f158u3tvPy8uyuD4Br8IwdgEJxzz33KCcnRxcvXrQOSPi7+vXry8vLS4cOHVKtWrVsXiEhIZKkDRs2qFWrVho0aJCaNWumWrVqae/evfn21axZM40ePVo///yzGjZsqMWLF0u6dOUwJSXFpq8987U1b95cv//+u0JDQ/PVVrJkSdWsWVMeHh42AfPUqVPatWuXI78iK3d3d5tRxFfy8PBQbm5uvvY6depoxIgRWr16tbp37259rtHT07PA/s5St25d67N+l125DMA1CHYACoW7u7t27NihP/74Q+7u7vnW+/v7a+TIkRoxYoQWLFigvXv3KikpSe+88451QEHt2rW1efNmrVq1Srt27dLYsWNtAsT+/fs1evRoJSYm6uDBg1q9erV2796tevXqSZLat2+vzZs3a+HChdq9e7fi4uK0ffv269Y+ePBgnTx5Ur169dKmTZu0d+9erVq1SjExMcrNzZWfn58GDBig559/Xj/88IO2b9+ufv36yc3t+h+phmEoNTVVqamp2r9/v+bMmaNVq1bpwQcfvOo2oaGhSkhIUGpqqk6dOqXz589ryJAhWrdunQ4ePKgNGzZo06ZN1vcdGhqqs2fPKiEhQenp6Tp37tx163LEs88+qw8//FALFizQ7t279dprr+m3335zeNAKAOfjViyAQhMQEHDN9RMmTFD58uUVHx+vffv2qVSpUmrevLleeuklSdLTTz+trVu3qmfPnrJYLOrVq5cGDRqk7777TpLk6+urnTt3asGCBTpx4oQqVqyowYMH6+mnn5YkRUdHa+zYsXrhhRd04cIF9e/fX3369NG2bduuWVelSpW0YcMGvfjii+rUqZOys7NVrVo13XPPPdbwNmXKFOstW39/fz333HPKyMi47u8kMzPT+syal5eXqlWrpldffVUvvvjiVbeZOnWqYmNj9f7776ty5cratWuXTpw4oT59+igtLU3lypVT9+7dNX78eElSq1atNHDgQPXs2VMnTpxQXFycdcoTZ3jssce0b98+jRw5UhcuXFCPHj3Ur18/bdy40WnHAHBjLMaVD6AAAOCgjh07Kjg4WB999JGrSwFua1yxAwA45Ny5c5o9e7aio6Pl7u6uTz75RGvWrNH333/v6tKA2x5X7AAADjl//ry6dOmirVu36sKFC6pbt67GjBmj7t27u7o04LZHsAMAADAJRsUCAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYxP8DbRH+lLfW7ZgAAAAASUVORK5CYII=\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -629,29 +630,29 @@
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'R': <bound method SNLToy1.gateduration_R of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'MS': <bound method SNLToy1.gateduration_MS of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Rz': <bound method SNLToy1.gateduration_Rz of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Rx': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Ry': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            "{'MS': <bound method SNLToy1.gateduration_MS of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Px': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Py': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Pz': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'R': <bound method SNLToy1.gateduration_R of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Rx': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Ry': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Rz': <bound method SNLToy1.gateduration_Rz of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Sx': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Sy': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Sz': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Sxd': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Sxx': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Sy': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
                             " 'Syd': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Szd': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
-                            " 'Sxx': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>}"
+                            " 'Sz': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>,\n",
+                            " 'Szd': <bound method ExtensibleBackend._curry.<locals>._inner.<locals>.newop of <qscout.v1.std.noisy.SNLToy1 object at 0x85aa69c9ca30>>}"
                         ]
                     },
                     "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -715,15 +716,15 @@
                     "shell.execute_reply": "1970-01-01T00:00:00.000000Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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MzNnztS3336rb7/9Vh999JHatm2rJ554QsuXL7fNWbZsmYKCgtShQwelp6fbHuHh4fL399fatWtvOkeDBg20detWPf744zpw4ICmT5+uLl26KDg4WO+9955D27BarfLwuPRnLDc3VydOnJC/v7/q1q2r5OTk666/detW7d69W7169dKJEyds7zMrK0vt27fX999/r7y8vOtu56mnnrL9TP/6qF+/vm2On5+f5s+frx07dujvf/+7VqxYobfeektVq1bNt73IyEiFh4fblqtWraoHH3xQq1atUm5urgzD0GeffabOnTvLMAy731FMTIwyMjLyvf8+ffrI19f3uu9FurRH7NFHH7Ut161bV6VKlVK9evUUERFhG7/873379knSDeWKjY2123t4eY/q5W0CcA6HYoHbTMuWLe0unujZs6eaNWumwYMH6/7775e3t7d2796tjIwMu3Pd/spVFzfUqVNHH374oXJzc/X777/r3//+tyZNmqSnnnpK1atXV3R09DXXz8vL0/Tp0/Xuu+9q//79ys3NtT1XtmzZ677+7t27JV0qPVeTkZGh0qVLX3M7tWvXvm5WSWrdurWeeeYZzZw5UzExMerXr99Vt3elOnXq6Ny5czp+/Lg8PDx0+vRpzZkzR3PmzClwG1f+jqpXr37dfJdVqVJFFovFbiwoKEihoaH5xiTZzrs8fvy407muLLaXf9auOpcTuN1Q7IDbnIeHh9q2bavp06dr9+7datCggfLy8lShQgUtWrSowHXKly/v0gyenp5q1KiRGjVqpMjISLVt21aLFi26bll6/fXXNWbMGPXr10/jx49XmTJl5OHhoWHDhjm0p+3ynMmTJ1/1NiiuPJ8rOzvbdqHC3r17de7cOfn5+Tm9ncu5H3/88auW0saNG9stO7q3Trr0+3Bm3DCMG851vW0CcA7FDoD+/PNPSdLZs2clSTVr1tSaNWvUunVrpwqBK1zem5iSkmIbu3Lv0WWffvqp2rZtqw8++MBu/PTp0ypXrtx1169Zs6YkKTAw0KE9bjcrPj5eO3bs0JtvvqkXX3xRI0eO1Ntvv51v3uU9iX+1a9cu+fn52Up1QECAcnNziyS3o8qXL18oua72+wOQH+fYAbe5ixcvavXq1fL29la9evUkSd27d1dubq7Gjx+fb/6ff/6p06dP3/Tr/vDDD7p48WK+8a+//lrSpfO6LitZsmSBr+np6Zlvz86yZct05MgRu7GSJUtKUr5thIeHq2bNmnrzzTdtpfavjh8/7tB7ccRPP/2kN998U8OGDdNzzz2n559/XjNmzND69evzzU1KSrI7F+3w4cP68ssv1bFjR3l6esrT01MPPfSQPvvsM23fvr1QczujsHKVLFlSGRkZNxsPuC2wxw64zXzzzTfauXOnpEvnOy1evFi7d+/WyJEjFRgYKEmKiorS008/rYSEBG3dulUdO3aUl5eXdu/erWXLlmn69Ol6+OGHbyrHxIkTtXnzZnXr1s12eC45OVkLFy5UmTJl7G6LER4erlmzZum1115TrVq1VKFCBbVr107333+/Xn31VcXGxqpVq1batm2bFi1apBo1ati9Vs2aNVWqVCnNnj1bAQEBKlmypCIiIlS9enW9//77uvfee9WgQQPFxsaqcuXKOnLkiNauXavAwEB99dVX130vycnJ+uijj/KN16xZU5GRkbpw4YL69Omj2rVra8KECZKkcePG6auvvlJsbKy2bdtmK5+S1LBhQ8XExNjd7uTyOpe98cYbWrt2rSIiIvTkk0+qfv36OnnypJKTk7VmzRqdPHnS8V+GCxVGrvDwcC1ZskRxcXG688475e/vr86dOxdCesAE3HhFLoAiVNDtTnx8fIymTZsas2bNsrvdx2Vz5swxwsPDDV9fXyMgIMBo1KiR8cILLxhHjx61zbnR251s2LDBGDRokNGwYUMjKCjI8PLyMqpWrWr07dvX2Lt3r93c1NRUo1OnTkZAQIAhyfZ6Fy5cMJ577jmjYsWKhq+vr9G6dWsjKSkpXybDMIwvv/zSqF+/vlGiRIl8+bZs2WJ069bNKFu2rGG1Wo1q1aoZ3bt3NxITE6/5Hq53u5M+ffoYhmEYw4cPNzw9PY2ffvrJbv1NmzYZJUqUMJ555hnbmCRj0KBBxkcffWTUrl3bsFqtRrNmzexuSXJZWlqaMWjQICM0NNTw8vIyQkJCjPbt2xtz5syxzbl8W5Fly5blW/9qtztp0KBBvrnVqlUzOnXqlG/8cl5X5Sro83P27FmjV69eRqlSpQxJ3PoEuAaLYXCGKgAUFxaLRYMGDdKMGTPcHQXALYhz7AAAAEyCYgcAAGASFDsAAACTcGux+/7779W5c2dVqlRJFotFX3zxxXXXWbdunZo3by6r1apatWpp/vz5hZ4TAIqKYRicXwfghrm12GVlZalJkyaaOXOmQ/P379+vTp06qW3bttq6dauGDRumJ554QqtWrSrkpAAAAMVfsbkq1mKx6PPPP1eXLl2uOufFF1/UihUr7G58+eijj+r06dNauXJlEaQEAAAovm6pGxQnJSXl+5qamJgYuxuZXik7O1vZ2dm25by8PJ08eVJly5bla2oAAECxZxiGzpw5o0qVKsnD49oHW2+pYpeamqrg4GC7seDgYGVmZur8+fMFfqdlQkKC3d3aAQAAbkWHDx9WlSpVrjnnlip2N2LUqFGKi4uzLWdkZKhq1ao6fPiw7euTAAAAiqvMzEyFhoYqICDgunNvqWIXEhKitLQ0u7G0tDQFBgYWuLdOkqxWq6xWa77xwMBAih0AALhlOHIK2S11H7vIyEglJibajX377beKjIx0UyIAAIDiw63F7uzZs9q6dau2bt0q6dLtTLZu3apDhw5JunQYtXfv3rb5AwYM0L59+/TCCy9o586devfdd7V06VINHz7cHfEBAACKFbcWu02bNqlZs2Zq1qyZJCkuLk7NmjXT2LFjJUkpKSm2kidJ1atX14oVK/Ttt9+qSZMmmjJlit5//33FxMS4JT8AAEBxUmzuY1dUMjMzFRQUpIyMDM6xAwAAxZ4z3eWWOscOAAAAV0exAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAmKHQAAgElQ7AAAAEyCYgcAAGASFDsAAACToNgBAACYBMUOAADAJCh2AAAAJkGxAwAAMAm3F7uZM2cqLCxMPj4+ioiI0M8//3zN+dOmTVPdunXl6+ur0NBQDR8+XBcuXCiitAAAAMWXW4vdkiVLFBcXp/j4eCUnJ6tJkyaKiYnRsWPHCpy/ePFijRw5UvHx8dqxY4c++OADLVmyRC+99FIRJwcAACh+3Frspk6dqieffFKxsbGqX7++Zs+eLT8/P82dO7fA+T/++KNat26tXr16KSwsTB07dlTPnj2vu5cPAADgduC2YpeTk6PNmzcrOjr6f2E8PBQdHa2kpKQC12nVqpU2b95sK3L79u3T119/rfvuu++qr5Odna3MzEy7BwAAgBmVcNcLp6enKzc3V8HBwXbjwcHB2rlzZ4Hr9OrVS+np6brrrrtkGIb+/PNPDRgw4JqHYhMSEjRu3DiXZgcAACiO3H7xhDPWrVun119/Xe+++66Sk5O1fPlyrVixQuPHj7/qOqNGjVJGRobtcfjw4SJMDAAAUHTctseuXLly8vT0VFpamt14WlqaQkJCClxnzJgx+sc//qEnnnhCktSoUSNlZWXpqaee0ssvvywPj/w91Wq1ymq1uv4NAAAAFDNu22Pn7e2t8PBwJSYm2sby8vKUmJioyMjIAtc5d+5cvvLm6ekpSTIMo/DCAgAA3ALctsdOkuLi4tSnTx+1aNFCLVu21LRp05SVlaXY2FhJUu/evVW5cmUlJCRIkjp37qypU6eqWbNmioiI0J49ezRmzBh17tzZVvAAAABuV24tdj169NDx48c1duxYpaamqmnTplq5cqXtgopDhw7Z7aEbPXq0LBaLRo8erSNHjqh8+fLq3LmzJkyY4K63AAAAUGxYjNvsGGZmZqaCgoKUkZGhwMBAd8cBAAC4Jme6yy11VSwAAACujmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADCJmy52mZmZ+uKLL7Rjxw5X5AEAAMANcrrYde/eXTNmzJAknT9/Xi1atFD37t3VuHFjffbZZy4PCAAAAMc4Xey+//573X333ZKkzz//XIZh6PTp03r77bf12muvuTwgAAAAHON0scvIyFCZMmUkSStXrtRDDz0kPz8/derUSbt373Z5QAAAADjG6WIXGhqqpKQkZWVlaeXKlerYsaMk6dSpU/Lx8XF5QAAAADimhLMrDBs2TI899pj8/f1VrVo1tWnTRtKlQ7SNGjVydT4AAAA4yOliN3DgQEVEROjQoUPq0KGDPDwu7fSrUaOGJkyY4PKAAAAAcIzTh2JfffVV1atXT127dpW/v79tvF27dlqzZo1LwwEAAMBxFsMwDGdW8PT0VEpKiipUqGA3fuLECVWoUEG5ubkuDehqmZmZCgoKUkZGhgIDA90dBwAA4Jqc6S5O77EzDEMWiyXf+C+//GK7WhYAAABFz+Fz7EqXLi2LxSKLxaI6derYlbvc3FydPXtWAwYMKJSQAAAAuD6Hi920adNkGIb69euncePGKSgoyPact7e3wsLCFBkZWSghAQAAcH0OF7s+ffpIkqpXr65WrVrJy8ur0EIBAADAeU7f7iQqKkp5eXnatWuXjh07pry8PLvn//73v7ssHAAAABzndLH7z3/+o169eungwYO68oJai8VS7K+KBQAAMCuni92AAQPUokULrVixQhUrVizwClkAAAAUPaeL3e7du/Xpp5+qVq1ahZEHAAAAN8jp+9hFRERoz549hZEFAAAAN8HpPXbPPvusnnvuOaWmpqpRo0b5ro5t3Lixy8IBAADAcU5/pZiHR/6dfBaLxfaNFMX94gm+UgwAANxKnOkuTu+x279//w0HAwAAQOFxuthVq1atMHIAAADgJjld7BYuXHjN53v37n3DYQAAAHDjnD7HrnTp0nbLFy9e1Llz5+Tt7S0/Pz+dPHnSpQFdjXPsAADArcSZ7uL07U5OnTpl9zh79qz++OMP3XXXXfr4449vODQAAABujtPFriC1a9fWG2+8oaFDh7picwAAALgBLil2klSiRAkdPXrUVZsDAACAk5wudv/617/sHl9++aVmz56txx9/XK1bt3Y6wMyZMxUWFiYfHx9FRETo559/vub806dPa9CgQapYsaKsVqvq1Kmjr7/+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CYodAACASVDsAAAATIJiBwAAYBIUOwAAAJOg2AEAAJgExQ4AAMAkKHYAAAAmQbEDABdp06aNhg0bdtPbCQsL07Rp0256O444cOCALBaLtm7dWiSvB6BwUewAuEzfvn1lsVg0YMCAfM8NGjRIFotFffv2LfpgxcT8+fNlsVhsD39/f4WHh2v58uV28zZu3KinnnrKtmyxWPTFF1849TqlSpVyaG5oaKhSUlLUsGFDh7cPoPii2AFwqdDQUH3yySc6f/68bezChQtavHixqlat6sZkjsnJySnU7QcGBiolJUUpKSnasmWLYmJi1L17d9sXoUtS+fLl5efnV6g5pEvv1dPTUyEhISpRokShvx6AwkexA+BSzZs3V2hoqN1eqOXLl6tq1apq1qyZ3dy8vDwlJCSoevXq8vX1VZMmTfTpp5/ans/NzVX//v1tz9etW1fTp0+328a6devUsmVLlSxZUqVKlVLr1q118OBBSZf2IHbp0sVu/rBhw9SmTRvbcps2bTR48GANGzZM5cqVU0xMjCRp+/btuvfee+Xv76/g4GD94x//UHp6um29rKws9e7dW/7+/qpYsaKmTJni0M/HYrEoJCREISEhql27tl577TV5eHjo119/tc3566HYsLAwSVLXrl1lsVhsy7/88ovatm2rgIAABQYGKjw8XJs2bdK6desUGxurjIwM257BV155xbat8ePHq3fv3goMDNRTTz2V71DsunXrZLFYlJiYqBYtWsjPz0+tWrWyK56S9Nprr6lChQoKCAjQE088oZEjR6pp06YO/QwAFB6KHQCX69evn+bNm2dbnjt3rmJjY/PNS0hI0MKFCzV79mz99ttvGj58uB5//HGtX79e0qXiV6VKFS1btky///67xo4dq5deeklLly6VJP3555/q0qWLoqKi9OuvvyopKUlPPfWULBaLU3kXLFggb29vbdiwQbNnz9bp06fVrl07NWvWTJs2bdLKlSuVlpam7t2729Z5/vnntX79en355ZdavXq11q1bp+TkZKdeNzc3VwsWLJB0qRAXZOPGjZKkefPmKSUlxbb82GOPqUqVKtq4caM2b96skSNHysvLS61atdK0adPs9gyOGDHCtr0333xTTZo00ZYtWzRmzJirZnv55Zc1ZcoUbdq0SSVKlFC/fv1szy1atEgTJkzQxIkTtXnzZlWtWlWzZs1y6r0DKCQGALhInz59jAcffNA4duyYYbVajQMHDhgHDhwwfHx8jOPHjxsPPvig0adPH8MwDOPChQuGn5+f8eOPP9pto3///kbPnj2v+hqDBg0yHnroIcMwDOPEiROGJGPdunXXzPNXQ4cONaKiomzLUVFRRrNmzezmjB8/3ujYsaPd2OHDhw1Jxh9//GGcOXPG8Pb2NpYuXWp7/sSJE4avr68xdOjQq2afN2+eIckoWbKkUbJkScPDw8OwWq3GvHnz7OZVq1bNeOutt2zLkozPP//cbk5AQIAxf/78q75OUFBQvvFq1aoZXbp0sRvbv3+/IcnYsmWLYRiGsXbtWkOSsWbNGtucFStWGJKM8+fPG4ZhGBEREcagQYPsttO6dWujSZMmV33vAIoGJ1UAcLny5curU6dOmj9/vgzDUKdOnVSuXDm7OXv27NG5c+fUoUMHu/GcnBy7Q7YzZ87U3LlzdejQIZ0/f145OTm2Q35lypRR3759FRMTow4dOig6Olrdu3dXxYoVncobHh5ut/zLL79o7dq18vf3zzd37969thwRERG28TJlyqhu3brXfa2AgADbnr1z585pzZo1GjBggMqWLavOnTs7nDkuLk5PPPGEPvzwQ0VHR+uRRx5RzZo1r7teixYtHNp+48aNbf++/PM8duyYqlatqj/++EMDBw60m9+yZUt99913DucHUDgodgAKRb9+/TR48GBJl8rZlc6ePStJWrFihSpXrmz3nNVqlSR98sknGjFihKZMmaLIyEgFBARo8uTJ+umnn2xz582bpyFDhmjlypVasmSJRo8erW+//VZ/+9vf5OHhIcMw7LZ98eLFfFlKliyZL1vnzp01ceLEfHMrVqyoPXv2OPIjKJCHh4dq1aplW27cuLFWr16tiRMnOlXsXnnlFfXq1UsrVqzQN998o/j4eH3yySfq2rXrNde78r1ejZeXl+3flw9t5+XlOZwPgHtwjh2AQnHPPfcoJydHFy9etF2Q8Ff169eX1WrVoUOHVKtWLbtHaGioJGnDhg1q1aqVBg4cqGbNmqlWrVrau3dvvm01a9ZMo0aN0o8//qiGDRtq8eLFki7tOUxJSbGb68j92po3b67ffvtNYWFh+bKVLFlSNWvWlJeXl13BPHXqlHbt2uXMj8jG09PT7iriK3l5eSk3NzffeJ06dTR8+HCtXr1a3bp1s53X6O3tXeB8V6lbt67tXL/LrlwG4B4UOwCFwtPTUzt27NDvv/8uT0/PfM8HBARoxIgRGj58uBYsWKC9e/cqOTlZ77zzju2Cgtq1a2vTpk1atWqVdu3apTFjxtgViP3792vUqFFKSkrSwYMHtXr1au3evVv16tWTJLVr106bNm3SwoULtXv3bsXHx2v79u3XzT5o0CCdPHlSPXv21MaNG7V3716tWrVKsbGxys3Nlb+/v/r376/nn39e3333nbZv366+ffvKw+P6f1INw1BqaqpSU1O1f/9+zZkzR6tWrdKDDz541XXCwsKUmJio1NRUnTp1SufPn9fgwYO1bt06HTx4UBs2bNDGjRtt7zssLExnz55VYmKi0tPTde7cuevmcsazzz6rDz74QAsWLNDu3bv12muv6ddff3X6ohUArsehWACFJjAw8JrPjx8/XuXLl1dCQoL27dunUqVKqXnz5nrppZckSU8//bS2bNmiHj16yGKxqGfPnho4cKC++eYbSZKfn5927typBQsW6MSJE6pYsaIGDRqkp59+WpIUExOjMWPG6IUXXtCFCxfUr18/9e7dW9u2bbtmrkqVKmnDhg168cUX1bFjR2VnZ6tatWq65557bOVt8uTJtkO2AQEBeu6555SRkXHdn0lmZqbtnDWr1apq1arp1Vdf1YsvvnjVdaZMmaK4uDi99957qly5snbt2qUTJ06od+/eSktLU7ly5dStWzeNGzdOktSqVSsNGDBAPXr00IkTJxQfH2+75YkrPPbYY9q3b59GjBihCxcuqHv37urbt69+/vlnl70GgBtjMa48AQUAACd16NBBISEh+vDDD90dBbitsccOAOCUc+fOafbs2YqJiZGnp6c+/vhjrVmzRt9++627owG3PfbYAQCccv78eXXu3FlbtmzRhQsXVLduXY0ePVrdunVzdzTgtkexAwAAMAmuigUAADAJih0AAIBJUOwAAABMgmIHAABgEhQ7AAAAk6DYAQAAmATFDgAAwCQodgAAACZBsQMAADCJ/wfzLvVasueAXAAAAABJRU5ErkJggg==\n",
+                        "image/png": "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LHCbmTlzpr7//nt9//33+vjjj9WuXTs98cQTWr58ubXPsmXLFBgYqI4dOyo9Pd36CgsLk5+fn9auXXvTdTRo0EDJycl6/PHHdeDAAc2YMUNdu3ZVUFCQ3n//fbv24eXlJTe3Sx9jubm5OnHihPz8/FS3bl0lJSVdd/vk5GTt3r1bvXv31okTJ6zvMysrSx06dNCPP/6ovLy86+7nqaeesv5O//6qX7++tY+vr6/mz5+vHTt26O6779aKFSv01ltvqWrVqvn2FxERobCwMOty1apV9eCDD2rVqlXKzc2VYRj6/PPP1aVLFxmGYfM3io6OVkZGRr7337dvX/n4+Fz3vUiXrog9+uij1uW6deuqVKlSqlevnsLDw63tl3/et2+fJN1QXTExMTZXDy9fUb28TwCO4VYscJtp2bKlzeCJXr16qVmzZhoyZIjuv/9+eXp6avfu3crIyLB51u3vnDW4oU6dOvroo4+Um5urP/74Q//+9781efJkPfXUU6pevbqioqKuuX1eXp5mzJih9957T/v371dubq51XdmyZa97/N27d0u6FHquJiMjQ6VLl77mfmrXrn3dWiWpdevWeuaZZzRz5kxFR0erf//+V93flerUqaNz587p+PHjcnNz0+nTpzVnzhzNmTOnwH1c+TeqXr36deu7rEqVKrJYLDZtgYGBCgkJydcmyfrc5fHjxx2u68pge/l37axnOYHbDcEOuM25ubmpXbt2mjFjhnbv3q0GDRooLy9PFSpU0KJFiwrcpnz58k6twd3dXY0aNVKjRo0UERGhdu3aadGiRdcNS6+//rrGjh2r/v37a8KECSpTpozc3Nw0fPhwu660Xe4zZcqUq06D4sznubKzs60DFfbu3atz587J19fX4f1crvvxxx+/aiht3LixzbK9V+ukS38PR9oNw7jhuq63TwCOIdgB0F9//SVJOnv2rCSpZs2aWrNmjVq3bu1QIHCGy1cTU1JSrG1XXj267LPPPlO7du304Ycf2rSfPn1a5cqVu+72NWvWlCQFBATYdcXtZsXFxWnHjh1688039eKLL2rUqFF6++238/W7fCXx73bt2iVfX19rqPb391dubm6R1G2v8uXLF0pdV/v7AciPZ+yA29zFixe1evVqeXp6ql69epKkHj16KDc3VxMmTMjX/6+//tLp06dv+rg//fSTLl68mK/922+/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t25d67N+l125DMA1CHYACoW7u7t27NihP/74Q+7u7vnW+/v7a+TIkRoxYoQWLFigvXv3KikpSe+88451QEHt2rW1efNmrVq1Srt27dLYsWNtAsT+/fs1evRoJSYm6uDBg1q9erV2796tevXqSZLat2+vzZs3a+HChdq9e7fi4uK0ffv269Y+ePBgnTx5Ur169dKmTZu0d+9erVq1SjExMcrNzZWfn58GDBig559/Xj/88IO2b9+ufv36yc3t+h+phmEoNTVVqamp2r9/v+bMmaNVq1bpwQcfvOo2oaGhSkhIUGpqqk6dOqXz589ryJAhWrdunQ4ePKgNGzZo06ZN1vcdGhqqs2fPKiEhQenp6Tp37tx163LEs88+qw8//FALFizQ7t279dprr+m3335zeNAKAOfjViyAQhMQEHDN9RMmTFD58uUVHx+vffv2qVSpUmrevLleeuklSdLTTz+trVu3qmfPnrJYLOrVq5cGDRqk7777TpLk6+urnTt3asGCBTpx4oQqVqyowYMH6+mnn5YkRUdHa+zYsXrhhRd04cIF9e/fX3369NG2bduuWVelSpW0YcMGvfjii+rUqZOys7NVrVo13XPPPdbwNmXKFOstW39/fz333HPKyMi47u8kMzPT+syal5eXqlWrpldffVUvvvjiVbeZOnWqYmNj9f7776ty5cratWuXTpw4oT59+igtLU3lypVT9+7dNX78eElSq1atNHDgQPXs2VMnTpxQXFycdcoTZ3jssce0b98+jRw5UhcuXFCPHj3Ur18/bdy40WnHAHBjLMaVD6AAAOCgjh07Kjg4WB999JGrSwFua1yxAwA45Ny5c5o9e7aio6Pl7u6uTz75RGvWrNH333/v6tKA2x5X7AAADjl//ry6dOmirVu36sKFC6pbt67GjBmj7t27u7o04LZHsAMAADAJRsUCAACYBMEOAADAJAh2AAAAJkGwAwAAMAmCHQAAgEkQ7AAAAEyCYAcAAGASBDsAAACTINgBAACYxP8DbRH+lLfW7ZgAAAAASUVORK5CYII=\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -772,15 +773,15 @@
             "outputs": [],
             "source": [
                 "# Useful tools:\n",
                 "from numpy import abs, diag, pi, kron\n",
                 "import pygsti\n",
                 "\n",
                 "# Description of the ideal gates\n",
-                "from qscout.v1.std.jaqal_gates import U_R, U_Rz, U_MS\n",
+                "from qscout.v1.std.jaqal_action import U_R, U_Rz, U_MS\n",
                 "\n",
                 "# This superclass will handle some details\n",
                 "from jaqalpaq.emulator.pygsti import AbstractNoisyNativeEmulator\n",
                 "\n",
                 "# The superclass needs a description of the gates to handle\n",
                 "from qscout.v1.std.jaqal_gates import ALL_GATES\n",
                 "\n",
@@ -959,15 +960,15 @@
                     "shell.execute_reply": "1970-01-01T00:00:00.000000Z"
                 },
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAnYAAAHWCAYAAAD6oMSKAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8qNh9FAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA+W0lEQVR4nO3deVRU9f/H8deAMIAs7uCC4p77gklohgtKZZZaaVpfFW0xNRey0lLJzEhN08r0a4tLaallq6UmqfUzvrmgpaW5L18FFBdQVDC4vz88zrcR1BkdGL0+H+fMOdzP/dx73wPXOS8/997PWAzDMAQAAICbnoe7CwAAAIBrEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAXJfWrVurdevWtuV9+/bJYrFozpw5bqsJjlm9erUsFotWr17t7lIAuAjBDrhFzJkzRxaLxe5Vrlw5tWnTRt9//71batq3b59iY2NVvXp1+fj4KCQkRHfddZfi4+Pt+r377rvXFRQPHz6sl19+WZs3b76+gi9xMcRe7vX666+79Hi3qgULFmjq1KnuLgO4KRRzdwEAitYrr7yiqlWryjAMpaWlac6cObr33nv1zTff6L777iuyOnbt2qXbb79dvr6+6tu3r8LCwpSSkqLk5GRNmDBBY8eOtfV99913VaZMGfXp0+eajnX48GGNHTtWYWFhaty4sWvewD/06NFD9957b772Jk2auPxYrnTXXXfp7Nmz8vb2dncpV7RgwQJt3bpVQ4cOdXcpwA2PYAfcYu655x41a9bMttyvXz8FBwfrk08+KdJg9+abb+r06dPavHmzqlSpYrfuyJEjRVaHKzRt2lSPPfaYu8tw2Llz5+Tt7S0PDw/5+Pi4uxwALsSlWOAWV6JECfn6+qpYMfv/5+Xl5Wnq1KmqV6+efHx8FBwcrKeeekonTpxwyXF3796tSpUq5Qt1klSuXDnbz2FhYfrjjz+0Zs0a2yXOi/f0HT9+XMOHD1eDBg3k7++vwMBA3XPPPfrtt99s269evVq33367JCk2Nta2j39e2v3111919913KygoSH5+foqKitLatWtd8j4l6ccff5SHh4fGjBlj175gwQJZLBbNmDHD1maxWDRo0CDNnz9ftWvXlo+Pj8LDw/XTTz/l2++hQ4fUt29fBQcHy2q1ql69evrwww/t+ly8j+7TTz/VqFGjVLFiRfn5+SkzM7PAe+xat26t+vXr6/fff1dUVJT8/PxUo0YNffbZZ5KkNWvWKCIiQr6+vqpdu7ZWrlx5XXUtWrRI48ePV6VKleTj46N27dpp165ddvUsXbpU+/fvt/3twsLCHP7dA7caRuyAW0xGRobS09NlGIaOHDmit99+W6dPn8434vTUU09pzpw5io2N1eDBg7V3716988472rRpk9auXSsvL6/rqqNKlSpauXKlfvzxR7Vt2/ay/aZOnapnnnlG/v7+eumllyRJwcHBkqQ9e/boyy+/1MMPP6yqVasqLS1N//73vxUVFaU///xTFSpUUJ06dfTKK69ozJgxevLJJ9WqVStJUosWLSRdCF333HOPwsPDFR8fLw8PD82ePVtt27bVzz//rObNm1/1vZw5c0bp6en52kuUKKFixYqpbdu2GjBggBISEtS5c2c1bdpUKSkpeuaZZxQdHa3+/fvbbbdmzRotXLhQgwcPltVq1bvvvqu7775b69atU/369SVJaWlpuuOOO2xBsGzZsvr+++/Vr18/ZWZm5rtsOW7cOHl7e2v48OHKzs6+4uXXEydO6L777tMjjzyihx9+WDNmzNAjjzyi+fPna+jQoerfv7969uypSZMm6aGHHtLBgwcVEBBwTXW9/vrr8vDw0PDhw5WRkaGJEyfq0Ucf1a+//ipJeumll5SRkaH//ve/evPNNyVJ/v7+V/2bALcsA8AtYfbs2YakfC+r1WrMmTPHru/PP/9sSDLmz59v175s2bJ87VFRUUZUVJRtee/evYYkY/bs2VesZ+vWrYavr68hyWjcuLExZMgQ48svvzSysrLy9a1Xr57dMS46d+6ckZuba9e2d+9ew2q1Gq+88oqtbf369QXWlJeXZ9SsWdOIiYkx8vLybO1nzpwxqlatarRv3/6K7+Hie73cKykpydY3KyvLqFGjhlGvXj3j3LlzRseOHY3AwEBj//79dvu8uO2GDRtsbfv37zd8fHyMLl262Nr69etnlC9f3khPT7fb/pFHHjGCgoKMM2fOGIZhGKtWrTIkGdWqVbO1XXRx3apVq2xtUVFRhiRjwYIFtrbt27cbkgwPDw/jP//5j619+fLl+X6vztZVp04dIzs729Zv2rRphiRjy5YttraOHTsaVapUMQBcHZdigVvM9OnT9cMPP+iHH37Qxx9/rDZt2ujxxx/XkiVLbH0WL16soKAgtW/fXunp6bZXeHi4/P39tWrVquuuo169etq8ebMee+wx7du3T9OmTVPnzp0VHBys9957z6F9WK1WeXhc+BjLzc3VsWPH5O/vr9q1ays5Ofmq22/evFk7d+5Uz549dezYMdv7zMrKUrt27fTTTz8pLy/vqvt58sknbb/Tf77q1q1r6+Pn56c5c+Zo27Ztuuuuu7R06VK9+eabqly5cr79RUZGKjw83LZcuXJlPfDAA1q+fLlyc3NlGIY+//xzderUSYZh2P2NYmJilJGRke/99+7dW76+vld9L9KFEbFHHnnEtly7dm2VKFFCderUUUREhK394s979uyRpGuqKzY21m708OKI6sV9AnAOl2KBW0zz5s3tHp7o0aOHmjRpokGDBum+++6Tt7e3du7cqYyMDLt73f7JVQ831KpVSx999JFyc3P1559/6ttvv9XEiRP15JNPqmrVqoqOjr7i9nl5eZo2bZreffdd7d27V7m5ubZ1pUuXvurxd+7cKelC6LmcjIwMlSxZ8or7qVmz5lVrlaSWLVvq6aef1vTp0xUTE6O+fftedn+XqlWrls6cOaOjR4/Kw8NDJ0+e1KxZszRr1qwC93Hp36hq1apXre+iSpUqyWKx2LUFBQUpNDQ0X5sk232XR48edbquS4Ptxd+1q+7lBG41BDvgFufh4aE2bdpo2rRp2rlzp+rVq6e8vDyVK1dO8+fPL3CbsmXLurQGT09PNWjQQA0aNFBkZKTatGmj+fPnXzUsvfbaaxo9erT69u2rcePGqVSpUvLw8NDQoUMdGmm72GfSpEmXnQbFlfdzZWdn2x5U2L17t86cOSM/Pz+n93Ox7scee+yyobRhw4Z2y46O1kkX/h7OtBuGcc11XW2fAJxDsAOgv//+W5J0+vRpSVL16tW1cuVKtWzZ0qlA4AoXRxNTUlJsbZeOHl302WefqU2bNvrggw/s2k+ePKkyZcpcdfvq1atLkgIDAx0acbte8fHx2rZtm9544w298MILGjFihN566618/S6OJP7Tjh075OfnZwvVAQEBys3NLZK6HVW2bNlCqetyfz8A+XGPHXCLO3/+vFasWCFvb2/VqVNHktStWzfl5uZq3Lhx+fr//fffOnny5HUf9+eff9b58+fztX/33XeS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i2EYRtFGSQAAABQG7rEDAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADABdp3bq1hg4det37CQsL09SpU697P47Yt2+fLBaLNm/eXCTHA1C4CHYAXKZPnz6yWCzq379/vnUDBw6UxWJRnz59ir6wG8ScOXNksVhsL39/f4WHh2vJkiV2/davX68nn3zStmyxWPTll186dZwSJUo41Dc0NFQpKSmqX7++w/sHcOMi2AFwqdDQUH366ac6e/asre3cuXNasGCBKleu7MbKHJOTk1Oo+w8MDFRKSopSUlK0adMmxcTEqFu3brYvQpeksmXLys/Pr1DrkC68V09PT4WEhKhYsWKFfjwAhY9gB8ClmjZtqtDQULtRqCVLlqhy5cpq0qSJXd+8vDwlJCSoatWq8vX1VaNGjfTZZ5/Z1ufm5qpfv3629bVr19a0adPs9rF69Wo1b95cxYsXV4kSJdSyZUvt379f0oURxM6dO9v1Hzp0qFq3bm1bbt26tQYNGqShQ4eqTJkyiomJkSRt3bpV99xzj/z9/RUcHKx//etfSk9Pt22XlZWlXr16yd/fX+XLl9fkyZMd+v1YLBaFhIQoJCRENWvW1KuvvioPDw/9/vvvtj7/vBQbFhYmSerSpYssFott+bffflObNm0UEBCgwMBAhYeHa8OGDVq9erViY2OVkZFhGxl8+eWXbfsaN26cevXqpcDAQD355JP5LsWuXr1aFotFiYmJatasmfz8/NSiRQu74ClJr776qsqVK6eAgAA9/vjjGjFihBo3buzQ7wBA4SHYAXC5vn37avbs2bblDz/8ULGxsfn6JSQkaN68eZo5c6b++OMPDRs2TI899pjWrFkj6ULwq1SpkhYvXqw///xTY8aM0YsvvqhFixZJkv7++2917txZUVFR+v3335WUlKQnn3xSFovFqXrnzp0rb29vrV27VjNnztTJkyfVtm1bNWnSRBs2bNCyZcuUlpambt262bZ57rnntGbNGn311VdasWKFVq9ereTkZKeOm5ubq7lz50q6EIgLsn79eknS7NmzlZKSYlt+9NFHValSJa1fv14bN27UiBEj5OXlpRYtWmjq1Kl2I4PDhw+37e+NN95Qo0aNtGnTJo0ePfqytb300kuaPHmyNmzYoGLFiqlv3762dfPnz9f48eM1YcIEbdy4UZUrV9aMGTOceu8ACokBAC7Su3dv44EHHjCOHDliWK1WY9++fca+ffsMHx8f4+jRo8YDDzxg9O7d2zAMwzh37pzh5+dn/PLLL3b76Nevn9GjR4/LHmPgwIHGgw8+aBiGYRw7dsyQZKxevfqK9fzTkCFDjKioKNtyVFSU0aRJE7s+48aNMzp06GDXdvDgQUOS8ddffxmnTp0yvL29jUWLFtnWHzt2zPD19TWGDBly2dpnz55tSDKKFy9uFC9e3PDw8DCsVqsxe/Zsu35VqlQx3nzzTduyJOOLL76w6xMQEGDMmTPnsscJCgrK116lShWjc+fOdm179+41JBmbNm0yDMMwVq1aZUgyVq5caeuzdOlSQ5Jx9uxZwzAMIyIiwhg4cKDdflq2bGk0atTosu8dQNHgpgoALle2bFl17NhRc+bMkWEY6tixo8qUKWPXZ9euXTpz5ozat29v156Tk2N3yXb69On68MMPdeDAAZ09e1Y5OTm2S36lSpVSnz59FBMTo/bt2ys6OlrdunVT+fLlnao3PDzcbvm3337TqlWr5O/vn6/v7t27bXVERETY2kuVKqXatWtf9VgBAQG2kb0zZ85o5cqV6t+/v0qXLq1OnTo5XHNcXJwef/xxffTRR4qOjtbDDz+s6tWrX3W7Zs2aObT/hg0b2n6++Ps8cuSIKleurL/++ksDBgyw69+8eXP9+OOPDtcPoHAQ7AAUir59+2rQoEGSLoSzS50+fVqStHTpUlWsWNFundVqlSR9+umnGj58uCZPnqzIyEgFBARo0qRJ+vXXX219Z8+ercGDB2vZsmVauHChRo0apR9++EF33HGHPDw8ZBiG3b7Pnz+fr5bixYvnq61Tp06aMGFCvr7ly5fXrl27HPkVFMjDw0M1atSwLTds2FArVqzQhAkTnAp2L7/8snr27KmlS5fq+++/V3x8vD799FN16dLlittd+l4vx8vLy/bzxUvbeXl5DtcHwD24xw5Aobj77ruVk5Oj8+fP2x5I+Ke6devKarXqwIEDqlGjht0rNDRUkrR27Vq1aNFCAwYMUJMmTVSjRg3t3r07376aNGmikSNH6pdfflH9+vW1YMECSRdGDlNSUuz6OjJfW9OmTfXHH38oLCwsX23FixdX9erV5eXlZRcwT5w4oR07djjzK7Lx9PS0e4r4Ul5eXsrNzc3XXqtWLQ0bNkwrVqxQ165dbfc1ent7F9jfVWrXrm271++iS5cBuAfBDkCh8PT01LZt2/Tnn3/K09Mz3/qAgAANHz5cw4YN09y5c7V7924lJyfr7bfftj1QULNmTW3YsEHLly/Xjh07NHr0aLsAsXfvXo0cOVJJSUnav3+/VqxYoZ07d6pOnTqSpLZt22rDhg2aN2+edu7cqfj4eG3duvWqtQ8cOFDHjx9Xjx49tH79eu3evVvLly9XbGyscnNz5e/vr379+um5557Tjz/+qK1bt6pPnz7y8Lj6R6phGEpNTVVqaqr27t2rWbNmafny5XrggQcuu01YWJgSExOVmpqqEydO6OzZsxo0aJBWr16t/fv3a+3atVq/fr3tfYeFhen06dNKTExUenq6zpw5c9W6nPHMM8/ogw8+0Ny5c7Vz5069+uqr+v33351+aAWA63EpFkChCQwMvOL6cePGqWzZskpISNCePXtUokQJNW3aVC+++KIk6amnntKmTZvUvXt3WSwW9ejRQwMGDND3338vSfLz89P27ds1d+5cHTt2TOXLl9fAgQP11FNPSZJiYmI0evRoPf/88zp37pz69u2rXr16acuWLVesq0KFClq7dq1eeOEFdejQQdnZ2apSpYruvvtuW3ibNGmS7ZJtQECAnn32WWVkZFz1d5KZmWm7Z81qtapKlSp65ZVX9MILL1x2m8mTJysuLk7vvfeeKlasqB07dujYsWPq1auX0tLSVKZMGXXt2lVjx46VJLVo0UL9+/dX9+7ddezYMcXHx9umPHGFRx99VHv27NHw4cN17tw5devWTX369NG6detcdgwA18ZiXHoDCgAATmrfvr1CQkL00UcfubsU4JbGiB0AwClnzpzRzJkzFRMTI09PT33yySdauXKlfvjhB3eXBtzyGLEDADjl7Nmz6tSpkzZt2qRz586pdu3aGjVqlLp27eru0oBbHsEOAADAJHgqFgAAwCQIdgAAACZBsAMAADAJgh0AAIBJEOwAAABMgmAHAABgEgQ7AAAAkyDYAQAAmATBDgAAwCT+H/azB+4VZmmgAAAAAElFTkSuQmCC\n",
+                        "image/png": "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j0uxwG1m5syZ+vbbb/Xtt9/qo48+Urt27fT4449r+fLltj7Lli1TUFCQOnbsqPT0dNsrPDxc/v7+Wrt27U3X0aBBA23btk2PPfaYDhw4oBkzZqhr164KDg7We++959A+rFarPDwufYzl5ubqxIkT8vf3V926dZWcnHzd7bdt26bdu3erd+/eOnHihO19ZmVlqUOHDvr++++Vl5d33f08+eSTtt/pX1/169e39fHz89P8+fO1Y8cO/f3vf9eKFSv05ptvqmrVqvn2FxkZqfDwcNty1apV9cADD2jVqlXKzc2VYRj67LPP1KVLFxmGYfc3iomJUUZGRr7337dvX/n6+l73vUiXRsQeeeQR23LdunVVqlQp1atXTxEREbb2yz/v27dPkm6ortjYWLvRw8sjqpf3CcA5XIoFbjMtW7a0e3iiV69eatasmYYMGaL77rtP3t7e2r17tzIyMuzudfsrVz3cUKdOHX344YfKzc3V77//rn//+9+aPHmynnzySVWvXl3R0dHX3D4vL08zZszQu+++q/379ys3N9e2rmzZstc9/u7duyVdCj1Xk5GRodKlS19zP7Vr175urZLUunVrPf3005o5c6ZiYmLUv3//q+7vSnXq1NG5c+d0/PhxeXh46PTp05ozZ47mzJlT4D6u/BtVr179uvVdVqVKFVksFru2oKAghYaG5muTZLvv8vjx407XdWWwvfy7dtW9nMDthmAH3OY8PDzUrl07zZgxQ7t371aDBg2Ul5enChUqaNGiRQVuU758eZfW4OnpqUaNGqlRo0aKjIxUu3bttGjRouuGpddee01jx45V//79NWHCBJUpU0YeHh4aPny4QyNtl/tMmTLlqtOguPJ+ruzsbNuDCnv37tW5c+fk5+fn9H4u1/3YY49dNZQ2btzYbtnR0Trp0t/DmXbDMG64ruvtE4BzCHYA9Oeff0qSzp49K0mqWbOm1qxZo9atWzsVCFzh8mhiSkqKre3K0aPLPv30U7Vr104ffPCBXfvp06dVrly5625fs2ZNSVJgYKBDI243Kz4+Xjt27NAbb7yhF154QaNGjdJbb72Vr9/lkcS/2rVrl/z8/GyhOiAgQLm5uUVSt6PKly9fKHVd7e8HID/usQNucxcvXtTq1avl7e2tevXqSZJ69Oih3NxcTZgwIV//P//8U6dPn77p4/7www+6ePFivvav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t7d3gf1dpW7durZ7/S67chmAexDsABQKT09P7dixQ7///rs8PT3zrQ8ICNDIkSM1YsQILViwQHv37lVycrLefvtt2wMFtWvX1ubNm7Vq1Srt2rVLY8eOtQsQ+/fv1+jRo5WUlKSDBw9q9erV2r17t+rVqydJat++vTZv3qyFCxdq9+7dio+P16+//nrd2gcPHqyTJ0+qV69e2rRpk/bu3atVq1YpNjZWubm58vf314ABA/Tcc8/pu+++06+//qp+/frJw+P6H6mGYSg1NVWpqanav3+/5syZo1WrVumBBx646jZhYWFKTExUamqqTp06pfPnz2vIkCFat26dDh48qA0bNmjTpk229x0WFqazZ88qMTFR6enpOnfu3HXrcsYzzzyjDz74QAsWLNDu3bv16quv6pdffnH6oRUArselWACFJjAw8JrrJ0yYoPLlyyshIUH79u1TqVKl1Lx5c7344ouSpKeeekpbt25Vz549ZbFY1KtXLw0aNEjffPONJMnPz087d+7UggULdOLECVWsWFGDBw/WU089JUmKiYnR2LFj9fzzz+vChQvq37+/+vTpo+3bt1+zrkqVKmnDhg164YUX1KlTJ2VnZ6tatWq6++67beFtypQptku2AQEBevbZZ5WRkXHd30lmZqbtnjWr1apq1arplVde0QsvvHDVbaZOnaq4uDi99957qly5snbt2qUTJ06oT58+SktLU7ly5dS9e3eNHz9ektSqVSsNHDhQPXv21IkTJxQfH2+b8sQVHn30Ue3bt08jR47UhQsX1KNHD/Xr108bN2502TEA3BiLceUNKAAAOKljx44KCQnRhx9+6O5SgNsaI3YAAKecO3dOs2fPVkxMjDw9PfXxxx9rzZo1+vbbb91dGnDbY8QOAOCU8+fPq0uXLtq6dasuXLigunXrasyYMerevbu7SwNuewQ7AAAAk+CpWAAAAJMg2AEAAJgEwQ4AAMAkCHYAAAAmQbADAAAwCYIdAACASRDsAAAATIJgBwAAYBIEOwAAAJP4f21/7uQmkxzaAAAAAElFTkSuQmCC\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
```

### Comparing `JaqalPaq-1.1.1/examples/jaqal/bell_prep.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/bell_prep.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/bell_prep.py` & `JaqalPaq-1.2.0a1/examples/jaqal/bell_prep.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/bell_prep_q.py` & `JaqalPaq-1.2.0a1/examples/jaqal/bell_prep_q.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/bell_prep_spec.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/bell_prep_spec.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/nested_bit_flips.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/nested_bit_flips.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/nested_bit_flips_q.py` & `JaqalPaq-1.2.0a1/examples/jaqal/nested_bit_flips_q.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/one-qubit-rotations.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/one-qubit-rotations.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/one-qubit-rotations_q.py` & `JaqalPaq-1.2.0a1/examples/jaqal/one-qubit-rotations_q.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/pi_fracs.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/pi_fracs.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/pi_fracs_q.py` & `JaqalPaq-1.2.0a1/examples/jaqal/pi_fracs_q.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst.jaqal` & `JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst.jaqal`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst.py` & `JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/examples/jaqal/single_qubit_gst_q.py` & `JaqalPaq-1.2.0a1/examples/jaqal/single_qubit_gst_q.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/setup.cfg` & `JaqalPaq-1.2.0a1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = JaqalPaq
 author = Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 author_email = qscout@sandia.gov
 description = Python tools for Jaqal
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
@@ -30,27 +30,30 @@
 include = 
 	jaqalpaq.*
 	jaqalpaq
 where = src
 
 [options.extras_require]
 tests = pytest
-docs = Sphinx; sphinx-rtd-theme; JaqalPaq[pygsti-integration]; JaqalPaq-extras[qiskit,pyquil,projectq,pytket]==1.1.1
-pygsti-integration = pyGSTi>=0.9.10.1,<0.9.11
+docs = Sphinx; sphinx-rtd-theme; JaqalPaq[pygsti-integration]; JaqalPaq-extras[qiskit,pyquil,projectq,pytket]==1.2.0a1
+pygsti-integration = pyGSTi==0.9.10.1
 notebooks = openfermion==1.1.0; pyscf>=1.7.6,<1.7.7; openfermionpyscf==0.5; h5py<3.3
 
 [options.data_files]
 share/jaqalpaq/tests = 
 	tests/__init__.py
 share/jaqalpaq/examples = 
 	examples/usage_example.py
 share/jaqalpaq/tests/ipc = 
 	tests/ipc/__init__.py
-	tests/ipc/_mock_server.py
 	tests/ipc/test_ipc.py
+share/jaqalpaq/tests/run = 
+	tests/run/__init__.py
+	tests/run/batching_reference.py
+	tests/run/test_classical_cursor.py
 share/jaqalpaq/tests/core = 
 	tests/core/__init__.py
 	tests/core/abstractgate.py
 	tests/core/common.py
 	tests/core/gpf1.py
 	tests/core/randomize.py
 	tests/core/test_block.py
@@ -72,14 +75,15 @@
 share/jaqalpaq/examples/jaqal = 
 	examples/jaqal/Sxx_circuit.jaqal
 	examples/jaqal/Sxx_circuit_q.py
 	examples/jaqal/bell_prep.jaqal
 	examples/jaqal/bell_prep.py
 	examples/jaqal/bell_prep_q.py
 	examples/jaqal/bell_prep_spec.jaqal
+	examples/jaqal/bell_prep_subcircuit.jaqal
 	examples/jaqal/empty_loop.jaqal
 	examples/jaqal/empty_loop_outside_subcircuit.jaqal
 	examples/jaqal/empty_loop_q.py
 	examples/jaqal/empty_parallel.jaqal
 	examples/jaqal/empty_parallel_q.py
 	examples/jaqal/empty_prog.jaqal
 	examples/jaqal/empty_prog_q.py
@@ -111,14 +115,15 @@
 	examples/jaqal/prepare-measure.jaqal
 	examples/jaqal/sequential_block_in_parallel_loop.jaqal
 	examples/jaqal/sequential_loop_in_parallel.jaqal
 	examples/jaqal/sequential_loop_in_parallel_q.py
 	examples/jaqal/single_qubit_gst.jaqal
 	examples/jaqal/single_qubit_gst.py
 	examples/jaqal/single_qubit_gst_q.py
+	examples/jaqal/subcircuit.jaqal
 	examples/jaqal/two-qubit-nonadjacent.jaqal
 	examples/jaqal/two-qubit-nonadjacent_q.py
 	examples/jaqal/zero_loop.jaqal
 	examples/jaqal/zero_loop_q.py
 share/jaqalpaq/tests/emulator = 
 	tests/emulator/__init__.py
 	tests/emulator/test_forward_simulation.py
@@ -133,14 +138,15 @@
 	tests/core/reload/gpf1.py
 share/jaqalpaq/tests/jaqalparser = 
 	tests/jaqalparser/__init__.py
 	tests/jaqalparser/test_examples.py
 	tests/jaqalparser/test_jaqalpup_parser.py
 	tests/jaqalparser/test_parser.py
 share/jaqalpaq/examples/Tutorials = 
+	examples/Tutorials/BatchingExamples.ipynb
 	examples/Tutorials/Emulator_Demo.ipynb
 share/jaqalpaq/tests/core/algorithm = 
 	tests/core/algorithm/__init__.py
 	tests/core/algorithm/test_expand_macros.py
 	tests/core/algorithm/test_expand_subcircuits.py
 	tests/core/algorithm/test_fill_in_let.py
 	tests/core/algorithm/test_unit_timing.py
```

### Comparing `JaqalPaq-1.1.1/src/JaqalPaq.egg-info/PKG-INFO` & `JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaqalPaq
-Version: 1.1.1
+Version: 1.2.0a1
 Summary: Python tools for Jaqal
 Home-page: https://qscout.sandia.gov
 Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 Author-email: qscout@sandia.gov
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `JaqalPaq-1.1.1/src/JaqalPaq.egg-info/SOURCES.txt` & `JaqalPaq-1.2.0a1/src/JaqalPaq.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 pyproject.toml
 setup.cfg
 examples/usage_example.py
 examples/H2 (Molecular Hydrogen)/JaqalPaq_H2_Exemplar.ipynb
 examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Tapered_Exemplar.ipynb
 examples/HeH+ (Helium Hydride)/JaqalPaq_HeH+_Untapered_Exemplar.ipynb
 examples/LiH (Lithium Hydride)/JaqalPaq_LiH_Exemplar.ipynb
+examples/Tutorials/BatchingExamples.ipynb
 examples/Tutorials/Emulator_Demo.ipynb
 examples/jaqal/Sxx_circuit.jaqal
 examples/jaqal/Sxx_circuit_q.py
 examples/jaqal/bell_prep.jaqal
 examples/jaqal/bell_prep.py
 examples/jaqal/bell_prep_q.py
 examples/jaqal/bell_prep_spec.jaqal
+examples/jaqal/bell_prep_subcircuit.jaqal
 examples/jaqal/empty_loop.jaqal
 examples/jaqal/empty_loop_outside_subcircuit.jaqal
 examples/jaqal/empty_loop_q.py
 examples/jaqal/empty_parallel.jaqal
 examples/jaqal/empty_parallel_q.py
 examples/jaqal/empty_prog.jaqal
 examples/jaqal/empty_prog_q.py
@@ -51,14 +53,15 @@
 examples/jaqal/prepare-measure.jaqal
 examples/jaqal/sequential_block_in_parallel_loop.jaqal
 examples/jaqal/sequential_loop_in_parallel.jaqal
 examples/jaqal/sequential_loop_in_parallel_q.py
 examples/jaqal/single_qubit_gst.jaqal
 examples/jaqal/single_qubit_gst.py
 examples/jaqal/single_qubit_gst_q.py
+examples/jaqal/subcircuit.jaqal
 examples/jaqal/two-qubit-nonadjacent.jaqal
 examples/jaqal/two-qubit-nonadjacent_q.py
 examples/jaqal/zero_loop.jaqal
 examples/jaqal/zero_loop_q.py
 examples/jaqal/spec_samples/bell.jaqal
 examples/jaqal/spec_samples/blocks.jaqal
 examples/jaqal/spec_samples/compile.jaqal
@@ -85,51 +88,57 @@
 src/jaqalpaq/core/branch.py
 src/jaqalpaq/core/circuit.py
 src/jaqalpaq/core/circuitbuilder.py
 src/jaqalpaq/core/constant.py
 src/jaqalpaq/core/gate.py
 src/jaqalpaq/core/gatedef.py
 src/jaqalpaq/core/identifier.py
+src/jaqalpaq/core/locus.py
 src/jaqalpaq/core/macro.py
 src/jaqalpaq/core/parameter.py
 src/jaqalpaq/core/register.py
-src/jaqalpaq/core/result.py
 src/jaqalpaq/core/stretch.py
 src/jaqalpaq/core/usepulses.py
 src/jaqalpaq/core/algorithm/__init__.py
 src/jaqalpaq/core/algorithm/expand_macros.py
 src/jaqalpaq/core/algorithm/expand_subcircuits.py
 src/jaqalpaq/core/algorithm/fill_in_let.py
 src/jaqalpaq/core/algorithm/fill_in_map.py
 src/jaqalpaq/core/algorithm/unit_timing.py
 src/jaqalpaq/core/algorithm/used_qubit_visitor.py
 src/jaqalpaq/core/algorithm/visitor.py
 src/jaqalpaq/core/algorithm/walkers.py
 src/jaqalpaq/emulator/__init__.py
+src/jaqalpaq/emulator/_import.py
 src/jaqalpaq/emulator/_validator.py
 src/jaqalpaq/emulator/backend.py
-src/jaqalpaq/emulator/frontend.py
 src/jaqalpaq/emulator/unitary.py
 src/jaqalpaq/emulator/pygsti/__init__.py
 src/jaqalpaq/emulator/pygsti/backends.py
 src/jaqalpaq/emulator/pygsti/circuit.py
 src/jaqalpaq/emulator/pygsti/model.py
 src/jaqalpaq/generator/__init__.py
 src/jaqalpaq/generator/generator.py
 src/jaqalpaq/ipc/__init__.py
-src/jaqalpaq/ipc/ipc.py
+src/jaqalpaq/ipc/client.py
+src/jaqalpaq/ipc/server.py
 src/jaqalpaq/parser/__init__.py
 src/jaqalpaq/parser/identifier.py
 src/jaqalpaq/parser/parser.py
 src/jaqalpaq/parser/slyparse.py
 src/jaqalpaq/qsyntax/__init__.py
 src/jaqalpaq/qsyntax/compile.py
 src/jaqalpaq/qsyntax/qsyntax.py
 src/jaqalpaq/run/__init__.py
-src/jaqalpaq/run/run.py
+src/jaqalpaq/run/_view.py
+src/jaqalpaq/run/backend.py
+src/jaqalpaq/run/classical_cursor.py
+src/jaqalpaq/run/cursor.py
+src/jaqalpaq/run/frontend.py
+src/jaqalpaq/run/result.py
 tests/__init__.py
 tests/core/__init__.py
 tests/core/abstractgate.py
 tests/core/common.py
 tests/core/gpf1.py
 tests/core/randomize.py
 tests/core/test_block.py
@@ -157,15 +166,17 @@
 tests/core/reload/gpf1.py
 tests/emulator/__init__.py
 tests/emulator/test_forward_simulation.py
 tests/emulator/test_jaqal_files.py
 tests/generator/__init__.py
 tests/generator/test_generator.py
 tests/ipc/__init__.py
-tests/ipc/_mock_server.py
 tests/ipc/test_ipc.py
 tests/jaqalparser/__init__.py
 tests/jaqalparser/test_examples.py
 tests/jaqalparser/test_jaqalpup_parser.py
 tests/jaqalparser/test_parser.py
 tests/qsyntax/__init__.py
-tests/qsyntax/test_qsyntax.py
+tests/qsyntax/test_qsyntax.py
+tests/run/__init__.py
+tests/run/batching_reference.py
+tests/run/test_classical_cursor.py
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/_cli.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/_cli.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/_import.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,19 @@
     sys.modules[mod_name] = module
     spec.loader.exec_module(module)
 
     return module
 
 
 def jaqal_import(
-    mod_name, obj_name, import_path, reload_module="relative_only", full_reload=True
+    mod_name,
+    obj_name,
+    import_path=None,
+    reload_module="relative_only",
+    full_reload=True,
 ):
     assert reload_module in (True, False, "relative_only")
 
     if mod_name.startswith("."):
         relative = True
         reload_module = not (reload_module is False)
         mod_name = mod_name[1:]
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/__init__.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/__init__.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/__init__.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/expand_macros.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/expand_macros.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,37 +42,47 @@
         return obj
 
     def visit_Circuit(self, circuit):
         """Return a new Circuit with the same metadata and normalized
         gates."""
 
         self.macros = circuit.macros
-        new_circuit = Circuit(native_gates=circuit.native_gates)
+        new_circuit = Circuit(
+            native_gates=circuit.native_gates,
+            name=f"(expanded) {circuit._name_hint}" if circuit._name_hint else None,
+        )
         if self.preserve_definitions:
             new_circuit.macros.update(circuit.macros)
         new_circuit.constants.update(circuit.constants)
         new_circuit.registers.update(circuit.registers)
         new_circuit.body.statements.extend(self.visit(circuit.body).statements)
+        new_circuit.usepulses.extend(circuit.usepulses)
         return new_circuit
 
     def visit_LoopStatement(self, loop):
         return LoopStatement(loop.iterations, self.visit(loop.statements))
 
     def visit_BlockStatement(self, block):
         new_statements = []
         for stmt in block.statements:
             new_stmt = self.visit(stmt)
             if (
                 isinstance(new_stmt, BlockStatement)
+                and (not new_stmt.subcircuit)
                 and new_stmt.parallel == block.parallel
             ):
                 new_statements.extend(new_stmt.statements)
             else:
                 new_statements.append(new_stmt)
-        return BlockStatement(parallel=block.parallel, statements=new_statements)
+        return BlockStatement(
+            parallel=block.parallel,
+            subcircuit=block.subcircuit,
+            iterations=block.iterations,
+            statements=new_statements,
+        )
 
     def visit_GateStatement(self, gate):
         return replace_gate(gate, self.macros)
 
 
 def replace_gate(gate, macros):
     """Replace a gate with its definition in macros, or return the gate if
@@ -101,28 +111,30 @@
     def visit_Macro(self, macro: Macro):
         self.parameters = macro.parameters
         return self.visit(macro.body)
 
     def visit_BlockStatement(self, block: BlockStatement):
         return BlockStatement(
             parallel=block.parallel,
+            subcircuit=block.subcircuit,
+            iterations=block.iterations,
             statements=[self.visit(stmt) for stmt in block.statements],
         )
 
     def visit_LoopStatement(self, loop: LoopStatement):
         return LoopStatement(
             iterations=self.visit(loop.iterations),
             statements=self.visit(loop.statements),
         )
 
     def visit_GateStatement(self, gate: GateStatement):
         new_parameters = {
             name: self.visit(param) for name, param in gate.parameters.items()
         }
-        new_gate = GateStatement(gate.gate_def, new_parameters)
+        new_gate = gate.gate_def(**new_parameters)
         return replace_gate(new_gate, self.macros)
 
     def visit_Parameter(self, param: Parameter):
         if param.name in self.arguments:
             arg = self.arguments[param.name]
             # This check will basically always pass as Jaqal has no
             # way of type annotating macro arguments.
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/expand_subcircuits.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/expand_subcircuits.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 
     def visit_Circuit(self, circuit):
         new_circuit = Circuit(native_gates=circuit.native_gates)
         new_circuit.macros.update(circuit.macros)
         new_circuit.constants.update(circuit.constants)
         new_circuit.registers.update(circuit.registers)
         new_circuit.body.statements.extend(self.visit(circuit.body).statements)
+        new_circuit.usepulses.extend(circuit.usepulses)
         return new_circuit
 
     def visit_LoopStatement(self, loop):
         return LoopStatement(loop.iterations, self.visit(loop.statements))
 
     def visit_BlockStatement(self, block):
         if block.subcircuit:
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/fill_in_let.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/fill_in_let.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,23 +53,27 @@
             "circuit",
             *circuit.constants.values(),
             *registers,
             *macros,
             *statements,
         ]
         inject_pulses = circuit.native_gates or None
-        return circuitbuilder.build(sexpr, inject_pulses=inject_pulses)
+        new_circuit = circuitbuilder.build(sexpr, inject_pulses=inject_pulses)
+        new_circuit.usepulses.extend(circuit.usepulses)
+        return new_circuit
 
     def visit_BlockStatement(self, block):
         if block.parallel:
-            block_type = "parallel_block"
+            sexpr = ["parallel_block"]
+        elif block.subcircuit:
+            sexpr = ["subcircuit_block", block.iterations]
         else:
-            block_type = "sequential_block"
+            sexpr = ["sequential_block"]
 
-        sexpr = [block_type, *[self.visit(stmt) for stmt in block.statements]]
+        sexpr.extend(self.visit(stmt) for stmt in block.statements)
         return sexpr
 
     def visit_LoopStatement(self, loop):
         sexpr = ["loop", self.visit(loop.iterations), self.visit(loop.statements)]
         return sexpr
 
     def visit_CaseStatement(self, case):
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/fill_in_map.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/fill_in_map.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,17 @@
             "circuit",
             *circuit.constants.values(),
             *circuit.registers.values(),
             *macros,
             *statements,
         ]
         inject_pulses = circuit.native_gates or None
-        return circuitbuilder.build(sexpr, inject_pulses=inject_pulses)
+        new_circuit = circuitbuilder.build(sexpr, inject_pulses=inject_pulses)
+        new_circuit.usepulses.extend(circuit.usepulses)
+        return new_circuit
 
     def visit_BlockStatement(self, block):
         if block.parallel:
             block_type = "parallel_block"
         else:
             block_type = "sequential_block"
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/unit_timing.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/unit_timing.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/used_qubit_visitor.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/used_qubit_visitor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/visitor.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/visitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,43 +26,46 @@
         self.started = trace is None
         self.trace = trace
         self.address = []
         super().__init__(*args, **kwargs)
 
     def trace_statements(self, statements):
         address = self.address
+        if self.trace:
+            start, end = (list(p.address) for p in self.trace)
+
         if self.started:
             n = 0
             address.append(n)
         else:
-            start = self.trace.start
             if start[: len(address)] != address:
                 assert start[: len(address)] > address
                 return
             n = start[len(address)]
             address.append(n)
             if start == address:
                 self.started = True
 
         len_address = len(address)
 
-        if self.trace and (address > self.trace.end):
+        if self.trace and (address[: len(end)] > end):
             # This is the measure -> prepare case
             while n < len(statements):
                 yield n, statements[n]
                 assert len(address) == len_address
                 n = address[-1] = n + 1
             n = address[-1] = 0
 
         while n < len(statements):
             yield n, statements[n]
             assert len(address) == len_address
             n = address[-1] = n + 1
-            if self.trace and (address > self.trace.end):
+            if self.trace and (address[: len(end)] > end):
                 break
+
         address.pop()
 
     def visit_default(self, obj, *args, **kwargs):
         """Method called when no method matches. Override to provide default behavior.
 
         :param object obj: The Jaqal core type object to visit.
         :raises JaqalError: Because this method should never be called unless overriden.
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/algorithm/walkers.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/algorithm/walkers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 from collections import defaultdict
 from itertools import chain
 
 from .used_qubit_visitor import UsedQubitIndicesVisitor
 from .visitor import Visitor
+from jaqalpaq.core.locus import Locus
 from jaqalpaq.error import JaqalError
 from jaqalpaq.core.block import BlockStatement, LoopStatement
+from jaqalpaq.core.branch import BranchStatement
 
 
 class Trace:
-    """Describes a portion of a Circuit traced out by start and stop locations."""
+    """(deprecated) Describes a portion of a Circuit traced out by start and stop locations."""
 
     def __init__(self, start=None, end=None, used_qubits=None):
         if start is None:
             self.start = []
         else:
             self.start = start
 
@@ -64,26 +66,32 @@
 
     # While this *is* the behavior of DiscoverSubcircuits, this flag does nothing.
     validate_parallel = True
 
     def __init__(self, *args, p_gate="prepare_all", m_gate="measure_all", **kwargs):
         super().__init__(*args, **kwargs)
         self.current = None
+        self.qubits = None
         self.subcircuits = []
         self.p_gate = p_gate
         self.m_gate = m_gate
 
     def visit_Circuit(self, circuit, context=None):
         # All qubits will be used in every subcircuit, because it is bounded by
         # prepare_all and measure_all.  In the future, we presumably will employ the used
         # qubit functionality of the superclass, and separately report the measured
-        # qubits.  But we do not support partial measurements yet.
+        # qubits.  But we do not support mid-circuit measurements yet.
+        if self.qubits is not None:
+            raise RuntimeError("Cannot reuse DiscoverSubcircuit object")
         self.qubits = list(chain.from_iterable(circuit.fundamental_registers()))
         super().visit_Circuit(circuit, context=context)
 
+        if self.current is not None:
+            raise JaqalError("Subcircuit did not end")
+
         subcircuits = self.subcircuits
         if len(subcircuits) == 0:
             return ()
 
         if subcircuits[-1].end is None:
             return subcircuits[:-1]
         else:
@@ -102,113 +110,156 @@
         # Calling UsedQubitIndicesVisitor as super() is
         # far too inflexible for the purposes here.
         indices = defaultdict(set)
 
         count = len(self.subcircuits)
         had_started = self.current is not None
 
+        if block.subcircuit:
+            self.start_trace(context=context)
+
         # XXX: using a trace restriction here is untested
         for n, stmt in self.trace_statements(block.statements):
             self.merge_into(
                 indices, self.visit(stmt, context=context), disjoint=block.parallel
             )
 
-        if had_started and (reps > 1) and (len(self.subcircuits) != count):
+        if block.subcircuit:
+            self.end_trace(context=context)
+
+        if had_started and (len(self.subcircuits) != count) and (reps > 1):
             raise JaqalError("measure_all -> prepare_all not supported in loops")
 
         return indices
 
     def visit_GateStatement(self, gate, context=None):
         if gate.name == self.p_gate:
-            # We allow for multiple prepare_all's in a row. But gates between those
-            # prepare_all's do nothing. Notice also, we would not yet know what the
-            # measured or used qubits are, if we had partial measurements.  That would
-            # have to wait until the measurement.
-            c = self.current = Trace(self.address[:])
+            self.start_trace(context=context)
         elif gate.name == self.m_gate:
-            if self.current is None:
-                raise JaqalError(f"{self.p_gate} must follow a {self.m_gate}")
-            self.current.end = self.address[:]
-            self.current.used_qubits = self.qubits
-            self.subcircuits.append(self.current)
-            self.current = None
+            self.end_trace(context=context)
         else:
             if self.current is None:
                 raise JaqalError(f"gates must follow a {self.p_gate}")
 
         return super().visit_GateStatement(gate, context=context)
 
+    def start_trace(self, context=None):
+        # We do not allow for multiple prepare_all's in a row.  Notice also, if we
+        # were doing mid-circuit measurements, that we would not know what the measured
+        # or used qubits are until until the measurement.
+        if self.current is not None:
+            raise JaqalError("Nested subcircuit are not allowed")
+        self.current = Trace(self.address[:])
+
+    def end_trace(self, context=None):
+        if self.current is None:
+            raise JaqalError(f"{self.m_gate} must follow a {self.p_gate}")
+        current = self.current
+        current.end = self.address[:]
+        current.used_qubits = self.qubits
+        self.subcircuits.append(current)
+        self.current = None
 
-class TraceVisitor(Visitor):
-    """Call process_trace at the start of every trace in execution order."""
 
-    def __init__(self, traces):
-        self.traces = traces
+def discover_subcircuits(circuit):
+    ds = DiscoverSubcircuits()
+    for tr in ds.visit(circuit):
+        locus = Locus.from_address(circuit, tr.start)
+        if tr.start != tr.end:
+            end_locus = Locus.from_address(circuit, tr.end)
+        else:
+            end_locus = locus
+        last = False
+        for parent in locus.lineage:
+            if last:
+                raise JaqalError("Cannot nest subcircuit in any other block")
+            obj = parent.object
+            if isinstance(obj, BranchStatement):
+                raise JaqalError("Cannot start subcircuit inside a branch")
+            elif isinstance(obj, BlockStatement) and obj.subcircuit:
+                last = True
+        yield locus, end_locus
+
+
+class CircuitWalker(Visitor):
+    """(internal) Walk a circuit in execution order, yielding at each breakpoint.
+
+    This requires the breakpoints to be given in the order they are
+    found by DiscoverSubcircuits.
+    """
+
+    def __init__(self, breakpoints):
+        self.breakpoints = breakpoints
         self.address = []
         self.index = 0
 
-    def process_trace(self):
-        raise NotImplementedError()
-
     def visit_Circuit(self, circuit):
-        if len(self.traces) == 0:
+        if len(self.breakpoints) == 0:
             return
-        self.objective = self.traces[self.index].start
+        self.objective = list(self.breakpoints[self.index].address)
 
-        return self.visit(circuit.body)
+        yield from self.visit(circuit.body)
 
     def visit_BlockStatement(self, block):
+        if block.subcircuit:
+            yield from self.do_loop(self.iterations, block)
+        else:
+            yield from self.do_block(block)
+
+    def do_block(self, block):
         first = True
         address = self.address
         while self.objective:
             if address != self.objective[: len(address)]:
                 assert not first
                 assert address < self.objective[: len(address)]
                 return
 
             first = False
 
             n = self.objective[len(address)]
             nxt = block.statements[n]
             if (len(address) + 1) == len(self.objective):
-                self.process_trace()
+                yield self.index
                 self.index += 1
-                if self.index == len(self.traces):
+                if self.index == len(self.breakpoints):
                     # We've found all the traces.  We're done!
                     self.objective = None
                     return
                 else:
-                    self.objective = self.traces[self.index].start
+                    self.objective = list(self.breakpoints[self.index].address)
             else:
                 address.append(n)
-                self.visit(nxt)
+                yield from self.visit(nxt)
                 address.pop()
 
     def visit_LoopStatement(self, loop):
+        yield from self.do_loop(loop.iterations, loop.statements)
+
+    def do_loop(self, iterations, block):
         # store the walk status
         index = self.index
         address = self.address[:]
         objective = self.objective
 
         # loop over the classical parts
-        for n in range(loop.iterations):
+        for n in range(iterations):
             # Restore the walk status at the start of every loop
             self.objective = objective
             self.address[:] = address[:]
             self.index = index
-            self.visit(loop.statements)
+            yield from self.visit(block)
 
     def visit_CaseStatement(self, case):
-        # store the walk status
-        index = self.index
-        address = self.address[:]
-        objective = self.objective
-
-        # loop over the classical parts
-        # Restore the walk status at the start of every loop
-        self.objective = objective
-        self.address[:] = address[:] + case.state
-        self.index = index
-        self.visit(case.statements)
+        raise NotImplementedError("case statements are not supporetd")
 
     def visit_BranchStatement(self, branch):
         raise JaqalError("Tracing a circuit with a branch not supported")
+
+
+def walk_circuit(circuit, breakpoints):
+    """Walk a circuit in execution order, yielding at each breakpoint.
+
+    This requires the breakpoints to be given in the order they are
+    found by DiscoverSubcircuits.
+    """
+    yield from CircuitWalker(breakpoints).visit(circuit)
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/block.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/block.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/branch.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/branch.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/circuit.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/circuit.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,21 +31,28 @@
     :raises JaqalError: If `native_gates` is a dict and any gate's name doesn't match its
         dictionary key.
     :raises JaqalError: If any of the `native_gates` aren't :class:`GateDefinition`.  For
         example, if a macro is passed as a native gate.
 
     """
 
-    def __init__(self, native_gates=None):
+    def __init__(self, native_gates=None, *, name=None):
         self._constants = {}
         self._macros = {}
         self._registers = {}
         self._native_gates = normalize_native_gates(native_gates)
         self._body = BlockStatement()
         self._usepulses = []
+        self._name_hint = name
+
+    def _repr_pretty_(self, printer, cycle=False):
+        if self._name_hint:
+            printer.text(f"<Circuit {self._name_hint}>")
+        else:
+            printer.text(repr(self))
 
     def __repr__(self):
         return f"Circuit(usepulses={self._usepulses}, constants={self._constants}, macros={self._macros}, native_gates={self._native_gates}, registers={self._registers}, body={self._body})"
 
     def __eq__(self, other):
         try:
             return (
@@ -100,23 +107,30 @@
         """
         :returns: all of the circuit's registers that correspond to ``register`` statements, that is, all those that are not aliases for some other register.
         :rtype: list(Register)
         """
         return [r for r in self.registers.values() if r.fundamental]
 
 
-def normalize_native_gates(native_gates):
+def normalize_native_gates(native_gates, origin=False):
     """Takes in the different ways that native gates can be represented and
     returns a dictionary.
 
     :param native_gates: A list or dict of gates, or None.
     :type native_gates: Optional[dict] or Optional[list]
+    :param origin: Assign an originating Jaqal module for the gate definitions.
+       If unset (or False), do not change the existing origin.
+    :type origin: str or None (optional)
+
     """
     native_gates = native_gates or {}
     if not isinstance(native_gates, dict):
         # This covers all iterables like list and tuple
         native_gates = {gate.name: gate for gate in native_gates}
     if any(name != gate.name for name, gate in native_gates.items()):
         raise JaqalError("Native gate dictionary key did not match its name")
     if any(not isinstance(gate, GateDefinition) for gate in native_gates.values()):
         raise JaqalError("Native gates must be GateDefinition instances")
+    if origin is not False:
+        for gate in native_gates.values():
+            gate._origin = origin
     return native_gates
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/circuitbuilder.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/circuitbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,15 +407,15 @@
     def __init__(self, context, gate_context):
         self.context = context
         self.gate_context = gate_context
 
     def visit_Macro(self, macro):
         changed, new_body = self.visit(macro.body)
         if changed:
-            return changed, Macro(macro.name, macro.parameters, new_body)
+            return changed, macro.copy(body=new_body)
         else:
             return changed, macro
 
     def visit_BlockStatement(self, block):
         changed = False
         new_statements = []
         for stmt in block.statements:
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/constant.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/constant.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/gate.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/gate.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/gatedef.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/gatedef.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,37 +2,42 @@
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 from collections import OrderedDict
 
 from jaqalpaq.error import JaqalError
 from .gate import GateStatement
 
+import warnings
+
 
 class AbstractGate:
     """
     The abstract base class for gate definitions. Everything here can be used whether the
     gate is defined by a macro in Jaqal, or is a gate defined by a pulse sequence in a
     gate definition file.
 
     :param str name: The name of the gate.
     :param parameters: What arguments (numbers, qubits, etc) the gate should be called
         with. If None, the gate takes no parameters.
-    :param function ideal_unitary: A function mapping a list of all classical arguments to
-        a numpy 2D array representation of the gate's ideal action in the computational
-        basis.
     :type parameters: list(Parameter) or None
+    :param function ideal_unitary: (deprecated) A function mapping a list of all classical
+        arguments to a numpy 2D array representation of the gate's ideal action in the
+        computational basis.
     """
 
     def __init__(self, name, parameters=None, ideal_unitary=None):
         self._name = name
         if parameters is None:
             self._parameters = []
         else:
             self._parameters = parameters
-        self._ideal_unitary = ideal_unitary
+
+        if ideal_unitary is not None:
+            warnings.warn("Define unitary in <path>.jaqal_action", DeprecationWarning)
+            self._ideal_unitary = ideal_unitary
 
     def __repr__(self):
         return f"{type(self).__name__}({self.name}, {self.parameters})"
 
     def __eq__(self, other):
         try:
             return self.name == other.name and self.parameters == other.parameters
@@ -47,15 +52,15 @@
     @property
     def parameters(self):
         """
         What arguments (numbers, qubits, etc) the gate should be called with.
         """
         return self._parameters
 
-    def call(self, *args, **kwargs):
+    def parse_parameters(self, *args, **kwargs):
         """
         Create a :class:`GateStatement` that calls this gate.
         The arguments to this method will be the arguments the gate is called with.
         If all arguments are keyword arguments, their names should match the names of this
         gate's parameters, and the values will be passed accordingly.
         If all arguments are positional arguments, each value will be passed to the next
         parameter in sequence.
@@ -95,50 +100,79 @@
             )
         if len(self.parameters) != len(params):
             raise JaqalError(
                 f"Bad argument count: expected {len(self.parameters)}, found {len(params)}"
             )
         for param in self.parameters:
             param.validate(params[param.name])
-        return GateStatement(self, params)
+        return params
+
+    def call(self, *args, **kwargs):
+        """(deprecated) use gatedef(*args) instead"""
+        warnings.warn("Use gatedef() instead of gatedef.call()", DeprecationWarning)
+        return self(*args, **kwargs)
 
     def __call__(self, *args, **kwargs):
-        return self.call(*args, **kwargs)
+        params = self.parse_parameters(*args, **kwargs)
+        return GateStatement(self, params)
 
-    def copy(self, *, name=None, parameters=None, ideal_unitary=None):
+    def copy(
+        self,
+        *,
+        name=None,
+        parameters=None,
+        ideal_unitary=False,
+        origin=False,
+        unitary=None,
+    ):
         """Returns a shallow copy of the gate or gate definition.
 
         :param name: (optional) change the name in the copy.
         :param parameters: (optional) change the parameters in the copy.
         """
 
         kls = type(self)
         copy = kls.__new__(kls)
         copy.__dict__ = self.__dict__.copy()
         if name is not None:
             copy._name = name
         if parameters is not None:
             copy._parameters = parameters
-        if ideal_unitary is not None:
+        if ideal_unitary is not False:
             copy._ideal_unitary = ideal_unitary
+        if origin is not False:
+            copy._origin = origin
+        if unitary is not None:
+            copy._unitary = unitary
 
         return copy
 
 
 class GateDefinition(AbstractGate):
     """
     Base: :class:`AbstractGate`
 
     Represents a gate that's implemented by a pulse sequence in a gate definition file.
+    :param bool unitary: Whether or not the gate represents a purely unitary action.
     """
 
+    def __init__(self, *args, origin=None, unitary=True, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._origin = origin
+        self._unitary = unitary
+
     @property
-    def ideal_unitary(self):
-        """The ideal unitary action of the gate on its target qubits"""
-        return self._ideal_unitary
+    def origin(self):
+        """The Jaqal module in which this gate is defined."""
+        return self._origin
+
+    @property
+    def unitary(self):
+        """Whether or not the gate is (ideally) unitary."""
+        return self._unitary
 
     @property
     def used_qubits(self):
         """Return the parameters in this gate that are qubits. Subclasses may
         return the special symbol `all` indicating they operate on all
         qubits. Otherwise this is identical to quantum_parameters."""
         for p in self.parameters:
@@ -173,41 +207,54 @@
         """
         try:
             return [param for param in self.parameters if param.classical]
         except JaqalError:
             pass
         raise JaqalError("Gate {self.name} has a parameter with unknown type")
 
+    @property
+    def ideal_unitary(self):
+        """(deprecated) The ideal unitary action of the gate on its target qubits"""
+        warnings.warn("Use get_ideal_action instead", DeprecationWarning)
+        from jaqalpaq.emulator._import import get_ideal_action
+
+        return get_ideal_action(self)
+
 
 class IdleGateDefinition(GateDefinition):
     """
-    Base: :class:`AbstractGate`
+    Base: :class:`GateDefinition`
 
     Represents a gate that merely idles for some duration.
     """
 
-    # Idle gates are a scheduling mechanism.  Formally, they act on no qubits.
-    _ideal_unitary = None
-
     def __init__(self, gate, name=None):
         # Special case handling of prepare and measure gates
         if gate.name in ("prepare_all", "measure_all"):
             raise JaqalError(f"Cannot make an idle gate for {gate.name}")
+        super().__init__(
+            name=name if name else f"I_{gate.name}",
+            parameters=gate._parameters,
+            origin=gate.origin,
+            unitary=True,
+        )
         self._parent_def = gate
-        self._parameters = gate._parameters
-        self._name = name if name else f"I_{gate.name}"
 
     @property
     def used_qubits(self):
         """Iterates over the qubits used by an idle gate: nothing.
 
         The idle operation does not act on any qubits.
         """
         yield from ()
 
+    def __call__(self, *args, **kwargs):
+        params = self._parent_def.parse_parameters(*args, **kwargs)
+        return GateStatement(self, params)
+
 
 class BusyGateDefinition(GateDefinition):
     """
     Base: :class:`AbstractGate`
 
     Represents an operation that cannot be parallelized with any other operation.
     """
@@ -224,17 +271,11 @@
       gates available.
     :return:  A list of GateDefinitions including both the active gates passed, and their
       associated idle gates.
     """
     gates = {}
     for n, g in active_gates.items():
         gates[n] = g
-
-        try:
-            g = IdleGateDefinition(g)
-        except JaqalError:
-            # Ignore gates that do not have corresponding idle gates
-            pass
-        else:
-            gates[g.name] = g
+        idle_gate = IdleGateDefinition(g)
+        gates[idle_gate.name] = idle_gate
 
     return gates
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/identifier.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/identifier.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/macro.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/macro.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,7 +37,21 @@
 
     @property
     def body(self):
         """
         A :class:`BlockStatement` that implements the macro.
         """
         return self._body
+
+    def copy(self, *, body=None, **kwargs):
+        """Returns a shallow copy of the gate or gate definition.
+
+        :param name: (optional) change the name in the copy.
+        :param parameters: (optional) change the parameters in the copy.
+        :param body: (optional) change the body of the macro in the copy
+        """
+        copy = super().copy(**kwargs)
+
+        if body is not None:
+            copy._body = body
+
+        return copy
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/parameter.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/parameter.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/register.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/register.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/core/usepulses.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/core/usepulses.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/_validator.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import OrderedDict
 
 import numpy as np
 
 from jaqalpaq.error import JaqalError
 from jaqalpaq.parser import JaqalParseError, parse_jaqal_string
 
-from .frontend import run_jaqal_circuit
+from jaqalpaq.run.frontend import run_jaqal_circuit
 
 
 def assertAlmostEqual(a, b):
     if np.isclose(a, b):
         return
 
     raise ValueError(f"{a} and {b} differ by {a-b}")
@@ -50,19 +50,24 @@
         )
     )
 
     emit("\n// EXPECTED PROBABILITIES")
 
     for sc_index, se in enumerate(exe.subcircuits):
         emit(f"// SUBCIRCUIT {sc_index}")
-        for n, ((s, ps), p) in enumerate(
-            zip(se.probability_by_str.items(), se.probability_by_int)
-        ):
-            assert ps == p
-            emit(f"// {s} {n} {p}")
+        total = 0
+        count = 0
+        for n, (s, ps) in enumerate(se.probability_by_str.items()):
+            total += ps
+            if not np.isclose(ps, 0):
+                count += 1
+                assertEqual(ps, se.simulated_probabilities[s])
+
+            emit(f"// {s} {n} {ps}")
+        assertAlmostEqual(total, 1)
 
     return "\n".join(output)
 
 
 def parse_jaqal_validation(txt):
     """[undocumented] parse Jaqal validation comments
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/backend.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,94 +1,43 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 import abc
 
 from numpy.random import choice
 
-from jaqalpaq.core.result import ExecutionResult, Readout
-from jaqalpaq.core.result import ProbabilisticSubcircuit
-from jaqalpaq.core.algorithm.walkers import TraceVisitor, DiscoverSubcircuits
+from jaqalpaq.error import JaqalError
+from jaqalpaq.core.locus import Locus
+from jaqalpaq.core.block import BlockStatement
+from jaqalpaq.core.algorithm.walkers import walk_circuit, discover_subcircuits
+from jaqalpaq.core.algorithm import fill_in_let
 
-
-class AbstractJob:
-    """Abstract Jaqal Compute Job"""
-
-    def __init__(self, backend, circuit):
-        self.backend = backend
-        self.circuit = circuit
-
-    def __repr__(self):
-        return f"<{type(self)} of {self.backend}>"
-
-    @abc.abstractmethod
-    def execute(self):
-        """Executes the job on the backend"""
-
-
-class AbstractBackend:
-    """Abstract Emulator Backend"""
-
-    @abc.abstractmethod
-    def __call__(self, circ):
-        """Creates a job object for circ
-
-        :param Circuit circ: circuit to run
-        """
-
-    def get_n_qubits(self, circ):
-        """Returns the number of qubits the backend will simulate/emulate.
-
-        Specifically, it will be the number of qubits in the considered circuit.
-
-        :param circ: The circuit object being emulated/simulated.
-        """
-
-        registers = circ.fundamental_registers()
-
-        try:
-            (register,) = registers
-        except ValueError:
-            raise NotImplementedError("Multiple fundamental registers unsupported.")
-
-        return register.size
+from jaqalpaq.run import result, cursor
+from jaqalpaq.run.backend import IndependentSubcircuitsBackend, AbstractBackend
 
 
 class ExtensibleBackend(AbstractBackend):
     """Abstract mixin providing an interface for extending a backend.
 
     Every gate to be emulated should have a corresponding gate_{name} and
       gateduration_{name} method defined.
     """
 
-    def __init__(self, n_qubits, stretched_gates=None, **kwargs):
+    def __init__(self, *args, stretched_gates=None, **kwargs):
         """(abstract) Perform part of the construction of a noisy model.
 
-        :param n_qubits: The number of qubits to simulate
         :param stretched_gates: (default False)  Add stretched gates to the model:
           - If None, do not modify the gates.
           - If 'add', add gates with '_stretched' appended that take an extra parameter,
             a stretch factor.
           - Otherwise, stretched_gates must be the numerical stretch factor that is
             applied to all gates (no extra stretched gates are added
         """
-        self.n_qubits = n_qubits
+        super().__init__(*args, **kwargs)
         self.stretched_gates = stretched_gates
-        model, durations = self.build_model()
-        super().__init__(model=model, gate_durations=durations, **kwargs)
-
-    def get_n_qubits(self, circ):
-        """Returns the number of qubits the backend will be simulating.
-
-        :param circ: The circuit object being emulated/simulated.
-        """
-        circuit_qubits = super().get_n_qubits(circ)
-        if circuit_qubits > self.n_qubits:
-            raise ValueError(f"{self} emulates fewer qubits than {circ} uses")
-        return self.n_qubits
 
     def set_defaults(self, kwargs, **defaults):
         """Set parameters from a list of defaults and function kwargs.
 
         For every value passed as a keyword argument (into **defaults), set it in the
           object's namespace.  Values in kwargs overrided the default.  Values used from
           kwargs are removed from kwargs.
@@ -133,75 +82,67 @@
           adds a corresponding entry in the returned dictionary, keyed by the associated
           gate name, of the gate model (i.e., the noisy process model) and the duration
           that the gate operates.
         : return dict: A dictionary of the models of the gates
         """
         gate_models = {}
 
-        for gate_name in type(self).__dict__:
+        for gate_name in dir(type(self)):
             if not gate_name.startswith("gate_"):
                 continue
 
             name = gate_name[5:]
             gate_models[name] = (
                 getattr(self, gate_name),
                 getattr(self, f"gateduration_{name}"),
             )
 
         return gate_models
 
 
-class IndependentSubcircuitsEmulatorWalker(TraceVisitor):
-    def __init__(self, traces, subcircuits):
-        """(internal) Instantiates an EmulationWalker.
-
-        Produce emulated output sampled from a given probability distribution.
-
-        :param List[Trace] traces: the prepare_all/measure_all subcircuits
-        :param List[List[Float]] probabilities: the probabilities of each outcome
-
-        """
-        super().__init__(traces)
-        self.results = []
-        self.readout_index = 0
-        self.subcircuits = subcircuits
-        # This is only valid because we must always do measure_all.
-        if self.traces:
-            self.qubits = len(self.traces[0].used_qubits)
-
-    def process_trace(self):
-        subcircuit = self.subcircuits[self.index]
-        nxt = choice(2**self.qubits, p=subcircuit.probability_by_int)
-        mr = Readout(nxt, self.readout_index)
-        subcircuit.accept_readout(mr)
-        self.results.append(mr)
-        self.readout_index += 1
-
-
-class IndependentSubcircuitsJob(AbstractJob):
-    """Job for circuit with subcircuits that are independent"""
-
-    def execute(self):
-        w = IndependentSubcircuitsEmulatorWalker(self.traces, self.subcircuits)
-        w.visit(self.circuit)
-        return ExecutionResult(self.subcircuits, w.results)
-
-
-class IndependentSubcircuitsBackend(AbstractBackend):
+class EmulatedIndependentSubcircuitsBackend(IndependentSubcircuitsBackend):
     """Abstract emulator backend for subcircuits that are independent"""
 
-    def __call__(self, circ):
-        """Attaches the backend to a particular circuit, creating a Job object.
-
-        Calculates the probabilities of outcomes for every subcircuit.
+    def simulate_subcircuit(self, job, subcircuit):
+        self._simulate_subcircuit(job, subcircuit)
+        subcircuit.simulated = True
+        subcircuit.tree.simulated_probability = 1
 
-        :param Circuit circ: parent circuit
-
-        :returns IndependentSubcircuitsJob:
-        """
+    @abc.abstractmethod
+    def _simulate_subcircuit(self, job, subcircuit):
+        """(internal) Populate a subcircuit object with simulated data
+        :param JaqalJob job: The job, describing the circuit and overrides
+        :param SubcircuitResult subcirc: Data-carrying object of ExecutionResulsts
+        """
+        raise NotImplementedError()
+
+    def _simulate_ci(self, ci, job):
+        subcircuit = ci._subcircuit
+        for _ in range(ci.num_repeats):
+            node = subcircuit.tree
+            while not node.classical_state.state == cursor.State.shutdown:
+                keys = list(node.subsequent.keys())
+                p = [node.subsequent[k].simulated_probability for k in keys]
+                nxt = choice(keys, p=p)
+                mr = result.Readout(nxt, job.meas_count, node)
+                yield mr
+                job.meas_count += 1
+                node = node[nxt]
+
+    def _execute_job(self, job):
+        """(internal) Execute the job on the backend"""
+
+        exe_res = result.ExecutionResult(job.expanded_circuit, job.overrides)
+        for sb in exe_res.by_subbatch:
+            for sc in sb.by_subcircuit:
+                self.simulate_subcircuit(job, sc._subcircuit)
+
+        parser = exe_res.accept_readouts()
+
+        job.meas_count = 0
+        for ci in exe_res.by_time:
+            parser.pass_data(self._simulate_ci(ci, job))
 
-        job = IndependentSubcircuitsJob(self, circ)
-        visitor = DiscoverSubcircuits()
-        job.traces = traces = visitor.visit(circ)
-        job.subcircuits = [self._make_subcircuit(job, *tr) for tr in enumerate(traces)]
+        if not parser.done:
+            raise JaqalError("Not enough readouts passed to ExecutionResults.")
 
-        return job
+        return exe_res
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/backends.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/backends.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,100 +3,97 @@
 # certain rights in this software.
 import itertools
 
 from numpy import zeros
 
 from pygsti.protocols import ModelFreeformSimulator
 
-from jaqalpaq.core.algorithm.walkers import TraceSerializer
-from jaqalpaq.core.result import ProbabilisticSubcircuit, ReadoutSubcircuit
-from jaqalpaq.emulator.backend import IndependentSubcircuitsBackend, ExtensibleBackend
+from jaqalpaq.run.cursor import SubcircuitCursor, State
+from jaqalpaq.run import result
+from jaqalpaq.emulator import backend
 
 from .circuit import pygsti_circuit_from_circuit
 from .model import build_noisy_native_model
 
 # Set this to True if you would like Subcircuit objects to retain the pyGSTi objects
 # used to generate probabilities during their emulation.
 KEEP_PYGSTI_OBJECTS = False
 
 
-class pyGSTiSubcircuit(ProbabilisticSubcircuit, ReadoutSubcircuit):
-    """Encapsulate one part of the circuit between a prepare_all and measure_all gate.
-
-    This tracks the output of a pyGSTi-generated simulation run, which provides access
-    to emulated measurement outcomes, their relative frequency, the *ideal* measurement
-    probabilities, and the ideal density matrix.
-
-    Additionally, you can also store the pyGSTi "circuit" and "model" objects used for
-    the simulation by setting KEEP_PYGSTI_OBJECTS = True.
-    """
-
-    _pygsti_circuit = None
-    _pygsti_model = None
-
-    def __init__(self, *args, pyGSTi_circuit, pyGSTi_model, density_matrix, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._density_matrix = density_matrix
-
-        if KEEP_PYGSTI_OBJECTS:
-            self._pygsti_circuit = pyGSTi_circuit
-            self._pygsti_model = pyGSTi_model
-
-
-class CircuitEmulator(IndependentSubcircuitsBackend):
+class CircuitEmulator(backend.EmulatedIndependentSubcircuitsBackend):
     """Emulator using pyGSTi circuit objects
 
     This object should be treated as an opaque symbol to be passed to run_jaqal_circuit.
     """
 
     def __init__(self, *args, model=None, gate_durations=None, **kwargs):
         self.model = model
         self.gate_durations = gate_durations if gate_durations is not None else {}
         super().__init__(*args, **kwargs)
 
-    def _make_subcircuit(self, job, index, trace):
-        """Generate the probabilities of outcomes of a subcircuit
-
-        :param Trace trace: the subcircut of circ to generate probabilities for
-        :return: A pyGSTi outcome dictionary.
-        """
+    def _simulate_subcircuit(self, job, subcirc):
+        start = subcirc.start
+        end = subcirc.end
+        circ = subcirc.filled_circuit
 
         pc = pygsti_circuit_from_circuit(
-            job.circuit, trace=trace, durations=self.gate_durations
+            circ, trace=(start, end), durations=self.gate_durations
         )
 
         model = self.model
         mfs = ModelFreeformSimulator(None)
         rho, prob_dict = mfs.compute_final_state(model, pc, include_probabilities=True)
 
         probs = zeros(len(prob_dict), dtype=float)
         for k, v in prob_dict.items():
             probs[int(k[::-1], 2)] = v
 
-        return pyGSTiSubcircuit(
-            trace,
-            index,
-            pyGSTi_circuit=pc,
-            pyGSTi_model=model,
-            density_matrix=rho,
-            probabilities=probs,
-        )
+        p = result.validate_probabilities(probs)
+
+        tree = subcirc.tree
+        tree.simulated_density_matrix = rho
+
+        for k, v in enumerate(p):
+            node = tree.force_get(k)
+            node.simulated_probability = v
+
+        if KEEP_PYGSTI_OBJECTS:
+            subcirc._pygsti_circuit = pc
+            subcirc._pygsti_model = model
 
 
-class AbstractNoisyNativeEmulator(ExtensibleBackend, CircuitEmulator):
+class AbstractNoisyNativeEmulator(backend.ExtensibleBackend, CircuitEmulator):
     """(abstract) Noisy emulator using pyGSTi circuit objects
 
     Provides helper functions to make the generation of a noisy native model simpler.
 
     Every gate to be emulated should have a corresponding gate_{name} and
       gateduration_{name} method defined.  These will be automatically converted into
       pyGSTi-appropriate objects for model construction.  See build_model for more
       details.
     """
 
+    def __init__(
+        self, n_qubits, model=None, gate_durations=None, stretched_gates=None, **kwargs
+    ):
+        self.n_qubits = n_qubits
+        self.stretched_gates = stretched_gates
+        model, gate_durations = self.build_model()
+        super().__init__(model=model, gate_durations=gate_durations, **kwargs)
+
+    def get_n_qubits(self, circ):
+        """Returns the number of qubits the backend will be simulating.
+
+        :param circ: The circuit object being emulated/simulated.
+        """
+        circuit_qubits = super().get_n_qubits(circ)
+        if circuit_qubits > self.n_qubits:
+            raise ValueError(f"{self} emulates fewer qubits than {circ} uses")
+        return self.n_qubits
+
     def build_model(self):
         return build_noisy_native_model(
             self.jaqal_gates,
             self.collect_gate_models(),
             self.idle,
             self.n_qubits,
             stretched_gates=self.stretched_gates,
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/circuit.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/circuit.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/pygsti/model.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/pygsti/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pygsti.modelmembers.povms import ComputationalBasisPOVM
 from pygsti.modelmembers.states import ComputationalBasisState
 from pygsti.models import LocalNoiseModel
 from pygsti.processors import QubitProcessorSpec
 from pygsti.baseobjs import UnitaryGateFunction
 
 from jaqalpaq.error import JaqalError
+from .._import import get_ideal_action
 
 
 def pygsti_gate_name(gate):
     """Returns the canonical pyGSTi gate name of a Jaqal gate."""
     return f"GJ{gate.name}"
 
 
@@ -107,65 +108,69 @@
 
     if fact:
         return JaqalOpFactory(fun, gate)
 
     return StaticArbitraryOp(fun(*[None for i in range(quantum_args)]))
 
 
-def pygsti_ideal_unitary(gate):
+def pygsti_ideal_unitary(gate, evotype):
     """Ideal unitary action of the gate with pyGSTi special casing.
 
     :param gate: The Jaqalpaq gate definition object describing the gate.
+    :param evotype: the pyGSTi evolution type to use for the model.  The default is
+        "statevec", which is sufficient for noiseless simulation.
     """
+    ideal_unitary = get_ideal_action(gate)
 
-    def _unitary_fun(*parms):
+    # Skip gates without defined action
+    if ideal_unitary is None:
+        return
+
+    if len(gate.quantum_parameters) == 0:
+        raise JaqalError(f"{gate.name} not supported")
+
+    # Cast to a PyGSTi StaticUnitaryOp to avoid autoconstruction logic
+    if len(gate.classical_parameters) == 0:
+        return StaticUnitaryOp(ideal_unitary(), evotype=evotype)
+
+    def _gate(*parms):
         """
         :param parms: A list of all classical arguments to the gate.
         :return: The ideal unitary action of the gate on its target qubits, or an
         identity gate on the target qubit.
         """
         if parms:
-            return gate.ideal_unitary(*parms)
+            return ideal_unitary(*parms)
         else:
             return np.identity(2 ** len(gate.quantum_parameters), "complex")
 
-    return _unitary_fun
+    # Cast to a JaqalOpFactory to avoid autoconstruction logic
+    return JaqalOpFactory(_gate, gate=gate, pass_args=("classical",), evotype=evotype)
 
 
 def build_processor_spec(n_qubits, gates, evotype="default"):
     """Build a ProcessorSpec of ideal unitaries suitable for pygsti model creation.
     Adds key names of the form GJ<gate name> for each Jaqal gate
 
     :param n_qubits: the number of qubits in the model
     :param gates: a dictionary of Jaqal gates
+    :param evotype: What kind of object pyGSTi simulates (e.g., density matrix or state
+      vector).  See pyGSTi documentation for details.
     :return: PyGSTi ProcessorSpec to be used in model creation
     """
     unitaries = {}
     dummy_unitaries = {}
     availability = {}
     for g in gates.values():
+        obj = pygsti_ideal_unitary(g, evotype)
+
         # Skip gates without defined action
-        if g.ideal_unitary is None:
+        if obj is None:
             continue
 
-        if len(g.quantum_parameters) == 0:
-            raise JaqalError(f"{g.name} not supported")
-
-        if len(g.classical_parameters) > 0:
-            obj = pygsti_ideal_unitary(g)
-        else:
-            obj = g.ideal_unitary()
-
-        # Cast to either a PyGSTi StaticUnitaryOp or OpFactory to avoid autoconstruction logic
-        if callable(obj):
-            # For the ideal unitary, only pass classical arguments to underlying function
-            obj = JaqalOpFactory(obj, gate=g, pass_args=("classical",), evotype=evotype)
-        else:
-            obj = StaticUnitaryOp(obj, evotype=evotype)
-
         pygsti_name = pygsti_gate_name(g)
         unitaries[pygsti_name] = obj
 
         if len(g.quantum_parameters) > 1:
             availability[pygsti_name] = "all-permutations"
         else:
             availability[pygsti_name] = [(sslbl,) for sslbl in range(n_qubits)]
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/emulator/unitary.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/emulator/unitary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,155 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 import numpy
 
-from jaqalpaq.core.algorithm.walkers import TraceSerializer
-from jaqalpaq.core.result import ProbabilisticSubcircuit, ReadoutSubcircuit
-from jaqalpaq.emulator.backend import IndependentSubcircuitsBackend
+from jaqalpaq.error import JaqalError
+from jaqalpaq.run.cursor import SubcircuitCursor, State
+from jaqalpaq.run import result
+from jaqalpaq.emulator.backend import EmulatedIndependentSubcircuitsBackend
+from ._import import get_ideal_action
 
 
-class EmulatorSubcircuit(ProbabilisticSubcircuit, ReadoutSubcircuit):
-    """Encapsulate one part of the circuit between a prepare_all and measure_all gate.
+def inplace_multiply(dsub, qind, vec, scratch):
+    # The plan is to apply the associated unitary to vec for each gate.
+    # now we need to sparse-multiply:
+    # vec = U * inp
+    # But! U isn't just dsub
 
-    This tracks the output of a unitary, forward-map simulation run, which provides access
-    to emulated measurement outcomes, their relative frequency, the *ideal* measurement
-    probabilities, and the ideal state vector before measurement.
-    """
+    # The current state-vector becomes the input to the matrix multiplication
+    inp, vec = vec, scratch
+    # (Notice that this initializes inp, from above)
+    vec[:] = 0
+
+    # For every column in the output matrix, we need to compute the sum
+    # over the nonzero rows of U.
+
+    # However, this corresponds to a sum only over rows of dsub, with
+    # a particular mapping between the rows and columns.
+    for i in range(len(vec)):
+        # Because we are only dealing with qubits, the binary representation
+        # of the row is precisely the standard basis label corresponding to that
+        # row.
+
+        # We need to re-map the qubits that are being acted on by dsub to
+        # the *column* of dsub.  Additionally, the qubits that are not being
+        # acted on by dsub are unaffected, and therefore are the same in both
+        # the input and output.
+
+        # mask is precisely these bystander qubits --- the affected qubits are
+        # set to zero, and shuffled into another variable, dsub_row
+        mask = i
+
+        # We initialize dsub_row to zero, and then build it up via bit-twiddling
+        dsub_row = 0
+
+        for dsub_bit, i_k in enumerate(qind):
+            # We iterate over all the qubits acted on by dsub
+
+            # Is this specific qubit high (for this row)?
+            n_high = mask & (0b1 << i_k)
+
+            # If it is high, lower it in the mask
+            # (notice this is equivalent to subtraction)
+            mask ^= n_high
+
+            # If it is high, raise it in the row to be passed to dsub
+            # (notice this is equivalent to addition)
+            dsub_row |= (n_high >> i_k) << dsub_bit
+
+        # We now have the row in dsub that corresponds to the row in U
 
-    def __init__(self, *args, state_vector, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._state_vector = state_vector
+        # Next, we need to iterate over the column of U, and simultaneously the
+        # column of inp --- this mapping is the same as the above, backwards.
+        for dsub_col in range(dsub.shape[0]):
+            j = mask
+            dsub_col_stack = dsub_col
+            for dsub_bit, j_k in enumerate(qind):
+                j |= (dsub_col_stack & 0b1) << j_k
+                dsub_col_stack >>= 1
 
-    @property
-    def state_vector(self):
-        return self._state_vector
+            # Suitably armed with the associated row and column, we
+            # do the standard matrix accumulation sum step.
 
+            vec[i] += dsub[dsub_row, dsub_col] * inp[j]
 
-class UnitarySerializedEmulator(IndependentSubcircuitsBackend):
+    return vec, inp
+
+
+class UnitarySerializedEmulator(EmulatedIndependentSubcircuitsBackend):
     """Serialized emulator using unitary matrices
 
     This object should be treated as an opaque symbol to be passed to run_jaqal_circuit.
     """
 
-    def _make_subcircuit(self, job, index, trace):
+    def _simulate_subcircuit(self, job, subcirc):
         """Generate the ProbabilisticSubcircuit associated with the trace of circuit
             being process in job.
 
         :param job: the job object controlling the emulation
         :param int index: the index of the trace in the circuit
         :param Trace trace: the trace of the subcircuit
-        :return: A ProbabilisticSubcircuit.
         """
+        circ = subcirc.filled_circuit
+        gatedefs = circ.native_gates
+
+        # fill_in_let modified the circuit here
+        cursor = SubcircuitCursor(subcirc.start, subcirc.end)
 
-        circ = job.circuit
         n_qubits = self.get_n_qubits(circ)
 
+        # We serialize the subcircuit, obtaining a list of gates.
+        # The plan is to apply the associated unitary to vec for each gate.
         hilb_dim = 2**n_qubits
-        gatedefs = circ.native_gates
-
-        # vec = U * inp
-        # We don't need to initialize inp yet
-        inp = numpy.empty(hilb_dim, dtype=complex)
         vec = numpy.zeros(hilb_dim, dtype=complex)
         vec[0] = 1
 
-        # We serialize the subcircuit, obtaining a list of gates.
-        # The plan is to apply the associated unitary to vec for each gate.
-        s = TraceSerializer(trace)
-        for gate in s.visit(circ):
-            # This captures the classical arguments to the gate
-            argv = []
-            # This capture the quantum arguments to the gate --- the qubit index
-            qind = []
-            gatedef = gatedefs[gate.name]
-            if gatedef.ideal_unitary is None:
-                # maybe add other checks?
-                continue
-
-            for param, val in zip(gatedef.parameters, gate.parameters.values()):
-                if param.classical:
-                    argv.append(val)
-                else:
-                    qind.append(val.alias_index)
-
-            # This is the dense submatrix
-            dsub = gatedef.ideal_unitary(*argv)
-
-            # now we need to sparse-multiply:
-            # vec = U * imp
-            # But! U isn't just dsub
-
-            # The current state-vector becomes the input to the matrix multiplication
-            inp, vec = vec, inp
-            # (Notice that this initializes inp, from above)
-            vec[:] = 0
-
-            # For every column in the output matrix, we need to compute the sum
-            # over the nonzero rows of U.
-
-            # However, this corresponds to a sum only over rows of dsub, with
-            # a particular mapping between the rows and columns.
-            for i in range(hilb_dim):
-                # Because we are only dealing with qubits, the binary representation
-                # of the row is precisely the standard basis label corresponding to that
-                # row.
-
-                # We need to re-map the qubits that are being acted on by dsub to
-                # the *column* of dsub.  Additionally, the qubits that are not being
-                # acted on by dsub are unaffected, and therefore are the same in both
-                # the input and output.
-
-                # mask is precisely these bystander qubits --- the affected qubits are
-                # set to zero, and shuffled into another variable, dsub_row
-                mask = i
-
-                # We initialize dsub_row to zero, and then build it up via bit-twiddling
-                dsub_row = 0
-
-                # Which bit (stored as a bitmask) is up to be changed?
-                dsub_bit = 1
-                for i_k in qind:
-                    # We iterate over all the qubits acted on by dsub
-
-                    # Is this specific qubit high (for this row)?
-                    n_high = mask & (1 << i_k)
-
-                    # If it is high, lower it in the mask
-                    # (notice this is equivalent to subtraction)
-                    mask ^= n_high
-
-                    # If it is high, raise it in the row to be passed to dsub
-                    # (notice this is equivalent to addition)
-                    if n_high:
-                        dsub_row |= dsub_bit
-
-                    # Advance the bit mask by one
-                    dsub_bit <<= 1
-
-                # We now have the row in dsub that corresponds to the row in U
-
-                # Next, we need to iterate over the column of U, and simultaneously the
-                # column of inp --- this mapping is the same as the above, backwards.
-                for dsub_col in range(dsub.shape[0]):
-                    j = mask
-                    dsub_bit = 1
-                    for j_k in qind:
-                        if dsub_col & dsub_bit:
-                            j |= 1 << j_k
-                        dsub_bit <<= 1
-
-                    # Suitably armed with the associated row and column, we
-                    # do the standard matrix accumulation sum step.
-
-                    vec[i] += inp[j] * dsub[dsub_row, dsub_col]
-
-        probs = numpy.abs(vec) ** 2
-
-        subcircuit = EmulatorSubcircuit(
-            trace, index, probabilities=probs, state_vector=vec
-        )
+        def handle_final_measurement(cursor, vec, node):
+            P = numpy.abs(vec) ** 2
+            P = result.validate_probabilities(P)
+            for i, prob in enumerate(P):
+                if prob <= result.CUTOFF_ZERO:
+                    continue
+                meas_cursor = cursor.copy()
+                meas = meas_cursor.next_measure()
+                assert meas_cursor.state == State.shutdown
+                sub = node.force_get(i, meas_cursor)
+                assert sub.classical_state == meas_cursor
+                sub.simulated_probability = prob
+            assert node.classical_state == cursor
+            node.state_vector = vec
+
+        def handle_unitary(cursor, vec, node):
+            # We don't need to initialize this yet.
+            scratch = numpy.empty(hilb_dim, dtype=complex)
+
+            while cursor.state == State.gate:
+                gate = cursor.next_gate()
+                cursor.report_gate_executed()
+
+                # This captures the classical arguments to the gate
+                argv = []
+                # This capture the quantum arguments to the gate --- the qubit index
+                qind = []
+                gatedef = gatedefs[gate.name]
+                ideal_unitary = get_ideal_action(gatedef)
+                if ideal_unitary is None:
+                    continue
+
+                for param, val in zip(gatedef.parameters, gate.parameters.values()):
+                    if param.classical:
+                        argv.append(val)
+                    else:
+                        qind.append(val.alias_index)
+
+                # This is the dense submatrix
+                dsub = ideal_unitary(*argv)
+
+                vec, scratch = inplace_multiply(dsub, qind, vec, scratch)
+
+            if cursor.state == State.final_measurement:
+                handle_final_measurement(cursor, vec, node)
+            else:
+                raise NotImplementedError()
 
-        return subcircuit
+        handle_unitary(cursor, vec, subcirc.tree)
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/generator/generator.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/generator/generator.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/parser/identifier.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/parser/identifier.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/parser/parser.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/parser/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,30 @@
     expand_macro=False,
     expand_let=False,
     expand_let_map=False,
     return_usepulses=False,
     inject_pulses=None,
     autoload_pulses=True,
     import_path=None,
+    use_name=True,
 ):
     """Parse a file written in Jaqal into core types.
 
     :param str filename: The name of the Jaqal file.
     :param override_dict:  An optional dictionary that overrides let statements in the Jaqal code.
         Note: all keys in this dictionary must exist as let statements or an error will be raised.
     :type override_dict: dict[str, float]
     :param bool expand_macro: Replace macro invocations by their body while parsing.
     :param bool expand_let: Replace let constants by their value while parsing.
     :param bool expand_let_map: Replace let constants and mapped qubits while parsing. expand_let is ignored if this is True.
     :param bool return_usepulses: Whether to both add a second return value and populate it with the usepulses statement.
     :param inject_pulses: If given, use these pulses specifically.
     :param bool autoload_pulses: Whether to employ the usepulses statement for parsing.  Requires appropriate gate definitions.
     :param str import_path: The path to be used for relative Jaqal imports. Defaults to the file's directory.
+    :param bool use_name:to remember the name of the Jaqal file
     :return: The circuit representation of the file and usepulses if
         requested. usepulses is stored in a dict under the key
         'usepulses'. It is itself a dict mapping :class:`Identifier`
         bjects to what the import, which may be the special symbol all.
 
     """
     if import_path is None:
@@ -50,41 +52,44 @@
             expand_macro=expand_macro,
             expand_let=expand_let,
             expand_let_map=expand_let_map,
             return_usepulses=return_usepulses,
             inject_pulses=inject_pulses,
             autoload_pulses=autoload_pulses,
             import_path=import_path,
+            name_hint=f"from '{filename}'" if use_name else None,
         )
 
 
 def parse_jaqal_string(
     jaqal,
     override_dict=None,
     expand_macro=False,
     expand_let=False,
     expand_let_map=False,
     return_usepulses=False,
     inject_pulses=None,
     autoload_pulses=True,
     import_path=None,
+    name_hint=None,
 ):
     """Parse a string written in Jaqal into core types.
 
     :param str jaqal: The Jaqal code.
     :param override_dict:  An optional dictionary that overrides let statements in the Jaqal code.
         Note: all keys in this dictionary must exist as let statements or an error will be raised.
     :type override_dict: dict[str, float]
     :param bool expand_macro: Replace macro invocations by their body while parsing.
     :param bool expand_let: Replace let constants by their value while parsing.
     :param bool expand_let_map: Replace let constants and mapped qubits while parsing. expand_let is ignored if this is True.
     :param bool return_usepulses: Whether to both add a second return value and populate it with the usepulses statement.
     :param inject_pulses: If given, use these pulses specifically.
     :param bool autoload_pulses: Whether to employ the usepulses statement for parsing.  Requires appropriate gate definitions.
     :param str import_path: The path to be used for relative Jaqal imports. Defaults to the current working directory.
+    :param str name_hint: Name to give to the circuit.
     :return: The circuit representation of the file and usepulses if
         requested. usepulses is stored in a dict under the key
         'usepulses'. It is itself a dict mapping :class:`Identifier`
         objects to what the import, which may be the special symbol all.
 
     """
 
@@ -108,14 +113,17 @@
         circuit = fill_in_map(circuit)
     elif expand_let:
         circuit = fill_in_let(circuit, override_dict=override_dict)
 
     if sum(reg.fundamental for reg in circuit.registers.values()) > 1:
         raise JaqalError(f"Circuit has too many registers: {list(circuit.registers)}")
 
+    if name_hint:
+        circuit._name_hint = name_hint
+
     if return_usepulses:
         return circuit, {"usepulses": usepulses}
     else:
         return circuit
 
 
 def parse_to_sexpression(jaqal, return_usepulses=False, header_only=False):
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/parser/slyparse.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/parser/slyparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return token
 
     def NUMBER(self, token):
         token.value = float(token.value)
         return token
 
     def BININT(self, token):
-        token.value = int(token.value[1:-1], base=2)
+        token.value = int(token.value[-2:0:-1], base=2)
         return token
 
 
 class JaqalParser(Parser):
     """Parse Jaqal into core types."""
 
     def __init__(self, source_text=None, source="<string>", header_only=False):
@@ -194,14 +194,15 @@
     # Define what statements are allowed in sequential blocks.
 
     @_(
         "gate_statement",
         "parallel_gate_block",
         "loop_statement",
         "subcircuit_gate_block",
+        "branch_statement",
     )
     def inner_seq_statement(self, tree):
         # No need to set self._in_body as we've definitely already set
         # it.
         return tree[0]
 
     # Define what statements are allowed in parallel blocks
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/compile.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 
 import argparse
-from .qsyntax import is_qcircuit
+from jaqalpaq.qsyntax.qsyntax import is_qcircuit
 from jaqalpaq.generator import generate_jaqal_program
 
 
 def main():
     args = get_args()
     try:
         ns = run_in_namespace(args.filename)
```

### Comparing `JaqalPaq-1.1.1/src/jaqalpaq/qsyntax/qsyntax.py` & `JaqalPaq-1.2.0a1/src/jaqalpaq/qsyntax/qsyntax.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/abstractgate.py` & `JaqalPaq-1.2.0a1/tests/core/abstractgate.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,51 +33,51 @@
 
     def test_instantiate_no_args(self):
         """Test creating a GateStatement from a GateDefinition with no arguments."""
         gatedef = self.create_random_instance(parameter_count=0)
         gate = gatedef()
         self.assertEqual({}, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
-        gate = gatedef.call()
+        gate = gatedef()
         self.assertEqual({}, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
 
     def test_positional_args(self):
         gatedef = self.create_random_instance()
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types)
         gate = gatedef(*arguments)
         arg_dict = {
             param.name: arg for param, arg in zip(gatedef.parameters, arguments)
         }
         self.assertEqual(arg_dict, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
-        gate = gatedef.call(*arguments)
+        gate = gatedef(*arguments)
         self.assertEqual(arg_dict, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
 
     def test_fail_too_many_args(self):
         """Test creating a GateStatement from a GateDefinition with the wrong number of arguments."""
         gatedef = self.create_random_instance()
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types + [None])
         with self.assertRaises(Exception):
             gatedef(*arguments)
         with self.assertRaises(Exception):
-            gatedef.call(*arguments)
+            gatedef(*arguments)
 
     def test_fail_too_few_args(self):
         """Test creating a GateStatement from a GateDefinition with the wrong number of arguments."""
         gatedef = self.create_random_instance(parameter_count=random_whole())
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types[:-1])
         with self.assertRaises(Exception):
             gatedef(*arguments)
         with self.assertRaises(Exception):
-            gatedef.call(*arguments)
+            gatedef(*arguments)
 
     def test_fail_wrong_arg_type(self):
         """Test creating a GateStatement with the wrong argument types."""
         param_types = [ParamType.INT, ParamType.FLOAT, ParamType.QUBIT]
         for param_type in param_types:
             parameter = common.make_random_parameter(allowed_types=[param_type])
             gatedef = self.tested_type(random_identifier(), parameters=[parameter])
@@ -85,27 +85,27 @@
             if param_type == ParamType.FLOAT:
                 other_types.remove(ParamType.INT)
             for other_type in other_types:
                 arguments = [common.make_random_value(other_type)]
                 with self.assertRaises(Exception):
                     gatedef(*arguments)
                 with self.assertRaises(Exception):
-                    gatedef.call(*arguments)
+                    gatedef(*arguments)
 
     def test_instantiate_keyword_args(self):
         """Test instantiating a GateStatement using keyword arguments."""
         # Note: Jaqal doesn't use keyword arguments, but maybe another supported language does.
         gatedef = self.create_random_instance()
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types)
         kwargs = {param.name: arg for param, arg in zip(gatedef.parameters, arguments)}
         gate = gatedef(**kwargs)
         self.assertEqual(kwargs, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
-        gate = gatedef.call(**kwargs)
+        gate = gatedef(**kwargs)
         self.assertEqual(kwargs, gate.parameters)
         self.assertEqual(gatedef.name, gate.name)
 
     def test_fail_on_mixing_arg_types(self):
         """Test failing when mixing positional and keyword arguments."""
         gatedef = self.create_random_instance(parameter_count=random_whole(lower=2))
         arg_types = [param.kind for param in gatedef.parameters]
@@ -125,26 +125,26 @@
                 lambda x: x[0] < len(arguments) // 2, enumerate(arg_dict.items())
             )
         }
         assert len(args) + len(kwargs) == len(arguments)
         with self.assertRaises(Exception):
             gatedef(*args, **kwargs)
         with self.assertRaises(Exception):
-            gatedef.call(*args, **kwargs)
+            gatedef(*args, **kwargs)
 
     def test_fail_too_few_keyword_args(self):
         """Test failing when not providing enough keyword arguments."""
         gatedef = self.create_random_instance(parameter_count=random_whole())
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types[:-1])
         kwargs = {param.name: arg for param, arg in zip(gatedef.parameters, arguments)}
         with self.assertRaises(Exception):
             gatedef(**kwargs)
         with self.assertRaises(Exception):
-            gatedef.call(**kwargs)
+            gatedef(**kwargs)
 
     def test_fail_too_many_keyword_args(self):
         """Test failing when providing unnecessary keyword arguments."""
         gatedef = self.create_random_instance(parameter_count=random_whole())
         arg_types = [param.kind for param in gatedef.parameters]
         arguments = common.make_random_argument_list(arg_types + [None])
         kwargs = {param.name: arg for param, arg in zip(gatedef.parameters, arguments)}
@@ -152,8 +152,8 @@
             new_name = random_identifier()
             if new_name not in kwargs:
                 break
         kwargs[new_name] = arguments[-1]
         with self.assertRaises(Exception):
             gatedef(**kwargs)
         with self.assertRaises(Exception):
-            gatedef.call(**kwargs)
+            gatedef(**kwargs)
```

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_expand_macros.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_expand_macros.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_expand_subcircuits.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_expand_subcircuits.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_fill_in_let.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_fill_in_let.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_unit_timing.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_unit_timing.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_used_qubits.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_used_qubits.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/algorithm/test_visitor.py` & `JaqalPaq-1.2.0a1/tests/core/algorithm/test_visitor.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/common.py` & `JaqalPaq-1.2.0a1/tests/core/common.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/randomize.py` & `JaqalPaq-1.2.0a1/tests/core/randomize.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_block.py` & `JaqalPaq-1.2.0a1/tests/core/test_block.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_branch.py` & `JaqalPaq-1.2.0a1/tests/core/test_branch.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_circuitbuilder.py` & `JaqalPaq-1.2.0a1/tests/core/test_circuitbuilder.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_constant.py` & `JaqalPaq-1.2.0a1/tests/core/test_constant.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_gate.py` & `JaqalPaq-1.2.0a1/tests/core/test_gate.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_loop.py` & `JaqalPaq-1.2.0a1/tests/core/test_loop.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_macro.py` & `JaqalPaq-1.2.0a1/tests/core/test_macro.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_named_qubit.py` & `JaqalPaq-1.2.0a1/tests/core/test_named_qubit.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_parameter.py` & `JaqalPaq-1.2.0a1/tests/core/test_parameter.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_register.py` & `JaqalPaq-1.2.0a1/tests/core/test_register.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/core/test_usepulses.py` & `JaqalPaq-1.2.0a1/tests/core/test_usepulses.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/emulator/test_forward_simulation.py` & `JaqalPaq-1.2.0a1/tests/emulator/test_forward_simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,42 @@
+from pathlib import Path
 import unittest, pytest
-import os
 
 import jaqalpaq
 import jaqalpaq.error
 from jaqalpaq.core.circuitbuilder import CircuitBuilder
 import numpy as np
 from jaqalpaq.emulator import run_jaqal_string, run_jaqal_circuit, run_jaqal_file
 from jaqalpaq.generator import generate_jaqal_program
 import jaqalpaq.parser
-from jaqalpaq.core.result import ExecutionResult, parse_jaqal_output_list
+from jaqalpaq.run.result import ExecutionResult, parse_jaqal_output_list
 from collections import OrderedDict
 from jaqalpaq.emulator._validator import (
     generate_jaqal_validation,
     validate_jaqal_string,
 )
 from jaqalpaq.emulator.pygsti.circuit import pygsti_circuit_from_circuit
 
 qscout = pytest.importorskip("qscout")
 
 from qscout.v1.std import jaqal_gates
 from qscout.v1.std.noisy import SNLToy1
 
 
 def example(*args):
-    return os.path.join("examples", "jaqal", *args)
+    return Path("examples", "jaqal", *args)
+
+
+def get_unif_val(view):
+    def _inner(v):
+        val = v[0]
+        assert val == v
+        return val
+
+    return {k: _inner(v) for (k, v) in view.items()}
 
 
 class ForwardSimulatorTester(unittest.TestCase):
     def setUp(self):
         builder = CircuitBuilder(jaqal_gates.ALL_GATES)
 
         pi2 = builder.let("pi2", np.pi / 2)
@@ -42,14 +51,32 @@
         self.jaqal_string = generate_jaqal_program(self.c)
 
         self.jaqal_c = jaqalpaq.parser.parse_jaqal_string(
             self.jaqal_string,
             inject_pulses=jaqal_gates.ALL_GATES,
         )
 
+    def check_subcircuit_readouts(self, results, subcircuit_i, true_output):
+        true_int_output = [int(s[::-1], 2) for s in true_output]
+
+        sc = results.subcircuits[subcircuit_i]
+        sc_n = results.by_subbatch[0].by_subcircuit[subcircuit_i]
+        int_output = [o.as_int for o in sc.readouts]
+        output = [o.as_str for o in sc.readouts]
+        self.assertEqual(int_output, true_int_output)
+        self.assertEqual(output, true_output)
+
+        true_total_prob = np.zeros(len(sc.relative_frequency_by_int))
+        for n, val in enumerate(true_int_output):
+            true_total_prob[val] += 1
+            self.assertEqual(sc_n.by_time[n].normalized_counts.by_int[val], 1)
+            self.assertEqual(sc_n.normalized_counts.by_int[val][n], 1)
+        true_total_prob /= len(true_output)
+        assert np.allclose(true_total_prob, sc.relative_frequency_by_int)
+
     def test_generate_jaqal_program(self):
         self.assertEqual(
             "\n".join([p for p in self.jaqal_string.split("\n")]),
             """let pi2 1.5707963267948966
 
 register q[3]
 
@@ -87,23 +114,81 @@
   MS q[1] q[0] pi2 pi2
 }
 """
         res = run_jaqal_string(
             "\n".join(("from qscout.v1.std usepulses *", jaqal_string))
         )
 
-        c_dict = res.subcircuits[0].probability_by_str
-        self.assertAlmostEqual(c_dict["000"], 0.5)
-        self.assertAlmostEqual(c_dict["001"], 0)
-        self.assertAlmostEqual(c_dict["010"], 0)
-        self.assertAlmostEqual(c_dict["011"], 0)
-        self.assertAlmostEqual(c_dict["100"], 0)
-        self.assertAlmostEqual(c_dict["101"], 0)
-        self.assertAlmostEqual(c_dict["110"], 0.5)
-        self.assertAlmostEqual(c_dict["111"], 0)
+        byt = res.by_subbatch[0].by_time[0]
+        bys = res.by_subbatch[0].by_subcircuit[0]
+
+        for c_dict in (
+            res.subcircuits[0].probability_by_str,
+            byt.simulated_probabilities,
+            byt.conditional_simulated_probabilities,
+            get_unif_val(bys.simulated_probabilities.by_str_dense),
+            get_unif_val(bys.conditional_simulated_probabilities.by_str_dense),
+        ):
+            self.assertAlmostEqual(c_dict["000"], 0.5)
+            self.assertAlmostEqual(c_dict["001"], 0)
+            self.assertAlmostEqual(c_dict["010"], 0)
+            self.assertAlmostEqual(c_dict["011"], 0)
+            self.assertAlmostEqual(c_dict["100"], 0)
+            self.assertAlmostEqual(c_dict["101"], 0)
+            self.assertAlmostEqual(c_dict["110"], 0.5)
+            self.assertAlmostEqual(c_dict["111"], 0)
+
+    def test_emulate_subcircuit_shots(self):
+        jaqal_string = """let pi2 1.5707963267948966
+
+register q[3]
+
+subcircuit 10 {
+  MS q[1] q[0] pi2 pi2
+}
+"""
+        np.random.seed(0)
+        res = run_jaqal_string(
+            "\n".join(("from qscout.v1.std usepulses *", jaqal_string))
+        )
+
+        byt = res.by_subbatch[0].by_time[0]
+        bys = res.by_subbatch[0].by_subcircuit[0]
+
+        for c_dict in (
+            res.subcircuits[0].probability_by_str,
+            byt.simulated_probabilities,
+            byt.conditional_simulated_probabilities,
+            get_unif_val(bys.simulated_probabilities.by_str_dense),
+            get_unif_val(bys.conditional_simulated_probabilities.by_str_dense),
+        ):
+            self.assertAlmostEqual(c_dict["000"], 0.5)
+            self.assertAlmostEqual(c_dict["001"], 0)
+            self.assertAlmostEqual(c_dict["010"], 0)
+            self.assertAlmostEqual(c_dict["011"], 0)
+            self.assertAlmostEqual(c_dict["100"], 0)
+            self.assertAlmostEqual(c_dict["101"], 0)
+            self.assertAlmostEqual(c_dict["110"], 0.5)
+            self.assertAlmostEqual(c_dict["111"], 0)
+
+        for c_dict in (
+            res.subcircuits[0].relative_frequency_by_str,
+            res.by_subbatch[0].by_time[0].normalized_counts,
+        ):
+            self.assertAlmostEqual(c_dict["000"], 0.3)
+            self.assertAlmostEqual(c_dict["001"], 0)
+            self.assertAlmostEqual(c_dict["010"], 0)
+            self.assertAlmostEqual(c_dict["011"], 0)
+            self.assertAlmostEqual(c_dict["100"], 0)
+            self.assertAlmostEqual(c_dict["101"], 0)
+            self.assertAlmostEqual(c_dict["110"], 0.7)
+            self.assertAlmostEqual(c_dict["111"], 0)
+
+        self.assertEqual(res.by_time[0].num_repeats, 10)
+        self.assertEqual(res.by_subbatch[0].by_subcircuit[0].num_repeats, [10])
 
     def test_five_qubit_GHZ(self):
         jaqal_text = """
 register q[5]
 
 let pi2 1.5707963267948966
 let mpi2 -1.5707963267948966
@@ -132,24 +217,24 @@
         )
         res = run_jaqal_circuit(jaqal_prog)
         output_probs = res.subcircuits[0].probability_by_str
         self.assertAlmostEqual(output_probs["00000"], 0.5)
         self.assertAlmostEqual(output_probs["11111"], 0.5)
 
     def test_JaqalError(self):
-        with pytest.raises(jaqalpaq.error.JaqalError):
-            jaqal_str = """
+        jaqal_str = """
 from qscout.v1.std usepulses *
 register q[1]
 prepare_all
 Px q[0]
 measure_all
 measure_all
 """
-            jaqal_circ = jaqalpaq.parser.parse_jaqal_string(jaqal_str)
+        jaqal_circ = jaqalpaq.parser.parse_jaqal_string(jaqal_str)
+        with pytest.raises(jaqalpaq.error.JaqalError):
             results = jaqalpaq.emulator.run_jaqal_circuit(jaqal_circ)
 
     def test_spec_bell_state(self):
         jaqal_str = """
 from qscout.v1.std usepulses *
 
 register q[2]
@@ -296,40 +381,27 @@
         Px q[1]
         measure_all
     }
 }
 
 prepare_all
 Px q[2]
-prepare_all
-Px q[2]
 measure_all
 """
         results = jaqalpaq.emulator.run_jaqal_string(jaqal_str)
         output = [o.as_str for o in results.readouts]
         int_output = [o.as_int for o in results.readouts]
         true_output = ["100", "010", "010", "100", "010", "010", "001"]
         true_int_output = [1, 2, 2, 1, 2, 2, 4]
         self.assertEqual(output, true_output)
         self.assertEqual(int_output, true_int_output)
 
-        int_output = [o.as_int for o in results.subcircuits[0].readouts]
-        output = [o.as_str for o in results.subcircuits[0].readouts]
-        self.assertEqual(int_output, [1, 1])
-        self.assertEqual(output, ["100", "100"])
-
-        int_output = [o.as_int for o in results.subcircuits[1].readouts]
-        output = [o.as_str for o in results.subcircuits[1].readouts]
-        self.assertEqual(int_output, [2, 2, 2, 2])
-        self.assertEqual(output, ["010", "010", "010", "010"])
-
-        int_output = [o.as_int for o in results.subcircuits[2].readouts]
-        output = [o.as_str for o in results.subcircuits[2].readouts]
-        self.assertEqual(int_output, [4])
-        self.assertEqual(output, ["001"])
+        self.check_subcircuit_readouts(results, 0, ["100", "100"])
+        self.check_subcircuit_readouts(results, 1, ["010", "010", "010", "010"])
+        self.check_subcircuit_readouts(results, 2, ["001"])
 
     def test_spec_pi_fracs(self):
         jaqal_str = """
 from qscout.v1.std usepulses *
 
 register q[1]
 let pi_32   0.09817477042
@@ -454,14 +526,56 @@
         txt.append(newval)
         txt = "".join(txt)
 
         res = validate_jaqal_string(txt)
 
         self.assertEqual(res, ["measurements agree", "probabilities agree"])
 
+    def test_stretched_gates_noiseless(self):
+        jc = jaqalpaq.parser.parse_jaqal_string(
+            """
+            from qscout.v1.std usepulses *
+
+            register u[3]
+
+            prepare_all
+
+            Rx u[0] 0.7
+            MS u[0] u[1] 0.1 0.3
+            Rz u[2] 0.8
+
+            measure_all
+        """
+        )
+
+        jc_stretched = jaqalpaq.parser.parse_jaqal_string(
+            """
+            from qscout.v1.std usepulses *
+            from qscout.v1.std.stretched usepulses *
+
+            register u[3]
+
+            prepare_all
+
+            Rx_stretched u[0] 0.7 1.5
+            MS_stretched u[0] u[1] 0.1 0.3 3
+            Rz_stretched u[2] 0.8 2.0
+
+            measure_all
+        """
+        )
+
+        res = run_jaqal_circuit(jc)
+        res_stretched = run_jaqal_circuit(jc_stretched)
+
+        for a, b in zip(*(r.by_subbatch[0].by_time for r in (res, res_stretched))):
+            assert np.allclose(
+                *(i.simulated_probabilities.by_int_dense for i in (a, b))
+            )
+
     def test_stretched_gates(self):
         jc = jaqalpaq.parser.parse_jaqal_string(
             """
             from qscout.v1.std usepulses *
             from qscout.v1.std.stretched usepulses *
 
             register u[3]
```

### Comparing `JaqalPaq-1.1.1/tests/emulator/test_jaqal_files.py` & `JaqalPaq-1.2.0a1/tests/emulator/test_jaqal_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os
+from pathlib import Path
 import unittest, pytest
 
 import numpy as np
 
 from jaqalpaq.parser import parse_jaqal_string
 from jaqalpaq.emulator._validator import (
     validate_jaqal_circuit,
@@ -14,23 +14,19 @@
 from jaqalpaq.emulator.pygsti.model import build_noiseless_native_model
 
 qscout = pytest.importorskip("qscout")
 
 from qscout.v1.std.noisy import SNLToy1
 
 
-def example(*args):
-    return os.path.join("examples", "jaqal", *args)
-
-
-_fnames = [example(fn) for fn in os.listdir(example()) if fn[-6:] == ".jaqal"]
+_fnames = [fn for fn in Path("examples", "jaqal").iterdir() if fn.suffix == ".jaqal"]
 
 
 def pytest_generate_tests(metafunc):
-    metafunc.parametrize("filename", [fn for fn in _fnames])
+    metafunc.parametrize("filename", list(_fnames))
 
 
 class TestExecuteAnnotatedJaqalFile:
     def test_jaqal_file(self, filename):
         with open(filename, "r") as f:
             txt = f.read()
```

### Comparing `JaqalPaq-1.1.1/tests/generator/test_generator.py` & `JaqalPaq-1.2.0a1/tests/generator/test_generator.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/jaqalparser/test_examples.py` & `JaqalPaq-1.2.0a1/tests/jaqalparser/test_examples.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/jaqalparser/test_jaqalpup_parser.py` & `JaqalPaq-1.2.0a1/tests/jaqalparser/test_jaqalpup_parser.py`

 * *Files identical despite different names*

### Comparing `JaqalPaq-1.1.1/tests/jaqalparser/test_parser.py` & `JaqalPaq-1.2.0a1/tests/jaqalparser/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,41 +183,41 @@
         """Test creating a loop."""
         text = "loop 1 { g0 1 }"
         sexpr = ["circuit", ["loop", 1, ["sequential_block", ["gate", "g0", 1]]]]
         self.run_test(text, sexpr)
 
     def test_branch_statement(self):
         """Test creating a branch statement."""
-        text = "branch { \n'0100': { g0 1 } \n '1010':{ g1 2} \n}"
+        text = "branch { \n'0010': { g0 1 } \n '0101':{ g1 2} \n}"
         sexpr = [
             "circuit",
             [
                 "branch",
                 ["case", 0b0100, ["sequential_block", ["gate", "g0", 1]]],
                 ["case", 0b1010, ["sequential_block", ["gate", "g1", 2]]],
             ],
         ]
         self.run_test(text, sexpr)
 
     def test_branch_statement_no_newlines(self):
         """Test creating a branch statement without using newlines."""
-        text = "branch { '0100': { g0 1 }; '1010':{ g1 2}; }"
+        text = "branch { '0010': { g0 1 }; '0101':{ g1 2}; }"
         sexpr = [
             "circuit",
             [
                 "branch",
                 ["case", 0b0100, ["sequential_block", ["gate", "g0", 1]]],
                 ["case", 0b1010, ["sequential_block", ["gate", "g1", 2]]],
             ],
         ]
         self.run_test(text, sexpr)
 
     def test_branch_statement_no_final_separator(self):
         """Test creating a branch with no separator after the final case."""
-        text = "branch { '0100': { g0 1 }; '1010':{ g1 2} }"
+        text = "branch { '0010': { g0 1 }; '0101':{ g1 2} }"
         sexpr = [
             "circuit",
             [
                 "branch",
                 ["case", 0b0100, ["sequential_block", ["gate", "g0", 1]]],
                 ["case", 0b1010, ["sequential_block", ["gate", "g1", 2]]],
             ],
```

### Comparing `JaqalPaq-1.1.1/tests/qsyntax/test_qsyntax.py` & `JaqalPaq-1.2.0a1/tests/qsyntax/test_qsyntax.py`

 * *Files identical despite different names*

