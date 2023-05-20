# Comparing `tmp/LARRY-dataset-0.0.1.tar.gz` & `tmp/LARRY-dataset-0.0.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LARRY-dataset-0.0.1.tar", last modified: Wed Sep 14 04:27:13 2022, max compression
+gzip compressed data, was "LARRY-dataset-0.0.2rc0.tar", last modified: Sat May 20 14:24:17 2023, max compression
```

## Comparing `LARRY-dataset-0.0.1.tar` & `LARRY-dataset-0.0.2rc0.tar`

### file list

```diff
@@ -1,45 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.945026 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-09-14 04:27:13.000000 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-09-14 04:27:13.000000 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 04:27:13.000000 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-14 04:27:13.000000 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-14 04:27:13.000000 LARRY-dataset-0.0.1/LARRY_dataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3348 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.945026 LARRY-dataset-0.0.1/larry/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.949025 LARRY-dataset-0.0.1/larry/_LightningDataModule/
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_LARRY_LightningDataModule.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.949025 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/_adata_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2816 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/_annotate_task_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/_download_LARRY_in_vitro.py
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/_format_time.py
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_LightningDataModule/_supporting_functions/_split_training_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/larry/_data/
--rw-r--r--   0 runner    (1001) docker     (121)  1076280 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/LARRY.in_vitro.X_fate.npy
--rw-r--r--   0 runner    (1001) docker     (121)   616309 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/LARRY.in_vitro.d2_fate_biases.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2355 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/LARRY_PathDict.pkl
--rw-r--r--   0 runner    (1001) docker     (121)  1047224 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/early_cells.npy
--rw-r--r--   0 runner    (1001) docker     (121)   262338 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/early_neu_mo.npy
--rw-r--r--   0 runner    (1001) docker     (121)  1047224 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/fate_score.npy
--rw-r--r--   0 runner    (1001) docker     (121)  1047224 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/growth_score.npy
--rw-r--r--   0 runner    (1001) docker     (121)   131015 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/neu_mo_mask.npy
--rw-r--r--   0 runner    (1001) docker     (121)  1047224 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_data/neu_vs_mo_pct.npy
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/larry/_fetch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_fetch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_fetch/_fetch_data_from_github.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_in_vitro.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/larry/_preprocess/
--rw-r--r--   0 runner    (1001) docker     (121)     4780 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_preprocess/_Yeo2021_preprocessing_recipe.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_preprocess/_add_data_from_supp_files.py
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_preprocess/_annotate_test_train.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/larry/_preprocess/_build_kNN.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 04:27:13.957025 LARRY-dataset-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      993 2022-09-14 04:26:59.000000 LARRY-dataset-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.142405 LARRY-dataset-0.0.2rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.130405 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-20 14:24:16.000000 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-20 14:24:17.000000 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 14:24:16.000000 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-20 14:24:16.000000 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 14:24:16.000000 LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-05-20 14:24:17.142405 LARRY-dataset-0.0.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.130405 LARRY-dataset-0.0.2rc0/larry/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.134405 LARRY-dataset-0.0.2rc0/larry/_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_LARRY_t0_test_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_calculate_dominate_fate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_count_clonal_lineages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_count_clones_by_timepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_count_d2_daughter_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_estimate_growth_rates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_get_annotated_metadata_d2_lineage_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_get_lineage_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_growth_rate_grouped_violin_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_analysis/_temporal_cmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.134405 LARRY-dataset-0.0.2rc0/larry/_callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_callbacks/_interpolation_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.134405 LARRY-dataset-0.0.2rc0/larry/_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_anndata_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_anndata_path_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.134405 LARRY-dataset-0.0.2rc0/larry/_datasets/_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_dataset_utils/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_directory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_in_vitro_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_load_expr_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/_url_path_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.138405 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/_cell_cycle_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/_remove_cell_cycle_correlated_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/_running_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_datasets/klein_lab_pp_recipe/_vscores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.138405 LARRY-dataset-0.0.2rc0/larry/_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_annotate_clone_idx_in_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_annotate_fated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_cell_fates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_count_fate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_fetch_fate_bias_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_index_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_subset_clonal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_time_occupance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_tools/_to_anndataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 14:24:17.142405 LARRY-dataset-0.0.2rc0/larry/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_accuracy_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_auto_parse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_count_fate_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_larry_in_vitro_cmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_lineage_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_model_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_multi_fate_color_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_multi_fated_lineage_prediction_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_multiclass_precision_recall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_sparse_mtx_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/larry/_utils/_task_two_eval_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 14:24:17.142405 LARRY-dataset-0.0.2rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-20 14:24:04.000000 LARRY-dataset-0.0.2rc0/setup.py
```

### Comparing `LARRY-dataset-0.0.1/LARRY_dataset.egg-info/PKG-INFO` & `LARRY-dataset-0.0.2rc0/LARRY_dataset.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,318 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4c41 5252  : 2.1.Name: LARR
 00000020: 592d 6461 7461 7365 740a 5665 7273 696f  Y-dataset.Versio
