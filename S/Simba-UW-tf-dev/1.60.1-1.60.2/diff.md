# Comparing `tmp/Simba-UW-tf-dev-1.60.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.60.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.1.tar", last modified: Fri May 19 21:16:11 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.60.2.tar", last modified: Sat May 20 12:38:25 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.60.1.tar` & `Simba-UW-tf-dev-1.60.2.tar`

### file list

```diff
@@ -1,504 +1,504 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.60.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15019 2023-05-19 18:30:31.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.60.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.60.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.60.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.1/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.60.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.1/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15608 2023-05-19 15:09:35.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13334 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.1/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19618 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-19 21:16:10.000000 Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.1/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-19 21:16:04.000000 Simba-UW-tf-dev-1.60.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-19 21:16:11.000000 Simba-UW-tf-dev-1.60.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-15 16:18:07.000000 Simba-UW-tf-dev-1.60.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-15 16:18:02.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3301 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6352 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12660 2023-05-16 16:46:42.000000 Simba-UW-tf-dev-1.60.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.60.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.60.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26536 2023-05-14 19:57:32.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.60.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:05.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-19 21:21:01.000000 Simba-UW-tf-dev-1.60.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     8242 2023-05-15 00:06:27.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15449 2023-04-30 14:02:53.000000 Simba-UW-tf-dev-1.60.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42134 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    29846 2023-05-19 16:02:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49963 2023-04-29 19:21:39.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:51:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    50201 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51865 2023-05-19 17:46:16.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-25 20:46:51.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    81535 2023-05-16 17:47:34.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    49894 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-04-24 19:06:57.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51139 2023-05-11 23:17:43.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-09 14:36:36.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.60.2/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6130 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17166 2023-05-04 17:44:05.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18224 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6992 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5281 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.60.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.60.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-08 20:24:55.000000 Simba-UW-tf-dev-1.60.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.60.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    41533 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.60.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.60.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.60.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    15392 2023-05-15 15:08:26.000000 Simba-UW-tf-dev-1.60.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.60.2/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.60.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13144 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12486 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13718 2023-05-15 18:46:07.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11204 2023-05-15 18:33:52.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9225 2023-05-15 18:46:34.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     6501 2023-05-18 22:42:15.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8404 2023-05-18 17:24:33.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12908 2023-05-18 13:34:46.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7654 2023-05-18 15:26:11.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.60.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.60.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.60.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.60.2/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.60.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-14 23:29:04.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    64830 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.60.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.60.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.60.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.60.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.60.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19618 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-20 12:38:24.000000 Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.60.2/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.60.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.60.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-20 12:38:16.000000 Simba-UW-tf-dev-1.60.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-20 12:38:25.000000 Simba-UW-tf-dev-1.60.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.60.1/PKG-INFO` & `Simba-UW-tf-dev-1.60.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.1
+Version: 1.60.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,28 +28,30 @@
         PopUpMixin.__init__(self, title='CREATE PATH PLOTS')
         self.resolutions.insert(0, 'As input')
         self.animal_cnt_options = list(range(1, self.animal_cnt+1))
 
         self.style_settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='STYLE SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.PATH_PLOTS.value)
         self.autocompute_var = BooleanVar(value=True)
         self.auto_compute_styles = Checkbutton(self.style_settings_frm, text='Auto-compute styles', variable=self.autocompute_var, command=self.enable_style_settings)
+        self.max_prior_lines_dropdown = DropDownMenu(self.style_settings_frm, 'Max prior lines:', ['Entire video', 'Specify milliseconds'], '16', com=self.enable_entrybox_from_dropdown)
+        self.max_lines_entry = Entry_Box(self.style_settings_frm, 'Max prior lines (ms): ', '16', validation='numeric')
         self.resolution_dropdown = DropDownMenu(self.style_settings_frm, 'Resolution:', self.resolutions, '16')
         self.bg_clr_dropdown = DropDownMenu(self.style_settings_frm, 'Background color:', list(self.colors_dict.keys()), '16')
-
         self.line_width = Entry_Box(self.style_settings_frm, 'Line width: ', '16', validation='numeric')
-        self.max_lines_entry = Entry_Box(self.style_settings_frm, 'Max prior lines (ms): ', '16', validation='numeric')
         self.font_size = Entry_Box(self.style_settings_frm, 'Font size: ', '16', validation='numeric')
         self.font_thickness = Entry_Box(self.style_settings_frm, 'Font thickness: ', '16', validation='numeric')
         self.circle_size = Entry_Box(self.style_settings_frm, 'Circle size: ', '16', validation='numeric')
         self.resolution_dropdown.setChoices(self.resolutions[0])
         self.line_width.entry_set(val=6)
         self.bg_clr_dropdown.setChoices('White')
         self.circle_size.entry_set(val=20)
         self.font_size.entry_set(val=3)
         self.font_thickness.entry_set(val=2)
+        self.max_prior_lines_dropdown.setChoices('Entire video')
+        self.max_prior_lines_dropdown.disable()
         self.max_lines_entry.entry_set(2000)
         self.resolution_dropdown.disable()
         self.line_width.set_state("disable")
         self.bg_clr_dropdown.disable()
         self.circle_size.set_state("disable")
         self.font_size.set_state("disable")
         self.max_lines_entry.set_state("disable")
@@ -61,15 +63,14 @@
 
         self.clf_frm = LabelFrame(self.main_frm, text='CHOOSE CLASSIFICATION VISUALIZATION', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5)
         self.include_clf_locations_var = BooleanVar(value=False)
         self.include_clf_locations_cb = Checkbutton(self.clf_frm, text='Include classification locations', variable=self.include_clf_locations_var, command=self.populate_clf_location_data)
         self.include_clf_locations_cb.grid(row=0, sticky=NW)
         self.populate_clf_location_data()
 
-
         self.populate_body_parts_menu(self.animal_cnt_options[0])
         self.settings_frm = LabelFrame(self.main_frm, text='VISUALIZATION SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value, pady=5, padx=5)
         self.path_frames_var = BooleanVar()
         self.path_videos_var = BooleanVar()
         self.path_last_frm_var = BooleanVar()
         self.multiprocessing_var = BooleanVar()
         path_frames_cb = Checkbutton(self.settings_frm, text='Create frames', variable=self.path_frames_var)
@@ -88,20 +89,21 @@
 
         self.run_multiple_videos = LabelFrame(self.run_frm, text='MULTIPLE VIDEO', font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5, padx=5, fg='black')
         self.run_multiple_video_btn = Button(self.run_multiple_videos, text='Create multiple videos ({} video(s) found)'.format(str(len(list(self.files_found_dict.keys())))), fg='blue', command= lambda: self.__create_path_plots(multiple_videos=True))
 
         self.style_settings_frm.grid(row=0, sticky=NW)
         self.auto_compute_styles.grid(row=0, sticky=NW)
         self.resolution_dropdown.grid(row=1, sticky=NW)
-        self.max_lines_entry.grid(row=2, sticky=NW)
-        self.line_width.grid(row=3, sticky=NW)
-        self.circle_size.grid(row=4, sticky=NW)
-        self.font_size.grid(row=5, sticky=NW)
-        self.font_thickness.grid(row=6, sticky=NW)
-        self.bg_clr_dropdown.grid(row=7, sticky=NW)
+        self.max_prior_lines_dropdown.grid(row=2, sticky=NW)
+        self.max_lines_entry.grid(row=3, sticky=NW)
+        self.line_width.grid(row=4, sticky=NW)
+        self.circle_size.grid(row=5, sticky=NW)
+        self.font_size.grid(row=6, sticky=NW)
+        self.font_thickness.grid(row=7, sticky=NW)
+        self.bg_clr_dropdown.grid(row=8, sticky=NW)
 
         self.clf_frm.grid(row=1, sticky=NW)
 
         self.body_parts_frm.grid(row=2, sticky=NW)
         self.number_of_animals_dropdown.grid(row=0, sticky=NW)
 
         self.settings_frm.grid(row=3, sticky=NW)
@@ -164,25 +166,34 @@
                 self.clf_size[clf_cnt].enable()
         else:
             for clf_cnt in self.clf_name.keys():
                 self.clf_name[clf_cnt].disable()
                 self.clf_clr[clf_cnt].disable()
                 self.clf_size[clf_cnt].disable()
 
+    def enable_entrybox_from_dropdown(self, dropdown_selection):
+        if dropdown_selection == 'Entire video':
+            self.max_lines_entry.set_state('disable')
+        else:
+            self.max_lines_entry.set_state('normal')
+
     def enable_style_settings(self):
         if not self.autocompute_var.get():
             self.resolution_dropdown.enable()
+            self.max_prior_lines_dropdown.enable()
             self.max_lines_entry.set_state('normal')
             self.line_width.set_state('normal')
             self.font_thickness.set_state("normal")
             self.circle_size.set_state('normal')
             self.font_size.set_state('normal')
             self.bg_clr_dropdown.enable()
+            self.enable_entrybox_from_dropdown(self.max_prior_lines_dropdown.getChoices())
         else:
             self.resolution_dropdown.disable()
+            self.max_prior_lines_dropdown.disable()
             self.max_lines_entry.set_state('disable')
             self.font_thickness.set_state("disable")
             self.line_width.set_state('disable')
             self.circle_size.set_state('disable')
             self.font_size.set_state('disable')
             self.bg_clr_dropdown.disable()
 
@@ -195,26 +206,30 @@
                 width = int(self.resolution_dropdown.getChoices().split('×')[0])
                 height = int(self.resolution_dropdown.getChoices().split('×')[1])
             else:
                 width, height = 'As input', 'As input'
             check_int(name='PATH LINE WIDTH', value=self.line_width.entry_get, min_value=1)
             check_int(name='PATH CIRCLE SIZE', value=self.circle_size.entry_get, min_value=1)
             check_int(name='PATH FONT SIZE', value=self.font_size.entry_get, min_value=1)
-            check_int(name='PATH MAX LINES', value=self.max_lines_entry.entry_get, min_value=1)
             check_int(name='FONT THICKNESS', value=self.font_thickness.entry_get, min_value=1)
             style_attr = {'width': width,
                           'height': height,
                           'line width': int(self.line_width.entry_get),
                           'font size': int(self.font_size.entry_get),
                           'font thickness': int(self.font_thickness.entry_get),
                           'circle size': int(self.circle_size.entry_get),
                           'bg color': self.bg_clr_dropdown.getChoices(),
-                          'max lines': int(self.max_lines_entry.entry_get),
                           'clf locations': self.include_clf_locations_var.get()}
 
+            if self.max_prior_lines_dropdown.getChoices() == 'Entire video':
+                style_attr['max lines'] = 'entire video'
+            else:
+                check_int(name='PATH MAX LINES', value=self.max_lines_entry.entry_get, min_value=1)
+                style_attr['max lines'] = self.max_lines_entry.entry_get
+
         animal_attr = defaultdict(list)
         for attr in (self.bp_dropdowns, self.bp_colors):
             for key, value in attr.items():
                 animal_attr[key].append(value.getChoices())
 
         clf_attr = None
         if self.include_clf_locations_var.get():
@@ -246,8 +261,8 @@
                                                 input_style_attr=style_attr,
                                                 animal_attr=animal_attr,
                                                 input_clf_attr=clf_attr,
                                                 cores=int(self.multiprocess_dropdown.getChoices()))
 
         path_plotter.run()
 
-#_ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
+#_ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.60.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.60.2/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.60.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.60.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.60.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.60.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -743,16 +743,16 @@
 00002e60: 01aa 01b3 0000 0000 0000 0201 0000 0000  ................
 00002e70: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
 00002e80: 0000 01b4 0000 000c 0075 006e 0073 0075  .........u.n.s.u
 00002e90: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
 00002ea0: 6d6f 4444 626c 6f62 0000 0008 04d0 54a0  moDDblob......T.
 00002eb0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
 00002ec0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-00002ed0: 6d6f 6444 626c 6f62 0000 0008 6269 0543  modDblob....bi.C
-00002ee0: 3a05 c541 0000 000c 0075 006e 0073 0075  :..A.....u.n.s.u
+00002ed0: 6d6f 6444 626c 6f62 0000 0008 04d0 54a0  modDblob......T.
+00002ee0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
 00002ef0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
 00002f00: 7068 3153 636f 6d70 0000 0000 0009 b000  ph1Scomp........
 00002f10: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
 00002f20: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
 00002f30: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
 00002f40: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
 00002f50: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
@@ -1281,16 +1281,16 @@
 00005000: 0000 0000 0000 0000 0000 001d 0000 0012  ................
 00005010: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 00005020: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 00005030: 006c 0073 6d6f 4444 626c 6f62 0000 0008  .l.smoDDblob....
 00005040: 1fe8 e082 4c09 c541 0000 0012 0062 006f  ....L..A.....b.o
 00005050: 0075 006e 0064 0069 006e 0067 005f 0062  .u.n.d.i.n.g._.b
 00005060: 006f 0078 005f 0074 006f 006f 006c 0073  .o.x._.t.o.o.l.s
-00005070: 6d6f 6444 626c 6f62 0000 0008 5311 5fb9  modDblob....S._.
-00005080: 9505 c541 0000 0012 0062 006f 0075 006e  ...A.....b.o.u.n
+00005070: 6d6f 6444 626c 6f62 0000 0008 1fe8 e082  modDblob........
+00005080: 4c09 c541 0000 0012 0062 006f 0075 006e  L..A.....b.o.u.n
 00005090: 0064 0069 006e 0067 005f 0062 006f 0078  .d.i.n.g._.b.o.x
 000050a0: 005f 0074 006f 006f 006c 0073 7068 3153  ._.t.o.o.l.sph1S
 000050b0: 636f 6d70 0000 0000 0003 c000 0000 0012  comp............
 000050c0: 0062 006f 0075 006e 0064 0069 006e 0067  .b.o.u.n.d.i.n.g
 000050d0: 005f 0062 006f 0078 005f 0074 006f 006f  ._.b.o.x._.t.o.o
 000050e0: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
 000050f0: 0000 000f 0063 0075 0065 005f 006c 0069  .....c.u.e._.l.i
@@ -1360,25 +1360,25 @@
 000054f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00005500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
 00005510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
 00005520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 00005530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 00005540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 00005550: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-00005560: 7b7b 3131 322c 2035 357d 2c20 7b31 3139  {{112, 55}, {119
-00005570: 392c 2037 3639 7d7d 0908 1725 313d 4960  9, 769}}...%1=I`
+00005560: 7b7b 3333 352c 2031 3938 7d2c 207b 3932  {{335, 198}, {92
+00005570: 372c 2035 3638 7d7d 0908 1725 313d 4960  7, 568}}...%1=I`
 00005580: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
 00005590: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 000055a0: 0000 0000 0000 009a 0000 000f 0064 0061  .............d.a
 000055b0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 000055c0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
 000055d0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
 000055e0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000055f0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-00005600: 0000 0453 9a00 0000 0f00 6400 6100 7400  ...S......d.a.t.
+00005600: 0000 0459 f000 0000 0f00 6400 6100 7400  ...Y......d.a.t.
 00005610: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005620: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
 00005630: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
 00005640: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
 00005650: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
 00005660: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
 00005670: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
@@ -1457,19 +1457,19 @@
 00005b00: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
 00005b10: 0180 0181 0183 018c 018d 0190 0191 0193  ................
 00005b20: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
 00005b30: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
 00005b40: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
 00005b50: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 00005b60: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00005b70: 6f62 0000 0008 3ebd 23b1 6d0b c541 0000  ob....>.#.m..A..
+00005b70: 6f62 0000 0008 10ae 0e75 fb0b c541 0000  ob.......u...A..
 00005b80: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
 00005b90: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
-00005ba0: 6d6f 6444 626c 6f62 0000 0008 b622 20d2  modDblob....." .
-00005bb0: 610b c541 0000 000f 0064 0061 0074 0061  a..A.....d.a.t.a
+00005ba0: 6d6f 6444 626c 6f62 0000 0008 10ae 0e75  modDblob.......u
+00005bb0: fb0b c541 0000 000f 0064 0061 0074 0061  ...A.....d.a.t.a
 00005bc0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00005bd0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
 00005be0: 0000 0005 b000 0000 000f 0064 0061 0074  ...........d.a.t
 00005bf0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005c00: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
 00005c10: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
 00005c20: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
@@ -1489,15 +1489,15 @@
 00005d00: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 9a00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00005d20: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00005d30: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00005d40: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00005d50: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d60: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d70: 6d70 0000 0000 0015 61e0 5863 6f6d 6d65  mp......a.Xcomme
+00005d70: 6d70 0000 0000 0016 34fb 5863 6f6d 6d65  mp......4.Xcomme
 00005d80: 6e74 73d4 0d0e 0f10 163e 1640 0810 c808  nts......>.@....
 00005d90: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
 00005da0: 0d0e 0f10 161c 1644 0808 5964 6174 6541  .......D..YdateA
 00005db0: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
 00005dc0: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
 00005dd0: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
 00005de0: 8c00 8e00 8f00 9b00 a400 ac00 b200 bc00  ................
@@ -1586,185 +1586,185 @@
 00006310: 086f ba2a 3a04 0cc5 4100 0000 1200 6600  .o.*:...A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
 00006340: 736d 6f64 4462 6c6f 6200 0000 086f ba2a  smodDblob....o.*
 00006350: 3a04 0cc5 4100 0000 1200 6600 6500 6100  :...A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 1820 0000 0000  Scomp...... ....
+00006380: 5363 6f6d 7000 0000 0000 1900 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
-000063e0: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
+000063e0: 0000 c962 706c 6973 7430 30d7 0102 0304  ...bplist00.....
 000063f0: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
 00006400: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
 00006410: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
 00006420: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
 00006430: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
 00006440: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
 00006450: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-00006460: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
-00006470: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
-00006480: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
-00006490: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000064a0: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
-000064b0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
-000064c0: 6e00 676c 6731 5363 6f6d 7000 0000 0000  n.glg1Scomp.....
-000064d0: 0240 7500 0000 0900 6c00 6100 6200 6500  .@u.....l.a.b.e.
-000064e0: 6c00 6c00 6900 6e00 676c 7376 4362 6c6f  l.l.i.n.glsvCblo
-000064f0: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
-00006500: 0304 0506 0708 090a 0b16 4647 480a 5f10  ..........FGH._.
-00006510: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00006520: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00006530: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00006540: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00006550: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00006560: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
-00006570: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
-00006580: 7310 0109 ab0c 151a 1f23 282d 3237 3c41  s........#(-27<A
-00006590: d40d 0e0f 100a 120a 1457 7669 7369 626c  .........Wvisibl
-000065a0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-000065b0: 675a 6964 656e 7469 6669 6572 0911 01c7  gZidentifier....
-000065c0: 0954 6e61 6d65 d40d 0e0f 1016 1716 1908  .Tname..........
-000065d0: 1023 0858 7562 6971 7569 7479 d40d 0e0f  .#.Xubiquity....
-000065e0: 100a 1c16 1e09 10b5 085c 6461 7465 4d6f  .........\dateMo
-000065f0: 6469 6669 6564 d40d 0e0f 1016 1c16 2208  dified........".
-00006600: 085b 6461 7465 4372 6561 7465 64d4 0d0e  .[dateCreated...
-00006610: 0f10 0a25 1627 0910 6108 5473 697a 65d4  ...%.'..a.Tsize.
-00006620: 0d0e 0f10 0a2a 0a2c 0910 7309 546b 696e  .....*.,..s.Tkin
-00006630: 64d4 0d0e 0f10 162f 0a31 0810 6409 556c  d....../.1..d.Ul
-00006640: 6162 656c d40d 0e0f 1016 340a 3608 104b  abel......4.6..K
-00006650: 0957 7665 7273 696f 6ed4 0d0e 0f10 1639  .Wversion......9
-00006660: 0a3b 0811 012c 0958 636f 6d6d 656e 7473  .;...,.Xcomments
-00006670: d40d 0e0f 1016 3e16 4008 10c8 085e 6461  ......>.@....^da
-00006680: 7465 4c61 7374 4f70 656e 6564 d40d 0e0f  teLastOpened....
-00006690: 1016 1c16 4408 0859 6461 7465 4164 6465  ....D..YdateAdde
-000066a0: 6408 2340 2800 0000 0000 0054 6e61 6d65  d.#@(......Tname
-000066b0: 2340 3000 0000 0000 0009 0008 0019 002e  #@0.............
-000066c0: 0040 0048 005c 0065 0070 0079 008c 008e  .@.H.\.e.p.y....
-000066d0: 008f 009b 00a4 00ac 00b2 00bc 00c7 00c8  ................
-000066e0: 00cb 00cc 00d1 00da 00db 00dd 00de 00e7  ................
-000066f0: 00f0 00f1 00f3 00f4 0101 010a 010b 010c  ................
-00006700: 0118 0121 0122 0124 0125 012a 0133 0134  ...!.".$.%.*.3.4
-00006710: 0136 0137 013c 0145 0146 0148 0149 014f  .6.7.<.E.F.H.I.O
-00006720: 0158 0159 015b 015c 0164 016d 016e 0171  .X.Y.[.\.d.m.n.q
-00006730: 0172 017b 0184 0185 0187 0188 0197 01a0  .r.{............
-00006740: 01a1 01a2 01ac 01ad 01b6 01bb 01c4 0000  ................
-00006750: 0000 0000 0201 0000 0000 0000 004a 0000  .............J..
-00006760: 0000 0000 0000 0000 0000 0000 01c5 0000  ................
-00006770: 0009 006c 0061 0062 0065 006c 006c 0069  ...l.a.b.e.l.l.i
-00006780: 006e 0067 6c73 7670 626c 6f62 0000 025e  .n.glsvpblob...^
-00006790: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-000067a0: 0809 0a0b 1d45 4647 0a5f 1012 7669 6577  .....EFG._..view
-000067b0: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-000067c0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-000067d0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000067e0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-000067f0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00006800: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
-00006810: 656c 6174 6976 6544 6174 6573 1001 09d9  elativeDates....
-00006820: 0c0d 0e0f 1011 1213 1415 1e23 272b 3035  ...........#'+05
-00006830: 3a3f 5863 6f6d 6d65 6e74 735e 6461 7465  :?Xcomments^date
-00006840: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
-00006850: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
-00006860: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
-00006870: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
-00006880: d416 1718 191a 1b0a 1d55 696e 6465 7855  .........UindexU
-00006890: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-000068a0: 7669 7369 626c 6510 0711 012c 0908 d416  visible....,....
-000068b0: 1718 191f 201d 1d10 0810 c808 08d4 1617  .... ...........
-000068c0: 1819 0924 1d0a 10b5 0809 d416 1718 1928  ...$...........(
-000068d0: 241d 1d10 0208 08d4 1617 1819 2c2d 1d0a  $...........,-..
-000068e0: 1003 1061 0809 d416 1718 1931 320a 1d10  ...a.......12...
-000068f0: 0510 6409 08d4 1617 1819 3637 0a0a 1004  ..d.......67....
-00006900: 1073 0909 d416 1718 193b 3c0a 1d10 0610  .s.......;<.....
-00006910: 4b09 08d4 1617 1819 4041 0a0a 1000 1101  K.......@A......
-00006920: c709 0908 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00006930: 6d65 2340 3000 0000 0000 0009 0008 0019  me#@0...........
-00006940: 002e 0040 0048 005c 0065 0070 0079 008c  ...@.H.\.e.p.y..
-00006950: 008e 008f 00a2 00ab 00ba 00c7 00d3 00d8  ................
-00006960: 00de 00e3 00eb 00f0 00f9 00ff 0105 010f  ................
-00006970: 0117 0119 011c 011d 011e 0127 0129 012b  ...........'.).+
-00006980: 012c 012d 0136 0138 0139 013a 0143 0145  .,.-.6.8.9.:.C.E
-00006990: 0146 0147 0150 0152 0154 0155 0156 015f  .F.G.P.R.T.U.V._
-000069a0: 0161 0163 0164 0165 016e 0170 0172 0173  .a.c.d.e.n.p.r.s
-000069b0: 0174 017d 017f 0181 0182 0183 018c 018e  .t.}............
-000069c0: 0191 0192 0193 0194 019d 01a2 01ab 0000  ................
-000069d0: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-000069e0: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-000069f0: 0009 006c 0061 0062 0065 006c 006c 0069  ...l.a.b.e.l.l.i
-00006a00: 006e 0067 6d6f 4444 626c 6f62 0000 0008  .n.gmoDDblob....
-00006a10: 9c3c 7c32 d208 c541 0000 0009 006c 0061  .<|2...A.....l.a
-00006a20: 0062 0065 006c 006c 0069 006e 0067 6d6f  .b.e.l.l.i.n.gmo
-00006a30: 6444 626c 6f62 0000 0008 c446 b51b 4305  dDblob.....F..C.
-00006a40: c541 0000 0009 006c 0061 0062 0065 006c  .A.....l.a.b.e.l
-00006a50: 006c 0069 006e 0067 7068 3153 636f 6d70  .l.i.n.gph1Scomp
-00006a60: 0000 0000 0002 a000 0000 0009 006c 0061  .............l.a
-00006a70: 0062 0065 006c 006c 0069 006e 0067 7653  .b.e.l.l.i.n.gvS
-00006a80: 726e 6c6f 6e67 0000 0001 0000 0006 006d  rnlong.........m
-00006a90: 0069 0078 0069 006e 0073 6277 7370 626c  .i.x.i.n.sbwspbl
-00006aa0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
-00006ab0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00006ac0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00006ad0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00006ae0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00006af0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00006b00: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00006b10: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00006b20: 0809 0809 5f10 187b 7b31 3332 2c20 3335  ...._..{{132, 35
-00006b30: 7d2c 207b 3131 3939 2c20 3736 397d 7d09  }, {1199, 769}}.
-00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00006b60: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
-00006b80: 6731 5363 6f6d 7000 0000 0000 0f9a 2d00  g1Scomp.......-.
-00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
-00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
-00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
-00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
-00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00006c00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00006c10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
-00006c20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
-00006c30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
-00006c40: 282d 3237 3c41 d40d 0e0f 1011 120a 0a5a  (-27<A.........Z
-00006c50: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
-00006c60: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00006c70: 6c65 546e 616d 6511 01c7 0909 d410 0e0f  leTname.........
-00006c80: 0d16 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
-00006c90: 7479 d40d 0e0f 101b 1c16 0a5c 6461 7465  ty.........\date
-00006ca0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-00006cb0: 1020 1c16 165b 6461 7465 4372 6561 7465  . ...[dateCreate
-00006cc0: 6408 08d4 0d0e 0f10 2425 160a 5473 697a  d.......$%..Tsiz
-00006cd0: 6510 6108 09d4 0d0e 0f10 292a 0a0a 546b  e.a.......)*..Tk
-00006ce0: 696e 6410 7309 09d4 0d0e 0f10 2e2f 0a16  ind.s......../..
-00006cf0: 556c 6162 656c 1064 0908 d40d 0e0f 1033  Ulabel.d.......3
-00006d00: 340a 1657 7665 7273 696f 6e10 4b09 08d4  4..Wversion.K...
-00006d10: 0d0e 0f10 3839 0a16 5863 6f6d 6d65 6e74  ....89..Xcomment
-00006d20: 7311 012c 0908 d40d 0e0f 103d 3e16 165e  s..,.......=>..^
-00006d30: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-00006d40: 0808 d410 0e0f 0d16 1c16 4408 0859 6461  ..........D..Yda
-00006d50: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-00006d60: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
-00006d70: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
-00006d80: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
-00006d90: 009b 00a4 00af 00b5 00bf 00c7 00cc 00cf  ................
-00006da0: 00d0 00d1 00da 00db 00dd 00de 00e7 00f0  ................
-00006db0: 00fd 00ff 0100 0101 010a 0116 0117 0118  ................
-00006dc0: 0121 0126 0128 0129 012a 0133 0138 013a  .!.&.(.).*.3.8.:
-00006dd0: 013b 013c 0145 014b 014d 014e 014f 0158  .;.<.E.K.M.N.O.X
-00006de0: 0160 0162 0163 0164 016d 0176 0179 017a  .`.b.c.d.m.v.y.z
-00006df0: 017b 0184 0193 0195 0196 0197 01a0 01a1  .{..............
-00006e00: 01a2 01ac 01ad 01b6 01c3 01cc 0000 0000  ................
-00006e10: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
-00006e20: 0000 0000 0000 0000 0000 01cd 4601 4801  ............F.H.
+00006460: 095f 1018 7b7b 3333 352c 2031 3938 7d2c  ._..{{335, 198},
+00006470: 207b 3932 372c 2035 3638 7d7d 0908 1725   {927, 568}}...%
+00006480: 313d 4960 6d79 7a7b 7c7d 7e99 0000 0000  1=I`myz{|}~.....
+00006490: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+000064a0: 0000 0000 0000 0000 0000 009a 0000 0009  ................
+000064b0: 006c 0061 0062 0065 006c 006c 0069 006e  .l.a.b.e.l.l.i.n
+000064c0: 0067 6c67 3153 636f 6d70 0000 0000 0002  .glg1Scomp......
+000064d0: 416b 0000 0009 006c 0061 0062 0065 006c  Ak.....l.a.b.e.l
+000064e0: 006c 0069 006e 0067 6c73 7643 626c 6f62  .l.i.n.glsvCblob
+000064f0: 0000 0279 6270 6c69 7374 3030 d801 0203  ...ybplist00....
+00006500: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
+00006510: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00006520: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00006530: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00006540: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00006550: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+00006560: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
+00006570: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00006580: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
+00006590: 0d0e 0f10 0a12 0a14 5776 6973 6962 6c65  ........Wvisible
+000065a0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+000065b0: 5a69 6465 6e74 6966 6965 7209 1101 c709  Zidentifier.....
+000065c0: 546e 616d 65d4 0d0e 0f10 1617 1619 0810  Tname...........
+000065d0: 2308 5875 6269 7175 6974 79d4 0d0e 0f10  #.Xubiquity.....
+000065e0: 0a1c 161e 0910 b508 5c64 6174 654d 6f64  ........\dateMod
+000065f0: 6966 6965 64d4 0d0e 0f10 161c 1622 0808  ified........"..
+00006600: 5b64 6174 6543 7265 6174 6564 d40d 0e0f  [dateCreated....
+00006610: 100a 2516 2709 1061 0854 7369 7a65 d40d  ..%.'..a.Tsize..
+00006620: 0e0f 100a 2a0a 2c09 1073 0954 6b69 6e64  ....*.,..s.Tkind
+00006630: d40d 0e0f 1016 2f0a 3108 1064 0955 6c61  ....../.1..d.Ula
+00006640: 6265 6cd4 0d0e 0f10 1634 0a36 0810 4b09  bel......4.6..K.
+00006650: 5776 6572 7369 6f6e d40d 0e0f 1016 390a  Wversion......9.
+00006660: 3b08 1101 2c09 5863 6f6d 6d65 6e74 73d4  ;...,.Xcomments.
+00006670: 0d0e 0f10 163e 1640 0810 c808 5e64 6174  .....>.@....^dat
+00006680: 654c 6173 744f 7065 6e65 64d4 0d0e 0f10  eLastOpened.....
+00006690: 161c 1644 0808 5964 6174 6541 6464 6564  ...D..YdateAdded
+000066a0: 0823 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
+000066b0: 4030 0000 0000 0000 0900 0800 1900 2e00  @0..............
+000066c0: 4000 4800 5c00 6500 7000 7900 8c00 8e00  @.H.\.e.p.y.....
+000066d0: 8f00 9b00 a400 ac00 b200 bc00 c700 c800  ................
+000066e0: cb00 cc00 d100 da00 db00 dd00 de00 e700  ................
+000066f0: f000 f100 f300 f401 0101 0a01 0b01 0c01  ................
+00006700: 1801 2101 2201 2401 2501 2a01 3301 3401  ..!.".$.%.*.3.4.
+00006710: 3601 3701 3c01 4501 4601 4801 4901 4f01  6.7.<.E.F.H.I.O.
+00006720: 5801 5901 5b01 5c01 6401 6d01 6e01 7101  X.Y.[.\.d.m.n.q.
+00006730: 7201 7b01 8401 8501 8701 8801 9701 a001  r.{.............
+00006740: a101 a201 ac01 ad01 b601 bb01 c400 0000  ................
+00006750: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
+00006760: 0000 0000 0000 0000 0000 0001 c500 0000  ................
+00006770: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
+00006780: 6e00 676c 7376 7062 6c6f 6200 0002 5e62  n.glsvpblob...^b
+00006790: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
+000067a0: 090a 0b1d 4546 470a 5f10 1276 6965 774f  ....EFG._..viewO
+000067b0: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+000067c0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+000067d0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+000067e0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+000067f0: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e58  SizeZsortColumnX
+00006800: 6963 6f6e 5369 7a65 5f10 1075 7365 5265  iconSize_..useRe
+00006810: 6c61 7469 7665 4461 7465 7310 0109 d90c  lativeDates.....
+00006820: 0d0e 0f10 1112 1314 151e 2327 2b30 353a  ..........#'+05:
+00006830: 3f58 636f 6d6d 656e 7473 5e64 6174 654c  ?Xcomments^dateL
+00006840: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
+00006850: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
+00006860: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
+00006870: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
+00006880: 1617 1819 1a1b 0a1d 5569 6e64 6578 5577  ........UindexUw
+00006890: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+000068a0: 6973 6962 6c65 1007 1101 2c09 08d4 1617  isible....,.....
+000068b0: 1819 1f20 1d1d 1008 10c8 0808 d416 1718  ... ............
+000068c0: 1909 241d 0a10 b508 09d4 1617 1819 2824  ..$...........($
+000068d0: 1d1d 1002 0808 d416 1718 192c 2d1d 0a10  ...........,-...
+000068e0: 0310 6108 09d4 1617 1819 3132 0a1d 1005  ..a.......12....
+000068f0: 1064 0908 d416 1718 1936 370a 0a10 0410  .d.......67.....
+00006900: 7309 09d4 1617 1819 3b3c 0a1d 1006 104b  s.......;<.....K
+00006910: 0908 d416 1718 1940 410a 0a10 0011 01c7  .......@A.......
+00006920: 0909 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
+00006930: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
+00006940: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
+00006950: 8e00 8f00 a200 ab00 ba00 c700 d300 d800  ................
+00006960: de00 e300 eb00 f000 f900 ff01 0501 0f01  ................
+00006970: 1701 1901 1c01 1d01 1e01 2701 2901 2b01  ..........'.).+.
+00006980: 2c01 2d01 3601 3801 3901 3a01 4301 4501  ,.-.6.8.9.:.C.E.
+00006990: 4601 4701 5001 5201 5401 5501 5601 5f01  F.G.P.R.T.U.V._.
+000069a0: 6101 6301 6401 6501 6e01 7001 7201 7301  a.c.d.e.n.p.r.s.
+000069b0: 7401 7d01 7f01 8101 8201 8301 8c01 8e01  t.}.............
+000069c0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
+000069d0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+000069e0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+000069f0: 0900 6c00 6100 6200 6500 6c00 6c00 6900  ..l.a.b.e.l.l.i.
+00006a00: 6e00 676d 6f44 4462 6c6f 6200 0000 0855  n.gmoDDblob....U
+00006a10: a5c5 4cc9 0bc5 4100 0000 0900 6c00 6100  ..L...A.....l.a.
+00006a20: 6200 6500 6c00 6c00 6900 6e00 676d 6f64  b.e.l.l.i.n.gmod
+00006a30: 4462 6c6f 6200 0000 0855 a5c5 4cc9 0bc5  Dblob....U..L...
+00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
+00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
+00006a60: 0000 0000 02a0 0000 0000 0900 6c00 6100  ............l.a.
+00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
+00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
+00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
+00006aa0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
+00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
+00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
+00006ae0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+00006af0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+00006b00: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
+00006b20: 0908 095f 1018 7b7b 3333 352c 2031 3938  ..._..{{335, 198
+00006b30: 7d2c 207b 3932 372c 2035 3638 7d7d 0908  }, {927, 568}}..
+00006b40: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
+00006b50: 0000 0000 0101 0000 0000 0000 000f 0000  ................
+00006b60: 0000 0000 0000 0000 0000 0000 009a 0000  ................
+00006b70: 0006 006d 0069 0078 0069 006e 0073 6c67  ...m.i.x.i.n.slg
+00006b80: 3153 636f 6d70 0000 0000 0010 6f38 0000  1Scomp......o8..
+00006b90: 0006 006d 0069 0078 0069 006e 0073 6c73  ...m.i.x.i.n.sls
+00006ba0: 7643 626c 6f62 0000 0281 6270 6c69 7374  vCblob....bplist
+00006bb0: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
+00006bc0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
+00006bd0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
+00006be0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00006bf0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00006c00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
+00006c10: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
+00006c20: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
+00006c30: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
+00006c40: 2d32 373c 41d4 0d0e 0f10 1112 0a0a 5a69  -27<A.........Zi
+00006c50: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
+00006c60: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+00006c70: 6554 6e61 6d65 1101 c709 09d4 100e 0f0d  eTname..........
+00006c80: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
+00006c90: 79d4 0d0e 0f10 1b1c 160a 5c64 6174 654d  y.........\dateM
+00006ca0: 6f64 6966 6965 6410 b508 09d4 0d0e 0f10  odified.........
+00006cb0: 201c 1616 5b64 6174 6543 7265 6174 6564   ...[dateCreated
+00006cc0: 0808 d40d 0e0f 1024 2516 0a54 7369 7a65  .......$%..Tsize
+00006cd0: 1061 0809 d40d 0e0f 1029 2a0a 0a54 6b69  .a.......)*..Tki
+00006ce0: 6e64 1073 0909 d40d 0e0f 102e 2f0a 1655  nd.s......../..U
+00006cf0: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3334  label.d.......34
+00006d00: 0a16 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
+00006d10: 0e0f 1038 390a 1658 636f 6d6d 656e 7473  ...89..Xcomments
+00006d20: 1101 2c09 08d4 0d0e 0f10 3d3e 1616 5e64  ..,.......=>..^d
+00006d30: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
+00006d40: 08d4 100e 0f0d 161c 1644 0808 5964 6174  .........D..Ydat
+00006d50: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00006d60: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
+00006d70: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
+00006d80: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
+00006d90: 9b00 a400 af00 b500 bf00 c700 cc00 cf00  ................
+00006da0: d000 d100 da00 db00 dd00 de00 e700 f000  ................
+00006db0: fd00 ff01 0001 0101 0a01 1601 1701 1801  ................
+00006dc0: 2101 2601 2801 2901 2a01 3301 3801 3a01  !.&.(.).*.3.8.:.
+00006dd0: 3b01 3c01 4501 4b01 4d01 4e01 4f01 5801  ;.<.E.K.M.N.O.X.
+00006de0: 6001 6201 6301 6401 6d01 7601 7901 7a01  `.b.c.d.m.v.y.z.
+00006df0: 7b01 8401 9301 9501 9601 9701 a001 a101  {...............
+00006e00: a201 ac01 ad01 b601 c301 cc00 0000 0000  ................
+00006e10: 0002 0100 0000 0000 0000 4a00 0000 0000  ..........J.....
+00006e20: 0000 0000 0000 0000 0001 cd01 4601 4801  ............F.H.
 00006e30: 4901 4f01 5801 5901 5b01 5c01 6401 6d01  I.O.X.Y.[.\.d.m.
 00006e40: 6e01 7101 7201 7b01 8401 8501 8701 8801  n.q.r.{.........
 00006e50: 9701 a001 a101 a201 ac01 ad01 b601 bb01  ................
 00006e60: c400 0000 0000 0002 0100 0000 0000 0000  ................
 00006e70: 4a00 0000 0000 0000 0000 0000 0000 0001  J...............
 00006e80: c500 0000 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,262 +1788,262 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 b5bc c412 5e0b c541  blob........^..A
+00007020: 626c 6f62 0000 0008 30ce 1923 0f0c c541  blob....0..#...A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 e997 ad04  modDblob........
-00007050: 050a c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 30ce 1923  modDblob....0..#
+00007050: 0f0c c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0010 f000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0011 e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
-000070a0: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
+000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000070f0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00007100: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00007120: 6261 7208 0809 0809 5f10 197b 7b32 3332  bar....._..{{232
-00007130: 2c20 3139 317d 2c20 7b31 3330 322c 2037  , 191}, {1302, 7
-00007140: 3134 7d7d 0908 1725 313d 4960 6d79 7a7b  14}}...%1=I`myz{
-00007150: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
-00007160: 0000 000f 0000 0000 0000 0000 0000 0000  ................
-00007170: 0000 009b 0000 0005 006d 006f 0064 0065  .........m.o.d.e
-00007180: 006c 6c67 3153 636f 6d70 0000 0000 0001  .llg1Scomp......
-00007190: 7e99 0000 0005 006d 006f 0064 0065 006c  ~......m.o.d.e.l
-000071a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
-000071b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-000071c0: 1846 470a 4958 6963 6f6e 5369 7a65 5f10  .FG.IXiconSize_.
-000071d0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-000071e0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-000071f0: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00007200: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00007210: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00007220: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00007230: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00007240: 0009 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
-00007250: 0e0f 1011 0a13 0a5a 6964 656e 7469 6669  .......Zidentifi
-00007260: 6572 5961 7363 656e 6469 6e67 5577 6964  erYascendingUwid
-00007270: 7468 5776 6973 6962 6c65 546e 616d 6509  thWvisibleTname.
-00007280: 1101 c709 d40d 0f0e 1016 1718 1858 7562  .............Xub
-00007290: 6971 7569 7479 1023 0808 d40d 0e0f 101b  iquity.#........
-000072a0: 181d 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
-000072b0: 0810 b509 d40d 0e0f 1020 181d 185b 6461  ......... ...[da
-000072c0: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
-000072d0: 2418 260a 5473 697a 6508 1061 09d4 0d0e  $.&.Tsize..a....
-000072e0: 0f10 290a 2b0a 546b 696e 6409 1073 09d4  ..).+.Tkind..s..
-000072f0: 0d0e 0f10 2e0a 3018 556c 6162 656c 0910  ......0.Ulabel..
-00007300: 6408 d40d 0e0f 1033 0a35 1857 7665 7273  d......3.5.Wvers
-00007310: 696f 6e09 104b 08d4 0d0e 0f10 380a 3a18  ion..K......8.:.
-00007320: 5863 6f6d 6d65 6e74 7309 1101 2c08 d40d  Xcomments...,...
-00007330: 0e0f 103d 183f 185e 6461 7465 4c61 7374  ...=.?.^dateLast
-00007340: 4f70 656e 6564 0810 c808 d40d 0f0e 1042  Opened.........B
-00007350: 1d18 1859 6461 7465 4164 6465 6408 0808  ...YdateAdded...
-00007360: 2340 2800 0000 0000 0054 6e61 6d65 0910  #@(......Tname..
-00007370: 0100 0800 1900 2200 3400 3c00 5000 5900  ......".4.<.P.Y.
-00007380: 6400 7700 8c00 9500 9600 a200 ab00 b600  d.w.............
-00007390: c000 c600 ce00 d300 d400 d700 d800 e100  ................
-000073a0: ea00 ec00 ed00 ee00 f701 0401 0501 0701  ................
-000073b0: 0801 1101 1d01 1e01 1f01 2801 2d01 2e01  ..........(.-...
-000073c0: 3001 3101 3a01 3f01 4001 4201 4301 4c01  0.1.:.?.@.B.C.L.
-000073d0: 5201 5301 5501 5601 5f01 6701 6801 6a01  R.S.U.V._.g.h.j.
-000073e0: 6b01 7401 7d01 7e01 8101 8201 8b01 9a01  k.t.}.~.........
-000073f0: 9b01 9d01 9e01 a701 b101 b201 b301 b401  ................
-00007400: bd01 c201 c300 0000 0000 0002 0100 0000  ................
-00007410: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-00007420: 0000 0001 c500 0000 0500 6d00 6f00 6400  ..........m.o.d.
-00007430: 6500 6c6c 7376 7062 6c6f 6200 0002 5e62  e.llsvpblob...^b
-00007440: 706c 6973 7430 30d8 0102 0304 0506 0708  plist00.........
-00007450: 090a 0b1a 4647 0a27 5869 636f 6e53 697a  ....FG.'XiconSiz
-00007460: 655f 100f 7368 6f77 4963 6f6e 5072 6576  e_..showIconPrev
-00007470: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00007480: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00007490: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-000074a0: 756d 6e5f 1010 7573 6552 656c 6174 6976  umn_..useRelativ
-000074b0: 6544 6174 6573 5f10 1276 6965 774f 7074  eDates_..viewOpt
-000074c0: 696f 6e73 5665 7273 696f 6e23 4030 0000  ionsVersion#@0..
-000074d0: 0000 0000 09d9 0c0d 0e0f 1011 1213 1415  ................
-000074e0: 1e23 282c 3136 3b40 5863 6f6d 6d65 6e74  .#(,16;@Xcomment
-000074f0: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-00007500: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-00007510: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00007520: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00007530: 6e54 6e61 6d65 d416 1718 191a 0a1c 1d57  nTname.........W
-00007540: 7669 7369 626c 6559 6173 6365 6e64 696e  visibleYascendin
-00007550: 6755 7769 6474 6855 696e 6465 7808 0911  gUwidthUindex...
-00007560: 012c 1007 d416 1718 191a 1a21 2208 0810  .,.........!"...
-00007570: c810 08d4 1617 1819 0a1a 2627 0908 10b5  ..........&'....
-00007580: 1001 d416 1718 191a 1a26 2b08 0810 02d4  .........&+.....
-00007590: 1617 1819 0a1a 2f30 0908 1061 1003 d416  ....../0...a....
-000075a0: 1718 191a 0a34 3508 0910 6410 05d4 1617  .....45...d.....
-000075b0: 1819 0a0a 393a 0909 1073 1004 d416 1718  ....9:...s......
-000075c0: 191a 0a3e 3f08 0910 4b10 06d4 1617 1819  ...>?...K.......
-000075d0: 0a0a 4344 0909 1101 c710 0008 2340 2800  ..CD........#@(.
-000075e0: 0000 0000 0054 6e61 6d65 0900 0800 1900  .....Tname......
-000075f0: 2200 3400 3c00 5000 5900 6400 7700 8c00  ".4.<.P.Y.d.w...
-00007600: 9500 9600 a900 b200 c100 ce00 da00 df00  ................
-00007610: e500 ea00 f200 f701 0001 0801 1201 1801  ................
-00007620: 1e01 1f01 2001 2301 2501 2e01 2f01 3001  .... .#.%.../.0.
-00007630: 3201 3401 3d01 3e01 3f01 4101 4301 4c01  2.4.=.>.?.A.C.L.
-00007640: 4d01 4e01 5001 5901 5a01 5b01 5d01 5f01  M.N.P.Y.Z.[.]._.
-00007650: 6801 6901 6a01 6c01 6e01 7701 7801 7901  h.i.j.l.n.w.x.y.
-00007660: 7b01 7d01 8601 8701 8801 8a01 8c01 9501  {.}.............
-00007670: 9601 9701 9a01 9c01 9d01 a601 ab00 0000  ................
-00007680: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
-00007690: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
-000076a0: 0500 6d00 6f00 6400 6500 6c6d 6f44 4462  ..m.o.d.e.lmoDDb
-000076b0: 6c6f 6200 0000 087f 06db 23b9 0ac5 4100  lob.......#...A.
-000076c0: 0000 0500 6d00 6f00 6400 6500 6c6d 6f64  ....m.o.d.e.lmod
-000076d0: 4462 6c6f 6200 0000 08dc c0ca 73c2 04c5  Dblob.......s...
-000076e0: 4100 0000 0500 6d00 6f00 6400 6500 6c70  A.....m.o.d.e.lp
-000076f0: 6831 5363 6f6d 7000 0000 0000 01c0 0000  h1Scomp.........
-00007700: 0000 0500 6d00 6f00 6400 6500 6c76 5372  ....m.o.d.e.lvSr
-00007710: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
-00007720: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
-00007730: 6f00 6f00 6c00 7362 7773 7062 6c6f 6200  o.o.l.sbwspblob.
-00007740: 0000 ca62 706c 6973 7430 30d7 0102 0304  ...bplist00.....
-00007750: 0506 0708 080a 080a 0d0a 5d53 686f 7753  ..........]ShowS
-00007760: 7461 7475 7342 6172 5b53 686f 7750 6174  tatusBar[ShowPat
-00007770: 6862 6172 5b53 686f 7754 6f6f 6c62 6172  hbar[ShowToolbar
-00007780: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
-00007790: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
-000077a0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
-000077b0: 5b53 686f 7753 6964 6562 6172 0808 0908  [ShowSidebar....
-000077c0: 095f 1019 7b7b 3233 322c 2031 3931 7d2c  ._..{{232, 191},
-000077d0: 207b 3133 3032 2c20 3731 347d 7d09 0817   {1302, 714}}...
-000077e0: 2531 3d49 606d 797a 7b7c 7d7e 9a00 0000  %1=I`myz{|}~....
-000077f0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-00007800: 0000 0000 0000 0000 0000 0000 9b00 0000  ................
-00007810: 0d00 6f00 7500 7400 6c00 6900 6500 7200  ..o.u.t.l.i.e.r.
-00007820: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00007830: 6f6d 7000 0000 0000 015f 9300 0000 0d00  omp......_......
-00007840: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
-00007850: 7400 6f00 6f00 6c00 736c 7376 4362 6c6f  t.o.o.l.slsvCblo
-00007860: 6200 0002 b062 706c 6973 7430 30da 0102  b....bplist00...
-00007870: 0304 0506 0708 090a 0b0c 0d18 4849 484a  ............HIHJ
-00007880: 0c4c 5f10 1276 6965 774f 7074 696f 6e73  .L_..viewOptions
-00007890: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-000078a0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-000078b0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-000078c0: 5369 7a65 735f 100f 7363 726f 6c6c 506f  Sizes_..scrollPo
-000078d0: 7369 7469 6f6e 5958 7465 7874 5369 7a65  sitionYXtextSize
-000078e0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000078f0: 6e58 5a73 6f72 7443 6f6c 756d 6e5f 1010  nXZsortColumn_..
-00007900: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00007910: 5869 636f 6e53 697a 6510 0109 ab0e 171c  XiconSize.......
-00007920: 2125 2a2f 3439 3e43 d40f 1011 1213 140c  !%*/49>C........
-00007930: 0c5a 6964 656e 7469 6669 6572 5577 6964  .ZidentifierUwid
-00007940: 7468 5961 7363 656e 6469 6e67 5776 6973  thYascendingWvis
-00007950: 6962 6c65 546e 616d 6511 01c7 0909 d412  ibleTname.......
-00007960: 1011 0f18 1918 1b08 1023 0858 7562 6971  .........#.Xubiq
-00007970: 7569 7479 d412 1011 0f0c 1e18 2009 10b5  uity........ ...
-00007980: 085c 6461 7465 4d6f 6469 6669 6564 d412  .\dateModified..
-00007990: 1011 0f18 1e18 2408 085b 6461 7465 4372  ......$..[dateCr
-000079a0: 6561 7465 64d4 1210 110f 0c27 1829 0910  eated......'.)..
-000079b0: 6108 5473 697a 65d4 1210 110f 0c2c 0c2e  a.Tsize......,..
-000079c0: 0910 7309 546b 696e 64d4 1210 110f 1831  ..s.Tkind......1
-000079d0: 0c33 0810 6409 556c 6162 656c d412 1011  .3..d.Ulabel....
-000079e0: 0f18 360c 3808 104b 0957 7665 7273 696f  ..6.8..K.Wversio
-000079f0: 6ed4 1210 110f 183b 0c3d 0811 012c 0958  n......;.=...,.X
-00007a00: 636f 6d6d 656e 7473 d412 1011 0f18 4018  comments......@.
-00007a10: 4208 10c8 085e 6461 7465 4c61 7374 4f70  B....^dateLastOp
-00007a20: 656e 6564 d412 1011 0f18 1e18 4608 0859  ened........F..Y
-00007a30: 6461 7465 4164 6465 6408 2300 0000 0000  dateAdded.#.....
-00007a40: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00007a50: 6509 2340 3000 0000 0000 0000 0800 1d00  e.#@0...........
-00007a60: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
-00007a70: ab00 b400 b600 b700 c300 cc00 d700 dd00  ................
-00007a80: e700 ef00 f400 f700 f800 f901 0201 0301  ................
-00007a90: 0501 0601 0f01 1801 1901 1b01 1c01 2901  ..............).
-00007aa0: 3201 3301 3401 4001 4901 4a01 4c01 4d01  2.3.4.@.I.J.L.M.
-00007ab0: 5201 5b01 5c01 5e01 5f01 6401 6d01 6e01  R.[.\.^._.d.m.n.
-00007ac0: 7001 7101 7701 8001 8101 8301 8401 8c01  p.q.w...........
-00007ad0: 9501 9601 9901 9a01 a301 ac01 ad01 af01  ................
-00007ae0: b001 bf01 c801 c901 ca01 d401 d501 de01  ................
-00007af0: e701 ec01 ed00 0000 0000 0002 0100 0000  ................
-00007b00: 0000 0000 4d00 0000 0000 0000 0000 0000  ....M...........
-00007b10: 0000 0001 f600 0000 0d00 6f00 7500 7400  ..........o.u.t.
-00007b20: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
-00007b30: 6c00 736c 7376 7062 6c6f 6200 0002 9562  l.slsvpblob....b
-00007b40: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
-00007b50: 090a 0b0c 0d1f 4748 4749 0c4b 5f10 1276  ......GHGI.K_..v
-00007b60: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00007b70: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-00007b80: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00007b90: 6c63 756c 6174 6541 6c6c 5369 7a65 735f  lculateAllSizes_
-00007ba0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-00007bb0: 5958 7465 7874 5369 7a65 5f10 0f73 6372  YXtextSize_..scr
-00007bc0: 6f6c 6c50 6f73 6974 696f 6e58 5a73 6f72  ollPositionXZsor
-00007bd0: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-00007be0: 6174 6976 6544 6174 6573 5869 636f 6e53  ativeDatesXiconS
-00007bf0: 697a 6510 0109 d90e 0f10 1112 1314 1516  ize.............
-00007c00: 1720 2529 2d32 373c 4158 636f 6d6d 656e  . %)-27<AXcommen
-00007c10: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-00007c20: 645c 6461 7465 4d6f 6469 6669 6564 5b64  d\dateModified[d
-00007c30: 6174 6543 7265 6174 6564 5473 697a 6555  ateCreatedTsizeU
-00007c40: 6c61 6265 6c54 6b69 6e64 5776 6572 7369  labelTkindWversi
-00007c50: 6f6e 546e 616d 65d4 1819 1a1b 1c1d 0c1f  onTname.........
-00007c60: 5569 6e64 6578 5577 6964 7468 5961 7363  UindexUwidthYasc
-00007c70: 656e 6469 6e67 5776 6973 6962 6c65 1007  endingWvisible..
-00007c80: 1101 2c09 08d4 1819 1a1b 2122 1f1f 1008  ..,.......!"....
-00007c90: 10c8 0808 d418 191a 1b0b 261f 0c10 b508  ..........&.....
-00007ca0: 09d4 1819 1a1b 2a26 1f1f 1002 0808 d418  ......*&........
-00007cb0: 191a 1b2e 2f1f 0c10 0310 6108 09d4 1819  ..../.....a.....
-00007cc0: 1a1b 3334 0c1f 1005 1064 0908 d418 191a  ..34.....d......
-00007cd0: 1b38 390c 0c10 0410 7309 09d4 1819 1a1b  .89.....s.......
-00007ce0: 3d3e 0c1f 1006 104b 0908 d41b 191a 180c  =>.....K........
-00007cf0: 430c 4509 1101 c709 1000 0823 0000 0000  C.E........#....
-00007d00: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00007d10: 6d65 0923 4030 0000 0000 0000 0008 001d  me.#@0..........
-00007d20: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00007d30: 00ab 00b4 00b6 00b7 00ca 00d3 00e2 00ef  ................
-00007d40: 00fb 0100 0106 010b 0113 0118 0121 0127  .............!.'
-00007d50: 012d 0137 013f 0141 0144 0145 0146 014f  .-.7.?.A.D.E.F.O
-00007d60: 0151 0153 0154 0155 015e 0160 0161 0162  .Q.S.T.U.^.`.a.b
-00007d70: 016b 016d 016e 016f 0178 017a 017c 017d  .k.m.n.o.x.z.|.}
-00007d80: 017e 0187 0189 018b 018c 018d 0196 0198  .~..............
-00007d90: 019a 019b 019c 01a5 01a7 01a9 01aa 01ab  ................
-00007da0: 01b4 01b5 01b8 01b9 01bb 01bc 01c5 01ce  ................
-00007db0: 01d3 01d4 0000 0000 0000 0201 0000 0000  ................
-00007dc0: 0000 004c 0000 0000 0000 0000 0000 0000  ...L............
-00007dd0: 0000 01dd 0000 000d 006f 0075 0074 006c  .........o.u.t.l
-00007de0: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
-00007df0: 0073 6d6f 4444 626c 6f62 0000 0008 56b2  .smoDDblob....V.
-00007e00: f350 8b0a c541 0000 000d 006f 0075 0074  .P...A.....o.u.t
-00007e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00007e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
-00007e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
-00007e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
-00007e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-00007e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
-00007e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00007e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
-00007e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00007ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
-00007eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00007ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00007ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00007ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00007ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00007f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00007f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00007f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-00007f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
-00007f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
-00007f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-00007f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00007f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
-00007f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00007f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
+00007120: 6261 7208 0809 0809 5f10 187b 7b33 3335  bar....._..{{335
+00007130: 2c20 3139 387d 2c20 7b39 3237 2c20 3536  , 198}, {927, 56
+00007140: 387d 7d09 0817 2531 3d49 606d 797a 7b7c  8}}...%1=I`myz{|
+00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
+00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
+00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 017c  llg1Scomp......|
+00007190: 0100 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
+000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
+000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
+000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+00007210: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00007220: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+00007230: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+00007240: 09ab 0c15 1a1f 2328 2d32 373c 41d4 0d0e  ......#(-27<A...
+00007250: 0f10 110a 130a 5a69 6465 6e74 6966 6965  ......Zidentifie
+00007260: 7259 6173 6365 6e64 696e 6755 7769 6474  rYascendingUwidt
+00007270: 6857 7669 7369 626c 6554 6e61 6d65 0911  hWvisibleTname..
+00007280: 01c7 09d4 0d0f 0e10 1617 1818 5875 6269  ............Xubi
+00007290: 7175 6974 7910 2308 08d4 0d0e 0f10 1b18  quity.#.........
+000072a0: 1d0a 5c64 6174 654d 6f64 6966 6965 6408  ..\dateModified.
+000072b0: 10b5 09d4 0d0e 0f10 2018 1d18 5b64 6174  ........ ...[dat
+000072c0: 6543 7265 6174 6564 0808 d40d 0e0f 1024  eCreated.......$
+000072d0: 1826 0a54 7369 7a65 0810 6109 d40d 0e0f  .&.Tsize..a.....
+000072e0: 1029 0a2b 0a54 6b69 6e64 0910 7309 d40d  .).+.Tkind..s...
+000072f0: 0e0f 102e 0a30 1855 6c61 6265 6c09 1064  .....0.Ulabel..d
+00007300: 08d4 0d0e 0f10 330a 3518 5776 6572 7369  ......3.5.Wversi
+00007310: 6f6e 0910 4b08 d40d 0e0f 1038 0a3a 1858  on..K......8.:.X
+00007320: 636f 6d6d 656e 7473 0911 012c 08d4 0d0e  comments...,....
+00007330: 0f10 3d18 3f18 5e64 6174 654c 6173 744f  ..=.?.^dateLastO
+00007340: 7065 6e65 6408 10c8 08d4 0d0f 0e10 421d  pened.........B.
+00007350: 1818 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
+00007360: 4028 0000 0000 0000 546e 616d 6509 1001  @(......Tname...
+00007370: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
+00007380: 0077 008c 0095 0096 00a2 00ab 00b6 00c0  .w..............
+00007390: 00c6 00ce 00d3 00d4 00d7 00d8 00e1 00ea  ................
+000073a0: 00ec 00ed 00ee 00f7 0104 0105 0107 0108  ................
+000073b0: 0111 011d 011e 011f 0128 012d 012e 0130  .........(.-...0
+000073c0: 0131 013a 013f 0140 0142 0143 014c 0152  .1.:.?.@.B.C.L.R
+000073d0: 0153 0155 0156 015f 0167 0168 016a 016b  .S.U.V._.g.h.j.k
+000073e0: 0174 017d 017e 0181 0182 018b 019a 019b  .t.}.~..........
+000073f0: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
+00007400: 01c2 01c3 0000 0000 0000 0201 0000 0000  ................
+00007410: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+00007420: 0000 01c5 0000 0005 006d 006f 0064 0065  .........m.o.d.e
+00007430: 006c 6c73 7670 626c 6f62 0000 025e 6270  .llsvpblob...^bp
+00007440: 6c69 7374 3030 d801 0203 0405 0607 0809  list00..........
+00007450: 0a0b 1a46 470a 2758 6963 6f6e 5369 7a65  ...FG.'XiconSize
+00007460: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00007470: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00007480: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00007490: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+000074a0: 6d6e 5f10 1075 7365 5265 6c61 7469 7665  mn_..useRelative
+000074b0: 4461 7465 735f 1012 7669 6577 4f70 7469  Dates_..viewOpti
+000074c0: 6f6e 7356 6572 7369 6f6e 2340 3000 0000  onsVersion#@0...
+000074d0: 0000 0009 d90c 0d0e 0f10 1112 1314 151e  ................
+000074e0: 2328 2c31 363b 4058 636f 6d6d 656e 7473  #(,16;@Xcomments
+000074f0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00007500: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00007510: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00007520: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00007530: 546e 616d 65d4 1617 1819 1a0a 1c1d 5776  Tname.........Wv
+00007540: 6973 6962 6c65 5961 7363 656e 6469 6e67  isibleYascending
+00007550: 5577 6964 7468 5569 6e64 6578 0809 1101  UwidthUindex....
+00007560: 2c10 07d4 1617 1819 1a1a 2122 0808 10c8  ,.........!"....
+00007570: 1008 d416 1718 190a 1a26 2709 0810 b510  .........&'.....
+00007580: 01d4 1617 1819 1a1a 262b 0808 1002 d416  ........&+......
+00007590: 1718 190a 1a2f 3009 0810 6110 03d4 1617  ...../0...a.....
+000075a0: 1819 1a0a 3435 0809 1064 1005 d416 1718  ....45...d......
+000075b0: 190a 0a39 3a09 0910 7310 04d4 1617 1819  ...9:...s.......
+000075c0: 1a0a 3e3f 0809 104b 1006 d416 1718 190a  ..>?...K........
+000075d0: 0a43 4409 0911 01c7 1000 0823 4028 0000  .CD........#@(..
+000075e0: 0000 0000 546e 616d 6509 0008 0019 0022  ....Tname......"
+000075f0: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
+00007600: 0096 00a9 00b2 00c1 00ce 00da 00df 00e5  ................
+00007610: 00ea 00f2 00f7 0100 0108 0112 0118 011e  ................
+00007620: 011f 0120 0123 0125 012e 012f 0130 0132  ... .#.%.../.0.2
+00007630: 0134 013d 013e 013f 0141 0143 014c 014d  .4.=.>.?.A.C.L.M
+00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
+00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
+00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
+00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
+00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
+00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
+000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
+000076b0: 6f62 0000 0008 7e87 fcf0 c80b c541 0000  ob....~......A..
+000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
+000076d0: 626c 6f62 0000 0008 7e87 fcf0 c80b c541  blob....~......A
+000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
+000076f0: 3153 636f 6d70 0000 0000 0001 c000 0000  1Scomp..........
+00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
+00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
+00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
+00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
+00007740: 00c9 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
+00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
+00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
+00007770: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
+00007780: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00007790: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+000077a0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+000077b0: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
+000077c0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
+000077d0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
+000077e0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
+000077f0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
+00007800: 0000 0000 0000 0000 0000 9a00 0000 0d00  ................
+00007810: 6f00 7500 7400 6c00 6900 6500 7200 5f00  o.u.t.l.i.e.r._.
+00007820: 7400 6f00 6f00 6c00 736c 6731 5363 6f6d  t.o.o.l.slg1Scom
+00007830: 7000 0000 0000 0159 9a00 0000 0d00 6f00  p......Y......o.
+00007840: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
+00007850: 6f00 6f00 6c00 736c 7376 4362 6c6f 6200  o.o.l.slsvCblob.
+00007860: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
+00007870: 0506 0708 090a 0b0c 0d18 4849 484a 0c4c  ..........HIHJ.L
+00007880: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00007890: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+000078a0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+000078b0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+000078c0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
+000078d0: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
+000078e0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
+000078f0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00007900: 6552 656c 6174 6976 6544 6174 6573 5869  eRelativeDatesXi
+00007910: 636f 6e53 697a 6510 0109 ab0e 171c 2125  conSize.......!%
+00007920: 2a2f 3439 3e43 d40f 1011 1213 140c 0c5a  */49>C.........Z
+00007930: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+00007940: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00007950: 6c65 546e 616d 6511 01c7 0909 d412 1011  leTname.........
+00007960: 0f18 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
+00007970: 7479 d412 1011 0f0c 1e18 2009 10b5 085c  ty........ ....\
+00007980: 6461 7465 4d6f 6469 6669 6564 d412 1011  dateModified....
+00007990: 0f18 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
+000079a0: 7465 64d4 1210 110f 0c27 1829 0910 6108  ted......'.)..a.
+000079b0: 5473 697a 65d4 1210 110f 0c2c 0c2e 0910  Tsize......,....
+000079c0: 7309 546b 696e 64d4 1210 110f 1831 0c33  s.Tkind......1.3
+000079d0: 0810 6409 556c 6162 656c d412 1011 0f18  ..d.Ulabel......
+000079e0: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
+000079f0: 1210 110f 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
+00007a00: 6d6d 656e 7473 d412 1011 0f18 4018 4208  mments......@.B.
+00007a10: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+00007a20: 6564 d412 1011 0f18 1e18 4608 0859 6461  ed........F..Yda
+00007a30: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
+00007a40: 0023 4028 0000 0000 0000 546e 616d 6509  .#@(......Tname.
+00007a50: 2340 3000 0000 0000 0000 0800 1d00 3200  #@0...........2.
+00007a60: 4400 4c00 6000 7200 7b00 8d00 9800 ab00  D.L.`.r.{.......
+00007a70: b400 b600 b700 c300 cc00 d700 dd00 e700  ................
+00007a80: ef00 f400 f700 f800 f901 0201 0301 0501  ................
+00007a90: 0601 0f01 1801 1901 1b01 1c01 2901 3201  ............).2.
+00007aa0: 3301 3401 4001 4901 4a01 4c01 4d01 5201  3.4.@.I.J.L.M.R.
+00007ab0: 5b01 5c01 5e01 5f01 6401 6d01 6e01 7001  [.\.^._.d.m.n.p.
+00007ac0: 7101 7701 8001 8101 8301 8401 8c01 9501  q.w.............
+00007ad0: 9601 9901 9a01 a301 ac01 ad01 af01 b001  ................
+00007ae0: bf01 c801 c901 ca01 d401 d501 de01 e701  ................
+00007af0: ec01 ed00 0000 0000 0002 0100 0000 0000  ................
+00007b00: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
+00007b10: 0001 f600 0000 0d00 6f00 7500 7400 6c00  ........o.u.t.l.
+00007b20: 6900 6500 7200 5f00 7400 6f00 6f00 6c00  i.e.r._.t.o.o.l.
+00007b30: 736c 7376 7062 6c6f 6200 0002 9562 706c  slsvpblob....bpl
+00007b40: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
+00007b50: 0b0c 0d1f 4748 4749 0c4b 5f10 1276 6965  ....GHGI.K_..vie
+00007b60: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+00007b70: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+00007b80: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+00007b90: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
+00007ba0: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
+00007bb0: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
+00007bc0: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
+00007bd0: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00007be0: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
+00007bf0: 6510 0109 d90e 0f10 1112 1314 1516 1720  e.............. 
+00007c00: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
+00007c10: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00007c20: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00007c30: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00007c40: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00007c50: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5569  Tname.........Ui
+00007c60: 6e64 6578 5577 6964 7468 5961 7363 656e  ndexUwidthYascen
+00007c70: 6469 6e67 5776 6973 6962 6c65 1007 1101  dingWvisible....
+00007c80: 2c09 08d4 1819 1a1b 2122 1f1f 1008 10c8  ,.......!"......
+00007c90: 0808 d418 191a 1b0b 261f 0c10 b508 09d4  ........&.......
+00007ca0: 1819 1a1b 2a26 1f1f 1002 0808 d418 191a  ....*&..........
+00007cb0: 1b2e 2f1f 0c10 0310 6108 09d4 1819 1a1b  ../.....a.......
+00007cc0: 3334 0c1f 1005 1064 0908 d418 191a 1b38  34.....d.......8
+00007cd0: 390c 0c10 0410 7309 09d4 1819 1a1b 3d3e  9.....s.......=>
+00007ce0: 0c1f 1006 104b 0908 d41b 191a 180c 430c  .....K........C.
+00007cf0: 4509 1101 c709 1000 0823 0000 0000 0000  E........#......
+00007d00: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00007d10: 0923 4030 0000 0000 0000 0008 001d 0032  .#@0...........2
+00007d20: 0044 004c 0060 0072 007b 008d 0098 00ab  .D.L.`.r.{......
+00007d30: 00b4 00b6 00b7 00ca 00d3 00e2 00ef 00fb  ................
+00007d40: 0100 0106 010b 0113 0118 0121 0127 012d  ...........!.'.-
+00007d50: 0137 013f 0141 0144 0145 0146 014f 0151  .7.?.A.D.E.F.O.Q
+00007d60: 0153 0154 0155 015e 0160 0161 0162 016b  .S.T.U.^.`.a.b.k
+00007d70: 016d 016e 016f 0178 017a 017c 017d 017e  .m.n.o.x.z.|.}.~
+00007d80: 0187 0189 018b 018c 018d 0196 0198 019a  ................
+00007d90: 019b 019c 01a5 01a7 01a9 01aa 01ab 01b4  ................
+00007da0: 01b5 01b8 01b9 01bb 01bc 01c5 01ce 01d3  ................
+00007db0: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
+00007dc0: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
+00007dd0: 01dd 0000 000d 006f 0075 0074 006c 0069  .......o.u.t.l.i
+00007de0: 0065 0072 005f 0074 006f 006f 006c 0073  .e.r._.t.o.o.l.s
+00007df0: 6d6f 4444 626c 6f62 0000 0008 e309 3e65  moDDblob......>e
+00007e00: fc0b c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
+00007e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00007e20: 0073 6d6f 6444 626c 6f62 0000 0008 e309  .smodDblob......
+00007e30: 3e65 fc0b c541 0000 000d 006f 0075 0074  >e...A.....o.u.t
+00007e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00007e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
+00007e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00007e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00007e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
+00007e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
+00007ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
+00007eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00007ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00007ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00007ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00007ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00007f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00007f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00007f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00007f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+00007f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
+00007f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+00007f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00007f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
+00007f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00007f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,18 +2088,18 @@
 00008270: 7901 7b01 7d01 7e01 7f01 8801 8a01 8c01  y.{.}.~.........
 00008280: 8d01 8e01 9701 9901 9b01 9c01 9d01 a601  ................
 00008290: a801 aa01 ab01 ac01 b501 b701 ba01 bb01  ................
 000082a0: bc01 bd01 c601 cf01 dc00 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 086f d1b6 5abb 0ac5  Dblob....o..Z...
+000082e0: 4462 6c6f 6200 0000 08d6 95ef 57e4 0bc5  Dblob.......W...
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 086f d1b6 5abb 0ac5 4100 0000 0800 7000  .o..Z...A.....p.
+00008310: 08d6 95ef 57e4 0bc5 4100 0000 0800 7000  ....W...A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
 00008330: 5363 6f6d 7000 0000 0000 0fb0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
@@ -2264,42 +2264,42 @@
 00008d70: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00008d80: 0000 0000 0000 0000 0000 009a 0000 000e  ................
 00008d90: 0070 006f 0073 0065 005f 0069 006d 0070  .p.o.s.e._.i.m.p
 00008da0: 006f 0072 0074 0065 0072 0073 6473 636c  .o.r.t.e.r.sdscl
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
-00008de0: 0000 03f6 c772 005f 0074 006f 006f 006c  .....r._.t.o.o.l
-00008df0: 0073 6d6f 4444 626c 6f62 0000 0008 56b2  .smoDDblob....V.
-00008e00: f350 8b0a c541 0000 000d 006f 0075 0074  .P...A.....o.u.t
-00008e10: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00008e20: 006c 0073 6d6f 6444 626c 6f62 0000 0008  .l.smodDblob....
-00008e30: 0bdb a04e 0b04 c541 0000 000d 006f 0075  ...N...A.....o.u
-00008e40: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
-00008e50: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
-00008e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
-00008e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00008e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
-00008e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00008ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
-00008eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00008ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00008ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00008ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00008ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00008f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00008f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00008f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-00008f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
-00008f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
-00008f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-00008f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00008f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
-00008f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00008f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
+00008de0: 0000 03f6 c75f 0074 006f 006f 006c 0073  ....._.t.o.o.l.s
+00008df0: 6d6f 4444 626c 6f62 0000 0008 e309 3e65  moDDblob......>e
+00008e00: fc0b c541 0000 000d 006f 0075 0074 006c  ...A.....o.u.t.l
+00008e10: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00008e20: 0073 6d6f 6444 626c 6f62 0000 0008 e309  .smodDblob......
+00008e30: 3e65 fc0b c541 0000 000d 006f 0075 0074  >e...A.....o.u.t
+00008e40: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
+00008e50: 006c 0073 7068 3153 636f 6d70 0000 0000  .l.sph1Scomp....
+00008e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00008e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00008e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
+00008e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
+00008ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
+00008eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00008ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00008ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00008ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00008ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00008f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00008f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00008f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00008f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+00008f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
+00008f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+00008f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00008f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
+00008f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00008f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2527,35 +2527,35 @@
 00009de0: 0101 010a 010b 010c 0118 0121 0122 0124  ...........!.".$
 00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
 00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
 00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
 00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-00009e50: 0000 0000 01c5 7068 3153 636f 6d70 0000  ......ph1Scomp..
-00009e60: 0000 0002 5000 0000 000d 006f 0075 0074  ....P......o.u.t
-00009e70: 006c 0069 0065 0072 005f 0074 006f 006f  .l.i.e.r._.t.o.o
-00009e80: 006c 0073 7653 726e 6c6f 6e67 0000 0001  .l.svSrnlong....
-00009e90: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00009ea0: 006e 0067 6277 7370 626c 6f62 0000 00ca  .n.gbwspblob....
-00009eb0: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00009ec0: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00009ed0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00009ee0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00009ef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00009f00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00009f10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00009f20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-00009f30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
-00009f40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
-00009f50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-00009f60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-00009f70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
-00009f80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-00009f90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
+00009e50: 0000 0000 01c5 3153 636f 6d70 0000 0000  ......1Scomp....
+00009e60: 0002 5000 0000 000d 006f 0075 0074 006c  ..P......o.u.t.l
+00009e70: 0069 0065 0072 005f 0074 006f 006f 006c  .i.e.r._.t.o.o.l
+00009e80: 0073 7653 726e 6c6f 6e67 0000 0001 0000  .svSrnlong......
+00009e90: 0008 0070 006c 006f 0074 0074 0069 006e  ...p.l.o.t.t.i.n
+00009ea0: 0067 6277 7370 626c 6f62 0000 00c9 6270  .gbwspblob....bp
+00009eb0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00009ec0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00009ed0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00009ee0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00009ef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00009f00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00009f10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00009f20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00009f30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+00009f40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
+00009f50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+00009f60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00009f70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
+00009f80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+00009f90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
@@ -2792,26 +2792,26 @@
 0000ae70: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
 0000ae80: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
 0000ae90: 0000 0001 ac00 0000 0200 7500 696d 6f44  ..........u.imoD
 0000aea0: 4462 6c6f 6200 0000 086c 6d0e 79f5 09c5  Dblob....lm.y...
 0000aeb0: 4100 0000 0200 7500 696d 6f64 4462 6c6f  A.....u.imodDblo
 0000aec0: 6200 0000 0862 2d63 9153 09c5 4100 0000  b....b-c.S..A...
 0000aed0: 0200 7500 6970 6831 5363 6f6d 7000 0000  ..u.iph1Scomp...
-0000aee0: 0000 0c50 0077 546f 6f6c 6261 725b 5368  ...P.wToolbar[Sh
-0000aef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-0000af00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-0000af10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-0000af20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-0000af30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
-0000af40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
-0000af50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-0000af60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-0000af70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
-0000af80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000af90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
+0000aee0: 0000 0c50 006f 6f6c 6261 725b 5368 6f77  ...P.oolbar[Show
+0000aef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+0000af00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+0000af10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+0000af20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+0000af30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+0000af40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
+0000af50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+0000af60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+0000af70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
+0000af80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+0000af90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2919,16 +2919,16 @@
 0000b660: 01aa 01b3 0000 0000 0000 0201 0000 0000  ................
 0000b670: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
 0000b680: 0000 01b4 0000 000c 0075 006e 0073 0075  .........u.n.s.u
 0000b690: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
 0000b6a0: 6d6f 4444 626c 6f62 0000 0008 04d0 54a0  moDDblob......T.
 0000b6b0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
 0000b6c0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-0000b6d0: 6d6f 6444 626c 6f62 0000 0008 6269 0543  modDblob....bi.C
-0000b6e0: 3a05 c541 0000 000c 0075 006e 0073 0075  :..A.....u.n.s.u
+0000b6d0: 6d6f 6444 626c 6f62 0000 0008 04d0 54a0  modDblob......T.
+0000b6e0: 920a c541 0000 000c 0075 006e 0073 0075  ...A.....u.n.s.u
 0000b6f0: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
 0000b700: 7068 3153 636f 6d70 0000 0000 0009 b000  ph1Scomp........
 0000b710: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
 0000b720: 0072 0076 0069 0073 0065 0064 7653 726e  .r.v.i.s.e.dvSrn
 0000b730: 6c6f 6e67 0000 0001 0000 0005 0075 0074  long.........u.t
 0000b740: 0069 006c 0073 6277 7370 626c 6f62 0000  .i.l.sbwspblob..
 0000b750: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
@@ -3048,26 +3048,26 @@
 0000be70: 9d01 a201 ab00 0000 0000 0002 0100 0000  ................
 0000be80: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
 0000be90: 0000 0001 ac00 0000 0200 7500 696d 6f44  ..........u.imoD
 0000bea0: 4462 6c6f 6200 0000 086c 6d0e 79f5 09c5  Dblob....lm.y...
 0000beb0: 4100 0000 0200 7500 696d 6f64 4462 6c6f  A.....u.imodDblo
 0000bec0: 6200 0000 0862 2d63 9153 09c5 4100 0000  b....b-c.S..A...
 0000bed0: 0200 7500 6970 6831 5363 6f6d 7000 0000  ..u.iph1Scomp...
-0000bee0: 0000 0c50 0077 546f 6f6c 6261 725b 5368  ...P.wToolbar[Sh
-0000bef0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-0000bf00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-0000bf10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-0000bf20: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-0000bf30: 197b 7b33 3539 2c20 2d36 327d 2c20 7b31  .{{359, -62}, {1
-0000bf40: 3139 392c 2037 3639 7d7d 0908 1725 313d  199, 769}}...%1=
-0000bf50: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-0000bf60: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-0000bf70: 0000 0000 0000 0000 009b 0000 0008 0070  ...............p
-0000bf80: 006c 006f 0074 0074 0069 006e 0067 6c67  .l.o.t.t.i.n.glg
-0000bf90: 3153 636f 6d70 0000 0000 000c 87b8 0000  1Scomp..........
+0000bee0: 0000 0c50 006f 6f6c 6261 725b 5368 6f77  ...P.oolbar[Show
+0000bef0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+0000bf00: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+0000bf10: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+0000bf20: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+0000bf30: 7b33 3335 2c20 3139 387d 2c20 7b39 3237  {335, 198}, {927
+0000bf40: 2c20 3536 387d 7d09 0817 2531 3d49 606d  , 568}}...%1=I`m
+0000bf50: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+0000bf60: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+0000bf70: 0000 0000 0000 9a00 0000 0800 7000 6c00  ............p.l.
+0000bf80: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
+0000bf90: 6f6d 7000 0000 0000 0c87 9100 0000 0000  omp.............
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.60.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-190.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-183.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-182.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-329.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-181.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py37m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi` & `Simba-UW-tf-dev-1.60.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-233.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.60.2/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.60.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.60.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         'project_folder/frames/path_plots' directory of the SimBA project.
         """
 
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer(start=True)
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, _, self.fps = self.read_video_info(video_name=self.video_name)
-            self.__get_styles()
             self.data_df = read_df(file_path, self.file_type)
+            self.__get_styles()
             self.temp_folder = os.path.join(self.path_plot_dir, self.video_name, 'temp')
             self.save_frame_folder_dir = os.path.join(self.path_plot_dir, self.video_name)
             if self.frame_setting:
                 if os.path.exists(self.save_frame_folder_dir): remove_a_folder(self.save_frame_folder_dir)
                 if not os.path.exists(self.save_frame_folder_dir): os.makedirs(self.save_frame_folder_dir)
             if self.video_setting:
                 self.video_folder = os.path.join(self.path_plot_dir, self.video_name)
@@ -190,15 +190,18 @@
             results[frm_idx] = np.hstack((group_col, data[frm_idx]))
         return results
 
     def __get_styles(self):
         self.style_attr = {}
         if self.input_style_attr is not None:
             self.style_attr['bg color'] = self.color_dict[self.input_style_attr['bg color']]
-            self.style_attr['max lines'] = int(self.input_style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
+            if self.input_style_attr['max lines'] == 'entire video':
+                self.style_attr['max lines'] = len(self.data_df)
+            else:
+                self.style_attr['max lines'] = int(int(self.input_style_attr['max lines']) * (int(self.video_info['fps'].values[0]) / 1000))
             self.style_attr['font thickness'] = self.input_style_attr['font thickness']
             self.style_attr['line width'] = self.input_style_attr['line width']
             self.style_attr['font size'] = self.input_style_attr['font size']
             self.style_attr['circle size'] = self.input_style_attr['circle size']
             if self.input_style_attr['width'] == 'As input':
                 self.style_attr['width'], self.style_attr['height'] = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             else:
@@ -207,15 +210,15 @@
             space_scaler, radius_scaler, res_scaler, font_scaler = 25, 10, 1500, 0.8
             self.style_attr['width'] = int(self.video_info['Resolution_width'].values[0])
             self.style_attr['height'] = int(self.video_info['Resolution_height'].values[0])
             max_res = max(self.style_attr['width'], self.style_attr['height'])
             self.style_attr['circle size'] = int(radius_scaler / (res_scaler / max_res))
             self.style_attr['font size'] = font_scaler / (res_scaler / max_res)
             self.style_attr['bg color'] = self.color_dict['White']
-            self.style_attr['max lines'] = int(self.video_info['fps'].values[0] * 2)
+            self.style_attr['max lines'] = len(self.data_df)
             self.style_attr['font thickness'] = 2
             self.style_attr['line width'] = 2
 
         self.style_attr['animal names'] = []
         self.style_attr['animal clrs'] = []
         for animal_cnt, animal_data in self.animal_attr.items():
             self.style_attr['animal names'].append(self.find_animal_name_from_body_part_name(bp_name=animal_data[0], bp_dict=self.animal_bp_dict))
```

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/path_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,17 @@
         """
 
         for file_cnt, file_path in enumerate(self.files_found):
             video_timer = SimbaTimer()
             video_timer.start_timer()
             _, self.video_name, _ = get_fn_ext(file_path)
             self.video_info, _, self.fps = self.read_video_info(video_name=self.video_name)
+            self.data_df = read_df(file_path, self.file_type)
             self.__get_styles()
             self.__get_deque_lookups()
-            self.data_df = read_df(file_path, self.file_type)
             if self.video_setting:
                 self.video_save_path = os.path.join(self.path_plot_dir, self.video_name + '.mp4')
                 self.fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
                 self.writer = cv2.VideoWriter(self.video_save_path, self.fourcc, self.fps, (self.style_attr['width'], self.style_attr['height']))
 
             if self.frame_setting:
                 self.save_video_folder = os.path.join(self.path_plot_dir, self.video_name)
@@ -153,15 +153,18 @@
         self.timer.stop_timer()
         stdout_success(msg=f'Path visualizations for {str(len(self.files_found))} videos saved in project_folder/frames/output/path_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __get_styles(self):
         self.style_attr = {}
         if self.input_style_attr is not None:
             self.style_attr['bg color'] = self.color_dict[self.input_style_attr['bg color']]
-            self.style_attr['max lines'] = int(self.input_style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
+            if self.input_style_attr['max lines'] == 'entire video':
+                self.style_attr['max lines'] = len(self.data_df)
+            else:
+                self.style_attr['max lines'] = int(int(self.input_style_attr['max lines']) * (int(self.video_info['fps'].values[0]) / 1000))
             self.style_attr['font thickness'] = self.input_style_attr['font thickness']
             self.style_attr['line width'] = self.input_style_attr['line width']
             self.style_attr['font size'] = self.input_style_attr['font size']
             self.style_attr['circle size'] = self.input_style_attr['circle size']
             if self.input_style_attr['width'] == 'As input':
                 self.style_attr['width'], self.style_attr['height'] = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             else:
@@ -170,15 +173,15 @@
             space_scaler, radius_scaler, res_scaler, font_scaler = 25, 10, 1500, 0.8
             self.style_attr['width'] = int(self.video_info['Resolution_width'].values[0])
             self.style_attr['height'] = int(self.video_info['Resolution_height'].values[0])
             max_res = max(self.style_attr['width'], self.style_attr['height'])
             self.style_attr['circle size'] = int(radius_scaler / (res_scaler / max_res))
             self.style_attr['font size'] = int(font_scaler / (res_scaler / max_res))
             self.style_attr['bg color'] = self.color_dict['White']
-            self.style_attr['max lines'] = int(self.video_info['fps'].values[0] * 2)
+            self.style_attr['max lines'] = len(self.data_df)
             self.style_attr['font thickness'] = 2
             self.style_attr['line width'] = 2
 
     def __get_deque_lookups(self):
         self.deque_dict = {}
         for animal_cnt, animal_data in self.animal_attr.items():
             animal_name = self.find_animal_name_from_body_part_name(bp_name=animal_data[0], bp_dict=self.animal_bp_dict)
```

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.60.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.60.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.60.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.60.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.60.2/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.60.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.60.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.60.2/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.60.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.60.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.60.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.60.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.60.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.60.2/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.60.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.60.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.60.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.60.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.60.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.60.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.60.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.60.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.60.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.60.1
+Version: 1.60.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.60.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/LICENSE.md` & `Simba-UW-tf-dev-1.60.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/README.md` & `Simba-UW-tf-dev-1.60.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.60.1/setup.py` & `Simba-UW-tf-dev-1.60.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.60.1",
+    version="1.60.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

