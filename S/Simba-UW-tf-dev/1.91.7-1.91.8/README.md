# Comparing `tmp/Simba-UW-tf-dev-1.91.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.91.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.91.7.tar", last modified: Wed May  8 18:14:22 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.91.8.tar", last modified: Wed May  8 23:57:41 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.91.7.tar` & `Simba-UW-tf-dev-1.91.8.tar`

### file list

```diff
@@ -1,669 +1,669 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.91.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)   100939 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.91.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.91.7/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-07 12:26:33.000000 Simba-UW-tf-dev-1.91.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.91.7/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.91.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    35776 2024-04-26 13:39:55.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   181397 2024-05-04 19:12:36.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   133041 2024-05-08 18:08:27.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   166127 2024-04-30 16:15:41.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26127 2024-05-07 18:38:46.000000 Simba-UW-tf-dev-1.91.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.7/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.91.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    56046 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79418 2024-04-29 18:45:39.000000 Simba-UW-tf-dev-1.91.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.91.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.91.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/CLAHE.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/downsample_video_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/downsample_multiple_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/mahalanobis.py
--rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/superpixels.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/superimpose_frame_count.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/lbp.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/eta_squared.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fleiss_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/jaccard_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/manhattan_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/seekable.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/relative_risk.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/contrast.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/youden_j.py
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/color_filtering.py
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.91.7/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.91.7/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.91.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.91.7/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17324 2024-05-08 18:12:28.000000 Simba-UW-tf-dev-1.91.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    18552 2024-04-28 20:07:14.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   123264 2024-05-08 16:16:57.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/brightness_contrast_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.91.7/simba/video_processors/clahe_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    82357 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-06 14:15:23.000000 Simba-UW-tf-dev-1.91.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.91.7/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/brightness.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    24073 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      797 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-08 18:14:21.000000 Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.91.7/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.91.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.91.7/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.91.7/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.91.7/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.7/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.91.7/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.91.7/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.7/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-08 18:12:53.000000 Simba-UW-tf-dev-1.91.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-08 18:14:22.000000 Simba-UW-tf-dev-1.91.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.91.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8831 2024-05-02 13:40:02.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9578 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9366 2024-04-29 16:29:26.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5830 2024-04-26 18:09:47.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3352 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)   100939 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3651 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.91.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.91.8/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-05-07 12:26:33.000000 Simba-UW-tf-dev-1.91.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.91.8/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.91.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    35776 2024-04-26 13:39:55.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   181397 2024-05-04 19:12:36.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    69908 2024-05-06 18:32:12.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    62121 2024-05-02 14:32:34.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   133234 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   166127 2024-04-30 16:15:41.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18963 2024-04-26 14:35:34.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17344 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26127 2024-05-07 18:38:46.000000 Simba-UW-tf-dev-1.91.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.8/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7734 2024-05-08 13:50:22.000000 Simba-UW-tf-dev-1.91.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    56046 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79418 2024-04-29 18:45:39.000000 Simba-UW-tf-dev-1.91.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.91.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46270 2024-04-26 16:10:44.000000 Simba-UW-tf-dev-1.91.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     4080 2024-05-06 15:09:47.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/CLAHE.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2623 2024-05-03 16:20:12.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     5109 2024-05-07 19:36:44.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/downsample_video_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     5254 2024-05-07 19:55:25.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/downsample_multiple_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2278 2024-05-04 19:11:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/mahalanobis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1626 2024-05-08 16:59:35.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/superpixels.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4166 2024-05-06 21:09:36.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/superimpose_frame_count.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      493 2024-05-02 16:25:29.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/lbp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     1951 2024-05-03 14:45:28.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/eta_squared.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)      770 2024-05-02 20:50:37.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fleiss_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     1214 2024-05-03 17:07:43.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/jaccard_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)     1378 2024-05-03 20:13:55.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/manhattan_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)     2671 2024-05-08 14:43:03.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/seekable.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-05-03 15:57:50.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/relative_risk.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)     6507 2024-05-06 12:58:30.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/contrast.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1157 2024-05-02 20:32:28.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/youden_j.py
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-05-06 15:36:55.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/color_filtering.py
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.91.8/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10307 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    23490 2024-04-29 16:23:41.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19315 2024-05-08 18:11:04.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12956 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10620 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16960 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21343 2024-04-29 18:50:27.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    14847 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13512 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11565 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24207 2024-05-07 12:24:30.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17511 2024-04-28 19:58:43.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-28 20:02:42.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14663 2024-05-06 15:39:18.000000 Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.91.8/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    13060 2024-04-26 18:13:38.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4872 2024-04-26 15:18:54.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    21997 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.91.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.91.8/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14317 2024-05-08 23:47:18.000000 Simba-UW-tf-dev-1.91.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18552 2024-04-28 20:07:14.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15406 2024-05-07 01:16:15.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   123264 2024-05-08 16:16:57.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     3674 2024-05-06 19:29:28.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/brightness_contrast_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     3595 2024-05-06 15:51:58.000000 Simba-UW-tf-dev-1.91.8/simba/video_processors/clahe_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    82357 2024-05-08 15:59:40.000000 Simba-UW-tf-dev-1.91.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-05-06 14:15:23.000000 Simba-UW-tf-dev-1.91.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.91.8/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     4256 2024-05-06 13:20:42.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/brightness.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.91.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    24073 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      797 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-05-08 23:57:40.000000 Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.91.8/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.91.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.91.8/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.91.8/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.91.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.91.8/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3921 2024-04-26 17:59:40.000000 Simba-UW-tf-dev-1.91.8/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.91.8/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.91.8/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-05-08 23:53:08.000000 Simba-UW-tf-dev-1.91.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-05-08 23:57:41.000000 Simba-UW-tf-dev-1.91.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.91.7/PKG-INFO` & `Simba-UW-tf-dev-1.91.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.91.7
+Version: 1.91.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.91.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.91.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.91.8/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.91.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.91.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.91.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.91.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.91.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.91.8/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.91.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/train_model_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import ast
 import concurrent
 import configparser
 import os
 import pickle
 import platform
+import subprocess
 from concurrent.futures import ProcessPoolExecutor
 from concurrent.futures.process import BrokenProcessPool
 from copy import deepcopy
 from datetime import datetime
 from itertools import repeat
 from subprocess import call
 
@@ -320,93 +321,62 @@
         print("Performing SMOTE oversampling...")
         smt = SMOTE(sampling_strategy=sample_ratio)
         if hasattr(smt, "fit_sample"):
             return smt.fit_sample(x_train, y_train)
         else:
             return smt.fit_resample(x_train, y_train)
 
-    def calc_permutation_importance(
-        self,
-        x_test: np.ndarray,
-        y_test: np.ndarray,
-        clf: RandomForestClassifier,
-        feature_names: List[str],
-        clf_name: str,
-        save_dir: Union[str, os.PathLike],
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def calc_permutation_importance(self,
+                                    x_test: np.ndarray,
+                                    y_test: np.ndarray,
+                                    clf: RandomForestClassifier,
+                                    feature_names: List[str],
+                                    clf_name: str,
+                                    save_dir: Union[str, os.PathLike],
+                                    save_file_no: Optional[int] = None) -> None:
         """
-        Helper to calculate feature permutation importance scores.
+        Computes feature permutation importance scores.
 
         :parameter np.ndarray x_test: 2d feature test data of shape len(frames) x len(features)
         :parameter np.ndarray y_test: 2d feature target test data of shape len(frames) x 1
         :parameter RandomForestClassifier clf: random forest classifier
         :parameter List[str] feature_names: Names of features in x_test
         :parameter str clf_name: Name of classifier in y_test
         :parameter str save_dir: Directory where to save results in CSV format
-        :parameter Optional[int] save_file_no: If permutation importance calculation is part of a grid search, provide integer representing sequence.
+        :parameter Optional[int] save_file_no: If permutation importance calculation is part of a grid search, provide integer identifier representing the model in the grid serach sequence. Will be used as suffix in output filename.
         """
 
         print("Calculating feature permutation importances...")
         timer = SimbaTimer(start=True)
-        p_importances = permutation_importance(
-            clf, x_test, y_test, n_repeats=10, random_state=0
-        )
-        df = pd.DataFrame(
-            np.column_stack(
-                [
-                    feature_names,
-                    p_importances.importances_mean,
-                    p_importances.importances_std,
-                ]
-            ),
-            columns=[
-                "FEATURE_NAME",
-                "FEATURE_IMPORTANCE_MEAN",
-                "FEATURE_IMPORTANCE_STDEV",
-            ],
-        )
+        p_importances = permutation_importance(clf, x_test, y_test, n_repeats=10, random_state=0)
+        df = pd.DataFrame(np.column_stack([feature_names, p_importances.importances_mean, p_importances.importances_std]), columns=["FEATURE_NAME","FEATURE_IMPORTANCE_MEAN","FEATURE_IMPORTANCE_STDEV"])
         df = df.sort_values(by=["FEATURE_IMPORTANCE_MEAN"], ascending=False)
         if save_file_no != None:
-            save_file_path = os.path.join(
-                save_dir,
-                clf_name
-                + "_"
-                + str(save_file_no + 1)
-                + "_permutations_importances.csv",
-            )
+            save_file_path = os.path.join(save_dir, f'{clf_name}_{save_file_no}_permutations_importances.csv')
         else:
-            save_file_path = os.path.join(
-                save_dir, clf_name + "_permutations_importances.csv"
-            )
+            save_file_path = os.path.join(save_dir, f"{clf_name}_permutations_importances.csv")
         df.to_csv(save_file_path, index=False)
         timer.stop_timer()
-        print(
-            "Permutation importance calculation complete (elapsed time: {}s) ...".format(
-                timer.elapsed_time_str
-            )
-        )
+        print(f"Permutation importance calculation complete (elapsed time: {timer.elapsed_time_str}s) ...")
 
-    def calc_learning_curve(
-        self,
-        x_y_df: pd.DataFrame,
-        clf_name: str,
-        shuffle_splits: int,
-        dataset_splits: int,
-        tt_size: float,
-        rf_clf: RandomForestClassifier,
-        save_dir: str,
-        save_file_no: Optional[int] = None,
-        multiclass: bool = False,
-    ) -> None:
+    def calc_learning_curve(self,
+                            x_y_df: pd.DataFrame,
+                            clf_name: str,
+                            shuffle_splits: int,
+                            dataset_splits: int,
+                            tt_size: float,
+                            rf_clf: RandomForestClassifier,
+                            save_dir: str,
+                            save_file_no: Optional[int] = None,
+                            multiclass: bool = False) -> None:
         """
         Helper to compute random forest learning curves with cross-validation.
 
         .. image:: _static/img/learning_curves.png
-           :width: 400
+           :width: 600
            :align: center
 
         :parameter pd.DataFrame x_y_df: Dataframe holding features and target.
         :parameter str clf_name: Name of the classifier
         :parameter int shuffle_splits: Number of cross-validation datasets at each data split.
         :parameter int dataset_splits: Number of data splits.
         :parameter float tt_size: test size
@@ -415,77 +385,48 @@
         :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not part of a grid search.
         :parameter bool multiclass: If True, then target consist of several categories [0, 1, 2 ...] and scoring becomes ``None``. If False, then coring ``f1``.
         """
 
         print("Calculating learning curves...")
         timer = SimbaTimer(start=True)
         x_df, y_df = self.split_df_to_x_y(x_y_df, clf_name)
+        check_int(name=f'calc_learning_curve shuffle_splits', value=shuffle_splits, min_value=2)
+        check_int(name=f'calc_learning_curve dataset_splits', value=dataset_splits, min_value=2)
         cv = ShuffleSplit(n_splits=shuffle_splits, test_size=tt_size)
         scoring = "f1"
         if multiclass:
             scoring = None
         if platform.system() == "Darwin":
             with parallel_backend("threading", n_jobs=-2):
-                train_sizes, train_scores, test_scores = learning_curve(
-                    estimator=rf_clf,
-                    X=x_df,
-                    y=y_df,
-                    cv=cv,
-                    scoring=scoring,
-                    shuffle=False,
-                    verbose=0,
-                    train_sizes=np.linspace(0.01, 1.0, dataset_splits),
-                    error_score="raise",
-                )
+                train_sizes, train_scores, test_scores = learning_curve(estimator=rf_clf, X=x_df, y=y_df, cv=cv, scoring=scoring, shuffle=False, verbose=0, train_sizes=np.linspace(0.01, 1.0, dataset_splits), error_score="raise")
         else:
-            train_sizes, train_scores, test_scores = learning_curve(
-                estimator=rf_clf,
-                X=x_df,
-                y=y_df,
-                cv=cv,
-                scoring=scoring,
-                shuffle=False,
-                n_jobs=-1,
-                verbose=0,
-                train_sizes=np.linspace(0.01, 1.0, dataset_splits),
-                error_score="raise",
-            )
+            train_sizes, train_scores, test_scores = learning_curve(estimator=rf_clf, X=x_df, y=y_df, cv=cv, scoring=scoring, shuffle=False, n_jobs=-1, verbose=0, train_sizes=np.linspace(0.01, 1.0, dataset_splits), error_score="raise")
         results_df = pd.DataFrame()
         results_df["FRACTION TRAIN SIZE"] = np.linspace(0.01, 1.0, dataset_splits)
         results_df["TRAIN_MEAN_F1"] = np.mean(train_scores, axis=1)
         results_df["TEST_MEAN_F1"] = np.mean(test_scores, axis=1)
         results_df["TRAIN_STDEV_F1"] = np.std(train_scores, axis=1)
         results_df["TEST_STDEV_F1"] = np.std(test_scores, axis=1)
         if save_file_no != None:
-            self.learning_curve_save_path = os.path.join(
-                save_dir, clf_name + "_" + str(save_file_no + 1) + "_learning_curve.csv"
-            )
+            self.learning_curve_save_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}_learning_curve.csv")
         else:
-            self.learning_curve_save_path = os.path.join(
-                save_dir, clf_name + "_learning_curve.csv"
-            )
+            self.learning_curve_save_path = os.path.join(save_dir, f"{clf_name}_learning_curve.csv")
         results_df.to_csv(self.learning_curve_save_path, index=False)
         timer.stop_timer()
-        print(
-            "Learning curve calculation complete (elapsed time: {}s) ...".format(
-                timer.elapsed_time_str
-            )
-        )
+        print(f"Learning curve calculation complete (elapsed time: {timer.elapsed_time_str}s) ...")
 
-    def calc_pr_curve(
-        self,
-        rf_clf: RandomForestClassifier,
-        x_df: pd.DataFrame,
-        y_df: pd.DataFrame,
-        clf_name: str,
-        save_dir: str,
-        multiclass: bool = False,
-        classifier_map: Dict[int, str] = None,
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def calc_pr_curve(self,
+                      rf_clf: RandomForestClassifier,
+                      x_df: pd.DataFrame,
+                      y_df: pd.DataFrame,
+                      clf_name: str,
+                      save_dir: str,
+                      multiclass: bool = False,
+                      classifier_map: Dict[int, str] = None,
+                      save_file_no: Optional[int] = None) -> None:
         """
         Helper to compute random forest precision-recall curve.
 
         .. image:: _static/img/pr_curves.png
            :width: 800
            :align: center
 
@@ -496,285 +437,231 @@
         :parameter str save_dir: Directory where to save output in csv file format.
         :parameter bool multiclass: If the classifier is a multi-classifier. Default: False.
         :parameter Dict[int, str] classifier_map: If multiclass, dictionary mapping integers to classifier names.
         :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not part of a grid search.
         """
 
         if multiclass and classifier_map is None:
-            raise InvalidInputError(
-                msg="Creating PR curve for multi-classifier but classifier_map not defined. Add classifier_map argument"
-            )
+            raise InvalidInputError(msg="Creating PR curve for multi-classifier but classifier_map not defined. Pass classifier_map argument")
         print("Calculating PR curves...")
         timer = SimbaTimer(start=True)
         if not multiclass:
             p = rf_clf.predict_proba(x_df)[:, 1]
             precision, recall, thresholds = precision_recall_curve(y_df, p, pos_label=1)
             pr_df = pd.DataFrame()
             pr_df["PRECISION"] = precision
             pr_df["RECALL"] = recall
-            pr_df["F1"] = (
-                2
-                * (pr_df["RECALL"] * pr_df["PRECISION"])
-                / (pr_df["RECALL"] + pr_df["PRECISION"])
-            )
+            pr_df["F1"] = (2 * (pr_df["RECALL"] * pr_df["PRECISION"]) / (pr_df["RECALL"] + pr_df["PRECISION"]))
             thresholds = list(thresholds)
             thresholds.insert(0, 0.00)
             pr_df["DISCRIMINATION THRESHOLDS"] = thresholds
         else:
             pr_df_lst = []
-            p = self.clf_predict_proba(
-                clf=rf_clf, x_df=x_df, multiclass=True, model_name=clf_name
-            )
+            p = self.clf_predict_proba(clf=rf_clf, x_df=x_df, multiclass=True, model_name=clf_name)
             for i in range(p.shape[1]):
-                precision, recall, thresholds = precision_recall_curve(
-                    y_df, p[:, i], pos_label=i
-                )
+                precision, recall, thresholds = precision_recall_curve(y_df, p[:, i], pos_label=i)
                 df = pd.DataFrame()
                 df["PRECISION"] = precision
                 df["RECALL"] = recall
-                df["F1"] = (
-                    2
-                    * (df["RECALL"] * df["PRECISION"])
-                    / (df["RECALL"] + df["PRECISION"])
-                )
+                df["F1"] = (2* (df["RECALL"] * df["PRECISION"]) / (df["RECALL"] + df["PRECISION"]))
                 thresholds = list(thresholds)
                 thresholds.insert(0, 0.00)
                 df["DISCRIMINATION THRESHOLDS"] = thresholds
                 df.insert(0, "BEHAVIOR CLASS", classifier_map[i])
                 pr_df_lst.append(df)
             pr_df = pd.concat(pr_df_lst, axis=0).reset_index(drop=True)
         if save_file_no != None:
-            self.pr_save_path = os.path.join(
-                save_dir, clf_name + "_" + str(save_file_no + 1) + "_pr_curve.csv"
-            )
+            self.pr_save_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}_pr_curve.csv")
         else:
-            self.pr_save_path = os.path.join(save_dir, clf_name + "_pr_curve.csv")
+            self.pr_save_path = os.path.join(save_dir, f"{clf_name}_pr_curve.csv")
         pr_df.to_csv(self.pr_save_path, index=False)
         timer.stop_timer()
-        print(
-            "Precision-recall curve calculation complete (elapsed time: {}s) ...".format(
-                timer.elapsed_time_str
-            )
-        )
+        print(f"Precision-recall curve calculation complete (elapsed time: {timer.elapsed_time_str}s) ...")
 
-    def create_example_dt(
-        self,
-        rf_clf: RandomForestClassifier,
-        clf_name: str,
-        feature_names: List[str],
-        class_names: List[str],
-        save_dir: str,
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def create_example_dt(self,
+                          rf_clf: RandomForestClassifier,
+                          clf_name: str,
+                          feature_names: List[str],
+                          class_names: List[str],
+                          save_dir: str,
+                          tree_id: Optional[int] = 3,
+                          save_file_no: Optional[int] = None) -> None:
         """
         Helper to produce visualization of random forest decision tree using graphviz.
 
+        .. image:: _static/img/create_example_dt.png
+           :width: 700
+           :align: center
+
+        .. note::
+           `Example expected output  <https://github.com/sgoldenlab/simba/blob/master/misc/create_example_dt.pdf>`__.
+
         :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
         :parameter str clf_name: Classifier name.
         :parameter List[str] feature_names: List of feature names.
         :parameter List[str] class_names: List of classes. E.g., ['Attack absent', 'Attack present']
         :parameter str save_dir: Directory where to save output in csv file format.
