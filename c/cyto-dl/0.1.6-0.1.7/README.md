# Comparing `tmp/cyto-dl-0.1.6.tar.gz` & `tmp/cyto-dl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyto-dl-0.1.6.tar", last modified: Fri May  3 16:17:38 2024, max compression
+gzip compressed data, was "cyto-dl-0.1.7.tar", last modified: Wed May  8 22:30:04 2024, max compression
```

## Comparing `cyto-dl-0.1.6.tar` & `cyto-dl-0.1.7.tar`

### file list

```diff
@@ -1,280 +1,280 @@
--rw-r--r--   0        0        0     5431 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/README.md
--rw-r--r--   0        0        0      403 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/default.yaml
--rw-r--r--   0        0        0     1250 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/early_stopping.yaml
--rw-r--r--   0        0        0       80 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/layer_freeze.yaml
--rw-r--r--   0        0        0       83 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/learning_rate_monitor.yaml
--rw-r--r--   0        0        0     1298 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/model_checkpoint.yaml
--rw-r--r--   0        0        0      402 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/model_summary.yaml
--rw-r--r--   0        0        0        0 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/none.yaml
--rw-r--r--   0        0        0      160 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/outlier_detection.yaml
--rw-r--r--   0        0        0      289 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/callbacks/rich_progress_bar.yaml
--rw-r--r--   0        0        0      758 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/compile.yaml
--rw-r--r--   0        0        0     2634 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     7077 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/gan.yaml
--rw-r--r--   0        0        0     7427 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     6880 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     5879 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/labelfree.yaml
--rw-r--r--   0        0        0     4374 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/mae.yaml
--rw-r--r--   0        0        0     6852 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation.yaml
--rw-r--r--   0        0        0     8053 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     7263 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0      450 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0      416 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rot_mnist.yaml
--rw-r--r--   0        0        0      450 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rot_mnist_vae.yaml
--rw-r--r--   0        0        0     1176 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/rotated_mnist.yaml
--rw-r--r--   0        0        0     1075 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d.yaml
--rw-r--r--   0        0        0      497 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_npm1.yaml
--rw-r--r--   0        0        0      770 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_npm_nuc_v2.yaml
--rw-r--r--   0        0        0     1802 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_3d_rotate.yaml
--rw-r--r--   0        0        0      547 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_centerslice.yaml
--rw-r--r--   0        0        0      719 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_centerslice_resize.yaml
--rw-r--r--   0        0        0      969 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_npm1.yaml
--rw-r--r--   0        0        0      312 2024-05-03 16:17:29.108416 cyto-dl-0.1.6/configs/data/private/variance_spharm.yaml
--rw-r--r--   0        0        0      462 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/alternating_batch.yaml
--rw-r--r--   0        0        0      200 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/omnipose.yaml
--rw-r--r--   0        0        0      200 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/data/test/segmentation.yaml
--rw-r--r--   0        0        0      899 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/default.yaml
--rw-r--r--   0        0        0      125 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/fdr.yaml
--rw-r--r--   0        0        0      223 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/limit.yaml
--rw-r--r--   0        0        0      209 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/overfit.yaml
--rw-r--r--   0        0        0      182 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/debug/profiler.yaml
--rw-r--r--   0        0        0      509 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/eval.yaml
--rw-r--r--   0        0        0      659 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/classification/per_timepoint.yaml
--rw-r--r--   0        0        0     1065 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/gan.yaml
--rw-r--r--   0        0        0     1083 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/gan_superres.yaml
--rw-r--r--   0        0        0      932 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/instance_seg.yaml
--rw-r--r--   0        0        0      854 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/labelfree.yaml
--rw-r--r--   0        0        0      892 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/mae.yaml
--rw-r--r--   0        0        0      863 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1622 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0      881 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1098 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/im2im/vit_segmentation.yaml
--rw-r--r--   0        0        0     2741 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/lattice_nuc_sdf.yaml
--rw-r--r--   0        0        0     1583 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/mnist_so2.yaml
--rw-r--r--   0        0        0      989 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_classical_3d_vae.yaml
--rw-r--r--   0        0        0     2902 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_classical_scale_inv.yaml
--rw-r--r--   0        0        0     1037 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
--rw-r--r--   0        0        0     2825 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
--rw-r--r--   0        0        0     2568 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so2.yaml
--rw-r--r--   0        0        0     3062 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so2_scale_inv.yaml
--rw-r--r--   0        0        0     3057 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_scale_inv.yaml
--rw-r--r--   0        0        0     2325 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae.yaml
--rw-r--r--   0        0        0     2179 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae_seg.yaml
--rw-r--r--   0        0        0      967 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_classical_2d_vae.yaml
--rw-r--r--   0        0        0     1053 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_classical_3d_vae.yaml
--rw-r--r--   0        0        0     1385 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae.yaml
--rw-r--r--   0        0        0     1605 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
--rw-r--r--   0        0        0     9822 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_spharm.yaml
--rw-r--r--   0        0        0     9728 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/experiment/private/variance_spharm_o2.yaml
--rw-r--r--   0        0        0      309 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/extras/default.yaml
--rw-r--r--   0        0        0     1818 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/hparams_search/mnist_optuna.yaml
--rw-r--r--   0        0        0      431 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/hydra/default.yaml
--rw-r--r--   0        0        0      372 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/comet.yaml
--rw-r--r--   0        0        0      157 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/csv.yaml
--rw-r--r--   0        0        0      148 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/many_loggers.yaml
--rw-r--r--   0        0        0      166 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/mlflow.yaml
--rw-r--r--   0        0        0      277 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/neptune.yaml
--rw-r--r--   0        0        0      258 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/tensorboard.yaml
--rw-r--r--   0        0        0      522 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/logger/wandb.yaml
--rw-r--r--   0        0        0      594 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/classification/single_timepoint.yaml
--rw-r--r--   0        0        0     1807 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/gan.yaml
--rw-r--r--   0        0        0     1948 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/gan_superres.yaml
--rw-r--r--   0        0        0     1333 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/instance_seg.yaml
--rw-r--r--   0        0        0     1237 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/labelfree.yaml
--rw-r--r--   0        0        0     1245 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/mae.yaml
--rw-r--r--   0        0        0     1333 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation.yaml
--rw-r--r--   0        0        0     1252 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation_plugin.yaml
--rw-r--r--   0        0        0     1472 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/segmentation_superres.yaml
--rw-r--r--   0        0        0     1365 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/im2im/vit_segmentation_decoder.yaml
--rw-r--r--   0        0        0      493 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/classical_image_ae.yaml
--rw-r--r--   0        0        0      536 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/classical_image_vae.yaml
--rw-r--r--   0        0        0       86 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
--rw-r--r--   0        0        0       76 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_loss.yaml
--rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_mse.yaml
--rw-r--r--   0        0        0       93 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
--rw-r--r--   0        0        0      316 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/so3_canon_image_vae.yaml
--rw-r--r--   0        0        0      332 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/so3_equiv_image_vae.yaml
--rw-r--r--   0        0        0      513 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/spharm.yaml
--rw-r--r--   0        0        0      501 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/private/spharm_so2.yaml
--rw-r--r--   0        0        0      597 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/test/base.yaml
--rw-r--r--   0        0        0      613 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/model/test/simple_segmentation.yaml
--rw-r--r--   0        0        0      492 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/paths/default.yaml
--rw-r--r--   0        0        0     1745 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/train.yaml
--rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/cpu.yaml
--rw-r--r--   0        0        0      394 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/ddp.yaml
--rw-r--r--   0        0        0      120 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/ddp_sim.yaml
--rw-r--r--   0        0        0      468 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/default.yaml
--rw-r--r--   0        0        0       55 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/gpu.yaml
--rw-r--r--   0        0        0       56 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/configs/trainer/mps.yaml
--rw-r--r--   0        0        0      410 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/__init__.py
--rw-r--r--   0        0        0       31 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/__init__.py
--rw-r--r--   0        0        0      111 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/__init__.py
--rw-r--r--   0        0        0     5137 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/cyto_dl_base_model.py
--rw-r--r--   0        0        0     3766 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/segmentation_plugin_model.py
--rw-r--r--   0        0        0     1040 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/data.py
--rw-r--r--   0        0        0     4007 2024-05-03 16:17:29.112416 cyto-dl-0.1.6/cyto_dl/api/model.py
--rw-r--r--   0        0        0      265 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/__init__.py
--rw-r--r--   0        0        0     6605 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/callback_utils.py
--rw-r--r--   0        0        0    11849 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/latent_walk.py
--rw-r--r--   0        0        0     1918 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/layer_freeze.py
--rw-r--r--   0        0        0     4613 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/model_utils.py
--rw-r--r--   0        0        0     6687 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/callbacks/outlier_detection.py
--rw-r--r--   0        0        0     3846 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/compile.py
--rw-r--r--   0        0        0      238 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/__init__.py
--rw-r--r--   0        0        0     8481 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/readers.py
--rw-r--r--   0        0        0      251 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/__init__.py
--rw-r--r--   0        0        0     4519 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/filter.py
--rw-r--r--   0        0        0     2931 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/group_cols.py
--rw-r--r--   0        0        0     2441 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/misc.py
--rw-r--r--   0        0        0     3376 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/dataframe/transforms/split.py
--rw-r--r--   0        0        0       86 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/__init__.py
--rw-r--r--   0        0        0     8995 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/czi.py
--rw-r--r--   0        0        0     1837 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/data_dict.py
--rw-r--r--   0        0        0      123 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/__init__.py
--rw-r--r--   0        0        0     7500 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
--rw-r--r--   0        0        0     4856 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
--rw-r--r--   0        0        0    11941 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/utils.py
--rw-r--r--   0        0        0     2885 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/folder.py
--rw-r--r--   0        0        0     8030 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/smartcache.py
--rw-r--r--   0        0        0     2296 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/datamodules/torchvision.py
--rw-r--r--   0        0        0     3442 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/eval.py
--rw-r--r--   0        0        0      200 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/__init__.py
--rw-r--r--   0        0        0      213 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/__init__.py
--rw-r--r--   0        0        0     2621 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/aicsimage_loader.py
--rw-r--r--   0        0        0     1892 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/monai_bio_reader.py
--rw-r--r--   0        0        0     1707 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/numpy_reader.py
--rw-r--r--   0        0        0     1885 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/ome_zarr_reader.py
--rw-r--r--   0        0        0     2550 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/polygon_loader.py
--rw-r--r--   0        0        0     1498 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/io/skimage_reader.py
--rw-r--r--   0        0        0      624 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/bright_sampler.py
--rw-r--r--   0        0        0     2468 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/clip.py
--rw-r--r--   0        0        0     2247 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/contrastadjust.py
--rw-r--r--   0        0        0     2586 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/merge.py
--rw-r--r--   0        0        0     6376 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/multiscale_cropper.py
--rw-r--r--   0        0        0     2365 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/pad.py
--rw-r--r--   0        0        0     1355 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/project.py
--rw-r--r--   0        0        0     3460 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/rotation_mask_transform.py
--rw-r--r--   0        0        0     1855 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/save.py
--rw-r--r--   0        0        0     1418 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/so2_random_rotation.py
--rw-r--r--   0        0        0     4975 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/image/transforms/track_transforms.py
--rw-r--r--   0        0        0       33 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/loggers/__init__.py
--rw-r--r--   0        0        0     6183 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/loggers/mlflow.py
--rw-r--r--   0        0        0        0 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/__init__.py
--rw-r--r--   0        0        0     7267 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/base_model.py
--rw-r--r--   0        0        0     3298 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/basic_model.py
--rw-r--r--   0        0        0      105 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/__init__.py
--rw-r--r--   0        0        0     4448 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/classification.py
--rw-r--r--   0        0        0     3047 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/classification/timepoint_classification.py
--rw-r--r--   0        0        0       38 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/__init__.py
--rw-r--r--   0        0        0     2832 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/base_handler.py
--rw-r--r--   0        0        0     1133 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/image_handler.py
--rw-r--r--   0        0        0     1139 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/handlers/load_image_patch.py
--rw-r--r--   0        0        0       60 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/__init__.py
--rw-r--r--   0        0        0     6319 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/gan.py
--rw-r--r--   0        0        0     8946 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/multi_task.py
--rw-r--r--   0        0        0      324 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/__init__.py
--rw-r--r--   0        0        0    21568 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/instance_seg.py
--rw-r--r--   0        0        0     1531 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/noise_annealer.py
--rw-r--r--   0        0        0      125 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/__init__.py
--rw-r--r--   0        0        0     2410 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
--rw-r--r--   0        0        0      927 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
--rw-r--r--   0        0        0     1287 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
--rw-r--r--   0        0        0       32 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/__init__.py
--rw-r--r--   0        0        0     1264 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/mlflow.py
--rw-r--r--   0        0        0      268 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/utils/utils.py
--rw-r--r--   0        0        0      284 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/__init__.py
--rw-r--r--   0        0        0    10624 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/base_vae.py
--rw-r--r--   0        0        0    10648 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_canon_vae.py
--rw-r--r--   0        0        0    11242 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_encoder.py
--rw-r--r--   0        0        0     8223 2024-05-03 16:17:29.116416 cyto-dl-0.1.6/cyto_dl/models/vae/image_vae.py
--rw-r--r--   0        0        0     9890 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/latent_loss_vae.py
--rw-r--r--   0        0        0       39 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/__init__.py
--rw-r--r--   0        0        0     3653 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
--rw-r--r--   0        0        0     4323 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
--rw-r--r--   0        0        0    11244 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/point_cloud_vae.py
--rw-r--r--   0        0        0      144 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/__init__.py
--rw-r--r--   0        0        0      574 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/abstract_prior.py
--rw-r--r--   0        0        0     5530 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/gaussian.py
--rw-r--r--   0        0        0      408 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/identity_prior.py
--rw-r--r--   0        0        0     1609 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/priors/joint_prior.py
--rw-r--r--   0        0        0     1280 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/models/vae/tabular_vae.py
--rw-r--r--   0        0        0      305 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/__init__.py
--rw-r--r--   0        0        0      118 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/__init__.py
--rw-r--r--   0        0        0     1695 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/multi_scale_discriminator.py
--rw-r--r--   0        0        0     3816 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/discriminators/n_layer_discriminator.py
--rw-r--r--   0        0        0      183 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/__init__.py
--rw-r--r--   0        0        0     3796 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/base_head.py
--rw-r--r--   0        0        0     3115 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/gan_head.py
--rw-r--r--   0        0        0     2850 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/gan_head_superres.py
--rw-r--r--   0        0        0      928 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/mae_head.py
--rw-r--r--   0        0        0     1984 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/mask_head.py
--rw-r--r--   0        0        0     4415 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/head/res_blocks_head.py
--rw-r--r--   0        0        0     1042 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/hr_skip.py
--rw-r--r--   0        0        0      592 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/adversarial_loss.py
--rw-r--r--   0        0        0     1119 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/chamfer_loss.py
--rw-r--r--   0        0        0     1046 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/continuous_bernoulli.py
--rw-r--r--   0        0        0      671 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/cosine_loss.py
--rw-r--r--   0        0        0     4431 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/gan_loss.py
--rw-r--r--   0        0        0      917 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/gaussian_nll_loss.py
--rw-r--r--   0        0        0      873 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/geomloss.py
--rw-r--r--   0        0        0     2155 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/loss_wrapper.py
--rw-r--r--   0        0        0     1015 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/spharm_loss.py
--rw-r--r--   0        0        0      895 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/threshold_loss.py
--rw-r--r--   0        0        0     1105 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/weibull.py
--rw-r--r--   0        0        0      675 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/losses/weighted_mse_loss.py
--rw-r--r--   0        0        0      958 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/mlp.py
--rw-r--r--   0        0        0       61 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/__init__.py
--rw-r--r--   0        0        0    13372 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/dgcnn.py
--rw-r--r--   0        0        0     2732 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/folding_net.py
--rw-r--r--   0        0        0     4934 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/graph_functions.py
--rw-r--r--   0        0        0     5754 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/point_cloud/vnn.py
--rw-r--r--   0        0        0     6848 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/res_unit.py
--rw-r--r--   0        0        0     2555 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/spatial_transformer.py
--rw-r--r--   0        0        0     2571 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/track_sequence_predictor.py
--rw-r--r--   0        0        0      165 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/__init__.py
--rw-r--r--   0        0        0      171 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/__init__.py
--rw-r--r--   0        0        0     4427 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/cross_attention.py
--rw-r--r--   0        0        0      848 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/intermediate_weigher.py
--rw-r--r--   0        0        0     5249 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/patchify.py
--rw-r--r--   0        0        0     5577 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/cross_mae.py
--rw-r--r--   0        0        0    10645 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/mae.py
--rw-r--r--   0        0        0    10199 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/seg.py
--rw-r--r--   0        0        0      208 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/nn/vits/utils.py
--rw-r--r--   0        0        0        0 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/__init__.py
--rw-r--r--   0        0        0       40 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/io/__init__.py
--rw-r--r--   0        0        0     4992 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/point_cloud/io/read_pcloud.py
--rw-r--r--   0        0        0     5355 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/train.py
--rw-r--r--   0        0        0      333 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/__init__.py
--rw-r--r--   0        0        0     1791 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/config.py
--rw-r--r--   0        0        0     2391 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/download_test_data.py
--rw-r--r--   0        0        0     2359 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/dummy_dataset.py
--rw-r--r--   0        0        0      671 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/pylogger.py
--rw-r--r--   0        0        0     3326 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/rich_utils.py
--rw-r--r--   0        0        0     3808 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/rotation.py
--rw-r--r--   0        0        0      237 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/__init__.py
--rw-r--r--   0        0        0     6015 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/reconstruction.py
--rw-r--r--   0        0        0     4360 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/spharm/rotation.py
--rw-r--r--   0        0        0     7103 2024-05-03 16:17:29.120416 cyto-dl-0.1.6/cyto_dl/utils/template_utils.py
--rw-r--r--   0        0        0     2849 2024-05-03 16:17:29.124416 cyto-dl-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0       36 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/cyto_dl_model/bad_config.yaml
--rw-r--r--   0        0        0     5602 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/cyto_dl_model/test_segmentation_plugin_model.py
--rw-r--r--   0        0        0      929 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/api/test_model.py
--rw-r--r--   0        0        0     3599 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/__init__.py
--rw-r--r--   0        0        0      857 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/package_available.py
--rw-r--r--   0        0        0     4307 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/helpers/run_if.py
--rw-r--r--   0        0        0   259123 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/rand_im.tif
--rw-r--r--   0        0        0      336 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/test.csv
--rw-r--r--   0        0        0      635 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/train.csv
--rw-r--r--   0        0        0      336 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/resources/valid.csv
--rw-r--r--   0        0        0     2675 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_alternating_batch_sampler.py
--rw-r--r--   0        0        0     1434 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_configs.py
--rw-r--r--   0        0        0     1604 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_eval.py
--rw-r--r--   0        0        0     3730 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_mlflow_logger.py
--rw-r--r--   0        0        0     1119 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_polygon_loader.py
--rw-r--r--   0        0        0     2243 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/test_train.py
--rw-r--r--   0        0        0      143 2024-05-03 16:17:29.128416 cyto-dl-0.1.6/tests/utils.py
--rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     5431 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/README.md
+-rw-r--r--   0        0        0      403 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/default.yaml
+-rw-r--r--   0        0        0     1250 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/early_stopping.yaml
+-rw-r--r--   0        0        0       80 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/layer_freeze.yaml
+-rw-r--r--   0        0        0       83 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/learning_rate_monitor.yaml
+-rw-r--r--   0        0        0     1298 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/model_checkpoint.yaml
+-rw-r--r--   0        0        0      402 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/model_summary.yaml
+-rw-r--r--   0        0        0        0 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/none.yaml
+-rw-r--r--   0        0        0      160 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/outlier_detection.yaml
+-rw-r--r--   0        0        0      289 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/callbacks/rich_progress_bar.yaml
+-rw-r--r--   0        0        0      758 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/compile.yaml
+-rw-r--r--   0        0        0     2634 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     7077 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/gan.yaml
+-rw-r--r--   0        0        0     7427 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     6880 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     5879 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     4374 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/mae.yaml
+-rw-r--r--   0        0        0     6852 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     8053 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     7263 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0      450 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0      416 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/rot_mnist.yaml
+-rw-r--r--   0        0        0      450 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/rot_mnist_vae.yaml
+-rw-r--r--   0        0        0     1176 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/rotated_mnist.yaml
+-rw-r--r--   0        0        0     1075 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_3d.yaml
+-rw-r--r--   0        0        0      497 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_3d_npm1.yaml
+-rw-r--r--   0        0        0      770 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_3d_npm_nuc_v2.yaml
+-rw-r--r--   0        0        0     1802 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_3d_rotate.yaml
+-rw-r--r--   0        0        0      547 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_centerslice.yaml
+-rw-r--r--   0        0        0      719 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_centerslice_resize.yaml
+-rw-r--r--   0        0        0      969 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_npm1.yaml
+-rw-r--r--   0        0        0      312 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/private/variance_spharm.yaml
+-rw-r--r--   0        0        0      462 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/test/alternating_batch.yaml
+-rw-r--r--   0        0        0      200 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/test/omnipose.yaml
+-rw-r--r--   0        0        0      200 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/data/test/segmentation.yaml
+-rw-r--r--   0        0        0      899 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/debug/default.yaml
+-rw-r--r--   0        0        0      125 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/debug/fdr.yaml
+-rw-r--r--   0        0        0      223 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/debug/limit.yaml
+-rw-r--r--   0        0        0      209 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/debug/overfit.yaml
+-rw-r--r--   0        0        0      182 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/debug/profiler.yaml
+-rw-r--r--   0        0        0      509 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/eval.yaml
+-rw-r--r--   0        0        0      659 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/classification/per_timepoint.yaml
+-rw-r--r--   0        0        0     1065 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/gan.yaml
+-rw-r--r--   0        0        0     1083 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0      932 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0      854 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/labelfree.yaml
+-rw-r--r--   0        0        0      892 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/mae.yaml
+-rw-r--r--   0        0        0      863 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1622 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0      881 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1098 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/im2im/vit_segmentation.yaml
+-rw-r--r--   0        0        0     2741 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/lattice_nuc_sdf.yaml
+-rw-r--r--   0        0        0     1583 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/mnist_so2.yaml
+-rw-r--r--   0        0        0      989 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     2902 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_classical_scale_inv.yaml
+-rw-r--r--   0        0        0     1037 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml
+-rw-r--r--   0        0        0     2825 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_scale_inv_canon_so3.yaml
+-rw-r--r--   0        0        0     2568 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_so2.yaml
+-rw-r--r--   0        0        0     3062 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_so2_scale_inv.yaml
+-rw-r--r--   0        0        0     3057 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_so3_scale_inv.yaml
+-rw-r--r--   0        0        0     2325 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_so3_vae.yaml
+-rw-r--r--   0        0        0     2179 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/npm1_so3_vae_seg.yaml
+-rw-r--r--   0        0        0      967 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_classical_2d_vae.yaml
+-rw-r--r--   0        0        0     1053 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_classical_3d_vae.yaml
+-rw-r--r--   0        0        0     1385 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_so2_3d_vae.yaml
+-rw-r--r--   0        0        0     1605 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_so2_3d_vae_profiling.yaml
+-rw-r--r--   0        0        0     9822 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_spharm.yaml
+-rw-r--r--   0        0        0     9728 2024-05-08 22:29:50.466922 cyto-dl-0.1.7/configs/experiment/private/variance_spharm_o2.yaml
+-rw-r--r--   0        0        0      309 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/extras/default.yaml
+-rw-r--r--   0        0        0     1818 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/hparams_search/mnist_optuna.yaml
+-rw-r--r--   0        0        0      431 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/hydra/default.yaml
+-rw-r--r--   0        0        0      372 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/comet.yaml
+-rw-r--r--   0        0        0      157 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/csv.yaml
+-rw-r--r--   0        0        0      148 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/many_loggers.yaml
+-rw-r--r--   0        0        0      166 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/mlflow.yaml
+-rw-r--r--   0        0        0      277 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/neptune.yaml
+-rw-r--r--   0        0        0      258 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/tensorboard.yaml
+-rw-r--r--   0        0        0      522 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/logger/wandb.yaml
+-rw-r--r--   0        0        0      594 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/classification/single_timepoint.yaml
+-rw-r--r--   0        0        0     1807 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/gan.yaml
+-rw-r--r--   0        0        0     1948 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/gan_superres.yaml
+-rw-r--r--   0        0        0     1333 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/instance_seg.yaml
+-rw-r--r--   0        0        0     1237 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/labelfree.yaml
+-rw-r--r--   0        0        0     1245 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/mae.yaml
+-rw-r--r--   0        0        0     1333 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/segmentation.yaml
+-rw-r--r--   0        0        0     1252 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/segmentation_plugin.yaml
+-rw-r--r--   0        0        0     1472 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/segmentation_superres.yaml
+-rw-r--r--   0        0        0     1365 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/im2im/vit_segmentation_decoder.yaml
+-rw-r--r--   0        0        0      493 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/classical_image_ae.yaml
+-rw-r--r--   0        0        0      536 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/classical_image_vae.yaml
+-rw-r--r--   0        0        0       86 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/reconstruction_loss/spharm_gaussian.yaml
+-rw-r--r--   0        0        0       76 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/reconstruction_loss/spharm_loss.yaml
+-rw-r--r--   0        0        0       56 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/reconstruction_loss/spharm_mse.yaml
+-rw-r--r--   0        0        0       93 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/reconstruction_loss/spharm_weighted_mse.yaml
+-rw-r--r--   0        0        0      316 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/so3_canon_image_vae.yaml
+-rw-r--r--   0        0        0      332 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/so3_equiv_image_vae.yaml
+-rw-r--r--   0        0        0      513 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/spharm.yaml
+-rw-r--r--   0        0        0      501 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/private/spharm_so2.yaml
+-rw-r--r--   0        0        0      597 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/test/base.yaml
+-rw-r--r--   0        0        0      613 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/model/test/simple_segmentation.yaml
+-rw-r--r--   0        0        0      492 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/paths/default.yaml
+-rw-r--r--   0        0        0     1745 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/train.yaml
+-rw-r--r--   0        0        0       56 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/cpu.yaml
+-rw-r--r--   0        0        0      394 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/ddp.yaml
+-rw-r--r--   0        0        0      120 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/ddp_sim.yaml
+-rw-r--r--   0        0        0      468 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/default.yaml
+-rw-r--r--   0        0        0       55 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/gpu.yaml
+-rw-r--r--   0        0        0       56 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/configs/trainer/mps.yaml
+-rw-r--r--   0        0        0      410 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/cyto_dl_model/__init__.py
+-rw-r--r--   0        0        0     5137 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/cyto_dl_model/cyto_dl_base_model.py
+-rw-r--r--   0        0        0     3766 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/cyto_dl_model/segmentation_plugin_model.py
+-rw-r--r--   0        0        0     1040 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/data.py
+-rw-r--r--   0        0        0     4113 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/api/model.py
+-rw-r--r--   0        0        0      265 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/__init__.py
+-rw-r--r--   0        0        0     6605 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/callback_utils.py
+-rw-r--r--   0        0        0    11849 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/latent_walk.py
+-rw-r--r--   0        0        0     1918 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/layer_freeze.py
+-rw-r--r--   0        0        0     4613 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/model_utils.py
+-rw-r--r--   0        0        0     6687 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/callbacks/outlier_detection.py
+-rw-r--r--   0        0        0     3846 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/compile.py
+-rw-r--r--   0        0        0      238 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/__init__.py
+-rw-r--r--   0        0        0     8481 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/readers.py
+-rw-r--r--   0        0        0      251 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/transforms/__init__.py
+-rw-r--r--   0        0        0     4519 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/transforms/filter.py
+-rw-r--r--   0        0        0     2931 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/transforms/group_cols.py
+-rw-r--r--   0        0        0     2441 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/transforms/misc.py
+-rw-r--r--   0        0        0     3376 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/dataframe/transforms/split.py
+-rw-r--r--   0        0        0       86 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/__init__.py
+-rw-r--r--   0        0        0     8995 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/czi.py
+-rw-r--r--   0        0        0     1837 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/data_dict.py
+-rw-r--r--   0        0        0      123 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/__init__.py
+-rw-r--r--   0        0        0     7500 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/dataframe_datamodule.py
+-rw-r--r--   0        0        0     4856 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py
+-rw-r--r--   0        0        0    11941 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/utils.py
+-rw-r--r--   0        0        0     2885 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/folder.py
+-rw-r--r--   0        0        0     8030 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/smartcache.py
+-rw-r--r--   0        0        0     2296 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/datamodules/torchvision.py
+-rw-r--r--   0        0        0     3442 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/eval.py
+-rw-r--r--   0        0        0      200 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/image/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/image/io/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/image/io/aicsimage_loader.py
+-rw-r--r--   0        0        0     1892 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/image/io/monai_bio_reader.py
+-rw-r--r--   0        0        0     1707 2024-05-08 22:29:50.470922 cyto-dl-0.1.7/cyto_dl/image/io/numpy_reader.py
+-rw-r--r--   0        0        0     1885 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/io/ome_zarr_reader.py
+-rw-r--r--   0        0        0     2550 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/io/polygon_loader.py
+-rw-r--r--   0        0        0     1498 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/io/skimage_reader.py
+-rw-r--r--   0        0        0      624 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/bright_sampler.py
+-rw-r--r--   0        0        0     2468 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/clip.py
+-rw-r--r--   0        0        0     2247 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/contrastadjust.py
+-rw-r--r--   0        0        0     2586 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/merge.py
+-rw-r--r--   0        0        0     6376 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/multiscale_cropper.py
+-rw-r--r--   0        0        0     2365 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/pad.py
+-rw-r--r--   0        0        0     1355 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/project.py
+-rw-r--r--   0        0        0     3460 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/rotation_mask_transform.py
+-rw-r--r--   0        0        0     1855 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/save.py
+-rw-r--r--   0        0        0     1418 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/so2_random_rotation.py
+-rw-r--r--   0        0        0     4975 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/image/transforms/track_transforms.py
+-rw-r--r--   0        0        0       33 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/loggers/__init__.py
+-rw-r--r--   0        0        0     6183 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/loggers/mlflow.py
+-rw-r--r--   0        0        0        0 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/__init__.py
+-rw-r--r--   0        0        0     7267 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/base_model.py
+-rw-r--r--   0        0        0     3298 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/basic_model.py
+-rw-r--r--   0        0        0      105 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/classification/__init__.py
+-rw-r--r--   0        0        0     4448 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/classification/classification.py
+-rw-r--r--   0        0        0     3047 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/classification/timepoint_classification.py
+-rw-r--r--   0        0        0       38 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/handlers/__init__.py
+-rw-r--r--   0        0        0     2832 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/handlers/base_handler.py
+-rw-r--r--   0        0        0     1133 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/handlers/image_handler.py
+-rw-r--r--   0        0        0     1139 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/handlers/load_image_patch.py
+-rw-r--r--   0        0        0       60 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/__init__.py
+-rw-r--r--   0        0        0     6319 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/gan.py
+-rw-r--r--   0        0        0     8946 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/multi_task.py
+-rw-r--r--   0        0        0      324 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/__init__.py
+-rw-r--r--   0        0        0    21568 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/instance_seg.py
+-rw-r--r--   0        0        0     1531 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/noise_annealer.py
+-rw-r--r--   0        0        0      125 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/__init__.py
+-rw-r--r--   0        0        0     2410 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py
+-rw-r--r--   0        0        0      927 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py
+-rw-r--r--   0        0        0     1287 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py
+-rw-r--r--   0        0        0       32 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/utils/__init__.py
+-rw-r--r--   0        0        0     1264 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/utils/mlflow.py
+-rw-r--r--   0        0        0      268 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/utils/utils.py
+-rw-r--r--   0        0        0      284 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/__init__.py
+-rw-r--r--   0        0        0    10624 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/base_vae.py
+-rw-r--r--   0        0        0    10648 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/image_canon_vae.py
+-rw-r--r--   0        0        0    11242 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/image_encoder.py
+-rw-r--r--   0        0        0     8223 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/image_vae.py
+-rw-r--r--   0        0        0     9890 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/latent_loss_vae.py
+-rw-r--r--   0        0        0       39 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/o2_spharm_vae/__init__.py
+-rw-r--r--   0        0        0     3653 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py
+-rw-r--r--   0        0        0     4323 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py
+-rw-r--r--   0        0        0    11244 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/point_cloud_vae.py
+-rw-r--r--   0        0        0      144 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/priors/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/priors/abstract_prior.py
+-rw-r--r--   0        0        0     5530 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/priors/gaussian.py
+-rw-r--r--   0        0        0      408 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/priors/identity_prior.py
+-rw-r--r--   0        0        0     1609 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/priors/joint_prior.py
+-rw-r--r--   0        0        0     1280 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/models/vae/tabular_vae.py
+-rw-r--r--   0        0        0      305 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/__init__.py
+-rw-r--r--   0        0        0      118 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/discriminators/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/discriminators/multi_scale_discriminator.py
+-rw-r--r--   0        0        0     3816 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/discriminators/n_layer_discriminator.py
+-rw-r--r--   0        0        0      183 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/__init__.py
+-rw-r--r--   0        0        0     3796 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/base_head.py
+-rw-r--r--   0        0        0     3115 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/gan_head.py
+-rw-r--r--   0        0        0     2850 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/gan_head_superres.py
+-rw-r--r--   0        0        0      928 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/mae_head.py
+-rw-r--r--   0        0        0     1984 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/mask_head.py
+-rw-r--r--   0        0        0     4415 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/head/res_blocks_head.py
+-rw-r--r--   0        0        0     1042 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/hr_skip.py
+-rw-r--r--   0        0        0      592 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/adversarial_loss.py
+-rw-r--r--   0        0        0     1119 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/chamfer_loss.py
+-rw-r--r--   0        0        0     1046 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/continuous_bernoulli.py
+-rw-r--r--   0        0        0      671 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/cosine_loss.py
+-rw-r--r--   0        0        0     4431 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/gan_loss.py
+-rw-r--r--   0        0        0      917 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/gaussian_nll_loss.py
+-rw-r--r--   0        0        0      873 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/geomloss.py
+-rw-r--r--   0        0        0     2155 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/loss_wrapper.py
+-rw-r--r--   0        0        0     1015 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/spharm_loss.py
+-rw-r--r--   0        0        0      895 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/threshold_loss.py
+-rw-r--r--   0        0        0     1105 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/weibull.py
+-rw-r--r--   0        0        0      675 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/losses/weighted_mse_loss.py
+-rw-r--r--   0        0        0      958 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/mlp.py
+-rw-r--r--   0        0        0       61 2024-05-08 22:29:50.474922 cyto-dl-0.1.7/cyto_dl/nn/point_cloud/__init__.py
+-rw-r--r--   0        0        0    13372 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/point_cloud/dgcnn.py
+-rw-r--r--   0        0        0     2732 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/point_cloud/folding_net.py
+-rw-r--r--   0        0        0     4934 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/point_cloud/graph_functions.py
+-rw-r--r--   0        0        0     5754 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/point_cloud/vnn.py
+-rw-r--r--   0        0        0     6848 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/res_unit.py
+-rw-r--r--   0        0        0     2555 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/spatial_transformer.py
+-rw-r--r--   0        0        0     2571 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/track_sequence_predictor.py
+-rw-r--r--   0        0        0      165 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/__init__.py
+-rw-r--r--   0        0        0     4427 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/cross_attention.py
+-rw-r--r--   0        0        0      848 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/intermediate_weigher.py
+-rw-r--r--   0        0        0     5249 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/patchify.py
+-rw-r--r--   0        0        0     5577 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/cross_mae.py
+-rw-r--r--   0        0        0    10645 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/mae.py
+-rw-r--r--   0        0        0    10199 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/seg.py
+-rw-r--r--   0        0        0      208 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/nn/vits/utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/point_cloud/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/point_cloud/io/__init__.py
+-rw-r--r--   0        0        0     4992 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/point_cloud/io/read_pcloud.py
+-rw-r--r--   0        0        0     5355 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/train.py
+-rw-r--r--   0        0        0      333 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/__init__.py
+-rw-r--r--   0        0        0     1791 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/config.py
+-rw-r--r--   0        0        0     2391 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/download_test_data.py
+-rw-r--r--   0        0        0     2359 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/dummy_dataset.py
+-rw-r--r--   0        0        0      671 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/pylogger.py
+-rw-r--r--   0        0        0     3326 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/rich_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/rotation.py
+-rw-r--r--   0        0        0      237 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/spharm/__init__.py
+-rw-r--r--   0        0        0     6015 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/spharm/reconstruction.py
+-rw-r--r--   0        0        0     4360 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/spharm/rotation.py
+-rw-r--r--   0        0        0     7103 2024-05-08 22:29:50.478922 cyto-dl-0.1.7/cyto_dl/utils/template_utils.py
+-rw-r--r--   0        0        0     2856 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0       36 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/api/cyto_dl_model/bad_config.yaml
+-rw-r--r--   0        0        0     5602 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/api/cyto_dl_model/test_segmentation_plugin_model.py
+-rw-r--r--   0        0        0      933 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/api/test_model.py
+-rw-r--r--   0        0        0     3599 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/helpers/package_available.py
+-rw-r--r--   0        0        0     4307 2024-05-08 22:29:50.482922 cyto-dl-0.1.7/tests/helpers/run_if.py
+-rw-r--r--   0        0        0   259123 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/resources/rand_im.tif
+-rw-r--r--   0        0        0      336 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/resources/test.csv
+-rw-r--r--   0        0        0      635 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/resources/train.csv
+-rw-r--r--   0        0        0      336 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/resources/valid.csv
+-rw-r--r--   0        0        0     2675 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_alternating_batch_sampler.py
+-rw-r--r--   0        0        0     1434 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_configs.py
+-rw-r--r--   0        0        0     1604 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_eval.py
+-rw-r--r--   0        0        0     3730 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_mlflow_logger.py
+-rw-r--r--   0        0        0     1119 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_polygon_loader.py
+-rw-r--r--   0        0        0     2243 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/test_train.py
+-rw-r--r--   0        0        0      143 2024-05-08 22:29:50.486922 cyto-dl-0.1.7/tests/utils.py
+-rw-r--r--   0        0        0     6142 1970-01-01 00:00:00.000000 cyto-dl-0.1.7/PKG-INFO
```

### Comparing `cyto-dl-0.1.6/README.md` & `cyto-dl-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/callbacks/early_stopping.yaml` & `cyto-dl-0.1.7/configs/callbacks/early_stopping.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/callbacks/model_checkpoint.yaml` & `cyto-dl-0.1.7/configs/callbacks/model_checkpoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/compile.yaml` & `cyto-dl-0.1.7/configs/compile.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/classification/single_timepoint.yaml` & `cyto-dl-0.1.7/configs/data/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/gan.yaml` & `cyto-dl-0.1.7/configs/data/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/gan_superres.yaml` & `cyto-dl-0.1.7/configs/data/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/instance_seg.yaml` & `cyto-dl-0.1.7/configs/data/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/labelfree.yaml` & `cyto-dl-0.1.7/configs/data/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/mae.yaml` & `cyto-dl-0.1.7/configs/data/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/segmentation.yaml` & `cyto-dl-0.1.7/configs/data/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.7/configs/data/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.7/configs/data/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/rotated_mnist.yaml` & `cyto-dl-0.1.7/configs/data/private/rotated_mnist.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_3d.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_3d.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_3d_npm_nuc_v2.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_3d_npm_nuc_v2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_3d_rotate.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_3d_rotate.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_centerslice.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_centerslice.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_centerslice_resize.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_centerslice_resize.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/data/private/variance_npm1.yaml` & `cyto-dl-0.1.7/configs/data/private/variance_npm1.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/debug/default.yaml` & `cyto-dl-0.1.7/configs/debug/default.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/classification/per_timepoint.yaml` & `cyto-dl-0.1.7/configs/experiment/classification/per_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/gan.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/gan_superres.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/instance_seg.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/labelfree.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/mae.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/segmentation.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/im2im/vit_segmentation.yaml` & `cyto-dl-0.1.7/configs/experiment/im2im/vit_segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/lattice_nuc_sdf.yaml` & `cyto-dl-0.1.7/configs/experiment/private/lattice_nuc_sdf.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/mnist_so2.yaml` & `cyto-dl-0.1.7/configs/experiment/private/mnist_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_classical_3d_vae.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_classical_scale_inv.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_classical_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_equiv_3d_vae_3dnucalign.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_scale_inv_canon_so3.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_scale_inv_canon_so3.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_so2.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_so2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_so2_scale_inv.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_so2_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_scale_inv.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_so3_scale_inv.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_so3_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/npm1_so3_vae_seg.yaml` & `cyto-dl-0.1.7/configs/experiment/private/npm1_so3_vae_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_classical_2d_vae.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_classical_2d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_classical_3d_vae.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_classical_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_so2_3d_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_so2_3d_vae_profiling.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_so2_3d_vae_profiling.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_spharm.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/experiment/private/variance_spharm_o2.yaml` & `cyto-dl-0.1.7/configs/experiment/private/variance_spharm_o2.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/hparams_search/mnist_optuna.yaml` & `cyto-dl-0.1.7/configs/hparams_search/mnist_optuna.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/logger/wandb.yaml` & `cyto-dl-0.1.7/configs/logger/wandb.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/classification/single_timepoint.yaml` & `cyto-dl-0.1.7/configs/model/classification/single_timepoint.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/gan.yaml` & `cyto-dl-0.1.7/configs/model/im2im/gan.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/gan_superres.yaml` & `cyto-dl-0.1.7/configs/model/im2im/gan_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/instance_seg.yaml` & `cyto-dl-0.1.7/configs/model/im2im/instance_seg.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/labelfree.yaml` & `cyto-dl-0.1.7/configs/model/im2im/labelfree.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/mae.yaml` & `cyto-dl-0.1.7/configs/model/im2im/mae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/segmentation.yaml` & `cyto-dl-0.1.7/configs/model/im2im/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/segmentation_plugin.yaml` & `cyto-dl-0.1.7/configs/model/im2im/segmentation_plugin.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/segmentation_superres.yaml` & `cyto-dl-0.1.7/configs/model/im2im/segmentation_superres.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/im2im/vit_segmentation_decoder.yaml` & `cyto-dl-0.1.7/configs/model/im2im/vit_segmentation_decoder.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/private/classical_image_vae.yaml` & `cyto-dl-0.1.7/configs/model/private/classical_image_vae.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/private/spharm.yaml` & `cyto-dl-0.1.7/configs/model/private/spharm.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/test/base.yaml` & `cyto-dl-0.1.7/configs/model/test/base.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/model/test/simple_segmentation.yaml` & `cyto-dl-0.1.7/configs/model/test/simple_segmentation.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/configs/train.yaml` & `cyto-dl-0.1.7/configs/train.yaml`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/cyto_dl_base_model.py` & `cyto-dl-0.1.7/cyto_dl/api/cyto_dl_model/cyto_dl_base_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/api/cyto_dl_model/segmentation_plugin_model.py` & `cyto-dl-0.1.7/cyto_dl/api/cyto_dl_model/segmentation_plugin_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/api/data.py` & `cyto-dl-0.1.7/cyto_dl/api/data.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/api/model.py` & `cyto-dl-0.1.7/cyto_dl/api/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,27 +71,33 @@
             cfg["paths"]["output_dir"] = output_dir
             cfg["paths"]["work_dir"] = output_dir
 
         output_dir = Path(output_dir)
         output_dir.mkdir(parents=True, exist_ok=True)
 
         self.cfg = cfg
-        OmegaConf.save(self.cfg, output_dir / f'{"train" if train else "eval"}_config.yaml')
 
     def print_config(self):
         print_config_tree(self.cfg, resolve=True)
 
     def override_config(self, overrides: Dict[str, Union[str, int, float, bool]]):
         """Override configuration from list of overrides."""
         if self.cfg is None:
             raise ValueError("Configuration must be loaded before overriding!")
 
         for k, v in overrides.items():
             OmegaConf.update(self.cfg, k, v)
 
+    def save_config(self, path: Path) -> None:
+        """Save current config to provided path.
+
+        :param path: path at which to save config
+        """
+        OmegaConf.save(self.cfg, path)
+
     async def _train_async(self):
         return train_model(self.cfg)
 
     async def _predict_async(self):
         return evaluate(self.cfg)
 
     def train(self, run_async=False):
```

