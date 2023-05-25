# Comparing `tmp/Simba-UW-tf-dev-1.61.2.tar.gz` & `tmp/Simba-UW-tf-dev-1.61.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.2.tar", last modified: Wed May 24 17:17:32 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.61.3.tar", last modified: Thu May 25 19:53:47 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.61.2.tar` & `Simba-UW-tf-dev-1.61.3.tar`

### file list

```diff
@@ -1,504 +1,506 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.61.2/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2544 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.2/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.2/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.2/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.2/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.2/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.2/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.2/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.2/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-23 15:41:51.000000 Simba-UW-tf-dev-1.61.2/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.2/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-24 17:11:58.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    30127 2023-05-23 12:26:01.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-18 20:03:49.000000 Simba-UW-tf-dev-1.61.2/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18214 2023-05-24 15:19:35.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.2/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    20972 2023-05-08 18:03:19.000000 Simba-UW-tf-dev-1.61.2/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.2/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.2/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8800 2023-05-16 00:24:15.000000 Simba-UW-tf-dev-1.61.2/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    42900 2023-05-24 17:01:14.000000 Simba-UW-tf-dev-1.61.2/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.2/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.61.2/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.2/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17732 2023-05-24 16:48:16.000000 Simba-UW-tf-dev-1.61.2/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.2/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.2/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     6514 2023-05-24 15:15:38.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10984 2023-05-24 16:55:20.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-19 18:26:50.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8550 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11410 2023-05-23 20:23:27.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9649 2023-05-18 13:48:41.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8129 2023-05-18 13:31:03.000000 Simba-UW-tf-dev-1.61.2/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.61.2/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.2/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.2/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.2/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.2/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.2/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6525 2023-05-19 17:31:41.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8160 2023-05-19 18:34:50.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2696 2023-05-23 12:33:12.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    64855 2023-05-21 18:08:05.000000 Simba-UW-tf-dev-1.61.2/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.2/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.2/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.2/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.2/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    18435 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-24 17:17:31.000000 Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.2/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.2/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/
--rw-r--r--   0 simon      (501) staff       (20)     1723 2023-05-23 20:16:59.000000 Simba-UW-tf-dev-1.61.2/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.2/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/two_c57/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3972 2023-05-21 18:23:01.000000 Simba-UW-tf-dev-1.61.2/tests/test_thirdparty_appenders.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.2/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.2/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-24 17:17:23.000000 Simba-UW-tf-dev-1.61.2/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-24 17:17:32.000000 Simba-UW-tf-dev-1.61.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-23 17:02:30.000000 Simba-UW-tf-dev-1.61.3/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5873 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10712 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.61.3/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.61.3/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.61.3/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    34040 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.3/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.61.3/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-05-23 15:41:51.000000 Simba-UW-tf-dev-1.61.3/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.61.3/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42902 2023-05-25 18:14:02.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1118 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37100 2023-05-19 15:31:55.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6175 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    60756 2023-05-25 14:55:02.000000 Simba-UW-tf-dev-1.61.3/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18214 2023-05-24 15:19:35.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.61.3/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20973 2023-05-25 13:55:35.000000 Simba-UW-tf-dev-1.61.3/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7365 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.61.3/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.61.3/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-05-15 14:49:42.000000 Simba-UW-tf-dev-1.61.3/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     3227 2023-05-15 15:41:04.000000 Simba-UW-tf-dev-1.61.3/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.61.3/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.61.3/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.61.3/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.61.3/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    13770 2023-05-23 16:26:11.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7915 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11491 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9113 2023-05-14 23:44:34.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9274 2023-05-23 16:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9926 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10984 2023-05-24 16:55:20.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11410 2023-05-23 20:23:27.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.61.3/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    19026 2023-05-19 11:15:45.000000 Simba-UW-tf-dev-1.61.3/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.61.3/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.3/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    18876 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.61.3/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.61.3/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.61.3/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8176 2023-05-25 14:24:49.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.61.3/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.61.3/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.61.3/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.61.3/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.61.3/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    18515 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.61.3/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.61.3/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5043 2023-05-25 14:14:27.000000 Simba-UW-tf-dev-1.61.3/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.61.3/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.61.3/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/two_c57/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3972 2023-05-21 18:23:01.000000 Simba-UW-tf-dev-1.61.3/tests/test_thirdparty_appenders.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.61.3/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.61.3/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-05-25 19:53:39.000000 Simba-UW-tf-dev-1.61.3/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-25 19:53:47.000000 Simba-UW-tf-dev-1.61.3/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.61.2/PKG-INFO` & `Simba-UW-tf-dev-1.61.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.2
+Version: 1.61.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,37 +12,51 @@
     def __init__(self,
                  config_path: str):
 
         PopUpMixin.__init__(self, title='ANALYZE CLASSIFICATIONS: DESCRIPTIVE STATISTICS')
         ConfigReader.__init__(self, config_path=config_path)
         measures_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='MEASUREMENTS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.ANALYZE_ML_RESULTS.value)
         clf_frm = LabelFrame(self.main_frm, text='CLASSIFIERS', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
+        video_meta_data_frm = LabelFrame(self.main_frm, text='METADATA', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.measurements_var_dict, self.clf_var_dict = {}, {}
         cbox_titles = Options.CLF_DESCRIPTIVES_OPTIONS.value
         for cnt, title in enumerate(cbox_titles):
             self.measurements_var_dict[title] = BooleanVar()
             cbox = Checkbutton(measures_frm, text=title, variable=self.measurements_var_dict[title])
             cbox.grid(row=cnt, sticky=NW)
         for cnt, clf_name in enumerate(self.clf_names):
             self.clf_var_dict[clf_name] = BooleanVar()
             cbox = Checkbutton(clf_frm, text=clf_name, variable=self.clf_var_dict[clf_name])
             cbox.grid(row=cnt, sticky=NW)
         run_button = Button(self.main_frm, text='Run', command=lambda: self.run_descriptive_analysis())
         measures_frm.grid(row=0, sticky=NW)
         clf_frm.grid(row=1, sticky=NW)
-        run_button.grid(row=2, sticky=NW)
+        self.metadata_frm_cnt_var, self.metadata_video_length_var = BooleanVar(), BooleanVar()
+        metadata_frm_cnt_cb = Checkbutton(video_meta_data_frm, text='Frame count', variable=self.metadata_frm_cnt_var)
+        metadata_frm_video_length_cb = Checkbutton(video_meta_data_frm, text='Video length (s)', variable=self.metadata_video_length_var)
+        video_meta_data_frm.grid(row=2, sticky=NW)
+        metadata_frm_cnt_cb.grid(row=0, column=0, sticky=NW)
+        metadata_frm_video_length_cb.grid(row=1, column=0, sticky=NW)
+        run_button.grid(row=3, sticky=NW)
 
     def run_descriptive_analysis(self):
-        measurement_lst, clf_list = [], []
+        measurement_lst, clf_list, meta_data_lst = [], [], []
         for name, val in self.measurements_var_dict.items():
             if val.get():
                 measurement_lst.append(name)
         for name, val in self.clf_var_dict.items():
             if val.get():
                 clf_list.append(name)
         if len(measurement_lst) == 0:
             raise NoChoosenMeasurementError()
         if len(clf_list) == 0:
             raise NoChoosenClassifierError()
-        data_log_analyzer = AggregateClfCalculator(config_path=self.config_path, data_measures=measurement_lst, classifiers=clf_list)
+        if self.metadata_frm_cnt_var.get():
+            meta_data_lst.append('Frame count')
+        if self.metadata_video_length_var.get():
+            meta_data_lst.append('Video length (s)')
+        data_log_analyzer = AggregateClfCalculator(config_path=self.config_path,
+                                                   data_measures=measurement_lst,
+                                                   video_meta_data=meta_data_lst,
+                                                   classifiers=clf_list)
         data_log_analyzer.run()
         data_log_analyzer.save()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.61.3/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.61.3/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.61.3/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.61.3/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.61.3/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.61.3/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.3/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/requirements.txt` & `Simba-UW-tf-dev-1.61.3/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/config_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,25 @@
                                 MissingProjectConfigEntryError,
                                 NotDirectoryError,
                                 InvalidInputError,
                                 DuplicationError,
                                 ParametersFileError)
 from simba.utils.warnings import (NoFileFoundWarning,
                                   BodypartColumnNotFoundWarning,
-                                  InvalidValueWarning)
+                                  InvalidValueWarning,
+                                  NoDataFoundWarning)
 from simba.utils.read_write import (read_project_path_and_file_type,
                                     get_fn_ext,
-                                    SimbaTimer,
                                     read_config_file,
                                     find_core_cnt,
-                                    get_all_clf_names)
-from simba.utils.checks import check_file_exist_and_readable
+                                    get_all_clf_names,
+                                    read_df,
+                                    write_df)
+from simba.utils.printing import SimbaTimer, stdout_success
+from simba.utils.checks import check_file_exist_and_readable, check_if_dir_exists, check_if_filepath_list_is_empty
 
 
 class ConfigReader(object):
     """
     Methods for reading SimBA configparser.Configparser project config and associated project data
 
     :param configparser.Configparser config_path: path to SimBA project_config.ini
@@ -536,25 +539,14 @@
             except TypeError:
                 raise ParametersFileError(msg=f'Make sure the videos that are going to be analyzed are represented with APPROPRIATE VALUES inside the project_folder/logs/video_info.csv file in your SimBA project. Could not interpret the fps, pixels per millimeter and/or fps as numerical values for video {video_name}')
 
     def check_multi_animal_status(self) -> None:
         """
         Helper to check if the project is a multi-animal SimBA project.
 
-        Parameters
-        ----------
-        config: configparser.ConfigParser
-            Parsed SimBA project_config.ini file.
-        no_animals: int
-            Number of animals in the SimBA project
-
-        Returns
-        -------
-        multi_animal_status: bool
-        multi_animal_id_lst: list
         """
         multi_animal_id_lst = []
         if not self.config.has_section('Multi animal IDs'):
             for animal in range(self.animal_cnt):
                 multi_animal_id_lst.append('Animal_' + str(animal + 1))
             multi_animal_status = False
 
@@ -568,9 +560,69 @@
                 for animal in range(self.animal_cnt):
                     multi_animal_id_lst.append('Animal_{}'.format(str(animal + 1)))
                 multi_animal_status = False
 
         self.multi_animal_status = multi_animal_status
         self.multi_animal_id_list = multi_animal_id_lst[:self.animal_cnt]
 
+    def remove_roi_features(self,
+                            data_dir: Union[str, os.PathLike]) -> None:
+        """
+        Helper to remove ROI-based features from datasets within a directory. The identified ROI-based fields are move to the
+        ``project_folder/logs/ROI_data_{datetime}`` directory.
+
+        .. note::
+           ROI-based features are identified based on the combined criteria of (i) The prefix of the field is a named ROI in
+           the ``project_folder/logs/ROI_definitions.h5`` file, and (ii) the suffix of the field is contained in the ['in zone',
+           'n zone_cumulative_time', 'in zone_cumulative_percent', 'distance', 'facing']
+
+        :param Union[str, os.PathLike] data_dir: directory with data to remove ROi features from.
+
+        :example:
+        >>> self.remove_roi_features('/project_folder/csv/features_extracted')
+
+        """
+        ROI_COL_SUFFIXES = ['in zone',
+                            'n zone_cumulative_time',
+                            'in zone_cumulative_percent',
+                            'distance',
+                            'facing']
+
+        check_if_dir_exists(in_dir=data_dir)
+        timer = SimbaTimer(start=True)
+        filepaths = glob.glob(data_dir + f'/*.{self.file_type}')
+        roi_dir = os.path.join(self.project_path, 'logs', f'ROI_data_{datetime.now().strftime("%Y%m%d%H%M%S")}')
+        check_if_filepath_list_is_empty(filepaths=filepaths, error_msg=f'No .{self.file_type} files found in {data_dir}.')
+        for file_cnt, file_path in enumerate(filepaths):
+            _, video_name, _ = get_fn_ext(filepath=file_path); roi_cols = set()
+            df = read_df(file_path=file_path, file_type=self.file_type)
+            for shape_name in self.shape_names: roi_cols.update([x for x in df.columns if shape_name in x])
+            for suffix in ROI_COL_SUFFIXES: roi_cols.update([x for x in roi_cols if x.endswith(suffix)])
+            if len(roi_cols) == 0:
+                NoDataFoundWarning(msg=f'NO ROI data found in {file_path}')
+            else:
+                roi_df = df[list(roi_cols)]; df = df.drop(list(roi_cols), axis=1)
+                roi_save_path = os.path.join(roi_dir, video_name + '.' + self.file_type)
+                if not os.path.exists(roi_dir): os.makedirs(roi_dir)
+                write_df(df=roi_df, file_type=self.file_type, save_path=roi_save_path)
+                write_df(df=df, file_type=self.file_type, save_path=file_path)
+                print(f'ROI features (N={len(roi_cols)}) removed from {video_name}...')
+        timer.stop_timer()
+        stdout_success(msg=f'ROI features removed from {len(filepaths)} files in the {data_dir} directory. The ROI features has been moved to the {roi_dir} directory', elapsed_time=timer.elapsed_time_str)
+
+
+
+            #x = [x for x in self.shape_names if any(x in y or y in x for y in df.colum)]
+
+
+
+
+# config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini', read_video_info=False)
+# config.read_roi_data()
+# config.remove_roi_features('/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/features_extracted')
+
+        # remove_roi_features(
+        #     config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini',
+        #     data_dir='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/features_extracted')
+
 #test = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.61.3/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.61.3/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.61.3/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/enums.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                               'Frame-by-frame body-parts inside ROIs (Boolean)']
     SMOOTHING_OPTIONS_W_NONE = ['None', 'Gaussian', 'Savitzky Golay']
     VIDEO_FORMAT_OPTIONS = ['mp4', 'avi']
     ALL_VIDEO_FORMAT_OPTIONS = ('.avi', '.mp4', '.mov', '.flv', '.m4v')
     WORKFLOW_FILE_TYPE_OPTIONS = ['csv','parquet']
     TRACKING_TYPE_OPTIONS = ['Classic tracking','Multi tracking', '3D tracking']
     UNSUPERVISED_FEATURE_OPTIONS = ['INCLUDE FEATURE DATA (ORIGINAL)', 'INCLUDE FEATURES (SCALED)', 'EXCLUDE FEATURE DATA']
-    TIMEBINS_MEASURMENT_OPTIONS = ['First occurance (s)', 'Event count', 'Total event duration (s)',
+    TIMEBINS_MEASURMENT_OPTIONS = ['First occurrence (s)', 'Event count', 'Total event duration (s)',
                                               'Mean event duration (s)', 'Median event duration (s)',
                                               'Mean event interval (s)', 'Median event interval (s)']
     CLF_DESCRIPTIVES_OPTIONS = ['Bout count', 'Total event duration (s)', 'Mean event bout duration (s)',
                                 'Median event bout duration (s)', 'First event occurrence (s)',
                                 'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']
     CLASSICAL_TRACKING_OPTIONS = ['1 animal; 4 body-parts', '1 animal; 7 body-parts', '1 animal; 8 body-parts', '1 animal; 9 body-parts',
                                   '2 animals; 8 body-parts', '2 animals; 14 body-parts', '2 animals; 16 body-parts', 'MARS']
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/checks.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         raise NotDirectoryError(msg=f'{in_dir} is not a valid directory')
 
 
 def check_that_column_exist(df: pd.DataFrame,
                             column_name: str,
                             file_name: str) -> None:
     """
-    Check if named field exist within a dataframe.
+    Check if single named field exist within a dataframe.
 
     :param pd.DataFrame df:
     :param str column_name: Name of putative field.
     :param str file_name: Path of ``df`` on disk.
     :raise ColumnNotFoundError: The  ``column_name`` does not exist within ``df``.
     """
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/read_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,21 +45,21 @@
             file_type: Union[str, os.PathLike],
             has_index: Optional[bool] = True,
             remove_columns: Optional[List[str]] = None,
             usecols: Optional[List[str]] = None,
             check_multiindex: bool = False) -> pd.DataFrame:
 
     """
-    Read single tabular data file.
+    Read single tabular data file or pickle
 
     .. note::
        For improved runtime, defaults to :external:py:meth:`pyarrow.csv.write_cs` if file type is ``csv``.
 
     :parameter str file_path: Path to data file
-    :parameter str file_type: Path to data file. OPTIONS: 'parquet', 'csv', 'pickle'.
+    :parameter str file_type: Type of data. OPTIONS: 'parquet', 'csv', 'pickle'.
     :parameter Optional[bool]: If the input file has an initial index column. Default: True.
     :parameter Optional[List[str]] remove_columns: If not None, then remove columns in lits.
     :parameter Optional[List[str]] usecols: If not None, then keep columns in list.
     :parameter bool check_multiindex: check file is multi-index headers. Default: False.
     :return pd.DataFrame
 
     :example:
@@ -232,22 +232,23 @@
     :return str: The set file type of the project (i.e., ``csv`` or ``parquet``).
     """
 
 
     project_path = read_config_entry(config=config,
                                      section=ConfigKey.GENERAL_SETTINGS.value,
                                      option=ConfigKey.PROJECT_PATH.value,
-                                     data_type=ConfigKey.FOLDER_PATH.value)
+                                     data_type=ConfigKey.FOLDER_PATH.value).strip()
     file_type = read_config_entry(config=config,
                                   section=ConfigKey.GENERAL_SETTINGS.value,
                                   option=ConfigKey.FILE_TYPE.value,
                                   data_type=Dtypes.STR.value,
-                                  default_value=Formats.CSV.value)
+                                  default_value=Formats.CSV.value).strip()
+    if not os.path.isdir(project_path): raise NotDirectoryError(msg=f'The project config file {config} has project path {project_path} that does not exist')
 
-    return project_path.strip(), file_type.strip()
+    return project_path, file_type
 
 
 def read_video_info_csv(file_path: Union[str, os.PathLike]) -> pd.DataFrame:
 
     """
     Read the project_folder/logs/video_info.csv of the SimBA project as a pd.DataFrame
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/errors.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/data.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 __author__ = "Simon Nilsson"
 
+import glob
 import os
 
 import pandas as pd
 from copy import deepcopy
 import configparser
 from pathlib import Path
 import ast
 from scipy.signal import savgol_filter
 from pylab import *
+from datetime import datetime
 from typing import List, Optional, Union, Dict
 try:
     from typing import Literal
 except:
     from typing_extensions import Literal
 
 from simba.utils.read_write import (get_fn_ext,
                                     read_project_path_and_file_type,
                                     find_video_of_file,
                                     read_df,
                                     write_df,
                                     read_config_file,
                                     read_config_entry,
                                     get_video_meta_data)
-from simba.utils.checks import check_file_exist_and_readable, check_int
+from simba.utils.checks import check_file_exist_and_readable, check_int, check_if_dir_exists, check_if_filepath_list_is_empty
 from simba.utils.errors import NoFilesFoundError,InvalidFileTypeError, CountError
 from simba.utils.printing import stdout_warning
 from simba.utils.enums import ConfigKey, Dtypes
 from simba.utils.lookups import get_bp_config_code_class_pairs
 
 
-
-
 def detect_bouts(data_df: pd.DataFrame,
                  target_lst: List[str],
                  fps: int) -> pd.DataFrame:
     """
     Detect behavior "bouts" (e.g., continous sequence of classified behavior-present frames) for specified classifiers.
 
     .. note::
@@ -397,8 +397,10 @@
     class_name = class_name[0]
     spec = importlib.util.spec_from_file_location(class_name, file_path)
     user_module = importlib.util.module_from_spec(spec)
     sys.modules[class_name] = user_module
     spec.loader.exec_module(user_module)
     user_class = getattr(user_module, class_name)
     print(f'Running user-defined {class_name} feature extraction file...')
-    user_class(config_path=config_path)
+    user_class(config_path=config_path)
+
+
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/utils/printing.py` & `Simba-UW-tf-dev-1.61.3/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.61.3/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.61.3/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.61.3/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.61.3/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/agg_clf_calculator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 __author__ = "Simon Nilsson"
 
 import pandas as pd
 import os
-from typing import List, Union
+from typing import List, Union, Optional
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 from simba.utils.checks import check_file_exist_and_readable, check_if_filepath_list_is_empty
 from simba.mixins.config_reader import ConfigReader
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
+from simba.utils.enums import Options
+from simba.utils.errors import InvalidInputError
 
 class AggregateClfCalculator(ConfigReader):
     """
     Compute aggregate descriptive statistics from classification data.
 
-    :parameter str config_path: path to SimBA project config file in Configparser format
-    :parameter List[str] data_measures: Aggregate statistics measures to calculate. OPTIONS: ['Bout count', 'Total event duration (s)',
+    :param str config_path: path to SimBA project config file in Configparser format
+    :param List[str] data_measures: Aggregate statistics measures to calculate. OPTIONS: ['Bout count', 'Total event duration (s)',
         'Mean event bout duration (s)', 'Median event bout duration (s)', 'First event occurrence (s)',
         'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']
-    :parameter List[str] classifiers: Classifiers to calculate aggregate statistics for. E.g.,: ['Attack', 'Sniffing']
+    :param List[str] classifiers: Classifiers to calculate aggregate statistics for. E.g.,: ['Attack', 'Sniffing']
+    :param Optional[List[str]]: Video meta data to include in the output. Options: 'Frame count', 'Video length (s)'.
 
     .. note::
        `GitHub tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
     Examples
     -----
     >>> clf_log_creator = AggregateClfCalculator(config_path="MyConfigPath", data_measures=['Bout count', 'Total event duration (s)'], classifiers=['Attack', 'Sniffing'])
     >>> clf_log_creator.run()
     >>> clf_log_creator.save()
     """
 
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  data_measures: List[Literal['Bout count', 'Total event duration (s)', 'Mean event bout duration (s)', 'Median event bout duration (s)', 'First event occurrence (s)', 'Mean event bout interval duration (s)', 'Median event bout interval duration (s)']],
+                 video_meta_data: Optional[List[Literal['Frame count', 'Video length (s)']]],
                  classifiers: List[str]):
 
         super().__init__(config_path=config_path)
-        self.chosen_measures, self.classifiers = data_measures, classifiers
-        self.file_save_name = os.path.join(self.project_path, 'logs', 'data_summary_' + str(self.datetime) + '.csv')
+        self.chosen_measures, self.classifiers, self.video_meta_data = data_measures, classifiers, video_meta_data
+        if len(list(set(self.chosen_measures).intersection(Options.CLF_DESCRIPTIVES_OPTIONS.value))) == 0:
+            raise InvalidInputError(msg=f'No valid input data measures. OPTIONS: {Options.CLF_DESCRIPTIVES_OPTIONS.value}')
+
+        self.save_path = os.path.join(self.project_path, 'logs', f'data_summary_{self.datetime}.csv')
         check_if_filepath_list_is_empty(filepaths=self.machine_results_paths,
                                         error_msg='SIMBA ERROR: No data files found in the project_folder/csv/machine_results directory. Run classifiers before analysing results.')
         print(f'Analyzing {str(len(self.machine_results_paths))} file(s) for {str(len(self.clf_names))} classifiers...')
 
     def run(self):
         self.results_df = pd.DataFrame()
         for file_cnt, file_path in enumerate(self.machine_results_paths):
@@ -60,15 +67,14 @@
             for clf in self.clf_names:
                 clf_results_dict = {}
                 clf_data = bouts_df.loc[bouts_df['Event'] == clf]
                 if len(clf_data) > 0:
                     clf_results_dict['First event occurrence (s)'] = round(clf_data['Start_time'].min(), 3)
                     clf_results_dict['Bout count'] = len(clf_data)
                     clf_results_dict['Total event duration (s)'] = round(clf_data['Bout_time'].sum(), 3)
-
                     clf_results_dict['Mean event bout duration (s)'] = round(clf_data['Bout_time'].mean(), 3)
                     clf_results_dict['Median event bout duration (s)'] = round(clf_data['Bout_time'].median(), 3)
                 else:
                     clf_results_dict['First event occurrence (s)'] = None
                     clf_results_dict['Bout count'] = None
                     clf_results_dict['Total event duration (s)'] = None
                     clf_results_dict['Mean event bout duration (s)'] = None
@@ -76,39 +82,40 @@
                 if len(clf_data) > 1:
                     interval_df = clf_data[:-1].copy()
                     clf_results_dict['Mean event bout interval duration (s)'] = round(interval_df['Interval duration'].mean(), 3)
                     clf_results_dict['Median event bout interval duration (s)'] = round(interval_df['Interval duration'].median(), 3)
                 else:
                     clf_results_dict['Mean event bout interval duration (s)'] = None
                     clf_results_dict['Median event bout interval duration (s)'] = None
+                if 'Frame count' in self.video_meta_data:
+                    clf_results_dict['Frame count'] = len(data_df)
+                if 'Video length (s)' in self.video_meta_data:
+                    clf_results_dict['Video length (s)'] = round(len(data_df) / fps, 3)
                 video_clf_pd = pd.DataFrame.from_dict(clf_results_dict, orient='index').reset_index().rename(columns={'index': 'Measure', 0: 'Value'})
                 video_clf_pd.insert(loc=0, column='Classifier', value=clf)
                 video_clf_pd.insert(loc=0, column='Video', value=file_name)
                 self.results_df = pd.concat([self.results_df, video_clf_pd], axis=0)
 
-    def save(self):
+    def save(self) -> None:
         """
         Method to save classifier aggregate statistics created in :meth:`~simba.ClfLogCreator.analyze_data` to disk.
         Results are stored in the `project_folder/logs` directory of the SimBA project