-        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
-            part of a grid search.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not part of a grid search.
         """
 
         print("Visualizing example decision tree using graphviz...")
-        estimator = rf_clf.estimators_[3]
+        timer = SimbaTimer(start=True)
+        estimator = rf_clf.estimators_[tree_id]
         if save_file_no != None:
-            dot_name = os.path.join(
-                save_dir, str(clf_name) + "_" + str(save_file_no) + "_tree.dot"
-            )
-            file_name = os.path.join(
-                save_dir, str(clf_name) + "_" + str(save_file_no) + "_tree.pdf"
-            )
+            dot_name = os.path.join(save_dir, f"{clf_name}_{save_file_no}_tree.dot")
+            file_name = os.path.join(save_dir, f"{clf_name}_{save_file_no}_tree.pdf")
         else:
-            dot_name = os.path.join(save_dir, str(clf_name) + "_tree.dot")
-            file_name = os.path.join(save_dir, str(clf_name) + "_tree.pdf")
-        export_graphviz(
-            estimator,
-            out_file=dot_name,
-            filled=True,
-            rounded=True,
-            special_characters=False,
-            impurity=False,
-            class_names=class_names,
-            feature_names=feature_names,
-        )
-        command = "dot " + str(dot_name) + " -T pdf -o " + str(file_name) + " -Gdpi=600"
+            dot_name = os.path.join(save_dir, f"{clf_name}_tree.dot")
+            file_name = os.path.join(save_dir, f"{clf_name}_tree.pdf")
+        export_graphviz(estimator,
+                        out_file=dot_name,
+                        filled=True,
+                        rounded=True,
+                        special_characters=False,
+                        impurity=False,
+                        class_names=class_names,
+                        feature_names=feature_names)
+
+        command = f"dot {dot_name} -T pdf -o {file_name} -Gdpi=600"
         call(command, shell=True)
+        timer.stop_timer()
+        print(f'Example tree saved at {file_name} (elapsed time: {timer.elapsed_time_str}s)')
+
+    def create_clf_report(self,
+                          rf_clf: RandomForestClassifier,
+                          x_df: pd.DataFrame,
+                          y_df: pd.DataFrame,
+                          class_names: List[str],
+                          save_dir: str,
+                          clf_name: Optional[str] = None,
+                          save_file_no: Optional[int] = None) -> None:
+
 
-    def create_clf_report(
-        self,
-        rf_clf: RandomForestClassifier,
-        x_df: pd.DataFrame,
-        y_df: pd.DataFrame,
-        class_names: List[str],
-        save_dir: str,
-        clf_name: Optional[str] = None,
-        save_file_no: Optional[int] = None,
-    ) -> None:
         """
         Helper to create classifier truth table report.
 
         .. seealso::
            `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
-            .. image:: _static/img/clf_report.png
-               :width: 400
-               :align: center
+
+        .. image:: _static/img/clf_report.png
+           :width: 500
+           :align: center
 
         :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
         :parameter pd.DataFrame x_df: dataframe holding test features
         :parameter pd.DataFrame y_df: dataframe holding test target
         :parameter List[str] class_names: List of classes. E.g., ['Attack absent', 'Attack present']
         :parameter Optional[str] clf_name: Name of the classifier. If not None, then used in the output file name.
         :parameter str save_dir: Directory where to save output in csv file format.
         :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
         """
 
         print("Creating classification report visualization...")
+        timer = SimbaTimer(start=True)
         try:
             visualizer = ClassificationReport(rf_clf, classes=class_names, support=True)
             visualizer.score(x_df, y_df)
             if save_file_no != None:
                 if not clf_name:
-                    save_path = os.path.join(
-                        save_dir,
-                        class_names[1]
-                        + "_"
-                        + str(save_file_no)
-                        + "_classification_report.png",
-                    )
+                    save_path = os.path.join(save_dir, f'{class_names[1]}_{save_file_no}_classification_report.png')
                 else:
-                    save_path = os.path.join(
-                        save_dir, f"{clf_name}_{save_file_no}_classification_report.png"
-                    )
+                    save_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}_classification_report.png")
             else:
                 if not clf_name:
-                    save_path = os.path.join(
-                        save_dir, class_names[1] + "_classification_report.png"
-                    )
+                    save_path = os.path.join(save_dir, f"{class_names[1]}_classification_report.png")
                 else:
-                    save_path = os.path.join(
-                        save_dir, f"{clf_name}_classification_report.png"
-                    )
+                    save_path = os.path.join(save_dir, f"{clf_name}_classification_report.png")
             visualizer.poof(outpath=save_path, clear_figure=True)
+            timer.stop_timer()
+            print(f'Classification report saved at {save_path} (elapsed time: {timer.elapsed_time_str}s)')
         except KeyError as e:
+            print(e.args)
             if not clf_name:
-                NotEnoughDataWarning(
-                    msg=f"Not enough data to create classification report, consider changing sampling settings or create more annotations: {class_names[1]}",
-                    source=self.__class__.__name__,
-                )
+                NotEnoughDataWarning(msg=f"Not enough data to create classification report, consider changing sampling settings or create more annotations: {class_names[1]}",source=self.__class__.__name__)
             else:
-                NotEnoughDataWarning(
-                    msg=f"Not enough data to create classification report, consider changing sampling settings or create more annotations: {clf_name}",
-                    source=self.__class__.__name__,
-                )
+                NotEnoughDataWarning(msg=f"Not enough data to create classification report, consider changing sampling settings or create more annotations: {clf_name}", source=self.__class__.__name__)
 
-    def create_x_importance_log(
-        self,
-        rf_clf: RandomForestClassifier,
-        x_names: List[str],
-        clf_name: str,
-        save_dir: str,
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def create_x_importance_log(self,
+                                rf_clf: RandomForestClassifier,
+                                x_names: List[str],
+                                clf_name: str,
+                                save_dir: str,
+                                save_file_no: Optional[int] = None) -> None:
         """
         Helper to save gini or entropy based feature importance scores.
 
+        .. note::
+           `Example expected output  <https://github.com/sgoldenlab/simba/blob/master/images/BtWGaNP_feature_importance_log.csv>`__.
+
         :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
         :parameter List[str] x_names: Names of features.
         :parameter str clf_name: Name of classifier
         :parameter str save_dir: Directory where to save output in csv file format.
