# Comparing `tmp/pyglove-0.3.1.dev20230519.tar.gz` & `tmp/pyglove-0.3.1.dev20230520.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyglove-0.3.1.dev20230519.tar", last modified: Fri May 19 08:06:23 2023, max compression
+gzip compressed data, was "pyglove-0.3.1.dev20230520.tar", last modified: Sat May 20 08:06:29 2023, max compression
```

## Comparing `pyglove-0.3.1.dev20230519.tar` & `pyglove-0.3.1.dev20230520.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-19 08:06:21.000000 pyglove-0.3.1.dev20230519/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove/core/detouring/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/geno/
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/random_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/space.py
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/space_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/logging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.266333 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/patching/
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based.py
--rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22322 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25881 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor.py
--rw-r--r--   0 runner    (1001) docker     (123)    29009 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    30859 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    74985 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/pure_symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.270333 pyglove-0.3.1.dev20230519/pyglove/core/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/core/typing/
--rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    48921 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/custom_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/pytype_support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    79219 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.274333 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators.py
--rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:06:23.262333 pyglove-0.3.1.dev20230519/pyglove.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-19 08:06:23.000000 pyglove-0.3.1.dev20230519/pyglove.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 08:06:23.278333 pyglove-0.3.1.dev20230519/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-19 08:06:12.000000 pyglove-0.3.1.dev20230519/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove/core/detouring/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.902125 pyglove-0.3.1.dev20230520/pyglove/core/geno/
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64370 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38561 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8330 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/space_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.902125 pyglove-0.3.1.dev20230520/pyglove/core/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23216 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22812 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22325 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/logging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21150 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13083 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/patching/
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17894 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.906125 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69750 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22447 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57913 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11911 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28989 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51901 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77608 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/pure_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/core/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17756 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/core/typing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49302 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25636 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/custom_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/pytype_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79366 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103891 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.910125 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50090 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29936 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17424 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40354 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19290 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21312 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11244 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 08:06:29.898125 pyglove-0.3.1.dev20230520/pyglove.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-20 08:06:29.000000 pyglove-0.3.1.dev20230520/pyglove.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 08:06:29.914126 pyglove-0.3.1.dev20230520/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-20 08:06:18.000000 pyglove-0.3.1.dev20230520/setup.py
```

### Comparing `pyglove-0.3.1.dev20230519/LICENSE` & `pyglove-0.3.1.dev20230520/LICENSE`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/PKG-INFO` & `pyglove-0.3.1.dev20230520/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230519
+Version: 0.3.1.dev20230520
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230519/README.md` & `pyglove-0.3.1.dev20230520/README.md`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/detouring/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/detouring/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour.py` & `pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/detouring/class_detour_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/detouring/class_detour_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/base.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/categorical_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/custom.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/custom_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/deduping_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/deduping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/dna_generator_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/dna_generator_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/numerical_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/random.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/random.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/random_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/random_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/space.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/space.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/space_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/space_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/geno/sweeping_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/geno/sweeping_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/base.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/categorical_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/categorical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/custom_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/custom_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/derived_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/derived_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/dynamic_evaluation_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/dynamic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/evolvable_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/evolvable_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/iter_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/iter_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/numerical_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/numerical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/hyper/object_template_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/hyper/object_template_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/logging.py` & `pyglove-0.3.1.dev20230520/pyglove/core/logging.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/logging_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/logging_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/codegen_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/codegen_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/common_traits_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/common_traits_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/docstr_utils_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/docstr_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/formatting_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/formatting_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/hierarchical_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/hierarchical_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/missing_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/thread_local_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/thread_local_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/object_utils/value_location_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/object_utils/value_location_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/object_factory_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/object_factory_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/pattern_based_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/pattern_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/patching/rule_based_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/patching/rule_based_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,11 +123,14 @@
 from pyglove.core.symbolic.base import default_save_handler
 from pyglove.core.symbolic.list import mark_as_insertion
 
 # Error types.
 from pyglove.core.symbolic.base import WritePermissionError
 
 # TODO(daiyip): internal dependencies, remove later.
-from pyglove.core.symbolic.schema_utils import update_schema
 from pyglove.core.symbolic.schema_utils import formalize_schema
+from pyglove.core.symbolic.schema_utils import augment_schema
+from pyglove.core.symbolic.schema_utils import function_schema
+from pyglove.core.symbolic.schema_utils import update_schema
+
 
 # pylint: enable=g-bad-import-order
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,11 +159,9 @@
         value._sym_attributes,  # pylint: disable=protected-access
         allow_partial=allow_partial,
         child_transform=_freeze_field)
 
   if init_arg_list is not None:
     schema_utils.validate_init_arg_list(init_arg_list, cls.schema)
     cls.schema.metadata['init_arg_list'] = init_arg_list
-  setattr(cls, '__serialization_key__', serialization_key or cls.type_name)
-  schema_utils.register_serialization_keys(
-      cls, serialization_key, additional_keys)
+  cls.register_for_deserialization(serialization_key, additional_keys)
   return cls
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/boilerplate_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/boilerplate_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,18 @@
     # `user_cls` will be used.
     use_symbolic_comparison = use_symbolic_comp
 
     # Do not infer symbolic fields from annotations. This is because that
     # symbolic fields are inspected from the `__init__`` signature.
     infer_symbolic_fields_from_annotations = False
 
+    # ClassWrapper's schema will be based inspected based on __init__ instead
+    # of annotations.
+    auto_schema = False
+
   cls = SubclassedWrapper
   cls.__name__ = class_name or user_cls.__name__
   cls.__module__ = module_name or user_cls.__module__
   cls.__doc__ = user_cls.__doc__
 
   # Enable automatic registration for subclass.
   cls.auto_register = True
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/class_wrapper_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/class_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/dict_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/dict_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/diff_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/diff_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/flags_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/flags_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,56 @@
 # limitations under the License.
 """Symbolic function (Functor)."""
 
 import abc
 import functools
 import inspect
 
+import types
 import typing
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import object as pg_object
 from pyglove.core.symbolic import schema_utils
 
 