-
-        Returns
-        -------
-        None
         """
-
-        self.results_df = self.results_df[self.results_df['Measure'].isin(self.chosen_measures)].sort_values(by=['Video', 'Classifier', 'Measure']).reset_index(drop=True)
+        self.results_df = self.results_df[self.results_df['Measure'].isin(self.chosen_measures + self.video_meta_data)].sort_values(by=['Video', 'Classifier', 'Measure']).reset_index(drop=True)
         self.results_df = self.results_df[self.results_df['Classifier'].isin(self.classifiers)].set_index('Video')
-        self.results_df.to_csv(self.file_save_name)
+        self.results_df.to_csv(self.save_path)
         self.timer.stop_timer()
-        stdout_success(msg=f'Data log saved at {self.file_save_name}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'Data log saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
-# test = AggregateClfCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini",
-#                      data_measures=['Bout count',
-#                                     'Total event duration (s)'],
-#                      classifiers=['Attack', 'Sniffing'])
+# test = AggregateClfCalculator(config_path=r"/Users/simon/Desktop/envs/troubleshooting/raph/project_folder/project_config.ini",
+#                      data_measures=['Total event duration (s)'],
+#                      classifiers=['walking'])
+#
+#
+#
 # test.run()
 # test.save()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolation_smoothing.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     :parameter str input_path: path to pose-estimation data in CSV or parquet format
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter Literal str: Type of interpolation. OPTIONS: 'Animal(s): Nearest', 'Animal(s): Linear', 'Animal(s): Quadratic','Body-parts: Nearest', 'Body-parts: Linear', 'Body-parts: Quadratic']
                             See `tutorial for info/images of the different interpolation types <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
     :parameter bool initial_import_multi_index: If True, the incoming data is multi-index columns dataframes. Default: False.
 
-    .. image:: _static/img/Interpolation_comparison.png
+    .. image:: _static/img/interpolation_comparison.png
        :width: 400
        :align: center
 
     .. note::
        `Interpolation tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#to-import-multiple-dlc-csv-files>`__.
 
     Examples
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_clf_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,26 @@
     from typing_extensions import Literal
 
 from simba.utils.checks import check_int, check_if_filepath_list_is_empty
 from simba.utils.data import detect_bouts
 from simba.utils.printing import stdout_success
 from simba.utils.read_write import get_fn_ext, read_df
 from simba.mixins.config_reader import ConfigReader
-from simba.utils.errors import NoChoosenMeasurementError
+from simba.utils.errors import NoChoosenMeasurementError, InvalidInputError
+from simba.utils.enums import Options
 
 class TimeBinsClfCalculator(ConfigReader):
 
     """
     Computes aggregate classification results in user-defined time-bins. Results are stored in
     the ``project_folder/logs`` directory of the SimBA project`
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter int bin_length: Integer representing the time bin size in seconds
-    :parameter List[str] measurements: Aggregate statistic measures calculated for each time bin. OPTIONS: ['First occurance (s)', 'Event count',
+    :parameter List[str] measurements: Aggregate statistic measures calculated for each time bin. OPTIONS: ['First occurrence (s)', 'Event count',
         Total event duration (s)', 'Mean event duration (s)', 'Median event duration (s)', 'Mean event interval (s)',
         'Median event interval (s)']
     :parameter List[str] classifiers: Names of classifiers to calculate aggregate statistics in time-bins for. EXAMPLE: ['Attack', 'Sniffing']
 
     .. note::
     `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md#part-4--analyze-machine-results>`__.
 