-        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
-            part of a grid search.
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not part of a grid search.
         """
 
         print("Creating feature importance log...")
+        timer = SimbaTimer(start=True)
         importances = list(rf_clf.feature_importances_)
-        feature_importances = [
-            (feature, round(importance, 2))
-            for feature, importance in zip(x_names, importances)
-        ]
-        df = pd.DataFrame(
-            feature_importances, columns=["FEATURE", "FEATURE_IMPORTANCE"]
-        ).sort_values(by=["FEATURE_IMPORTANCE"], ascending=False)
+        feature_importances = [(feature, round(importance, 2)) for feature, importance in zip(x_names, importances)]
+        df = pd.DataFrame(feature_importances, columns=["FEATURE", "FEATURE_IMPORTANCE"]).sort_values(by=["FEATURE_IMPORTANCE"], ascending=False)
         if save_file_no != None:
-            self.f_importance_save_path = os.path.join(
-                save_dir,
-                clf_name + "_" + str(save_file_no) + "_feature_importance_log.csv",
-            )
+            self.f_importance_save_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}_feature_importance_log.csv")
         else:
-            self.f_importance_save_path = os.path.join(
-                save_dir, clf_name + "_feature_importance_log.csv"
-            )
+            self.f_importance_save_path = os.path.join(save_dir, f"{clf_name}_feature_importance_log.csv")
         df.to_csv(self.f_importance_save_path, index=False)
+        timer.stop_timer()
+        print(f'Feature importance log saved at {self.f_importance_save_path} (elapsed time: {timer.elapsed_time_str}s)')
 
-    def create_x_importance_bar_chart(
-        self,
-        rf_clf: RandomForestClassifier,
-        x_names: list,
-        clf_name: str,
-        save_dir: str,
-        n_bars: int,
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def create_x_importance_bar_chart(self,
+                                      rf_clf: RandomForestClassifier,
+                                      x_names: list,
+                                      clf_name: str,
+                                      save_dir: str,
+                                      n_bars: int,
+                                      palette: Optional[str] = 'hot',
+                                      save_file_no: Optional[int] = None) -> None:
         """
         Helper to create a bar chart displaying the top N gini or entropy feature importance scores.
 
         .. seealso::
            `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
-            .. image:: _static/img/gini_bar_chart.png
-               :width: 400
-               :align: center
+        
+        .. image:: _static/img/gini_bar_chart.png
+           :width: 600
+           :align: center
 
         :parameter RandomForestClassifier rf_clf: sklearn RandomForestClassifier object.
         :parameter List[str] x_names: Names of features.
         :parameter str clf_name: Name of classifier.
         :parameter str save_dir: Directory where to save output in csv file format.
         :parameter int n_bars: Number of bars in the plot.
-        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
-            part of a grid search
+        :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not part of a grid search
         """
 
         check_int(name="FEATURE IMPORTANCE BAR COUNT", value=n_bars, min_value=1)
         print("Creating feature importance bar chart...")
+        timer = SimbaTimer(start=True)
         self.create_x_importance_log(rf_clf, x_names, clf_name, save_dir)
-        importances_df = pd.read_csv(
-            os.path.join(save_dir, clf_name + "_feature_importance_log.csv")
-        )
+        importances_df = pd.read_csv(os.path.join(save_dir, f"{clf_name}_feature_importance_log.csv"))
         importances_head = importances_df.head(n_bars)
-        colors = create_color_palette(
-            pallete_name="hot", increments=n_bars, as_rgb_ratio=True
-        )
+        colors = create_color_palette(pallete_name=palette, increments=n_bars, as_rgb_ratio=True)
         colors = [x[::-1] for x in colors]
-        ax = importances_head.plot.bar(
-            x="FEATURE",
-            y="FEATURE_IMPORTANCE",
-            legend=False,
-            rot=90,
-            fontsize=6,
-            color=colors,
-        )
+        ax = importances_head.plot.bar(x="FEATURE", y="FEATURE_IMPORTANCE", legend=False, rot=90, fontsize=6, color=colors)
         plt.ylabel("Feature importances' (mean decrease impurity)", fontsize=6)
         plt.tight_layout()
         if save_file_no != None:
-            save_file_path = os.path.join(
-                save_dir,
-                clf_name
-                + "_"
-                + str(save_file_no)
-                + "_feature_importance_bar_graph.png",
-            )
+            save_file_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}_feature_importance_bar_graph.png")
         else:
-            save_file_path = os.path.join(
-                save_dir, clf_name + "_feature_importance_bar_graph.png"
-            )
+            save_file_path = os.path.join(save_dir, f"{clf_name}_feature_importance_bar_graph.png")
         plt.savefig(save_file_path, dpi=600)
         plt.close("all")
+        timer.stop_timer()
+        print(f'Feature importance bar chart complete, saved at {save_file_path} (elapsed time: {timer.elapsed_time_str}s)')
 
     def dviz_classification_visualization(
         self,
         x_train: np.ndarray,
         y_train: np.ndarray,
         clf_name: str,
         class_names: List[str],
@@ -815,17 +702,15 @@
         except:
             NoModuleWarning(
                 msg='Skipping dtreeviz example decision tree visualization. Make sure "graphviz" is installed.',
                 source=self.__class__.__name__,
             )
 
     @staticmethod
-    def split_and_group_df(
-        df: pd.DataFrame, splits: int, include_split_order: bool = True
-    ) -> (List[pd.DataFrame], int):
+    def split_and_group_df(df: pd.DataFrame, splits: int, include_split_order: bool = True) -> (List[pd.DataFrame], int):
         """
         Helper to split a dataframe for multiprocessing. If include_split_order, then include the group number
         in split data as a column. Returns split data and approximations of number of observations per split.
         """
         data_arr = np.array_split(df, splits)
         if include_split_order:
             for df_cnt in range(len(data_arr)):
@@ -849,17 +734,17 @@
         Compute SHAP values for a random forest classifier.
 
         This method computes SHAP (SHapley Additive exPlanations) values for a given random forest classifier.
 
         .. seealso::
            `Documentation <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#train-predictive-classifiers-settings>`_
 