### Comparing `cyto-dl-0.1.6/cyto_dl/callbacks/callback_utils.py` & `cyto-dl-0.1.7/cyto_dl/callbacks/callback_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/callbacks/latent_walk.py` & `cyto-dl-0.1.7/cyto_dl/callbacks/latent_walk.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/callbacks/layer_freeze.py` & `cyto-dl-0.1.7/cyto_dl/callbacks/layer_freeze.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/callbacks/model_utils.py` & `cyto-dl-0.1.7/cyto_dl/callbacks/model_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/callbacks/outlier_detection.py` & `cyto-dl-0.1.7/cyto_dl/callbacks/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/compile.py` & `cyto-dl-0.1.7/cyto_dl/compile.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/dataframe/readers.py` & `cyto-dl-0.1.7/cyto_dl/dataframe/readers.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/filter.py` & `cyto-dl-0.1.7/cyto_dl/dataframe/transforms/filter.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/group_cols.py` & `cyto-dl-0.1.7/cyto_dl/dataframe/transforms/group_cols.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/misc.py` & `cyto-dl-0.1.7/cyto_dl/dataframe/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/dataframe/transforms/split.py` & `cyto-dl-0.1.7/cyto_dl/dataframe/transforms/split.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/czi.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/czi.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/data_dict.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/data_dict.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/dataframe_datamodule.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/dataframe_datamodule.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/grouped_dataframe_datamodule.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/dataframe/utils.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/folder.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/folder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/smartcache.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/smartcache.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/datamodules/torchvision.py` & `cyto-dl-0.1.7/cyto_dl/datamodules/torchvision.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/eval.py` & `cyto-dl-0.1.7/cyto_dl/eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/aicsimage_loader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/aicsimage_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/monai_bio_reader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/monai_bio_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/numpy_reader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/numpy_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/ome_zarr_reader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/ome_zarr_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/polygon_loader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/polygon_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/io/skimage_reader.py` & `cyto-dl-0.1.7/cyto_dl/image/io/skimage_reader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/__init__.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/bright_sampler.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/bright_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/clip.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/clip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/contrastadjust.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/contrastadjust.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/merge.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/merge.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/multiscale_cropper.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/multiscale_cropper.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/pad.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/pad.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/project.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/project.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/rotation_mask_transform.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/rotation_mask_transform.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/save.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/save.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/so2_random_rotation.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/so2_random_rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/image/transforms/track_transforms.py` & `cyto-dl-0.1.7/cyto_dl/image/transforms/track_transforms.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/loggers/mlflow.py` & `cyto-dl-0.1.7/cyto_dl/loggers/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/base_model.py` & `cyto-dl-0.1.7/cyto_dl/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/basic_model.py` & `cyto-dl-0.1.7/cyto_dl/models/basic_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/classification/classification.py` & `cyto-dl-0.1.7/cyto_dl/models/classification/classification.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/classification/timepoint_classification.py` & `cyto-dl-0.1.7/cyto_dl/models/classification/timepoint_classification.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/handlers/base_handler.py` & `cyto-dl-0.1.7/cyto_dl/models/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/handlers/image_handler.py` & `cyto-dl-0.1.7/cyto_dl/models/handlers/image_handler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/handlers/load_image_patch.py` & `cyto-dl-0.1.7/cyto_dl/models/handlers/load_image_patch.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/gan.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/gan.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/multi_task.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/multi_task.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/instance_seg.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/utils/instance_seg.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/noise_annealer.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/utils/noise_annealer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/act_thresh_label.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/auto_thresh.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py` & `cyto-dl-0.1.7/cyto_dl/models/im2im/utils/postprocessing/dict_to_im.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/utils/mlflow.py` & `cyto-dl-0.1.7/cyto_dl/models/utils/mlflow.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/base_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/base_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/image_canon_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/image_canon_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/image_encoder.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/image_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/image_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/image_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/latent_loss_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/latent_loss_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_encoder.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/o2_spharm_vae/o2_spharm_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/point_cloud_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/point_cloud_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/priors/abstract_prior.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/priors/abstract_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/priors/gaussian.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/priors/gaussian.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/priors/joint_prior.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/priors/joint_prior.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/models/vae/tabular_vae.py` & `cyto-dl-0.1.7/cyto_dl/models/vae/tabular_vae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/discriminators/multi_scale_discriminator.py` & `cyto-dl-0.1.7/cyto_dl/nn/discriminators/multi_scale_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/discriminators/n_layer_discriminator.py` & `cyto-dl-0.1.7/cyto_dl/nn/discriminators/n_layer_discriminator.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/base_head.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/base_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/gan_head.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/gan_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/gan_head_superres.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/gan_head_superres.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/mae_head.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/mae_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/mask_head.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/mask_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/head/res_blocks_head.py` & `cyto-dl-0.1.7/cyto_dl/nn/head/res_blocks_head.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/hr_skip.py` & `cyto-dl-0.1.7/cyto_dl/nn/hr_skip.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/__init__.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/adversarial_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/adversarial_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/chamfer_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/chamfer_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/continuous_bernoulli.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/continuous_bernoulli.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/cosine_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/cosine_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/gan_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/gan_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/gaussian_nll_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/gaussian_nll_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/geomloss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/geomloss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/loss_wrapper.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/loss_wrapper.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/spharm_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/spharm_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/threshold_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/threshold_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/weibull.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/weibull.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/losses/weighted_mse_loss.py` & `cyto-dl-0.1.7/cyto_dl/nn/losses/weighted_mse_loss.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/mlp.py` & `cyto-dl-0.1.7/cyto_dl/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/dgcnn.py` & `cyto-dl-0.1.7/cyto_dl/nn/point_cloud/dgcnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/folding_net.py` & `cyto-dl-0.1.7/cyto_dl/nn/point_cloud/folding_net.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/graph_functions.py` & `cyto-dl-0.1.7/cyto_dl/nn/point_cloud/graph_functions.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/point_cloud/vnn.py` & `cyto-dl-0.1.7/cyto_dl/nn/point_cloud/vnn.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/res_unit.py` & `cyto-dl-0.1.7/cyto_dl/nn/res_unit.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/spatial_transformer.py` & `cyto-dl-0.1.7/cyto_dl/nn/spatial_transformer.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/track_sequence_predictor.py` & `cyto-dl-0.1.7/cyto_dl/nn/track_sequence_predictor.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/cross_attention.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/cross_attention.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/intermediate_weigher.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/intermediate_weigher.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/blocks/patchify.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/blocks/patchify.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/cross_mae.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/cross_mae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/mae.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/mae.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/nn/vits/seg.py` & `cyto-dl-0.1.7/cyto_dl/nn/vits/seg.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/point_cloud/io/read_pcloud.py` & `cyto-dl-0.1.7/cyto_dl/point_cloud/io/read_pcloud.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/train.py` & `cyto-dl-0.1.7/cyto_dl/train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/config.py` & `cyto-dl-0.1.7/cyto_dl/utils/config.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/download_test_data.py` & `cyto-dl-0.1.7/cyto_dl/utils/download_test_data.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/dummy_dataset.py` & `cyto-dl-0.1.7/cyto_dl/utils/dummy_dataset.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/pylogger.py` & `cyto-dl-0.1.7/cyto_dl/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/rich_utils.py` & `cyto-dl-0.1.7/cyto_dl/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/rotation.py` & `cyto-dl-0.1.7/cyto_dl/utils/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/spharm/reconstruction.py` & `cyto-dl-0.1.7/cyto_dl/utils/spharm/reconstruction.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/spharm/rotation.py` & `cyto-dl-0.1.7/cyto_dl/utils/spharm/rotation.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/cyto_dl/utils/template_utils.py` & `cyto-dl-0.1.7/cyto_dl/utils/template_utils.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/pyproject.toml` & `cyto-dl-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "pdm-pep517>=1.0.0",
     "numpy>=1.23.5",
 ]
 build-backend = "pdm.pep517.api"
 
 [project]
 name = "cyto-dl"