@@ -37,20 +38,22 @@
     >>> timebin_clf_analyzer = TimeBinsClfCalculator(config_path='MyConfigPath', bin_length=15, measurements=['Event count', 'Total event duration (s)'])
     >>> timebin_clf_analyzer.run()
 
     """
     def __init__(self,
                  config_path: str,
                  bin_length: int,
-                 measurements: List[Literal['First occurance (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)', 'Median event duration (s)', 'Mean event interval (s)', 'Median event interval (s)']],
+                 measurements: List[Literal['First occurrence (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)', 'Median event duration (s)', 'Mean event interval (s)', 'Median event interval (s)']],
                  classifiers: List[str]):
 
         super().__init__(config_path=config_path)
         if len(measurements) == 0:
             raise NoChoosenMeasurementError()
+        if len(set(measurements).intersection(set(Options.TIMEBINS_MEASURMENT_OPTIONS.value))) == 0:
+            raise InvalidInputError(msg=f'No valid input data measures. OPTIONS: {Options.TIMEBINS_MEASURMENT_OPTIONS.value}')
         check_int(name='Bin length', value=bin_length, min_value=1)
         self.bin_length, self.measurements, self.classifiers = int(bin_length), measurements, classifiers
         self.files_found = glob.glob(self.machine_results_dir + '/*.' + self.file_type)
         check_if_filepath_list_is_empty(filepaths=self.files_found,
                                         error_msg=f'SIMBA ERROR: Cannot perform time-bin classification analysis, no data in {self.machine_results_dir} directory')
         print('Processing {} video(s)...'.format(str(len(self.files_found))))
         self.out_df_lst = []
@@ -79,21 +82,21 @@
                 bouts_df = detect_bouts(data_df=df, target_lst=list(self.clf_names), fps=fps)
                 bouts_df['Shifted start'] = bouts_df['Start_time'].shift(-1)
                 bouts_df['Interval duration'] = bouts_df['Shifted start'] - bouts_df['End Time']
                 for clf in self.clf_names:
                     video_dict[file_name][bin_cnt][clf] = defaultdict(list)
                     bout_df = bouts_df.loc[bouts_df['Event'] == clf]
                     if len(bouts_df) > 0:
-                        video_dict[file_name][bin_cnt][clf]['First occurance (s)'] = round(bout_df['Start_time'].min(), 3)
+                        video_dict[file_name][bin_cnt][clf]['First occurrence (s)'] = round(bout_df['Start_time'].min(), 3)
                         video_dict[file_name][bin_cnt][clf]['Event count'] = len(bout_df)
                         video_dict[file_name][bin_cnt][clf]['Total event duration (s)'] = round(bout_df['Bout_time'].sum(), 3)
                         video_dict[file_name][bin_cnt][clf]['Mean event duration (s)'] = round(bout_df["Bout_time"].mean(), 3)
                         video_dict[file_name][bin_cnt][clf]['Median event duration (s)'] = round(bout_df['Bout_time'].median(), 3)
                     else:
-                        video_dict[file_name][bin_cnt][clf]['First occurance (s)'] = None
+                        video_dict[file_name][bin_cnt][clf]['First occurrence (s)'] = None
                         video_dict[file_name][bin_cnt][clf]['Event count'] = 0
                         video_dict[file_name][bin_cnt][clf]['Total event duration (s)'] = 0
                         video_dict[file_name][bin_cnt][clf]['Mean event duration (s)'] = 0
                         video_dict[file_name][bin_cnt][clf]['Median event duration (s)'] = 0
                     if len(bouts_df) > 1:
                         video_dict[file_name][bin_cnt][clf]['Mean event interval (s)'] = round(bout_df[:-1]['Interval duration'].mean(), 3)
                         video_dict[file_name][bin_cnt][clf]['Median event interval (s)'] = round(bout_df[:-1]['Interval duration'].median(), 3)
@@ -107,23 +110,23 @@
                 data_df = pd.melt(data_df, id_vars=['Measurement']).rename(columns={'value':'Value', 'variable': 'Classifier'})
                 data_df.insert(loc=0, column='Time bin #', value=bin_number)
                 data_df.insert(loc=0, column='Video', value=video_name)
                 self.out_df_lst.append(data_df)
         out_df = pd.concat(self.out_df_lst, axis=0).sort_values(by=['Video', 'Time bin #']).set_index('Video')
         out_df = out_df[out_df['Measurement'].isin(self.measurements)]
         out_df = out_df[out_df['Classifier'].isin(self.classifiers)]
-        save_path = os.path.join(self.project_path, 'logs', 'Time_bins_ML_results_' + self.datetime + '.csv')
-        out_df.to_csv(save_path)
+        self.save_path = os.path.join(self.project_path, 'logs', f'Time_bins_ML_results_{self.datetime}.csv')
+        out_df.to_csv(self.save_path)
         self.timer.stop_timer()
         stdout_success(msg=f'Classification time-bins results saved at project_folder/logs/output/{str("Time_bins_ML_results_" + self.datetime + ".csv")}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = TimeBinsClf(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                    bin_length=2,
-#                    measurements=['First occurance (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)'],
+#                    measurements=['First occurrence (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)'],
 #                    classifiers=['Attack', 'Sniffing'])
 # test.analyze_timebins_clf()
 
 
 # test = TimeBinsClf(config_path='/Users/simon/Desktop/troubleshooting/light_analyzer/project_folder/project_config.ini',
 #                    bin_length=2,
-#                    measurements=['First occurance (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)'])
+#                    measurements=['First occurrence (s)', 'Event count', 'Total event duration (s)', 'Mean event duration (s)'])
 # test.analyze_timebins_clf()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/timebins_movement_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
         for video_name in self.results['VIDEO'].unique():
             video_df = self.results.loc[(self.results['VIDEO'] == video_name) & (self.results['MEASUREMENT'] == 'Movement (cm)')]
             for body_part in video_df['BODY-PART'].unique():
                 body_part_df = video_df[video_df['BODY-PART'] == body_part].reset_index(drop=True).sort_values(by=['Time bin #'])
                 body_part_df['Time bin #'] = body_part_df['Time bin #'].astype(str)
                 line_plot = sns.lineplot(data=body_part_df, x="Time bin #", y="VALUE")
                 plt.ylabel("Distance (cm)")
-                line_plot.figure.savefig(os.path.join(plots_dir, f'{video_name}_{body_part}.png'))
+                self.plot_save_path = os.path.join(plots_dir, f'{video_name}_{body_part}.png')
+                line_plot.figure.savefig(self.plot_save_path)
                 plt.close()
         timer.stop_timer()
         stdout_success(msg=f'Time bin movement plots saved in {plots_dir}', elapsed_time=timer.elapsed_time_str)
 
 
 
 
@@ -88,15 +89,15 @@
         of the SimBA project.
 
         Returns
         ----------
         None
         """
         video_dict, out_df_lst = {}, []