-           .. image:: _static/img/shap.png
-              :width: 400
-              :align: center
+        .. image:: _static/img/shap.png
+           :width: 600
+           :align: center
 
         .. note::
            For improved run-times, use multiprocessing through :meth:`simba.mixins.train_model_mixins.TrainModelMixin.create_shap_log_mp`
            Uses TreeSHAP `Documentation <https://shap.readthedocs.io/en/latest/index.html>`_
 
         The SHAP value for feature 'i' in the context of a prediction 'f' and input 'x' is calculated using the following formula:
 
@@ -1001,17 +886,16 @@
             ["Over sampling ratio", model_dict[MLParamKeys.OVERSAMPLE_RATIO.value]],
             ["criterion", model_dict[MLParamKeys.RF_CRITERION.value]],
             ["Min sample leaf", model_dict[MLParamKeys.MIN_LEAF.value]],
         ]
         table = tabulate(table_view, ["Setting", "value"], tablefmt="grid")
         print(f"{table} {Defaults.STR_SPLIT_DELIMITER.value}TABLE")
 
-    def create_meta_data_csv_training_one_model(
-        self, meta_data_lst: list, clf_name: str, save_dir: Union[str, os.PathLike]
-    ) -> None:
+    def create_meta_data_csv_training_one_model(self, meta_data_lst: list, clf_name: str, save_dir: Union[str, os.PathLike]) -> None:
+
         """
         Helper to save single model meta data (hyperparameters, sampling settings etc.) from list format into SimBA
         compatible CSV config file.
 
         :parameter list meta_data_lst: Meta data in list format
         :parameter str clf_name: Name of classifier
         :parameter str clf_name: Name of classifier
@@ -1019,49 +903,41 @@
         """
         print("Saving model meta data file...")
         save_path = os.path.join(save_dir, clf_name + "_meta.csv")
         out_df = pd.DataFrame(columns=get_meta_data_file_headers())
         out_df.loc[len(out_df)] = meta_data_lst
         out_df.to_csv(save_path)
 