-class Functor(pg_object.Object, object_utils.Functor):
+class FunctorMeta(pg_object.ObjectMeta):
+  """Functor meta class."""
+
+  def _on_schema_update(cls) -> None:   # pylint: disable=no-self-argument
+    super()._on_schema_update()
+    cls._update_init_signature()
+    cls._update_call_signature()
+
+  def _update_call_signature(cls) -> None:  # pylint: disable=no-self-argument
+    """Updates call signature."""
+    call_signature = pg_typing.Signature.from_schema(
+        cls.schema, name='__call__',
+        module_name=cls.__module__, qualname=cls.__qualname__,
+        is_method=False)
+    setattr(cls, 'signature', call_signature)
+
+  def _update_init_signature(cls) -> None:  # pylint: disable=no-self-argument
+    """Updates __init__ signature."""
+    init_signature = pg_typing.Signature.from_schema(
+        cls.schema, name='__init__',
+        module_name=cls.__module__, qualname=cls.__qualname__)
+
+    pseudo_init = init_signature.make_function(['pass'])
+    @functools.wraps(pseudo_init)
+    def _init(self, *args, **kwargs):
+      Functor.__init__(self, *args, **kwargs)
+    setattr(cls, '__init__', _init)
+
+
+class Functor(pg_object.Object, object_utils.Functor, metaclass=FunctorMeta):
   """Symbolic functions (Functors).
 
   A symbolic function is a symbolic class with a ``__call__`` method, whose
   arguments can be bound partially, incrementally bound by attribute
   assignment, or provided at call time.
 
   Another useful trait is that a symbolic function is serializable, when
@@ -68,14 +98,19 @@
   # Allow assignment on symbolic attributes.
   allow_symbolic_assignment = True
 
   # Do not infer symbolic fields from annotations, since functors are
   # created from function definition which does not have class-level attributes.
   infer_symbolic_fields_from_annotations = False
 
+  # Functor's schema will be inferred from the function signature based on
+  # `pg.functor` or `pg.symbolize`. Therefore we do not infer the schema
+  # automatically during class creation.
+  auto_schema = False
+
   # Signature of this function.
   signature: pg_typing.Signature
 
   def __new__(cls, *args, **kwargs):
     instance = object.__new__(cls)
     if flags.should_call_functors_during_init():
       instance.__init__(*args, **kwargs)
@@ -297,16 +332,19 @@
     assert len(keyword_args) == len(self._specified_args)
 
     # Work out varargs when positional arguments are provided.
     varargs = None
     if self.signature.has_varargs:
       varargs = list(args[len(self.signature.args):])
       if flags.is_type_check_enabled():
-        varargs = self.signature.varargs.value_spec.apply(
-            varargs, root_path=self.sym_path + self.signature.varargs.name)
+        varargs = [
+            self.signature.varargs.value_spec.apply(
+                v, root_path=self.sym_path + self.signature.varargs.name)
+            for v in varargs
+        ]
       args = args[:len(self.signature.args)]
 
     # Convert positional arguments to keyword arguments so we can map them back
     # later.
     for i in range(len(args)):
       arg_spec = self.signature.args[i]
       arg_name = arg_spec.name
@@ -442,21 +480,21 @@
       fn, args, returns,
       base_class=base_class,
       add_to_registry=True,
       **kwargs)
 
 
 def functor_class(
-    func: Callable,  # pylint: disable=g-bare-generic
+    func: types.FunctionType,
     args: Optional[List[Union[
         Tuple[Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
         Tuple[Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any]]]
     ] = None,   # pylint: disable=bad-continuation
     returns: Optional[pg_typing.ValueSpec] = None,
-    base_class: Optional[Type['Functor']] = None,
+    base_class: Optional[Type[Functor]] = None,
     *,
     auto_doc: bool = False,
     auto_typing: bool = False,
     serialization_key: Optional[str] = None,
     additional_keys: Optional[List[str]] = None,
     add_to_registry: bool = False,
 ) -> Type[Functor]:
@@ -486,23 +524,24 @@
       python functions, instead of being set at `schema.Field` level. But
       validation rules can be set using `args` and apply to argument values.
       For example::
 
           @pg.functor([('c', pg.typing.Int(min_value=0), 'Arg c')])
           def foo(a, b, c=1, **kwargs):
             return a + b + c + sum(kwargs.values())
-            assert foo.schema.fields() == [
-                pg.typing.Field('a', pg.Any(), 'Argument a'.),
-                pg.typing.Field('b', pg.Any(), 'Argument b'.),
-                pg.typing.Field('c', pg.typing.Int(), 'Arg c.),
-                pg.typing.Filed(
-                    pg.typing.StrKey(), pg.Any(), 'Other arguments.')
-            ]
-            # Prebind a=1, b=2, with default value c=1.
-            assert foo(1, 2)() == 4
+          
+          assert foo.schema.fields() == [
+              pg.typing.Field('a', pg.Any(), 'Argument a'.),
+              pg.typing.Field('b', pg.Any(), 'Argument b'.),
+              pg.typing.Field('c', pg.typing.Int(), 'Arg c.),
+              pg.typing.Filed(
+                  pg.typing.StrKey(), pg.Any(), 'Other arguments.')
+          ]
+          # Prebind a=1, b=2, with default value c=1.
+          assert foo(1, 2)() == 4
 
     returns: Optional schema specification for the return value.
     base_class: Optional base class (derived from `symbolic.Functor`).
       If None, returned type will inherit from `Functor` directly.
     auto_doc: If True, the descriptions of argument fields will be inherited
       from funciton docstr if they are not explicitly specified through
       ``args``.
@@ -527,118 +566,39 @@
     KeyError: names of symbolic arguments are not compatible with
       function signature.
     TypeError: types of symbolic arguments are not compatible with
       function signature.
     ValueError: default values of symbolic arguments are not compatible
       with  function signature.
   """
-  args_docstr = None
-  description = None
-  if auto_doc:
-    docstr = object_utils.docstr(func)
-    if docstr:
-      args_docstr = docstr.args
-      description = schema_utils.schema_description_from_docstr(docstr)
-
-  signature = pg_typing.get_signature(func, auto_typing=auto_typing)
-  arg_fields = pg_typing.get_arg_fields(signature, args, args_docstr)
-  if returns is not None and pg_typing.MISSING_VALUE != returns.default:
-    raise ValueError('return value spec should not have default value.')
 
-  base_class = base_class or Functor
-
-  class _Functor(base_class):
+  class _Functor(base_class or Functor):
     """Functor wrapper for input function."""
 
-    # Disable auto register so we can use function module and name
-    # for registration later.
-    auto_register = False
-
     def _call(self, *args, **kwargs):
       return func(*args, **kwargs)
 
-  cls = _Functor
-  cls.__name__ = signature.name
-  cls.__qualname__ = signature.qualname
-  cls.__module__ = signature.module_name
+  cls = typing.cast(Type[Functor], _Functor)
+  cls.__name__ = func.__name__
+  cls.__qualname__ = func.__qualname__
+  cls.__module__ = getattr(func, '__module__', 'wrapper')
   cls.__doc__ = func.__doc__
 
   # Enable automatic registration for subclass.
-  cls.auto_register = True  # pylint: disable=protected-access
+  cls.auto_register = True
 