-version = "0.1.6"
+version = "0.1.7"
 description = "Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization."
 readme = "README.md"
 authors = [
     { name = "Benji Morris", email = "benjamin.morris@alleninstitute.org" },
     { name = "Guilherme Pires", email = "guilherme.pires@alleninstitute.org" },
     { name = "Ritvik Vasan", email = "ritvik.vasan@alleninstitute.org" },
 ]
@@ -38,15 +38,15 @@
     "tqdm>=4.64",
     "lightning>=2.0",
     "einops>=0.6.1",
     "edt>=2.3.1",
     "astropy>=5.2",
     "rich",
     "boto3",
-    "bioio",
+    "bioio>=1.0.1",
     "bioio-czi",
     "bioio-ome-tiff",
     "bioio-tifffile",
 ]
 requires-python = ">=3.9,<3.11"
 
 [project.optional-dependencies]
```

### Comparing `cyto-dl-0.1.6/tests/api/cyto_dl_model/test_segmentation_plugin_model.py` & `cyto-dl-0.1.7/tests/api/cyto_dl_model/test_segmentation_plugin_model.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/api/test_model.py` & `cyto-dl-0.1.7/tests/api/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # mock these functions to avoid attempts to write to file system
 @patch("cyto_dl.api.model.OmegaConf.save")
 @patch("cyto_dl.api.model.Path.mkdir")
 def test_load_default_experiment_valid_exp_type(MockMkdir, MockSave):
     model: CytoDLModel = CytoDLModel()
     model.load_default_experiment(ExperimentType.SEGMENTATION.value, "fake_dir")
     MockMkdir.assert_called()