-    def create_meta_data_csv_training_multiple_models(
-        self, meta_data, clf_name, save_dir, save_file_no: Optional[int] = None
-    ) -> None:
+    def create_meta_data_csv_training_multiple_models(self, meta_data, clf_name, save_dir, save_file_no: Optional[int] = None) -> None:
         print("Saving model meta data file...")
         save_path = os.path.join(save_dir, f"{clf_name}_{str(save_file_no)}_meta.csv")
         out_df = pd.DataFrame.from_dict(meta_data, orient="index").T
         out_df.to_csv(save_path)
 
-    def save_rf_model(
-        self,
-        rf_clf: RandomForestClassifier,
-        clf_name: str,
-        save_dir: Union[str, os.PathLike],
-        save_file_no: Optional[int] = None,
-    ) -> None:
+    def save_rf_model(self,
+                      rf_clf: RandomForestClassifier,
+                      clf_name: str,
+                      save_dir: Union[str, os.PathLike],
+                      save_file_no: Optional[int] = None) -> None:
         """
         Helper to save pickled classifier object to disk.
 
         :parameter RandomForestClassifier rf_clf: sklearn random forest classifier
         :parameter str clf_name: Classifier name
         :parameter str save_dir: Directory where to save output in csv file format.
         :parameter Optional[int] save_file_no: If integer, represents the count of the classifier within a grid search. If none, the classifier is not
             part of a grid search.
         """
         if save_file_no != None:
-            save_path = os.path.join(
-                save_dir, clf_name + "_" + str(save_file_no) + ".sav"
-            )
+            save_path = os.path.join(save_dir, f"{clf_name}_{save_file_no}.sav")
         else:
-            save_path = os.path.join(save_dir, clf_name + ".sav")
+            save_path = os.path.join(save_dir, f"{clf_name}.sav")
         pickle.dump(rf_clf, open(save_path, "wb"))
 
-    def get_model_info(
-        self, config: configparser.ConfigParser, model_cnt: int
-    ) -> Dict[int, Any]:
+    def get_model_info(self, config: configparser.ConfigParser, model_cnt: int) -> Dict[int, Any]:
         """
         Helper to read in N SimBA random forest config meta files to python dict memory.
 
         :parameter configparser.ConfigParser config: Parsed SimBA project_config.ini
         :parameter int model_cnt: Count of models
         :return dict: Dictionary with integers as keys and hyperparameter dictionaries as keys.
         """
```

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.91.8/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.91.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.91.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.91.8/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/CLAHE.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/CLAHE.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/downsample_video_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/downsample_video_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/downsample_multiple_videos_popup.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/downsample_multiple_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/mahalanobis.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/mahalanobis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/superpixels.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/superpixels.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/superimpose_frame_count.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/superimpose_frame_count.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/eta_squared.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/eta_squared.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fleiss_kappa.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fleiss_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/jaccard_distance.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/jaccard_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/manhattan_distance.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/manhattan_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/seekable.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/seekable.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/relative_risk.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/relative_risk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/contrast.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/contrast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/youden_j.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/youden_j.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.91.8/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.91.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.91.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.91.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.91.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.91.8/simba/model/train_rf.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,57 +25,38 @@
     :param str config_path: path to SimBA project config file in Configparser format
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario1.md#step-7-train-machine-model>`_
 
     :example:
     >>> model_trainer = TrainRandomForestClassifier(config_path='MyConfigPath')