-  # Generate init_arg_list from signature.
-  init_arg_list = [arg.name for arg in signature.args]
-  if signature.varargs:
-    init_arg_list.append(f'*{signature.varargs.name}')
-  schema_utils.update_schema(
-      cls,
-      arg_fields,
-      init_arg_list=init_arg_list,
-      description=description,
-      serialization_key=serialization_key,
-      additional_keys=additional_keys,
-      add_to_registry=add_to_registry)
-
-  # Update signature with symbolic value specs.
-  def _value_spec_by_name(name: str):
-    field = cls.schema.get_field(name)  # pytype: disable=attribute-error  # re-none
-    assert field is not None
-    return field.value
-  varkw_field = cls.schema.dynamic_field  # pytype: disable=attribute-error  # re-none
-  assert signature.has_varkw == (varkw_field is not None), varkw_field
-  signature = pg_typing.Signature(
-      callable_type=signature.callable_type,
-      name=signature.name,
-      module_name=signature.module_name,
-      qualname=signature.qualname,
-      args=[
-          pg_typing.Argument(arg.name, _value_spec_by_name(arg.name))
-          for arg in signature.args
-      ],
-      kwonlyargs=[
-          pg_typing.Argument(arg.name, _value_spec_by_name(arg.name))
-          for arg in signature.kwonlyargs
-      ],
-      varargs=(
-          pg_typing.Argument(signature.varargs.name,
-                             _value_spec_by_name(signature.varargs.name))
-          if signature.varargs else None),
-      varkw=(pg_typing.Argument(signature.varkw.name, varkw_field.value)
-             if signature.varkw else None),
-      return_value=returns or signature.return_value)
-  setattr(cls, 'signature', signature)
-
-  # Update signature for the __init__ method.
-  varargs = None
-  if signature.varargs:
-    # For variable positional arguments, PyType uses the element type as
-    # anntoation. Therefore we need to use the element type to generate
-    # the right annotation.
-    varargs_spec = signature.varargs.value_spec
-    assert isinstance(varargs_spec, pg_typing.List), varargs_spec
-    varargs = pg_typing.Argument(signature.varargs.name, varargs_spec.element)
-
-  init_signature = pg_typing.Signature(
-      callable_type=pg_typing.CallableType.FUNCTION,
-      name='__init__',
-      module_name=signature.module_name,
-      qualname=f'{signature.name}.__init__',
-      args=[
-          pg_typing.Argument('self', pg_typing.Any())
-      ] + signature.args,
-      kwonlyargs=signature.kwonlyargs,
-      varargs=varargs,
-      varkw=signature.varkw)
-  pseudo_init = init_signature.make_function(['pass'])
-
-  @functools.wraps(pseudo_init)
-  def _init(self, *args, **kwargs):
-    Functor.__init__(self, *args, **kwargs)
-  setattr(cls, '__init__', _init)
-  return cls  # pytype: disable=bad-return-type  # re-none
+  # Apply function schema.
+  schema = schema_utils.function_schema(
+      func, args, returns, auto_doc=auto_doc, auto_typing=auto_typing)
+  cls.apply_schema(schema)
+
+  # Register functor class for deserialization if needed.
+  if add_to_registry:
+    cls.register_for_deserialization(serialization_key, additional_keys)
+  return cls
 
 
 def as_functor(
     func: Callable,  # pylint: disable=g-bare-generic
     ignore_extra_args: bool = False) -> Functor:
   """Make a functor object from a regular python function.
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/functor_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/functor_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         ])
     self.assertEqual(f.signature.args, [
         pg_typing.Argument('a', pg_typing.Any()),
         pg_typing.Argument('b', pg_typing.Any())
     ])
     self.assertEqual(
         f.signature.varargs,
-        pg_typing.Argument('args', pg_typing.List(pg_typing.Any(), default=[])))
+        pg_typing.Argument('args', pg_typing.Any()))
     self.assertEqual(
         f.signature.varkw, pg_typing.Argument('kwargs', pg_typing.Any()))
     self.assertEqual(
         f.signature.kwonlyargs,
         [pg_typing.Argument('c', pg_typing.Any(default=0))])
     self.assertIsNone(f.signature.return_value, None)
     self.assertTrue(f.signature.has_varargs)
@@ -175,15 +175,15 @@
             pg_typing.Field(pg_typing.StrKey(), pg_typing.Any()),
         ])
     self.assertEqual(
         f.signature.args,
         [pg_typing.Argument('a', pg_typing.Int())])
     self.assertEqual(
         f.signature.varargs,
-        pg_typing.Argument('args', pg_typing.List(pg_typing.Any(), default=[])))
+        pg_typing.Argument('args', pg_typing.Any()))
     self.assertEqual(
         f.signature.kwonlyargs,
         [pg_typing.Argument('b', pg_typing.Int(default=2))])
     self.assertEqual(
         f.signature.varkw,
         pg_typing.Argument('kwargs', pg_typing.Any()))
     self.assertEqual(f.signature.return_value, pg_typing.Int())
@@ -259,14 +259,15 @@
         ('b', pg_typing.Int(max_value=10)),
         ('args', pg_typing.List(pg_typing.Int())),
         (pg_typing.StrKey(), pg_typing.Int(max_value=5))
     ], returns=pg_typing.Int(min_value=0))
     def f(a, *args, b, **kwargs):
       return a + b + sum(args) + sum(kwargs.values())
 
+    print('SIGNATURE', f.signature)
     self.assertEqual(f(1, 2, b=3)(c=4), 10)
 
     # Validate during pre-binding.
     with self.assertRaisesRegex(
         ValueError, 'Value -1 is out of range .*min=0'):
       f(-1, b=1)
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/list_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/list_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import typing
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import dict as pg_dict
+from pyglove.core.symbolic import flags
 from pyglove.core.symbolic import schema_utils
 
 
 class ObjectMeta(abc.ABCMeta):
   """Meta class for pg.Object."""
 
   @property
@@ -54,15 +55,165 @@
   def serialization_key(cls) -> str:
     """Gets serialization type key."""
     return getattr(cls, '__serialization_key__')
 
   @property
   def init_arg_list(cls) -> List[str]:
     """Gets __init__ positional argument list."""
-    return cls.schema.metadata['init_arg_list']
+    return typing.cast(List[str], cls.schema.metadata['init_arg_list'])
+
+  def apply_schema(cls, schema: pg_typing.Schema) -> None:
+    """Applies a schema to a symbolic class.
+
+    Args:
+      schema: The schema that will be applied to class. If `cls` was attached
+        with an existing schema. The old schema will be dropped.
+    """
+    setattr(cls, '__schema__', schema)
+    setattr(cls, '__sym_fields', pg_typing.Dict(schema))
+
+    # Update `init_arg_list`` based on the updated schema.
+    init_arg_list = schema.metadata.get('init_arg_list', None)
+    if init_arg_list is None:
+      init_arg_list = schema_utils.auto_init_arg_list(cls)
+      cls.schema.metadata['init_arg_list'] = init_arg_list
+    schema_utils.validate_init_arg_list(init_arg_list, cls.schema)
+    cls._on_schema_update()  # pylint: disable=no-value-for-parameter
+
+  def register_for_deserialization(
+      cls,
+      serialization_key: Optional[str] = None,
+      additional_keys: Optional[List[str]] = None,
+  ) -> None:
+    """Register current symbolic class for deserialization."""
+    serialization_key = serialization_key or cls.type_name
+    setattr(cls, '__serialization_key__', serialization_key)
+
+    serialization_keys = []
+    serialization_keys.append(serialization_key)
+    serialization_keys.extend(additional_keys or [])
+    if cls.type_name not in serialization_keys:
+      serialization_keys.append(cls.type_name)
+
+    # Register class with 'type' property.
+    for key in serialization_keys:
+      object_utils.JSONConvertible.register(
+          key, cls, flags.is_repeated_class_registration_allowed()
+      )
+
+  def _on_schema_update(cls):
+    """Triggers when the schema for the class has been updated."""
+    # Update the default value for each field after schema is updated. This is
+    # because that users may change a field's default value via class attribute.
+    cls._update_default_values_from_class_attributes()  # pylint: disable=no-value-for-parameter
+
+    # Update the signature of __init__.
+    cls._update_init_signature_based_on_schema()  # pylint: disable=no-value-for-parameter
+
+    # Expose symbolic attributes as object attributes when being asked.
+    if cls.allow_symbolic_attribute:  # pytype: disable=attribute-error
+      cls._generate_sym_attributes()  # pylint: disable=no-value-for-parameter
+
+  def _infer_fields_from_annotations(cls) -> List[pg_typing.Field]:
+    """Infers symbolic fields from class annotations."""
+    if not cls.infer_symbolic_fields_from_annotations:  # pytype: disable=attribute-error
+      return []
+
+    # NOTE(daiyip): refer to https://docs.python.org/3/howto/annotations.html.
+    if hasattr(inspect, 'get_annotations'):
+      annotations = inspect.get_annotations(cls)
+    else:
+      annotations = cls.__dict__.get('__annotations__', {})
+
+    fields = []
+    for attr_name, attr_annotation in annotations.items():
+      if attr_name == '__kwargs__':
+        # __kwargs__ is speical annotation for enabling keyword arguments.
+        key = pg_typing.StrKey()
+      elif not attr_name.isupper() and not attr_name.startswith('_'):
+        key = pg_typing.ConstStrKey(attr_name)
+      else:
+        # We consider class-level attributes in upper cases non-fields even
+        # when they appear with annotations.
+        key = None
+
+      if key is None:
+        continue
+
+      field = pg_typing.Field.from_annotation(key, attr_annotation)
+      if isinstance(key, pg_typing.ConstStrKey):
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if attr_value != pg_typing.MISSING_VALUE:
+          field.value.set_default(attr_value)
+      fields.append(field)
+    return fields
+
+  def _update_init_signature_based_on_schema(cls):
+    """Updates the signature of `__init__` if needed."""
+    if cls.__init__ is not Object.__init__ and not hasattr(
+        cls.__init__, '__sym_generated_init__'
+    ):
+      # We only generate `__init__` from pg.Object subclass which does not
+      # override the `__init__` method.
+      # Functor and ClassWrapper override their `__init__` methods, therefore
+      # they need to synchronize the __init__ signature by themselves.
+      return
+    signature = pg_typing.Signature.from_schema(
+        cls.schema, cls.__module__, '__init__', f'{cls.__name__}.__init__'
+    )
+    pseudo_init = signature.make_function(['pass'])
+
+    # Create a new `__init__` that passes through all the arguments to
+    # in `pg.Object.__init__`. This is needed for each class to use different
+    # signature.
+    @functools.wraps(pseudo_init)
+    def _init(self, *args, **kwargs):
+      # We pass through the arguments to `Object.__init__` instead of
+      # `super()` since the parent class uses a generated `__init__` will
+      # be delegated to `Object.__init__` eventually. Therefore, directly
+      # calling `Object.__init__` is equivalent to calling `super().__init__`.
+      Object.__init__(self, *args, **kwargs)
+
+    setattr(_init, '__sym_generated_init__', True)
+    setattr(cls, '__init__', _init)
+
+  def _update_default_values_from_class_attributes(cls):
+    for field in cls.schema.fields.values():
+      if isinstance(field.key, pg_typing.ConstStrKey):
+        attr_name = field.key.text
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if (
+            attr_value != pg_typing.MISSING_VALUE
+            and not isinstance(attr_value, property)
+            and not inspect.isfunction(attr_value)
+        ):
+          field.value.set_default(attr_value)
+
+  def _generate_sym_attributes(cls):
+    """Generates symbolic attributes based on schema if they are enabled."""
+
+    def _create_sym_attribute(attr_name, field):
+      return property(
+          object_utils.make_function(
+              attr_name,
+              ['self'],
+              [f"return self._sym_attributes['{attr_name}']"],
+              return_type=field.value.annotation,
+          )
+      )
+
+    for key, field in cls.schema.fields.items():
+      if isinstance(key, pg_typing.ConstStrKey):
+        attr_name = str(key)
+        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
+        if attr_value == pg_typing.MISSING_VALUE or (
+            not inspect.isfunction(attr_value)
+            and not isinstance(attr_value, property)
+        ):
+          setattr(cls, attr_name, _create_sym_attribute(attr_name, field))
 
 
 # Use ObjectMeta as meta class to inherit schema and type_name property.
 class Object(base.Symbolic, metaclass=ObjectMeta):
   """Base class for symbolic user classes.
 
   PyGlove allow symbolic programming interfaces to be easily added to most
