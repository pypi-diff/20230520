# Comparing `tmp/fitsnap3-3.0.1.2.tar.gz` & `tmp/fitsnap3-3.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsnap3-3.0.1.2.tar", last modified: Fri Apr 28 14:54:37 2023, max compression
+gzip compressed data, was "fitsnap3-3.1.0.1.tar", last modified: Fri May 19 23:51:21 2023, max compression
```

## Comparing `fitsnap3-3.0.1.2.tar` & `fitsnap3-3.1.0.1.tar`

### file list

```diff
@@ -1,171 +1,168 @@
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/
--rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.0.1.2/LICENSE
--rw-rw-r--   0 drew      (1000) drew      (1000)    24955 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/README.md
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1799 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3/__main__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3/fitsnap.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3.egg-info/
--rw-rw-r--   0 drew      (1000) drew      (1000)    24955 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     5292 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/SOURCES.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/dependency_links.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/requires.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-04-28 14:54:37.000000 fitsnap3-3.0.1.2/fitsnap3.egg-info/top_level.txt
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.947444 fitsnap3-3.0.1.2/fitsnap3lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/calculators/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2060 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    16381 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1191 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8511 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_base.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11541 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17979 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19992 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      433 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/calculators/template_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6496 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/fitsnap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3670 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/initialize.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/io/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/error.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6468 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/input.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      313 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.951444 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1712 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      746 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/output_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8305 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/outputs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7156 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14246 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      263 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/template_output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.955444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8204 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/ace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      322 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7382 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2183 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1033 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      902 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/eshift.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2267 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/extras.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4832 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/groups.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      855 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/memory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      996 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/outfile.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      717 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/path.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1223 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/reference.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1607 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2039 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/section_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6731 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/sections.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1112 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3152 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      473 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4578 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5629 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      482 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1587 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      364 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/template.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      960 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/io/sections/trainshift.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.959444 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pairwise.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pas.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12046 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/write.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13217 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/pace/pace.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/regressor.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/setup.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.963444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/gen_labels.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/genlib.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/tree_method.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/young.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      349 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/parallel_output.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    35256 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/parallel_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.967444 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4345 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/json_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17413 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scrape.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      759 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scraper_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/template_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    27314 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/vasp_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19146 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/scrapers/xyz_scraper.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.971444 fitsnap3-3.0.1.2/fitsnap3lib/solvers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3082 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/anl.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3169 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10164 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/bcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8565 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1786 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/lreg.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5291 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/mcmc.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4994 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/merr.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    39513 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2329 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/opt.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    42023 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2161 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3005 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    24006 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1091 2023-04-28 14:39:05.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1559 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/svd.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      388 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/template_solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1793 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/solvers/tensorflowsvd.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/fitsnap3lib/tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/configuration.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/dataframe_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/dataloaders.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/lammps_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/nn_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/tools/test_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/fitsnap3lib/units/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/conversion_finder.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/energy.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/force.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/length.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/mass.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/pressure.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/temperature.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/time.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.0.1.2/fitsnap3lib/units/units.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1095 2023-04-28 14:54:30.000000 fitsnap3-3.0.1.2/pyproject.toml
--rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/setup.cfg
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-04-28 14:54:37.975444 fitsnap3-3.0.1.2/tests/
--rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/tests/test_examples.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12841 2023-04-28 14:38:35.000000 fitsnap3-3.0.1.2/tests/test_pytorch.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.1.0.1/LICENSE
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24956 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3819 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/README.md
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2062 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3/__main__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3/fitsnap.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3.egg-info/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24956 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5206 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/SOURCES.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/dependency_links.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/requires.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-05-19 23:51:21.000000 fitsnap3-3.1.0.1/fitsnap3.egg-info/top_level.txt
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.847093 fitsnap3-3.1.0.1/fitsnap3lib/calculators/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    18640 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1240 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     9650 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_base.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11388 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    25241 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    28349 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10443 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/fitsnap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3811 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/initialize.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.851093 fitsnap3-3.1.0.1/fitsnap3lib/io/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/error.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7670 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/input.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      374 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.851093 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1645 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      905 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/output_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8636 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/outputs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7918 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14208 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      287 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/template_output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8163 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      346 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7408 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2209 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1057 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      850 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/eshift.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2301 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/extras.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4860 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/groups.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      881 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/memory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1022 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/outfile.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      745 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/path.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1249 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/reference.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1633 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/section_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6824 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/sections.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1136 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      497 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4495 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5562 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      506 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1611 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      387 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/template.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      986 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/io/sections/trainshift.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.855093 fitsnap3-3.1.0.1/fitsnap3lib/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pairwise.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pas.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12048 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/write.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.859093 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/regressor.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.863093 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/setup.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.863093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/genlib.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.867093 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/young.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      354 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/parallel_output.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    37710 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/parallel_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.871093 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4024 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/ase_funcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4513 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/json_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17005 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scrape.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      783 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scraper_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/template_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    27319 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/vasp_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19569 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/scrapers/xyz_scraper.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.875093 fitsnap3-3.1.0.1/fitsnap3lib/solvers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2906 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/anl.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2984 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10116 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/bcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8379 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/lreg.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5167 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/mcmc.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4828 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/merr.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    39329 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/opt.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    43491 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2868 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24358 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1110 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1622 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/svd.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      187 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/template_solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1733 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/solvers/tensorflowsvd.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.875093 fitsnap3-3.1.0.1/fitsnap3lib/tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/configuration.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/dataframe_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/dataloaders.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1157 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/group_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/lammps_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/nn_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/tools/test_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.879093 fitsnap3-3.1.0.1/fitsnap3lib/units/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/conversion_finder.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/energy.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/force.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/length.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/mass.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/pressure.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/temperature.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/time.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.1/fitsnap3lib/units/units.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1096 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/pyproject.toml
+-rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/setup.cfg
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-19 23:51:21.883093 fitsnap3-3.1.0.1/tests/
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.1/tests/test_examples.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11801 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.1/tests/test_pytorch.py
```

### Comparing `fitsnap3-3.0.1.2/LICENSE` & `fitsnap3-3.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/PKG-INFO` & `fitsnap3-3.1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.1.2
+Version: 3.1.0.1
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -356,15 +356,15 @@
         GNU Library General Public License instead of this License.
         
 Project-URL: repository, https://github.com/FitSNAP/FitSNAP
 Project-URL: documentation, https://fitsnap.github.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!----------------BEGIN-HEADER------------------------------------>
 
 <img width="300" alt="FitSNAP" src="https://github.com/FitSNAP/FitSNAP/blob/master/docs/images/FitSNAP.png">
```

### Comparing `fitsnap3-3.0.1.2/README.md` & `fitsnap3-3.1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3/__main__.py` & `fitsnap3-3.1.0.1/fitsnap3/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,45 +11,46 @@
 # #### Original author:
 #     Aidan P. Thompson, athomps (at) sandia (dot) gov (Sandia National Labs)
 #     http://www.cs.sandia.gov/~athomps
 #
 # #### Key contributors (alphabetical):
 #     Mary Alice Cusentino (Sandia National Labs)
 #     Nicholas Lubbers (Los Alamos National Lab)
+#     Drew Rohskopf (Sandia National Labs)
 #     Charles Sievers (UC Davis, Sandia National Labs)
 #     Adam Stephens (Sandia National Labs)
 #     Mitchell Wood (Sandia National Labs)
 #
 # #### Additional authors (alphabetical):
 #     Elizabeth Decolvenaere (D. E. Shaw Research)
 #     Stan Moore (Sandia National Labs)
 #     Steve Plimpton (Sandia National Labs)
 #     Gary Saavedra (Sandia National Labs)
 #     Peter Schultz (Sandia National Labs)
 #     Laura Swiler (Sandia National Labs)
 # <!-----------------END-HEADER------------------------------------->
 
 from fitsnap3lib.fitsnap import FitSnap
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.output import output
-from fitsnap3lib.initialize import initialize_fitsnap_run
 
 
-pt = ParallelTools()
-
-
-@pt.single_timeit
 def main():
-    try:
-        initialize_fitsnap_run()
-        snap = FitSnap()
-        snap.scrape_configs()
-        snap.process_configs()
-        pt.all_barrier()
-        snap.perform_fit()
-        snap.write_output()
+    # Instantiate single fitsnap instance for traditional flow of control.
+    # This will create an internal parallel tools instance which will detect
+    # availability of MPI for parallelization.
+    snap = FitSnap()
+    snap.scrape_configs(delete_scraper=True)
+    snap.process_configs(delete_data=True)
+    # Good practice after a large parallel operation is to impose a barrier.
+    snap.pt.all_barrier()
+    snap.perform_fit()
+    snap.write_output()
+    """
+    # TODO: Might be cleaner ways to output errors when doing massively parallel runs.
     except Exception as e:
-        output.exception(e)
+        #output.exception(e)
+        print(str(e))
+        snap.pt.single_print(f"{e}")
+    """
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3.egg-info/PKG-INFO` & `fitsnap3-3.1.0.1/fitsnap3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.0.1.2
+Version: 3.1.0.1
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991 
         
@@ -356,15 +356,15 @@
         GNU Library General Public License instead of this License.
         
 Project-URL: repository, https://github.com/FitSNAP/FitSNAP
 Project-URL: documentation, https://fitsnap.github.io/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!----------------BEGIN-HEADER------------------------------------>
 
 <img width="300" alt="FitSNAP" src="https://github.com/FitSNAP/FitSNAP/blob/master/docs/images/FitSNAP.png">
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3.egg-info/SOURCES.txt` & `fitsnap3-3.1.0.1/fitsnap3.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 fitsnap3.egg-info/top_level.txt
 fitsnap3lib/__init__.py
 fitsnap3lib/fitsnap.py
 fitsnap3lib/initialize.py
 fitsnap3lib/parallel_output.py
 fitsnap3lib/parallel_tools.py
 fitsnap3lib/calculators/__init__.py
-fitsnap3lib/calculators/basic_calculator.py
 fitsnap3lib/calculators/calculator.py
 fitsnap3lib/calculators/calculator_factory.py
 fitsnap3lib/calculators/lammps_base.py
 fitsnap3lib/calculators/lammps_custom.py
 fitsnap3lib/calculators/lammps_pace.py
 fitsnap3lib/calculators/lammps_snap.py
-fitsnap3lib/calculators/template_calculator.py
 fitsnap3lib/io/__init__.py
 fitsnap3lib/io/error.py
 fitsnap3lib/io/input.py
 fitsnap3lib/io/output.py
 fitsnap3lib/io/outputs/__init__.py
 fitsnap3lib/io/outputs/custom.py
 fitsnap3lib/io/outputs/output_factory.py
@@ -68,16 +66,14 @@
 fitsnap3lib/lib/neural_networks/pairwise.py
 fitsnap3lib/lib/neural_networks/pas.py
 fitsnap3lib/lib/neural_networks/pytorch.py
 fitsnap3lib/lib/neural_networks/write.py
 fitsnap3lib/lib/neural_networks/descriptors/__init__.py
 fitsnap3lib/lib/neural_networks/descriptors/bessel.py
 fitsnap3lib/lib/neural_networks/descriptors/g3b.py
-fitsnap3lib/lib/pace/__init__.py
-fitsnap3lib/lib/pace/pace.py
 fitsnap3lib/lib/ridge_solver/__init__.py
 fitsnap3lib/lib/ridge_solver/regressor.py
 fitsnap3lib/lib/scalapack_solver/__init__.py
 fitsnap3lib/lib/scalapack_solver/scalapack.py
 fitsnap3lib/lib/scalapack_solver/setup.py
 fitsnap3lib/lib/sym_ACE/__init__.py
 fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
@@ -95,14 +91,15 @@
 fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
 fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
 fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
 fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
 fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
 fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
 fitsnap3lib/scrapers/__init__.py
+fitsnap3lib/scrapers/ase_funcs.py
 fitsnap3lib/scrapers/json_scraper.py
 fitsnap3lib/scrapers/scrape.py
 fitsnap3lib/scrapers/scraper_factory.py
 fitsnap3lib/scrapers/template_scraper.py
 fitsnap3lib/scrapers/vasp_scraper.py
 fitsnap3lib/scrapers/xyz_scraper.py
 fitsnap3lib/solvers/__init__.py
@@ -124,14 +121,15 @@
 fitsnap3lib/solvers/svd.py
 fitsnap3lib/solvers/template_solver.py
 fitsnap3lib/solvers/tensorflowsvd.py
 fitsnap3lib/tools/__init__.py
 fitsnap3lib/tools/configuration.py
 fitsnap3lib/tools/dataframe_tools.py
 fitsnap3lib/tools/dataloaders.py
+fitsnap3lib/tools/group_tools.py
 fitsnap3lib/tools/lammps_tools.py
 fitsnap3lib/tools/nn_tools.py
 fitsnap3lib/tools/test_tools.py
 fitsnap3lib/units/__init__.py
 fitsnap3lib/units/conversion_finder.py
 fitsnap3lib/units/energy.py
 fitsnap3lib/units/force.py
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,80 @@
-from fitsnap3lib.parallel_tools import ParallelTools, double_size, DistributedList, stubs
-from fitsnap3lib.io.input import Config
-from fitsnap3lib.io.output import output
+from fitsnap3lib.parallel_tools import double_size, DistributedList, stubs #, ParallelTools
+#from fitsnap3lib.io.input import Config
+#from fitsnap3lib.io.output import output
 import numpy as np
 import pandas as pd
 
 
 #config = Config()
 #pt = ParallelTools()
 
 
 class Calculator:
+    """ Class for allocating, calculating, and collating descriptors. """
 
-    def __init__(self, name):
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        self.pt = pt #ParallelTools()
+        self.config = config #Config()
         self.name = name
         self.number_of_atoms = None
         self.number_of_files_per_node = None
         self.shared_index = None
         self.distributed_index = 0
 
     def get_width(self):
         pass
+    
+    def create_dicts(self, nconfigs):
+        """
+        Create dictionaries for certain distributed lists.
+        Each list should be of size `nconfigs` of a single proc.
+
+        Args:
+            nconfigs: int number of configs on this proc.
+        """
+
+        # Lists of length number of configs.
+        self.pt.add_2_fitsnap("Groups", DistributedList(nconfigs))
+        self.pt.add_2_fitsnap("Configs", DistributedList(nconfigs))
+        self.pt.add_2_fitsnap("Testing", DistributedList(nconfigs))
+
+    def allocate_per_config(self, data: list):
+        """
+        Allocate shared arrays for total number of atoms. This is only needed 
+        when doing big A matrix fits (need number of atoms) or nonlinear 
+        fits.
+
+        Args:
+            data: List of data dictionaries.
+        """
+        ncpn = self.pt.get_ncpn(len(data))
+
+        self.pt.create_shared_array('number_of_atoms', ncpn, dtype='i')
+        self.pt.slice_array('number_of_atoms')
+
+        # number of dgrad rows serves similar purpose as number of atoms
+        
+        self.pt.create_shared_array('number_of_dgrad_rows', ncpn, dtype='i')
+        self.pt.slice_array('number_of_dgrad_rows')
+
+        # number of neighs serves similar purpose as number of atoms for custom calculator
+        
+        self.pt.create_shared_array('number_of_neighs_scrape', ncpn, dtype='i')
+        self.pt.slice_array('number_of_neighs_scrape')
+
+        # Loop through data and set sliced number of atoms.
+        for i, configuration in enumerate(data):
+            natoms = np.shape(configuration["Positions"])[0]
+            self.pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
 
     def create_a(self):
+        """
+        Allocate shared arrays for calculator.
+        """
 
         # TODO : Any extra config pulls should be done before this
 
         self.pt.sub_barrier()
         # total number of atoms in all configs, summed
         self.number_of_atoms = self.pt.shared_arrays["number_of_atoms"].array.sum()
         # total number of configs on all procs in a node