-00000030: 6e3a 2030 2e30 2e31 0a53 756d 6d61 7279  n: 0.0.1.Summary
-00000040: 3a20 4c41 5252 5920 4461 7461 7365 743a  : LARRY Dataset:
-00000050: 206c 696e 6561 6765 2061 6e64 2052 4e41   lineage and RNA
-00000060: 2072 6563 6f76 6572 790a 486f 6d65 2d70   recovery.Home-p
-00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000080: 6875 622e 636f 6d2f 7069 6e65 6c6c 6f6c  hub.com/pinellol
-00000090: 6162 2f4c 4152 5259 2d64 6174 6173 6574  ab/LARRY-dataset
-000000a0: 0a41 7574 686f 723a 204d 6963 6861 656c  .Author: Michael
-000000b0: 2045 2e20 5669 6e79 6172 6420 2d20 4861   E. Vinyard - Ha
-000000c0: 7276 6172 6420 556e 6976 6572 7369 7479  rvard University
-000000d0: 202d 204d 6173 7361 6368 7573 7365 7474   - Massachussett
-000000e0: 7320 4765 6e65 7261 6c20 486f 7370 6974  s General Hospit
-000000f0: 616c 202d 2042 726f 6164 2049 6e73 7469  al - Broad Insti
-00000100: 7475 7465 206f 6620 4d49 5420 616e 6420  tute of MIT and 
-00000110: 4861 7276 6172 640a 4175 7468 6f72 2d65  Harvard.Author-e
-00000120: 6d61 696c 3a20 6d76 696e 7961 7264 4062  mail: mvinyard@b
-00000130: 726f 6164 696e 7374 6974 7574 652e 6f72  roadinstitute.or
-00000140: 670a 4c69 6365 6e73 653a 204d 4954 0a43  g.License: MIT.C
-00000150: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000160: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000170: 2032 202d 2050 7265 2d41 6c70 6861 0a43   2 - Pre-Alpha.C
-00000180: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
-000001b0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-000001c0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-000001d0: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-000001e0: 6368 0a43 6c61 7373 6966 6965 723a 2054  ch.Classifier: T
-000001f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000200: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000210: 3a20 4269 6f2d 496e 666f 726d 6174 6963  : Bio-Informatic
-00000220: 730a 5265 7175 6972 6573 2d50 7974 686f  s.Requires-Pytho
-00000230: 6e3a 203e 332e 372e 300a 4465 7363 7269  n: >3.7.0.Descri
-00000240: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000250: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000260: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000270: 4c49 4345 4e53 450a 0a23 204c 4152 5259  LICENSE..# LARRY
-00000280: 2064 6174 6173 6574 0a5b 215b 5079 5049   dataset.[![PyPI
-00000290: 2070 7976 6572 7369 6f6e 735d 2868 7474   pyversions](htt
-000002a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000002b0: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-000002c0: 6f6e 732f 6c61 7272 792d 6461 7461 7365  ons/larry-datase
-000002d0: 742e 7376 6729 5d28 6874 7470 733a 2f2f  t.svg)](https://
-000002e0: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-000002f0: 7079 7069 2f6c 6172 7279 2d64 6174 6173  pypi/larry-datas
-00000300: 6574 2f29 0a5b 215b 5079 5049 2076 6572  et/).[![PyPI ver
-00000310: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
-00000320: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000330: 6172 7279 2d64 6174 6173 6574 2e73 7667  arry-dataset.svg
-00000340: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000350: 2e66 7572 792e 696f 2f70 792f 6c61 7272  .fury.io/py/larr
-00000360: 792d 6461 7461 7365 7429 0a5b 215b 436f  y-dataset).[![Co
-00000370: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
-00000380: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000390: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-000003a0: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-000003b0: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
-000003c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003d0: 2f70 7366 2f62 6c61 636b 290a 0a23 2320  /psf/black)..## 
-000003e0: 496e 7374 616c 6c61 7469 6f6e 0a0a 2323  Installation..##
-000003f0: 2323 205b 6070 6970 605d 2829 2064 6973  ## [`pip`]() dis
-00000400: 7472 6962 7574 696f 6e0a 6060 6042 4153  tribution.```BAS
-00000410: 480a 7069 7020 696e 7374 616c 6c20 6c61  H.pip install la
-00000420: 7272 792d 6461 7461 7365 740a 6060 600a  rry-dataset.```.
-00000430: 0a23 2323 2320 4465 7665 6c6f 706d 656e  .#### Developmen
-00000440: 7420 7665 7273 696f 6e0a 6060 6042 4153  t version.```BAS
-00000450: 480a 6769 7420 636c 6f6e 6520 6874 7470  H.git clone http
-00000460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000470: 7669 6e79 6172 642f 4c41 5252 592d 6461  vinyard/LARRY-da
-00000480: 7461 7365 742e 6769 743b 2063 6420 4c41  taset.git; cd LA
-00000490: 5252 592d 6461 7461 7365 740a 0a70 6970  RRY-dataset..pip
-000004a0: 2069 6e73 7461 6c6c 202d 6520 2e0a 6060   install -e ..``
-000004b0: 600a 0a23 2320 5175 6963 6b73 7461 7274  `..## Quickstart
-000004c0: 0a44 6f77 6e6c 6f61 6473 2070 7265 2d70  .Downloads pre-p
-000004d0: 726f 6365 7373 6564 2064 6174 6120 6672  rocessed data fr
-000004e0: 6f6d 205b 2a2a 416c 6c6f 6e4b 6c65 696e  om [**AllonKlein
-000004f0: 4c61 622a 2a2f 7061 7065 722d 6461 7461  Lab**/paper-data
-00000500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000510: 2e63 6f6d 2f41 6c6c 6f6e 4b6c 6569 6e4c  .com/AllonKleinL
-00000520: 6162 2f70 6170 6572 2d64 6174 612f 7472  ab/paper-data/tr
-00000530: 6565 2f6d 6173 7465 722f 4c69 6e65 6167  ee/master/Lineag
-00000540: 655f 7472 6163 696e 675f 6f6e 5f74 7261  e_tracing_on_tra
-00000550: 6e73 6372 6970 7469 6f6e 616c 5f6c 616e  nscriptional_lan
-00000560: 6473 6361 7065 735f 6c69 6e6b 735f 7374  dscapes_links_st
-00000570: 6174 655f 746f 5f66 6174 655f 6475 7269  ate_to_fate_duri
-00000580: 6e67 5f64 6966 6665 7265 6e74 6961 7469  ng_differentiati
-00000590: 6f6e 2920 746f 2060 2e2f 4b6c 6569 6e4c  on) to `./KleinL
-000005a0: 6162 4461 7461 6020 2862 7920 6465 6661  abData` (by defa
-000005b0: 756c 7429 2e20 5468 6520 6461 7461 2069  ult). The data i
-000005c0: 7320 666f 726d 6174 7465 6420 696e 746f  s formatted into
-000005d0: 205b 6041 6e6e 4461 7461 605d 2868 7474   [`AnnData`](htt
-000005e0: 7073 3a2f 2f61 6e6e 6461 7461 2e72 6561  ps://anndata.rea
-000005f0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000600: 6174 6573 742f 2920 616e 6420 7265 7475  atest/) and retu
-00000610: 726e 6564 2074 6f20 7468 6520 7573 6572  rned to the user
-00000620: 2e20 4120 602e 6835 6164 6020 6669 6c65  . A `.h5ad` file
-00000630: 2069 7320 616c 736f 2073 6176 6564 2c20   is also saved, 
-00000640: 6c6f 6361 6c6c 792e 2054 6865 2064 6174  locally. The dat
-00000650: 6120 646f 776e 6c6f 6164 696e 6720 616e  a downloading an
-00000660: 6420 636f 6e76 6572 7369 6f6e 2073 7465  d conversion ste
-00000670: 7020 7461 6b65 2073 6576 6572 616c 206d  p take several m
-00000680: 696e 7574 6573 2064 7565 2074 6f20 7468  inutes due to th
-00000690: 6520 6c61 7267 6520 6578 7072 6573 7369  e large expressi
-000006a0: 6f6e 2060 6e6f 726d 6564 5f63 6f75 6e74  on `normed_count
-000006b0: 7360 206d 6174 7269 6365 7320 7468 6f75  s` matrices thou
-000006c0: 6768 2074 6869 7320 6f6e 6c79 2068 6170  gh this only hap
-000006d0: 7065 6e73 206f 6e63 652e 0a0a 6060 6070  pens once...```p
-000006e0: 7974 686f 6e0a 696d 706f 7274 206c 6172  ython.import lar
-000006f0: 7279 0a20 2020 200a 6461 7461 7365 7420  ry.    .dataset 
-00000700: 3d20 2269 6e5f 7669 7472 6f22 2023 2063  = "in_vitro" # c
-00000710: 616e 2061 6c73 6f20 6368 6f6f 7365 2066  an also choose f
-00000720: 726f 6d3a 2022 696e 5f76 6976 6f22 206f  rom: "in_vivo" o
-00000730: 7220 2263 7974 6f6b 696e 655f 7065 7274  r "cytokine_pert
-00000740: 7572 6261 7469 6f6e 220a 6164 6174 6120  urbation".adata 
-00000750: 3d20 6c61 7272 792e 6665 7463 6828 6461  = larry.fetch(da
-00000760: 7461 7365 7429 0a60 6060 0a60 6060 0a41  taset).```.```.A
-00000770: 6e6e 4461 7461 206f 626a 6563 7420 7769  nnData object wi
-00000780: 7468 206e 5f6f 6273 20c3 9720 6e5f 7661  th n_obs .. n_va
-00000790: 7273 203d 2031 3330 3838 3720 c397 2032  rs = 130887 .. 2
-000007a0: 3532 3839 0a20 2020 206f 6273 3a20 274c  5289.    obs: 'L
-000007b0: 6962 7261 7279 272c 2027 4365 6c6c 2062  ibrary', 'Cell b
-000007c0: 6172 636f 6465 272c 2027 5469 6d65 2070  arcode', 'Time p
-000007d0: 6f69 6e74 272c 2027 5374 6172 7469 6e67  oint', 'Starting
-000007e0: 2070 6f70 756c 6174 696f 6e27 2c20 2743   population', 'C
-000007f0: 656c 6c20 7479 7065 2061 6e6e 6f74 6174  ell type annotat
-00000800: 696f 6e27 2c20 2757 656c 6c27 2c20 2753  ion', 'Well', 'S
-00000810: 5052 494e 472d 7827 2c20 2753 5052 494e  PRING-x', 'SPRIN
-00000820: 472d 7927 0a20 2020 2076 6172 3a20 2767  G-y'.    var: 'g
-00000830: 656e 655f 6e61 6d65 270a 2020 2020 6f62  ene_name'.    ob
-00000840: 736d 3a20 2758 5f63 6c6f 6e65 270a 6060  sm: 'X_clone'.``
-00000850: 600a 0a60 6060 7079 7468 6f6e 0a69 6d70  `..```python.imp
-00000860: 6f72 7420 6c61 7272 790a 0a4c 4152 5259  ort larry..LARRY
-00000870: 5f4c 6967 6874 6e69 6e67 4461 7461 203d  _LightningData =
-00000880: 206c 6172 7279 2e4c 4152 5259 5f4c 6967   larry.LARRY_Lig
-00000890: 6874 6e69 6e67 4461 7461 4d6f 6475 6c65  htningDataModule
-000008a0: 2829 0a4c 4152 5259 5f4c 6967 6874 6e69  ().LARRY_Lightni
-000008b0: 6e67 4461 7461 2e70 7265 7061 7265 5f64  ngData.prepare_d
-000008c0: 6174 6128 290a 6060 600a 6060 600a 2041  ata().```.```. A
-000008d0: 6e6e 4461 7461 206f 626a 6563 7420 7769  nnData object wi
-000008e0: 7468 206e 5f6f 6273 20c3 9720 6e5f 7661  th n_obs .. n_va
-000008f0: 7273 203d 2031 3330 3838 3720 c397 2032  rs = 130887 .. 2
-00000900: 3532 3839 0a20 2020 206f 6273 3a20 274c  5289.    obs: 'L
-00000910: 6962 7261 7279 272c 2027 4365 6c6c 2062  ibrary', 'Cell b
-00000920: 6172 636f 6465 272c 2027 5469 6d65 2070  arcode', 'Time p
-00000930: 6f69 6e74 272c 2027 5374 6172 7469 6e67  oint', 'Starting
-00000940: 2070 6f70 756c 6174 696f 6e27 2c20 2743   population', 'C
-00000950: 656c 6c20 7479 7065 2061 6e6e 6f74 6174  ell type annotat
-00000960: 696f 6e27 2c20 2757 656c 6c27 2c20 2753  ion', 'Well', 'S
-00000970: 5052 494e 472d 7827 2c20 2753 5052 494e  PRING-x', 'SPRIN
-00000980: 472d 7927 0a20 2020 2076 6172 3a20 2767  G-y'.    var: 'g
-00000990: 656e 655f 6e61 6d65 270a 2020 2020 756e  ene_name'.    un
-000009a0: 733a 2027 6461 7461 7365 7427 2c20 2768  s: 'dataset', 'h
-000009b0: 3561 645f 7061 7468 270a 2020 2020 6f62  5ad_path'.    ob
-000009c0: 736d 3a20 2758 5f63 6c6f 6e65 270a 5072  sm: 'X_clone'.Pr
-000009d0: 6570 726f 6365 7373 696e 6720 7065 7266  eprocessing perf
-000009e0: 6f72 6d65 6420 7072 6576 696f 7573 6c79  ormed previously
-000009f0: 2e20 4c6f 6164 696e 672e 2e2e 646f 6e65  . Loading...done
-00000a00: 2e0a 6060 600a 556e 6465 7220 7468 6520  ..```.Under the 
-00000a10: 686f 6f64 2c20 7468 6520 604c 4152 5259  hood, the `LARRY
-00000a20: 5f4c 6967 6874 6e69 6e67 4461 7461 6020  _LightningData` 
-00000a30: 6361 6c6c 7320 606c 6172 7279 2e66 6574  calls `larry.fet
-00000a40: 6368 2829 6020 616e 6420 606c 6172 7279  ch()` and `larry
-00000a50: 2e70 702e 5965 6f32 3032 315f 7265 6369  .pp.Yeo2021_reci
-00000a60: 7065 2829 602c 2061 6e64 2069 6620 6074  pe()`, and if `t
-00000a70: 6173 6b20 3d3d 2022 6661 7465 5f70 7265  ask == "fate_pre
-00000a80: 6469 6374 696f 6e22 602c 2060 6c61 7272  diction"`, `larr
-00000a90: 792e 7070 2e61 6e6e 6f74 6174 655f 6661  y.pp.annotate_fa
-00000aa0: 7465 5f74 6573 745f 7472 6169 6e28 2960  te_test_train()`
-00000ab0: 200a 0a60 6060 7079 7468 6f6e 0a4c 4152   ..```python.LAR
-00000ac0: 5259 5f4c 6967 6874 6e69 6e67 4461 7461  RY_LightningData
-00000ad0: 2e61 6461 7461 0a60 6060 0a50 7269 6e74  .adata.```.Print
-00000ae0: 2074 6865 2075 7064 6174 6564 2060 6164   the updated `ad
-00000af0: 6174 6160 3a0a 6060 600a 416e 6e44 6174  ata`:.```.AnnDat
-00000b00: 6120 6f62 6a65 6374 2077 6974 6820 6e5f  a object with n_
-00000b10: 6f62 7320 c397 206e 5f76 6172 7320 3d20  obs .. n_vars = 
-00000b20: 3133 3038 3837 20c3 9720 3235 3238 390a  130887 .. 25289.
-00000b30: 2020 2020 6f62 733a 2027 4c69 6272 6172      obs: 'Librar
-00000b40: 7927 2c20 2743 656c 6c20 6261 7263 6f64  y', 'Cell barcod
-00000b50: 6527 2c20 2754 696d 6520 706f 696e 7427  e', 'Time point'
-00000b60: 2c20 2753 7461 7274 696e 6720 706f 7075  , 'Starting popu
-00000b70: 6c61 7469 6f6e 272c 2027 4365 6c6c 2074  lation', 'Cell t
-00000b80: 7970 6520 616e 6e6f 7461 7469 6f6e 272c  ype annotation',
-00000b90: 2027 5765 6c6c 272c 2027 5350 5249 4e47   'Well', 'SPRING
-00000ba0: 2d78 272c 2027 5350 5249 4e47 2d79 272c  -x', 'SPRING-y',
-00000bb0: 2027 6365 6c6c 5f69 6478 272c 2027 636c   'cell_idx', 'cl
-00000bc0: 6f6e 655f 6964 7827 0a20 2020 2076 6172  one_idx'.    var
-00000bd0: 3a20 2767 656e 655f 6e61 6d65 272c 2027  : 'gene_name', '
-00000be0: 6869 6768 6c79 5f76 6172 6961 626c 6527  highly_variable'
-00000bf0: 2c20 2763 6f72 725f 6365 6c6c 5f63 7963  , 'corr_cell_cyc
-00000c00: 6c65 272c 2027 7061 7373 5f66 696c 7465  le', 'pass_filte
-00000c10: 7227 0a20 2020 2075 6e73 3a20 2764 6174  r'.    uns: 'dat
-00000c20: 6173 6574 272c 2027 6835 6164 5f70 6174  aset', 'h5ad_pat
-00000c30: 6827 2c20 2768 6967 686c 795f 7661 7269  h', 'highly_vari
-00000c40: 6162 6c65 5f67 656e 6573 5f69 6478 272c  able_genes_idx',
-00000c50: 2027 6e5f 636f 7272 5f63 656c 6c5f 6379   'n_corr_cell_cy
-00000c60: 636c 6527 2c20 276e 5f68 7627 2c20 276e  cle', 'n_hv', 'n
-00000c70: 5f6d 6974 6f27 2c20 276e 5f70 6173 7327  _mito', 'n_pass'
-00000c80: 2c20 276e 5f74 6f74 616c 272c 2027 7070  , 'n_total', 'pp
-00000c90: 5f68 3561 645f 7061 7468 270a 2020 2020  _h5ad_path'.    
-00000ca0: 6f62 736d 3a20 2758 5f63 6c6f 6e65 272c  obsm: 'X_clone',
-00000cb0: 2027 585f 7063 6127 2c20 2758 5f73 6361   'X_pca', 'X_sca
-00000cc0: 6c65 6427 2c20 2758 5f75 6d61 7027 0a60  led', 'X_umap'.`
-00000cd0: 6060 0a0a 2323 2053 6f75 7263 6573 0a0a  ``..## Sources..
-00000ce0: 2323 2323 2052 6570 6f73 6974 6f72 6965  #### Repositorie
-00000cf0: 730a 2a20 5b2a 2a41 6c6c 6f6e 4b6c 6569  s.* [**AllonKlei
-00000d00: 6e4c 6162 2a2a 2f70 6170 6572 2d64 6174  nLab**/paper-dat
-00000d10: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00000d20: 622e 636f 6d2f 416c 6c6f 6e4b 6c65 696e  b.com/AllonKlein
-00000d30: 4c61 622f 7061 7065 722d 6461 7461 2f74  Lab/paper-data/t
-00000d40: 7265 652f 6d61 7374 6572 2f4c 696e 6561  ree/master/Linea
-00000d50: 6765 5f74 7261 6369 6e67 5f6f 6e5f 7472  ge_tracing_on_tr
-00000d60: 616e 7363 7269 7074 696f 6e61 6c5f 6c61  anscriptional_la
-00000d70: 6e64 7363 6170 6573 5f6c 696e 6b73 5f73  ndscapes_links_s
-00000d80: 7461 7465 5f74 6f5f 6661 7465 5f64 7572  tate_to_fate_dur
-00000d90: 696e 675f 6469 6666 6572 656e 7469 6174  ing_differentiat
-00000da0: 696f 6e29 0a2a 205b 2a2a 416c 6c6f 6e4b  ion).* [**AllonK
-00000db0: 6c65 696e 4c61 622a 2a2f 4c41 5252 595d  leinLab**/LARRY]
-00000dc0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000dd0: 636f 6d2f 416c 6c6f 6e4b 6c65 696e 4c61  com/AllonKleinLa
-00000de0: 622f 4c41 5252 5929 0a0a 2323 2323 2052  b/LARRY)..#### R
-00000df0: 6566 6572 656e 6365 0a2a 2057 6569 6e72  eference.* Weinr
-00000e00: 6562 2c20 432e 2c20 526f 6472 6967 7565  eb, C., Rodrigue
-00000e10: 7a2d 4672 6174 6963 656c 6c69 2c20 412e  z-Fraticelli, A.
-00000e20: 2c20 4361 6d61 7267 6f2c 2046 2e44 2e2c  , Camargo, F.D.,
-00000e30: 204b 6c65 696e 2c20 412e 4d2e 203c 6120   Klein, A.M. <a 
-00000e40: 6872 6566 3d22 6874 7470 733a 2f2f 7363  href="https://sc
-00000e50: 6965 6e63 652e 7363 6965 6e63 656d 6167  ience.sciencemag
-00000e60: 2e6f 7267 2f63 6f6e 7465 6e74 2f33 3637  .org/content/367
-00000e70: 2f36 3437 392f 6561 6177 3333 3831 223e  /6479/eaaw3381">
-00000e80: 2a2a 4c69 6e65 6167 6520 7472 6163 696e  **Lineage tracin
-00000e90: 6720 6f6e 2074 7261 6e73 6372 6970 7469  g on transcripti
-00000ea0: 6f6e 616c 206c 616e 6473 6361 7065 7320  onal landscapes 
-00000eb0: 6c69 6e6b 7320 7374 6174 6520 746f 2066  links state to f
-00000ec0: 6174 6520 6475 7269 6e67 2064 6966 6665  ate during diffe
-00000ed0: 7265 6e74 6961 7469 6f6e 2a2a 3c2f 613e  rentiation**</a>
-00000ee0: 2e20 2a53 6369 656e 6365 2a20 2a2a 3830  . *Science* **80
-00000ef0: 2a2a 2028 3230 3230 292e 2068 7474 7073  ** (2020). https
-00000f00: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3131  ://doi.org/10.11
-00000f10: 3236 2f73 6369 656e 6365 2e61 6177 3333  26/science.aaw33
-00000f20: 3831 0a0a 2d2d 2d0a 0a50 6c65 6173 6520  81..---..Please 
-00000f30: 656d 6169 6c20 4d69 6368 6165 6c20 452e  email Michael E.
-00000f40: 2056 696e 7961 7264 2028 2a2a 6d76 696e   Vinyard (**mvin
-00000f50: 7961 7264 4062 726f 6164 696e 7374 6974  yard@broadinstit
-00000f60: 7574 652e 6f72 672a 2a29 2077 6974 6820  ute.org**) with 
-00000f70: 616e 7920 7175 6573 7469 6f6e 7320 6f72  any questions or
-00000f80: 2069 6e74 6572 6573 7473 2e20 0a          interests. .
+00000030: 6e3a 2030 2e30 2e32 7263 300a 5375 6d6d  n: 0.0.2rc0.Summ
+00000040: 6172 793a 204c 4152 5259 2044 6174 6173  ary: LARRY Datas
+00000050: 6574 3a20 6c69 6e65 6167 6520 616e 6420  et: lineage and 
+00000060: 524e 4120 7265 636f 7665 7279 0a48 6f6d  RNA recovery.Hom
+00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000080: 6769 7468 7562 2e63 6f6d 2f70 696e 656c  github.com/pinel
+00000090: 6c6f 6c61 622f 4c41 5252 592d 6461 7461  lolab/LARRY-data
+000000a0: 7365 740a 4175 7468 6f72 3a20 4d69 6368  set.Author: Mich
+000000b0: 6165 6c20 452e 2056 696e 7961 7264 202d  ael E. Vinyard -
+000000c0: 2048 6172 7661 7264 2055 6e69 7665 7273   Harvard Univers
+000000d0: 6974 7920 2d20 4d61 7373 6163 6875 7373  ity - Massachuss
+000000e0: 6574 7473 2047 656e 6572 616c 2048 6f73  etts General Hos
+000000f0: 7069 7461 6c20 2d20 4272 6f61 6420 496e  pital - Broad In
+00000100: 7374 6974 7574 6520 6f66 204d 4954 2061  stitute of MIT a
+00000110: 6e64 2048 6172 7661 7264 0a41 7574 686f  nd Harvard.Autho
+00000120: 722d 656d 6169 6c3a 206d 7669 6e79 6172  r-email: mvinyar
+00000130: 6440 6272 6f61 6469 6e73 7469 7475 7465  d@broadinstitute
+00000140: 2e6f 7267 0a4c 6963 656e 7365 3a20 4d49  .org.License: MI
+00000150: 540a 436c 6173 7369 6669 6572 3a20 4465  T.Classifier: De
+00000160: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000170: 203a 3a20 3220 2d20 5072 652d 416c 7068   :: 2 - Pre-Alph
+00000180: 610a 436c 6173 7369 6669 6572 3a20 5072  a.Classifier: Pr
+00000190: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001b0: 332e 370a 436c 6173 7369 6669 6572 3a20  3.7.Classifier: 
+000001c0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000001d0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+000001e0: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
+000001f0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000200: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000210: 6720 3a3a 2042 696f 2d49 6e66 6f72 6d61  g :: Bio-Informa
+00000220: 7469 6373 0a52 6571 7569 7265 732d 5079  tics.Requires-Py
+00000230: 7468 6f6e 3a20 3e33 2e39 2e30 0a44 6573  thon: >3.9.0.Des
+00000240: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000250: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000260: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+00000270: 653a 204c 4943 454e 5345 0a0a 2320 3c69  e: LICENSE..# <i
+00000280: 6d67 2061 6c74 3d22 4c41 5252 592d 6461  mg alt="LARRY-da
+00000290: 7461 7365 742d 6c6f 676f 2220 7372 633d  taset-logo" src=
+000002a0: 222f 646f 6373 2f69 6d67 732f 4c41 5252  "/docs/imgs/LARR
+000002b0: 595f 6c6f 676f 2e73 7667 2220 7769 6474  Y_logo.svg" widt
+000002c0: 683d 2233 3030 223e 0a0a 5468 6973 2069  h="300">..This i
+000002d0: 7320 6120 5079 7468 6f6e 2070 6163 6b61  s a Python packa
+000002e0: 6765 2074 6861 7420 646f 776e 6c6f 6164  ge that download
+000002f0: 7320 616e 6420 7072 6570 726f 6365 7373  s and preprocess
+00000300: 6573 2074 6865 204c 4152 5259 2064 6174  es the LARRY dat
+00000310: 6173 6574 2066 726f 6d20 7468 6520 416c  aset from the Al
+00000320: 6c6f 6e4b 6c65 696e 4c61 6220 4769 7448  lonKleinLab GitH
+00000330: 7562 2072 6570 6f73 6974 6f72 792e 2054  ub repository. T
+00000340: 6865 204c 4152 5259 2064 6174 6173 6574  he LARRY dataset
+00000350: 2069 7320 6120 6772 6f75 7020 6f66 2073   is a group of s
+00000360: 696e 676c 652d 6365 6c6c 206c 696e 6561  ingle-cell linea
+00000370: 6765 2d74 7261 6365 6420 6461 7461 7365  ge-traced datase
+00000380: 7473 2074 6861 7420 6861 7665 2062 6565  ts that have bee
+00000390: 6e20 7573 6564 2074 6f20 7374 7564 7920  n used to study 
+000003a0: 7472 616e 7363 7269 7074 696f 6e61 6c20  transcriptional 
+000003b0: 6c61 6e64 7363 6170 6573 2061 6e64 2063  landscapes and c
+000003c0: 656c 6c20 6661 7465 2064 7572 696e 6720  ell fate during 
+000003d0: 6469 6666 6572 656e 7469 6174 696f 6e20  differentiation 
+000003e0: 5b5b 315d 2823 5265 6665 7265 6e63 6573  [[1](#References
+000003f0: 295d 2e20 5468 6572 6520 6172 6520 7468  )]. There are th
+00000400: 7265 6520 6461 7461 7365 7473 2077 6974  ree datasets wit
+00000410: 6869 6e20 7468 6973 2067 726f 7570 206f  hin this group o
+00000420: 6620 6461 7461 7365 7473 2c20 616c 6c20  f datasets, all 
+00000430: 7573 696e 6720 6865 6d61 746f 706f 6965  using hematopoie
+00000440: 7469 6320 7072 6f67 656e 6974 6f72 2063  tic progenitor c
+00000450: 656c 6c73 2066 726f 6d20 6d6f 7573 6520  ells from mouse 
+00000460: 626f 6e65 206d 6172 726f 7720 616e 6420  bone marrow and 
+00000470: 7468 6520 4c41 5252 5920 6c65 6e74 6976  the LARRY lentiv
+00000480: 6972 616c 2062 6172 636f 6469 6e67 2073  iral barcoding s
+00000490: 7472 6174 6567 792e 0a0a 312e 202a 2a2a  trategy...1. ***
+000004a0: 696e 2076 6974 726f 2a2a 2a0a 322e 202a  in vitro***.2. *
+000004b0: 2a2a 696e 2076 6976 6f2a 2a2a 202d 2074  **in vivo*** - t
+000004c0: 7261 6e73 706c 616e 7465 6420 696e 746f  ransplanted into
+000004d0: 206d 6963 650a 332e 202a 2a43 7974 6f6b   mice.3. **Cytok
+000004e0: 696e 652d 7065 7274 7572 6265 642a 2a20  ine-perturbed** 
+000004f0: 282a 696e 2076 6974 726f 2a29 202d 2073  (*in vitro*) - s
+00000500: 706c 6974 2062 6574 7765 656e 2076 6172  plit between var
+00000510: 696f 7573 2063 7974 6f6b 696e 6520 6375  ious cytokine cu
+00000520: 6c74 7572 6520 636f 6e64 6974 696f 6e73  lture conditions
+00000530: 2e0a 0a54 6865 2070 6163 6b61 6765 2069  ...The package i
+00000540: 6e63 6c75 6465 7320 6675 6e63 7469 6f6e  ncludes function
+00000550: 7320 746f 2064 6f77 6e6c 6f61 6420 7468  s to download th
+00000560: 6520 4c41 5252 5920 6461 7461 7365 742c  e LARRY dataset,
+00000570: 2066 6f72 6d61 7420 7468 6520 6669 6c65   format the file
+00000580: 7320 696e 746f 205b 6041 6e6e 4461 7461  s into [`AnnData
+00000590: 605d 2868 7474 7073 3a2f 2f61 6e6e 6461  `](https://annda
+000005a0: 7461 2e72 6561 6474 6865 646f 6373 2e69  ta.readthedocs.i
+000005b0: 6f2f 656e 2f6c 6174 6573 742f 2920 616e  o/en/latest/) an
+000005c0: 6420 7065 7266 6f72 6d20 7072 6570 726f  d perform prepro
+000005d0: 6365 7373 696e 6720 2f20 6765 6e65 2d66  cessing / gene-f
+000005e0: 696c 7465 7269 6e67 2073 7465 7073 2e20  iltering steps. 
+000005f0: 5468 6520 7072 6570 726f 6365 7373 6564  The preprocessed
+00000600: 2064 6174 6120 6361 6e20 7468 656e 2062   data can then b
+00000610: 6520 7370 6c69 7420 696e 746f 2074 6573  e split into tes
+00000620: 7420 616e 6420 7472 6169 6e69 6e67 2073  t and training s
+00000630: 6574 7320 666f 7220 7573 6520 696e 2064  ets for use in d
+00000640: 6966 6665 7265 6e74 206d 6163 6869 6e65  ifferent machine
+00000650: 206c 6561 726e 696e 6720 7461 736b 732e   learning tasks.
+00000660: 2044 696d 656e 7369 6f6e 2072 6564 7563   Dimension reduc
+00000670: 7469 6f6e 2063 616e 2062 6520 7065 7266  tion can be perf
+00000680: 6f72 6d65 6420 6166 7465 7220 6461 7461  ormed after data
+00000690: 2073 706c 6974 7469 6e67 2074 6f20 7265   splitting to re
+000006a0: 7370 6563 7420 696e 666f 726d 6174 696f  spect informatio
+000006b0: 6e20 6c65 616b 6167 6520 6f72 206f 6e20  n leakage or on 
+000006c0: 616c 6c20 6f66 2074 6865 2064 6174 612e  all of the data.
+000006d0: 0a0a 5b21 5b50 7950 4920 7079 7665 7273  ..[![PyPI pyvers
+000006e0: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
+000006f0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000700: 692f 7079 7665 7273 696f 6e73 2f6c 6172  i/pyversions/lar
+00000710: 7279 2d64 6174 6173 6574 2e73 7667 295d  ry-dataset.svg)]
+00000720: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+00000730: 7468 6f6e 2e6f 7267 2f70 7970 692f 6c61  thon.org/pypi/la
+00000740: 7272 792d 6461 7461 7365 742f 290a 5b21  rry-dataset/).[!
+00000750: 5b50 7950 4920 7665 7273 696f 6e5d 2868  [PyPI version](h
+00000760: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+00000770: 792e 696f 2f70 792f 6c61 7272 792d 6461  y.io/py/larry-da
+00000780: 7461 7365 742e 7376 6729 5d28 6874 7470  taset.svg)](http
+00000790: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
+000007a0: 6f2f 7079 2f6c 6172 7279 2d64 6174 6173  o/py/larry-datas
+000007b0: 6574 290a 5b21 5b43 6f64 6520 7374 796c  et).[![Code styl
+000007c0: 653a 2062 6c61 636b 5d28 6874 7470 733a  e: black](https:
+000007d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007e0: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+000007f0: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+00000800: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000810: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
+00000820: 6163 6b29 0a0a 2323 2049 6e73 7461 6c6c  ack)..## Install
+00000830: 6174 696f 6e0a 0a23 2323 2320 5b60 7069  ation..#### [`pi
+00000840: 7060 5d28 2920 6469 7374 7269 6275 7469  p`]() distributi
+00000850: 6f6e 0a60 6060 4241 5348 0a70 6970 2069  on.```BASH.pip i
+00000860: 6e73 7461 6c6c 206c 6172 7279 2d64 6174  nstall larry-dat
+00000870: 6173 6574 0a60 6060 0a0a 2323 2323 2044  aset.```..#### D
+00000880: 6576 656c 6f70 6d65 6e74 2076 6572 7369  evelopment versi
+00000890: 6f6e 0a60 6060 4241 5348 0a67 6974 2063  on.```BASH.git c
+000008a0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000008b0: 6875 622e 636f 6d2f 6d76 696e 7961 7264  hub.com/mvinyard
+000008c0: 2f4c 4152 5259 2d64 6174 6173 6574 2e67  /LARRY-dataset.g
+000008d0: 6974 3b20 6364 204c 4152 5259 2d64 6174  it; cd LARRY-dat
+000008e0: 6173 6574 0a0a 7069 7020 696e 7374 616c  aset..pip instal
+000008f0: 6c20 2d65 202e 0a60 6060 0a0a 2323 2051  l -e ..```..## Q
+00000900: 7569 636b 7374 6172 740a 446f 776e 6c6f  uickstart.Downlo
+00000910: 6164 7320 7072 652d 7072 6f63 6573 7365  ads pre-processe
+00000920: 6420 6461 7461 2066 726f 6d20 5b2a 2a41  d data from [**A
+00000930: 6c6c 6f6e 4b6c 6569 6e4c 6162 2a2a 2f70  llonKleinLab**/p
+00000940: 6170 6572 2d64 6174 615d 2868 7474 7073  aper-data](https
+00000950: 3a2f 2f67 6974 6875 622e 636f 6d2f 416c  ://github.com/Al
+00000960: 6c6f 6e4b 6c65 696e 4c61 622f 7061 7065  lonKleinLab/pape
+00000970: 722d 6461 7461 2f74 7265 652f 6d61 7374  r-data/tree/mast
+00000980: 6572 2f4c 696e 6561 6765 5f74 7261 6369  er/Lineage_traci
+00000990: 6e67 5f6f 6e5f 7472 616e 7363 7269 7074  ng_on_transcript
+000009a0: 696f 6e61 6c5f 6c61 6e64 7363 6170 6573  ional_landscapes
+000009b0: 5f6c 696e 6b73 5f73 7461 7465 5f74 6f5f  _links_state_to_
+000009c0: 6661 7465 5f64 7572 696e 675f 6469 6666  fate_during_diff
+000009d0: 6572 656e 7469 6174 696f 6e29 2074 6f20  erentiation) to 
+000009e0: 602e 2f4b 6c65 696e 4c61 6244 6174 6160  `./KleinLabData`
+000009f0: 2028 6279 2064 6566 6175 6c74 292e 2054   (by default). T
+00000a00: 6865 2064 6174 6120 6973 2066 6f72 6d61  he data is forma
+00000a10: 7474 6564 2069 6e74 6f20 5b60 416e 6e44  tted into [`AnnD
+00000a20: 6174 6160 5d28 6874 7470 733a 2f2f 616e  ata`](https://an
+00000a30: 6e64 6174 612e 7265 6164 7468 6564 6f63  ndata.readthedoc
+00000a40: 732e 696f 2f65 6e2f 6c61 7465 7374 2f29  s.io/en/latest/)
+00000a50: 2061 6e64 2072 6574 7572 6e65 6420 746f   and returned to
+00000a60: 2074 6865 2075 7365 722e 2041 2060 2e68   the user. A `.h
+00000a70: 3561 6460 2066 696c 6520 6973 2061 6c73  5ad` file is als
+00000a80: 6f20 7361 7665 642c 206c 6f63 616c 6c79  o saved, locally
+00000a90: 2e20 5468 6520 6461 7461 2064 6f77 6e6c  . The data downl
+00000aa0: 6f61 6469 6e67 2061 6e64 2063 6f6e 7665  oading and conve
+00000ab0: 7273 696f 6e20 7374 6570 2074 616b 6520  rsion step take 
+00000ac0: 7365 7665 7261 6c20 6d69 6e75 7465 7320  several minutes 
+00000ad0: 6475 6520 746f 2074 6865 206c 6172 6765  due to the large
+00000ae0: 2065 7870 7265 7373 696f 6e20 606e 6f72   expression `nor
+00000af0: 6d65 645f 636f 756e 7473 6020 6d61 7472  med_counts` matr
+00000b00: 6963 6573 2074 686f 7567 6820 7468 6973  ices though this
+00000b10: 206f 6e6c 7920 6861 7070 656e 7320 6f6e   only happens on
+00000b20: 6365 2e0a 0a60 6060 7079 7468 6f6e 0a69  ce...```python.i
+00000b30: 6d70 6f72 7420 6c61 7272 790a 2020 2020  mport larry.    
+00000b40: 0a64 6174 6173 6574 203d 2022 696e 5f76  .dataset = "in_v
+00000b50: 6974 726f 2220 2320 6361 6e20 616c 736f  itro" # can also
+00000b60: 2063 686f 6f73 6520 6672 6f6d 3a20 2269   choose from: "i
+00000b70: 6e5f 7669 766f 2220 6f72 2022 6379 746f  n_vivo" or "cyto
+00000b80: 6b69 6e65 5f70 6572 7475 7262 6174 696f  kine_perturbatio
+00000b90: 6e22 0a61 6461 7461 203d 206c 6172 7279  n".adata = larry
+00000ba0: 2e66 6574 6368 2864 6174 6173 6574 290a  .fetch(dataset).
+00000bb0: 6060 600a 6060 600a 416e 6e44 6174 6120  ```.```.AnnData 
+00000bc0: 6f62 6a65 6374 2077 6974 6820 6e5f 6f62  object with n_ob
+00000bd0: 7320 c397 206e 5f76 6172 7320 3d20 3133  s .. n_vars = 13
+00000be0: 3038 3837 20c3 9720 3235 3238 390a 2020  0887 .. 25289.  
+00000bf0: 2020 6f62 733a 2027 4c69 6272 6172 7927    obs: 'Library'
+00000c00: 2c20 2743 656c 6c20 6261 7263 6f64 6527  , 'Cell barcode'
+00000c10: 2c20 2754 696d 6520 706f 696e 7427 2c20  , 'Time point', 
+00000c20: 2753 7461 7274 696e 6720 706f 7075 6c61  'Starting popula
+00000c30: 7469 6f6e 272c 2027 4365 6c6c 2074 7970  tion', 'Cell typ
+00000c40: 6520 616e 6e6f 7461 7469 6f6e 272c 2027  e annotation', '
+00000c50: 5765 6c6c 272c 2027 5350 5249 4e47 2d78  Well', 'SPRING-x
+00000c60: 272c 2027 5350 5249 4e47 2d79 270a 2020  ', 'SPRING-y'.  
+00000c70: 2020 7661 723a 2027 6765 6e65 5f6e 616d    var: 'gene_nam
+00000c80: 6527 0a20 2020 206f 6273 6d3a 2027 585f  e'.    obsm: 'X_
+00000c90: 636c 6f6e 6527 0a60 6060 0a0a 6060 6070  clone'.```..```p
+00000ca0: 7974 686f 6e0a 696d 706f 7274 206c 6172  ython.import lar
+00000cb0: 7279 0a0a 4c41 5252 595f 4c69 6768 746e  ry..LARRY_Lightn
+00000cc0: 696e 6744 6174 6120 3d20 6c61 7272 792e  ingData = larry.
+00000cd0: 4c41 5252 595f 4c69 6768 746e 696e 6744  LARRY_LightningD
+00000ce0: 6174 614d 6f64 756c 6528 290a 4c41 5252  ataModule().LARR
+00000cf0: 595f 4c69 6768 746e 696e 6744 6174 612e  Y_LightningData.
+00000d00: 7072 6570 6172 655f 6461 7461 2829 0a60  prepare_data().`
+00000d10: 6060 0a60 6060 0a20 416e 6e44 6174 6120  ``.```. AnnData 
+00000d20: 6f62 6a65 6374 2077 6974 6820 6e5f 6f62  object with n_ob
+00000d30: 7320 c397 206e 5f76 6172 7320 3d20 3133  s .. n_vars = 13
+00000d40: 3038 3837 20c3 9720 3235 3238 390a 2020  0887 .. 25289.  
+00000d50: 2020 6f62 733a 2027 4c69 6272 6172 7927    obs: 'Library'
+00000d60: 2c20 2743 656c 6c20 6261 7263 6f64 6527  , 'Cell barcode'
+00000d70: 2c20 2754 696d 6520 706f 696e 7427 2c20  , 'Time point', 
+00000d80: 2753 7461 7274 696e 6720 706f 7075 6c61  'Starting popula
+00000d90: 7469 6f6e 272c 2027 4365 6c6c 2074 7970  tion', 'Cell typ
+00000da0: 6520 616e 6e6f 7461 7469 6f6e 272c 2027  e annotation', '
+00000db0: 5765 6c6c 272c 2027 5350 5249 4e47 2d78  Well', 'SPRING-x
+00000dc0: 272c 2027 5350 5249 4e47 2d79 270a 2020  ', 'SPRING-y'.  
+00000dd0: 2020 7661 723a 2027 6765 6e65 5f6e 616d    var: 'gene_nam
+00000de0: 6527 0a20 2020 2075 6e73 3a20 2764 6174  e'.    uns: 'dat
+00000df0: 6173 6574 272c 2027 6835 6164 5f70 6174  aset', 'h5ad_pat
+00000e00: 6827 0a20 2020 206f 6273 6d3a 2027 585f  h'.    obsm: 'X_
+00000e10: 636c 6f6e 6527 0a50 7265 7072 6f63 6573  clone'.Preproces
+00000e20: 7369 6e67 2070 6572 666f 726d 6564 2070  sing performed p
+00000e30: 7265 7669 6f75 736c 792e 204c 6f61 6469  reviously. Loadi
+00000e40: 6e67 2e2e 2e64 6f6e 652e 0a60 6060 0a55  ng...done..```.U
+00000e50: 6e64 6572 2074 6865 2068 6f6f 642c 2074  nder the hood, t
+00000e60: 6865 2060 4c41 5252 595f 4c69 6768 746e  he `LARRY_Lightn
+00000e70: 696e 6744 6174 6160 2063 616c 6c73 2060  ingData` calls `
+00000e80: 6c61 7272 792e 6665 7463 6828 2960 2061  larry.fetch()` a
+00000e90: 6e64 2060 6c61 7272 792e 7070 2e59 656f  nd `larry.pp.Yeo
+00000ea0: 3230 3231 5f72 6563 6970 6528 2960 2c20  2021_recipe()`, 
+00000eb0: 616e 6420 6966 2060 7461 736b 203d 3d20  and if `task == 
+00000ec0: 2266 6174 655f 7072 6564 6963 7469 6f6e  "fate_prediction
+00000ed0: 2260 2c20 606c 6172 7279 2e70 702e 616e  "`, `larry.pp.an
+00000ee0: 6e6f 7461 7465 5f66 6174 655f 7465 7374  notate_fate_test
+00000ef0: 5f74 7261 696e 2829 6020 0a0a 6060 6070  _train()` ..```p
+00000f00: 7974 686f 6e0a 4c41 5252 595f 4c69 6768  ython.LARRY_Ligh
+00000f10: 746e 696e 6744 6174 612e 6164 6174 610a  tningData.adata.
+00000f20: 6060 600a 5072 696e 7420 7468 6520 7570  ```.Print the up
+00000f30: 6461 7465 6420 6061 6461 7461 603a 0a60  dated `adata`:.`
+00000f40: 6060 0a41 6e6e 4461 7461 206f 626a 6563  ``.AnnData objec
+00000f50: 7420 7769 7468 206e 5f6f 6273 20c3 9720  t with n_obs .. 
+00000f60: 6e5f 7661 7273 203d 2031 3330 3838 3720  n_vars = 130887 
+00000f70: c397 2032 3532 3839 0a20 2020 206f 6273  .. 25289.    obs
+00000f80: 3a20 274c 6962 7261 7279 272c 2027 4365  : 'Library', 'Ce
+00000f90: 6c6c 2062 6172 636f 6465 272c 2027 5469  ll barcode', 'Ti
+00000fa0: 6d65 2070 6f69 6e74 272c 2027 5374 6172  me point', 'Star
+00000fb0: 7469 6e67 2070 6f70 756c 6174 696f 6e27  ting population'
+00000fc0: 2c20 2743 656c 6c20 7479 7065 2061 6e6e  , 'Cell type ann
+00000fd0: 6f74 6174 696f 6e27 2c20 2757 656c 6c27  otation', 'Well'
+00000fe0: 2c20 2753 5052 494e 472d 7827 2c20 2753  , 'SPRING-x', 'S
+00000ff0: 5052 494e 472d 7927 2c20 2763 656c 6c5f  PRING-y', 'cell_
+00001000: 6964 7827 2c20 2763 6c6f 6e65 5f69 6478  idx', 'clone_idx
+00001010: 270a 2020 2020 7661 723a 2027 6765 6e65  '.    var: 'gene
+00001020: 5f6e 616d 6527 2c20 2768 6967 686c 795f  _name', 'highly_
+00001030: 7661 7269 6162 6c65 272c 2027 636f 7272  variable', 'corr
+00001040: 5f63 656c 6c5f 6379 636c 6527 2c20 2770  _cell_cycle', 'p
+00001050: 6173 735f 6669 6c74 6572 270a 2020 2020  ass_filter'.    
+00001060: 756e 733a 2027 6461 7461 7365 7427 2c20  uns: 'dataset', 
+00001070: 2768 3561 645f 7061 7468 272c 2027 6869  'h5ad_path', 'hi
+00001080: 6768 6c79 5f76 6172 6961 626c 655f 6765  ghly_variable_ge
+00001090: 6e65 735f 6964 7827 2c20 276e 5f63 6f72  nes_idx', 'n_cor
+000010a0: 725f 6365 6c6c 5f63 7963 6c65 272c 2027  r_cell_cycle', '
+000010b0: 6e5f 6876 272c 2027 6e5f 6d69 746f 272c  n_hv', 'n_mito',
+000010c0: 2027 6e5f 7061 7373 272c 2027 6e5f 746f   'n_pass', 'n_to
+000010d0: 7461 6c27 2c20 2770 705f 6835 6164 5f70  tal', 'pp_h5ad_p
+000010e0: 6174 6827 0a20 2020 206f 6273 6d3a 2027  ath'.    obsm: '
+000010f0: 585f 636c 6f6e 6527 2c20 2758 5f70 6361  X_clone', 'X_pca
+00001100: 272c 2027 585f 7363 616c 6564 272c 2027  ', 'X_scaled', '
+00001110: 585f 756d 6170 270a 6060 600a 0a23 2320  X_umap'.```..## 
+00001120: 536f 7572 6365 730a 0a23 2323 2320 5265  Sources..#### Re
+00001130: 706f 7369 746f 7269 6573 0a2a 205b 2a2a  positories.* [**
+00001140: 416c 6c6f 6e4b 6c65 696e 4c61 622a 2a2f  AllonKleinLab**/
+00001150: 7061 7065 722d 6461 7461 5d28 6874 7470  paper-data](http
+00001160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00001170: 6c6c 6f6e 4b6c 6569 6e4c 6162 2f70 6170  llonKleinLab/pap
+00001180: 6572 2d64 6174 612f 7472 6565 2f6d 6173  er-data/tree/mas
+00001190: 7465 722f 4c69 6e65 6167 655f 7472 6163  ter/Lineage_trac
+000011a0: 696e 675f 6f6e 5f74 7261 6e73 6372 6970  ing_on_transcrip
+000011b0: 7469 6f6e 616c 5f6c 616e 6473 6361 7065  tional_landscape
+000011c0: 735f 6c69 6e6b 735f 7374 6174 655f 746f  s_links_state_to
+000011d0: 5f66 6174 655f 6475 7269 6e67 5f64 6966  _fate_during_dif
+000011e0: 6665 7265 6e74 6961 7469 6f6e 290a 2a20  ferentiation).* 
+000011f0: 5b2a 2a41 6c6c 6f6e 4b6c 6569 6e4c 6162  [**AllonKleinLab
+00001200: 2a2a 2f4c 4152 5259 5d28 6874 7470 733a  **/LARRY](https:
+00001210: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6c6c  //github.com/All
+00001220: 6f6e 4b6c 6569 6e4c 6162 2f4c 4152 5259  onKleinLab/LARRY
+00001230: 290a 0a23 2323 2320 5265 6665 7265 6e63  )..#### Referenc
+00001240: 6573 0a31 2e20 5765 696e 7265 622c 2043  es.1. Weinreb, C
+00001250: 2e2c 2052 6f64 7269 6775 657a 2d46 7261  ., Rodriguez-Fra
+00001260: 7469 6365 6c6c 692c 2041 2e2c 2043 616d  ticelli, A., Cam
+00001270: 6172 676f 2c20 462e 442e 2c20 4b6c 6569  argo, F.D., Klei
+00001280: 6e2c 2041 2e4d 2e20 3c61 2068 7265 663d  n, A.M. <a href=
+00001290: 2268 7474 7073 3a2f 2f73 6369 656e 6365  "https://science
+000012a0: 2e73 6369 656e 6365 6d61 672e 6f72 672f  .sciencemag.org/
+000012b0: 636f 6e74 656e 742f 3336 372f 3634 3739  content/367/6479
+000012c0: 2f65 6161 7733 3338 3122 3e2a 2a4c 696e  /eaaw3381">**Lin
+000012d0: 6561 6765 2074 7261 6369 6e67 206f 6e20  eage tracing on 
+000012e0: 7472 616e 7363 7269 7074 696f 6e61 6c20  transcriptional 
+000012f0: 6c61 6e64 7363 6170 6573 206c 696e 6b73  landscapes links
+00001300: 2073 7461 7465 2074 6f20 6661 7465 2064   state to fate d
+00001310: 7572 696e 6720 6469 6666 6572 656e 7469  uring differenti
+00001320: 6174 696f 6e2a 2a3c 2f61 3e2e 202a 5363  ation**</a>. *Sc
+00001330: 6965 6e63 652a 202a 2a38 302a 2a20 2832  ience* **80** (2
+00001340: 3032 3029 2e20 6874 7470 733a 2f2f 646f  020). https://do
+00001350: 692e 6f72 672f 3130 2e31 3132 362f 7363  i.org/10.1126/sc
+00001360: 6965 6e63 652e 6161 7733 3338 310a 0a2d  ience.aaw3381..-
+00001370: 2d2d 0a0a 506c 6561 7365 2065 6d61 696c  --..Please email
+00001380: 204d 6963 6861 656c 2045 2e20 5669 6e79   Michael E. Viny
+00001390: 6172 6420 282a 2a6d 7669 6e79 6172 6440  ard (**mvinyard@
+000013a0: 6272 6f61 6469 6e73 7469 7475 7465 2e6f  broadinstitute.o
+000013b0: 7267 2a2a 2920 7769 7468 2061 6e79 2071  rg**) with any q
+000013c0: 7565 7374 696f 6e73 206f 7220 696e 7465  uestions or inte
+000013d0: 7265 7374 732e 200a                      rests. .
```

### Comparing `LARRY-dataset-0.0.1/LICENSE` & `LARRY-dataset-0.0.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `LARRY-dataset-0.0.1/PKG-INFO` & `LARRY-dataset-0.0.2rc0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,249 +1,318 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4c41 5252  : 2.1.Name: LARR
 00000020: 592d 6461 7461 7365 740a 5665 7273 696f  Y-dataset.Versio
-00000030: 6e3a 2030 2e30 2e31 0a53 756d 6d61 7279  n: 0.0.1.Summary
-00000040: 3a20 4c41 5252 5920 4461 7461 7365 743a  : LARRY Dataset:
-00000050: 206c 696e 6561 6765 2061 6e64 2052 4e41   lineage and RNA
-00000060: 2072 6563 6f76 6572 790a 486f 6d65 2d70   recovery.Home-p
-00000070: 6167 653a 2068 7474 7073 3a2f 2f67 6974  age: https://git
-00000080: 6875 622e 636f 6d2f 7069 6e65 6c6c 6f6c  hub.com/pinellol
-00000090: 6162 2f4c 4152 5259 2d64 6174 6173 6574  ab/LARRY-dataset
-000000a0: 0a41 7574 686f 723a 204d 6963 6861 656c  .Author: Michael
-000000b0: 2045 2e20 5669 6e79 6172 6420 2d20 4861   E. Vinyard - Ha
-000000c0: 7276 6172 6420 556e 6976 6572 7369 7479  rvard University
-000000d0: 202d 204d 6173 7361 6368 7573 7365 7474   - Massachussett
-000000e0: 7320 4765 6e65 7261 6c20 486f 7370 6974  s General Hospit
-000000f0: 616c 202d 2042 726f 6164 2049 6e73 7469  al - Broad Insti
-00000100: 7475 7465 206f 6620 4d49 5420 616e 6420  tute of MIT and 
-00000110: 4861 7276 6172 640a 4175 7468 6f72 2d65  Harvard.Author-e
-00000120: 6d61 696c 3a20 6d76 696e 7961 7264 4062  mail: mvinyard@b
-00000130: 726f 6164 696e 7374 6974 7574 652e 6f72  roadinstitute.or
-00000140: 670a 4c69 6365 6e73 653a 204d 4954 0a43  g.License: MIT.C
-00000150: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000160: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000170: 2032 202d 2050 7265 2d41 6c70 6861 0a43   2 - Pre-Alpha.C
-00000180: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-00000190: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000001a0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e37  :: Python :: 3.7
-000001b0: 0a43 6c61 7373 6966 6965 723a 2049 6e74  .Classifier: Int
-000001c0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
-000001d0: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
-000001e0: 6368 0a43 6c61 7373 6966 6965 723a 2054  ch.Classifier: T
-000001f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000200: 6963 2f45 6e67 696e 6565 7269 6e67 203a  ic/Engineering :
-00000210: 3a20 4269 6f2d 496e 666f 726d 6174 6963  : Bio-Informatic
-00000220: 730a 5265 7175 6972 6573 2d50 7974 686f  s.Requires-Pytho
-00000230: 6e3a 203e 332e 372e 300a 4465 7363 7269  n: >3.7.0.Descri
-00000240: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
-00000250: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
-00000260: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
-00000270: 4c49 4345 4e53 450a 0a23 204c 4152 5259  LICENSE..# LARRY
-00000280: 2064 6174 6173 6574 0a5b 215b 5079 5049   dataset.[![PyPI
-00000290: 2070 7976 6572 7369 6f6e 735d 2868 7474   pyversions](htt
-000002a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-000002b0: 2e69 6f2f 7079 7069 2f70 7976 6572 7369  .io/pypi/pyversi
-000002c0: 6f6e 732f 6c61 7272 792d 6461 7461 7365  ons/larry-datase
-000002d0: 742e 7376 6729 5d28 6874 7470 733a 2f2f  t.svg)](https://
-000002e0: 7079 7069 2e70 7974 686f 6e2e 6f72 672f  pypi.python.org/
-000002f0: 7079 7069 2f6c 6172 7279 2d64 6174 6173  pypi/larry-datas
-00000300: 6574 2f29 0a5b 215b 5079 5049 2076 6572  et/).[![PyPI ver
-00000310: 7369 6f6e 5d28 6874 7470 733a 2f2f 6261  sion](https://ba
-00000320: 6467 652e 6675 7279 2e69 6f2f 7079 2f6c  dge.fury.io/py/l
-00000330: 6172 7279 2d64 6174 6173 6574 2e73 7667  arry-dataset.svg
-00000340: 295d 2868 7474 7073 3a2f 2f62 6164 6765  )](https://badge
-00000350: 2e66 7572 792e 696f 2f70 792f 6c61 7272  .fury.io/py/larr
-00000360: 792d 6461 7461 7365 7429 0a5b 215b 436f  y-dataset).[![Co
-00000370: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
-00000380: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000390: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
-000003a0: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
-000003b0: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
-000003c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000003d0: 2f70 7366 2f62 6c61 636b 290a 0a23 2320  /psf/black)..## 
-000003e0: 496e 7374 616c 6c61 7469 6f6e 0a0a 2323  Installation..##
-000003f0: 2323 205b 6070 6970 605d 2829 2064 6973  ## [`pip`]() dis
-00000400: 7472 6962 7574 696f 6e0a 6060 6042 4153  tribution.```BAS
-00000410: 480a 7069 7020 696e 7374 616c 6c20 6c61  H.pip install la
-00000420: 7272 792d 6461 7461 7365 740a 6060 600a  rry-dataset.```.
-00000430: 0a23 2323 2320 4465 7665 6c6f 706d 656e  .#### Developmen
-00000440: 7420 7665 7273 696f 6e0a 6060 6042 4153  t version.```BAS
-00000450: 480a 6769 7420 636c 6f6e 6520 6874 7470  H.git clone http
-00000460: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000470: 7669 6e79 6172 642f 4c41 5252 592d 6461  vinyard/LARRY-da
-00000480: 7461 7365 742e 6769 743b 2063 6420 4c41  taset.git; cd LA
-00000490: 5252 592d 6461 7461 7365 740a 0a70 6970  RRY-dataset..pip
-000004a0: 2069 6e73 7461 6c6c 202d 6520 2e0a 6060   install -e ..``
-000004b0: 600a 0a23 2320 5175 6963 6b73 7461 7274  `..## Quickstart
-000004c0: 0a44 6f77 6e6c 6f61 6473 2070 7265 2d70  .Downloads pre-p
-000004d0: 726f 6365 7373 6564 2064 6174 6120 6672  rocessed data fr
-000004e0: 6f6d 205b 2a2a 416c 6c6f 6e4b 6c65 696e  om [**AllonKlein
-000004f0: 4c61 622a 2a2f 7061 7065 722d 6461 7461  Lab**/paper-data
-00000500: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000510: 2e63 6f6d 2f41 6c6c 6f6e 4b6c 6569 6e4c  .com/AllonKleinL
-00000520: 6162 2f70 6170 6572 2d64 6174 612f 7472  ab/paper-data/tr
-00000530: 6565 2f6d 6173 7465 722f 4c69 6e65 6167  ee/master/Lineag
-00000540: 655f 7472 6163 696e 675f 6f6e 5f74 7261  e_tracing_on_tra
-00000550: 6e73 6372 6970 7469 6f6e 616c 5f6c 616e  nscriptional_lan
-00000560: 6473 6361 7065 735f 6c69 6e6b 735f 7374  dscapes_links_st
-00000570: 6174 655f 746f 5f66 6174 655f 6475 7269  ate_to_fate_duri
-00000580: 6e67 5f64 6966 6665 7265 6e74 6961 7469  ng_differentiati
-00000590: 6f6e 2920 746f 2060 2e2f 4b6c 6569 6e4c  on) to `./KleinL
-000005a0: 6162 4461 7461 6020 2862 7920 6465 6661  abData` (by defa
-000005b0: 756c 7429 2e20 5468 6520 6461 7461 2069  ult). The data i
-000005c0: 7320 666f 726d 6174 7465 6420 696e 746f  s formatted into
-000005d0: 205b 6041 6e6e 4461 7461 605d 2868 7474   [`AnnData`](htt
-000005e0: 7073 3a2f 2f61 6e6e 6461 7461 2e72 6561  ps://anndata.rea
-000005f0: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000600: 6174 6573 742f 2920 616e 6420 7265 7475  atest/) and retu
-00000610: 726e 6564 2074 6f20 7468 6520 7573 6572  rned to the user
-00000620: 2e20 4120 602e 6835 6164 6020 6669 6c65  . A `.h5ad` file
-00000630: 2069 7320 616c 736f 2073 6176 6564 2c20   is also saved, 
-00000640: 6c6f 6361 6c6c 792e 2054 6865 2064 6174  locally. The dat
-00000650: 6120 646f 776e 6c6f 6164 696e 6720 616e  a downloading an
-00000660: 6420 636f 6e76 6572 7369 6f6e 2073 7465  d conversion ste
-00000670: 7020 7461 6b65 2073 6576 6572 616c 206d  p take several m
-00000680: 696e 7574 6573 2064 7565 2074 6f20 7468  inutes due to th
-00000690: 6520 6c61 7267 6520 6578 7072 6573 7369  e large expressi
-000006a0: 6f6e 2060 6e6f 726d 6564 5f63 6f75 6e74  on `normed_count
-000006b0: 7360 206d 6174 7269 6365 7320 7468 6f75  s` matrices thou
-000006c0: 6768 2074 6869 7320 6f6e 6c79 2068 6170  gh this only hap
-000006d0: 7065 6e73 206f 6e63 652e 0a0a 6060 6070  pens once...```p
-000006e0: 7974 686f 6e0a 696d 706f 7274 206c 6172  ython.import lar
-000006f0: 7279 0a20 2020 200a 6461 7461 7365 7420  ry.    .dataset 
-00000700: 3d20 2269 6e5f 7669 7472 6f22 2023 2063  = "in_vitro" # c
-00000710: 616e 2061 6c73 6f20 6368 6f6f 7365 2066  an also choose f
-00000720: 726f 6d3a 2022 696e 5f76 6976 6f22 206f  rom: "in_vivo" o
-00000730: 7220 2263 7974 6f6b 696e 655f 7065 7274  r "cytokine_pert
-00000740: 7572 6261 7469 6f6e 220a 6164 6174 6120  urbation".adata 
-00000750: 3d20 6c61 7272 792e 6665 7463 6828 6461  = larry.fetch(da
-00000760: 7461 7365 7429 0a60 6060 0a60 6060 0a41  taset).```.```.A
-00000770: 6e6e 4461 7461 206f 626a 6563 7420 7769  nnData object wi
-00000780: 7468 206e 5f6f 6273 20c3 9720 6e5f 7661  th n_obs .. n_va
-00000790: 7273 203d 2031 3330 3838 3720 c397 2032  rs = 130887 .. 2
-000007a0: 3532 3839 0a20 2020 206f 6273 3a20 274c  5289.    obs: 'L
-000007b0: 6962 7261 7279 272c 2027 4365 6c6c 2062  ibrary', 'Cell b
-000007c0: 6172 636f 6465 272c 2027 5469 6d65 2070  arcode', 'Time p
-000007d0: 6f69 6e74 272c 2027 5374 6172 7469 6e67  oint', 'Starting
-000007e0: 2070 6f70 756c 6174 696f 6e27 2c20 2743   population', 'C
-000007f0: 656c 6c20 7479 7065 2061 6e6e 6f74 6174  ell type annotat
-00000800: 696f 6e27 2c20 2757 656c 6c27 2c20 2753  ion', 'Well', 'S
-00000810: 5052 494e 472d 7827 2c20 2753 5052 494e  PRING-x', 'SPRIN
-00000820: 472d 7927 0a20 2020 2076 6172 3a20 2767  G-y'.    var: 'g
-00000830: 656e 655f 6e61 6d65 270a 2020 2020 6f62  ene_name'.    ob
-00000840: 736d 3a20 2758 5f63 6c6f 6e65 270a 6060  sm: 'X_clone'.``
-00000850: 600a 0a60 6060 7079 7468 6f6e 0a69 6d70  `..```python.imp
-00000860: 6f72 7420 6c61 7272 790a 0a4c 4152 5259  ort larry..LARRY
-00000870: 5f4c 6967 6874 6e69 6e67 4461 7461 203d  _LightningData =
-00000880: 206c 6172 7279 2e4c 4152 5259 5f4c 6967   larry.LARRY_Lig
-00000890: 6874 6e69 6e67 4461 7461 4d6f 6475 6c65  htningDataModule
-000008a0: 2829 0a4c 4152 5259 5f4c 6967 6874 6e69  ().LARRY_Lightni
-000008b0: 6e67 4461 7461 2e70 7265 7061 7265 5f64  ngData.prepare_d
-000008c0: 6174 6128 290a 6060 600a 6060 600a 2041  ata().```.```. A
-000008d0: 6e6e 4461 7461 206f 626a 6563 7420 7769  nnData object wi
-000008e0: 7468 206e 5f6f 6273 20c3 9720 6e5f 7661  th n_obs .. n_va
-000008f0: 7273 203d 2031 3330 3838 3720 c397 2032  rs = 130887 .. 2
-00000900: 3532 3839 0a20 2020 206f 6273 3a20 274c  5289.    obs: 'L
-00000910: 6962 7261 7279 272c 2027 4365 6c6c 2062  ibrary', 'Cell b
-00000920: 6172 636f 6465 272c 2027 5469 6d65 2070  arcode', 'Time p
-00000930: 6f69 6e74 272c 2027 5374 6172 7469 6e67  oint', 'Starting
-00000940: 2070 6f70 756c 6174 696f 6e27 2c20 2743   population', 'C
-00000950: 656c 6c20 7479 7065 2061 6e6e 6f74 6174  ell type annotat
-00000960: 696f 6e27 2c20 2757 656c 6c27 2c20 2753  ion', 'Well', 'S
-00000970: 5052 494e 472d 7827 2c20 2753 5052 494e  PRING-x', 'SPRIN
-00000980: 472d 7927 0a20 2020 2076 6172 3a20 2767  G-y'.    var: 'g
-00000990: 656e 655f 6e61 6d65 270a 2020 2020 756e  ene_name'.    un
-000009a0: 733a 2027 6461 7461 7365 7427 2c20 2768  s: 'dataset', 'h
-000009b0: 3561 645f 7061 7468 270a 2020 2020 6f62  5ad_path'.    ob
-000009c0: 736d 3a20 2758 5f63 6c6f 6e65 270a 5072  sm: 'X_clone'.Pr
-000009d0: 6570 726f 6365 7373 696e 6720 7065 7266  eprocessing perf
-000009e0: 6f72 6d65 6420 7072 6576 696f 7573 6c79  ormed previously
-000009f0: 2e20 4c6f 6164 696e 672e 2e2e 646f 6e65  . Loading...done
-00000a00: 2e0a 6060 600a 556e 6465 7220 7468 6520  ..```.Under the 
-00000a10: 686f 6f64 2c20 7468 6520 604c 4152 5259  hood, the `LARRY
-00000a20: 5f4c 6967 6874 6e69 6e67 4461 7461 6020  _LightningData` 
-00000a30: 6361 6c6c 7320 606c 6172 7279 2e66 6574  calls `larry.fet
-00000a40: 6368 2829 6020 616e 6420 606c 6172 7279  ch()` and `larry
-00000a50: 2e70 702e 5965 6f32 3032 315f 7265 6369  .pp.Yeo2021_reci
-00000a60: 7065 2829 602c 2061 6e64 2069 6620 6074  pe()`, and if `t
-00000a70: 6173 6b20 3d3d 2022 6661 7465 5f70 7265  ask == "fate_pre
-00000a80: 6469 6374 696f 6e22 602c 2060 6c61 7272  diction"`, `larr
-00000a90: 792e 7070 2e61 6e6e 6f74 6174 655f 6661  y.pp.annotate_fa
-00000aa0: 7465 5f74 6573 745f 7472 6169 6e28 2960  te_test_train()`
-00000ab0: 200a 0a60 6060 7079 7468 6f6e 0a4c 4152   ..```python.LAR
-00000ac0: 5259 5f4c 6967 6874 6e69 6e67 4461 7461  RY_LightningData
-00000ad0: 2e61 6461 7461 0a60 6060 0a50 7269 6e74  .adata.```.Print
-00000ae0: 2074 6865 2075 7064 6174 6564 2060 6164   the updated `ad
-00000af0: 6174 6160 3a0a 6060 600a 416e 6e44 6174  ata`:.```.AnnDat
-00000b00: 6120 6f62 6a65 6374 2077 6974 6820 6e5f  a object with n_
-00000b10: 6f62 7320 c397 206e 5f76 6172 7320 3d20  obs .. n_vars = 
-00000b20: 3133 3038 3837 20c3 9720 3235 3238 390a  130887 .. 25289.
-00000b30: 2020 2020 6f62 733a 2027 4c69 6272 6172      obs: 'Librar
-00000b40: 7927 2c20 2743 656c 6c20 6261 7263 6f64  y', 'Cell barcod
-00000b50: 6527 2c20 2754 696d 6520 706f 696e 7427  e', 'Time point'
-00000b60: 2c20 2753 7461 7274 696e 6720 706f 7075  , 'Starting popu
-00000b70: 6c61 7469 6f6e 272c 2027 4365 6c6c 2074  lation', 'Cell t
-00000b80: 7970 6520 616e 6e6f 7461 7469 6f6e 272c  ype annotation',
-00000b90: 2027 5765 6c6c 272c 2027 5350 5249 4e47   'Well', 'SPRING
-00000ba0: 2d78 272c 2027 5350 5249 4e47 2d79 272c  -x', 'SPRING-y',
-00000bb0: 2027 6365 6c6c 5f69 6478 272c 2027 636c   'cell_idx', 'cl
-00000bc0: 6f6e 655f 6964 7827 0a20 2020 2076 6172  one_idx'.    var
-00000bd0: 3a20 2767 656e 655f 6e61 6d65 272c 2027  : 'gene_name', '
-00000be0: 6869 6768 6c79 5f76 6172 6961 626c 6527  highly_variable'
-00000bf0: 2c20 2763 6f72 725f 6365 6c6c 5f63 7963  , 'corr_cell_cyc
-00000c00: 6c65 272c 2027 7061 7373 5f66 696c 7465  le', 'pass_filte
-00000c10: 7227 0a20 2020 2075 6e73 3a20 2764 6174  r'.    uns: 'dat
-00000c20: 6173 6574 272c 2027 6835 6164 5f70 6174  aset', 'h5ad_pat
-00000c30: 6827 2c20 2768 6967 686c 795f 7661 7269  h', 'highly_vari
-00000c40: 6162 6c65 5f67 656e 6573 5f69 6478 272c  able_genes_idx',
-00000c50: 2027 6e5f 636f 7272 5f63 656c 6c5f 6379   'n_corr_cell_cy
-00000c60: 636c 6527 2c20 276e 5f68 7627 2c20 276e  cle', 'n_hv', 'n
-00000c70: 5f6d 6974 6f27 2c20 276e 5f70 6173 7327  _mito', 'n_pass'
-00000c80: 2c20 276e 5f74 6f74 616c 272c 2027 7070  , 'n_total', 'pp
-00000c90: 5f68 3561 645f 7061 7468 270a 2020 2020  _h5ad_path'.    
-00000ca0: 6f62 736d 3a20 2758 5f63 6c6f 6e65 272c  obsm: 'X_clone',
-00000cb0: 2027 585f 7063 6127 2c20 2758 5f73 6361   'X_pca', 'X_sca
-00000cc0: 6c65 6427 2c20 2758 5f75 6d61 7027 0a60  led', 'X_umap'.`
-00000cd0: 6060 0a0a 2323 2053 6f75 7263 6573 0a0a  ``..## Sources..
-00000ce0: 2323 2323 2052 6570 6f73 6974 6f72 6965  #### Repositorie
-00000cf0: 730a 2a20 5b2a 2a41 6c6c 6f6e 4b6c 6569  s.* [**AllonKlei
-00000d00: 6e4c 6162 2a2a 2f70 6170 6572 2d64 6174  nLab**/paper-dat
-00000d10: 615d 2868 7474 7073 3a2f 2f67 6974 6875  a](https://githu
-00000d20: 622e 636f 6d2f 416c 6c6f 6e4b 6c65 696e  b.com/AllonKlein
-00000d30: 4c61 622f 7061 7065 722d 6461 7461 2f74  Lab/paper-data/t
-00000d40: 7265 652f 6d61 7374 6572 2f4c 696e 6561  ree/master/Linea
-00000d50: 6765 5f74 7261 6369 6e67 5f6f 6e5f 7472  ge_tracing_on_tr
-00000d60: 616e 7363 7269 7074 696f 6e61 6c5f 6c61  anscriptional_la
-00000d70: 6e64 7363 6170 6573 5f6c 696e 6b73 5f73  ndscapes_links_s
-00000d80: 7461 7465 5f74 6f5f 6661 7465 5f64 7572  tate_to_fate_dur
-00000d90: 696e 675f 6469 6666 6572 656e 7469 6174  ing_differentiat
-00000da0: 696f 6e29 0a2a 205b 2a2a 416c 6c6f 6e4b  ion).* [**AllonK
-00000db0: 6c65 696e 4c61 622a 2a2f 4c41 5252 595d  leinLab**/LARRY]
-00000dc0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000dd0: 636f 6d2f 416c 6c6f 6e4b 6c65 696e 4c61  com/AllonKleinLa
-00000de0: 622f 4c41 5252 5929 0a0a 2323 2323 2052  b/LARRY)..#### R
-00000df0: 6566 6572 656e 6365 0a2a 2057 6569 6e72  eference.* Weinr
-00000e00: 6562 2c20 432e 2c20 526f 6472 6967 7565  eb, C., Rodrigue
-00000e10: 7a2d 4672 6174 6963 656c 6c69 2c20 412e  z-Fraticelli, A.
-00000e20: 2c20 4361 6d61 7267 6f2c 2046 2e44 2e2c  , Camargo, F.D.,
-00000e30: 204b 6c65 696e 2c20 412e 4d2e 203c 6120   Klein, A.M. <a 
-00000e40: 6872 6566 3d22 6874 7470 733a 2f2f 7363  href="https://sc
-00000e50: 6965 6e63 652e 7363 6965 6e63 656d 6167  ience.sciencemag
-00000e60: 2e6f 7267 2f63 6f6e 7465 6e74 2f33 3637  .org/content/367
-00000e70: 2f36 3437 392f 6561 6177 3333 3831 223e  /6479/eaaw3381">
-00000e80: 2a2a 4c69 6e65 6167 6520 7472 6163 696e  **Lineage tracin
-00000e90: 6720 6f6e 2074 7261 6e73 6372 6970 7469  g on transcripti
-00000ea0: 6f6e 616c 206c 616e 6473 6361 7065 7320  onal landscapes 
-00000eb0: 6c69 6e6b 7320 7374 6174 6520 746f 2066  links state to f
-00000ec0: 6174 6520 6475 7269 6e67 2064 6966 6665  ate during diffe
-00000ed0: 7265 6e74 6961 7469 6f6e 2a2a 3c2f 613e  rentiation**</a>
-00000ee0: 2e20 2a53 6369 656e 6365 2a20 2a2a 3830  . *Science* **80
-00000ef0: 2a2a 2028 3230 3230 292e 2068 7474 7073  ** (2020). https
-00000f00: 3a2f 2f64 6f69 2e6f 7267 2f31 302e 3131  ://doi.org/10.11
-00000f10: 3236 2f73 6369 656e 6365 2e61 6177 3333  26/science.aaw33
-00000f20: 3831 0a0a 2d2d 2d0a 0a50 6c65 6173 6520  81..---..Please 
-00000f30: 656d 6169 6c20 4d69 6368 6165 6c20 452e  email Michael E.
-00000f40: 2056 696e 7961 7264 2028 2a2a 6d76 696e   Vinyard (**mvin
-00000f50: 7961 7264 4062 726f 6164 696e 7374 6974  yard@broadinstit
-00000f60: 7574 652e 6f72 672a 2a29 2077 6974 6820  ute.org**) with 
-00000f70: 616e 7920 7175 6573 7469 6f6e 7320 6f72  any questions or
-00000f80: 2069 6e74 6572 6573 7473 2e20 0a          interests. .
+00000030: 6e3a 2030 2e30 2e32 7263 300a 5375 6d6d  n: 0.0.2rc0.Summ
+00000040: 6172 793a 204c 4152 5259 2044 6174 6173  ary: LARRY Datas
+00000050: 6574 3a20 6c69 6e65 6167 6520 616e 6420  et: lineage and 
+00000060: 524e 4120 7265 636f 7665 7279 0a48 6f6d  RNA recovery.Hom
+00000070: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
+00000080: 6769 7468 7562 2e63 6f6d 2f70 696e 656c  github.com/pinel
+00000090: 6c6f 6c61 622f 4c41 5252 592d 6461 7461  lolab/LARRY-data
+000000a0: 7365 740a 4175 7468 6f72 3a20 4d69 6368  set.Author: Mich
+000000b0: 6165 6c20 452e 2056 696e 7961 7264 202d  ael E. Vinyard -
+000000c0: 2048 6172 7661 7264 2055 6e69 7665 7273   Harvard Univers
+000000d0: 6974 7920 2d20 4d61 7373 6163 6875 7373  ity - Massachuss
+000000e0: 6574 7473 2047 656e 6572 616c 2048 6f73  etts General Hos
+000000f0: 7069 7461 6c20 2d20 4272 6f61 6420 496e  pital - Broad In
+00000100: 7374 6974 7574 6520 6f66 204d 4954 2061  stitute of MIT a
+00000110: 6e64 2048 6172 7661 7264 0a41 7574 686f  nd Harvard.Autho
+00000120: 722d 656d 6169 6c3a 206d 7669 6e79 6172  r-email: mvinyar
+00000130: 6440 6272 6f61 6469 6e73 7469 7475 7465  d@broadinstitute
+00000140: 2e6f 7267 0a4c 6963 656e 7365 3a20 4d49  .org.License: MI
+00000150: 540a 436c 6173 7369 6669 6572 3a20 4465  T.Classifier: De
+00000160: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+00000170: 203a 3a20 3220 2d20 5072 652d 416c 7068   :: 2 - Pre-Alph
+00000180: 610a 436c 6173 7369 6669 6572 3a20 5072  a.Classifier: Pr
+00000190: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001a0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001b0: 332e 370a 436c 6173 7369 6669 6572 3a20  3.7.Classifier: 
+000001c0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000001d0: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+000001e0: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
+000001f0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000200: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000210: 6720 3a3a 2042 696f 2d49 6e66 6f72 6d61  g :: Bio-Informa
+00000220: 7469 6373 0a52 6571 7569 7265 732d 5079  tics.Requires-Py
+00000230: 7468 6f6e 3a20 3e33 2e39 2e30 0a44 6573  thon: >3.9.0.Des
+00000240: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000250: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000260: 646f 776e 0a4c 6963 656e 7365 2d46 696c  down.License-Fil
+00000270: 653a 204c 4943 454e 5345 0a0a 2320 3c69  e: LICENSE..# <i
+00000280: 6d67 2061 6c74 3d22 4c41 5252 592d 6461  mg alt="LARRY-da
+00000290: 7461 7365 742d 6c6f 676f 2220 7372 633d  taset-logo" src=
+000002a0: 222f 646f 6373 2f69 6d67 732f 4c41 5252  "/docs/imgs/LARR
+000002b0: 595f 6c6f 676f 2e73 7667 2220 7769 6474  Y_logo.svg" widt
+000002c0: 683d 2233 3030 223e 0a0a 5468 6973 2069  h="300">..This i
+000002d0: 7320 6120 5079 7468 6f6e 2070 6163 6b61  s a Python packa
+000002e0: 6765 2074 6861 7420 646f 776e 6c6f 6164  ge that download
+000002f0: 7320 616e 6420 7072 6570 726f 6365 7373  s and preprocess
+00000300: 6573 2074 6865 204c 4152 5259 2064 6174  es the LARRY dat
+00000310: 6173 6574 2066 726f 6d20 7468 6520 416c  aset from the Al
+00000320: 6c6f 6e4b 6c65 696e 4c61 6220 4769 7448  lonKleinLab GitH
+00000330: 7562 2072 6570 6f73 6974 6f72 792e 2054  ub repository. T
+00000340: 6865 204c 4152 5259 2064 6174 6173 6574  he LARRY dataset
+00000350: 2069 7320 6120 6772 6f75 7020 6f66 2073   is a group of s
+00000360: 696e 676c 652d 6365 6c6c 206c 696e 6561  ingle-cell linea
+00000370: 6765 2d74 7261 6365 6420 6461 7461 7365  ge-traced datase
+00000380: 7473 2074 6861 7420 6861 7665 2062 6565  ts that have bee
+00000390: 6e20 7573 6564 2074 6f20 7374 7564 7920  n used to study 
+000003a0: 7472 616e 7363 7269 7074 696f 6e61 6c20  transcriptional 
+000003b0: 6c61 6e64 7363 6170 6573 2061 6e64 2063  landscapes and c
+000003c0: 656c 6c20 6661 7465 2064 7572 696e 6720  ell fate during 
+000003d0: 6469 6666 6572 656e 7469 6174 696f 6e20  differentiation 
+000003e0: 5b5b 315d 2823 5265 6665 7265 6e63 6573  [[1](#References
+000003f0: 295d 2e20 5468 6572 6520 6172 6520 7468  )]. There are th
+00000400: 7265 6520 6461 7461 7365 7473 2077 6974  ree datasets wit
+00000410: 6869 6e20 7468 6973 2067 726f 7570 206f  hin this group o
+00000420: 6620 6461 7461 7365 7473 2c20 616c 6c20  f datasets, all 
+00000430: 7573 696e 6720 6865 6d61 746f 706f 6965  using hematopoie
+00000440: 7469 6320 7072 6f67 656e 6974 6f72 2063  tic progenitor c
+00000450: 656c 6c73 2066 726f 6d20 6d6f 7573 6520  ells from mouse 
+00000460: 626f 6e65 206d 6172 726f 7720 616e 6420  bone marrow and 
+00000470: 7468 6520 4c41 5252 5920 6c65 6e74 6976  the LARRY lentiv
+00000480: 6972 616c 2062 6172 636f 6469 6e67 2073  iral barcoding s
+00000490: 7472 6174 6567 792e 0a0a 312e 202a 2a2a  trategy...1. ***
+000004a0: 696e 2076 6974 726f 2a2a 2a0a 322e 202a  in vitro***.2. *
+000004b0: 2a2a 696e 2076 6976 6f2a 2a2a 202d 2074  **in vivo*** - t
+000004c0: 7261 6e73 706c 616e 7465 6420 696e 746f  ransplanted into
+000004d0: 206d 6963 650a 332e 202a 2a43 7974 6f6b   mice.3. **Cytok
+000004e0: 696e 652d 7065 7274 7572 6265 642a 2a20  ine-perturbed** 
+000004f0: 282a 696e 2076 6974 726f 2a29 202d 2073  (*in vitro*) - s
+00000500: 706c 6974 2062 6574 7765 656e 2076 6172  plit between var
+00000510: 696f 7573 2063 7974 6f6b 696e 6520 6375  ious cytokine cu
+00000520: 6c74 7572 6520 636f 6e64 6974 696f 6e73  lture conditions
+00000530: 2e0a 0a54 6865 2070 6163 6b61 6765 2069  ...The package i
+00000540: 6e63 6c75 6465 7320 6675 6e63 7469 6f6e  ncludes function
+00000550: 7320 746f 2064 6f77 6e6c 6f61 6420 7468  s to download th
+00000560: 6520 4c41 5252 5920 6461 7461 7365 742c  e LARRY dataset,
+00000570: 2066 6f72 6d61 7420 7468 6520 6669 6c65   format the file
+00000580: 7320 696e 746f 205b 6041 6e6e 4461 7461  s into [`AnnData
+00000590: 605d 2868 7474 7073 3a2f 2f61 6e6e 6461  `](https://annda
+000005a0: 7461 2e72 6561 6474 6865 646f 6373 2e69  ta.readthedocs.i
+000005b0: 6f2f 656e 2f6c 6174 6573 742f 2920 616e  o/en/latest/) an
+000005c0: 6420 7065 7266 6f72 6d20 7072 6570 726f  d perform prepro
+000005d0: 6365 7373 696e 6720 2f20 6765 6e65 2d66  cessing / gene-f
+000005e0: 696c 7465 7269 6e67 2073 7465 7073 2e20  iltering steps. 
+000005f0: 5468 6520 7072 6570 726f 6365 7373 6564  The preprocessed
+00000600: 2064 6174 6120 6361 6e20 7468 656e 2062   data can then b
+00000610: 6520 7370 6c69 7420 696e 746f 2074 6573  e split into tes
+00000620: 7420 616e 6420 7472 6169 6e69 6e67 2073  t and training s
+00000630: 6574 7320 666f 7220 7573 6520 696e 2064  ets for use in d
+00000640: 6966 6665 7265 6e74 206d 6163 6869 6e65  ifferent machine
+00000650: 206c 6561 726e 696e 6720 7461 736b 732e   learning tasks.
+00000660: 2044 696d 656e 7369 6f6e 2072 6564 7563   Dimension reduc
+00000670: 7469 6f6e 2063 616e 2062 6520 7065 7266  tion can be perf
+00000680: 6f72 6d65 6420 6166 7465 7220 6461 7461  ormed after data
+00000690: 2073 706c 6974 7469 6e67 2074 6f20 7265   splitting to re
+000006a0: 7370 6563 7420 696e 666f 726d 6174 696f  spect informatio
+000006b0: 6e20 6c65 616b 6167 6520 6f72 206f 6e20  n leakage or on 
+000006c0: 616c 6c20 6f66 2074 6865 2064 6174 612e  all of the data.
+000006d0: 0a0a 5b21 5b50 7950 4920 7079 7665 7273  ..[![PyPI pyvers
+000006e0: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
+000006f0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000700: 692f 7079 7665 7273 696f 6e73 2f6c 6172  i/pyversions/lar
+00000710: 7279 2d64 6174 6173 6574 2e73 7667 295d  ry-dataset.svg)]
+00000720: 2868 7474 7073 3a2f 2f70 7970 692e 7079  (https://pypi.py
+00000730: 7468 6f6e 2e6f 7267 2f70 7970 692f 6c61  thon.org/pypi/la
+00000740: 7272 792d 6461 7461 7365 742f 290a 5b21  rry-dataset/).[!
+00000750: 5b50 7950 4920 7665 7273 696f 6e5d 2868  [PyPI version](h
+00000760: 7474 7073 3a2f 2f62 6164 6765 2e66 7572  ttps://badge.fur
+00000770: 792e 696f 2f70 792f 6c61 7272 792d 6461  y.io/py/larry-da
+00000780: 7461 7365 742e 7376 6729 5d28 6874 7470  taset.svg)](http
+00000790: 733a 2f2f 6261 6467 652e 6675 7279 2e69  s://badge.fury.i
+000007a0: 6f2f 7079 2f6c 6172 7279 2d64 6174 6173  o/py/larry-datas
+000007b0: 6574 290a 5b21 5b43 6f64 6520 7374 796c  et).[![Code styl
+000007c0: 653a 2062 6c61 636b 5d28 6874 7470 733a  e: black](https:
+000007d0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000007e0: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
+000007f0: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
+00000800: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
+00000810: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
+00000820: 6163 6b29 0a0a 2323 2049 6e73 7461 6c6c  ack)..## Install
+00000830: 6174 696f 6e0a 0a23 2323 2320 5b60 7069  ation..#### [`pi
+00000840: 7060 5d28 2920 6469 7374 7269 6275 7469  p`]() distributi
+00000850: 6f6e 0a60 6060 4241 5348 0a70 6970 2069  on.```BASH.pip i
+00000860: 6e73 7461 6c6c 206c 6172 7279 2d64 6174  nstall larry-dat
+00000870: 6173 6574 0a60 6060 0a0a 2323 2323 2044  aset.```..#### D
+00000880: 6576 656c 6f70 6d65 6e74 2076 6572 7369  evelopment versi
+00000890: 6f6e 0a60 6060 4241 5348 0a67 6974 2063  on.```BASH.git c
+000008a0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000008b0: 6875 622e 636f 6d2f 6d76 696e 7961 7264  hub.com/mvinyard
+000008c0: 2f4c 4152 5259 2d64 6174 6173 6574 2e67  /LARRY-dataset.g
+000008d0: 6974 3b20 6364 204c 4152 5259 2d64 6174  it; cd LARRY-dat
+000008e0: 6173 6574 0a0a 7069 7020 696e 7374 616c  aset..pip instal
+000008f0: 6c20 2d65 202e 0a60 6060 0a0a 2323 2051  l -e ..```..## Q
+00000900: 7569 636b 7374 6172 740a 446f 776e 6c6f  uickstart.Downlo
+00000910: 6164 7320 7072 652d 7072 6f63 6573 7365  ads pre-processe
+00000920: 6420 6461 7461 2066 726f 6d20 5b2a 2a41  d data from [**A
+00000930: 6c6c 6f6e 4b6c 6569 6e4c 6162 2a2a 2f70  llonKleinLab**/p
+00000940: 6170 6572 2d64 6174 615d 2868 7474 7073  aper-data](https
+00000950: 3a2f 2f67 6974 6875 622e 636f 6d2f 416c  ://github.com/Al
+00000960: 6c6f 6e4b 6c65 696e 4c61 622f 7061 7065  lonKleinLab/pape
+00000970: 722d 6461 7461 2f74 7265 652f 6d61 7374  r-data/tree/mast
+00000980: 6572 2f4c 696e 6561 6765 5f74 7261 6369  er/Lineage_traci
+00000990: 6e67 5f6f 6e5f 7472 616e 7363 7269 7074  ng_on_transcript
+000009a0: 696f 6e61 6c5f 6c61 6e64 7363 6170 6573  ional_landscapes
+000009b0: 5f6c 696e 6b73 5f73 7461 7465 5f74 6f5f  _links_state_to_
+000009c0: 6661 7465 5f64 7572 696e 675f 6469 6666  fate_during_diff
+000009d0: 6572 656e 7469 6174 696f 6e29 2074 6f20  erentiation) to 
+000009e0: 602e 2f4b 6c65 696e 4c61 6244 6174 6160  `./KleinLabData`
+000009f0: 2028 6279 2064 6566 6175 6c74 292e 2054   (by default). T
+00000a00: 6865 2064 6174 6120 6973 2066 6f72 6d61  he data is forma
+00000a10: 7474 6564 2069 6e74 6f20 5b60 416e 6e44  tted into [`AnnD
+00000a20: 6174 6160 5d28 6874 7470 733a 2f2f 616e  ata`](https://an
+00000a30: 6e64 6174 612e 7265 6164 7468 6564 6f63  ndata.readthedoc
+00000a40: 732e 696f 2f65 6e2f 6c61 7465 7374 2f29  s.io/en/latest/)
+00000a50: 2061 6e64 2072 6574 7572 6e65 6420 746f   and returned to
+00000a60: 2074 6865 2075 7365 722e 2041 2060 2e68   the user. A `.h
+00000a70: 3561 6460 2066 696c 6520 6973 2061 6c73  5ad` file is als
+00000a80: 6f20 7361 7665 642c 206c 6f63 616c 6c79  o saved, locally
+00000a90: 2e20 5468 6520 6461 7461 2064 6f77 6e6c  . The data downl
+00000aa0: 6f61 6469 6e67 2061 6e64 2063 6f6e 7665  oading and conve
+00000ab0: 7273 696f 6e20 7374 6570 2074 616b 6520  rsion step take 
+00000ac0: 7365 7665 7261 6c20 6d69 6e75 7465 7320  several minutes 
+00000ad0: 6475 6520 746f 2074 6865 206c 6172 6765  due to the large
+00000ae0: 2065 7870 7265 7373 696f 6e20 606e 6f72   expression `nor
+00000af0: 6d65 645f 636f 756e 7473 6020 6d61 7472  med_counts` matr
+00000b00: 6963 6573 2074 686f 7567 6820 7468 6973  ices though this
+00000b10: 206f 6e6c 7920 6861 7070 656e 7320 6f6e   only happens on
+00000b20: 6365 2e0a 0a60 6060 7079 7468 6f6e 0a69  ce...```python.i
+00000b30: 6d70 6f72 7420 6c61 7272 790a 2020 2020  mport larry.    
+00000b40: 0a64 6174 6173 6574 203d 2022 696e 5f76  .dataset = "in_v
+00000b50: 6974 726f 2220 2320 6361 6e20 616c 736f  itro" # can also
+00000b60: 2063 686f 6f73 6520 6672 6f6d 3a20 2269   choose from: "i
+00000b70: 6e5f 7669 766f 2220 6f72 2022 6379 746f  n_vivo" or "cyto
+00000b80: 6b69 6e65 5f70 6572 7475 7262 6174 696f  kine_perturbatio
+00000b90: 6e22 0a61 6461 7461 203d 206c 6172 7279  n".adata = larry
+00000ba0: 2e66 6574 6368 2864 6174 6173 6574 290a  .fetch(dataset).
+00000bb0: 6060 600a 6060 600a 416e 6e44 6174 6120  ```.```.AnnData 
+00000bc0: 6f62 6a65 6374 2077 6974 6820 6e5f 6f62  object with n_ob
+00000bd0: 7320 c397 206e 5f76 6172 7320 3d20 3133  s .. n_vars = 13
+00000be0: 3038 3837 20c3 9720 3235 3238 390a 2020  0887 .. 25289.  
+00000bf0: 2020 6f62 733a 2027 4c69 6272 6172 7927    obs: 'Library'
+00000c00: 2c20 2743 656c 6c20 6261 7263 6f64 6527  , 'Cell barcode'
+00000c10: 2c20 2754 696d 6520 706f 696e 7427 2c20  , 'Time point', 
+00000c20: 2753 7461 7274 696e 6720 706f 7075 6c61  'Starting popula
+00000c30: 7469 6f6e 272c 2027 4365 6c6c 2074 7970  tion', 'Cell typ
+00000c40: 6520 616e 6e6f 7461 7469 6f6e 272c 2027  e annotation', '
+00000c50: 5765 6c6c 272c 2027 5350 5249 4e47 2d78  Well', 'SPRING-x
+00000c60: 272c 2027 5350 5249 4e47 2d79 270a 2020  ', 'SPRING-y'.  
+00000c70: 2020 7661 723a 2027 6765 6e65 5f6e 616d    var: 'gene_nam
+00000c80: 6527 0a20 2020 206f 6273 6d3a 2027 585f  e'.    obsm: 'X_
+00000c90: 636c 6f6e 6527 0a60 6060 0a0a 6060 6070  clone'.```..```p
+00000ca0: 7974 686f 6e0a 696d 706f 7274 206c 6172  ython.import lar
+00000cb0: 7279 0a0a 4c41 5252 595f 4c69 6768 746e  ry..LARRY_Lightn
+00000cc0: 696e 6744 6174 6120 3d20 6c61 7272 792e  ingData = larry.
+00000cd0: 4c41 5252 595f 4c69 6768 746e 696e 6744  LARRY_LightningD
+00000ce0: 6174 614d 6f64 756c 6528 290a 4c41 5252  ataModule().LARR
+00000cf0: 595f 4c69 6768 746e 696e 6744 6174 612e  Y_LightningData.
+00000d00: 7072 6570 6172 655f 6461 7461 2829 0a60  prepare_data().`
+00000d10: 6060 0a60 6060 0a20 416e 6e44 6174 6120  ``.```. AnnData 
+00000d20: 6f62 6a65 6374 2077 6974 6820 6e5f 6f62  object with n_ob
+00000d30: 7320 c397 206e 5f76 6172 7320 3d20 3133  s .. n_vars = 13
+00000d40: 3038 3837 20c3 9720 3235 3238 390a 2020  0887 .. 25289.  
+00000d50: 2020 6f62 733a 2027 4c69 6272 6172 7927    obs: 'Library'
+00000d60: 2c20 2743 656c 6c20 6261 7263 6f64 6527  , 'Cell barcode'
+00000d70: 2c20 2754 696d 6520 706f 696e 7427 2c20  , 'Time point', 
+00000d80: 2753 7461 7274 696e 6720 706f 7075 6c61  'Starting popula
+00000d90: 7469 6f6e 272c 2027 4365 6c6c 2074 7970  tion', 'Cell typ
+00000da0: 6520 616e 6e6f 7461 7469 6f6e 272c 2027  e annotation', '
+00000db0: 5765 6c6c 272c 2027 5350 5249 4e47 2d78  Well', 'SPRING-x
+00000dc0: 272c 2027 5350 5249 4e47 2d79 270a 2020  ', 'SPRING-y'.  
+00000dd0: 2020 7661 723a 2027 6765 6e65 5f6e 616d    var: 'gene_nam
+00000de0: 6527 0a20 2020 2075 6e73 3a20 2764 6174  e'.    uns: 'dat
+00000df0: 6173 6574 272c 2027 6835 6164 5f70 6174  aset', 'h5ad_pat
+00000e00: 6827 0a20 2020 206f 6273 6d3a 2027 585f  h'.    obsm: 'X_
+00000e10: 636c 6f6e 6527 0a50 7265 7072 6f63 6573  clone'.Preproces
+00000e20: 7369 6e67 2070 6572 666f 726d 6564 2070  sing performed p
+00000e30: 7265 7669 6f75 736c 792e 204c 6f61 6469  reviously. Loadi
+00000e40: 6e67 2e2e 2e64 6f6e 652e 0a60 6060 0a55  ng...done..```.U
+00000e50: 6e64 6572 2074 6865 2068 6f6f 642c 2074  nder the hood, t
+00000e60: 6865 2060 4c41 5252 595f 4c69 6768 746e  he `LARRY_Lightn
+00000e70: 696e 6744 6174 6160 2063 616c 6c73 2060  ingData` calls `
+00000e80: 6c61 7272 792e 6665 7463 6828 2960 2061  larry.fetch()` a
+00000e90: 6e64 2060 6c61 7272 792e 7070 2e59 656f  nd `larry.pp.Yeo
+00000ea0: 3230 3231 5f72 6563 6970 6528 2960 2c20  2021_recipe()`, 
+00000eb0: 616e 6420 6966 2060 7461 736b 203d 3d20  and if `task == 
+00000ec0: 2266 6174 655f 7072 6564 6963 7469 6f6e  "fate_prediction
+00000ed0: 2260 2c20 606c 6172 7279 2e70 702e 616e  "`, `larry.pp.an
+00000ee0: 6e6f 7461 7465 5f66 6174 655f 7465 7374  notate_fate_test
+00000ef0: 5f74 7261 696e 2829 6020 0a0a 6060 6070  _train()` ..```p
+00000f00: 7974 686f 6e0a 4c41 5252 595f 4c69 6768  ython.LARRY_Ligh
+00000f10: 746e 696e 6744 6174 612e 6164 6174 610a  tningData.adata.
+00000f20: 6060 600a 5072 696e 7420 7468 6520 7570  ```.Print the up
+00000f30: 6461 7465 6420 6061 6461 7461 603a 0a60  dated `adata`:.`
+00000f40: 6060 0a41 6e6e 4461 7461 206f 626a 6563  ``.AnnData objec
+00000f50: 7420 7769 7468 206e 5f6f 6273 20c3 9720  t with n_obs .. 
+00000f60: 6e5f 7661 7273 203d 2031 3330 3838 3720  n_vars = 130887 
+00000f70: c397 2032 3532 3839 0a20 2020 206f 6273  .. 25289.    obs
+00000f80: 3a20 274c 6962 7261 7279 272c 2027 4365  : 'Library', 'Ce
+00000f90: 6c6c 2062 6172 636f 6465 272c 2027 5469  ll barcode', 'Ti
+00000fa0: 6d65 2070 6f69 6e74 272c 2027 5374 6172  me point', 'Star
+00000fb0: 7469 6e67 2070 6f70 756c 6174 696f 6e27  ting population'
+00000fc0: 2c20 2743 656c 6c20 7479 7065 2061 6e6e  , 'Cell type ann
+00000fd0: 6f74 6174 696f 6e27 2c20 2757 656c 6c27  otation', 'Well'
+00000fe0: 2c20 2753 5052 494e 472d 7827 2c20 2753  , 'SPRING-x', 'S
+00000ff0: 5052 494e 472d 7927 2c20 2763 656c 6c5f  PRING-y', 'cell_
+00001000: 6964 7827 2c20 2763 6c6f 6e65 5f69 6478  idx', 'clone_idx
+00001010: 270a 2020 2020 7661 723a 2027 6765 6e65  '.    var: 'gene
+00001020: 5f6e 616d 6527 2c20 2768 6967 686c 795f  _name', 'highly_
+00001030: 7661 7269 6162 6c65 272c 2027 636f 7272  variable', 'corr
+00001040: 5f63 656c 6c5f 6379 636c 6527 2c20 2770  _cell_cycle', 'p
+00001050: 6173 735f 6669 6c74 6572 270a 2020 2020  ass_filter'.    
+00001060: 756e 733a 2027 6461 7461 7365 7427 2c20  uns: 'dataset', 
+00001070: 2768 3561 645f 7061 7468 272c 2027 6869  'h5ad_path', 'hi
+00001080: 6768 6c79 5f76 6172 6961 626c 655f 6765  ghly_variable_ge
+00001090: 6e65 735f 6964 7827 2c20 276e 5f63 6f72  nes_idx', 'n_cor
+000010a0: 725f 6365 6c6c 5f63 7963 6c65 272c 2027  r_cell_cycle', '
+000010b0: 6e5f 6876 272c 2027 6e5f 6d69 746f 272c  n_hv', 'n_mito',
+000010c0: 2027 6e5f 7061 7373 272c 2027 6e5f 746f   'n_pass', 'n_to
+000010d0: 7461 6c27 2c20 2770 705f 6835 6164 5f70  tal', 'pp_h5ad_p
+000010e0: 6174 6827 0a20 2020 206f 6273 6d3a 2027  ath'.    obsm: '
+000010f0: 585f 636c 6f6e 6527 2c20 2758 5f70 6361  X_clone', 'X_pca
+00001100: 272c 2027 585f 7363 616c 6564 272c 2027  ', 'X_scaled', '
+00001110: 585f 756d 6170 270a 6060 600a 0a23 2320  X_umap'.```..## 
+00001120: 536f 7572 6365 730a 0a23 2323 2320 5265  Sources..#### Re
+00001130: 706f 7369 746f 7269 6573 0a2a 205b 2a2a  positories.* [**
+00001140: 416c 6c6f 6e4b 6c65 696e 4c61 622a 2a2f  AllonKleinLab**/
+00001150: 7061 7065 722d 6461 7461 5d28 6874 7470  paper-data](http
+00001160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00001170: 6c6c 6f6e 4b6c 6569 6e4c 6162 2f70 6170  llonKleinLab/pap
+00001180: 6572 2d64 6174 612f 7472 6565 2f6d 6173  er-data/tree/mas
+00001190: 7465 722f 4c69 6e65 6167 655f 7472 6163  ter/Lineage_trac
+000011a0: 696e 675f 6f6e 5f74 7261 6e73 6372 6970  ing_on_transcrip
+000011b0: 7469 6f6e 616c 5f6c 616e 6473 6361 7065  tional_landscape
+000011c0: 735f 6c69 6e6b 735f 7374 6174 655f 746f  s_links_state_to
+000011d0: 5f66 6174 655f 6475 7269 6e67 5f64 6966  _fate_during_dif
+000011e0: 6665 7265 6e74 6961 7469 6f6e 290a 2a20  ferentiation).* 
+000011f0: 5b2a 2a41 6c6c 6f6e 4b6c 6569 6e4c 6162  [**AllonKleinLab
+00001200: 2a2a 2f4c 4152 5259 5d28 6874 7470 733a  **/LARRY](https:
+00001210: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6c6c  //github.com/All
+00001220: 6f6e 4b6c 6569 6e4c 6162 2f4c 4152 5259  onKleinLab/LARRY
+00001230: 290a 0a23 2323 2320 5265 6665 7265 6e63  )..#### Referenc
+00001240: 6573 0a31 2e20 5765 696e 7265 622c 2043  es.1. Weinreb, C
+00001250: 2e2c 2052 6f64 7269 6775 657a 2d46 7261  ., Rodriguez-Fra
+00001260: 7469 6365 6c6c 692c 2041 2e2c 2043 616d  ticelli, A., Cam
+00001270: 6172 676f 2c20 462e 442e 2c20 4b6c 6569  argo, F.D., Klei
+00001280: 6e2c 2041 2e4d 2e20 3c61 2068 7265 663d  n, A.M. <a href=
+00001290: 2268 7474 7073 3a2f 2f73 6369 656e 6365  "https://science
+000012a0: 2e73 6369 656e 6365 6d61 672e 6f72 672f  .sciencemag.org/
+000012b0: 636f 6e74 656e 742f 3336 372f 3634 3739  content/367/6479
+000012c0: 2f65 6161 7733 3338 3122 3e2a 2a4c 696e  /eaaw3381">**Lin
+000012d0: 6561 6765 2074 7261 6369 6e67 206f 6e20  eage tracing on 
+000012e0: 7472 616e 7363 7269 7074 696f 6e61 6c20  transcriptional 
+000012f0: 6c61 6e64 7363 6170 6573 206c 696e 6b73  landscapes links
+00001300: 2073 7461 7465 2074 6f20 6661 7465 2064   state to fate d
+00001310: 7572 696e 6720 6469 6666 6572 656e 7469  uring differenti
+00001320: 6174 696f 6e2a 2a3c 2f61 3e2e 202a 5363  ation**</a>. *Sc
+00001330: 6965 6e63 652a 202a 2a38 302a 2a20 2832  ience* **80** (2
+00001340: 3032 3029 2e20 6874 7470 733a 2f2f 646f  020). https://do
+00001350: 692e 6f72 672f 3130 2e31 3132 362f 7363  i.org/10.1126/sc
+00001360: 6965 6e63 652e 6161 7733 3338 310a 0a2d  ience.aaw3381..-
+00001370: 2d2d 0a0a 506c 6561 7365 2065 6d61 696c  --..Please email
+00001380: 204d 6963 6861 656c 2045 2e20 5669 6e79   Michael E. Viny
+00001390: 6172 6420 282a 2a6d 7669 6e79 6172 6440  ard (**mvinyard@
+000013a0: 6272 6f61 6469 6e73 7469 7475 7465 2e6f  broadinstitute.o
+000013b0: 7267 2a2a 2920 7769 7468 2061 6e79 2071  rg**) with any q
+000013c0: 7565 7374 696f 6e73 206f 7220 696e 7465  uestions or inte
+000013d0: 7265 7374 732e 200a                      rests. .
```

### Comparing `LARRY-dataset-0.0.1/README.md` & `LARRY-dataset-0.0.2rc0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,210 +1,278 @@
-00000000: 2320 4c41 5252 5920 6461 7461 7365 740a  # LARRY dataset.
-00000010: 5b21 5b50 7950 4920 7079 7665 7273 696f  [![PyPI pyversio
-00000020: 6e73 5d28 6874 7470 733a 2f2f 696d 672e  ns](https://img.
-00000030: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
-00000040: 7079 7665 7273 696f 6e73 2f6c 6172 7279  pyversions/larry
-00000050: 2d64 6174 6173 6574 2e73 7667 295d 2868  -dataset.svg)](h
-00000060: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-00000070: 6f6e 2e6f 7267 2f70 7970 692f 6c61 7272  on.org/pypi/larr
-00000080: 792d 6461 7461 7365 742f 290a 5b21 5b50  y-dataset/).[![P
-00000090: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
-000000a0: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-000000b0: 696f 2f70 792f 6c61 7272 792d 6461 7461  io/py/larry-data
-000000c0: 7365 742e 7376 6729 5d28 6874 7470 733a  set.svg)](https:
-000000d0: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-000000e0: 7079 2f6c 6172 7279 2d64 6174 6173 6574  py/larry-dataset
-000000f0: 290a 5b21 5b43 6f64 6520 7374 796c 653a  ).[![Code style:
-00000100: 2062 6c61 636b 5d28 6874 7470 733a 2f2f   black](https://
-00000110: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000120: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-00000130: 652d 626c 6163 6b2d 3030 3030 3030 2e73  e-black-000000.s
-00000140: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
-00000150: 6875 622e 636f 6d2f 7073 662f 626c 6163  hub.com/psf/blac
-00000160: 6b29 0a0a 2323 2049 6e73 7461 6c6c 6174  k)..## Installat
-00000170: 696f 6e0a 0a23 2323 2320 5b60 7069 7060  ion..#### [`pip`
-00000180: 5d28 2920 6469 7374 7269 6275 7469 6f6e  ]() distribution
-00000190: 0a60 6060 4241 5348 0a70 6970 2069 6e73  .```BASH.pip ins
-000001a0: 7461 6c6c 206c 6172 7279 2d64 6174 6173  tall larry-datas
-000001b0: 6574 0a60 6060 0a0a 2323 2323 2044 6576  et.```..#### Dev
-000001c0: 656c 6f70 6d65 6e74 2076 6572 7369 6f6e  elopment version
-000001d0: 0a60 6060 4241 5348 0a67 6974 2063 6c6f  .```BASH.git clo
-000001e0: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-000001f0: 622e 636f 6d2f 6d76 696e 7961 7264 2f4c  b.com/mvinyard/L
-00000200: 4152 5259 2d64 6174 6173 6574 2e67 6974  ARRY-dataset.git
-00000210: 3b20 6364 204c 4152 5259 2d64 6174 6173  ; cd LARRY-datas
-00000220: 6574 0a0a 7069 7020 696e 7374 616c 6c20  et..pip install 
-00000230: 2d65 202e 0a60 6060 0a0a 2323 2051 7569  -e ..```..## Qui
-00000240: 636b 7374 6172 740a 446f 776e 6c6f 6164  ckstart.Download
-00000250: 7320 7072 652d 7072 6f63 6573 7365 6420  s pre-processed 
-00000260: 6461 7461 2066 726f 6d20 5b2a 2a41 6c6c  data from [**All
-00000270: 6f6e 4b6c 6569 6e4c 6162 2a2a 2f70 6170  onKleinLab**/pap
-00000280: 6572 2d64 6174 615d 2868 7474 7073 3a2f  er-data](https:/
-00000290: 2f67 6974 6875 622e 636f 6d2f 416c 6c6f  /github.com/Allo
-000002a0: 6e4b 6c65 696e 4c61 622f 7061 7065 722d  nKleinLab/paper-
-000002b0: 6461 7461 2f74 7265 652f 6d61 7374 6572  data/tree/master
-000002c0: 2f4c 696e 6561 6765 5f74 7261 6369 6e67  /Lineage_tracing
-000002d0: 5f6f 6e5f 7472 616e 7363 7269 7074 696f  _on_transcriptio
-000002e0: 6e61 6c5f 6c61 6e64 7363 6170 6573 5f6c  nal_landscapes_l
-000002f0: 696e 6b73 5f73 7461 7465 5f74 6f5f 6661  inks_state_to_fa
-00000300: 7465 5f64 7572 696e 675f 6469 6666 6572  te_during_differ
-00000310: 656e 7469 6174 696f 6e29 2074 6f20 602e  entiation) to `.
-00000320: 2f4b 6c65 696e 4c61 6244 6174 6160 2028  /KleinLabData` (
-00000330: 6279 2064 6566 6175 6c74 292e 2054 6865  by default). The
-00000340: 2064 6174 6120 6973 2066 6f72 6d61 7474   data is formatt
-00000350: 6564 2069 6e74 6f20 5b60 416e 6e44 6174  ed into [`AnnDat
-00000360: 6160 5d28 6874 7470 733a 2f2f 616e 6e64  a`](https://annd
-00000370: 6174 612e 7265 6164 7468 6564 6f63 732e  ata.readthedocs.
-00000380: 696f 2f65 6e2f 6c61 7465 7374 2f29 2061  io/en/latest/) a
-00000390: 6e64 2072 6574 7572 6e65 6420 746f 2074  nd returned to t
-000003a0: 6865 2075 7365 722e 2041 2060 2e68 3561  he user. A `.h5a
-000003b0: 6460 2066 696c 6520 6973 2061 6c73 6f20  d` file is also 
-000003c0: 7361 7665 642c 206c 6f63 616c 6c79 2e20  saved, locally. 
-000003d0: 5468 6520 6461 7461 2064 6f77 6e6c 6f61  The data downloa
-000003e0: 6469 6e67 2061 6e64 2063 6f6e 7665 7273  ding and convers
-000003f0: 696f 6e20 7374 6570 2074 616b 6520 7365  ion step take se
-00000400: 7665 7261 6c20 6d69 6e75 7465 7320 6475  veral minutes du
-00000410: 6520 746f 2074 6865 206c 6172 6765 2065  e to the large e
-00000420: 7870 7265 7373 696f 6e20 606e 6f72 6d65  xpression `norme
-00000430: 645f 636f 756e 7473 6020 6d61 7472 6963  d_counts` matric
-00000440: 6573 2074 686f 7567 6820 7468 6973 206f  es though this o
-00000450: 6e6c 7920 6861 7070 656e 7320 6f6e 6365  nly happens once
-00000460: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
-00000470: 6f72 7420 6c61 7272 790a 2020 2020 0a64  ort larry.    .d
-00000480: 6174 6173 6574 203d 2022 696e 5f76 6974  ataset = "in_vit
-00000490: 726f 2220 2320 6361 6e20 616c 736f 2063  ro" # can also c
-000004a0: 686f 6f73 6520 6672 6f6d 3a20 2269 6e5f  hoose from: "in_
-000004b0: 7669 766f 2220 6f72 2022 6379 746f 6b69  vivo" or "cytoki
-000004c0: 6e65 5f70 6572 7475 7262 6174 696f 6e22  ne_perturbation"
-000004d0: 0a61 6461 7461 203d 206c 6172 7279 2e66  .adata = larry.f
-000004e0: 6574 6368 2864 6174 6173 6574 290a 6060  etch(dataset).``
-000004f0: 600a 6060 600a 416e 6e44 6174 6120 6f62  `.```.AnnData ob
-00000500: 6a65 6374 2077 6974 6820 6e5f 6f62 7320  ject with n_obs 
-00000510: c397 206e 5f76 6172 7320 3d20 3133 3038  .. n_vars = 1308
-00000520: 3837 20c3 9720 3235 3238 390a 2020 2020  87 .. 25289.    
-00000530: 6f62 733a 2027 4c69 6272 6172 7927 2c20  obs: 'Library', 
-00000540: 2743 656c 6c20 6261 7263 6f64 6527 2c20  'Cell barcode', 
-00000550: 2754 696d 6520 706f 696e 7427 2c20 2753  'Time point', 'S
-00000560: 7461 7274 696e 6720 706f 7075 6c61 7469  tarting populati
-00000570: 6f6e 272c 2027 4365 6c6c 2074 7970 6520  on', 'Cell type 
-00000580: 616e 6e6f 7461 7469 6f6e 272c 2027 5765  annotation', 'We
-00000590: 6c6c 272c 2027 5350 5249 4e47 2d78 272c  ll', 'SPRING-x',
-000005a0: 2027 5350 5249 4e47 2d79 270a 2020 2020   'SPRING-y'.    
-000005b0: 7661 723a 2027 6765 6e65 5f6e 616d 6527  var: 'gene_name'
-000005c0: 0a20 2020 206f 6273 6d3a 2027 585f 636c  .    obsm: 'X_cl
-000005d0: 6f6e 6527 0a60 6060 0a0a 6060 6070 7974  one'.```..```pyt
-000005e0: 686f 6e0a 696d 706f 7274 206c 6172 7279  hon.import larry
-000005f0: 0a0a 4c41 5252 595f 4c69 6768 746e 696e  ..LARRY_Lightnin
-00000600: 6744 6174 6120 3d20 6c61 7272 792e 4c41  gData = larry.LA
-00000610: 5252 595f 4c69 6768 746e 696e 6744 6174  RRY_LightningDat
-00000620: 614d 6f64 756c 6528 290a 4c41 5252 595f  aModule().LARRY_
-00000630: 4c69 6768 746e 696e 6744 6174 612e 7072  LightningData.pr
-00000640: 6570 6172 655f 6461 7461 2829 0a60 6060  epare_data().```
-00000650: 0a60 6060 0a20 416e 6e44 6174 6120 6f62  .```. AnnData ob
-00000660: 6a65 6374 2077 6974 6820 6e5f 6f62 7320  ject with n_obs 
-00000670: c397 206e 5f76 6172 7320 3d20 3133 3038  .. n_vars = 1308
-00000680: 3837 20c3 9720 3235 3238 390a 2020 2020  87 .. 25289.    
-00000690: 6f62 733a 2027 4c69 6272 6172 7927 2c20  obs: 'Library', 
-000006a0: 2743 656c 6c20 6261 7263 6f64 6527 2c20  'Cell barcode', 
-000006b0: 2754 696d 6520 706f 696e 7427 2c20 2753  'Time point', 'S
-000006c0: 7461 7274 696e 6720 706f 7075 6c61 7469  tarting populati
-000006d0: 6f6e 272c 2027 4365 6c6c 2074 7970 6520  on', 'Cell type 
-000006e0: 616e 6e6f 7461 7469 6f6e 272c 2027 5765  annotation', 'We
-000006f0: 6c6c 272c 2027 5350 5249 4e47 2d78 272c  ll', 'SPRING-x',
-00000700: 2027 5350 5249 4e47 2d79 270a 2020 2020   'SPRING-y'.    
-00000710: 7661 723a 2027 6765 6e65 5f6e 616d 6527  var: 'gene_name'
-00000720: 0a20 2020 2075 6e73 3a20 2764 6174 6173  .    uns: 'datas
-00000730: 6574 272c 2027 6835 6164 5f70 6174 6827  et', 'h5ad_path'
-00000740: 0a20 2020 206f 6273 6d3a 2027 585f 636c  .    obsm: 'X_cl
-00000750: 6f6e 6527 0a50 7265 7072 6f63 6573 7369  one'.Preprocessi
-00000760: 6e67 2070 6572 666f 726d 6564 2070 7265  ng performed pre
-00000770: 7669 6f75 736c 792e 204c 6f61 6469 6e67  viously. Loading
-00000780: 2e2e 2e64 6f6e 652e 0a60 6060 0a55 6e64  ...done..```.Und
-00000790: 6572 2074 6865 2068 6f6f 642c 2074 6865  er the hood, the
-000007a0: 2060 4c41 5252 595f 4c69 6768 746e 696e   `LARRY_Lightnin
-000007b0: 6744 6174 6160 2063 616c 6c73 2060 6c61  gData` calls `la
-000007c0: 7272 792e 6665 7463 6828 2960 2061 6e64  rry.fetch()` and
-000007d0: 2060 6c61 7272 792e 7070 2e59 656f 3230   `larry.pp.Yeo20
-000007e0: 3231 5f72 6563 6970 6528 2960 2c20 616e  21_recipe()`, an
-000007f0: 6420 6966 2060 7461 736b 203d 3d20 2266  d if `task == "f
-00000800: 6174 655f 7072 6564 6963 7469 6f6e 2260  ate_prediction"`
-00000810: 2c20 606c 6172 7279 2e70 702e 616e 6e6f  , `larry.pp.anno
-00000820: 7461 7465 5f66 6174 655f 7465 7374 5f74  tate_fate_test_t
-00000830: 7261 696e 2829 6020 0a0a 6060 6070 7974  rain()` ..```pyt
-00000840: 686f 6e0a 4c41 5252 595f 4c69 6768 746e  hon.LARRY_Lightn
-00000850: 696e 6744 6174 612e 6164 6174 610a 6060  ingData.adata.``
-00000860: 600a 5072 696e 7420 7468 6520 7570 6461  `.Print the upda
-00000870: 7465 6420 6061 6461 7461 603a 0a60 6060  ted `adata`:.```
-00000880: 0a41 6e6e 4461 7461 206f 626a 6563 7420  .AnnData object 
-00000890: 7769 7468 206e 5f6f 6273 20c3 9720 6e5f  with n_obs .. n_
-000008a0: 7661 7273 203d 2031 3330 3838 3720 c397  vars = 130887 ..
-000008b0: 2032 3532 3839 0a20 2020 206f 6273 3a20   25289.    obs: 
-000008c0: 274c 6962 7261 7279 272c 2027 4365 6c6c  'Library', 'Cell
-000008d0: 2062 6172 636f 6465 272c 2027 5469 6d65   barcode', 'Time
-000008e0: 2070 6f69 6e74 272c 2027 5374 6172 7469   point', 'Starti
-000008f0: 6e67 2070 6f70 756c 6174 696f 6e27 2c20  ng population', 
-00000900: 2743 656c 6c20 7479 7065 2061 6e6e 6f74  'Cell type annot
-00000910: 6174 696f 6e27 2c20 2757 656c 6c27 2c20  ation', 'Well', 
-00000920: 2753 5052 494e 472d 7827 2c20 2753 5052  'SPRING-x', 'SPR
-00000930: 494e 472d 7927 2c20 2763 656c 6c5f 6964  ING-y', 'cell_id
-00000940: 7827 2c20 2763 6c6f 6e65 5f69 6478 270a  x', 'clone_idx'.
-00000950: 2020 2020 7661 723a 2027 6765 6e65 5f6e      var: 'gene_n
-00000960: 616d 6527 2c20 2768 6967 686c 795f 7661  ame', 'highly_va
-00000970: 7269 6162 6c65 272c 2027 636f 7272 5f63  riable', 'corr_c
-00000980: 656c 6c5f 6379 636c 6527 2c20 2770 6173  ell_cycle', 'pas
-00000990: 735f 6669 6c74 6572 270a 2020 2020 756e  s_filter'.    un
-000009a0: 733a 2027 6461 7461 7365 7427 2c20 2768  s: 'dataset', 'h
-000009b0: 3561 645f 7061 7468 272c 2027 6869 6768  5ad_path', 'high
-000009c0: 6c79 5f76 6172 6961 626c 655f 6765 6e65  ly_variable_gene
-000009d0: 735f 6964 7827 2c20 276e 5f63 6f72 725f  s_idx', 'n_corr_
-000009e0: 6365 6c6c 5f63 7963 6c65 272c 2027 6e5f  cell_cycle', 'n_
-000009f0: 6876 272c 2027 6e5f 6d69 746f 272c 2027  hv', 'n_mito', '
-00000a00: 6e5f 7061 7373 272c 2027 6e5f 746f 7461  n_pass', 'n_tota
-00000a10: 6c27 2c20 2770 705f 6835 6164 5f70 6174  l', 'pp_h5ad_pat
-00000a20: 6827 0a20 2020 206f 6273 6d3a 2027 585f  h'.    obsm: 'X_
-00000a30: 636c 6f6e 6527 2c20 2758 5f70 6361 272c  clone', 'X_pca',
-00000a40: 2027 585f 7363 616c 6564 272c 2027 585f   'X_scaled', 'X_
-00000a50: 756d 6170 270a 6060 600a 0a23 2320 536f  umap'.```..## So
-00000a60: 7572 6365 730a 0a23 2323 2320 5265 706f  urces..#### Repo
-00000a70: 7369 746f 7269 6573 0a2a 205b 2a2a 416c  sitories.* [**Al
-00000a80: 6c6f 6e4b 6c65 696e 4c61 622a 2a2f 7061  lonKleinLab**/pa
-00000a90: 7065 722d 6461 7461 5d28 6874 7470 733a  per-data](https:
-00000aa0: 2f2f 6769 7468 7562 2e63 6f6d 2f41 6c6c  //github.com/All
-00000ab0: 6f6e 4b6c 6569 6e4c 6162 2f70 6170 6572  onKleinLab/paper
-00000ac0: 2d64 6174 612f 7472 6565 2f6d 6173 7465  -data/tree/maste
-00000ad0: 722f 4c69 6e65 6167 655f 7472 6163 696e  r/Lineage_tracin
-00000ae0: 675f 6f6e 5f74 7261 6e73 6372 6970 7469  g_on_transcripti
-00000af0: 6f6e 616c 5f6c 616e 6473 6361 7065 735f  onal_landscapes_
-00000b00: 6c69 6e6b 735f 7374 6174 655f 746f 5f66  links_state_to_f
-00000b10: 6174 655f 6475 7269 6e67 5f64 6966 6665  ate_during_diffe
-00000b20: 7265 6e74 6961 7469 6f6e 290a 2a20 5b2a  rentiation).* [*
-00000b30: 2a41 6c6c 6f6e 4b6c 6569 6e4c 6162 2a2a  *AllonKleinLab**
-00000b40: 2f4c 4152 5259 5d28 6874 7470 733a 2f2f  /LARRY](https://
-00000b50: 6769 7468 7562 2e63 6f6d 2f41 6c6c 6f6e  github.com/Allon
-00000b60: 4b6c 6569 6e4c 6162 2f4c 4152 5259 290a  KleinLab/LARRY).
-00000b70: 0a23 2323 2320 5265 6665 7265 6e63 650a  .#### Reference.
-00000b80: 2a20 5765 696e 7265 622c 2043 2e2c 2052  * Weinreb, C., R
-00000b90: 6f64 7269 6775 657a 2d46 7261 7469 6365  odriguez-Fratice
-00000ba0: 6c6c 692c 2041 2e2c 2043 616d 6172 676f  lli, A., Camargo
-00000bb0: 2c20 462e 442e 2c20 4b6c 6569 6e2c 2041  , F.D., Klein, A
-00000bc0: 2e4d 2e20 3c61 2068 7265 663d 2268 7474  .M. <a href="htt
-00000bd0: 7073 3a2f 2f73 6369 656e 6365 2e73 6369  ps://science.sci
-00000be0: 656e 6365 6d61 672e 6f72 672f 636f 6e74  encemag.org/cont
-00000bf0: 656e 742f 3336 372f 3634 3739 2f65 6161  ent/367/6479/eaa
-00000c00: 7733 3338 3122 3e2a 2a4c 696e 6561 6765  w3381">**Lineage
-00000c10: 2074 7261 6369 6e67 206f 6e20 7472 616e   tracing on tran
-00000c20: 7363 7269 7074 696f 6e61 6c20 6c61 6e64  scriptional land
-00000c30: 7363 6170 6573 206c 696e 6b73 2073 7461  scapes links sta
-00000c40: 7465 2074 6f20 6661 7465 2064 7572 696e  te to fate durin
-00000c50: 6720 6469 6666 6572 656e 7469 6174 696f  g differentiatio
-00000c60: 6e2a 2a3c 2f61 3e2e 202a 5363 6965 6e63  n**</a>. *Scienc
-00000c70: 652a 202a 2a38 302a 2a20 2832 3032 3029  e* **80** (2020)
-00000c80: 2e20 6874 7470 733a 2f2f 646f 692e 6f72  . https://doi.or
-00000c90: 672f 3130 2e31 3132 362f 7363 6965 6e63  g/10.1126/scienc
-00000ca0: 652e 6161 7733 3338 310a 0a2d 2d2d 0a0a  e.aaw3381..---..
-00000cb0: 506c 6561 7365 2065 6d61 696c 204d 6963  Please email Mic
-00000cc0: 6861 656c 2045 2e20 5669 6e79 6172 6420  hael E. Vinyard 
-00000cd0: 282a 2a6d 7669 6e79 6172 6440 6272 6f61  (**mvinyard@broa
-00000ce0: 6469 6e73 7469 7475 7465 2e6f 7267 2a2a  dinstitute.org**
-00000cf0: 2920 7769 7468 2061 6e79 2071 7565 7374  ) with any quest
-00000d00: 696f 6e73 206f 7220 696e 7465 7265 7374  ions or interest
-00000d10: 732e 200a                                s. .
+00000000: 2320 3c69 6d67 2061 6c74 3d22 4c41 5252  # <img alt="LARR
+00000010: 592d 6461 7461 7365 742d 6c6f 676f 2220  Y-dataset-logo" 
+00000020: 7372 633d 222f 646f 6373 2f69 6d67 732f  src="/docs/imgs/
+00000030: 4c41 5252 595f 6c6f 676f 2e73 7667 2220  LARRY_logo.svg" 
+00000040: 7769 6474 683d 2233 3030 223e 0a0a 5468  width="300">..Th
+00000050: 6973 2069 7320 6120 5079 7468 6f6e 2070  is is a Python p
+00000060: 6163 6b61 6765 2074 6861 7420 646f 776e  ackage that down
+00000070: 6c6f 6164 7320 616e 6420 7072 6570 726f  loads and prepro
+00000080: 6365 7373 6573 2074 6865 204c 4152 5259  cesses the LARRY
+00000090: 2064 6174 6173 6574 2066 726f 6d20 7468   dataset from th
+000000a0: 6520 416c 6c6f 6e4b 6c65 696e 4c61 6220  e AllonKleinLab 
+000000b0: 4769 7448 7562 2072 6570 6f73 6974 6f72  GitHub repositor
+000000c0: 792e 2054 6865 204c 4152 5259 2064 6174  y. The LARRY dat
+000000d0: 6173 6574 2069 7320 6120 6772 6f75 7020  aset is a group 
+000000e0: 6f66 2073 696e 676c 652d 6365 6c6c 206c  of single-cell l
+000000f0: 696e 6561 6765 2d74 7261 6365 6420 6461  ineage-traced da
+00000100: 7461 7365 7473 2074 6861 7420 6861 7665  tasets that have
+00000110: 2062 6565 6e20 7573 6564 2074 6f20 7374   been used to st
+00000120: 7564 7920 7472 616e 7363 7269 7074 696f  udy transcriptio
+00000130: 6e61 6c20 6c61 6e64 7363 6170 6573 2061  nal landscapes a
+00000140: 6e64 2063 656c 6c20 6661 7465 2064 7572  nd cell fate dur
+00000150: 696e 6720 6469 6666 6572 656e 7469 6174  ing differentiat
+00000160: 696f 6e20 5b5b 315d 2823 5265 6665 7265  ion [[1](#Refere
+00000170: 6e63 6573 295d 2e20 5468 6572 6520 6172  nces)]. There ar
+00000180: 6520 7468 7265 6520 6461 7461 7365 7473  e three datasets
+00000190: 2077 6974 6869 6e20 7468 6973 2067 726f   within this gro
+000001a0: 7570 206f 6620 6461 7461 7365 7473 2c20  up of datasets, 
+000001b0: 616c 6c20 7573 696e 6720 6865 6d61 746f  all using hemato
+000001c0: 706f 6965 7469 6320 7072 6f67 656e 6974  poietic progenit
+000001d0: 6f72 2063 656c 6c73 2066 726f 6d20 6d6f  or cells from mo
+000001e0: 7573 6520 626f 6e65 206d 6172 726f 7720  use bone marrow 
+000001f0: 616e 6420 7468 6520 4c41 5252 5920 6c65  and the LARRY le
+00000200: 6e74 6976 6972 616c 2062 6172 636f 6469  ntiviral barcodi
+00000210: 6e67 2073 7472 6174 6567 792e 0a0a 312e  ng strategy...1.
+00000220: 202a 2a2a 696e 2076 6974 726f 2a2a 2a0a   ***in vitro***.
+00000230: 322e 202a 2a2a 696e 2076 6976 6f2a 2a2a  2. ***in vivo***
+00000240: 202d 2074 7261 6e73 706c 616e 7465 6420   - transplanted 
+00000250: 696e 746f 206d 6963 650a 332e 202a 2a43  into mice.3. **C
+00000260: 7974 6f6b 696e 652d 7065 7274 7572 6265  ytokine-perturbe
+00000270: 642a 2a20 282a 696e 2076 6974 726f 2a29  d** (*in vitro*)
+00000280: 202d 2073 706c 6974 2062 6574 7765 656e   - split between
+00000290: 2076 6172 696f 7573 2063 7974 6f6b 696e   various cytokin
+000002a0: 6520 6375 6c74 7572 6520 636f 6e64 6974  e culture condit
+000002b0: 696f 6e73 2e0a 0a54 6865 2070 6163 6b61  ions...The packa
+000002c0: 6765 2069 6e63 6c75 6465 7320 6675 6e63  ge includes func
+000002d0: 7469 6f6e 7320 746f 2064 6f77 6e6c 6f61  tions to downloa
+000002e0: 6420 7468 6520 4c41 5252 5920 6461 7461  d the LARRY data
+000002f0: 7365 742c 2066 6f72 6d61 7420 7468 6520  set, format the 
+00000300: 6669 6c65 7320 696e 746f 205b 6041 6e6e  files into [`Ann
+00000310: 4461 7461 605d 2868 7474 7073 3a2f 2f61  Data`](https://a
+00000320: 6e6e 6461 7461 2e72 6561 6474 6865 646f  nndata.readthedo
+00000330: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000340: 2920 616e 6420 7065 7266 6f72 6d20 7072  ) and perform pr
+00000350: 6570 726f 6365 7373 696e 6720 2f20 6765  eprocessing / ge
+00000360: 6e65 2d66 696c 7465 7269 6e67 2073 7465  ne-filtering ste
+00000370: 7073 2e20 5468 6520 7072 6570 726f 6365  ps. The preproce
+00000380: 7373 6564 2064 6174 6120 6361 6e20 7468  ssed data can th
+00000390: 656e 2062 6520 7370 6c69 7420 696e 746f  en be split into
+000003a0: 2074 6573 7420 616e 6420 7472 6169 6e69   test and traini
+000003b0: 6e67 2073 6574 7320 666f 7220 7573 6520  ng sets for use 
+000003c0: 696e 2064 6966 6665 7265 6e74 206d 6163  in different mac
+000003d0: 6869 6e65 206c 6561 726e 696e 6720 7461  hine learning ta
+000003e0: 736b 732e 2044 696d 656e 7369 6f6e 2072  sks. Dimension r
+000003f0: 6564 7563 7469 6f6e 2063 616e 2062 6520  eduction can be 
+00000400: 7065 7266 6f72 6d65 6420 6166 7465 7220  performed after 
+00000410: 6461 7461 2073 706c 6974 7469 6e67 2074  data splitting t
+00000420: 6f20 7265 7370 6563 7420 696e 666f 726d  o respect inform
+00000430: 6174 696f 6e20 6c65 616b 6167 6520 6f72  ation leakage or
+00000440: 206f 6e20 616c 6c20 6f66 2074 6865 2064   on all of the d
+00000450: 6174 612e 0a0a 5b21 5b50 7950 4920 7079  ata...[![PyPI py
+00000460: 7665 7273 696f 6e73 5d28 6874 7470 733a  versions](https:
+00000470: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000480: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00000490: 2f6c 6172 7279 2d64 6174 6173 6574 2e73  /larry-dataset.s
+000004a0: 7667 295d 2868 7474 7073 3a2f 2f70 7970  vg)](https://pyp
+000004b0: 692e 7079 7468 6f6e 2e6f 7267 2f70 7970  i.python.org/pyp
+000004c0: 692f 6c61 7272 792d 6461 7461 7365 742f  i/larry-dataset/
+000004d0: 290a 5b21 5b50 7950 4920 7665 7273 696f  ).[![PyPI versio
+000004e0: 6e5d 2868 7474 7073 3a2f 2f62 6164 6765  n](https://badge
+000004f0: 2e66 7572 792e 696f 2f70 792f 6c61 7272  .fury.io/py/larr
+00000500: 792d 6461 7461 7365 742e 7376 6729 5d28  y-dataset.svg)](
+00000510: 6874 7470 733a 2f2f 6261 6467 652e 6675  https://badge.fu
+00000520: 7279 2e69 6f2f 7079 2f6c 6172 7279 2d64  ry.io/py/larry-d
+00000530: 6174 6173 6574 290a 5b21 5b43 6f64 6520  ataset).[![Code 
+00000540: 7374 796c 653a 2062 6c61 636b 5d28 6874  style: black](ht
+00000550: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000560: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+00000570: 3230 7374 796c 652d 626c 6163 6b2d 3030  20style-black-00
+00000580: 3030 3030 2e73 7667 295d 2868 7474 7073  0000.svg)](https
+00000590: 3a2f 2f67 6974 6875 622e 636f 6d2f 7073  ://github.com/ps
+000005a0: 662f 626c 6163 6b29 0a0a 2323 2049 6e73  f/black)..## Ins
+000005b0: 7461 6c6c 6174 696f 6e0a 0a23 2323 2320  tallation..#### 
+000005c0: 5b60 7069 7060 5d28 2920 6469 7374 7269  [`pip`]() distri
+000005d0: 6275 7469 6f6e 0a60 6060 4241 5348 0a70  bution.```BASH.p
+000005e0: 6970 2069 6e73 7461 6c6c 206c 6172 7279  ip install larry
+000005f0: 2d64 6174 6173 6574 0a60 6060 0a0a 2323  -dataset.```..##
+00000600: 2323 2044 6576 656c 6f70 6d65 6e74 2076  ## Development v
+00000610: 6572 7369 6f6e 0a60 6060 4241 5348 0a67  ersion.```BASH.g
+00000620: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000630: 2f67 6974 6875 622e 636f 6d2f 6d76 696e  /github.com/mvin
+00000640: 7961 7264 2f4c 4152 5259 2d64 6174 6173  yard/LARRY-datas
+00000650: 6574 2e67 6974 3b20 6364 204c 4152 5259  et.git; cd LARRY
+00000660: 2d64 6174 6173 6574 0a0a 7069 7020 696e  -dataset..pip in
+00000670: 7374 616c 6c20 2d65 202e 0a60 6060 0a0a  stall -e ..```..
+00000680: 2323 2051 7569 636b 7374 6172 740a 446f  ## Quickstart.Do
+00000690: 776e 6c6f 6164 7320 7072 652d 7072 6f63  wnloads pre-proc
+000006a0: 6573 7365 6420 6461 7461 2066 726f 6d20  essed data from 
+000006b0: 5b2a 2a41 6c6c 6f6e 4b6c 6569 6e4c 6162  [**AllonKleinLab
+000006c0: 2a2a 2f70 6170 6572 2d64 6174 615d 2868  **/paper-data](h
+000006d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000006e0: 6d2f 416c 6c6f 6e4b 6c65 696e 4c61 622f  m/AllonKleinLab/
+000006f0: 7061 7065 722d 6461 7461 2f74 7265 652f  paper-data/tree/
+00000700: 6d61 7374 6572 2f4c 696e 6561 6765 5f74  master/Lineage_t
+00000710: 7261 6369 6e67 5f6f 6e5f 7472 616e 7363  racing_on_transc
+00000720: 7269 7074 696f 6e61 6c5f 6c61 6e64 7363  riptional_landsc
+00000730: 6170 6573 5f6c 696e 6b73 5f73 7461 7465  apes_links_state
+00000740: 5f74 6f5f 6661 7465 5f64 7572 696e 675f  _to_fate_during_
+00000750: 6469 6666 6572 656e 7469 6174 696f 6e29  differentiation)
+00000760: 2074 6f20 602e 2f4b 6c65 696e 4c61 6244   to `./KleinLabD
+00000770: 6174 6160 2028 6279 2064 6566 6175 6c74  ata` (by default
+00000780: 292e 2054 6865 2064 6174 6120 6973 2066  ). The data is f
+00000790: 6f72 6d61 7474 6564 2069 6e74 6f20 5b60  ormatted into [`
+000007a0: 416e 6e44 6174 6160 5d28 6874 7470 733a  AnnData`](https:
+000007b0: 2f2f 616e 6e64 6174 612e 7265 6164 7468  //anndata.readth
+000007c0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000007d0: 7374 2f29 2061 6e64 2072 6574 7572 6e65  st/) and returne
+000007e0: 6420 746f 2074 6865 2075 7365 722e 2041  d to the user. A
+000007f0: 2060 2e68 3561 6460 2066 696c 6520 6973   `.h5ad` file is
+00000800: 2061 6c73 6f20 7361 7665 642c 206c 6f63   also saved, loc
+00000810: 616c 6c79 2e20 5468 6520 6461 7461 2064  ally. The data d
+00000820: 6f77 6e6c 6f61 6469 6e67 2061 6e64 2063  ownloading and c
+00000830: 6f6e 7665 7273 696f 6e20 7374 6570 2074  onversion step t
+00000840: 616b 6520 7365 7665 7261 6c20 6d69 6e75  ake several minu
+00000850: 7465 7320 6475 6520 746f 2074 6865 206c  tes due to the l
+00000860: 6172 6765 2065 7870 7265 7373 696f 6e20  arge expression 
+00000870: 606e 6f72 6d65 645f 636f 756e 7473 6020  `normed_counts` 
+00000880: 6d61 7472 6963 6573 2074 686f 7567 6820  matrices though 
+00000890: 7468 6973 206f 6e6c 7920 6861 7070 656e  this only happen
+000008a0: 7320 6f6e 6365 2e0a 0a60 6060 7079 7468  s once...```pyth
+000008b0: 6f6e 0a69 6d70 6f72 7420 6c61 7272 790a  on.import larry.
+000008c0: 2020 2020 0a64 6174 6173 6574 203d 2022      .dataset = "
+000008d0: 696e 5f76 6974 726f 2220 2320 6361 6e20  in_vitro" # can 
+000008e0: 616c 736f 2063 686f 6f73 6520 6672 6f6d  also choose from
+000008f0: 3a20 2269 6e5f 7669 766f 2220 6f72 2022  : "in_vivo" or "
+00000900: 6379 746f 6b69 6e65 5f70 6572 7475 7262  cytokine_perturb
+00000910: 6174 696f 6e22 0a61 6461 7461 203d 206c  ation".adata = l
+00000920: 6172 7279 2e66 6574 6368 2864 6174 6173  arry.fetch(datas
+00000930: 6574 290a 6060 600a 6060 600a 416e 6e44  et).```.```.AnnD
+00000940: 6174 6120 6f62 6a65 6374 2077 6974 6820  ata object with 
+00000950: 6e5f 6f62 7320 c397 206e 5f76 6172 7320  n_obs .. n_vars 
+00000960: 3d20 3133 3038 3837 20c3 9720 3235 3238  = 130887 .. 2528
+00000970: 390a 2020 2020 6f62 733a 2027 4c69 6272  9.    obs: 'Libr
+00000980: 6172 7927 2c20 2743 656c 6c20 6261 7263  ary', 'Cell barc
+00000990: 6f64 6527 2c20 2754 696d 6520 706f 696e  ode', 'Time poin
+000009a0: 7427 2c20 2753 7461 7274 696e 6720 706f  t', 'Starting po
+000009b0: 7075 6c61 7469 6f6e 272c 2027 4365 6c6c  pulation', 'Cell
+000009c0: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
+000009d0: 272c 2027 5765 6c6c 272c 2027 5350 5249  ', 'Well', 'SPRI
+000009e0: 4e47 2d78 272c 2027 5350 5249 4e47 2d79  NG-x', 'SPRING-y
+000009f0: 270a 2020 2020 7661 723a 2027 6765 6e65  '.    var: 'gene
+00000a00: 5f6e 616d 6527 0a20 2020 206f 6273 6d3a  _name'.    obsm:
+00000a10: 2027 585f 636c 6f6e 6527 0a60 6060 0a0a   'X_clone'.```..
+00000a20: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00000a30: 206c 6172 7279 0a0a 4c41 5252 595f 4c69   larry..LARRY_Li
+00000a40: 6768 746e 696e 6744 6174 6120 3d20 6c61  ghtningData = la
+00000a50: 7272 792e 4c41 5252 595f 4c69 6768 746e  rry.LARRY_Lightn
+00000a60: 696e 6744 6174 614d 6f64 756c 6528 290a  ingDataModule().
+00000a70: 4c41 5252 595f 4c69 6768 746e 696e 6744  LARRY_LightningD
+00000a80: 6174 612e 7072 6570 6172 655f 6461 7461  ata.prepare_data
+00000a90: 2829 0a60 6060 0a60 6060 0a20 416e 6e44  ().```.```. AnnD
+00000aa0: 6174 6120 6f62 6a65 6374 2077 6974 6820  ata object with 
+00000ab0: 6e5f 6f62 7320 c397 206e 5f76 6172 7320  n_obs .. n_vars 
+00000ac0: 3d20 3133 3038 3837 20c3 9720 3235 3238  = 130887 .. 2528
+00000ad0: 390a 2020 2020 6f62 733a 2027 4c69 6272  9.    obs: 'Libr
+00000ae0: 6172 7927 2c20 2743 656c 6c20 6261 7263  ary', 'Cell barc
+00000af0: 6f64 6527 2c20 2754 696d 6520 706f 696e  ode', 'Time poin
+00000b00: 7427 2c20 2753 7461 7274 696e 6720 706f  t', 'Starting po
+00000b10: 7075 6c61 7469 6f6e 272c 2027 4365 6c6c  pulation', 'Cell
+00000b20: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
+00000b30: 272c 2027 5765 6c6c 272c 2027 5350 5249  ', 'Well', 'SPRI
+00000b40: 4e47 2d78 272c 2027 5350 5249 4e47 2d79  NG-x', 'SPRING-y
+00000b50: 270a 2020 2020 7661 723a 2027 6765 6e65  '.    var: 'gene
+00000b60: 5f6e 616d 6527 0a20 2020 2075 6e73 3a20  _name'.    uns: 
+00000b70: 2764 6174 6173 6574 272c 2027 6835 6164  'dataset', 'h5ad
+00000b80: 5f70 6174 6827 0a20 2020 206f 6273 6d3a  _path'.    obsm:
+00000b90: 2027 585f 636c 6f6e 6527 0a50 7265 7072   'X_clone'.Prepr
+00000ba0: 6f63 6573 7369 6e67 2070 6572 666f 726d  ocessing perform
+00000bb0: 6564 2070 7265 7669 6f75 736c 792e 204c  ed previously. L
+00000bc0: 6f61 6469 6e67 2e2e 2e64 6f6e 652e 0a60  oading...done..`
+00000bd0: 6060 0a55 6e64 6572 2074 6865 2068 6f6f  ``.Under the hoo
+00000be0: 642c 2074 6865 2060 4c41 5252 595f 4c69  d, the `LARRY_Li
+00000bf0: 6768 746e 696e 6744 6174 6160 2063 616c  ghtningData` cal
+00000c00: 6c73 2060 6c61 7272 792e 6665 7463 6828  ls `larry.fetch(
+00000c10: 2960 2061 6e64 2060 6c61 7272 792e 7070  )` and `larry.pp
+00000c20: 2e59 656f 3230 3231 5f72 6563 6970 6528  .Yeo2021_recipe(
+00000c30: 2960 2c20 616e 6420 6966 2060 7461 736b  )`, and if `task
+00000c40: 203d 3d20 2266 6174 655f 7072 6564 6963   == "fate_predic
+00000c50: 7469 6f6e 2260 2c20 606c 6172 7279 2e70  tion"`, `larry.p
+00000c60: 702e 616e 6e6f 7461 7465 5f66 6174 655f  p.annotate_fate_
+00000c70: 7465 7374 5f74 7261 696e 2829 6020 0a0a  test_train()` ..
+00000c80: 6060 6070 7974 686f 6e0a 4c41 5252 595f  ```python.LARRY_
+00000c90: 4c69 6768 746e 696e 6744 6174 612e 6164  LightningData.ad
+00000ca0: 6174 610a 6060 600a 5072 696e 7420 7468  ata.```.Print th
+00000cb0: 6520 7570 6461 7465 6420 6061 6461 7461  e updated `adata
+00000cc0: 603a 0a60 6060 0a41 6e6e 4461 7461 206f  `:.```.AnnData o
+00000cd0: 626a 6563 7420 7769 7468 206e 5f6f 6273  bject with n_obs
+00000ce0: 20c3 9720 6e5f 7661 7273 203d 2031 3330   .. n_vars = 130
+00000cf0: 3838 3720 c397 2032 3532 3839 0a20 2020  887 .. 25289.   
+00000d00: 206f 6273 3a20 274c 6962 7261 7279 272c   obs: 'Library',
+00000d10: 2027 4365 6c6c 2062 6172 636f 6465 272c   'Cell barcode',
+00000d20: 2027 5469 6d65 2070 6f69 6e74 272c 2027   'Time point', '
+00000d30: 5374 6172 7469 6e67 2070 6f70 756c 6174  Starting populat
+00000d40: 696f 6e27 2c20 2743 656c 6c20 7479 7065  ion', 'Cell type
+00000d50: 2061 6e6e 6f74 6174 696f 6e27 2c20 2757   annotation', 'W
+00000d60: 656c 6c27 2c20 2753 5052 494e 472d 7827  ell', 'SPRING-x'
+00000d70: 2c20 2753 5052 494e 472d 7927 2c20 2763  , 'SPRING-y', 'c
+00000d80: 656c 6c5f 6964 7827 2c20 2763 6c6f 6e65  ell_idx', 'clone
+00000d90: 5f69 6478 270a 2020 2020 7661 723a 2027  _idx'.    var: '
+00000da0: 6765 6e65 5f6e 616d 6527 2c20 2768 6967  gene_name', 'hig
+00000db0: 686c 795f 7661 7269 6162 6c65 272c 2027  hly_variable', '
+00000dc0: 636f 7272 5f63 656c 6c5f 6379 636c 6527  corr_cell_cycle'
+00000dd0: 2c20 2770 6173 735f 6669 6c74 6572 270a  , 'pass_filter'.
+00000de0: 2020 2020 756e 733a 2027 6461 7461 7365      uns: 'datase
+00000df0: 7427 2c20 2768 3561 645f 7061 7468 272c  t', 'h5ad_path',
+00000e00: 2027 6869 6768 6c79 5f76 6172 6961 626c   'highly_variabl
+00000e10: 655f 6765 6e65 735f 6964 7827 2c20 276e  e_genes_idx', 'n
+00000e20: 5f63 6f72 725f 6365 6c6c 5f63 7963 6c65  _corr_cell_cycle
+00000e30: 272c 2027 6e5f 6876 272c 2027 6e5f 6d69  ', 'n_hv', 'n_mi
+00000e40: 746f 272c 2027 6e5f 7061 7373 272c 2027  to', 'n_pass', '
+00000e50: 6e5f 746f 7461 6c27 2c20 2770 705f 6835  n_total', 'pp_h5
+00000e60: 6164 5f70 6174 6827 0a20 2020 206f 6273  ad_path'.    obs
+00000e70: 6d3a 2027 585f 636c 6f6e 6527 2c20 2758  m: 'X_clone', 'X
+00000e80: 5f70 6361 272c 2027 585f 7363 616c 6564  _pca', 'X_scaled
+00000e90: 272c 2027 585f 756d 6170 270a 6060 600a  ', 'X_umap'.```.
+00000ea0: 0a23 2320 536f 7572 6365 730a 0a23 2323  .## Sources..###
+00000eb0: 2320 5265 706f 7369 746f 7269 6573 0a2a  # Repositories.*
+00000ec0: 205b 2a2a 416c 6c6f 6e4b 6c65 696e 4c61   [**AllonKleinLa
+00000ed0: 622a 2a2f 7061 7065 722d 6461 7461 5d28  b**/paper-data](
+00000ee0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000ef0: 6f6d 2f41 6c6c 6f6e 4b6c 6569 6e4c 6162  om/AllonKleinLab
+00000f00: 2f70 6170 6572 2d64 6174 612f 7472 6565  /paper-data/tree
+00000f10: 2f6d 6173 7465 722f 4c69 6e65 6167 655f  /master/Lineage_
+00000f20: 7472 6163 696e 675f 6f6e 5f74 7261 6e73  tracing_on_trans
+00000f30: 6372 6970 7469 6f6e 616c 5f6c 616e 6473  criptional_lands
+00000f40: 6361 7065 735f 6c69 6e6b 735f 7374 6174  capes_links_stat
+00000f50: 655f 746f 5f66 6174 655f 6475 7269 6e67  e_to_fate_during
+00000f60: 5f64 6966 6665 7265 6e74 6961 7469 6f6e  _differentiation
+00000f70: 290a 2a20 5b2a 2a41 6c6c 6f6e 4b6c 6569  ).* [**AllonKlei
+00000f80: 6e4c 6162 2a2a 2f4c 4152 5259 5d28 6874  nLab**/LARRY](ht
+00000f90: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000fa0: 2f41 6c6c 6f6e 4b6c 6569 6e4c 6162 2f4c  /AllonKleinLab/L
+00000fb0: 4152 5259 290a 0a23 2323 2320 5265 6665  ARRY)..#### Refe
+00000fc0: 7265 6e63 6573 0a31 2e20 5765 696e 7265  rences.1. Weinre
+00000fd0: 622c 2043 2e2c 2052 6f64 7269 6775 657a  b, C., Rodriguez
+00000fe0: 2d46 7261 7469 6365 6c6c 692c 2041 2e2c  -Fraticelli, A.,
+00000ff0: 2043 616d 6172 676f 2c20 462e 442e 2c20   Camargo, F.D., 
+00001000: 4b6c 6569 6e2c 2041 2e4d 2e20 3c61 2068  Klein, A.M. <a h
+00001010: 7265 663d 2268 7474 7073 3a2f 2f73 6369  ref="https://sci
+00001020: 656e 6365 2e73 6369 656e 6365 6d61 672e  ence.sciencemag.
+00001030: 6f72 672f 636f 6e74 656e 742f 3336 372f  org/content/367/
+00001040: 3634 3739 2f65 6161 7733 3338 3122 3e2a  6479/eaaw3381">*
+00001050: 2a4c 696e 6561 6765 2074 7261 6369 6e67  *Lineage tracing
+00001060: 206f 6e20 7472 616e 7363 7269 7074 696f   on transcriptio
+00001070: 6e61 6c20 6c61 6e64 7363 6170 6573 206c  nal landscapes l
+00001080: 696e 6b73 2073 7461 7465 2074 6f20 6661  inks state to fa
+00001090: 7465 2064 7572 696e 6720 6469 6666 6572  te during differ
+000010a0: 656e 7469 6174 696f 6e2a 2a3c 2f61 3e2e  entiation**</a>.
+000010b0: 202a 5363 6965 6e63 652a 202a 2a38 302a   *Science* **80*
+000010c0: 2a20 2832 3032 3029 2e20 6874 7470 733a  * (2020). https:
+000010d0: 2f2f 646f 692e 6f72 672f 3130 2e31 3132  //doi.org/10.112
+000010e0: 362f 7363 6965 6e63 652e 6161 7733 3338  6/science.aaw338
+000010f0: 310a 0a2d 2d2d 0a0a 506c 6561 7365 2065  1..---..Please e
+00001100: 6d61 696c 204d 6963 6861 656c 2045 2e20  mail Michael E. 
+00001110: 5669 6e79 6172 6420 282a 2a6d 7669 6e79  Vinyard (**mviny
+00001120: 6172 6440 6272 6f61 6469 6e73 7469 7475  ard@broadinstitu
+00001130: 7465 2e6f 7267 2a2a 2920 7769 7468 2061  te.org**) with a
+00001140: 6e79 2071 7565 7374 696f 6e73 206f 7220  ny questions or 
+00001150: 696e 7465 7265 7374 732e 200a            interests. .
```

### Comparing `LARRY-dataset-0.0.1/setup.py` & `LARRY-dataset-0.0.2rc0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import setuptools
 import re
 import os
 import sys
 
 setuptools.setup(
     name='LARRY-dataset',
-    version='0.0.1',
-    python_requires='>3.7.0',
+    version='0.0.2rc0',
+    python_requires='>3.9.0',
     author='Michael E. Vinyard - Harvard University - Massachussetts General Hospital - Broad Institute of MIT and Harvard',
     author_email='mvinyard@broadinstitute.org',
     url = 'https://github.com/pinellolab/LARRY-dataset',
     long_description = open("README.md", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
     description='LARRY Dataset: lineage and RNA recovery',
     packages = setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
-        "anndata>=0.8",
-        "pytorch-lightning>=1.7.5",
+        "anndata>=0.9.1",
+        "pytorch-lightning>=2.0.2",
         "wget>=3.2",
     ],
     classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.7",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
```