-    >>> model_trainer.perform_sampling()
-    >>> model_trainer.train_model()
-    >>> model_trainer.save_model()
+    >>> model_trainer.run()
+    >>> model_trainer.save()
     """
 
-    def __init__(self, config_path: Union[str, os.PathLike]):
+    def __init__(self,
+                 config_path: Union[str, os.PathLike]):
 
         ConfigReader.__init__(self, config_path=config_path, create_logger=False)
         TrainModelMixin.__init__(self)
         self.read_model_settings_from_config(config=self.config)
-        check_if_filepath_list_is_empty(
-            filepaths=self.target_file_paths,
-            error_msg="Zero annotation files found in project_folder/csv/targets_inserted directory, cannot create model.",
-        )
+        check_if_filepath_list_is_empty(filepaths=self.target_file_paths, error_msg=f"Zero annotation files found in directory {self.targets_folder}, cannot create model.")
         print(f"Reading in {len(self.target_file_paths)} annotated files...")
-        self.data_df, self.frm_idx = self.read_all_files_in_folder_mp(
-            self.target_file_paths, self.file_type, [self.clf_name]
-        )
-        self.frm_idx = pd.DataFrame(
-            {"VIDEO": list(self.data_df.index), "FRAME_IDX": self.frm_idx}
-        )
-        self.data_df = self.check_raw_dataset_integrity(
-            df=self.data_df, logs_path=self.logs_path
-        )
+        self.data_df, self.frm_idx = self.read_all_files_in_folder_mp(self.target_file_paths, self.file_type, [self.clf_name])
+        self.frm_idx = pd.DataFrame({"VIDEO": list(self.data_df.index), "FRAME_IDX": self.frm_idx})
+        self.data_df = self.check_raw_dataset_integrity(df=self.data_df, logs_path=self.logs_path)
         self.data_df_wo_cords = self.drop_bp_cords(df=self.data_df)
-        annotation_cols_to_remove = self.read_in_all_model_names_to_remove(
-            self.config, self.clf_cnt, self.clf_name
-        )
-        self.x_y_df = self.delete_other_annotation_columns(
-            self.data_df_wo_cords, list(annotation_cols_to_remove)
-        )
+        annotation_cols_to_remove = self.read_in_all_model_names_to_remove(self.config, self.clf_cnt, self.clf_name)
+        self.x_y_df = self.delete_other_annotation_columns(self.data_df_wo_cords, list(annotation_cols_to_remove))
         self.class_names = ["Not_" + self.clf_name, self.clf_name]
         self.x_df, self.y_df = self.split_df_to_x_y(self.x_y_df, self.clf_name)
         self.feature_names = self.x_df.columns
         self.check_sampled_dataset_integrity(x_df=self.x_df, y_df=self.y_df)
-        print("Number of features in dataset: " + str(len(self.x_df.columns)))
-        print(
-            "Number of {} frames in dataset: {} ({}%)".format(
-                self.clf_name,
-                str(self.y_df.sum()),
-                str(round(self.y_df.sum() / len(self.y_df), 4) * 100),
-            )
-        )
+        print(f"Number of features in dataset: {len(self.x_df.columns)}")
+        print(f"Number of {self.clf_name} frames in dataset: {self.y_df.sum()} ({str(round(self.y_df.sum() / len(self.y_df), 4) * 100)}%)")
 
     def perform_sampling(self):
         """
         Method for sampling data for training and testing, and perform over and under-sampling of the training sets
         as indicated within the SimBA project config.
         """
 
@@ -127,130 +108,37 @@
         """
         Method for training single random forest model.
         """
         print("Training and evaluating model...")
         self.timer = SimbaTimer(start=True)
         self.perform_sampling()
         if self.algo == "RF":
-            n_estimators = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.RF_ESTIMATORS.value,
-                data_type=Dtypes.INT.value,
-            )
-            max_features = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.RF_MAX_FEATURES.value,
-                data_type=Dtypes.STR.value,
-            )
+            n_estimators = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.RF_ESTIMATORS.value,data_type=Dtypes.INT.value)
+            max_features = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.RF_MAX_FEATURES.value,data_type=Dtypes.STR.value)
             if max_features == "None":
                 max_features = None
-            criterion = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.RF_CRITERION.value,
-                data_type=Dtypes.STR.value,
-                options=Options.CLF_CRITERION.value,
-            )
-            min_sample_leaf = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.MIN_LEAF.value,
-                data_type=Dtypes.INT.value,
-            )
-            compute_permutation_importance = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.PERMUTATION_IMPORTANCE.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_learning_curve = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.LEARNING_CURVE.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_precision_recall_curve = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.PRECISION_RECALL.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_example_decision_tree = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.EX_DECISION_TREE.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_classification_report = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.CLF_REPORT.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_features_importance_log = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.IMPORTANCE_LOG.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_features_importance_bar_graph = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.IMPORTANCE_LOG.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_example_decision_tree_fancy = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.EX_DECISION_TREE_FANCY.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            generate_shap_scores = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.SHAP_SCORES.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            save_meta_data = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.RF_METADATA.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-            compute_partial_dependency = read_config_entry(
-                self.config,
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.PARTIAL_DEPENDENCY.value,
-                data_type=Dtypes.STR.value,
-                default_value=False,
-            )
-
-            if self.config.has_option(
-                ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                MLParamKeys.CLASS_WEIGHTS.value,
-            ):
-                class_weights = read_config_entry(
-                    self.config,
-                    ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
-                    MLParamKeys.CLASS_WEIGHTS.value,
-                    data_type=Dtypes.STR.value,
-                    default_value=Dtypes.NONE.value,
-                )
+            criterion = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.RF_CRITERION.value, data_type=Dtypes.STR.value, options=Options.CLF_CRITERION.value)
+            min_sample_leaf = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.MIN_LEAF.value, data_type=Dtypes.INT.value)
+            compute_permutation_importance = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.PERMUTATION_IMPORTANCE.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_learning_curve = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.LEARNING_CURVE.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_precision_recall_curve = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.PRECISION_RECALL.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_example_decision_tree = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.EX_DECISION_TREE.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_classification_report = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.CLF_REPORT.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_features_importance_log = read_config_entry(self.config, ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.IMPORTANCE_LOG.value, data_type=Dtypes.STR.value, default_value=False)
+            generate_features_importance_bar_graph = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.IMPORTANCE_LOG.value,data_type=Dtypes.STR.value,default_value=False)
+            generate_example_decision_tree_fancy = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.EX_DECISION_TREE_FANCY.value,data_type=Dtypes.STR.value,default_value=False)
+            generate_shap_scores = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.SHAP_SCORES.value,data_type=Dtypes.STR.value,default_value=False)
+            save_meta_data = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.RF_METADATA.value,data_type=Dtypes.STR.value,default_value=False)
+            compute_partial_dependency = read_config_entry(self.config,ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,MLParamKeys.PARTIAL_DEPENDENCY.value,data_type=Dtypes.STR.value,default_value=False)
+            if self.config.has_option(ConfigKey.CREATE_ENSEMBLE_SETTINGS.value, MLParamKeys.CLASS_WEIGHTS.value):
+                class_weights = read_config_entry(self.config,
+                                                  ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
+                                                  MLParamKeys.CLASS_WEIGHTS.value,
+                                                  data_type=Dtypes.STR.value,
+                                                  default_value=Dtypes.NONE.value)
                 if class_weights == "custom":
                     class_weights = ast.literal_eval(
                         read_config_entry(
                             self.config,
                             ConfigKey.CREATE_ENSEMBLE_SETTINGS.value,
                             MLParamKeys.CLASS_CUSTOM_WEIGHTS.value,
                             data_type=Dtypes.STR.value,
```

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.91.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.91.8/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.91.8/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.91.8/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.91.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.91.8/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.91.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.91.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.91.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/brightness_contrast_ui.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/brightness_contrast_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/video_processors/clahe_ui.py` & `Simba-UW-tf-dev-1.91.8/simba/video_processors/clahe_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.91.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.91.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.91.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.91.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.91.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.91.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.91.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.91.8/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.91.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.91.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.91.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.91.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.91.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/brightness.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/brightness.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.91.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.91.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.91.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.91.7
+Version: 1.91.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.91.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/LICENSE` & `Simba-UW-tf-dev-1.91.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.91.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.91.8/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_stats.py` & `Simba-UW-tf-dev-1.91.8/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.91.8/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.91.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.91.8/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.91.8/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.91.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.91.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.91.8/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.91.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.91.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.91.8/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/README.md` & `Simba-UW-tf-dev-1.91.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.91.7/setup.py` & `Simba-UW-tf-dev-1.91.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.91.7",
+    version="1.91.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```