@@ -66,22 +113,23 @@
 
             a_width = self.get_width()
             assert isinstance(a_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
 
             a_size = ( (a_len * a_width) + (dgrad_len * a_width) ) * double_size
-            output.screen(">>> Matrix of descriptors and descriptor derivatives takes up ", 
-                          "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
-                          "% of the total memory:", 
-                          "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
+            if self.config.args.verbose:
+                self.pt.single_print(">>> Matrix of descriptors and descriptor derivatives takes up ", 
+                              "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
+                              "% of the total memory:", 
+                              "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The descriptor matrix is larger than 50% of your RAM. \n Aborting...!")
             elif a_size / self.pt.get_ram() > 0.5 and self.config.sections["MEMORY"].override:
-                output.screen("Warning: I hope you know what you are doing!")
+                self.pt.single_print("Warning: > 50% RAM. I hope you know what you are doing!")
 
             self.pt.create_shared_array('a', a_len, a_width, 
                                         tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('b', b_len, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('c', c_len, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('w', b_len, 2, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('t', a_len, 1, tm=self.config.sections["SOLVER"].true_multinode)
@@ -145,20 +193,21 @@
 
             a_width = 2 # types and numneighs
             neighlist_width = self.get_width()
             assert isinstance(neighlist_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
             a_size = (neighlist_len * neighlist_width + 2 * c_len * c_width) * double_size
-            output.screen(">>> Matrix of data takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
-                          "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
+            if self.config.args.verbose:
+                self.pt.single_print(">>> Matrix of data takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
+                              "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The data memory larger than 50% of your RAM. \n Aborting...!")
             elif a_size / self.pt.get_ram() > 0.5 and self.config.sections["MEMORY"].override:
-                output.screen("Warning: I hope you know what you are doing!")
+                self.pt.single_print("Warning: > 50 % RAM. I hope you know what you are doing!")
 
             # create shared arrays
             a_width = 5
             neighlist_width = 2 # i j 
             xneigh_width = 3 # xj yj zj, with PBC corrections
             self.pt.create_shared_array('a', a_len, a_width, 
                                         tm=self.config.sections["SOLVER"].true_multinode)
@@ -222,25 +271,25 @@
                 a_len += self.number_of_files_per_node * 6
 
             a_width = self.get_width()
             assert isinstance(a_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
             a_size = a_len * a_width * double_size
-            output.screen(">>> Matrix of descriptors takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
-                          "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
+            if self.config.args.verbose:
+                self.pt.single_print(">>> Matrix of descriptors takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
+                              "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB") #, "on rank", "{:d}".format(self.pt._rank))
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The descriptor matrix is larger than 50% of your RAM. \n Aborting...!")
             elif a_size / self.pt.get_ram() > 0.5 and self.config.sections["MEMORY"].override:
-                output.screen("Warning: I hope you know what you are doing!")
+                self.pt.single_print("Warning: > 50 % RAM. I hope you know what you are doing!")
 
             self.pt.create_shared_array('a', a_len, a_width, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('b', a_len, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.create_shared_array('w', a_len, tm=self.config.sections["SOLVER"].true_multinode)
-            #self.pt.create_shared_array('ref', a_len, tm=self.config.sections["SOLVER"].true_multinode)
             self.pt.new_slice_a()
             self.shared_index = self.pt.fitsnap_dict["sub_a_indices"][0]
             # pt.slice_array('a')
 
             self.pt.add_2_fitsnap("Groups", DistributedList(self.pt.fitsnap_dict["sub_a_size"]))
             self.pt.add_2_fitsnap("Configs", DistributedList(self.pt.fitsnap_dict["sub_a_size"]))
             self.pt.add_2_fitsnap("Row_Type", DistributedList(self.pt.fitsnap_dict["sub_a_size"]))
@@ -253,49 +302,50 @@
 
     def preprocess_configs(self, data, i):
         pass
 
     def preprocess_allocate(self, nconfigs):
         pass
 
-    @staticmethod
-    def collect_distributed_lists():
+    #@staticmethod # NOTE: Does this need to be a static method?
+    def collect_distributed_lists(self, allgather: bool=False):
         """
         Gathers all the distributed lists on each proc to the root proc.
         For each distributed list (fitsnap dicts) this will create a concatenated list on the root proc.
         We use this function in fitsnap.py after processing configs.
-        """
-        pt = ParallelTools()    
-        for key in pt.fitsnap_dict.keys():
-            if isinstance(pt.fitsnap_dict[key], DistributedList):
-                pt.gather_fitsnap(key)
-                if pt.fitsnap_dict[key] is not None and stubs != 1:
-                    pt.fitsnap_dict[key] = [item for sublist in pt.fitsnap_dict[key] for item in sublist]
-                elif pt.fitsnap_dict[key] is not None:
-                    pt.fitsnap_dict[key] = pt.fitsnap_dict[key].get_list()
+
+        Args:
+            allgather: Whether to gather lists on all nodes or just the head node.
+        """   
+        for key in self.pt.fitsnap_dict.keys():
+            if isinstance(self.pt.fitsnap_dict[key], DistributedList):
+                self.pt.gather_fitsnap(key)
+                if self.pt.fitsnap_dict[key] is not None and stubs != 1:
+                    self.pt.fitsnap_dict[key] = [item for sublist in self.pt.fitsnap_dict[key] for item in sublist]
+                elif self.pt.fitsnap_dict[key] is not None:
+                    self.pt.fitsnap_dict[key] = self.pt.fitsnap_dict[key].get_list()
 
     #@pt.rank_zero
     def extras(self):
         @self.pt.rank_zero
-        def decorated_extras():
-            pt = ParallelTools()
-            config = Config()
-            if config.sections["EXTRAS"].dump_a:
-                np.save(config.sections['EXTRAS'].descriptor_file, pt.shared_arrays['a'].array)
-            if config.sections["EXTRAS"].dump_b:
-                np.save(config.sections['EXTRAS'].truth_file, pt.shared_arrays['b'].array)
-            if config.sections["EXTRAS"].dump_w:
-                np.save(config.sections['EXTRAS'].weights_file, pt.shared_arrays['w'].array)
-            if config.sections["EXTRAS"].dump_dataframe:
-                df = pd.DataFrame(pt.shared_arrays['a'].array)
-                df['truths'] = pt.shared_arrays['b'].array.tolist()
-                df['weights'] = pt.shared_arrays['w'].array.tolist()
-                for key in pt.fitsnap_dict.keys():
-                    if isinstance(pt.fitsnap_dict[key], list) and len(pt.fitsnap_dict[key]) == len(df.index):
-                        df[key] = pt.fitsnap_dict[key]
-                df.to_pickle(config.sections['EXTRAS'].dataframe_file)
+        def extras():
+            if self.config.sections["EXTRAS"].dump_a:
+                np.save(self.config.sections['EXTRAS'].descriptor_file, self.pt.shared_arrays['a'].array)
+            if self.config.sections["EXTRAS"].dump_b:
+                np.save(self.config.sections['EXTRAS'].truth_file, self.pt.shared_arrays['b'].array)
+            if self.config.sections["EXTRAS"].dump_w:
+                np.save(self.config.sections['EXTRAS'].weights_file, self.pt.shared_arrays['w'].array)
+            if self.config.sections["EXTRAS"].dump_dataframe:
+                df = pd.DataFrame(self.pt.shared_arrays['a'].array)
+                df['truths'] = self.pt.shared_arrays['b'].array.tolist()
+                df['weights'] = self.pt.shared_arrays['w'].array.tolist()
+                for key in self.pt.fitsnap_dict.keys():
+                    if isinstance(self.pt.fitsnap_dict[key], list) and len(self.pt.fitsnap_dict[key]) == len(df.index):
+                        df[key] = self.pt.fitsnap_dict[key]
+                df.to_pickle(self.config.sections['EXTRAS'].dataframe_file)
                 del df
-        decorated_extras()
+        if "EXTRAS" in self.config.sections:
+            extras()
 
         # if not config.sections["SOLVER"].detailed_errors:
         #     print(
         #         ">>>Enable [SOLVER], detailed_errors = 1 to characterize the training/testing split of your output *.npy matricies")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/calculator_factory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/calculator_factory.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from fitsnap3lib.parallel_tools import ParallelTools
 from fitsnap3lib.calculators.calculator import Calculator
 from fitsnap3lib.calculators.lammps_pace import LammpsPace
 from fitsnap3lib.calculators.lammps_snap import LammpsSnap
-from fitsnap3lib.calculators.basic_calculator import Basic
+#from fitsnap3lib.calculators.basic_calculator import Basic
 from fitsnap3lib.calculators.lammps_custom import LammpsCustom
 
 
 #pt = ParallelTools()
 
-def calculator(calculator_name):
+def calculator(calculator_name, pt, cfg):
     """Calculator Factory"""
     instance = search(calculator_name)
-    pt = ParallelTools()
-    pt.single_print("Using {} as FitSNAP calculator".format(calculator_name))
+    #pt = ParallelTools()
+    if cfg.args.verbose:
+        pt.single_print("Using {} as FitSNAP calculator".format(calculator_name))
     
-    instance.__init__(calculator_name)
+    instance.__init__(calculator_name, pt, cfg)
     return instance
 
 
 def search(calculator_name):
     instance = None
 
     # loop over subclasses of Calculator
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_base.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 import ctypes
 from fitsnap3lib.calculators.calculator import Calculator
-from fitsnap3lib.parallel_tools import ParallelTools, DistributedList
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 class LammpsBase(Calculator):
 
-    def __init__(self, name):
-        super().__init__(name)
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self._data = {}
         self._i = 0
         self._lmp = None
         self.pt.check_lammps()
 
     def create_a(self):
         super().create_a()
 
-    def preprocess_allocate(self, nconfigs):
+    def preprocess_allocate(self, nconfigs: int):
         """
         Allocate arrays to be used by this proc. These arrays have size nconfigs.
 
-        Attributes
-        ----------
-        nconfigs : int 
-            number of configs on this proc
-
-        pt.shared_arrays['number_of_dgradrows'] : np array
-            number of dgrad rows per config, organized like the other shared arrays in calculator.py
-            
-        pt.shared_arrays['number_of_neighs'] : np array
-            number of neighbors per config, organized like the other shared arrays in calculator.py
+        Args:
+            nconfigs : number of configs on this proc
         """
         self.dgradrows = np.zeros(nconfigs).astype(int)
+        # number of dgrad rows per config, organized like the other shared arrays in calculator.py
         self.pt.create_shared_array('number_of_dgradrows', nconfigs, tm=self.config.sections["SOLVER"].true_multinode)
+        # number of neighbors per config, organized like the other shared arrays in calculator.py
         self.pt.create_shared_array('number_of_neighs', nconfigs, tm=self.config.sections["SOLVER"].true_multinode)
         self.nconfigs = nconfigs
 
     def preprocess_configs(self, data, i):
         try:
             self._data = data
             self._i = i
@@ -58,33 +46,41 @@
             self._prepare_lammps()
             self._run_lammps()
             self._collect_lammps_preprocess()
             self._lmp = self.pt.close_lammps()
             raise e
 
     def process_configs(self, data, i):
+        """
+        Calculate descriptors for a given configuration.
+        Action of this function is altered by certain attributes.
+
+        Args:
+            transpose_trick : Don't touch shared arrays in `_collect_lammps()` if true. Instead 
+                              store smaller matrices `self.aw`, `self.bw`.
+        """
         try:
             self._data = data
             self._i = i
             self._initialize_lammps()
             self._prepare_lammps()
             self._run_lammps()
             self._collect_lammps()
             self._lmp = self.pt.close_lammps()
         except Exception as e:
-            if self.config.args.printlammps:
-                self._data = data
-                self._i = i
-                self._initialize_lammps(1)
-                self._prepare_lammps()
-                self._run_lammps()
-                self._collect_lammps()
-                self._lmp = self.pt.close_lammps()
+            #if self.config.args.printlammps:
+            self._data = data
+            self._i = i
+            self._initialize_lammps(1)
+            self._prepare_lammps()
+            self._run_lammps()
+            self._collect_lammps()
+            self._lmp = self.pt.close_lammps()
             raise e
-
+        
     def process_configs_nonlinear(self, data, i):
         try:
             self._data = data
             self._i = i
             self._initialize_lammps()
             self._prepare_lammps()
             self._run_lammps()
@@ -97,14 +93,41 @@
             self._initialize_lammps(1)
             self._prepare_lammps()
             self._run_lammps()
             self._collect_lammps_nonlinear()
             self._lmp = self.pt.close_lammps()
             raise e
 
+        
+    def process_single(self, data, i=0):
+        """
+        Calculate descriptors on a single configuration without touching the shraed arrays.
+
+        Args:
+            data: dictionary of structural and fitting info for a configuration in fitsnap
+                  data dictionary format.
+            i: integer index which is optional, mainly for debugging purposes.
+        
+        Returns: 
+            - A matrix of descriptors depending on settings declared in `CALCULATOR`. If 
+              `bikflag` is 0 (default) then A has 1 and 0s in the first column since it is ready to 
+              fit with linear solvers; the descriptors are also divided by no. atoms in this case. 
+              If `bikflag` is 1, then A is simply an unaltered per-atom descriptor matrix.
+            - b vector of truths
+            - w vector of weights
+        """
+        self._data = data
+        self._i = i
+        self._initialize_lammps()
+        self._prepare_lammps()
+        self._run_lammps()
+        a,b,w = self._collect_lammps_single()
+        self._lmp = self.pt.close_lammps()
+        return a,b,w
+
     def _prepare_lammps(self):
         raise NotImplementedError
 
     def _collect_lammps(self):
         raise NotImplementedError
 
     def _set_box(self):
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_custom.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np
-from fitsnap3lib.parallel_tools import ParallelTools, DistributedList
 from fitsnap3lib.io.input import Config
 from fitsnap3lib.lib.neural_networks.descriptors.bessel import Bessel
 from fitsnap3lib.lib.neural_networks.descriptors.g3b import Gaussian3Body
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
 class LammpsCustom(LammpsBase):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self._data = {}
         self._i = 0
         self._lmp = None
         self._row_index = 0
         self.pt.check_lammps()
 
         # declare objects for calculating descriptors used to standardize the network
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_pace.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_pace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 class LammpsPace(LammpsBase):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self._data = {}
         self._i = 0
         self._lmp = None
         self._row_index = 0
         self.pt.check_lammps()
 
     def get_width(self):
-        if (self.config.sections["SOLVER"].solver == "PYTORCH"):
+        if (self.config.sections["CALCULATOR"].nonlinear):
             a_width = self.config.sections["ACE"].ncoeff
         else:
             num_types = self.config.sections["ACE"].numtypes
             a_width = self.config.sections["ACE"].ncoeff  * num_types
             if not self.config.sections["ACE"].bzeroflag:
                 a_width += num_types
         return a_width
@@ -197,14 +189,165 @@
 
         self.shared_index = index
         self.distributed_index = dindex
         self.shared_index_b = index_b
         self.shared_index_c = index_c
         self.shared_index_dgrad = index_dgrad
 
+    def _collect_lammps_single(self):
+        num_atoms = self._data["NumAtoms"]
+        num_types = self.config.sections['ACE'].numtypes
+        n_coeff = self.config.sections['ACE'].ncoeff
+        energy = self._data["Energy"]
+
+        lmp_atom_ids = self._lmp.numpy.extract_atom_iarray("id", num_atoms).ravel()
+        assert np.all(lmp_atom_ids == 1 + np.arange(num_atoms)), "LAMMPS seems to have lost atoms"
+
+        # Extract positions
+        lmp_pos = self._lmp.numpy.extract_atom_darray(name="x", nelem=num_atoms, dim=3)
+        # Extract types
+        lmp_types = self._lmp.numpy.extract_atom_iarray(name="type", nelem=num_atoms).ravel()
+        lmp_volume = self._lmp.get_thermo("vol")
+
+        # Extract pace data, including reference potential data
+
+        nrows_energy = 1
+        bik_rows = 1
+        ndim_force = 3
+        nrows_force = ndim_force * num_atoms
+        ndim_virial = 6
+        nrows_virial = ndim_virial
+        nrows_pace = nrows_energy + nrows_force + nrows_virial
+        ncols_bispectrum = n_coeff * num_types
+        ncols_reference = 1
+        ncols_pace = ncols_bispectrum + ncols_reference
+        index = 0 #self.shared_index
+        dindex = self.distributed_index
+        lmp_pace = _extract_compute_np(self._lmp, "pace", 0, 2, (nrows_pace, ncols_pace))
+
+        # If doing per-atom descriptors, we want a different shape (one less column).
+        if self.config.sections['ACE'].bikflag:
+            if not self.config.sections['ACE'].bzeroflag:
+                raise ValueError("bikflag = 1 requires bzeroflag = 1")
+            nrows = 0
+            if self.config.sections['CALCULATOR'].energy:
+                nrows += num_atoms
+            if self.config.sections['CALCULATOR'].force:
+                nrows += 3*num_atoms
+            if self.config.sections['CALCULATOR'].stress:
+                nrows += 6
+            nd = np.shape(lmp_pace)[1]-1
+            na = nrows #np.shape(lmp_snap)[0]
+            a = np.zeros((na, nd))
+            b = np.zeros(na)
+            w = np.zeros(na)
+            #print(lmp_pace[0:,:])
+            #assert(False)
+        else:
+            nd = np.shape(lmp_pace)[1]
+            na = np.shape(lmp_pace)[0]
+            a = np.zeros((na, nd))
+            b = np.zeros(na)
+            w = np.zeros(na)
+
+        if (np.isinf(lmp_pace)).any() or (np.isnan(lmp_pace)).any():
+            self.pt.single_print('WARNING! applying np.nan_to_num()')
+            lmp_pace = np.nan_to_num(lmp_pace)
+        if (np.isinf(lmp_pace)).any() or (np.isnan(lmp_pace)).any():
+            raise ValueError('Nan in computed data of file {} in group {}'.format(self._data["File"],
+                                                                                  self._data["Group"]))
+
+        irow = 0
+        bik_rows = 1
+        if self.config.sections['ACE'].bikflag:
+            bik_rows = num_atoms
+        icolref = ncols_bispectrum
+        if self.config.sections["CALCULATOR"].energy:
+            b_sum_temp = lmp_pace[irow:irow+bik_rows, :ncols_bispectrum]
+            if not self.config.sections["ACE"].bikflag:
+                # Divide by natoms if not extracting per-atom descriptors.
+                b_sum_temp /= num_atoms
+
+            # Check for no neighbors using B[0,0,0] components
+            # these strictly increase with total neighbor count
+            # minimum value depends on PACE variant
+
+            EPS = 1.0e-10
+            b000sum0 = 0.0
+            nstride = n_coeff
+            b000sum = sum(b_sum_temp[::nstride])
+            if not self.config.sections['ACE'].bikflag:
+                if not self.config.sections["ACE"].bzeroflag:
+                    b000sum0 = 1.0
+                    if (abs(b000sum - b000sum0) < EPS): 
+                        self.pt.single_print("WARNING: Configuration has no PACE neighbors")
+
+                b_sum_temp.shape = (num_types, n_coeff)
+                onehot_atoms = np.zeros((num_types, 1))
+                for atom in self._data["AtomTypes"]:
+                    onehot_atoms[self.config.sections["ACE"].type_mapping[atom]-1] += 1
+                onehot_atoms /= len(self._data["AtomTypes"])
+                b_sum_temp = np.concatenate((onehot_atoms, b_sum_temp), axis=1)
+                #b_sum_temp.shape = (num_types * (n_coeff + num_types))
+                b_sum_temp.shape = (num_types * n_coeff + num_types)
+
+            #a[irow] = b_sum_temp * self.config.sections["ACE"].blank2J
+            a[irow:irow+bik_rows] = b_sum_temp * self.config.sections["ACE"].blank2J[np.newaxis, :]
+            ref_energy = lmp_pace[irow, icolref]
+            b[irow] = (energy - ref_energy) / num_atoms
+            w[irow] = self._data["eweight"] if "eweight" in self._data else 1.0
+
+            index += nrows_energy
+            dindex += nrows_energy
+        irow += nrows_energy
+
+        if self.config.sections["CALCULATOR"].force:
+            db_atom_temp = lmp_pace[irow:irow + nrows_force, :ncols_bispectrum]
+            db_atom_temp.shape = (num_atoms * ndim_force, n_coeff * num_types)
+            if not self.config.sections["ACE"].bzeroflag:
+                db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types, n_coeff)
+                onehot_atoms = np.zeros((np.shape(db_atom_temp)[0], num_types, 1))
+                db_atom_temp = np.concatenate([onehot_atoms, db_atom_temp], axis=2)
+                db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types * n_coeff + num_types)
+            a[irow:irow+num_atoms * ndim_force] = np.matmul(db_atom_temp, np.diag(self.config.sections["ACE"].blank2J))
+            ref_forces = lmp_pace[irow:irow + nrows_force, icolref]
+            b[irow:irow+num_atoms * ndim_force] = self._data["Forces"].ravel() - ref_forces
+            w[irow:irow+nrows_force] = self._data["fweight"] if "fweight" in self._data else 1.0
+            index += nrows_force
+            dindex += nrows_force
+        irow += nrows_force
+
+        if self.config.sections["CALCULATOR"].stress:
+            vb_sum_temp = 1.6021765e6*lmp_pace[irow:irow + nrows_virial, :ncols_bispectrum] / lmp_volume
+            vb_sum_temp.shape = (ndim_virial, n_coeff * num_types)
+            if not self.config.sections["ACE"].bzeroflag:
+                vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types, n_coeff)
+                onehot_atoms = np.zeros((np.shape(vb_sum_temp)[0], num_types, 1))
+                vb_sum_temp = np.concatenate([onehot_atoms, vb_sum_temp], axis=2)
+                vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types * n_coeff + num_types)
+            a[irow:irow+ndim_virial] = np.matmul(vb_sum_temp, np.diag(self.config.sections["ACE"].blank2J))
+            ref_stress = lmp_pace[irow:irow + nrows_virial, icolref]
+            b[irow:irow+ndim_virial] = self._data["Stress"][[0, 1, 2, 1, 0, 0], [0, 1, 2, 2, 2, 1]].ravel() - ref_stress
+            w[irow:irow+ndim_virial] = self._data["vweight"] if "vweight" in self._data else 1.0
+            index += ndim_virial
+            dindex += ndim_virial
+
+        length = dindex - self.distributed_index
+
+        """
+        self.pt.fitsnap_dict['Groups'][self.distributed_index:dindex] = ['{}'.format(self._data['Group'])] * length
+        self.pt.fitsnap_dict['Configs'][self.distributed_index:dindex] = ['{}'.format(self._data['File'])] * length
+        self.pt.fitsnap_dict['Testing'][self.distributed_index:dindex] = [bool(self._data['test_bool'])] * length
+        """
+        self.shared_index = index
+        self.distributed_index = dindex
+
+        return a,b,w
+        
+
     def _collect_lammps(self):
 
         num_atoms = self._data["NumAtoms"]
         num_types = self.config.sections['ACE'].numtypes
         n_coeff = self.config.sections['ACE'].ncoeff
         energy = self._data["Energy"]
 
@@ -228,14 +371,15 @@
         nrows_pace = nrows_energy + nrows_force + nrows_virial
         ncols_bispectrum = n_coeff * num_types
         ncols_reference = 1
         ncols_pace = ncols_bispectrum + ncols_reference
         index = self.shared_index
         dindex = self.distributed_index
         lmp_pace = _extract_compute_np(self._lmp, "pace", 0, 2, (nrows_pace, ncols_pace))
+
         if (np.isinf(lmp_pace)).any() or (np.isnan(lmp_pace)).any():
             self.pt.single_print('WARNING! applying np.nan_to_num()')
             lmp_pace = np.nan_to_num(lmp_pace)
         if (np.isinf(lmp_pace)).any() or (np.isnan(lmp_pace)).any():
             raise ValueError('Nan in computed data of file {} in group {}'.format(self._data["File"],
                                                                                   self._data["Group"]))
 
@@ -263,15 +407,14 @@
 
                 b_sum_temp.shape = (num_types, n_coeff)
                 onehot_atoms = np.zeros((num_types, 1))
                 for atom in self._data["AtomTypes"]:
                     onehot_atoms[self.config.sections["ACE"].type_mapping[atom]-1] += 1
                 onehot_atoms /= len(self._data["AtomTypes"])
                 b_sum_temp = np.concatenate((onehot_atoms, b_sum_temp), axis=1)
-                #b_sum_temp.shape = (num_types * (n_coeff + num_types))
                 b_sum_temp.shape = (num_types * n_coeff + num_types)
             self.pt.shared_arrays['a'].array[index] = b_sum_temp * self.config.sections["ACE"].blank2J
             ref_energy = lmp_pace[irow, icolref]
             self.pt.shared_arrays['b'].array[index] = (energy - ref_energy) / num_atoms
             self.pt.shared_arrays['w'].array[index] = self._data["eweight"]
             self.pt.fitsnap_dict['Row_Type'][dindex:dindex + bik_rows] = ['Energy'] * nrows_energy
             self.pt.fitsnap_dict['Atom_I'][dindex:dindex + bik_rows] = [int(i) for i in range(nrows_energy)]
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/calculators/lammps_snap.py` & `fitsnap3-3.1.0.1/fitsnap3lib/calculators/lammps_snap.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from fitsnap3lib.calculators.lammps_base import LammpsBase, _extract_compute_np
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 class LammpsSnap(LammpsBase):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self._data = {}
         self._i = 0
         self._lmp = None
         self._row_index = 0
         self.pt.check_lammps()
 
     def get_width(self):
-        if (self.config.sections["SOLVER"].solver == "PYTORCH"):
+        if (self.config.sections["CALCULATOR"].nonlinear):
             a_width = self.config.sections["BISPECTRUM"].ncoeff #+ 3
         else:
             num_types = self.config.sections["BISPECTRUM"].numtypes
             a_width = self.config.sections["BISPECTRUM"].ncoeff * num_types
             if not self.config.sections["BISPECTRUM"].bzeroflag:
                 a_width += num_types
         return a_width
@@ -219,14 +211,186 @@
 
         self.shared_index = index
         self.distributed_index = dindex
         self.shared_index_b = index_b
         self.shared_index_c = index_c
         self.shared_index_dgrad = index_dgrad
 
+    def _collect_lammps_single(self):
+
+        num_atoms = self._data["NumAtoms"]
+        num_types = self.config.sections['BISPECTRUM'].numtypes
+        n_coeff = self.config.sections['BISPECTRUM'].ncoeff
+        energy = self._data["Energy"]
+        lmp_atom_ids = self._lmp.numpy.extract_atom_iarray("id", num_atoms).ravel()
+        assert np.all(lmp_atom_ids == 1 + np.arange(num_atoms)), "LAMMPS seems to have lost atoms"
+
+        # Extract positions
+        lmp_pos = self._lmp.numpy.extract_atom_darray(name="x", nelem=num_atoms, dim=3)
+        # Extract types
+        lmp_types = self._lmp.numpy.extract_atom_iarray(name="type", nelem=num_atoms).ravel()
+        lmp_volume = self._lmp.get_thermo("vol")
+
+        # Extract SNAP data, including reference potential data
+
+        bik_rows = 1
+        if self.config.sections['BISPECTRUM'].bikflag:
+            bik_rows = num_atoms
+        nrows_energy = bik_rows
+        ndim_force = 3
+        nrows_force = ndim_force * num_atoms
+        ndim_virial = 6
+        nrows_virial = ndim_virial
+        nrows_snap = nrows_energy + nrows_force + nrows_virial
+        ncols_bispectrum = n_coeff * num_types
+        ncols_reference = 1
+        ncols_snap = ncols_bispectrum + ncols_reference
+        # index = pt.fitsnap_dict['a_indices'][self._i]
+        index = 0
+        dindex = self.distributed_index
+
+        lmp_snap = _extract_compute_np(self._lmp, "snap", 0, 2, (nrows_snap, ncols_snap))
+
+        # We want first column to be 1, 0, ... 0.
+        # Next columns are bispectrum components.
+        # Take last column of `lmp_snap` as the `b` vector.
+
+        # Get individual A matrices for this configuration.
+
+        #print(np.shape(lmp_snap))
+        #assert(False)
+
+        # If doing per-atom descriptors, we want a different shape (one less column).
+        if self.config.sections['BISPECTRUM'].bikflag:
+            nrows = 0
+            if self.config.sections['CALCULATOR'].energy:
+                nrows += num_atoms
+            if self.config.sections['CALCULATOR'].force:
+                nrows += 3*num_atoms
+            if self.config.sections['CALCULATOR'].stress:
+                nrows += 6
+            nd = np.shape(lmp_snap)[1]-1
+            na = nrows #np.shape(lmp_snap)[0]
+            a = np.zeros((na, nd))
+            b = np.zeros(na)
+            w = np.zeros(na)
+        else:
+            nd = np.shape(lmp_snap)[1]
+            na = np.shape(lmp_snap)[0]
+            a = np.zeros((na, nd))
+            b = np.zeros(na)
+            w = np.zeros(na)
+
+        if (np.isinf(lmp_snap)).any() or (np.isnan(lmp_snap)).any():
+            raise ValueError('Nan in computed data of file {} in group {}'.format(self._data["File"],
+                                                                                  self._data["Group"]))
+        irow = 0
+        bik_rows = 1
+        if self.config.sections['BISPECTRUM'].bikflag:
+            bik_rows = num_atoms
+        icolref = ncols_bispectrum
+        if self.config.sections["CALCULATOR"].energy:
+            b_sum_temp = lmp_snap[irow:irow+bik_rows, :ncols_bispectrum]
+            if not self.config.sections["BISPECTRUM"].bikflag:
+                # Divide by natoms if not extracting per-atom descriptors.
+                b_sum_temp /= num_atoms
+
+            # Check for no neighbors using B[0,0,0] components
+            # these strictly increase with total neighbor count
+            # minimum value depends on SNAP variant
+
+            EPS = 1.0e-10
+            b000sum0 = 0.0
+            nstride = n_coeff
+            if not self.config.sections['BISPECTRUM'].bikflag:
+                if not self.config.sections["BISPECTRUM"].bzeroflag:
+                    b000sum0 = 1.0
+                if self.config.sections["BISPECTRUM"].chemflag:
+                    nstride //= num_types*num_types*num_types
+                    if self.config.sections["BISPECTRUM"].wselfallflag:
+                        b000sum0 *= num_types*num_types*num_types
+                b000sum = sum(b_sum_temp[0, ::nstride])
+                if abs(b000sum - b000sum0) < EPS:
+                    print("WARNING: Configuration has no SNAP neighbors")
+
+            if not self.config.sections["BISPECTRUM"].bzeroflag:
+                if self.config.sections['BISPECTRUM'].bikflag:
+                    raise NotImplementedError("per atom energy is not implemented without bzeroflag")
+                b_sum_temp.shape = (num_types, n_coeff)
+                onehot_atoms = np.zeros((num_types, 1))
+                for atom in self._data["AtomTypes"]:
+                    onehot_atoms[self.config.sections["BISPECTRUM"].type_mapping[atom]-1] += 1
+                onehot_atoms /= len(self._data["AtomTypes"])
+                b_sum_temp = np.concatenate((onehot_atoms, b_sum_temp), axis=1)
+                b_sum_temp.shape = (num_types * n_coeff + num_types)
+
+            # Get matrix of descriptors (A).
+            a[irow:irow+bik_rows] = b_sum_temp * self.config.sections["BISPECTRUM"].blank2J[np.newaxis, :]
+
+            # Get vector of truths (b).
+            ref_energy = lmp_snap[irow, icolref]
+            b[irow:irow+bik_rows] = 0.0
+            b[irow] = (energy - ref_energy) / num_atoms
+
+            # Get weights (w).
+            w[irow] = self._data["eweight"] if "eweight" in self._data else 1.0
+
+            index += nrows_energy
+            dindex += nrows_energy
+        irow += nrows_energy
+
+        if self.config.sections["CALCULATOR"].force:
+            db_atom_temp = lmp_snap[irow:irow + nrows_force, :ncols_bispectrum]
+            db_atom_temp.shape = (num_atoms * ndim_force, n_coeff * num_types)
+            if not self.config.sections["BISPECTRUM"].bzeroflag:
+                db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types, n_coeff)
+                onehot_atoms = np.zeros((np.shape(db_atom_temp)[0], num_types, 1))
+                db_atom_temp = np.concatenate([onehot_atoms, db_atom_temp], axis=2)
+                db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types * n_coeff + num_types)
+            # Get matrix of descriptor derivatives (A).
+            a[irow:irow+nrows_force] = np.matmul(db_atom_temp, np.diag(self.config.sections["BISPECTRUM"].blank2J)) 
+            
+            # Get vector of true forces (b).
+            ref_forces = lmp_snap[irow:irow + nrows_force, icolref]
+            b[irow:irow+nrows_force] = self._data["Forces"].ravel() - ref_forces
+            
+            # Get vector of force weights (w).
+            w[irow:irow+nrows_force] = self._data["fweight"] if "fweight" in self._data else 1.0
+
+            index += nrows_force
+            dindex += nrows_force
+        irow += nrows_force
+
+        if self.config.sections["CALCULATOR"].stress:
+            vb_sum_temp = 1.6021765e6*lmp_snap[irow:irow + nrows_virial, :ncols_bispectrum] / lmp_volume
+            vb_sum_temp.shape = (ndim_virial, n_coeff * num_types)
+            if not self.config.sections["BISPECTRUM"].bzeroflag:
+                vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types, n_coeff)
+                onehot_atoms = np.zeros((np.shape(vb_sum_temp)[0], num_types, 1))
+                vb_sum_temp = np.concatenate([onehot_atoms, vb_sum_temp], axis=2)
+                vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types * n_coeff + num_types)
+            
+            # Get matrix of descriptor virials (A).
+            a[irow:irow+ndim_virial] = np.matmul(vb_sum_temp, np.diag(self.config.sections["BISPECTRUM"].blank2J))
+
+            # Get vector of true stresses (b).
+            ref_stress = lmp_snap[irow:irow + nrows_virial, icolref]
+            b[irow:irow+ndim_virial] = self._data["Stress"][[0, 1, 2, 1, 0, 0], [0, 1, 2, 2, 2, 1]].ravel() - ref_stress
+
+            # Get stress weights (w).
+            w[irow:irow+ndim_virial] = self._data["vweight"] if "vweight" in self._data else 1.0
+
+            index += ndim_virial
+            dindex += ndim_virial
+
+        self.shared_index = index
+        self.distributed_index = dindex
+
+        return a,b,w
+
     def _collect_lammps(self):
 
         num_atoms = self._data["NumAtoms"]
         num_types = self.config.sections['BISPECTRUM'].numtypes
         n_coeff = self.config.sections['BISPECTRUM'].ncoeff
         energy = self._data["Energy"]
 
@@ -295,22 +459,29 @@
                 onehot_atoms = np.zeros((num_types, 1))
                 for atom in self._data["AtomTypes"]:
                     onehot_atoms[self.config.sections["BISPECTRUM"].type_mapping[atom]-1] += 1
                 onehot_atoms /= len(self._data["AtomTypes"])
                 b_sum_temp = np.concatenate((onehot_atoms, b_sum_temp), axis=1)
                 b_sum_temp.shape = (num_types * n_coeff + num_types)
 
+            # Get matrix of descriptors (A).
             self.pt.shared_arrays['a'].array[index:index+bik_rows] = \
                 b_sum_temp * self.config.sections["BISPECTRUM"].blank2J[np.newaxis, :]
+            
             ref_energy = lmp_snap[irow, icolref]
+
+            # Get vector of truths (b).
             self.pt.shared_arrays['b'].array[index:index+bik_rows] = 0.0
             self.pt.shared_arrays['b'].array[index] = (energy - ref_energy) / num_atoms
+
+            # Get weights (w).
             self.pt.shared_arrays['w'].array[index] = self._data["eweight"]
             self.pt.fitsnap_dict['Row_Type'][dindex:dindex + bik_rows] = ['Energy'] * nrows_energy
             self.pt.fitsnap_dict['Atom_I'][dindex:dindex + bik_rows] = [int(i) for i in range(nrows_energy)]
+
             # create an atom types list for the energy rows, if bikflag=1
             if self.config.sections['BISPECTRUM'].bikflag:
                 types_energy = [int(i) for i in lmp_types]
                 self.pt.fitsnap_dict['Atom_Type'][dindex:dindex + bik_rows] = types_energy
             else:
                 self.pt.fitsnap_dict['Atom_Type'][dindex:dindex + bik_rows] = [0]
 
@@ -322,21 +493,27 @@
             db_atom_temp = lmp_snap[irow:irow + nrows_force, :ncols_bispectrum]
             db_atom_temp.shape = (num_atoms * ndim_force, n_coeff * num_types)
             if not self.config.sections["BISPECTRUM"].bzeroflag:
                 db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types, n_coeff)
                 onehot_atoms = np.zeros((np.shape(db_atom_temp)[0], num_types, 1))
                 db_atom_temp = np.concatenate([onehot_atoms, db_atom_temp], axis=2)
                 db_atom_temp.shape = (np.shape(db_atom_temp)[0], num_types * n_coeff + num_types)
+            # Get matrix of descriptor derivatives (A).
             self.pt.shared_arrays['a'].array[index:index+nrows_force] = \
                 np.matmul(db_atom_temp, np.diag(self.config.sections["BISPECTRUM"].blank2J))
+            
             ref_forces = lmp_snap[irow:irow + nrows_force, icolref]
+            # Get vector of true forces (b).
             self.pt.shared_arrays['b'].array[index:index+nrows_force] = \
                 self._data["Forces"].ravel() - ref_forces
+            
+            # Get vector of force weights (w).
             self.pt.shared_arrays['w'].array[index:index+nrows_force] = \
                 self._data["fweight"]
+            # Populate dictionaries.
             self.pt.fitsnap_dict['Row_Type'][dindex:dindex + nrows_force] = ['Force'] * nrows_force
             self.pt.fitsnap_dict['Atom_I'][dindex:dindex + nrows_force] = [int(np.floor(i/3)) for i in range(nrows_force)]
             # create a types list for the force rows
             types_force = [] 
             for typ in lmp_types:
                 for a in range(0,3):
                     types_force.append(typ)
@@ -349,21 +526,26 @@
             vb_sum_temp = 1.6021765e6*lmp_snap[irow:irow + nrows_virial, :ncols_bispectrum] / lmp_volume
             vb_sum_temp.shape = (ndim_virial, n_coeff * num_types)
             if not self.config.sections["BISPECTRUM"].bzeroflag:
                 vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types, n_coeff)
                 onehot_atoms = np.zeros((np.shape(vb_sum_temp)[0], num_types, 1))
                 vb_sum_temp = np.concatenate([onehot_atoms, vb_sum_temp], axis=2)
                 vb_sum_temp.shape = (np.shape(vb_sum_temp)[0], num_types * n_coeff + num_types)
+            
+            # Get matrix of descriptor virials (A).
             self.pt.shared_arrays['a'].array[index:index+ndim_virial] = \
                 np.matmul(vb_sum_temp, np.diag(self.config.sections["BISPECTRUM"].blank2J))
             ref_stress = lmp_snap[irow:irow + nrows_virial, icolref]
+            # Get vector of true stresses (b).
             self.pt.shared_arrays['b'].array[index:index+ndim_virial] = \
                 self._data["Stress"][[0, 1, 2, 1, 0, 0], [0, 1, 2, 2, 2, 1]].ravel() - ref_stress
+            # Get stress weights (w).
             self.pt.shared_arrays['w'].array[index:index+ndim_virial] = \
                 self._data["vweight"]
+            # Populate dictionaries.
             self.pt.fitsnap_dict['Row_Type'][dindex:dindex + ndim_virial] = ['Stress'] * ndim_virial
             self.pt.fitsnap_dict['Atom_I'][dindex:dindex + ndim_virial] = [int(0)] * ndim_virial
             self.pt.fitsnap_dict['Atom_Type'][dindex:dindex + ndim_virial] = [int(0)] * ndim_virial
             index += ndim_virial
             dindex += ndim_virial
 
         length = dindex - self.distributed_index
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/initialize.py` & `fitsnap3-3.1.0.1/fitsnap3lib/initialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,48 +58,51 @@
         from fitsnap3lib.io.input import Config
         config = Config()
         if (pt._rank==0):
             print(f"Hash: {config.hash}")
         pt.single_print("Finished reading input")
         pt.single_print("------------------")
 
-        from fitsnap3lib.io.input import output
+        #from fitsnap3lib.io.input import output
     except Exception as e:
         pt.single_print("Trouble reading input, exiting...")
         pt.exception(e)
 
     try:
-        output.screen("mpi4py version: ", mpi4py.__version__)
+        pt.single_print("mpi4py version: ", mpi4py.__version__)
 
     except NameError:
         print("No mpi4py detected, using fitsnap stubs...")
 
     try:
         import numpy as np
-        output.screen("numpy version: ", np.__version__)
+        #output.screen("numpy version: ", np.__version__)
+        pt.single_print
     except Exception as e:
-        output.screen("Trouble importing numpy package, exiting...")
-        output.exception(e)
+        #output.screen("Trouble importing numpy package, exiting...")
+        #output.exception(e)
+        pt.single_print("Trouble importing numpy package, exiting...")
+        pt.single_print(f"{e}")
 
     try:
         import scipy as sp
-        output.screen("scipy version: ", sp.__version__)
+        pt.single_print("scipy version: ", sp.__version__)
     except Exception as e:
-        output.screen("Trouble importing scipy package, exiting...")
-        output.exception(e)
+        pt.single_print("Trouble importing scipy package, exiting...")
+        pt.single_print(e)
 
     try:
         import pandas as pd
-        output.screen("pandas version: ", pd.__version__)
+        pt.single_print("pandas version: ", pd.__version__)
     except Exception as e:
-        output.screen("Trouble importing pandas package, exiting...")
-        output.exception(e)
+        pt.single_print("Trouble importing pandas package, exiting...")
+        pt.single_print(e)
 
     try:
         import lammps
         lmp = lammps.lammps()
         #print("LAMMPS version: ",lammps.__version__)
         pt.lammps_version = lammps.__version__
     except Exception as e:
         print("Trouble importing LAMMPS library, exiting...")
         raise e
-    output.screen("-----------")
+    pt.single_print("-----------")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/input.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/input.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 import configparser
 import argparse
 import sys
 from pickle import HIGHEST_PROTOCOL
 from fitsnap3lib.io.sections.section_factory import new_section
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.parallel_output import Output
 from pathlib import Path
 import random
 
 
-output = Output()
-#pt = ParallelTools()
-
-
-class Singleton(type):
-    _instances = {}
-
-    def __call__(cls, *args, **kwargs):
-        if (
-                kwargs is not None
-                and "arguments_lst" in kwargs.keys()
-                and kwargs["arguments_lst"] is not None
-        ):
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        return cls._instances[cls]
-
-
-class Config(metaclass=Singleton):
+class Config():
     """ 
     Class for storing input settings in a `config` instance. The `config` instance is first created 
-    in `io/output.py`.
+    in `io/output.py`. If given a path to an input script, we use Python's native ConfigParser 
+    to parse the settings. If given a nested dictionary, the sections are determined from the 
+    first keys and specific settings from the nested keys.
+
+    Args:
+        pt: A ParallelTools instance.
+        input: Optional input can either be a filename or a dictionary.
+        arguments_lst: List of args that can be supplied at the command line.
 
     Attributes:
-        parse_cmdline (list): List of args that can be supplied at the command line, must include a 
-            string to the location of the FitSNAP input script .
+        infile: String for optional input filename. Defaults to None.
+        indict: Dictionary for optional input dictionary of settings, to replace input file. Defaults 
+            to None.
+        
     """
 
-    def __init__(self, arguments_lst=None):
-        self.pt = ParallelTools()
+    def __init__(self, pt, input: (str | dict) = None, arguments_lst: list = None):
+        self.pt = pt
+        self.input = input
+        # Input file (infile) and dictionary (indict) set to None by default and get set in 
+        # parse_config.
+        self.infile = None
+        self.indict = None
         self.default_protocol = HIGHEST_PROTOCOL
         self.args = None
         self.parse_cmdline(arguments_lst=arguments_lst)
         self.sections = {}
         self.parse_config()
 
-        # Generate random 128 bit hash to identify this fit
-
+        # Generate random 128 bit hash to identify this fit on rank 0.
         if self.pt._rank == 0:
             self.hash = f"{random.getrandbits(128):032x}"
+        else:
+            self.hash = None
 
     def parse_cmdline(self, arguments_lst=None):
+        """ Parse command line args. """
         parser = argparse.ArgumentParser(prog="fitsnap3")
-
-        parser.add_argument("infile", action="store",
-                            help="Input file with bispectrum etc. options")
+        if (self.input is None):
+            parser.add_argument("infile", action="store",
+                                help="Input file with bispectrum etc. options")
 
         # Optional args.
         parser.add_argument("--lammpslog", "-l", action="store_true", dest="lammpslog",
                             help="Write logs from LAMMPS. Logs will appear in current working directory.")
         parser.add_argument("--nofit", "-nf", action="store_false", dest="perform_fit",
                             help="Don't perform fit, just compute bispectrum data.")
         parser.add_argument("--overwrite", action="store_true", dest="overwrite",
@@ -84,15 +79,14 @@
                             help="Print fitsnap output to each nodes screen.")
         parser.add_argument("--pscreen", "-ps", action="store_true", dest="pscreen",
                             help="Print fitsnap output to each processors screen.")
         parser.add_argument("--log", action="store", dest="log",
                             default=None, help="Write fitsnap log to this file.")
         parser.add_argument("--screen2file", "-s2f", action="store", dest="screen2file",
                             default=None, help="Print screen to a file")
-
         # Not Implemented.
         """
         parser.add_argument("--lammps_noexceptions", action="store_true",
                             help="Allow LAMMPS compiled without C++ exceptions handling enabled")
         parser.add_argument("--printlammps", "-pl", action="store_true", dest="printlammps",
                             help="Print all lammps commands")
         """
@@ -104,33 +98,56 @@
                 # We're building docs in this case.
                 arguments_lst = arguments_lst=["../examples/Ta_Linear_JCP2014/Ta-example-nodump.in", "--overwrite"]
         self.args = parser.parse_args(arguments_lst)
 
     def parse_config(self):
         tmp_config = configparser.ConfigParser(inline_comment_prefixes='#')
         tmp_config.optionxform = str
-        if not Path(self.args.infile).is_file():
-            raise FileNotFoundError("Input file not found")
-        tmp_config.read(self.args.infile)
-        infile_folder = str(Path(self.args.infile).parent.absolute())
-        file_name = self.args.infile.split('/')[-1]
-        if not Path(infile_folder+'/'+file_name).is_file():
-            raise RuntimeError("Input file {} not found in {}", file_name, infile_folder)
-
-        vprint = output.screen if self.args.verbose else lambda *arguments, **kwargs: None
-        if self.args.keyword_replacements:
-            for kwg, kwn, kwv in self.args.keyword_replacements:
-                if kwg not in tmp_config:
-                    raise ValueError(f"{kwg} is not a valid keyword group")
-                vprint(f"Substituting {kwg}:{kwn}={kwv}")
-                tmp_config[kwg][kwn] = kwv
+        if self.input is not None:
+            if (isinstance(self.input, str)):
+                self.infile = self.input
+            elif (isinstance(self.input, dict)):
+                self.indict = self.input
+        else:
+            if not Path(self.args.infile).is_file():
+                raise FileNotFoundError("Input file not found")
+            self.infile = self.args.infile
+
+        if (self.infile is not None):
+            # We have an input file.
+            tmp_config.read(self.infile)
+            infile_folder = str(Path(self.infile).parent.absolute())
+            file_name = self.infile.split('/')[-1]
+            if not Path(infile_folder+'/'+file_name).is_file():
+                raise RuntimeError("Input file {} not found in {}", file_name, infile_folder)
+
+            #vprint = output.screen if self.args.verbose else lambda *arguments, **kwargs: None
+            # This adds keyword replacements to the config.
+            if self.args.keyword_replacements:
+                for kwg, kwn, kwv in self.args.keyword_replacements:
+                    if kwg not in tmp_config:
+                        raise ValueError(f"{kwg} is not a valid keyword group")
+                    tmp_config[kwg][kwn] = kwv
+
+        elif (self.indict is not None):
+            # We have an input dictionary  instead of a file.
+            for key1, data1 in self.indict.items():
+                tmp_config[key1] = {}
+                for key2, data2 in data1.items():
+                    tmp_config[key1]["{}".format(key2)] = str(data2)
+            # Default missing sections to empty dicts which will prompt default values.
+            names = ["ESHIFT", "EXTRAS", "GROUPS", "MEMORY"]
+            for name in names:
+                if name not in tmp_config:
+                    tmp_config[name] = {}
 
+        # Make sections based on input settings.
         self.set_sections(tmp_config)
 
     def set_sections(self, tmp_config):
         sections = tmp_config.sections()
         for section in sections:
             if section == "TEMPLATE":
                 section = "DEFAULT"
             if section == "BASIC_CALCULATOR":
                 section = "BASIC"
-            self.sections[section] = new_section(section, tmp_config, self.args)
+            self.sections[section] = new_section(section, tmp_config, self.pt, self.infile, self.args)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/custom.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/custom.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from fitsnap3lib.io.outputs.outputs import Output, optional_open
-from fitsnap3lib.parallel_tools import ParallelTools
 from datetime import datetime
-from fitsnap3lib.io.input import Config
 import numpy as np
 import random
 import tarfile
 
 
 #config = Config()
 #pt = ParallelTools()
 
 
 class Custom(Output):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.config = Config()
-        self.pt = ParallelTools()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
+        #self.config = Config()
+        #self.pt = ParallelTools()
 
     def output(self, coeffs, errors):
         self.write_nn(errors)
 
     #@pt.rank_zero
     def write(self, coeffs, errors):
         @self.pt.rank_zero
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/output_factory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/output_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 from fitsnap3lib.io.outputs.pace import Pace
 from fitsnap3lib.io.outputs.snap import Snap
 from fitsnap3lib.io.outputs.custom import Custom
 
 
 #pt = ParallelTools()
 
+def output(output_name, pt, cfg):
+    """Output Factory"""
+    instance = search(output_name)
+    instance.__init__(output_name, pt, cfg)
+    return instance
+
 
 def output_factory(output_name):
     """Output Factory"""
     instance = search(output_name)
     instance.__init__(output_name)
     return instance
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/outputs.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from fitsnap3lib.io.input import Config
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.io.input import Config
+#from fitsnap3lib.parallel_tools import ParallelTools
 from contextlib import contextmanager
 import gzip
 from datetime import datetime
 import logging
 
 
 #config = Config()
 #pt = ParallelTools()
 
 
 class Output:
 
-    def __init__(self, name):
-        self.config = Config()
-        self.pt = ParallelTools()
+    def __init__(self, name, pt, config):
+        self.config = config #Config()
+        self.pt = pt #ParallelTools()
         self.name = name
         self._screen = self.config.args.screen
         self._pscreen = self.config.args.pscreen
         self._nscreen = self.config.args.nscreen
         self._logfile = self.config.args.log
         self._s2f = self.config.args.screen2file
         self._tarball = self.config.args.tarball
@@ -64,14 +64,18 @@
         # if '{}'.format(err) == 'MPI_ERR_INTERN: internal error':
         #     # Known Issues: Allocating too much memory
         #     self.screen("Attempting to handle MPI error gracefully.\nAborting MPI...")
         #     pt.abort()
 
     def output(self, *args):
         pass
+    
+    def write_lammps(self, *args):
+        """Parent class function for writing LAMMPS-ready potential files."""
+        pass
 
     #@pt.rank_zero
     def write_errors(self, errors):
         @self.pt.rank_zero
         def decorated_write_errors():
             fname = self.config.sections["OUTFILE"].metric_file
             arguments = {}
@@ -97,23 +101,26 @@
                 write_type = 'wb'
             else:
                 raise NotImplementedError("Metric style {} not implemented".format(
                     self.config.sections["OUTFILE"].metrics_style))
             with optional_open(fname, write_type) as file:
                 function(file, **arguments)
 
+        # Don't write errors if using scalapack.
         if not self.config.sections["SOLVER"].true_multinode: 
-            decorated_write_errors()
+            # Don't write errors if `errors` is a list (default is empty list).
+            if type(errors) != type([]):
+                decorated_write_errors()
 
     def write_errors_nn(self, errors):
         """ 
         Write errors for nonlinear fits. 
         
         Args:
-            errors : sequence of dictionaries (mae_f, mae_e, rmse_e, rmse_f, count_train, count_test)
+            errors : sequence of dictionaries (mae_f, mae_e, rmse_f, rmse_e, count_train, count_test)
         """
         @self.pt.rank_zero
         def decorated_write_errors_nn():
             mae_f = errors[0]
             mae_e = errors[1]
             rmse_f = errors[2]
             rmse_e = errors[3]
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/pace.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/pace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,65 @@
 from fitsnap3lib.io.outputs.outputs import Output, optional_open
-from fitsnap3lib.parallel_tools import ParallelTools
 from datetime import datetime
-from fitsnap3lib.io.input import Config
 import numpy as np
 import itertools
 
 #config = Config()
 #pt = ParallelTools()
 
 try:
 
     from fitsnap3lib.lib.sym_ACE.yamlpace_tools.potential import AcePot
 
     class Pace(Output):
 
-        def __init__(self, name):
-            super().__init__(name)
-            self.config = Config()
-            self.pt = ParallelTools()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
+            #self.config = Config()
+            #self.pt = ParallelTools()
 
         def output(self, coeffs, errors):
             if (self.config.sections["CALCULATOR"].nonlinear):
                 self.write_nn(errors)
             else:
                 new_coeffs = None
                 # new_coeffs = pt.combine_coeffs(coeffs)
                 if new_coeffs is not None:
                     coeffs = new_coeffs
                 self.write(coeffs, errors)
 
+        def write_lammps(self, coeffs):
+            """
+            Write LAMMPS ready ACE files.
+
+            Args:
+                coeffs: list of linear model coefficients.
+            """
+            if self.config.sections["EXTRAS"].only_test != 1:
+                if self.config.sections["CALCULATOR"].calculator != "LAMMPSPACE":
+                    raise TypeError("PACE output style must be paired with LAMMPSPACE calculator")
+                with optional_open(self.config.sections["OUTFILE"].potential_name and
+                                  self.config.sections["OUTFILE"].potential_name + '.acecoeff', 'wt') as file:
+                    file.write(_to_coeff_string(coeffs, self.config))
+                self.write_potential(coeffs)
+
         #@pt.rank_zero
         def write(self, coeffs, errors):
             @self.pt.rank_zero
             def decorated_write():
+                """
                 if self.config.sections["EXTRAS"].only_test != 1:
                     if self.config.sections["CALCULATOR"].calculator != "LAMMPSPACE":
                         raise TypeError("PACE output style must be paired with LAMMPSPACE calculator")
                     with optional_open(self.config.sections["OUTFILE"].potential_name and
                                       self.config.sections["OUTFILE"].potential_name + '.acecoeff', 'wt') as file:
-                        file.write(_to_coeff_string(coeffs))
+                        file.write(_to_coeff_string(coeffs, self.config))
                     self.write_potential(coeffs)
+                """
+                self.write_lammps(coeffs)
                 self.write_errors(errors)
             decorated_write()
 
         def write_nn(self, errors):
             """ 
             Write output for nonlinear fits. 
             
@@ -125,19 +141,19 @@
         """
         Dummy class for factory to read if torch is not available for import.
         """
         def __init__(self, name):
             super().__init__(name)
             raise ModuleNotFoundError("Missing sympy or pyyaml modules.")
 
-def _to_coeff_string(coeffs):
+def _to_coeff_string(coeffs, config):
     """
-    Convert a set of coefficients along with bispec options into a .snapparam file
+    Convert a set of coefficients along with descriptor options to a coeffs file.
     """
-    config = Config()
+
     desc_str = "ACE"
     coeffs = coeffs.reshape((config.sections[desc_str].numtypes, -1))
     blank2Js = config.sections[desc_str].blank2J.reshape((config.sections[desc_str].numtypes, -1))
     if config.sections[desc_str].bzeroflag:
         blank2Js = np.insert(blank2Js, 0, [1.0], axis=1)
     coeffs = np.multiply(coeffs, blank2Js)
     coeff_names = [[0]]+config.sections[desc_str].blist
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/outputs/snap.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/outputs/snap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 from fitsnap3lib.io.outputs.outputs import Output, optional_open
-from fitsnap3lib.parallel_tools import ParallelTools
 from datetime import datetime
-from fitsnap3lib.io.input import Config
 import numpy as np
 import random
 import tarfile
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 class Snap(Output):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.config = Config()
-        self.pt = ParallelTools()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
     def output(self, coeffs, errors):
         if (self.config.sections["CALCULATOR"].nonlinear):
             # Currently coeffs and errors are empty for nonlinear.
             # TODO: Add nonlinear error calculation for output here, similar format as linear.
             self.write_nn(errors)
         else:
             new_coeffs = None
             # new_coeffs = pt.combine_coeffs(coeffs)
             if new_coeffs is not None:
                 coeffs = new_coeffs
             self.write(coeffs, errors)
 
+    def write_lammps(self, coeffs):
+        """
+        Write LAMMPS-ready SNAP files.
+        
+        Args:
+            coeffs: list of linear model coefficients.
+        """
+        if self.config.sections["EXTRAS"].only_test != 1:
+            if self.config.sections["CALCULATOR"].calculator != "LAMMPSSNAP":
+                raise TypeError("SNAP output style must be paired with LAMMPSSNAP calculator")
+        with optional_open(self.config.sections["OUTFILE"].potential_name and
+                            self.config.sections["OUTFILE"].potential_name + '.snapcoeff', 'wt') as file:
+            file.write(_to_coeff_string(self.config, coeffs))
+        with optional_open(self.config.sections["OUTFILE"].potential_name and
+                            self.config.sections["OUTFILE"].potential_name + '.snapparam', 'wt') as file:
+            file.write(_to_param_string(self.config))
+        with optional_open(self.config.sections["OUTFILE"].potential_name and
+                            self.config.sections["OUTFILE"].potential_name + '.mod', 'wt') as file:
+            file.write(_to_potential_file(self.config))
+        if (self._tarball):
+            with optional_open("in.lammps", 'wt') as file:
+                file.write(_to_lammps_input())
+            # Package these files into a tarball
+            fp = tarfile.open(f"fit-{self.config.hash}.tar.gz", 'w:gz')
+            potname = self.config.sections["OUTFILE"].potential_name
+            potname_prefix = potname.split('/')[-1]
+            fp.add(potname + '.snapcoeff', arcname = potname_prefix + '.snapcoeff')
+            fp.add(potname + '.snapparam', arcname = potname_prefix + '.snapparam')
+            fp.add(potname + '.mod', arcname = potname_prefix)
+            fp.add("in.lammps")
+            fp.close()
+
     #@pt.rank_zero
     def write(self, coeffs, errors):
+        """ Write both LAMMPS files and error files"""
         @self.pt.rank_zero
         def decorated_write():
-            if self.config.sections["EXTRAS"].only_test != 1:
-                if self.config.sections["CALCULATOR"].calculator != "LAMMPSSNAP":
-                    raise TypeError("SNAP output style must be paired with LAMMPSSNAP calculator")
-            with optional_open(self.config.sections["OUTFILE"].potential_name and
-                               self.config.sections["OUTFILE"].potential_name + '.snapcoeff', 'wt') as file:
-                file.write(_to_coeff_string(coeffs))
-            with optional_open(self.config.sections["OUTFILE"].potential_name and
-                               self.config.sections["OUTFILE"].potential_name + '.snapparam', 'wt') as file:
-                file.write(_to_param_string())
-            with optional_open(self.config.sections["OUTFILE"].potential_name and
-                               self.config.sections["OUTFILE"].potential_name + '.mod', 'wt') as file:
-                file.write(_to_potential_file())
-            if (self._tarball):
-                with optional_open("in.lammps", 'wt') as file:
-                    file.write(_to_lammps_input())
-                # Package these files into a tarball
-                fp = tarfile.open(f"fit-{self.config.hash}.tar.gz", 'w:gz')
-                potname = self.config.sections["OUTFILE"].potential_name
-                potname_prefix = potname.split('/')[-1]
-                fp.add(potname + '.snapcoeff', arcname = potname_prefix + '.snapcoeff')
-                fp.add(potname + '.snapparam', arcname = potname_prefix + '.snapparam')
-                fp.add(potname + '.mod', arcname = potname_prefix)
-                fp.add("in.lammps")
-                fp.close()
-
+            self.write_lammps(coeffs)
             self.write_errors(errors)
         decorated_write()
 
     def write_nn(self, errors):
         """ 
         Write output for nonlinear fits. 
         
@@ -72,18 +73,18 @@
         @self.pt.rank_zero
         def decorated_write():
             if self.config.sections["EXTRAS"].only_test != 1:
                 if (self.config.sections["CALCULATOR"].calculator != "LAMMPSSNAP"):
                     raise TypeError("SNAP output style must be paired with LAMMPSSNAP calculator")
             with optional_open(self.config.sections["OUTFILE"].potential_name and
                                self.config.sections["OUTFILE"].potential_name + '.mliap.descriptor', 'wt') as file:
-                file.write(_to_mliap_string())
+                file.write(_to_mliap_string(self.config))
             with optional_open(self.config.sections["OUTFILE"].potential_name and
                                self.config.sections["OUTFILE"].potential_name + '.mod', 'wt') as file:
-                file.write(_to_mliap_mod())
+                file.write(_to_mliap_mod(self.config))
 
             self.write_errors_nn(errors)
         decorated_write()
 
     #@pt.sub_rank_zero
     def read_fit(self):
         @self.pt.sub_rank_zero
@@ -114,16 +115,15 @@
                     for j in range(ncoeff-1):
                         fit[i][j] = float(file.readline().split()[0])
             return fit
         fit = decorated_read_fit()
         return fit.flatten()
 
 
-def _to_param_string():
-    config = Config()
+def _to_param_string(config):
     if config.sections["BISPECTRUM"].chemflag != 0:
         chemflag_int = 1
     else:
         chemflag_int = 0
     # Report reference section settings
     unit = f"# units {config.sections['REFERENCE'].units}\n"
     atom = f"# atom_style {config.sections['REFERENCE'].atom_style}\n"
@@ -149,19 +149,18 @@
     out += "# This file was generated by FitSNAP.\n"
     out += f"# Hash: {config.hash}\n"
     out += "# FitSNAP REFERENCE section settings:\n"
     out += f"{refsec}"
 
     return out
 
-def _to_coeff_string(coeffs):
+def _to_coeff_string(config, coeffs):
     """
     Convert a set of coefficients along with bispec options into a .snapparam file
     """
-    config = Config()
 
     numtypes = config.sections["BISPECTRUM"].numtypes
     ncoeff = config.sections["BISPECTRUM"].ncoeff
     coeffs = coeffs.reshape((numtypes, -1))
     blank2Js = config.sections["BISPECTRUM"].blank2J.reshape((numtypes, -1))
     if config.sections["BISPECTRUM"].bzeroflag:
         blank2Js = np.insert(blank2Js, 0, [1.0], axis=1)
@@ -180,19 +179,18 @@
 
         out += "{} {} {}\n".format(elname, rjval, wjval)
         out += "\n".join(f" {bval:<30.18} #  B{bname} " for bval, bname in zip(column, bnames))
         out += "\n"
     out += "\n# End of potential"
     return out
 
-def _to_potential_file():
+def _to_potential_file(config):
     """
     Use config settings to write a LAMMPS potential .mod file.
     """
-    config = Config()
 
     ps = config.sections["REFERENCE"].lmp_pairdecl[0]
     snap_filename = config.sections["OUTFILE"].potential_name.split("/")[-1]
 
     out = "# This file was generated by FitSNAP.\n"
     out += f"# Hash: {config.hash}\n\n"
 
@@ -217,21 +215,19 @@
         pc_snap = f"pair_coeff * * {snap_filename}.snapcoeff {snap_filename}.snapparam"
         for t in config.sections["BISPECTRUM"].types:
             pc_snap += f" {t}"
         out += pc_snap
 
     return out
 
-def _to_lammps_input():
+def _to_lammps_input(config):
     """
     Use config settings to write a LAMMPS input script.
     """
 
-    config = Config()
-
     snap_filename = config.sections["OUTFILE"].potential_name.split("/")[-1]
     pot_filename = snap_filename + ".mod"
 
     out = "# LAMMPS template input written by FitSNAP.\n"
     out += "# Runs a NVE simulation at specified temperature and timestep.\n"
     out += "\n"
     out += "# Declare simulation variables\n"
@@ -259,17 +255,16 @@
     out += "\n"
     out += "# Run dynamics\n"
     out += "\n"
     out += "run 1000\n"
 
     return out
 
-def _to_mliap_string():
+def _to_mliap_string(config):
     """ Build mliap descriptor file. """
-    config = Config()
     out = "# required\n"
     out += f"rcutfac {config.sections['BISPECTRUM'].rcutfac}\n"
     out += f"twojmax {max(config.sections['BISPECTRUM'].twojmax)}\n\n"
     out += "#elements\n"
     out += f"nelems {config.sections['BISPECTRUM'].numtypes}\n"
     out += "elems"
     for t in config.sections['BISPECTRUM'].types:
@@ -299,17 +294,16 @@
     pair = "\n".join(["# " + s for s in config.sections["REFERENCE"].lmp_pairdecl]) + "\n"
     refsec = unit + atom + pair
     out += f"# FitSNAP generated Hash: {config.hash}\n"
     out += "# FitSNAP REFERENCE section settings:\n"
     out += f"{refsec}"
     return out
 
-def _to_mliap_mod():
+def _to_mliap_mod(config):
     """ Build mliap mod file for using the potential. """
-    config = Config()
     ps = config.sections["REFERENCE"].lmp_pairdecl[0]
     snap_filename = config.sections["OUTFILE"].potential_name.split("/")[-1]
 
     out = f"# FitSNAP generated Hash: {config.hash}\n"
 
     if "hybrid" in ps:
         # extract non zero parts of pair style
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/ace.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/ace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import numpy as np
 import itertools
 #from fitsnap3lib.lib.sym_ACE.rpi_lib import *
 #from fitsnap3lib.lib.sym_ACE.yamlpace_tools.potential import  *
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
 
 try:
 
     from fitsnap3lib.lib.sym_ACE.rpi_lib import *
     from fitsnap3lib.lib.sym_ACE.yamlpace_tools.potential import  *
 
     class Ace(Section):
 
-        def __init__(self, name, config, args):
-            super().__init__(name, config, args)
+        def __init__(self, name, config, pt, infile, args):
+            super().__init__(name, config, pt, infile, args)
             
             allowedkeys = ['numTypes', 'ranks', 'lmax', 'nmax', 'mumax', 'nmaxbase', 'rcutfac', 'lambda', 
                           'type', 'bzeroflag', 'erefs', 'rcinner', 'drcinner', 'RPI_heuristic', 'lmin', 
                           'bikflag', 'dgradflag']
             for value_name in config['ACE']:
                 if value_name in allowedkeys: continue
                 else:
@@ -41,18 +40,17 @@
             self.type_mapping = {}
             for i, atom_type in enumerate(self.types):
                 self.type_mapping[atom_type] = i+1
 
             self.bzeroflag = self.get_value("ACE", "bzeroflag", "0", "bool")
             self.wigner_flag = self.get_value("ACE", "wigner_flag", "1", "bool")
 
-            if self.bikflag:
-                self._assert_dependency('bikflag', "CALCULATOR", "per_atom_energy", True)
+            #if self.bikflag:
+            #    self._assert_dependency('bikflag', "CALCULATOR", "per_atom_energy", True)
             self.lmax_dct = {int(rnk):int(lmx) for rnk,lmx in zip(self.ranks,self.lmax)}
-            self.pt = ParallelTools()
             if self.RPI_heuristic != 'root_SO3_span':
                 self.pt.single_print('WARNING: do not change RPI flags unless you know what you are doing!')
             self._generate_b_list()
             self._write_couple()
             Section.num_desc = len(self.blist)
             self.delete()
 
@@ -144,10 +142,10 @@
 
 except ModuleNotFoundError:
 
     class Ace(Section):
         """
         Dummy class for factory to read if torch is not available for import.
         """
-        def __init__(self, name, config, args):
-            super().__init__(name, config, args)
+        def __init__(self, name, config, pt, infile, args):
+            super().__init__(name, config, pt, infile, args)
             raise ModuleNotFoundError("Missing sympy or pyyaml modules.")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/bispectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from fitsnap3lib.io.sections.sections import Section
 from itertools import combinations_with_replacement
 import numpy as np
 
 
 class Bispectrum(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
 
         self.allowedkeys = ['numTypes', 'twojmax', 'rcutfac', 'rfac0', 'rmin0', 'wj', 'radelem', 'type',
                             'wselfallflag', 'chemflag', 'bzeroflag', 'quadraticflag', 'bnormflag', 'bikflag',
                             'switchinnerflag', 'switchflag', 'sinner', 'dinner', 'dgradflag']
         self._check_section()
 
         self._check_if_used("CALCULATOR", "calculator", "LAMMPSSNAP", "LAMMPSSNAP")
@@ -43,16 +43,16 @@
         self.bzeroflag = self.get_value("BISPECTRUM", "bzeroflag", "0", "bool")
         # quadraticflag true enables the quadratic model
         self.quadraticflag = self.get_value("BISPECTRUM", "quadraticflag", "0", "bool")
         if (self.chemflag and self.quadraticflag):
             raise ValueError("Quadratic chemsnap not impelemented.")
         # bikflag true enables computing of bispectrum per atom instead of sum
         self.bikflag = self.get_value("BISPECTRUM", "bikflag", "0", "bool")
-        if self.bikflag:
-            self._assert_dependency('bikflag', "CALCULATOR", "per_atom_energy", True)
+        #if self.bikflag:
+        #    self._assert_dependency('bikflag', "CALCULATOR", "per_atom_energy", True)
         self._generate_b_list()
         self._reset_chemflag()
         Section.num_desc = len(self.blist)
         # switchinnerflag true enables inner cutoff function
         self.switchinnerflag = self.get_value("BISPECTRUM", "switchinnerflag", "0", "bool")
         if (self.switchinnerflag):
             default_sinner = self.numtypes*"0.9 "
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/calculator.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
 #pt = ParallelTools()
 
 
 class Calculator(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
-        self.pt = ParallelTools()
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
+        #self.pt = ParallelTools()
         self.allowedkeys = ['calculator', 'energy', 'per_atom_energy', 'force', 'stress', \
                             'nonlinear', 'per_atom_scalar']
         self._check_section()
 
         self.calculator = self.get_value("CALCULATOR", "calculator", "LAMMPSSNAP")
         self.energy = self.get_value("CALCULATOR", "energy", "True", "bool")
         self.per_atom_energy = self.get_value("CALCULATOR", "per_atom_energy", "False", "bool")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/calculator_sections/custom.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/calculator_sections/custom.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Custom Class"""
 from fitsnap3lib.io.sections.sections import Section
 
 
 class Custom(Section):
 
-    def __init__(self, name, config, args):
+    def __init__(self, name, config, pt, infile, args):
         # let parent hold config and args
-        super().__init__(name, config, args)
+        super().__init__(name, config, pt, infile, args)
         self.num_atoms = self.get_value("CUSTOM", "numAtoms", "1", "int")
         self.numtypes = self.get_value("CUSTOM", "numTypes", "1", "int")
         self.types = self.get_value("CUSTOM", "type", "H").split()
         self.type_mapping = {}
         #print(self.types)
         for i, atom_type in enumerate(self.types):
             self.type_mapping[atom_type] = i+1
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/eshift.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/eshift.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from fitsnap3lib.io.sections.sections import Section
 import numpy as np
-from fitsnap3lib.parallel_tools import ParallelTools
-
-
-pt = ParallelTools()
 
 
 class Eshift(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         types = []
         if config.has_section("BISPECTRUM"):
             self.types = self.get_value("BISPECTRUM", "type", "H").split()
         elif config.has_section("ACE"):
             self.types = self.get_value("ACE", "type", "H").split()
         elif config.has_section("CUSTOM"):
             self.types = self.get_value("CUSTOM", "type", "H").split()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/extras.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/extras.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
 class Extras(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['multinode_testing', 'apply_transpose', 'only_test', \
                             'dump_descriptors', 'dump_truth', 'dump_weights', 'dump_dataframe', \
                             'dump_peratom', 'dump_perconfig', 'dump_configs']
         self._check_section()
 
         # Set EXTRAS section file dump flags.
-
+        
         self.multinode_testing = self.get_value("EXTRAS", "multinode_testing", "0", "bool")
         self.apply_transpose = self.get_value("EXTRAS", "apply_transpose", "0", "bool")
         self.only_test = self.get_value("EXTRAS", "only_test", "0", "bool")
         self.dump_a = self.get_value("EXTRAS", "dump_descriptors", "0", "bool")
         self.dump_b = self.get_value("EXTRAS", "dump_truth", "0", "bool")
         self.dump_w = self.get_value("EXTRAS", "dump_weights", "0", "bool")
         self.dump_dataframe = self.get_value("EXTRAS", "dump_dataframe", "0", "bool")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/groups.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Groups Class"""
 from fitsnap3lib.io.sections.sections import Section
 from pandas import read_csv
 from os import path
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.parallel_output import Output
+#from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_output import Output
 
 
-pt = ParallelTools()
-output = Output()
+#pt = ParallelTools()
+#output = Output()
 
 
 def _str_2_fun(some_list):
     for i, item in enumerate(some_list):
         if item == 'str':
             some_list[i] = str
         if item == 'bool':
@@ -20,16 +20,16 @@
             some_list[i] = int
         if item == 'float':
             some_list[i] = float
 
 
 class Groups(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['group_sections', 'group_types', 'smartweights', 'random_sampling', 'random_seed', 'vasp_use_TOTEN','vasp_json_pathname','vasp_ignore_incomplete','vasp_ignore_jsons','vasp_unconverged_label','BOLTZ']
 
         # for value_name in config['GROUPS']:
         #     if value_name in allowedkeys: continue
         #      else: pt.single_print(">>> Found unmatched variable in GROUPS section of input: ",value_name)
 
         self.group_sections = self.get_value("GROUPS", "group_sections", "name size eweight fweight vweight").split()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/memory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/memory.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from fitsnap3lib.io.sections.sections import Section
 from os import sysconf
 from subprocess import check_output
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
 class Memory(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['memory', 'override']
         self._check_section()
 
         self._check_memory()
         self.memory = self.get_value("MEMORY", "memory", "{}".format(self.mem_bytes), "int")
         self.override = self.get_value("MEMORY", "override", "False", interpreter="bool")
         self.delete()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/outfile.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/outfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from os import path
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
 #pt = ParallelTools()
 
 
 class Outfile(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
-        self.pt = ParallelTools()
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
+        #self.pt = ParallelTools()
         self.allowedkeys = ['output_style',
                             'metrics',
                             'metrics_style',
                             'potential',
                             'detailed_errors']
         self._check_section()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/path.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/path.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from fitsnap3lib.io.sections.sections import Section
 from os import path
-from fitsnap3lib.parallel_tools import ParallelTools
-
-
-pt = ParallelTools()
 
 
 class Path(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['dataPath', 'groupFile']
         self._check_section()
 
+        # Set infile directory if we have an infile (as opposed to an indict):
+
         self.infile_directory = Section.get_infile_directory(self)
         self.outfile_directory = Section.get_outfile_directory(self)
         self.datapath = path.join(self.infile_directory, self.get_value("PATH", "dataPath", "JSON"))
         self.group_file = path.join(self.infile_directory, self.get_value("PATH", "groupFile", "grouplist.in"))
         self.delete()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/reference.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/reference.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
 class Reference(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['units', 'atom_style', 'pair_style', 'pair_coeff']
 
         # for value_name in config['REFERENCE']:
         #     if value_name in allowedkeys: continue
         #     else: pt.single_print(">>> Found unmatched variable in REFERENCE section of input: ",value_name)
 
         self.units = self.get_value("REFERENCE", "units", "metal").lower()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/scraper.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.parallel_output import Output
+#from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_output import Output
 
 
-pt = ParallelTools()
-output = Output()
+#pt = ParallelTools()
+#output = Output()
 
 
 class Scraper(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt,infile, args):
+        super().__init__(name, config, pt, infile,args)
         self.allowedkeys = ['scraper', 'save_group_scrape', 'read_group_scrape', 'property_array']
         self._check_section()
 
         self.scraper = self.get_value("SCRAPER", "scraper", "JSON")
         self.save_group_scrape = self.get_value("SCRAPER", "save_group_scrape", "None", "str")
         self.read_group_scrape = self.get_value("SCRAPER", "read_group_scrape", "None", "str")
         self.properties = {"Stress": ["pressure", "Metal", "Metal"],
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/section_factory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/section_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,22 @@
 from fitsnap3lib.io.sections.solver_sections.ridge import Ridge
 from fitsnap3lib.io.sections.solver_sections.jax import JAX
 from fitsnap3lib.io.sections.solver_sections.pytorch import PYTORCH
 from fitsnap3lib.io.sections.solver_sections.network import NETWORK
 from fitsnap3lib.io.sections.template import Default
 
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
-def new_section(section, config, args):
+def new_section(section, config, pt, infile, args):
     """Section Factory"""
     instance = search(section)
     try:
-        instance.__init__(section, config, args)
+        instance.__init__(section, config, pt, infile, args)
     except ExitFunc:
         pass
     return instance
 
 
 def search(section):
     instance = None
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/sections.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/sections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.parallel_output import Output
 from fitsnap3lib.io.error import ExitFunc
 from distutils.util import strtobool
 from os import getcwd, path
 
 
-pt = ParallelTools()
-output = Output()
-
-
 class Section:
     parameters = []
     _infile_directory = None
     _outfile_directory = None
     sections = {}
     dependencies = {}
     num_desc = 0
 
-    def __init__(self, name, config, args=None):
+    def __init__(self, name, config, pt, infile, args=None):
         self.name = name
+        self.pt = pt
+        self.infile = infile
         Section.sections[name] = self
         self._config = config
         self._args = args
         self.allowedkeys = None
         try:
             on = self._on
         except AttributeError:
@@ -43,15 +39,15 @@
             if value_name in self.allowedkeys:
                 continue
             else:
                 raise RuntimeError(">>> Found unmatched variable in {} section of input: {}".format(self.name,
                                                                                                     value_name))
 
     def print_name(self):
-        output.screen(self.name)
+        self.pt.single_print(self.name)
 
     def get_value(self, section, key, fallback, interpreter="str"):
         if self._args == "verbose" and section.lower() == self.name.lower():
             Section.add_parameter(section, key, fallback, interpreter)
         if interpreter == "str" or interpreter == "string":
             convert = str
         elif interpreter == "bool":
@@ -139,20 +135,24 @@
     def get_outfile_directory(cls, self):
         if cls._outfile_directory is None:
             cls._set_outfile_directory(self)
         return cls._outfile_directory
 
     @classmethod
     def _set_infile_directory(cls, self):
-        """ Set path to input file directory """
+        """ 
+        Set path to input file directory.
+        This is the directory that we read input from.
+        If no infile is supplied (i.e. we have indict), then no need for this.
+        """
         cwd = getcwd().split('/')
-        path_to_file = self._args.infile.split('/')[:-1]
+        path_to_file = self.infile.split('/')[:-1] if self.infile else None
         if not path_to_file:
             cls._infile_directory = ''
-        elif not path.isabs(self._args.infile):
+        elif not path.isabs(self.infile):
             cls._infile_directory = '/'.join(path_to_file)
         else:
             count = 0
             while path_to_file[count] == cwd[count]:
                 count += 1
             cwd = (['..'] * (len(cwd)-count)) + path_to_file[count:]
             cls._infile_directory = '/'.join(cwd)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/ard.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/ard.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fitsnap3lib.io.sections.sections import Section
 
 
 class Ard(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['alphabig', 'alphasmall', 'lambdabig', 'lambdasmall', 'threshold_lambda','directmethod','scap','scai','logcut']
         self._check_section()
 
         self._check_if_used("SOLVER", "solver", "SVD")
 
         self.alphabig = self.get_value("ARD", "alphabig", "1.0E-12", "float")
         self.alphasmall = self.get_value("ARD", "alphasmall", "1.0E-14", "float")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/jax.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/jax.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         """
         w_key, b_key = random.split(key)
         return scale * random.normal(w_key, (n, m)), scale * random.normal(b_key, (n,))
 
 
     class JAX(Section):
 
-        def __init__(self, name, config, args):
+        def __init__(self, name, config, pt, infile, args):
             raise Exception("JAX solver not implemented yet.")
             super().__init__(name, config, args)
             self.allowedkeys = ['layer_sizes', 'learning_rate', 'num_epochs', 'batch_size', 'output_style',
                                 'output_file', 'save_state_input', 'opt_state_input', 'opt_state_output']
             self._check_section()
 
             self._check_if_used("SOLVER", "solver", "SVD")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/network.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
-
 try:
     import torch
     from fitsnap3lib.lib.neural_networks.pairwise import create_torch_network    
     from torch.nn import Parameter
 
 
     class NETWORK(Section):
 
-        def __init__(self, name, config, args):
-            super().__init__(name, config, args)
+        def __init__(self, name, config, pt, infile, args):
+            super().__init__(name, config, pt, infile, args)
             self.allowedkeys = ['layer_sizes', 'learning_rate', 'num_epochs', 'batch_size', 'save_state_output',
                                 'save_freq', 'save_state_input', 'output_file', 'energy_weight', 'force_weight',
                                 'training_fraction', 'multi_element_option', 'num_elements', 'manual_seed_flag']
             self._check_section()
 
             self._check_if_used("SOLVER", "solver", "SVD")
 
@@ -37,29 +35,28 @@
             if (self.dtype_setting==1):
                 self.dtype = torch.float32
             else:
                 self.dtype = torch.float64
 
             # catch errors associated with settings, and set necessary flags for later
 
-            self.pt = ParallelTools()
             if (self.energy_weight != self.energy_weight and self.force_weight == self.force_weight):
                 raise Exception("Must use global energy weight with global force weight.")
             elif (self.energy_weight == self.energy_weight and self.force_weight != self.force_weight):
                 raise Exception("Must use global force weight with global energy weight.")
             elif (self.energy_weight == self.energy_weight and self.force_weight == self.force_weight):
-                if (self.pt._rank==0):
+                if (pt._rank==0):
                     print("----- Global weights set: Overriding group weights.")
                 self.global_weight_bool = True
             if (self.training_fraction == self.training_fraction):
-                if (self.pt._rank==0):
+                if (pt._rank==0):
                     print("----- Global training fraction set: Overriding group fractions.")
                 self.global_fraction_bool = True
             if (self.manual_seed_flag):
-                if (self.pt._rank==0):
+                if (pt._rank==0):
                     print("----- manual_seed_flag=1: Setting random seed to 0 for debugging.")
                 torch.manual_seed(0)
             
             self.delete()
             
 except ModuleNotFoundError:
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/pytorch.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from fitsnap3lib.io.sections.sections import Section
-from fitsnap3lib.parallel_tools import ParallelTools
 
 try:
     import torch
     from fitsnap3lib.lib.neural_networks.pytorch import create_torch_network    
     from torch.nn import Parameter
 
 
     class PYTORCH(Section):
 
-        def __init__(self, name, config, args):
-            super().__init__(name, config, args)
+        def __init__(self, name, config, pt, infile, args):
+            super().__init__(name, config, pt, infile, args)
             self.allowedkeys = ['layer_sizes', 'learning_rate', 'num_epochs', 'batch_size', 'save_state_output',
                                 'save_freq', 'save_state_input', 'output_file', 'energy_weight', 'force_weight',
                                 'training_fraction', 'multi_element_option', 'num_elements', 'manual_seed_flag',
                                 'shuffle_flag']
             self._check_section()
 
             self._check_if_used("SOLVER", "solver", "SVD")
@@ -45,15 +44,14 @@
                 self.dtype = torch.float32
             else:
                 self.dtype = torch.float64
             self.shuffle_flag = self.get_value("PYTORCH", "shuffle_flag", "True", "bool")
 
             # catch errors associated with settings, and set necessary flags for later
 
-            self.pt = ParallelTools()
             if (self.energy_weight != self.energy_weight and self.force_weight == self.force_weight):
                 raise Exception("Must use global energy weight with global force weight.")
             elif (self.energy_weight == self.energy_weight and self.force_weight != self.force_weight):
                 raise Exception("Must use global force weight with global energy weight.")
             elif (self.energy_weight == self.energy_weight and self.force_weight == self.force_weight):
                 if (self.pt._rank==0):
                     print("----- Global weights set: Overriding group weights.")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/solver_sections/solver.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/solver_sections/solver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fitsnap3lib.io.sections.sections import Section
 
 
 class Solver(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
         self.allowedkeys = ['solver', 'normalweight', 'normratio', \
                             'compute_testerrs', 'detailed_errors', \
                             'nsam', 'cov_nugget', \
                             'mcmc_num', 'mcmc_gamma', \
                             'merr_mult', 'merr_method', "merr_cfs"]
         self._check_section()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/io/sections/trainshift.py` & `fitsnap3-3.1.0.1/fitsnap3lib/io/sections/trainshift.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from fitsnap3lib.io.sections.sections import Section
 import numpy as np
-from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.parallel_tools import ParallelTools
 
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
 class Trainshift(Section):
 
-    def __init__(self, name, config, args):
-        super().__init__(name, config, args)
+    def __init__(self, name, config, pt, infile, args):
+        super().__init__(name, config, pt, infile, args)
 
         if config.has_section("BISPECTRUM"):
             self.types = self.get_value("BISPECTRUM", "type", "H").split()
         elif config.has_section("ACE"):
             self.types = self.get_value("ACE", "type", "H").split()
         elif config.has_section("CUSTOM"):
             self.types = self.get_value("CUSTOM", "type", "H").split()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/bessel.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/descriptors/g3b.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/jax.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pairwise.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pairwise.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pas.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pas.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/pytorch.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,18 +254,18 @@
         
         #from lammps.mliap.pytorch import IgnoreElems, TorchWrapper, ElemwiseModels
         from fitsnap3lib.lib.neural_networks.write import IgnoreElems, TorchWrapper, ElemwiseModels
 
         # self.network_architecture0 is network model for the first element type
 
         if self.n_elem == 1:
-            print("Single element, saving model with IgnoreElems ML-IAP wrapper")
+            #print("Single element, saving model with IgnoreElems ML-IAP wrapper")
             model = IgnoreElems(self.network_architecture0)
         else:
-            print("Multi element, saving model with ElemwiseModels ML-IAP wrapper")
+            #print("Multi element, saving model with ElemwiseModels ML-IAP wrapper")
             model = ElemwiseModels(self.networks, self.n_elem)
         linked_model = TorchWrapper(model, n_descriptors=self.desc_len, n_elements=self.n_elem)
         torch.save(linked_model, filename)
         
 
     def load_lammps_torch(self, filename="FitTorch.pt"):
         """
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/neural_networks/write.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/neural_networks/write.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/ridge_solver/regressor.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/ridge_solver/regressor.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/scalapack.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/scalapack_solver/setup.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/scalapack_solver/setup.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/gen_labels.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/gen_labels.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/genlib.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/genlib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/rpi_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/tree_method.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/tree_method.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/wigner_couple.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/lib/sym_ACE/young.py` & `fitsnap3-3.1.0.1/fitsnap3lib/lib/sym_ACE/young.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/parallel_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/parallel_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,14 @@
 try:
     # stubs = 0 MPI is active
     stubs = 0
     from mpi4py import MPI
 except ModuleNotFoundError:
     stubs = 1
 
-
-class Singleton(type):
-    _instances = {}
-
-    def __call__(cls, *args, **kwargs):
-        if (
-                kwargs is not None
-                and "comm" in kwargs.keys()
-                and kwargs["comm"] is not None
-        ):
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        return cls._instances[cls]
-
-
 def printf(*args, **kw):
     kw['flush'] = True
 
     if 'overwrite' in kw:
         del kw['overwrite']
         kw['end'] = ''
         print("\r", end='')
@@ -153,37 +137,35 @@
 def print_lammps(method):
     def new_method(*args, **kw):
         printf(*args)
         return method(*args, **kw)
     return new_method
 
 
-class ParallelTools(metaclass=Singleton):
+#class ParallelTools(metaclass=Singleton):
+class ParallelTools():
     """
     This classes creates and contains arrays used for fitting, across multiple processors.
 
     Attributes:
         check_fitsnap_exist (bool): Checks whether fitsnap dictionaries exist before creating a new 
             one, set to `False` to allow recreating a dictionary.
     """
 
     def __init__(self, comm=None):
-
         self.check_fitsnap_exist = True # set to False if want to allow re-creating dictionary
-
         if stubs == 0:
             if comm is None:
                 comm = MPI.COMM_WORLD
             self._comm = comm
             self._rank = self._comm.Get_rank()
             self._size = self._comm.Get_size()
-            """
-            Set this to False if want to avoid shared arrays. This is helpful when using the library 
-            to loop over functions that create shared arrays, to avoid mem leaks.
-            """
+            #print(f">>> Parallel tools comm rank {self._rank} size {self._size}: {self._comm}")
+            # Set this to False if want to avoid shared arrays. This is helpful when using the library 
+            # to loop over functions that create shared arrays, to avoid mem leaks.
             self.create_shared_bool = True
 
         if stubs == 1:
             self._rank = 0
             self._size = 1
             self._comm = None
             self._sub_rank = 0
@@ -201,14 +183,29 @@
         self._set_seed()
         self.shared_arrays = {}
         self.fitsnap_dict = {}
         self.logger = None
         self.pytest = False
         self._fp = None
 
+    """
+    def __del__(self):
+        self.free()
+        del self
+    """
+
+    """
+    def __setattr__(self, name:str, value):
+        protected = ("_comm")
+        if name in protected and hasattr(self, name):
+            raise AttributeError(f"Overwriting {name} is not allowed.")
+        else:
+            super().__setattr__(name, value)
+    """
+
     @stub_check
     def _comm_split(self):
         self._sub_comm = self._comm.Split_type(MPI.COMM_TYPE_SHARED)
         self._sub_rank = self._sub_comm.Get_rank()
         self._sub_size = self._sub_comm.Get_size()
         self._sub_head_proc = 0
         if self._sub_rank == 0:
@@ -315,19 +312,39 @@
     def sub_rank_zero(self, method):
         if self._sub_rank == 0:
             def check_if_rank_zero(*args, **kw):
                 return method(*args, **kw)
             return check_if_rank_zero
         else:
             return dummy_function
+        
+    def free(self):
+        """ Free memory associated with all shared arrays. """
+        if not stubs:
+            for name in self.shared_arrays:
+                # There is no mpi4py native clean way to check if an array is
+                # already freed, so let's do try/except for now.
+                try:
+                    self.shared_arrays[name].win.Free()
+                except:
+                    pass
+        else:
+            self.single_print("Trying to free a stubs array; doing nothing.")
 
     def create_shared_array(self, name, size1, size2=1, dtype='d', tm=0):
 
         if isinstance(name, str):
             if (stubs == 0 and self.create_shared_bool):
+                # If key exists, free the window memory to prevent memory leaks.
+                # TODO: Is there a way to check state of the window instead of the key?
+                if (name in self.shared_arrays and not stubs):
+                    try:
+                        self.shared_arrays[name].win.Free()
+                    except Exception as e:
+                        self.single_print(f"Trouble deallocating shared array with name {name}: {e}.")
                 comms = [[self._comm, self._rank, self._size],
                          [self._sub_comm, self._sub_rank, self._sub_size],
                          [self._head_group_comm, self._node_index, self._number_of_nodes]]
 
                 self.shared_arrays[name] = SharedArray(size1, size2=size2,
                                                        dtype=dtype,
                                                        multinode=tm,
@@ -340,15 +357,16 @@
     # @stub_check
     def add_2_fitsnap(self, name, an_object):
 
         # TODO: Replace cluttered shared array hanging objects!
         if isinstance(name, str):
             if (self.check_fitsnap_exist):
                 if name in self.fitsnap_dict:
-                    raise NameError("name is already in dictionary")
+                    #raise NameError("name is already in dictionary")
+                    self.fitsnap_dict.pop(name)
             self.fitsnap_dict[name] = an_object
         else:
             raise TypeError("name must be a string")
 
     @stub_check
     def _bcast_fitsnap(self, name):
 
@@ -357,19 +375,31 @@
                 raise NameError("Dictionary element not yet in fitsnap_dictionary")
         else:
             self.fitsnap_dict[name] = None
 
         self.fitsnap_dict[name] = self._sub_comm.bcast(self.fitsnap_dict[name])
 
     @stub_check
-    def gather_fitsnap(self, name):
-
+    def gather_fitsnap(self, name, allgather:bool=None):
+        """
+        Gather distributed lists.
+        Args:
+            allgather: If true then we allgather. When number of procs is large this can 
+                       result in large (but not prohibitive) memory usage, where each proc has 
+                       ~10 lists with size of number of configs.
+        """
         if name not in self.fitsnap_dict:
             raise NameError("Dictionary element not yet in fitsnap_dictionary")
-        self.fitsnap_dict[name] = self._sub_comm.gather(self.fitsnap_dict[name], root=0)
+        # TODO: Make some sort of option to either gather or allgather.
+        #       It saves memory to simply gather, but allgather is useful in 
+        #       scenarios when using multiple instances in parallel, we might need 
+        #       the fitsnap dict on all procs.
+        # NOTE: When number of procs is large, allgather could quickly consume all memory.
+        #self.fitsnap_dict[name] = self._sub_comm.gather(self.fitsnap_dict[name], root=0)
+        self.fitsnap_dict[name] = self._sub_comm.allgather(self.fitsnap_dict[name])
 
     @stub_check
     @_sub_rank_zero
     def gather_to_head_node(self, array):
         return self._head_group_comm.allgather(array)
 
     @stub_check
@@ -477,14 +507,31 @@
 
     def close_lammps(self):
         if self._lmp is not None:
             # Kill lammps jobs
             self._lmp.close()   
             self._lmp = None
         return self._lmp
+    
+    def get_ncpn(self, nconfigs):
+        """
+        Get number of configs per node; return nconfigs if stubs.
+
+        Args:
+            nconfigs: integer number of configurations on this process, typically length of list of 
+                      data dictionaries.
+
+        Returns number of configs per node, reduced across procs, or just nconfigs if stubs.
+        """
+        if not stubs:
+            ncpp = np.array([nconfigs]) # Num. configs per proc.
+            ncpn = np.array([0]) # Num. configs per node.
+            self._comm.Allreduce([ncpp, MPI.INT], [ncpn, MPI.INT])
+            return ncpn[0]
+        return nconfigs
 
     def slice_array(self, name):
         if name in self.shared_arrays:
             if name != 'a':
                 s = slice(self._sub_rank, None, self._sub_size)
                 self.shared_arrays[name].sliced_array = self.shared_arrays[name].array[s][:]
             else:
@@ -866,17 +913,17 @@
             raise TypeError("dtype {} has not been implemented yet".format(dtype))
         if self._comms[1][1] == 0:
             self._nbytes = self._length * self._width * item_size
         else:
             self._nbytes = 0
 
         #win = MPI.Win.Allocate_shared(self._nbytes, item_size, Intracomm_comm=self._comms[1][0])
-        win = MPI.Win.Allocate_shared(self._nbytes, item_size, comm=self._comms[1][0])
+        self.win = MPI.Win.Allocate_shared(self._nbytes, item_size, comm=self._comms[1][0])
 
-        buff, item_size = win.Shared_query(0)
+        buff, item_size = self.win.Shared_query(0)
 
         if dtype == 'd':
             assert item_size == MPI.DOUBLE.Get_size()
         elif dtype == 'i':
             assert item_size == MPI.INT32_T.Get_size()
         if self._width == 1:
             self.array = np.ndarray(buffer=buff, dtype=dtype, shape=(self._length, ))
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/json_scraper.py` & `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/json_scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 from fitsnap3lib.scrapers.scrape import Scraper, convert
-from fitsnap3lib.io.input import Config
 from json import loads
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.output import output
 from copy import copy
 import numpy as np
 
 
-config = Config()
-pt = ParallelTools()
-
-
 class Json(Scraper):
 
-    def __init__(self, name):
-        super().__init__(name)
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self.all_data = []
 
     def scrape_groups(self):
         super().scrape_groups()
         self.configs = self.files
 
     def scrape_configs(self):
+        """
+        Loop file files in parallel and populate the data dictionary on this proc.
+        Note that `self.configs` at this point includes all filenames on this proc.
+        """
+        self.all_data = [] # Reset to empty list in case running scraper twice.
         self.files = self.configs
         self.conversions = copy(self.default_conversions)
         data_path = self.config.sections["PATH"].datapath
         for i, file_name in enumerate(self.files):
             if file_name.endswith('.json'):
                 with open(file_name) as file:
                     if file.readline()[0]=="{":
                         file.seek(0)
                     try:
                         self.data = loads(file.read(), parse_constant=True)
                     except Exception as e:
-                        output.screen("Trouble Parsing Training Data: ", file_name)
-                        output.exception(e)
+                        self.pt.single_print(f"Trouble parsing training data: {file_name}")
+                        self.pt.single_print(f"{e}")
 
                     assert len(self.data) == 1, "More than one object (dataset) is in this file"
 
                     self.data = self.data['Dataset']
 
                     assert len(self.data['Data']) == 1, "More than one configuration in this dataset"
                     
@@ -52,24 +50,24 @@
 
                     # Move data up one level
                     self.data.update(self.data.pop('Data')[0])  
 
                     for key in self.data:
                         if "Style" in key:
                             if key.replace("Style", "") in self.conversions:
-                                temp = config.sections["SCRAPER"].properties[key.replace("Style", "")]
+                                temp = self.config.sections["SCRAPER"].properties[key.replace("Style", "")]
                                 temp[1] = self.data[key]
                                 self.conversions[key.replace("Style", "")] = convert(temp)
 
-                    for key in config.sections["SCRAPER"].properties:
+                    for key in self.config.sections["SCRAPER"].properties:
                         if key in self.data:
                             self.data[key] = np.asarray(self.data[key])
 
                     natoms = np.shape(self.data["Positions"])[0]
-                    pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
+                    #self.pt.shared_arrays["number_of_atoms"].sliced_array[i] = natoms
                     self.data["QMLattice"] = (self.data["Lattice"] * self.conversions["Lattice"]).T
 
                     # Populate with LAMMPS-normalized lattice
                     del self.data["Lattice"]  
 
                     # TODO Check whether "Label" container useful to keep around
                     if "Label" in self.data:
@@ -80,25 +78,25 @@
 
                     # Insert electronegativities, which are per-atom scalars
                     if (self.config.sections["CALCULATOR"].per_atom_scalar):
                         if not isinstance(self.data["Chis"], float):
                             self.data["Chis"] = self.data["Chis"]
 
                     # Currently, ESHIFT should be in units of your training data (note there is no conversion)
-                    if hasattr(config.sections["ESHIFT"], 'eshift'):
+                    if hasattr(self.config.sections["ESHIFT"], 'eshift'):
                         for atom in self.data["AtomTypes"]:
-                            self.data["Energy"] += config.sections["ESHIFT"].eshift[atom]
+                            self.data["Energy"] += self.config.sections["ESHIFT"].eshift[atom]
 
                     self.data["test_bool"] = self.test_bool[i]
 
                     self.data["Energy"] *= self.conversions["Energy"]
 
                     self._rotate_coords()
                     self._translate_coords()
 
                     self._weighting(natoms)
 
                     self.all_data.append(self.data)
             else:
-                pt.single_print("Non-json file found: ", file_name)    
+                self.pt.single_print("Non-json file found: ", file_name)    
 
         return self.all_data
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scrape.py` & `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scrape.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,69 +25,68 @@
 #     Steve Plimpton (Sandia National Labs)
 #     Gary Saavedra (Sandia National Labs)
 #     Peter Schultz (Sandia National Labs)
 #     Laura Swiler (Sandia National Labs)
 #
 # <!-----------------END-HEADER------------------------------------->
 
-from fitsnap3lib.io.input import Config
 from os import path, listdir, stat
 import numpy as np
-from random import seed, random, shuffle
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.output import output
+from random import random, seed, shuffle
 from fitsnap3lib.units.units import convert
 from copy import copy
-# from natsort import natsorted
-
-
-#config = Config()
-#pt = ParallelTools()
 
 
 class Scraper:
 
-    def __init__(self, name):
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        self.pt = pt #ParallelTools()
+        self.config = config #Config()
         self.name = name
         self.group_types = {}
         self.group_table = []
         self.files = {}
-        self.configs = {}
+        self.configs = {} # Originally a dict for `scrape_groups` but gets transformed to list of files.
         self.tests = None
         self.data = {}
         self.test_bool = None
         self.default_conversions = {key: convert(self.config.sections["SCRAPER"].properties[key])
                                     for key in self.config.sections["SCRAPER"].properties}
         self.conversions = {}
 
         self._init_units()
 
     def scrape_groups(self):
+        """
+        Scrape groups of files for a particular fitsnap instance.
+        """
+        # Reset as empty dict in case running scrape twice.
+        self.files = {}
+
         group_dict = {k: self.config.sections["GROUPS"].group_types[i]
                       for i, k in enumerate(self.config.sections["GROUPS"].group_sections)}
         self.group_table = self.config.sections["GROUPS"].group_table
         size_type = None
         testing_size_type = None
         user_set_random_seed = self.config.sections["GROUPS"].random_seed ## default is 0
 
         if self.config.sections["GROUPS"].random_sampling:
-            output.screen(f"Random sampling of groups toggled on.")
+            #output.screen(f"Random sampling of groups toggled on.")
+            self.pt.single_print(f"Random sampling of groups toggled on.")
             if not user_set_random_seed:
                 sampling_seed = self.pt.get_seed()
                 seed_txt = f"FitSNAP-generated seed for random sampling: {self.pt.get_seed()}"
             else:
                 ## groups.py casts random_seed to float, just in case user
                 ## uses continuous variable. if user input was originally
                 ## an integer, this casts it to int (less confusing for user)
                 if user_set_random_seed.is_integer():
                     sampling_seed = int(user_set_random_seed)
                 seed_txt = f"User-set seed for random sampling: {sampling_seed}"
-            output.screen(seed_txt)
+            self.pt.single_print(seed_txt)
             seed(sampling_seed)
             self._write_seed_file(seed_txt)
 
         for key in self.group_table:
             bc_bool = False
             training_size = None
             if 'size' in self.group_table[key]:
@@ -127,35 +126,39 @@
                     testing_size = nfiles - training_size
             if testing_size != 0 and (testing_size < 1 or (testing_size == 1 and testing_size_type == float)):
                 testing_size = max(1, int(abs(testing_size) * nfiles + 0.5))
             training_size = self._float_to_int(training_size)
             testing_size = self._float_to_int(testing_size)
             if nfiles-testing_size-training_size < 0:
                 # Force testing_size and training_size to add up to nfiles.
-                #raise ValueError("training size: {} + testing size: {} is greater than files in folder: {}".format(
-                #    training_size, testing_size, nfiles))
                 warnstr = f"\nWARNING: {key} train size {training_size} + test size {testing_size} > nfiles {nfiles}\n"
                 warnstr += "         Forcing testing size to add up properly.\n"
                 self.pt.single_print(warnstr)
                 testing_size = nfiles - training_size
-            output.screen(key, ": Detected ", nfiles, " fitting on ", training_size, " testing on ", testing_size)
+            if (self.config.args.verbose):
+                self.pt.single_print(key, ": Detected ", nfiles, " fitting on ", training_size, " testing on ", testing_size)
             if self.tests is None:
                 self.tests = {}
             self.tests[folder] = []
             for i in range(nfiles - training_size - testing_size):
                 self.files[folder].pop()
             for i in range(testing_size):
                 self.tests[folder].append(self.files[folder].pop())
 
             self.group_table[key]['training_size'] = training_size
             self.group_table[key]['testing_size'] = testing_size
             # self.files[folder] = natsorted(self.files[folder])
 
     # TODO : Fix divvy up to distribute groups evenly and based on memory
     def divvy_up_configs(self):
+        """
+        Function to organize groups and allocate shared arrays used in Calculator.
+        """
+
+        # Loop over `configs` which is a list of filenames, and organize into groups.
         self.test_bool = []
         groups = []
         group_list = []
         temp_list = []
         test_list = []
         for i, folder in enumerate(self.configs):
             for configuration in self.configs[folder]:
@@ -193,41 +196,26 @@
         for i, group in enumerate(group_set):
             group_counts[i] = groups.count(group)
         for i, group in enumerate(group_test):
             group_counts[i+len(group_set)] = group_list.count(group)
         for i in range(len(group_test)):
             group_test[i] += '_testing'
 
+        # TODO: `configs_per_group` shared array doesn't seemed to be used anywhere except bcs, 
+        #       mcmc, and opt solvers.
         self.pt.create_shared_array('configs_per_group', len(group_counts), dtype='i')
         if self.pt.get_rank() == 0:
             for i in range(len(group_counts)):
                 self.pt.shared_arrays['configs_per_group'].array[i] = group_counts[i]
         self.pt.shared_arrays['configs_per_group'].list = group_set + group_test
-
         self.pt.shared_arrays['configs_per_group'].testing = 0
         if self.tests is not None:
             self.pt.shared_arrays['configs_per_group'].testing = len(test_list)
 
-        number_of_configs_per_node = len(self.configs)
-        self.pt.create_shared_array('number_of_atoms', number_of_configs_per_node, dtype='i')
-        self.pt.slice_array('number_of_atoms')
-        self.pt.shared_arrays['number_of_atoms'].configs = temp_configs
-
-        # number of dgrad rows serves similar purpose as number of atoms
-        
-        self.pt.create_shared_array('number_of_dgrad_rows', number_of_configs_per_node, dtype='i')
-        self.pt.slice_array('number_of_dgrad_rows')
-        self.pt.shared_arrays['number_of_dgrad_rows'].configs = temp_configs
-
-        # number of neighs serves similar purpose as number of atoms for custom calculator
-        
-        self.pt.create_shared_array('number_of_neighs_scrape', number_of_configs_per_node, dtype='i')
-        self.pt.slice_array('number_of_neighs_scrape')
-
-        # PROCS SPLIT UP HERE
+        # Procs split up here. This is for injecting into the data dictionary in `scrape_configs()`.
         self.test_bool = self.pt.split_within_node(self.test_bool)
         self.configs = self.pt.split_within_node(self.configs)
 
     def scrape_configs(self):
         raise NotImplementedError("Call to virtual Scraper.scrape_configs method")
 
     def _init_units(self):
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/scraper_factory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/scraper_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from fitsnap3lib.scrapers.xyz_scraper import XYZ
 from fitsnap3lib.scrapers.vasp_scraper import Vasp
 
 
 #pt = ParallelTools()
 
 
-def scraper(scraper_name):
+def scraper(scraper_name, pt, config):
     """Section Factory"""
     instance = search(scraper_name)
-    instance.__init__(scraper_name)
+    instance.__init__(scraper_name, pt, config)
     return instance
 
 
 def search(scraper_name):
     instance = None
     for cls in Scraper.__subclasses__():
         if cls.__name__.lower() == scraper_name.lower():
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/vasp_scraper.py` & `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/vasp_scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from fitsnap3lib.scrapers.scrape import Scraper, convert
-from fitsnap3lib.io.input import Config
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.output import output
+#from fitsnap3lib.io.input import Config
+#from fitsnap3lib.parallel_tools import ParallelTools
+#from fitsnap3lib.io.output import output
 from copy import copy
 from glob import glob
 from random import shuffle
 from datetime import datetime
 import numpy as np
 import os, json
 
 
-config = Config()
-pt = ParallelTools()
+#config = Config()
+#pt = ParallelTools()
 
 class Vasp(Scraper):
 
     def __init__(self, name): 
         super().__init__(name)
         pt.single_print("Initializing VASP scraper")
         self.all_data = []
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/scrapers/xyz_scraper.py` & `fitsnap3-3.1.0.1/fitsnap3lib/scrapers/xyz_scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from fitsnap3lib.scrapers.scrape import Scraper
-from fitsnap3lib.io.input import Config
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.output import output
 import numpy as np
 from random import shuffle, random
 from os import path, listdir
 from copy import copy
 import re
 from _collections import defaultdict
 
 
-config = Config()
-pt = ParallelTools()
+#config = Config()
+#pt = ParallelTools()
 
 
 UNPROCESSED_KEYS = ['uid']
 
 PROPERTY_NAME_MAP = {'positions': 'pos',
                      'numbers': 'Z',
                      'charges': 'charge',
@@ -270,41 +267,47 @@
         del arrays['symbols']
 
     return data, arrays, info
 
 
 class XYZ(Scraper):
 
-    def __init__(self, name):
-        super().__init__(name)
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
         self.conversions = copy(self.default_conversions)
         self.all_data = []
         self.style_info = {}
 
     def scrape_groups(self):
-        if config.sections["SCRAPER"].save_group_scrape != "None":
-            save_file = config.sections["PATH"].relative_directory + '/' + config.sections["SCRAPER"].save_group_scrape
+        # Reset as empty dict in case running scrape twice.
+        self.files = {}
+        self.configs = {}
+
+        pt = self.pt
+        config = self.config
+        if self.config.sections["SCRAPER"].save_group_scrape != "None":
+            save_file = self.config.sections["PATH"].relative_directory + '/' + self.config.sections["SCRAPER"].save_group_scrape
             if pt.get_rank() == 0:
                 with open(save_file, 'w') as fp:
                     fp.write('')
         else:
             save_file = None
-        if config.sections["SCRAPER"].read_group_scrape != "None":
-            if config.sections["SCRAPER"].save_group_scrape != "None":
+        if self.config.sections["SCRAPER"].read_group_scrape != "None":
+            if self.config.sections["SCRAPER"].save_group_scrape != "None":
                 raise RuntimeError("Do not set both reading and writing of group_scrape")
-            read_file = config.sections["PATH"].relative_directory + '/' + config.sections["SCRAPER"].read_group_scrape
+            read_file = self.config.sections["PATH"].relative_directory + '/' + self.config.sections["SCRAPER"].read_group_scrape
         else:
             read_file = None
 
-        group_dict = {k: config.sections["GROUPS"].group_types[i]
-                      for i, k in enumerate(config.sections["GROUPS"].group_sections)}
-        self.group_table = config.sections["GROUPS"].group_table
+        group_dict = {k: self.config.sections["GROUPS"].group_types[i]
+                      for i, k in enumerate(self.config.sections["GROUPS"].group_sections)}
+        self.group_table = self.config.sections["GROUPS"].group_table
         size_type = None
         testing_size_type = None
-        folder_files = listdir(config.sections["PATH"].datapath)
+        folder_files = listdir(self.config.sections["PATH"].datapath)
 
         for key in self.group_table:
             bc_bool = False
             training_size = None
             if 'size' in self.group_table[key]:
                 training_size = self.group_table[key]['size']
                 bc_bool = True
@@ -318,32 +321,32 @@
                 testing_size = self.group_table[key]['testing_size']
                 testing_size_type = group_dict['testing_size']
             else:
                 testing_size = 0
             if training_size is None:
                 raise ValueError("Please set training size for {}".format(key))
 
-            file_base = path.join(config.sections["PATH"].datapath, key)
+            file_base = path.join(self.config.sections["PATH"].datapath, key)
 
             if file_base.split('/')[-1] + ".extxyz" in folder_files:
                 file_name = file_base + ".extxyz"
             elif file_base.split('/')[-1] + ".xyz" in folder_files:
                 file_name = file_base + ".xyz"
             else:
-                raise FileNotFoundError("{}.xyz not found in {}".format(file_base, config.sections["PATH"].datapath))
+                raise FileNotFoundError("{}.xyz not found in {}".format(file_base, self.config.sections["PATH"].datapath))
 
             if file_base + '.xyz' not in self.files or file_base + '.extxyz':
                 self.files[file_base] = []
                 self.configs[file_base] = []
             else:
                 raise FileExistsError("{} was already found".format(file_base))
 
             self.files[file_base].append(file_name)
 
-            if config.sections["SCRAPER"].read_group_scrape != "None":
+            if self.config.sections["SCRAPER"].read_group_scrape != "None":
                 with open(read_file, 'r') as fp:
                     for line in fp:
                         split_line = line.split()
                         if split_line[0] == file_base:
                             for element in split_line[1:]:
                                 self.configs[file_base].append(int(element))
             else:
@@ -386,28 +389,37 @@
             if testing_size != 0 and (testing_size < 1 or (testing_size == 1 and testing_size_type == float)):
                 testing_size = max(1, int(abs(testing_size) * nconfigs + 0.5))
             training_size = self._float_to_int(training_size)
             testing_size = self._float_to_int(testing_size)
             if nconfigs - testing_size - training_size < 0:
                 raise ValueError("training size: {} + testing size: {} is greater than files in folder: {}".format(
                     training_size, testing_size, nconfigs))
-            output.screen(key, ": Detected ", nconfigs, " fitting on ", training_size, " testing on ", testing_size)
+            pt.single_print(key, ": Detected ", nconfigs, " fitting on ", training_size, " testing on ", testing_size)
             if self.tests is None:
                 self.tests = {}
             self.tests[file_base] = []
             for i in range(nconfigs - training_size - testing_size):
                 self.configs[file_base].pop()
             for i in range(testing_size):
                 self.tests[file_base].append(self.configs[file_base].pop())
 
             self.group_table[key]['training_size'] = training_size
             self.group_table[key]['testing_size'] = testing_size
             # self.files[folder] = natsorted(self.files[folder])
 
     def scrape_configs(self):
+        """
+        Scrape configs defined in the iterables of files and configs.
+
+        Returns a list of data dictionaries containing structural info.
+        """
+        self.all_data = [] # Reset to empty list in case running scraper twice.
+
+        pt = self.pt
+        config = self.config
         for folder_num, folder in enumerate(self.files):
             filename = self.files[folder][0]
             with open(filename) as file:
                 for i, configuration in enumerate(self.configs):
                     if configuration[1] != folder:
                         continue
                     starting_line = configuration[0]
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/anl.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/anl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 from fitsnap3lib.io.outputs.outputs import optional_open
 from fitsnap3lib.io.outputs.snap import _to_coeff_string
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 from sys import float_info as fi
 
-#pt = ParallelTools()
-#config = Config()
-
 class ANL(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name ,pt, config)
 
     #@pt.sub_rank_zero
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
             pt = self.pt   
             config = self.config
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/ard.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/ard.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 try:
     from sklearn.linear_model import ARDRegression
 
 
     class ARD(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
-            self.pt = ParallelTools()
-            self.config = Config()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
 
         #@pt.sub_rank_zero
         def perform_fit(self):
             @self.pt.sub_rank_zero
             def decorated_perform_fit():
                 training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
                 w = self.pt.shared_arrays['w'].array[training]
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/bcs.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/bcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 from scipy.linalg import lstsq
 import numpy as np
 
-pt = ParallelTools()
-config = Config()
 
 def bcs(A, y, sigma2=None, eta=1.e-8, adaptive=0, optimal=1, scale=0.1):
     #------------------------------------------------------------------
     # The BCS algorithm for the following paper:
     # "Bayesian Compressive Sesning" (Preprint, 2007). The algorithm
     # adopts from the fast RVM algorithm [Tipping & Faul, 2003].
     # Coded by: Shihao Ji, ECE, Duke University
@@ -204,19 +200,21 @@
             idx = np.argmin(D)
             basis = V[:, idx]
 
     return weights, errbars, used, sigma2, basis, Sig # the last Sig was recently added
 
 class BCS(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
     @pt.sub_rank_zero
     def perform_fit(self):
+        pt = self.pt
+        config = self.config
         if pt.shared_arrays['configs_per_group'].testing_elements != 0:
             testing = -1*pt.shared_arrays['configs_per_group'].testing_elements
         else:
             testing = len(pt.shared_arrays['w'].array)
         w = pt.shared_arrays['w'].array[:testing]
         aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[:testing], w * pt.shared_arrays['b'].array[:testing]
 #        Transpose method does not work with Quadratic SNAP (why?)
@@ -237,15 +235,15 @@
         print("AAA ", used, aw.shape, used.shape, fit_.shape, Sig.shape)
         self.cov[np.ix_(used, used)] = Sig
         nsam = config.sections["SOLVER"].nsam
         self.fit_sam = np.random.multivariate_normal(self.fit, self.cov, size=(nsam,))
         # self.fit_sam = self.fit + np.sqrt(np.diag(self.cov))*np.random.randn(nsam,nbas)
 
     def _dump_a(self):
-        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
+        np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
-        b = pt.shared_arrays['a'].array @ self.fit
+        b = self.pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/jax.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/jax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
-
 import numpy as np
 from functools import partial
 from time import time
 import pickle
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 try:
     from fitsnap3lib.lib.neural_networks.pytorch import create_torch_network, FitTorch
     from fitsnap3lib.lib.neural_networks.jax import jnp, loss, accuracy, mae, jit, grad, adam, apply_updates
     from fitsnap3lib.tools.dataloaders import InRAMDatasetJAX, DataLoader, jax_collate
 
     class JAX(Solver):
 
-        def __init__(self, name):
-            super().__init__(name, linear=False)
-            self.config = Config()
-            self.pt = ParallelTools()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config, linear=False)
             self.params = self.config.sections["JAX"].params
             self.learning_rate = self.config.sections["JAX"].learning_rate
             self.optimizer = adam(self.learning_rate)
             self.targets = None
             self.indices = []
             self.num_atoms = None
             self.opt_state = None
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/lasso.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/ridge.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,53 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
+from fitsnap3lib.lib.ridge_solver.regressor import Local_Ridge
 import numpy as np
 
 
 #config = Config()
 #pt = ParallelTools()
 
+class RIDGE(Solver):
 
-try:
-    from sklearn.linear_model import Lasso
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
+    def perform_fit(self):
+        @self.pt.sub_rank_zero
+        def decorated_perform_fit():
+
+            training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
+            w = self.pt.shared_arrays['w'].array[training]
+            aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
+            if 'EXTRAS' in self.config.sections and self.config.sections['EXTRAS'].apply_transpose:
+                bw = aw.T @ bw
+                aw = aw.T @ aw
+            alval = self.config.sections['RIDGE'].alpha
+            #print (self.config.sections['RIDGE'].local_solver, type(self.config.sections['RIDGE'].local_solver))
+            if not self.config.sections['RIDGE'].local_solver:
+                try:
+                    from sklearn.linear_model import Ridge
+                    reg = Ridge(alpha = alval, fit_intercept = False)
+                except ModuleNotFoundError:
+                    self.pt.single_print('Cannot find sklearn module, using local ridge solver anyway')
+                    reg = Local_Ridge(alpha = alval, fit_intercept = False)
+            elif self.config.sections['RIDGE'].local_solver:
+                reg = Local_Ridge(alpha = alval, fit_intercept = False)
+
+            reg.fit(aw, bw)
+            self.pt.single_print('printing fit: ', reg.coef_)
+            self.fit = reg.coef_
+            residues = np.matmul(aw,reg.coef_) - bw
+        decorated_perform_fit()
+
+
+    #@staticmethod
+    def _dump_a():
+        np.savez_compressed('a.npz', a= self.pt.shared_arrays['a'].array)
+
+    def _dump_x(self):
+        np.savez_compressed('x.npz', x=self.fit)
+
+    def _dump_b(self):
+        b = self.pt.shared_arrays['a'].array @ self.fit
+        np.savez_compressed('b.npz', b=b)
 
-    class LASSO(Solver):
-
-        def __init__(self, name):
-            super().__init__(name)
-            self.pt = ParallelTools()
-            self.config = Config()
-
-        def perform_fit(self):
-            @self.pt.sub_rank_zero
-            def decorated_perform_fit():
-                training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
-                w = self.pt.shared_arrays['w'].array[training]
-                aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
-                if self.config.sections['EXTRAS'].apply_transpose:
-                    bw = aw.T @ bw
-                    aw = aw.T @ aw
-                alval = self.config.sections['LASSO'].alpha
-                maxitr = self.config.sections['LASSO'].max_iter
-                reg = Lasso(alpha=alval, fit_intercept=False, max_iter=maxitr)
-                reg.fit(aw, bw)
-                self.fit = reg.coef_
-            decorated_perform_fit()
-
-        #@staticmethod
-        def _dump_a():
-            np.savez_compressed('a.npz', a= self.pt.shared_arrays['a'].array)
-
-        def _dump_x(self):
-            np.savez_compressed('x.npz', x=self.fit)
-
-        def _dump_b(self):
-            b = self.pt.shared_arrays['a'].array @ self.fit
-            np.savez_compressed('b.npz', b=b)
-
-except ModuleNotFoundError:
-
-    class LASSO(Solver):
-
-        def __init__(self, name):
-            super().__init__(name)
-            raise ModuleNotFoundError("No module named 'sklearn'")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/lreg.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/lreg.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/mcmc.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/mcmc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 from scipy.linalg import lstsq
 
 #pt = ParallelTools()
 #config = Config()
 
 
@@ -76,18 +74,16 @@
 def logpost(x, aw, bw):
     lpostm = log_norm_pdf(aw@x,bw,sigma=0.1)
     return np.sum(lpostm)
 
 
 class MCMC(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
             pt = self.pt
             config = self.config
             if pt.shared_arrays['configs_per_group'].testing_elements != 0:
@@ -123,15 +119,15 @@
             np.savetxt('chn_sam.txt', self.fit_sam)
             np.save('mean.npy', self.fit)
 
         decorated_perform_fit()
 
 
     def _dump_a(self):
-        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
+        np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
-        b = pt.shared_arrays['a'].array @ self.fit
+        b = self.pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/merr.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/merr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 from fitsnap3lib.io.outputs.outputs import optional_open
 from fitsnap3lib.io.outputs.snap import _to_coeff_string
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 from sys import float_info as fi
 
 from .lreg import lreg_merr
 
-#pt = ParallelTools()
-#config = Config()
-
 class MERR(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
             pt = self.pt
             config = self.config
             training = [not elem for elem in pt.fitsnap_dict['Testing']]
@@ -96,15 +89,15 @@
             if nsam:
                 self.fit_sam = np.random.multivariate_normal(self.fit, self.cov, size=(nsam,))
             # self.fit_sam = self.fit + np.sqrt(np.diag(self.cov))*np.random.randn(nsam,nbas)
 
         decorated_perform_fit()
 
     def _dump_a(self):
-        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
+        np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
-        b = pt.shared_arrays['a'].array @ self.fit
+        b = self.pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/network.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import sys
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 from time import time
 import numpy as np
 import psutil
 
-#config = Config()
-#pt = ParallelTools()
 
 try:
     from fitsnap3lib.lib.neural_networks.pairwise import FitTorch, create_torch_network
     from fitsnap3lib.tools.dataloader.pairwise import InRAMDatasetPyTorch, torch_collate, DataLoader
     from fitsnap3lib.tools.configuration import Configuration
     import torch
 
@@ -29,19 +25,16 @@
             learning_rate (:obj:`float`): Learning rate for gradient descent
             scheduler (:obj:`torch.optim.lr_scheduler.ReduceLROnPlateau`): Learning rate scheduler
             device: Accelerator device
             training_data (:obj:`torch.utils.data.Dataset`): Torch dataset for training
             training_loader (:obj:`torch.utils.data.DataLoader`): Data loader for loading in datasets
         """
 
-        def __init__(self, name):
-            super().__init__(name, linear=False)
-
-            self.pt = ParallelTools()
-            self.config = Config()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config, linear=False)
 
             self.global_weight_bool = self.config.sections['NETWORK'].global_weight_bool
             self.energy_weight = self.config.sections['NETWORK'].energy_weight
             self.force_weight = self.config.sections['NETWORK'].force_weight
 
             self.global_fraction_bool = self.config.sections['NETWORK'].global_fraction_bool
             self.training_fraction = self.config.sections['NETWORK'].training_fraction
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/opt.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/opt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 from scipy.optimize import minimize
 import numpy as np
 
-#pt = ParallelTools()
-#config = Config()
 
 def distance(x, aw, bw):
     return np.linalg.norm(np.dot(aw, x) - bw)
 
 
 def distance_grad(x, aw, bw):
     # get analytical gradient:
     return np.dot(aw.T, np.dot(aw, x) - bw)
 
 
 class OPT(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.pt = ParallelTools()
-        self.config = Config()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
 
     @self.pt.sub_rank_zero
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
             pt = self.pt
             config = self.config
@@ -48,15 +42,15 @@
             res = minimize(distance, param_ini, args=(aw, bw), method='BFGS', options={'gtol': 1e-13}, jac=distance_grad)
             self.fit = res.x
             np.save('mean.npy', self.fit)
 
         decorated_perform_fit()
 
     def _dump_a(self):
-        np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
+        np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
 
     def _dump_b(self):
-        b = pt.shared_arrays['a'].array @ self.fit
+        b = self.pt.shared_arrays['a'].array @ self.fit
         np.savez_compressed('b.npz', b=b)
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/pytorch.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 
 import sys
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 from time import time
 import numpy as np
 import psutil
 
-#config = Config()
-#pt = ParallelTools()
-
 try:
     from fitsnap3lib.lib.neural_networks.pytorch import FitTorch, create_torch_network
     from fitsnap3lib.lib.neural_networks.pas import FitTorchPAS
     from fitsnap3lib.tools.dataloaders import InRAMDatasetPyTorch, torch_collate, DataLoader
     from fitsnap3lib.tools.configuration import Configuration
     import torch
 
@@ -32,19 +27,16 @@
             learning_Rate (float): Learning rate for gradient descent.
             scheduler (torch.optim.lr_scheduler.ReduceLROnPlateau): Torch learning rate scheduler.
             device: Torch accelerator device.
             training_data (torch.utils.data.Dataset): Torch dataset for training.
             training_loader (torch.utils.data.DataLoader): Data loader for loading datasets.
         """
 
-        def __init__(self, name):
-            super().__init__(name, linear=False)
-
-            self.pt = ParallelTools()
-            self.config = Config()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config, linear=False)
 
             self.global_weight_bool = self.config.sections['PYTORCH'].global_weight_bool
             self.energy_weight = self.config.sections['PYTORCH'].energy_weight
             self.force_weight = self.config.sections['PYTORCH'].force_weight
 
             self.global_fraction_bool = self.config.sections['PYTORCH'].global_fraction_bool
             self.training_fraction = self.config.sections['PYTORCH'].training_fraction
@@ -110,71 +102,85 @@
                                                                         patience=49,
                                                                         verbose=True,
                                                                         threshold=0.0001,
                                                                         threshold_mode='abs')
 
             self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
             # self.device = "cpu"
-            self.pt.single_print("Pytorch device is set to", self.device)
+            if (self.config.args.verbose):
+                self.pt.single_print("Pytorch device is set to", self.device)
             self.model = self.model.to(self.device)
             self.total_data = None
             self.training_data = None
             self.validation_data = None
             self.training_loader = None
 
         def weighted_mse_loss(self, prediction, target, weight):
             return torch.mean(weight * (prediction - target)**2)
 
-        def create_datasets(self):
+        def create_datasets(self, configs=None, pt=None):
             """
             Creates the dataset to be used for training and the data loader for the batch system.
+
+            Args:
+                configs: Optional list of Configuration objects. If not supplied, we generate a 
+                         configs list using the shared arrays.
+                pt: Optional ParallelTools instance containing data we want to fit to.
             """
 
             # TODO: when only fitting to energy, we don't need all this extra data, and could save 
-            # resources by only fitting some configs to forces. 
+            # resources by only fitting some configs to forces.
 
-            self.configs = [Configuration(int(natoms)) for natoms in self.pt.fitsnap_dict['NumAtoms']]
+            #print(f">>> rank {pt._rank} dict {pt.fitsnap_dict}")
+            if pt is None:
+                pt = self.pt
 
-            # add descriptors and atom types
+            if configs is None:
+                self.configs = [Configuration(int(natoms)) for natoms in pt.fitsnap_dict['NumAtoms']]
 
-            indx_natoms_low = 0
-            indx_forces_low = 0
-            indx_dgrad_low = 0
-            for i, config in enumerate(self.configs):
-                
-                indx_natoms_high = indx_natoms_low + config.natoms
-                indx_forces_high = indx_forces_low + 3*config.natoms
-
-                if (self.pt.fitsnap_dict['force']):
-                    nrows_dgrad = int(self.pt.fitsnap_dict["NumDgradRows"][i])
-                    indx_dgrad_high = indx_dgrad_low + nrows_dgrad
-                    config.forces = self.pt.shared_arrays['c'].array[indx_forces_low:indx_forces_high]
-                    config.dgrad = self.pt.shared_arrays['dgrad'].array[indx_dgrad_low:indx_dgrad_high]
-                    config.dgrad_indices = self.pt.shared_arrays['dbdrindx'].array[indx_dgrad_low:indx_dgrad_high]
-                    indx_dgrad_low += nrows_dgrad
+                # add descriptors and atom types
 
-                if (self.pt.fitsnap_dict['energy']):
-                    config.energy = self.pt.shared_arrays['b'].array[i]
-                    config.weights = self.pt.shared_arrays['w'].array[i]
+                indx_natoms_low = 0
+                indx_forces_low = 0
+                indx_dgrad_low = 0
+                for i, config in enumerate(self.configs):
+                    
+                    indx_natoms_high = indx_natoms_low + config.natoms
+                    indx_forces_high = indx_forces_low + 3*config.natoms
 
-                if (self.pt.fitsnap_dict['per_atom_scalar']):
-                    config.pas = self.pt.shared_arrays['pas'].array[indx_natoms_low:indx_natoms_high]
+                    if (pt.fitsnap_dict['force']):
+                        nrows_dgrad = int(pt.fitsnap_dict["NumDgradRows"][i])
+                        indx_dgrad_high = indx_dgrad_low + nrows_dgrad
+                        config.forces = pt.shared_arrays['c'].array[indx_forces_low:indx_forces_high]
+                        config.dgrad = pt.shared_arrays['dgrad'].array[indx_dgrad_low:indx_dgrad_high]
+                        config.dgrad_indices = pt.shared_arrays['dbdrindx'].array[indx_dgrad_low:indx_dgrad_high]
+                        indx_dgrad_low += nrows_dgrad
+
+                    if (pt.fitsnap_dict['energy']):
+                        config.energy = pt.shared_arrays['b'].array[i]
+                        config.weights = pt.shared_arrays['w'].array[i]
+
+                    if (pt.fitsnap_dict['per_atom_scalar']):
+                        config.pas = pt.shared_arrays['pas'].array[indx_natoms_low:indx_natoms_high]
+
+                    config.filename = pt.fitsnap_dict['Configs'][i]
+                    config.group = pt.fitsnap_dict['Groups'][i]
+                    config.testing_bool = pt.fitsnap_dict['Testing'][i]
+                    config.descriptors = pt.shared_arrays['a'].array[indx_natoms_low:indx_natoms_high]
+                    config.types = pt.shared_arrays['t'].array[indx_natoms_low:indx_natoms_high] - 1 # start types at zero
 
-                config.filename = self.pt.fitsnap_dict['Configs'][i]
-                config.group = self.pt.fitsnap_dict['Groups'][i]
-                config.testing_bool = self.pt.fitsnap_dict['Testing'][i]
-                config.descriptors = self.pt.shared_arrays['a'].array[indx_natoms_low:indx_natoms_high]
-                config.types = self.pt.shared_arrays['t'].array[indx_natoms_low:indx_natoms_high] - 1 # start types at zero
+                    indx_natoms_low += config.natoms
+                    indx_forces_low += 3*config.natoms
 
-                indx_natoms_low += config.natoms
-                indx_forces_low += 3*config.natoms
+                # check that we make assignments (not copies) of data, to save memory
 
-            # check that we make assignments (not copies) of data, to save memory
+                assert(np.shares_memory(self.configs[0].descriptors, pt.shared_arrays['a'].array))
 
-            assert(np.shares_memory(self.configs[0].descriptors, self.pt.shared_arrays['a'].array))
+            else:
+                self.configs = configs
 
             self.total_data = InRAMDatasetPyTorch(self.configs)
 
             # randomly shuffle and split into training/validation data if using global fractions
 
             if (self.global_fraction_bool):
 
@@ -189,15 +195,18 @@
                     torch.utils.data.random_split(self.total_data, 
                                                   [self.train_size, self.test_size])
 
             else: 
 
                 # we are using group training/testing fractions
 
-                training_bool_indices = [not elem for elem in self.pt.fitsnap_dict['Testing']]
+                #blah = [not config.testing_bool for config in self.configs]
+
+                #training_bool_indices = [not elem for elem in self.pt.fitsnap_dict['Testing']]
+                training_bool_indices = [not config.testing_bool for config in self.configs]
                 training_indices = [i for i, x in enumerate(training_bool_indices) if x]
                 testing_indices = [i for i, x in enumerate(training_bool_indices) if not x]
                 self.training_data = torch.utils.data.Subset(self.total_data, training_indices)
                 self.validation_data = torch.utils.data.Subset(self.total_data, testing_indices)
 
             # make training and validation data loaders for batch training
 
@@ -209,29 +218,40 @@
 
             self.validation_loader = DataLoader(self.validation_data,
                                               batch_size=self.config.sections["PYTORCH"].batch_size,
                                               shuffle=self.config.sections['PYTORCH'].shuffle_flag,
                                               collate_fn=torch_collate,
                                               num_workers=0) if len(self.validation_data) > 1 else []
         #@pt.sub_rank_zero
-        def perform_fit(self):
+        def perform_fit(self, configs: list=None, pt=None, outfile: str=None, verbose: bool=True):
             """
             Performs PyTorch fitting using previously calculated descriptors. 
+
+            Args:
+                configs: Optional list of Configuration objects to perform fitting on.
+                pt: ParallelTools instance containing shared arrays and data we want 
+                    to fit to.
+                outfile: Optional output file to write progress to.
+                verbose: Optional flag to print progress to screen; overrides the verbose CLI.
             """
 
             @self.pt.sub_rank_zero
-            def decorated_perform_fit():
-                self.create_datasets()
+            def perform_fit(pt=None,outfile=None):
+                pt = self.pt if pt is None else pt
+                if outfile is not None:
+                    fh = open(outfile, 'w')
+                
+                #self.create_datasets()
                 if self.config.sections['PYTORCH'].save_state_input is None:
 
                     # standardization
                     # need to perform on all network types in the model
 
-                    inv_std = 1/np.std(self.pt.shared_arrays['a'].array, axis=0)
-                    mean_inv_std = np.mean(self.pt.shared_arrays['a'].array, axis=0) * inv_std
+                    inv_std = 1/np.std(pt.shared_arrays['a'].array, axis=0)
+                    mean_inv_std = np.mean(pt.shared_arrays['a'].array, axis=0) * inv_std
                     state_dict = self.model.state_dict()
 
                     # look for the first layer for all types of networks, these are keys like
                     # network_architecture0.0.weight and network_architecture0.0.bias
                     # for the first network, and
                     # network_architecture1.0.weight and network_architecture0.1.bias for the next,
                     # and so forth
@@ -262,16 +282,17 @@
                 target_force_plot_val = []
                 model_force_plot_val = []
                 target_energy_plot_val = []
                 model_energy_plot_val = []
                 target_pas_plot_val = []
                 model_pas_plot_val = []
                 natoms_per_config = [] # stores natoms per config for calculating eV/atom errors later.
+                if (self.config.args.verbose or verbose):
+                    self.pt.single_print(f"{'Epoch': <2} {'Train': ^10} {'Val': ^10} {'Time (s)': >2}")
                 for epoch in range(self.config.sections["PYTORCH"].num_epochs):
-                    print(f"----- epoch: {epoch}")
                     start = time()
 
                     # loop over training data
 
                     train_losses_step = []
                     loss = None
                     self.model.train()
@@ -472,18 +493,22 @@
                             #loss = torch.sqrt(self.loss_function(pas, targets))
                             loss = self.loss_function(pas, targets)
                         
                         val_losses_step.append(loss.item())
 
                     # average training and validation losses across all batches
 
-                    self.pt.single_print("Batch averaged train/val loss:", np.mean(np.asarray(train_losses_step)), np.mean(np.asarray(val_losses_step)))
+                    progress_str = f"{epoch: <2} {np.mean(np.asarray(train_losses_step)): ^10.3e} {np.mean(np.asarray(val_losses_step)): ^10.3e} {time()-start: >2.3e}"
+                    #self.pt.single_print(progress_str)
+                    if (self.config.args.verbose or verbose):
+                        self.pt.single_print(progress_str)
+                    if outfile is not None:
+                        fh.write(progress_str + "\n")
                     train_losses_epochs.append(np.mean(np.asarray(train_losses_step)))
                     val_losses_epochs.append(np.mean(np.asarray(val_losses_step)))
-                    self.pt.single_print("Epoch time", time()-start)
                     if epoch % self.config.sections['PYTORCH'].save_freq == 0:
                         torch.save({
                             'epoch': epoch,
                             'model_state_dict': self.model.state_dict(),
                             'optimizer_state_dict': self.optimizer.state_dict(),
                             'loss': loss},
                             self.config.sections['PYTORCH'].save_state_output
@@ -562,26 +587,25 @@
 
                 epochs = np.arange(self.config.sections["PYTORCH"].num_epochs)
                 epochs = np.array([epochs]).T
                 train_losses_epochs = np.array([train_losses_epochs]).T
                 val_losses_epochs = np.array([val_losses_epochs]).T
                 loss_dat = np.concatenate((epochs,train_losses_epochs,val_losses_epochs),axis=1)
                 np.savetxt("loss_vs_epochs.dat", loss_dat)
-
-                self.pt.single_print("Average loss over batches is", np.mean(np.asarray(train_losses_step)))
                 
                 #if 'lammps.mliap' in sys.modules:
                 self.model.write_lammps_torch(self.config.sections["PYTORCH"].output_file)
                 #else:
                 #    print("Warning: This interpreter is not compatible with python-based mliap for LAMMPS. If you are using a Mac please make sure you have compiled python from source with './configure --enabled-shared' ")
                 #    print("Warning: FitSNAP will continue without ML-IAP")
                 
                 self.fit = None
 
-            decorated_perform_fit()
+            self.create_datasets(configs=configs, pt=pt)
+            perform_fit(pt=pt, outfile=outfile)
 
         #@pt.sub_rank_zero
         def evaluate_configs(self, config_idx = 0, standardize_bool = True, dtype=torch.float64, eval_device='cpu'):
             """
             Evaluates energies and forces on configs for testing purposes. 
 
             Args:
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/scalapack.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/scalapack.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
-#config = Config()
-#pt = ParallelTools()
-
-
 try:
     from fitsnap3lib.lib.scalapack_solver.scalapack import lstsq, dummy_lstsq
 
     class ScaLAPACK(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
-            self.config = Config()
-            self.pt = ParallelTools()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
 
         def perform_fit(self):
             # This dictionary is NoneType on other subranks.
             if self.pt.get_subrank() == 0:
                 if any(self.pt.fitsnap_dict['Testing']):
                     raise NotImplementedError("Testing w/ the ScaLAPACK solver is not implemented!")
             self.pt.split_by_node(self.pt.shared_arrays['w'])
@@ -58,18 +50,18 @@
             b = self.pt.shared_arrays['a'].array @ self.fit
             np.savez_compressed('b.npz', b=b)
 
 except ModuleNotFoundError:
 
     class ScaLAPACK(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
             raise ModuleNotFoundError("ScaLAPACK module not installed in lib")
 
 except ImportError:
 
     class ScaLAPACK(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
             raise ImportError("ScaLAPACK module not installed in lib")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
     This class declares the method to solve the machine learning problem, e.g. linear regression,
     nonlinear regression, etc.
 
     Attributes:
         fit: Numpy array containing coefficients of fit.
     """
 
-    def __init__(self, name, linear=True):
-        self.config = Config()
-        self.pt = ParallelTools()
+    def __init__(self, name, pt, config, linear=True):
+        self.config = config #Config()
+        self.pt = pt #ParallelTools()
         self.name = name
         self.configs = None
         self.fit = None
         self.all_fits = None
         self.template_error = False
         self.errors = []
         self.weighted = 'Unweighted'
@@ -155,22 +155,23 @@
                 count_test['*ALL'] = {}
                 count_test['*ALL']["nconfigs"] = 0 # Total number test configs in group.
                 count_test['*ALL']["natoms"] = 0 # Total number test atoms in group.
                 count_train['*ALL'] = {}
                 count_train['*ALL']["nconfigs"] = 0 # Total number test configs in group.
                 count_train['*ALL']["natoms"] = 0 # Total number test atoms in group.
 
-                if (self.config.sections["EXTRAS"].dump_peratom):
-                    fha = open(self.config.sections["EXTRAS"].peratom_file, 'w')
-                    line = f"Filename Group AtomID Type Fx_Truth Fy_Truth Fz_Truth Fx_Pred Fy_Pred Fz_Pred Testing_Bool"
-                    fha.write(line + "\n")
-                if (self.config.sections["EXTRAS"].dump_perconfig):
-                    fhc = open(self.config.sections["EXTRAS"].perconfig_file, 'w')
-                    line = f"Filename Group Natoms Energy_Truth Energy_Pred Testing_Bool"
-                    fhc.write(line + "\n")
+                if 'EXTRAS' in self.config.sections:
+                    if (self.config.sections["EXTRAS"].dump_peratom):
+                        fha = open(self.config.sections["EXTRAS"].peratom_file, 'w')
+                        line = f"Filename Group AtomID Type Fx_Truth Fy_Truth Fz_Truth Fx_Pred Fy_Pred Fz_Pred Testing_Bool"
+                        fha.write(line + "\n")
+                    if (self.config.sections["EXTRAS"].dump_perconfig):
+                        fhc = open(self.config.sections["EXTRAS"].perconfig_file, 'w')
+                        line = f"Filename Group Natoms Energy_Truth Energy_Pred Testing_Bool"
+                        fhc.write(line + "\n")
                 atom_indx = 0
                 m = 0
                 for idx, c in enumerate(self.configs):
                     (energies_model, forces_model) = self.evaluate_configs(config_idx=idx, \
                                                                            standardize_bool=False, \
                                                                            dtype=torch.float64)
                     e_pred = energies_model.detach().numpy()/c.natoms # Model per-atom energy.
@@ -323,21 +324,19 @@
             for key in self.pt.fitsnap_dict.keys():
                 if isinstance(self.pt.fitsnap_dict[key], list) and \
                     len(self.pt.fitsnap_dict[key]) == len(self.df.index):
                     self.df[key] = self.pt.fitsnap_dict[key]
             if self.config.sections["EXTRAS"].dump_dataframe:
                 self.df.to_pickle(self.config.sections['EXTRAS'].dataframe_file)
 
-            # proceed with error analysis if doing a fit
-
+            # Proceed with error analysis if doing a fit.
             if self.fit is not None and not self.config.sections["SOLVER"].true_multinode:
 
-                # return data for each group
-                #print(f"^^^ {self.pt._rank}")
-                #print(self.df)
+                # Return data for each group.
+
                 grouped = self.df.groupby(['Groups', \
                     'Testing', \
                     'Row_Type']).apply(self._ncount_mae_rmse_rsq_unweighted_and_weighted)
 
                 # reformat the weighted and unweighted data into separate rows
 
                 grouped = concat({'Unweighted':grouped[['ncount', 'mae', 'rmse', 'rsq']], \
@@ -357,27 +356,35 @@
                         rename(columns={'w_ncount':'ncount', 'w_mae':'mae', 'w_rmse':'rmse', 'w_rsq':'rsq'})}, \
                         names=['Weighting']).\
                             reorder_levels(['Weighting','Testing', 'Row_Type']).sort_index()
 
                 # combine dataframes
 
                 self.errors = concat([concat({'*ALL':all}, names=['Groups']), grouped])
+                #print(self.errors['mae'].keys())
+                #print(self.errors['mae'][('*ALL', 'Unweighted', False, 'Energy')])
+
+                #assert(False)
                 self.errors.ncount = self.errors.ncount.astype(int)
                 self.errors.index.rename(["Group", "Weighting", "Testing", "Subsystem", ], inplace=True)
 
                 # format for markdown printing
 
                 self.errors.index = self.errors.index.set_levels(['Testing' if e else 'Training' \
                     for e in self.errors.index.levels[2]], \
                         level=2)
-                
+            
+            # Adjust coefficients for bzeroflag.
+            if self.fit is not None: 
                 if (self.config.sections["CALCULATOR"].calculator == "LAMMPSSNAP" and \
                     self.config.sections["BISPECTRUM"].bzeroflag):
                     self._offset()
 
+        # Reset errors to default empty list.
+        self.errors = []
         decorated_error_analysis()
 
     def _all_error(self):
         ## replaced by groupby().apply(ncount_mae_rmse_rsq_unweighted_and_weighted)
         # if self.config.sections["CALCULATOR"].energy:
         #     self._errors("*ALL", "Energy", (self.df['Row_Type'] == 'Energy'))
         # if self.config.sections["CALCULATOR"].force:
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/solver_factory.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/solver_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from fitsnap3lib.solvers.scalapack import ScaLAPACK
 from fitsnap3lib.solvers.svd import SVD
 from fitsnap3lib.solvers.tensorflowsvd import TensorflowSVD
 from fitsnap3lib.solvers.anl import ANL
 from fitsnap3lib.solvers.merr import MERR
 from fitsnap3lib.solvers.network import NETWORK
 
-pt = ParallelTools()
+#pt = ParallelTools()
 
 
-def solver(solver_name):
+def solver(solver_name, pt, cfg):
     """Solver Factory"""
     instance = search(solver_name)
-    instance.__init__(solver_name)
+    instance.__init__(solver_name, pt, cfg)
     return instance
 
 
 def search(solver_name):
     instance = None
     for cls in Solver.__subclasses__():
         if cls.__name__.lower() == solver_name.lower():
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/svd.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/svd.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 #config = Config()
 #pt = ParallelTools()
 
 
 class SVD(Solver):
 
-    def __init__(self, name):
-        super().__init__(name)
-        self.config = Config()
-        self.pt = ParallelTools()
+    def __init__(self, name, pt, config):
+        super().__init__(name, pt, config)
+        #self.config = Config()
+        #self.pt = ParallelTools()
 
     #@pt.sub_rank_zero
     def perform_fit(self):
         @self.pt.sub_rank_zero
         def decorated_perform_fit():
             training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
             w = self.pt.shared_arrays['w'].array[training]
             aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
     #       Look into gradient based linear solvers as well.
-            if self.config.sections['EXTRAS'].apply_transpose:
+            if 'EXTRAS' in self.config.sections and self.config.sections['EXTRAS'].apply_transpose:
                 if np.linalg.cond(aw)**2 < 1 / fi.epsilon:
                     bw = aw[:, :].T @ bw
                     aw = aw[:, :].T @ aw
                 else:
                     print("The Matrix is ill-conditioned for the transpose trick")
             self.fit, residues, rank, s = lstsq(aw, bw, 1.0e-13)
         decorated_perform_fit()
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/solvers/tensorflowsvd.py` & `fitsnap3-3.1.0.1/fitsnap3lib/solvers/tensorflowsvd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from fitsnap3lib.solvers.solver import Solver
-from fitsnap3lib.parallel_tools import ParallelTools
-from fitsnap3lib.io.input import Config
 import numpy as np
 
 
 #config = Config()
 #pt = ParallelTools()
 
 
 try:
     import tensorflow as tf
 
 
     class TensorflowSVD(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
-            self.pt = ParallelTools()
-            self.config = Config()
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
 
         #@pt.single_timeit
         #@pt.sub_rank_zero
         def perform_fit(self):
+            pt = self.pt
+            config = self.config
             @self.pt.single_timeit
             @self.pt.sub_rank_zero
             def decorated_perform_fit():
                 training = [not elem for elem in pt.fitsnap_dict['Testing']]
                 w = pt.shared_arrays['w'].array[training]
                 aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
                 # NOTE: Transpose does not produce correct output
@@ -42,10 +40,10 @@
                     self._offset()
             decorated_perform_fit()
 
 except ModuleNotFoundError:
 
     class TensorflowSVD(Solver):
 
-        def __init__(self, name):
-            super().__init__(name)
+        def __init__(self, name, pt, config):
+            super().__init__(name, pt, config)
             raise ModuleNotFoundError("No module named 'tensorflow'")
```

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/configuration.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/dataframe_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/dataloaders.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/dataloaders.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/lammps_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/lammps_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/nn_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/nn_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/tools/test_tools.py` & `fitsnap3-3.1.0.1/fitsnap3lib/tools/test_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/units/conversion_finder.py` & `fitsnap3-3.1.0.1/fitsnap3lib/units/conversion_finder.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/fitsnap3lib/units/units.py` & `fitsnap3-3.1.0.1/fitsnap3lib/units/units.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/pyproject.toml` & `fitsnap3-3.1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "setuptools>=42",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "fitsnap3"
-version = "3.0.1.2"
+version = "3.1.0.1"
 description = "Molecular Machine Learning Interface"
 license = {file = "LICENSE"}
 readme = "README.md"
-requires-python = ">=3.8.0"
+requires-python = ">=3.10.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 authors = [
     { name = "Drew Rohskopf", email = "adrohsk@sandia.gov" },
```

### Comparing `fitsnap3-3.0.1.2/tests/test_examples.py` & `fitsnap3-3.1.0.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.0.1.2/tests/test_pytorch.py` & `fitsnap3-3.1.0.1/tests/test_pytorch.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,63 +4,57 @@
 import os
 import importlib.util
 import numpy as np
 from mpi4py import MPI
 import argparse
 import random
 import torch
+from fitsnap3lib.fitsnap import FitSnap
 
 
 this_path = Path(__file__).parent.resolve()
 parent_path = Path(__file__).parent.resolve().parent
 example_path = parent_path / 'examples'
 ta_example_file = example_path / 'Ta_PyTorch_NN' / 'Ta-example.in'
 wbe_example_file = example_path / 'WBe_PyTorch_NN' / 'WBe-example.in'
 ace_ta_example_file = example_path / 'Ta_PACE_PyTorch_NN' / 'Ta.in'
 
 def test_fd_single_elem():
     # TODO: Make equivalent test using MPI
 
     h = 1e-4 # size of finite difference
 
-    # import parallel tools and create pt object
-    from fitsnap3lib.parallel_tools import ParallelTools
-    #pt = ParallelTools(comm=comm)
-    pt = ParallelTools()
-    # don't check for existing fitsnap objects since we'll be overwriting things
-    pt.check_fitsnap_exist = False
-    from fitsnap3lib.io.input import Config
-    #fitsnap_in = "../examples/Ta_Pytorch_NN/Ta-example.in"
     fitsnap_in = ta_example_file.as_posix()
-    config = Config(arguments_lst = [fitsnap_in, "--overwrite"])
-    config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
-    config.sections['PYTORCH'].manual_seed_flag = 1
-    config.sections['PYTORCH'].dtype = torch.float64
-    config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
+
+    comm = MPI.COMM_WORLD
+    snap = FitSnap(fitsnap_in, comm=comm, arglist=["--overwrite"])
+    snap.config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
+    snap.config.sections['PYTORCH'].manual_seed_flag = 1
+    snap.config.sections['PYTORCH'].dtype = torch.float64
+    snap.config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
     # only perform calculations on displaced BCC structures
-    config.sections['GROUPS'].group_table = {'Displaced_BCC': \
+    snap.config.sections['GROUPS'].group_table = {'Displaced_BCC': \
         {'training_size': 1.0, \
         'testing_size': 0.0, \
         'eweight': 100.0, \
         'fweight': 1.0, \
         'vweight': 1e-08}}
-    # create a fitsnap object
-    from fitsnap3lib.fitsnap import FitSnap
-    snap = FitSnap()
 
     # get config positions
     snap.scrape_configs()
     data0 = snap.data
     # don't delete the data since we'll use it many times with finite difference
     snap.delete_data = False 
+    # don't check for existing fitsnap objects since we'll be overwriting things
+    snap.pt.check_fitsnap_exist = False
 
     # calculate model forces
 
     snap.process_configs()
-    pt.all_barrier()
+    snap.pt.all_barrier()
     snap.solver.create_datasets()
     (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
@@ -114,59 +108,52 @@
     max_err = np.max(np.abs(percent_errors))
 
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
 
     assert(mean_err < 0.001 and max_err < 0.1)
 
-    del pt
-    del config
-    del snap.data
+    #del pt
+    #del config
+    #del snap.data
     del snap
 
 def test_fd_multi_elem():
     # TODO: Make equivalent test using MPI
 
     h = 1e-4 # size of finite difference
 
-    # import parallel tools and create pt object
-    from fitsnap3lib.parallel_tools import ParallelTools
-    #pt = ParallelTools(comm=comm)
-    pt = ParallelTools()
-    # don't check for existing fitsnap objects since we'll be overwriting things
-    pt.check_fitsnap_exist = False
-    from fitsnap3lib.io.input import Config
-    #fitsnap_in = "../examples/WBe_Pytorch_NN/WBe-example.in"
     fitsnap_in = wbe_example_file.as_posix()
-    config = Config(arguments_lst = [fitsnap_in, "--overwrite"])
-    config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
-    config.sections['PYTORCH'].manual_seed_flag = 1
-    config.sections['PYTORCH'].dtype = torch.float64
-    config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
-    # only perform calculations on a certain group
-    config.sections['GROUPS'].group_table = {'DFT_MD_300K': \
+
+    comm = MPI.COMM_WORLD
+    snap = FitSnap(fitsnap_in, comm=comm, arglist=["--overwrite"])
+    snap.config.sections['BISPECTRUM'].switchflag = 1 # required for smooth finite difference
+    snap.config.sections['PYTORCH'].manual_seed_flag = 1
+    snap.config.sections['PYTORCH'].dtype = torch.float64
+    snap.config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
+    # only perform calculations on certain group
+    snap.config.sections['GROUPS'].group_table = {'DFT_MD_300K': \
         {'training_size': 0.01, \
         'testing_size': 0.0, \
         'eweight': 100.0, \
         'fweight': 1.0, \
         'vweight': 1e-08}}
-    # create a fitsnap object
-    from fitsnap3lib.fitsnap import FitSnap
-    snap = FitSnap()
 
     # get config positions
     snap.scrape_configs()
     data0 = snap.data
     # don't delete the data since we'll use it many times with finite difference
     snap.delete_data = False 
+    # don't check for existing fitsnap objects since we'll be overwriting things
+    snap.pt.check_fitsnap_exist = False
 
     # calculate model forces
 
     snap.process_configs()
-    pt.all_barrier()
+    snap.pt.all_barrier()
     snap.solver.create_datasets()
     (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
@@ -224,59 +211,48 @@
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
 
     print(f"max_err: {max_err}")
 
     assert(mean_err < 0.001 and max_err < 0.1)
 
-    del pt
-    del config
-    del snap.data
     del snap
 
 def test_fd_ace_single_elem():
     # TODO: Make equivalent test using MPI
 
     h = 1e-4 # size of finite difference
 
-    # import parallel tools and create pt object
-    from fitsnap3lib.parallel_tools import ParallelTools
-    #pt = ParallelTools(comm=comm)
-    pt = ParallelTools()
-    # don't check for existing fitsnap objects since we'll be overwriting things
-    pt.check_fitsnap_exist = False
-    from fitsnap3lib.io.input import Config
-    #fitsnap_in = "../examples/Ta_Pytorch_NN/Ta-example.in"
     fitsnap_in = ace_ta_example_file.as_posix()
-    config = Config(arguments_lst = [fitsnap_in, "--overwrite"])
-    #config.sections['ACE'].switchflag = 1 # required for smooth finite difference
-    config.sections['PYTORCH'].manual_seed_flag = 1
-    config.sections['PYTORCH'].dtype = torch.float64
-    config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
+
+    comm = MPI.COMM_WORLD
+    snap = FitSnap(fitsnap_in, comm=comm, arglist=["--overwrite"])
+    snap.config.sections['PYTORCH'].manual_seed_flag = 1
+    snap.config.sections['PYTORCH'].dtype = torch.float64
+    snap.config.sections['PYTORCH'].shuffle_flag = False # helps these finite difference tests
     # only perform calculations on displaced BCC structures
-    config.sections['GROUPS'].group_table = {'Displaced_BCC': \
+    snap.config.sections['GROUPS'].group_table = {'Displaced_BCC': \
         {'training_size': 1.0, \
         'testing_size': 0.0, \
         'eweight': 100.0, \
         'fweight': 1.0, \
         'vweight': 1e-08}}
-    # create a fitsnap object
-    from fitsnap3lib.fitsnap import FitSnap
-    snap = FitSnap()
 
     # get config positions
     snap.scrape_configs()
     data0 = snap.data
     # don't delete the data since we'll use it many times with finite difference
     snap.delete_data = False 
+    # don't check for existing fitsnap objects since we'll be overwriting things
+    snap.pt.check_fitsnap_exist = False
 
     # calculate model forces
 
     snap.process_configs()
-    pt.all_barrier()
+    snap.pt.all_barrier()
     snap.solver.create_datasets()
     (energies_model, forces_model) = snap.solver.evaluate_configs(config_idx=None, standardize_bool=True)
 
     print(f"Length of data: {len(snap.data)}")
 
     # chose a random config to test against
 
@@ -331,11 +307,8 @@
     max_err = np.max(np.abs(percent_errors))
 
     # mean and max percent error should be < 0.001 %
     # max percent error should be < 0.1 %
 
     assert(mean_err < 0.001 and max_err < 0.1)
 
-    del pt
-    del config
-    del snap.data
     del snap
```