@@ -145,151 +296,56 @@
   #
   #     class A(pg.Object):
   #        x: int
   #        y: str
   #
   # Please note that class attributes in UPPER_CASE or starting with '_' will
   # not be considered as symbolic fields even if they have annotations.
-
   infer_symbolic_fields_from_annotations = True
 
+  # Automatically infer schema during subclass creation time.
+  auto_schema = True
+
   @classmethod
   def __init_subclass__(cls):
     super().__init_subclass__()
 
-    # Inherit schema from base classes that have schema
-    # in the ordered of inheritance.
-    # TODO(daiyip): size of base_schema_list can be reduced
-    # by looking at their inheritance chains.
-    base_schema_list = []
-    for base_cls in cls.__bases__:
-      base_schema = getattr(base_cls, 'schema', None)
-      if isinstance(base_schema, pg_typing.Schema):
-        base_schema_list.append(base_schema)
-
-    cls_schema = schema_utils.formalize_schema(
-        pg_typing.create_schema(
-            maybe_field_list=cls._infer_fields_from_annotations(),
-            name=cls.type_name,
-            base_schema_list=base_schema_list,
-            allow_nonconst_keys=True,
-            metadata={}))
-    setattr(cls, '__schema__', cls_schema)
-    setattr(cls, '__sym_fields', pg_typing.Dict(cls_schema))
-    setattr(cls, '__serialization_key__', cls.type_name)
-    cls_schema.metadata['init_arg_list'] = schema_utils.auto_init_arg_list(cls)
-
-    # Trigger schema update event.
-    cls._on_schema_update()
-
-  @classmethod
-  def _infer_fields_from_annotations(cls) -> List[pg_typing.Field]:
-    """Infers symbolic fields from class annotations."""
-    if not cls.infer_symbolic_fields_from_annotations:
-      return []
-
-    # NOTE(daiyip): refer to https://docs.python.org/3/howto/annotations.html.
-    if hasattr(inspect, 'get_annotations'):
-      annotations = inspect.get_annotations(cls)
-    else:
-      annotations = cls.__dict__.get('__annotations__', {})
-
-    fields = []
-    for attr_name, attr_annotation in annotations.items():
-      if attr_name == '__kwargs__':
-        # __kwargs__ is speical annotation for enabling keyword arguments.
-        key = pg_typing.StrKey()
-      elif not attr_name.isupper() and not attr_name.startswith('_'):
-        key = pg_typing.ConstStrKey(attr_name)
-      else:
-        # We consider class-level attributes in upper cases non-fields even
-        # when they appear with annotations.
-        key = None
-
-      if key is None:
-        continue
-
-      field = pg_typing.Field.from_annotation(key, attr_annotation)
-      if isinstance(key, pg_typing.ConstStrKey):
-        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-        if attr_value != pg_typing.MISSING_VALUE:
-          field.value.set_default(attr_value)
-      fields.append(field)
-    return fields
-
-  @classmethod
-  def _on_schema_update(cls):
-    """Triggers when the schema for the class has been updated."""
-    # Update the default value for each field after schema is updated. This is
-    # because that users may change a field's default value via class attribute.
-    cls._update_default_values_from_class_attributes()
-
-    # Update the signature of __init__.
-    cls._update_init_signature_based_on_schema()
-
-    # Expose symbolic attributes as object attributes when being asked.
-    if cls.allow_symbolic_attribute:
-      cls._generate_sym_attributes()
-
-  @classmethod
-  def _update_init_signature_based_on_schema(cls):
-    """Updates the signature of `__init__` if needed."""
-    if (cls.__init__ is not Object.__init__
-        and not hasattr(cls.__init__, '__sym_generated_init__')):
-      # We only generate `__init__` from pg.Object subclass which does not
-      # override the `__init__` method.
-      # Functor and ClassWrapper override their `__init__` methods, therefore
-      # they need to synchronize the __init__ signature by themselves.
-      return
-    signature = pg_typing.get_init_signature(
-        cls.schema, cls.__module__, '__init__', f'{cls.__name__}.__init__')
-    pseudo_init = signature.make_function(['pass'])
-
-    # Create a new `__init__` that passes through all the arguments to
-    # in `pg.Object.__init__`. This is needed for each class to use different
-    # signature.
-    @functools.wraps(pseudo_init)
-    def _init(self, *args, **kwargs):
-      # We pass through the arguments to `Object.__init__` instead of
-      # `super()` since the parent class uses a generated `__init__` will
-      # be delegated to `Object.__init__` eventually. Therefore, directly
-      # calling `Object.__init__` is equivalent to calling `super().__init__`.
-      Object.__init__(self, *args, **kwargs)
-    setattr(_init, '__sym_generated_init__', True)
-    setattr(cls, '__init__', _init)
-
-  @classmethod
-  def _update_default_values_from_class_attributes(cls):
-    for field in cls.schema.fields.values():
-      if isinstance(field.key, pg_typing.ConstStrKey):
-        attr_name = field.key.text
-        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-        if (attr_value != pg_typing.MISSING_VALUE
-            and not isinstance(attr_value, property)
-            and not inspect.isfunction(attr_value)):
-          field.value.set_default(attr_value)
+    if cls.auto_schema:
+      # Inherit schema from base classes that have schema
+      # in the ordered of inheritance.
+      # TODO(daiyip): size of base_schema_list can be reduced
+      # by looking at their inheritance chains.
+      base_schema_list = []
+      for base_cls in cls.__bases__:
+        base_schema = getattr(base_cls, 'schema', None)
+        if isinstance(base_schema, pg_typing.Schema):
+          base_schema_list.append(base_schema)
+
+      new_fields = cls._infer_fields_from_annotations()
+      cls_schema = schema_utils.formalize_schema(
+          pg_typing.create_schema(
+              maybe_field_list=new_fields,
+              name=cls.type_name,
+              base_schema_list=base_schema_list,
+              allow_nonconst_keys=True,
+              metadata={},
+          )
+      )
+
+      # NOTE(daiyip): When new fields are added through class attributes.
+      # We invalidate `init_arg_list` so PyGlove could recompute it based
+      # on its schema during `apply_schema`. Otherwise, we inherit the
+      # `init_arg_list` from the base class.
+      # TODO(daiyip): detect new fields based on the differences from the base
+      # schema.
+      if new_fields:
+        cls_schema.metadata['init_arg_list'] = None
+      cls.apply_schema(cls_schema)
 
-  @classmethod
-  def _generate_sym_attributes(cls):
-    """Generates symbolic attributes based on schema if they are enabled."""
-    def _create_sym_attribute(attr_name, field):
-      return property(object_utils.make_function(
-          attr_name,
-          ['self'],
-          [f'return self._sym_attributes[\'{attr_name}\']'],
-          return_type=field.value.annotation))
-
-    for key, field in cls.schema.fields.items():
-      if isinstance(key, pg_typing.ConstStrKey):
-        attr_name = str(key)
-        attr_value = getattr(cls, attr_name, pg_typing.MISSING_VALUE)
-        if (attr_value == pg_typing.MISSING_VALUE
-            or (not inspect.isfunction(attr_value)
-                and not isinstance(attr_value, property))):
-          setattr(cls, attr_name, _create_sym_attribute(attr_name, field))
+    setattr(cls, '__serialization_key__', cls.type_name)
 
   @classmethod
   def partial(cls, *args, **kwargs) -> 'Object':
     """Class method that creates a partial object of current class."""
     return cls(*args, allow_partial=True, **kwargs)
 
   @classmethod