-        save_path = os.path.join(self.project_path, 'logs', 'Time_bins_movement_results_' + self.datetime + '.csv')
+        self.save_path = os.path.join(self.project_path, 'logs', 'Time_bins_movement_results_' + self.datetime + '.csv')
         for file_cnt, file_path in enumerate(self.outlier_corrected_paths):
             video_timer = SimbaTimer(start=True)
             _, video_name, _ = get_fn_ext(file_path)
             print(f'Processing time-bin movements for video {video_name} ({str(file_cnt+1)}/{str(len(self.outlier_corrected_paths))})...')
             video_dict[video_name] = {}
             video_settings, px_per_mm, fps = self.read_video_info(video_name=video_name)
             fps, self.movement_cols, self.velocity_cols = int(fps), set(), set()
@@ -127,17 +128,17 @@
                 movement_df['MEASUREMENT'] = 'Movement (cm)'
                 results = pd.concat([movement_df, velocity_df], axis=0)
                 results['VIDEO'] = video_name
                 out_df_lst.append(results)
             video_timer.stop_timer()
             print(f'Video {video_name} complete (elapsed time: {video_timer.elapsed_time_str}s)...')
         self.results = pd.concat(out_df_lst, axis=0).sort_values(by=['VIDEO', 'Time bin #', 'MEASUREMENT', 'ANIMAL'])[['VIDEO', 'Time bin #', 'ANIMAL', 'BODY-PART', 'MEASUREMENT', 'VALUE']]