-    MockSave.assert_called()
+    MockSave.assert_not_called()
 
 
 @patch("cyto_dl.api.model.OmegaConf.save")
 @patch("cyto_dl.api.model.Path.mkdir")
 def test_load_default_experiment_invalid_exp_type(MockMkdir, MockSave):
     model: CytoDLModel = CytoDLModel()
     with pytest.raises(AssertionError):
```

### Comparing `cyto-dl-0.1.6/tests/conftest.py` & `cyto-dl-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/helpers/package_available.py` & `cyto-dl-0.1.7/tests/helpers/package_available.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/helpers/run_if.py` & `cyto-dl-0.1.7/tests/helpers/run_if.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/resources/rand_im.tif` & `cyto-dl-0.1.7/tests/resources/rand_im.tif`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/resources/train.csv` & `cyto-dl-0.1.7/tests/resources/train.csv`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_alternating_batch_sampler.py` & `cyto-dl-0.1.7/tests/test_alternating_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_configs.py` & `cyto-dl-0.1.7/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_eval.py` & `cyto-dl-0.1.7/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_mlflow_logger.py` & `cyto-dl-0.1.7/tests/test_mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_polygon_loader.py` & `cyto-dl-0.1.7/tests/test_polygon_loader.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/tests/test_train.py` & `cyto-dl-0.1.7/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `cyto-dl-0.1.6/PKG-INFO` & `cyto-dl-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyto-dl
-Version: 0.1.6
+Version: 0.1.7
 Summary: Collection of representation learning models, techniques, callbacks, utils, used to create latent variable models of cell shape, morphology and intracellular organization.
 Author-email: Benji Morris <benjamin.morris@alleninstitute.org>,Guilherme Pires <guilherme.pires@alleninstitute.org>,Ritvik Vasan <ritvik.vasan@alleninstitute.org>
 Requires-Python: >=3.9,<3.11
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: equiv
 Provides-Extra: pcloud
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.6 Summary: Collection of
+Metadata-Version: 2.1 Name: cyto-dl Version: 0.1.7 Summary: Collection of
 representation learning models, techniques, callbacks, utils, used to create
 latent variable models of cell shape, morphology and intracellular
 organization. Author-email: Benji Morris
 alleninstitute.org>,Guilherme Pires
 alleninstitute.org>,Ritvik Vasan
 alleninstitute.org> Requires-Python: >=3.9,<3.11 Provides-Extra: all Provides-
 Extra: docs Provides-Extra: equiv Provides-Extra: pcloud Provides-Extra: s3
```