@@ -813,13 +869,15 @@
     raise TypeError(f'Unsupported keyword arguments: {list(kwargs.keys())!r}.')
 
   def _decorator(cls):
     """Decorator function that registers schema with an Object class."""
     schema_utils.update_schema(
         cls,
         fields,
-        metadata=metadata,
+        extend=True,
         init_arg_list=init_arg_list,
+        metadata=metadata,
         serialization_key=serialization_key,
-        additional_keys=additional_keys)
+        additional_keys=additional_keys,
+    )
     return cls
   return typing.cast(pg_typing.Decorator, _decorator)
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/object_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/object_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,23 +213,29 @@
 
     with self.assertRaisesRegex(
         ValueError, '.* should call `super.*__init__`'):
       _ = B(1)
 
   def test_symbolic_fields_from_annotations(self):
 
-    class A(Object):
+    class X(Object):
+      pass
+
+    self.assertEqual(X.init_arg_list, [])
+
+    class A(X):
       x: int
       y: typing.Annotated[float, 'field y'] = 0.0
       z = 2
       # P is upper-case, thus will not be treated as symbolic field.
       P: int = 1
       # _q starts with _, which will not be treated as symbolic field either.
       _q: int = 2
 
+    self.assertEqual(A.init_arg_list, ['x', 'y'])
     self.assertEqual(
         list(A.schema.fields.keys()),
         ['x', 'y'])
 
     a = A(1)
     self.assertEqual(a.x, 1)
     self.assertEqual(a.y, 0.0)
@@ -239,14 +245,15 @@
     self.assertEqual(a.x, 2)
     self.assertEqual(a.y, 1.0)
 
     class B(A):
       p: str = 'foo'
       q: typing.Any = None
 
+    self.assertEqual(B.init_arg_list, ['x', 'y', 'p', 'q'])
     self.assertEqual(
         list(B.schema.fields.keys()),
         ['x', 'y', 'p', 'q'],
     )
     b = B(1, q=2)
     self.assertEqual(b.x, 1)
     self.assertEqual(b.y, 0.0)
@@ -256,39 +263,54 @@
     @pg_members([
         ('k', pg_typing.Int())
     ])
     class C(B):
       # Override the default value of 'y'.
       y: float = 1.0
 
+    self.assertEqual(
+        list(C.schema.fields.keys()),
+        ['x', 'y', 'p', 'q', 'k'],
+    )
+    self.assertEqual(C.init_arg_list, ['x', 'y', 'p', 'q', 'k'])
+
     c = C(1, q=2, k=3)
     self.assertEqual(c.x, 1)
     self.assertEqual(c.y, 1.0)
     self.assertEqual(c.q, 2)
     self.assertEqual(c.k, 3)
 
     @pg_members([
         ('e', pg_typing.Int())
     ])
     class D(C):
       f: int = 5
 
+    self.assertEqual(D.init_arg_list, ['x', 'y', 'p', 'q', 'k', 'f', 'e'])
+    self.assertEqual(
+        list(D.schema.fields.keys()),
+        ['x', 'y', 'p', 'q', 'k', 'f', 'e'],
+    )
     d = D(1, q=2, k=3, e=4)
     self.assertEqual(d.x, 1)
     self.assertEqual(d.y, 1.0)
     self.assertEqual(d.q, 2)
     self.assertEqual(d.k, 3)
     self.assertEqual(d.e, 4)
     self.assertEqual(d.f, 5)
 
     class E(Object):
       __kwargs__: typing.Any
       x: int
 
-    self.assertIsNotNone(E.schema.dynamic_field)
+    self.assertEqual(E.init_arg_list, ['x'])
+    self.assertEqual(
+        list(E.schema.fields.keys()),
+        [pg_typing.StrKey(), 'x'],
+    )
     e = E(1, y=3)
     self.assertEqual(e.x, 1)
     self.assertEqual(e.y, 3)
 
   def test_update_of_default_values(self):
 
     class A(Object):
@@ -1666,25 +1688,90 @@
 
     self.assertEqual(
         signature.parameters['x'].kind,
         inspect.Parameter.KEYWORD_ONLY)
     self.assertEqual(signature.parameters['x'].annotation, int)
     self.assertEqual(signature.parameters['x'].default, 1)
 
+  def test_user_specified_init_arg_list_with_metadata(self):
+
+    @pg_members([
+        ('x', pg_typing.Int(default=1)),
+        ('y', pg_typing.Any()),
+        ('z', pg_typing.List(pg_typing.Int())),
+    ], metadata=dict(init_arg_list=['y', '*z']))
+    class B(Object):
+      pass
+
+    signature = inspect.signature(B.__init__)
+    self.assertEqual(
+        list(signature.parameters.keys()), ['self', 'y', 'z', 'x'])
+
+    self.assertEqual(
+        signature.parameters['self'].kind,
+        inspect.Parameter.POSITIONAL_OR_KEYWORD)
+    self.assertEqual(
+        signature.parameters['self'].annotation,
+        inspect.Signature.empty)
+    self.assertEqual(
+        signature.parameters['self'].default,
+        inspect.Signature.empty)
+
+    self.assertEqual(
+        signature.parameters['y'].kind,
+        inspect.Parameter.POSITIONAL_OR_KEYWORD)
+    self.assertEqual(
+        signature.parameters['y'].annotation, inspect.Signature.empty)
+    self.assertEqual(
+        signature.parameters['y'].default, inspect.Signature.empty)
+
+    self.assertEqual(
+        signature.parameters['z'].kind,
+        inspect.Parameter.VAR_POSITIONAL)
+    self.assertEqual(
+        signature.parameters['z'].annotation, int)
+    self.assertEqual(
+        signature.parameters['z'].default, inspect.Signature.empty)
+
+    self.assertEqual(
+        signature.parameters['x'].kind,
+        inspect.Parameter.KEYWORD_ONLY)
+    self.assertEqual(signature.parameters['x'].annotation, int)
+    self.assertEqual(signature.parameters['x'].default, 1)
+
+  def test_custom_init(self):
+
+    @pg_members([
+        ('x', pg_typing.Int(default=1)),
+        ('y', pg_typing.Any()),
+        ('z', pg_typing.List(pg_typing.Int())),
+    ], init_arg_list=['y', '*z'])
+    class B(Object):
+      pass
+
     class C(B):
       """Custom __init__."""
 
       def __init__(self, a, b):
         super().__init__(b, x=a)
 
     signature = inspect.signature(C.__init__)
     self.assertEqual(
         list(signature.parameters.keys()), ['self', 'a', 'b'])
 
-    # Bad cases:
+  def test_bad_init_arg_list(self):
+
+    @pg_members([
+        ('x', pg_typing.Int(default=1)),
+        ('y', pg_typing.Any()),
+        ('z', pg_typing.List(pg_typing.Int())),
+    ], init_arg_list=['y', '*z'])
+    class B(Object):
+      pass
+
     with self.assertRaisesRegex(
         TypeError, 'Argument .* from `init_arg_list` is not defined.'):
 
       @pg_members([], init_arg_list=['a'])
       class D(B):  # pylint: disable=unused-variable
         pass
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/origin_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/origin_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/pure_symbolic.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/pure_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,36 +9,104 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Utilities for handling schema for symbolic classes."""
 
+import types
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from pyglove.core import object_utils
 from pyglove.core import typing as pg_typing
 from pyglove.core.symbolic import base
 from pyglove.core.symbolic import flags
 
 
+def augment_schema(
+    schema: pg_typing.Schema,
+    fields: List[
+        Union[
+            pg_typing.Field,
+            Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
+            Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any],
+        ]
+    ],
+    extend: bool = True,
+    *,
+    init_arg_list: Optional[Sequence[str]] = None,
+    metadata: Optional[Dict[str, Any]] = None,
+    description: Optional[str] = None,
+) -> pg_typing.Schema:
+  """Gets the augmented schema from class with extra fields and metadata.
+
+  Args:
+    schema: The original schema.
+    fields: A list of `pg.typing.Field` or equivalent tuple representation as
+      (<key>, <value-spec>, [description], [metadata-objects]). `key` should be
+      a string. `value-spec` should be pg_typing.ValueSpec classes or
+      equivalent, e.g. primitive values which will be converted to ValueSpec
+      implementation according to its type and used as its default value.
+      `description` is optional only when field overrides a field from its
+      parent class. `metadata-objects` is an optional list of any type, which
+      can be used to generate code according to the schema.
+    extend: If True, extend existing schema using `fields`. Otherwise replace
+      existing schema with a new schema created from `fields`.
+    init_arg_list: An optional sequence of strings as the positional argument
+      list for `__init__`. This is helpful when symbolic attributes are
+      inherited from base classes or the user want to change its order. If not
+      provided, the `init_arg_list` will be automatically generated from
+      symbolic attributes defined from ``pg.members`` in their declaration
+      order, from the base classes to the subclass.
+    metadata: Optional dict of user objects as class-level metadata which will
+      be attached to class schema.
+    description: An optional description to set.
+
+  Returns:
+    The augmented schema (new copy).
+  """
+  metadata = metadata or {}
+  if init_arg_list is None:
+    init_arg_list = metadata.get('init_arg_list', None)
+  metadata = object_utils.merge([schema.metadata, metadata])
+
+  # NOTE(daiyip): Consider to inherit `init_arg_list` from the parent when
+  # there is no new field.
+  metadata['init_arg_list'] = init_arg_list
+
+  return formalize_schema(
+      pg_typing.create_schema(
+          maybe_field_list=fields,
+          name=schema.name,
+          base_schema_list=[schema] if extend else [],
+          description=description or schema.description,
+          allow_nonconst_keys=True,
+          metadata=metadata,
+      )
+  )
+
+
 def update_schema(
     cls,
-    fields: List[Union[
-        pg_typing.Field,
-        Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
-        Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any]]],
-    metadata: Optional[Dict[str, Any]] = None,
-    init_arg_list: Optional[Sequence[str]] = None,
-    *,
+    fields: List[
+        Union[
+            pg_typing.Field,
+            Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
+            Tuple[Union[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any],
+        ]
+    ],
     extend: bool = True,
+    *,
+    init_arg_list: Optional[Sequence[str]] = None,
+    metadata: Optional[Dict[str, Any]] = None,
     description: Optional[str] = None,
     serialization_key: Optional[str] = None,
     additional_keys: Optional[List[str]] = None,
-    add_to_registry: bool = True) -> None:
+    add_to_registry: bool = True,
+) -> None:
   """Updates the schema for a ``pg.Object`` subclass.
 
   This function allows the user to update the symbolic fields associated
   with a symbolic class. It was intended to support meta-programming
   scenarios in which symbolic fields are dynamically generated.
 
   Example::