-        self.results.to_csv(save_path)
+        self.results.to_csv(self.save_path)
         self.timer.stop_timer()
-        stdout_success(msg=f'Movement time-bins results saved at {save_path}', elapsed_time=self.timer.elapsed_time_str)
+        stdout_success(msg=f'Movement time-bins results saved at {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
         if self.plots:
             self.__create_plots()
 
 # test = TimeBinsMovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini',
 #                                   bin_length=60, plots=True, body_parts=['midpoint', 'mouth'])
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/kleinberg_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     :parameter str config_path: path to SimBA project config file in Configparser format
     :parameter List[str] classifier_names: Classifier names to apply Kleinberg smoothing to.
     :parameter float sigma: Burst detection sigma value. Higher sigma values and fewer, longer, behavioural bursts will be recognised. Default: 2.
     :parameter float gamma: Burst detection gamma value. Higher gamma values and fewer behavioural bursts will be recognised. Default: 0.3.
     :parameter int hierarchy: Burst detection hierarchy level. Higher hierarchy values and fewer behavioural bursts will to be recognised. Default: 1.
     :parameter bool hierarchical_search: See `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md#hierarchical-search-example>`_ Default: False.
 
-
-
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/kleinberg_filter.md>`__.
 
     Examples
     ----------
     >>> kleinberg_calculator = KleinbergCalculator(config_path='MySimBAConfigPath', classifier_names=['Attack'], sigma=2, gamma=0.3, hierarchy=2, hierarchical_search=False)
     >>> kleinberg_calculator.run()
@@ -138,18 +136,18 @@
                     hierarchy_idx = [x for xs in hierarchy_idx for x in xs]
                     hierarchy_idx = [x for x in hierarchy_idx if x in list(data_df.index)]
                     video_out_df.loc[hierarchy_idx, clf] = 1
             write_df(video_out_df, self.file_type, file_path)
 
         self.timer.stop_timer()
         if len(detailed_df_lst) > 0:
-            detailed_df = pd.concat(detailed_df_lst, axis=0)
+            self.detailed_df = pd.concat(detailed_df_lst, axis=0)
             detailed_save_path = os.path.join(self.logs_path, 'Kleinberg_detailed_log_{}.csv'.format(str(self.datetime)))
-            detailed_df.to_csv(detailed_save_path)
-            stdout_success(msg='Kleinberg analysis complete. See {detailed_save_path} for details of detected bouts of all classifiers in all hierarchies', elapsed_time=self.timer.elapsed_time_str)
+            self.detailed_df.to_csv(detailed_save_path)
+            stdout_success(msg=f'Kleinberg analysis complete. See {detailed_save_path} for details of detected bouts of all classifiers in all hierarchies', elapsed_time=self.timer.elapsed_time_str)
         else:
             KleinbergWarning(msg='All behavior bouts removed following kleinberg smoothing')
 
 # test = KleinbergCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals/project_folder/project_config.ini',
 #                            classifier_names=['Attack'],
 #                            sigma=1.1,
 #                            gamma=0.3,
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/data_processors/movement_calculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,16 @@
         stdout_success(msg= f'Movement log saved in {self.save_path}', elapsed_time=self.timer.elapsed_time_str)
 
 # test = MovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                           body_parts=['Simon CENTER OF GRAVITY'], #['Simon CENTER OF GRAVITY', 'JJ CENTER OF GRAVITY']
 #                           threshold=0.00)
 # test.run()
 
+
+
 #test.save()
 
 # test = MovementCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/locomotion/project_folder/project_config.ini',
 #                           body_parts=['Animal_1 CENTER OF GRAVITY'], #['Simon CENTER OF GRAVITY', 'JJ CENTER OF GRAVITY']
 #                           threshold=0.00)
 # test.run()
 # test.save()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.61.3/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.61.3/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.61.3/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.61.3/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.61.3/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.61.3/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.61.3/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.61.3/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
             self.__outlier_replacer()
             write_df(df=self.data_df, file_type=self.file_type, save_path=save_path)
             video_timer.stop_timer()
             print(f'Corrected movement outliers for file {self.video_name} (elapsed time: {video_timer.elapsed_time_str}s)...')
         self.__save_log_file()
 
     def __save_log_file(self):
-        log_fn = os.path.join(self.logs_path, 'Outliers_movement_{}.csv'.format(self.datetime))
-        self.log.to_csv(log_fn)
+        self.log_fn = os.path.join(self.logs_path, 'Outliers_movement_{}.csv'.format(self.datetime))
+        self.log.to_csv(self.log_fn)
         self.timer.stop_timer()
         stdout_success(msg='Log for corrected "movement outliers" saved in project_folder/logs', elapsed_time=self.timer.elapsed_time_str)
 #
 # test = OutlierCorrecterMovement(config_path='/Users/simon/Desktop/envs/troubleshooting/dorian_2/project_folder/project_config.ini')
 # test.run()
 
 # test = OutlierCorrecterMovement(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/outlier_corrector_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,16 +116,16 @@
         out_df_lst = []
         for video_name, video_data in self.above_criterion_dict_dict.items():
             for animal_name, animal_data in video_data.items():
                 for bp_name, vid_idx_lst in animal_data.items():
                     correction_ratio = round(len(vid_idx_lst) / len(self.data_df), 6)
                     out_df_lst.append(pd.DataFrame([[video_name, animal_name, bp_name, len(vid_idx_lst), correction_ratio]], columns=['Video', 'Animal', 'Body-part', 'Corrections', 'Correction ratio (%)']))
         out_df = pd.concat(out_df_lst, axis=0).reset_index(drop=True)
-        log_fn = os.path.join(self.logs_path, 'Outliers_location_{}.csv'.format(self.datetime))
-        out_df.to_csv(log_fn)
+        self.logs_path = os.path.join(self.logs_path, 'Outliers_location_{}.csv'.format(self.datetime))
+        out_df.to_csv(self.logs_path)
         self.timer.stop_timer()
         stdout_success(msg='Log for corrected "location outliers" saved in project_folder/logs', elapsed_time=self.timer.elapsed_time_str)
 
 
 # test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/naresh/project_folder/project_config.ini')
 # test.run()
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/skip_outlier_correction.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
             data_df = read_df(file_path=file_path, file_type=self.file_type, check_multiindex=True)
             if "scorer" in data_df.columns:
                 data_df = data_df.set_index("scorer")
 
             data_df = self.insert_column_headers_for_outlier_correction(
                 data_df=data_df, new_headers=self.bp_headers, filepath=file_path
             )
-            print(data_df)
             data_df.index.name = None
             save_path = os.path.join(
                 self.outlier_corrected_dir, video_name + "." + self.file_type
             )
             write_df(df=data_df, file_type=self.file_type, save_path=save_path)
             video_timer.stop_timer()
             print(
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.61.3/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/SimBA.py` & `Simba-UW-tf-dev-1.61.3/simba/SimBA.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 from simba.ui.pop_ups.data_plot_pop_up import DataPlotterPopUp
 from simba.ui.pop_ups.clf_plot_pop_up import SklearnVisualizationPopUp
 from simba.ui.pop_ups.roi_tracking_plot_pop_up import VisualizeROITrackingPopUp
 from simba.ui.pop_ups.roi_features_plot_pop_up import VisualizeROIFeaturesPopUp
 from simba.ui.pop_ups.clf_validation_plot_pop_up import ClassifierValidationPopUp
 from simba.ui.pop_ups.clf_probability_plot_pop_up import VisualizeClassificationProbabilityPopUp
 from simba.ui.pop_ups.directing_other_animals_plot_pop_up import DirectingOtherAnimalsVisualizerPopUp
+from simba.ui.pop_ups.remove_roi_features_pop_up import RemoveROIFeaturesPopUp
 from simba.ui.pop_ups.validation_plot_pop_up import ValidationVideoPopUp
 from simba.ui.pop_ups.pose_reorganizer_pop_up import PoseReorganizerPopUp
 from simba.ui.pop_ups.pup_retrieval_pop_up import PupRetrievalPopUp
 from simba.ui.pop_ups.pose_bp_drop_pop_up import DropTrackingDataPopUp
 from simba.ui.pop_ups.outlier_settings_pop_up import OutlierSettingsPopUp
 from simba.ui.pop_ups.about_simba_pop_up import AboutSimBAPopUp
 from simba.ui.pop_ups.csv_2_parquet_pop_up import Csv2ParquetPopUp, Parquet2CsvPopUp
@@ -297,14 +298,15 @@
         self.scriptfile.btnFind.configure(state='disabled')
         self.user_defined_var = BooleanVar(value=False)
         userscript = Checkbutton(labelframe_usrdef,text='Apply user-defined feature extraction script',variable=self.user_defined_var, command=lambda: activate(self.user_defined_var, self.scriptfile.btnFind))
 
         roi_feature_frm = CreateLabelFrameWithIcon(parent=tab5, header='APPEND ROI FEATURES', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.APPEND_ROI_FEATURES.value)
         append_roi_features_by_animal = Button(roi_feature_frm, text='APPEND ROI DATA TO FEATURES: BY ANIMAL (CAUTION)', fg='red',command=lambda: AppendROIFeaturesByAnimalPopUp(config_path=self.config_path))
         append_roi_features_by_body_part = Button(roi_feature_frm, text='APPEND ROI DATA TO FEATURES: BY BODY-PARTS (CAUTION)', fg='orange',command=lambda: AppendROIFeaturesByBodyPartPopUp(config_path=self.config_path))
+        remove_roi_features_from_feature_set = Button(roi_feature_frm, text='REMOVE ROI FEATURES FROM FEATURE SET', fg='darkred', command=lambda: RemoveROIFeaturesPopUp(config_path=self.config_path, dataset='features_extracted'))
 
         feature_tools_frm = LabelFrame(tab5, text='FEATURE TOOLS', pady=5, font=Formats.LABELFRAME_HEADER_FORMAT.value)
         compute_feature_subset_btn = Button(feature_tools_frm, text='CALCULATE FEATURE SUBSETS', fg='blue',command=lambda: FeatureSubsetExtractorPopUp(config_path=self.config_path))
 
         label_behavior_frm = CreateLabelFrameWithIcon(parent=tab7, header='LABEL BEHAVIOR', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.LABEL_BEHAVIOR.value)
         #label_behavior_frm = LabelFrame(tab7,text='LABEL BEHAVIOR',font=Formats.LABELFRAME_HEADER_FORMAT.value,pady=5,padx=5,fg='black')
         select_video_btn_new = Button(label_behavior_frm, text='Select video (create new video annotation)',command= lambda:select_labelling_video(config_path=self.config_path,
@@ -350,15 +352,15 @@
         label_adv_note_2.bind("<Button-1>", lambda e: self.callback('https://github.com/sgoldenlab/simba/blob/master/docs/advanced_labelling.md'))
         adv_label_btn_new = Button(label_adv_label, text='Select video (create new video annotation)',command= lambda: select_labelling_video_advanced(config_path=self.config_path, continuing=False))
         adv_label_btn_continue = Button(label_adv_label, text='Select video (continue existing video annotation)',command=lambda: select_labelling_video_advanced(config_path=self.config_path, continuing=True))
 
         lbl_tools_frm = LabelFrame(tab7, text='LABELLING TOOLS', font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         visualize_annotation_img_btn = Button(lbl_tools_frm, text='Visualize annotations', fg='blue', command=lambda: ExtractAnnotationFramesPopUp(config_path=self.config_path))
         third_party_annotations_btn = Button(lbl_tools_frm, text='Append third-party annotations', fg='purple', command=lambda: ThirdPartyAnnotatorAppenderPopUp(config_path=self.config_path))
-
+        remove_roi_features_from_annotation_set = Button(lbl_tools_frm, text='Remove ROI features from label set', fg='darkred', command=lambda: RemoveROIFeaturesPopUp(config_path=self.config_path, dataset='targets_inserted'))
 
         label_trainmachinemodel = CreateLabelFrameWithIcon(parent=tab8, header='TRAIN MACHINE MODELS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.TRAIN_ML_MODEL.value)
         button_trainmachinesettings = Button(label_trainmachinemodel,text='SETTINGS', fg='darkorange', command=self.trainmachinemodelsetting)
         button_trainmachinemodel = Button(label_trainmachinemodel,text='TRAIN SINGLE MODEL (GLOBAL ENVIRONMENT)',fg='blue',command = lambda: threading.Thread(target=self.train_single_model(config_path=self.config_path)).start())
         button_train_multimodel = Button(label_trainmachinemodel, text='TRAIN MULTIPLE MODELS (ONE FOR EACH SAVED SETTING)',fg='green',command = lambda: threading.Thread(target=self.train_multiple_models_from_meta(config_path=self.config_path)).start())
 
         label_model_validation = CreateLabelFrameWithIcon(parent=tab9, header='VALIDATE MODEL ON SINGLE VIDEO', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.OUT_OF_SAMPLE_VALIDATION.value)
@@ -462,14 +464,15 @@
         labelframe_usrdef.grid(row=1, column=0, sticky=NW, pady=5)
         userscript.grid(row=1, column=0, sticky=NW)
         self.scriptfile.grid(row=2, column=0, sticky=NW)
 
         roi_feature_frm.grid(row=1, column=0, sticky=NW)
         append_roi_features_by_animal.grid(row=0, column=0, sticky=NW)
         append_roi_features_by_body_part.grid(row=1, column=0, sticky=NW)
+        remove_roi_features_from_feature_set.grid(row=2, column=0, sticky=NW)
 
         feature_tools_frm.grid(row=2, column=0, sticky=NW)
         compute_feature_subset_btn.grid(row=0, column=0, sticky=NW)
 
 
         label_behavior_frm.grid(row=5,sticky=W)
         select_video_btn_new.grid(row=0,sticky=W)
@@ -496,14 +499,15 @@
         button_importethovision.grid(row=0, column=1, sticky=NW)
         button_importdeepethogram.grid(row=1, column=1, sticky=NW)
         import_observer_btn.grid(row=2, column=1, sticky=NW)
 
         lbl_tools_frm.grid(row=9, column=0, sticky=NW)
         visualize_annotation_img_btn.grid(row=0, column=0, sticky=NW)
         third_party_annotations_btn.grid(row=1, column=0, sticky=NW)
+        remove_roi_features_from_annotation_set.grid(row=2, column=0, sticky=NW)
 
         label_trainmachinemodel.grid(row=6,sticky=W)
         button_trainmachinesettings.grid(row=0,column=0,sticky=NW,padx=5)
         button_trainmachinemodel.grid(row=1,column=0,sticky=NW,padx=5)
         button_train_multimodel.grid(row=2,column=0,sticky=NW,padx=5)
 
         label_model_validation.grid(row=7, sticky=W, pady=5)
```

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.61.3/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.61.3/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.61.3/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.61.3/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.61.3/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.61.3/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.61.3/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.61.3/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.61.3/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.61.2
+Version: 1.61.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,15 @@
 simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
 simba/ui/pop_ups/outlier_settings_pop_up.py
 simba/ui/pop_ups/path_plot_pop_up.py
 simba/ui/pop_ups/pose_bp_drop_pop_up.py
 simba/ui/pop_ups/pose_reorganizer_pop_up.py
 simba/ui/pop_ups/pup_retrieval_pop_up.py
 simba/ui/pop_ups/quick_path_plot_pop_up.py
+simba/ui/pop_ups/remove_roi_features_pop_up.py
 simba/ui/pop_ups/roi_analysis_pop_up.py
 simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
 simba/ui/pop_ups/roi_features_plot_pop_up.py
 simba/ui/pop_ups/roi_tracking_plot_pop_up.py
 simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
 simba/ui/pop_ups/severity_analysis_pop_up.py
 simba/ui/pop_ups/smoothing_interpolation_pop_up.py
@@ -427,14 +428,15 @@
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
 tests/__init__.py
 tests/test_data_processors.py
 tests/test_featurizers.py
+tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
 tests/data/__init__.py
 tests/data/test_projects/__init__.py
 tests/data/test_projects/mouse_open_field/__init__.py
 tests/data/test_projects/two_c57/__init__.py
 tests/data/test_projects/zebrafish/__init__.py
 tests/data/test_projects/zebrafish/feature_file/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.61.2/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.61.3/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/LICENSE.md` & `Simba-UW-tf-dev-1.61.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.61.3/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.61.3/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.61.3/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/README.md` & `Simba-UW-tf-dev-1.61.3/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.61.2/setup.py` & `Simba-UW-tf-dev-1.61.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.61.2",
+    version="1.61.3",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