@@ -67,63 +135,104 @@
       (<key>, <value-spec>, [description], [metadata-objects]). `key` should be
       a string. `value-spec` should be pg_typing.ValueSpec classes or
       equivalent, e.g. primitive values which will be converted to ValueSpec
       implementation according to its type and used as its default value.
       `description` is optional only when field overrides a field from its
       parent class. `metadata-objects` is an optional list of any type, which
       can be used to generate code according to the schema.
-    metadata: Optional dict of user objects as class-level metadata which will
-      be attached to class schema.
+    extend: If True, extend existing schema using `fields`. Otherwise replace
+      existing schema with a new schema created from `fields`.
     init_arg_list: An optional sequence of strings as the positional argument
       list for `__init__`. This is helpful when symbolic attributes are
-      inherited from base classes or the user want to change its order.
-      If not provided, the `init_arg_list` will be automatically generated
-      from symbolic attributes defined from ``pg.members`` in their declaration
+      inherited from base classes or the user want to change its order. If not
+      provided, the `init_arg_list` will be automatically generated from
+      symbolic attributes defined from ``pg.members`` in their declaration
       order, from the base classes to the subclass.
-    extend: If True, extend existing schema using `fields`. Otherwise replace
-      existing schema with a new schema created from `fields`.
+    metadata: Optional dict of user objects as class-level metadata which will
+      be attached to class schema.
     description: An optional description to set.
     serialization_key: An optional string to be used as the serialization key
       for the class during `sym_jsonify`. If None, `cls.type_name` will be used.
       This is introduced for scenarios when we want to relocate a class, before
       the downstream can recognize the new location, we need the class to
       serialize it using previous key.
     additional_keys: An optional list of strings as additional keys to
-      deserialize an object of the registered class. This can be useful
-      when we need to relocate or rename the registered class while being able
-      to load existing serialized JSON values.
+      deserialize an object of the registered class. This can be useful when we
+      need to relocate or rename the registered class while being able to load
+      existing serialized JSON values.
     add_to_registry: If True, the newly created functor class will be added to
       the registry for deserialization.
   """
-  metadata = metadata or {}
-  cls_schema = formalize_schema(
-      pg_typing.create_schema(
-          maybe_field_list=fields,
-          name=cls.type_name,
-          base_schema_list=[cls.schema] if extend else [],
-          allow_nonconst_keys=True,
-          metadata=metadata))
+  cls.apply_schema(
+      augment_schema(
+          cls.schema,
+          fields=fields,
+          extend=extend,
+          init_arg_list=init_arg_list,
+          metadata=metadata,
+          description=description,
+      )
+  )
 
-  setattr(cls, '__schema__', cls_schema)
-  setattr(cls, '__sym_fields', pg_typing.Dict(cls_schema))
-  setattr(cls, '__serialization_key__', serialization_key or cls.type_name)
-
-  if init_arg_list is None:
-    init_arg_list = metadata.pop('init_arg_list', auto_init_arg_list(cls))
-  validate_init_arg_list(init_arg_list, cls_schema)
-  cls_schema.metadata['init_arg_list'] = init_arg_list
+  if add_to_registry:
+    cls.register_for_deserialization(serialization_key, additional_keys)
 
-  if description is not None:
-    cls_schema.set_description(description)
 
-  cls._on_schema_update()  # pylint: disable=protected-access
+def function_schema(
+    func: types.FunctionType,
+    args: Optional[
+        List[
+            Union[
+                Tuple[Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str],
+                Tuple[
+                    Tuple[str, pg_typing.KeySpec], pg_typing.ValueSpec, str, Any
+                ],
+            ]
+        ]
+    ] = None,  # pylint: disable=bad-continuation
+    returns: Optional[pg_typing.ValueSpec] = None,
+    *,
+    auto_typing: bool = True,
+    auto_doc: bool = True,
+) -> pg_typing.Schema:
+  """Returns the schema from the signature of a function."""
+  args_docstr = None
+  description = None
+  if auto_doc:
+    docstr = object_utils.docstr(func)
+    if docstr:
+      args_docstr = docstr.args
+      description = schema_description_from_docstr(docstr)
+
+  signature = pg_typing.get_signature(func, auto_typing=auto_typing)
+  arg_fields = pg_typing.get_arg_fields(signature, args, args_docstr)
+
+  if returns is not None and pg_typing.MISSING_VALUE != returns.default:
+    raise ValueError('return value spec should not have default value.')
+  returns = returns or signature.return_value
+
+  # Generate init_arg_list from signature.
+  init_arg_list = [arg.name for arg in signature.args]
+  if signature.varargs:
+    init_arg_list.append(f'*{signature.varargs.name}')
 
-  if add_to_registry:
-    register_serialization_keys(
-        cls, serialization_key, additional_keys)
+  return formalize_schema(
+      pg_typing.create_schema(
+          maybe_field_list=arg_fields,
+          name=f'{func.__module__}.{func.__name__}',
+          metadata={
+              'init_arg_list': init_arg_list,
+              'varargs_name': getattr(signature.varargs, 'name', None),
+              'varkw_name': getattr(signature.varkw, 'name', None),
+              'returns': returns,
+          },
+          description=description,
+          allow_nonconst_keys=True,
+      )
+  )
 
 
 def validate_init_arg_list(
     init_arg_list: List[str], cls_schema: pg_typing.Schema) -> None:
   """Validate init arg list."""
   for i, arg in enumerate(init_arg_list):
     is_vararg = False
@@ -157,32 +266,14 @@
     # Automatically generate from the field definitions in their
     # declaration order from base classes to subclasses.
     init_arg_list = [str(key) for key in cls.schema.fields.keys()
                      if isinstance(key, pg_typing.ConstStrKey)]
   return init_arg_list
 
 
-def register_serialization_keys(
-    cls,
-    serialization_key: Optional[str] = None,
-    additional_keys: Optional[List[str]] = None):
-  """Register a symbolic class for deserialization."""
-  serialization_keys = []
-  if serialization_key:
-    serialization_keys.append(serialization_key)
-  serialization_keys.append(cls.type_name)
-  if additional_keys:
-    serialization_keys.extend(additional_keys)
-
-  # Register class with 'type' property.
-  for key in serialization_keys:
-    object_utils.JSONConvertible.register(
-        key, cls, flags.is_repeated_class_registration_allowed())
-
-
 def formalize_schema(schema: pg_typing.Schema) -> pg_typing.Schema:  # pylint: disable=redefined-outer-name
   """Formalize default values in the schema."""
 
   def _formalize_field(path: object_utils.KeyPath, node: Any) -> bool:
     """Formalize field."""
     if isinstance(node, pg_typing.Field):
       field = node
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/schema_utils_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/symbolic/symbolize_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/symbolic/symbolize_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/backend_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/backend_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/early_stopping.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/early_stopping.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/local_backend.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/local_backend.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/protocols_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/protocols_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/tuning/sample_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/tuning/sample_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,14 @@
 from pyglove.core.typing.class_schema import Field
 from pyglove.core.typing.class_schema import Schema
 from pyglove.core.typing.class_schema import create_field
 from pyglove.core.typing.class_schema import create_schema
 from pyglove.core.typing.class_schema import ForwardRef
 
 # Class schema helpers.
-from pyglove.core.typing.class_schema_utils import get_init_signature
 from pyglove.core.typing.class_schema_utils import get_arg_fields
 from pyglove.core.typing.class_schema_utils import ensure_value_spec
 
 # Concrete key specifications.
 from pyglove.core.typing.key_specs import ConstStrKey
 from pyglove.core.typing.key_specs import NonConstKey
 from pyglove.core.typing.key_specs import StrKey
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/annotation_conversion_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/annotation_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_ext_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_ext_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature.py`

 * *Files 17% similar despite different names*

```diff
@@ -164,14 +164,92 @@
         ('returns', object_utils.format(self.return_value, **kwargs), 'None'),
         ('varargs', object_utils.format(self.varargs, **kwargs), 'None'),
         ('varkw', object_utils.format(self.varkw, **kwargs), 'None'),
     ])
     return f'{self.__class__.__name__}({details})'
 
   @classmethod
+  def from_schema(
+      cls,
+      schema: class_schema.Schema,
+      module_name: str,
+      name: str,
+      qualname: Optional[str] = None,
+      is_method: bool = True) -> 'Signature':
+    """Creates a signature from a schema object.
+
+    Args:
+      schema: A `pg.typing.Schema` object associated with a `pg.Object`.
+      module_name: Module name for the signature.
+      name: Function or method name of the signature.
+      qualname: Qualname of the signature.
+      is_method: If True, `self` will be added in the signature as the first
+        argument.
+
+    Returns:
+      A signature object from the schema.
+    """
+    arg_names = list(schema.metadata.get('init_arg_list', []))
+    if arg_names and arg_names[-1].startswith('*'):
+      vararg_name = arg_names[-1][1:]
+      arg_names.pop(-1)
+    else:
+      vararg_name = None
+
+    def get_arg_spec(arg_name):
+      field = schema.get_field(arg_name)
+      if not field:
+        raise ValueError(f'Argument {arg_name!r} is not a symbolic field.')
+      return field.value
+
+    args = []
+    if is_method:
+      args.append(Argument.from_annotation('self'))
+
+    # Prepare positional arguments.
+    args.extend([Argument(n, get_arg_spec(n)) for n in arg_names])
+
+    # Prepare varargs.
+    varargs = None
+    if vararg_name:
+      vararg_spec = get_arg_spec(vararg_name)
+      if not isinstance(vararg_spec, class_schema.ValueSpec.ListType):
+        raise ValueError(
+            f'Variable positional argument {vararg_name!r} should have a value '
+            f'of `pg.typing.List` type. Encountered: {vararg_spec!r}.')
+      varargs = Argument(vararg_name, vararg_spec.element.value)  # pytype: disable=attribute-error
+
+    # Prepare keyword-only arguments.
+    existing_names = set(arg_names)
+    if vararg_name:
+      existing_names.add(vararg_name)
+
+    kwonlyargs = []
+    varkw = None
+    for key, field in schema.fields.items():
+      if key not in existing_names:
+        if key.is_const:
+          kwonlyargs.append(Argument(str(key), field.value))
+        else:
+          varkw = Argument(
+              schema.metadata.get('varkw_name', None) or 'kwargs',
+              field.value)
+
+    return Signature(
+        callable_type=CallableType.FUNCTION,
+        name=name,
+        module_name=module_name,
+        qualname=qualname,
+        args=args,
+        kwonlyargs=kwonlyargs,
+        varargs=varargs,
+        varkw=varkw,
+        return_value=schema.metadata.get('returns', None))
+
+  @classmethod
   def from_callable(
       cls,
       callable_object: Callable[..., Any],
       auto_typing: bool = False) -> 'Signature':
     """Creates Signature from a callable object."""
     callable_object = typing.cast(object, callable_object)
     if not callable(callable_object):
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/callable_signature_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/callable_signature_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 import copy
 import inspect
 import unittest
 
 from pyglove.core.typing import annotation_conversion   # pylint: disable=unused-import
 from pyglove.core.typing import callable_signature
+from pyglove.core.typing import class_schema
+from pyglove.core.typing import key_specs as ks
 from pyglove.core.typing import value_specs as vs
 
 
 class SignatureTest(unittest.TestCase):
   """Tests for `Signature` class."""
 
   def test_basics(self):
@@ -217,9 +219,86 @@
     for func in [func1, func2, func3, func4, func5, func6]:
       new_func = callable_signature.get_signature(func).make_function(['pass'])
       old_signature = inspect.signature(func)
       new_signature = inspect.signature(new_func)
       self.assertEqual(old_signature, new_signature)
 
 
+class FromSchemaTest(unittest.TestCase):
+  """Tests for `Signature.from_schema`."""
+
+  def _get_signature(self, init_arg_list, is_method: bool = True):
+    s = class_schema.Schema([
+        class_schema.Field('x', vs.Int(), 'x'),
+        class_schema.Field('y', vs.Int(), 'y'),
+        class_schema.Field('z', vs.List(vs.Int()), 'z'),
+        class_schema.Field(ks.StrKey(), vs.Str(), 'kwargs'),
+    ], metadata=dict(init_arg_list=init_arg_list), allow_nonconst_keys=True)
+    return callable_signature.Signature.from_schema(
+        s, 'bar', 'foo', is_method=is_method)
+
+  def test_classmethod_with_regular_args(self):
+    self.assertEqual(
+        self._get_signature(['x', 'y', 'z']),
+        callable_signature.Signature(
+            callable_type=callable_signature.CallableType.FUNCTION,
+            module_name='bar',
+            name='foo',
+            args=[
+                callable_signature.Argument('self', vs.Any()),
+                callable_signature.Argument('x', vs.Int()),
+                callable_signature.Argument('y', vs.Int()),
+                callable_signature.Argument('z', vs.List(vs.Int())),
+            ],
+            varkw=callable_signature.Argument('kwargs', vs.Str())))
+
+  def test_function_with_varargs(self):
+    self.assertEqual(
+        self._get_signature(['x', '*z'], is_method=False),
+        callable_signature.Signature(
+            callable_type=callable_signature.CallableType.FUNCTION,
+            module_name='bar',
+            name='foo',
+            args=[
+                callable_signature.Argument('x', vs.Int()),
+            ],
+            kwonlyargs=[
+                callable_signature.Argument('y', vs.Int()),
+            ],
+            varargs=callable_signature.Argument('z', vs.Int()),
+            varkw=callable_signature.Argument('kwargs', vs.Str())))
+
+  def test_classmethod_with_kwonly_args(self):
+    self.assertEqual(
+        self._get_signature([]),
+        callable_signature.Signature(
+            callable_type=callable_signature.CallableType.FUNCTION,
+            module_name='bar',
+            name='foo',
+            args=[
+                callable_signature.Argument('self', vs.Any()),
+            ],
+            kwonlyargs=[
+                callable_signature.Argument('x', vs.Int()),
+                callable_signature.Argument('y', vs.Int()),
+                callable_signature.Argument(
+                    'z', vs.List(vs.Int())),
+            ],
+            varkw=callable_signature.Argument('kwargs', vs.Str())))
+
+  def test_bad_cases(self):
+    with self.assertRaisesRegex(
+        ValueError,
+        'Variable positional argument \'x\' should have a value of '
+        '`pg.typing.List` type'):
+      _ = self._get_signature(['*x'])
+
+    with self.assertRaisesRegex(
+        ValueError,
+        'Argument \'a\' is not a symbolic field.'):
+      _ = callable_signature.Signature.from_schema(
+          class_schema.Schema([], metadata=dict(init_arg_list=['a'])),
+          '__main__', 'foo')
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,26 @@
         ('b', {'key': 'value}),
         ('c', Optional[list]),
         ('x', int),
         ('y', Optional[str]),
         ('z', Union[int, float])
     ])
   """
+  # pylint: disable=invalid-name
+
+  # List-type value spec class.
+  ListType: Type['ValueSpec']
+
+  # Dict-type value spec class.
+  DictType: Type['ValueSpec']
+
+  # Object-type value spec class.
+  ObjectType: Type['ValueSpec']
+
+  # pylint: enable=invalid-name
 
   @property
   @abc.abstractmethod
   def value_type(self) -> Union[
       Type[Any],
       Tuple[Type[Any], ...]]:  # pyformat: disable
     """Returns acceptable (resolved) value type(s)."""
@@ -1288,32 +1300,33 @@
 
 
 def create_schema(
     maybe_field_list: List[Union[Field, Tuple]],  # pylint: disable=g-bare-generic
     name: Optional[str] = None,
     base_schema_list: Optional[List[Schema]] = None,
     allow_nonconst_keys: bool = False,
-    metadata: Optional[Dict[str, Any]] = None
+    metadata: Optional[Dict[str, Any]] = None,
+    description: Optional[str] = None,
 ) -> Schema:
   """Creates ``Schema`` from a list of ``Field``s or equivalences.
 
   Args:
     maybe_field_list: A list of field equivalent values. A Field equivalent
-      value is either a Field object or a tuple of 2 - 4 elements:
-      `(<key>, <value>, [description], [metadata])`.
-      `key` can be a KeySpec subclass object or string. `value` can be a
-      ValueSpec subclass object or equivalent value. (see
-      ``ValueSpec.from_value`` method). `description` is the description of this
-      field. It can be optional when this field overrides the default value of a
-      field defined in parent schema. `metadata` is an optional field which is a
-      dict of user objects.
+      value is either a Field object or a tuple of 2 - 4 elements: `(<key>,
+      <value>, [description], [metadata])`. `key` can be a KeySpec subclass
+      object or string. `value` can be a ValueSpec subclass object or equivalent
+      value. (see ``ValueSpec.from_value`` method). `description` is the
+      description of this field. It can be optional when this field overrides
+      the default value of a field defined in parent schema. `metadata` is an
+      optional field which is a dict of user objects.
     name: An optional name for the schema.
     base_schema_list: A list of schema objects as bases.
     allow_nonconst_keys: Whether to allow non const keys in schema.
     metadata: Optional dict of user objects as schema-level metadata.
+    description: Optional description of the schema.
 
   Returns:
     Schema object.
 
   Raises:
     TypeError: If input type is incorrect.
   """
@@ -1327,8 +1340,10 @@
                     f'Encountered: {metadata}.')
 
   return Schema(
       fields=[create_field(maybe_field) for maybe_field in maybe_field_list],
       name=name,
       base_schema_list=base_schema_list,
       allow_nonconst_keys=allow_nonconst_keys,
-      metadata=metadata)
+      metadata=metadata,
+      description=description,
+  )
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/class_schema_utils.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/class_schema_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,15 @@
       assert isinstance(arg[0], (str, ks.ConstStrKey))
       if arg[0] in arg_dict:
         raise KeyError(
             f'{signature.id}: multiple symbolic fields '
             f'found for argument {arg[0]!r}.')
       if signature.varargs and signature.varargs.name == arg[0]:
         varargs_spec = arg
+
       elif arg[0] not in func_arg_names:
         if signature.has_varkw:
           extra_arg_names.append(arg[0])
         else:
           raise KeyError(
               f'{signature.id}: found extra symbolic argument {arg[0]!r}.')
       arg_dict[arg[0]] = arg
@@ -167,79 +168,14 @@
       kwarg_spec = (ks.StrKey(), vs.Any())
     varkw_field = maybe_add_description(
         f'**{signature.varkw.name}', class_schema.Field(*kwarg_spec))
     arg_fields.append(varkw_field)
   return arg_fields
 
 
-def get_init_signature(
-    schema: class_schema.Schema,
-    module_name: str,
-    name: str,
-    qualname: Optional[str] = None,
-    is_method: bool = True) -> callable_signature.Signature:
-  """Get __init__ signature from schema."""
-  arg_names = list(schema.metadata.get('init_arg_list', []))
-  if arg_names and arg_names[-1].startswith('*'):
-    vararg_name = arg_names[-1][1:]
-    arg_names.pop(-1)
-  else:
-    vararg_name = None
-
-  def get_arg_spec(arg_name):
-    field = schema.get_field(arg_name)
-    if not field:
-      raise ValueError(f'Argument {arg_name!r} is not a symbolic field.')
-    return field.value
-
-  args = []
-  if is_method:
-    args.append(callable_signature.Argument.from_annotation('self'))
-
-  # Prepare positional arguments.
-  args.extend([callable_signature.Argument(n, get_arg_spec(n))
-               for n in arg_names])
-
-  # Prepare varargs.
-  varargs = None
-  if vararg_name:
-    vararg_spec = get_arg_spec(vararg_name)
-    if not isinstance(vararg_spec, vs.List):
-      raise ValueError(
-          f'Variable positional argument {vararg_name!r} should have a value '
-          f'of `pg.typing.List` type. Encountered: {vararg_spec!r}.')
-    varargs = callable_signature.Argument(
-        vararg_name, vararg_spec.element.value)
-
-  # Prepare keyword-only arguments.
-  existing_names = set(arg_names)
-  if vararg_name:
-    existing_names.add(vararg_name)
-
-  kwonlyargs = []
-  varkw = None
-  for key, field in schema.fields.items():
-    if key not in existing_names:
-      if key.is_const:
-        kwonlyargs.append(callable_signature.Argument(str(key), field.value))
-      else:
-        varkw = callable_signature.Argument('kwargs', field.value)
-
-  return callable_signature.Signature(
-      callable_type=callable_signature.CallableType.FUNCTION,
-      name=name,
-      module_name=module_name,
-      qualname=qualname,
-      args=args,
-      kwonlyargs=kwonlyargs,
-      varargs=varargs,
-      varkw=varkw,
-      return_value=None)
-
-
 def ensure_value_spec(
     value_spec: class_schema.ValueSpec,
     src_spec: class_schema.ValueSpec,
     root_path: Optional[object_utils.KeyPath] = None
 ) -> Optional[class_schema.ValueSpec]:
   """Extract counter part from value spec that matches dest spec type.
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/custom_typing.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/custom_typing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/key_specs_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/key_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/pytype_support.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/pytype_support.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/type_conversion_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/type_conversion_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/typed_missing_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/typed_missing_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2242,7 +2242,12 @@
   calling_module = None
   callstack = inspect.stack()
   for frame, file, *_ in callstack[1:]:
     if all(not file.endswith(site) for site in _VALUE_SPEC_CREATION_ROOT_SITES):
       calling_module = inspect.getmodule(frame)
       break
   return calling_module or __main__
+
+# Set the forward declared values to avoid circular dependency.
+ValueSpec.ListType = List
+ValueSpec.DictType = Dict
+ValueSpec.ObjectType = Object
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove/core/typing/value_specs_test.py` & `pyglove-0.3.1.dev20230520/pyglove/core/typing/value_specs_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/early_stopping/step_wise_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/early_stopping/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/hill_climb_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/hill_climb_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/mutators_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/mutators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/neat_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/neat_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/nsga2_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/nsga2_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/recombinators_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/recombinators_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/regularized_evolution_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/regularized_evolution_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/selectors_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/selectors_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/evolution/where_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/evolution/where_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/mutfun/basic_ops_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/mutfun/basic_ops_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/__init__.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/base_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/base_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/maths_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/maths_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/randoms_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/randoms_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove/ext/scalars/step_wise_test.py` & `pyglove-0.3.1.dev20230520/pyglove/ext/scalars/step_wise_test.py`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/pyglove.egg-info/PKG-INFO` & `pyglove-0.3.1.dev20230520/pyglove.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyglove
-Version: 0.3.1.dev20230519
+Version: 0.3.1.dev20230520
 Summary: PyGlove: A library for manipulating Python objects.
 Home-page: https://github.com/google/pyglove
 Author: PyGlove Authors
 Author-email: pyglove-authors@google.com
 License: Apache License 2.0
 Keywords: ai machine learning automl mutable symbolic framework meta-programming
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyglove-0.3.1.dev20230519/pyglove.egg-info/SOURCES.txt` & `pyglove-0.3.1.dev20230520/pyglove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyglove-0.3.1.dev20230519/setup.py` & `pyglove-0.3.1.dev20230520/setup.py`

 * *Files identical despite different names*

