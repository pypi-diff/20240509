# Comparing `tmp/zhousf-lib-1.5.5.tar.gz` & `tmp/zhousf-lib-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhousf-lib-1.5.5.tar", last modified: Thu Apr 25 02:34:14 2024, max compression
+gzip compressed data, was "zhousf-lib-1.5.6.tar", last modified: Thu May  9 02:54:12 2024, max compression
```

## Comparing `zhousf-lib-1.5.5.tar` & `zhousf-lib-1.5.6.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.771865 zhousf-lib-1.5.5/
--rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/LICENSE
--rw-rw-rw-   0        0        0     3232 2024-04-25 02:34:14.770864 zhousf-lib-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-25 02:34:14.772864 zhousf-lib-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     4535 2024-04-25 02:34:11.000000 zhousf-lib-1.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.577942 zhousf-lib-1.5.5/zhousf_lib.egg-info/
--rw-rw-rw-   0        0        0     3232 2024-04-25 02:34:14.000000 zhousf-lib-1.5.5/zhousf_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3912 2024-04-25 02:34:14.000000 zhousf-lib-1.5.5/zhousf_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:34:14.000000 zhousf-lib-1.5.5/zhousf_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-25 02:34:14.000000 zhousf-lib-1.5.5/zhousf_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.579943 zhousf-lib-1.5.5/zhousflib/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.580942 zhousf-lib-1.5.5/zhousflib/ann/
--rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.583943 zhousf-lib-1.5.5/zhousflib/ann/onnx/
--rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.5/zhousflib/ann/onnx/__init__.py
--rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/onnx/onnx_to_trt.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.587005 zhousf-lib-1.5.5/zhousflib/ann/tensorrt/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/tensorrt/__init__.py
--rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/tensorrt/tensorrt_infer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.591005 zhousf-lib-1.5.5/zhousflib/ann/torch/
--rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/torch/__init__.py
--rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/torch/torch_to_onnx.py
--rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/torch/torch_to_script.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.593005 zhousf-lib-1.5.5/zhousflib/ann/transformers/
--rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ann/transformers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.597006 zhousf-lib-1.5.5/zhousflib/database/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/database/__init__.py
--rw-rw-rw-   0        0        0     2630 2024-04-24 02:58:49.000000 zhousf-lib-1.5.5/zhousflib/database/lmdb_master.py
--rw-rw-rw-   0        0        0     2860 2024-04-24 02:55:52.000000 zhousf-lib-1.5.5/zhousflib/database/tinydb_master.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.599007 zhousf-lib-1.5.5/zhousflib/datasets/
--rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.602006 zhousf-lib-1.5.5/zhousflib/datasets/classification/
--rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/classification/__init__.py
--rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/classification/classification_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.611681 zhousf-lib-1.5.5/zhousflib/datasets/coco/
--rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/__init__.py
--rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_extract.py
--rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_update.py
--rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_vis.py
--rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_dataset_merge.py
--rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.624681 zhousf-lib-1.5.5/zhousflib/datasets/labelme/
--rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/__init__.py
--rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_bbox_update.py
--rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_clip.py
--rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_coco.py
--rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_seg.py
--rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_uiex.py
--rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_dataset_clip.py
--rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/labelme/shape_convert.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.627760 zhousf-lib-1.5.5/zhousflib/datasets/segmentation/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/segmentation/__init__.py
--rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/datasets/segmentation/seg_dataset_split.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.631761 zhousf-lib-1.5.5/zhousflib/decorator/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/decorator/__init__.py
--rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/decorator/except_util.py
--rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/decorator/interceptor_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.637763 zhousf-lib-1.5.5/zhousflib/file/
--rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.5/zhousflib/file/__init__.py
--rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/file/delete_file.py
--rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.5/zhousflib/file/download.py
--rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.5/zhousflib/file/zip_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.654350 zhousf-lib-1.5.5/zhousflib/font/
--rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/font/SimSun.ttf
--rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/font/Symbola.ttf
--rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/font/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.665922 zhousf-lib-1.5.5/zhousflib/image/
--rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.5/zhousflib/image/__init__.py
--rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.5/zhousflib/image/cv.py
--rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.5/zhousflib/image/cv_util.py
--rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.5/zhousflib/image/img_util.py
--rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/image/nms_util.py
--rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.5/zhousflib/image/op.py
--rw-rw-rw-   0        0        0     4228 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/image/pil_util.py
--rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.5/zhousflib/image/similarity.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.666921 zhousf-lib-1.5.5/zhousflib/infer_framework/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.678922 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/
--rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/__init__.py
--rw-rw-rw-   0        0        0      851 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend.py
--rw-rw-rw-   0        0        0     3594 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_http.py
--rw-rw-rw-   0        0        0     3685 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_onnx.py
--rw-rw-rw-   0        0        0      612 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_original.py
--rw-rw-rw-   0        0        0     3152 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
--rw-rw-rw-   0        0        0     2661 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_torch_script.py
--rw-rw-rw-   0        0        0     7080 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/fast_infer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.681923 zhousf-lib-1.5.5/zhousflib/infer_framework/triton/
--rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/triton/__init__.py
--rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/infer_framework/triton/client_http.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.684922 zhousf-lib-1.5.5/zhousflib/locust/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/locust/__init__.py
--rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/locust/locust_demo.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.687922 zhousf-lib-1.5.5/zhousflib/metrics/
--rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.5/zhousflib/metrics/__init__.py
--rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.5/zhousflib/metrics/f_score.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.698922 zhousf-lib-1.5.5/zhousflib/ml/
--rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ml/__init__.py
--rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ml/feature_vector.py
--rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ml/model_base.py
--rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ml/model_cluster.py
--rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.5/zhousflib/ml/model_gbdt.py
--rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/ml/model_lr.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.702922 zhousf-lib-1.5.5/zhousflib/pandas/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/pandas/__init__.py
--rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/pandas/openpyxl_util.py
--rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.5/zhousflib/pandas/pandas_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.707987 zhousf-lib-1.5.5/zhousflib/pdf/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/pdf/__init__.py
--rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/pdf/export_image.py
--rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/pdf/pdfplumber_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.712017 zhousf-lib-1.5.5/zhousflib/so/
--rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/so/__init__.py
--rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/so/project_to_so.py
--rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/so/py_to_so.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.714529 zhousf-lib-1.5.5/zhousflib/text/
--rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.5/zhousflib/text/__init__.py
--rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.5/zhousflib/text/similarity.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.720188 zhousf-lib-1.5.5/zhousflib/thread/
--rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.5/zhousflib/thread/__init__.py
--rw-rw-rw-   0        0        0     2318 2024-04-08 01:21:36.000000 zhousf-lib-1.5.5/zhousflib/thread/thread_util.py
--rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/thread/threadpool_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.724191 zhousf-lib-1.5.5/zhousflib/time/
--rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.5/zhousflib/time/__init__.py
--rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.5/zhousflib/time/time_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.753188 zhousf-lib-1.5.5/zhousflib/util/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/calculater_util.py
--rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/char_util.py
--rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/dict_util.py
--rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/encrypt_util.py
--rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/iou_util.py
--rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/json_util.py
--rw-rw-rw-   0        0        0     5205 2024-04-25 02:34:00.000000 zhousf-lib-1.5.5/zhousflib/util/list_util.py
--rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/math_util.py
--rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/permission_util.py
--rw-rw-rw-   0        0        0     3526 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/poly_util.py
--rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/random_util.py
--rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/re_util.py
--rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/singleton.py
--rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/util/string_util.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:34:14.767863 zhousf-lib-1.5.5/zhousflib/web/
--rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/web/__init__.py
--rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/web/config.py
--rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.5/zhousflib/web/fast_api.py
--rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/web/log_util.py
--rw-rw-rw-   0        0        0     4497 2024-03-25 07:18:11.000000 zhousf-lib-1.5.5/zhousflib/web/logger.py
--rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.5/zhousflib/web/response.py
--rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.5/zhousflib/web/web.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:12.049388 zhousf-lib-1.5.6/
+-rw-rw-rw-   0        0        0     1086 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/LICENSE
+-rw-rw-rw-   0        0        0     3232 2024-05-09 02:54:12.048388 zhousf-lib-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2338 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:54:12.049388 zhousf-lib-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     4535 2024-05-09 02:54:06.000000 zhousf-lib-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.989902 zhousf-lib-1.5.6/zhousf_lib.egg-info/
+-rw-rw-rw-   0        0        0     3232 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3912 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 02:54:10.000000 zhousf-lib-1.5.6/zhousf_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.990902 zhousf-lib-1.5.6/zhousflib/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:10.992904 zhousf-lib-1.5.6/zhousflib/ann/
+-rw-rw-rw-   0        0        0     6638 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.015599 zhousf-lib-1.5.6/zhousflib/ann/onnx/
+-rw-rw-rw-   0        0        0     3170 2024-03-25 07:18:11.000000 zhousf-lib-1.5.6/zhousflib/ann/onnx/__init__.py
+-rw-rw-rw-   0        0        0     6855 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/onnx/onnx_to_trt.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.029679 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/__init__.py
+-rw-rw-rw-   0        0        0     5990 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/tensorrt/tensorrt_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.067783 zhousf-lib-1.5.6/zhousflib/ann/torch/
+-rw-rw-rw-   0        0        0     1251 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/__init__.py
+-rw-rw-rw-   0        0        0     6881 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_onnx.py
+-rw-rw-rw-   0        0        0     5934 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_script.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.070783 zhousf-lib-1.5.6/zhousflib/ann/transformers/
+-rw-rw-rw-   0        0        0     1709 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ann/transformers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.089859 zhousf-lib-1.5.6/zhousflib/database/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/database/__init__.py
+-rw-rw-rw-   0        0        0     2630 2024-04-24 02:58:49.000000 zhousf-lib-1.5.6/zhousflib/database/lmdb_master.py
+-rw-rw-rw-   0        0        0     2860 2024-04-24 02:55:52.000000 zhousf-lib-1.5.6/zhousflib/database/tinydb_master.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.112859 zhousf-lib-1.5.6/zhousflib/datasets/
+-rw-rw-rw-   0        0        0       84 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.120193 zhousf-lib-1.5.6/zhousflib/datasets/classification/
+-rw-rw-rw-   0        0        0       73 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/classification/__init__.py
+-rw-rw-rw-   0        0        0     4897 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/classification/classification_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.189065 zhousf-lib-1.5.6/zhousflib/datasets/coco/
+-rw-rw-rw-   0        0        0     1416 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/__init__.py
+-rw-rw-rw-   0        0        0     8259 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_extract.py
+-rw-rw-rw-   0        0        0     5499 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_update.py
+-rw-rw-rw-   0        0        0     6641 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_vis.py
+-rw-rw-rw-   0        0        0     2896 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_merge.py
+-rw-rw-rw-   0        0        0     4946 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.278433 zhousf-lib-1.5.6/zhousflib/datasets/labelme/
+-rw-rw-rw-   0        0        0      981 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/__init__.py
+-rw-rw-rw-   0        0        0     1276 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_bbox_update.py
+-rw-rw-rw-   0        0        0     3906 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_clip.py
+-rw-rw-rw-   0        0        0     8093 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_coco.py
+-rw-rw-rw-   0        0        0     9624 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_seg.py
+-rw-rw-rw-   0        0        0    10464 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_uiex.py
+-rw-rw-rw-   0        0        0     3832 2024-03-25 07:25:54.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_dataset_clip.py
+-rw-rw-rw-   0        0        0     1674 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/labelme/shape_convert.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.287567 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     2958 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/datasets/segmentation/seg_dataset_split.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.296589 zhousf-lib-1.5.6/zhousflib/decorator/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/__init__.py
+-rw-rw-rw-   0        0        0      504 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/except_util.py
+-rw-rw-rw-   0        0        0     1094 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/decorator/interceptor_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.334598 zhousf-lib-1.5.6/zhousflib/file/
+-rw-rw-rw-   0        0        0     1230 2024-01-30 02:48:23.000000 zhousf-lib-1.5.6/zhousflib/file/__init__.py
+-rw-rw-rw-   0        0        0     3250 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/file/delete_file.py
+-rw-rw-rw-   0        0        0     4725 2024-04-01 06:46:05.000000 zhousf-lib-1.5.6/zhousflib/file/download.py
+-rw-rw-rw-   0        0        0     3227 2024-04-01 06:46:05.000000 zhousf-lib-1.5.6/zhousflib/file/zip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.482673 zhousf-lib-1.5.6/zhousflib/font/
+-rw-rw-rw-   0        0        0 15320040 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/SimSun.ttf
+-rw-rw-rw-   0        0        0  2152796 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/Symbola.ttf
+-rw-rw-rw-   0        0        0      765 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/font/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.592577 zhousf-lib-1.5.6/zhousflib/image/
+-rw-rw-rw-   0        0        0     1159 2024-04-01 06:55:42.000000 zhousf-lib-1.5.6/zhousflib/image/__init__.py
+-rw-rw-rw-   0        0        0     5599 2024-01-30 02:48:23.000000 zhousf-lib-1.5.6/zhousflib/image/cv.py
+-rw-rw-rw-   0        0        0     6818 2024-04-01 06:55:42.000000 zhousf-lib-1.5.6/zhousflib/image/cv_util.py
+-rw-rw-rw-   0        0        0     8570 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/image/img_util.py
+-rw-rw-rw-   0        0        0     5768 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/image/nms_util.py
+-rw-rw-rw-   0        0        0     8569 2024-03-25 07:25:55.000000 zhousf-lib-1.5.6/zhousflib/image/op.py
+-rw-rw-rw-   0        0        0     4228 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/image/pil_util.py
+-rw-rw-rw-   0        0        0    10277 2024-03-07 06:30:39.000000 zhousf-lib-1.5.6/zhousflib/image/similarity.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.604547 zhousf-lib-1.5.6/zhousflib/infer_framework/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.666102 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/
+-rw-rw-rw-   0        0        0       86 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/__init__.py
+-rw-rw-rw-   0        0        0      851 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend.py
+-rw-rw-rw-   0        0        0     3594 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_http.py
+-rw-rw-rw-   0        0        0     3685 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_onnx.py
+-rw-rw-rw-   0        0        0      612 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_original.py
+-rw-rw-rw-   0        0        0     3152 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_tensorrt.py
+-rw-rw-rw-   0        0        0     2661 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_torch_script.py
+-rw-rw-rw-   0        0        0     7080 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/fast_infer.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.687091 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/
+-rw-rw-rw-   0        0        0     3124 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/__init__.py
+-rw-rw-rw-   0        0        0    12167 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/infer_framework/triton/client_http.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.697559 zhousf-lib-1.5.6/zhousflib/locust/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/locust/__init__.py
+-rw-rw-rw-   0        0        0     1525 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/locust/locust_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.711587 zhousf-lib-1.5.6/zhousflib/metrics/
+-rw-rw-rw-   0        0        0       76 2024-02-29 06:32:37.000000 zhousf-lib-1.5.6/zhousflib/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3429 2024-03-25 07:21:21.000000 zhousf-lib-1.5.6/zhousflib/metrics/f_score.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.760794 zhousf-lib-1.5.6/zhousflib/ml/
+-rw-rw-rw-   0        0        0       99 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/__init__.py
+-rw-rw-rw-   0        0        0     4515 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/feature_vector.py
+-rw-rw-rw-   0        0        0     8568 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_base.py
+-rw-rw-rw-   0        0        0     2923 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_cluster.py
+-rw-rw-rw-   0        0        0    10995 2024-01-31 01:40:34.000000 zhousf-lib-1.5.6/zhousflib/ml/model_gbdt.py
+-rw-rw-rw-   0        0        0     7630 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/ml/model_lr.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.784286 zhousf-lib-1.5.6/zhousflib/pandas/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4839 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pandas/openpyxl_util.py
+-rw-rw-rw-   0        0        0     6180 2024-04-01 06:42:29.000000 zhousf-lib-1.5.6/zhousflib/pandas/pandas_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.819288 zhousf-lib-1.5.6/zhousflib/pdf/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/__init__.py
+-rw-rw-rw-   0        0        0     1847 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/export_image.py
+-rw-rw-rw-   0        0        0     1465 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/pdf/pdfplumber_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.838437 zhousf-lib-1.5.6/zhousflib/so/
+-rw-rw-rw-   0        0        0       85 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/__init__.py
+-rw-rw-rw-   0        0        0     3840 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/project_to_so.py
+-rw-rw-rw-   0        0        0      286 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/so/py_to_so.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.840407 zhousf-lib-1.5.6/zhousflib/text/
+-rw-rw-rw-   0        0        0       87 2024-01-31 01:12:08.000000 zhousf-lib-1.5.6/zhousflib/text/__init__.py
+-rw-rw-rw-   0        0        0     3141 2024-02-29 06:26:47.000000 zhousf-lib-1.5.6/zhousflib/text/similarity.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.860250 zhousf-lib-1.5.6/zhousflib/thread/
+-rw-rw-rw-   0        0        0       60 2024-04-01 07:09:10.000000 zhousf-lib-1.5.6/zhousflib/thread/__init__.py
+-rw-rw-rw-   0        0        0     2318 2024-04-08 01:21:36.000000 zhousf-lib-1.5.6/zhousflib/thread/thread_util.py
+-rw-rw-rw-   0        0        0      829 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/thread/threadpool_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.878812 zhousf-lib-1.5.6/zhousflib/time/
+-rw-rw-rw-   0        0        0     1159 2024-03-25 07:19:09.000000 zhousf-lib-1.5.6/zhousflib/time/__init__.py
+-rw-rw-rw-   0        0        0     4671 2024-03-25 07:18:11.000000 zhousf-lib-1.5.6/zhousflib/time/time_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:11.999397 zhousf-lib-1.5.6/zhousflib/util/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/__init__.py
+-rw-rw-rw-   0        0        0     3143 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/calculater_util.py
+-rw-rw-rw-   0        0        0     2161 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/char_util.py
+-rw-rw-rw-   0        0        0     2703 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/dict_util.py
+-rw-rw-rw-   0        0        0     2195 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/encrypt_util.py
+-rw-rw-rw-   0        0        0    13480 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/iou_util.py
+-rw-rw-rw-   0        0        0     3373 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/json_util.py
+-rw-rw-rw-   0        0        0     5241 2024-04-29 05:35:07.000000 zhousf-lib-1.5.6/zhousflib/util/list_util.py
+-rw-rw-rw-   0        0        0     1481 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/math_util.py
+-rw-rw-rw-   0        0        0     1358 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/permission_util.py
+-rw-rw-rw-   0        0        0     3526 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/poly_util.py
+-rw-rw-rw-   0        0        0      527 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/random_util.py
+-rw-rw-rw-   0        0        0     4692 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/re_util.py
+-rw-rw-rw-   0        0        0      520 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/singleton.py
+-rw-rw-rw-   0        0        0     5122 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/util/string_util.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:54:12.033155 zhousf-lib-1.5.6/zhousflib/web/
+-rw-rw-rw-   0        0        0       60 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/__init__.py
+-rw-rw-rw-   0        0        0     4246 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/config.py
+-rw-rw-rw-   0        0        0     1200 2024-03-21 07:56:35.000000 zhousf-lib-1.5.6/zhousflib/web/fast_api.py
+-rw-rw-rw-   0        0        0     3107 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/log_util.py
+-rw-rw-rw-   0        0        0     4497 2024-05-09 02:53:54.000000 zhousf-lib-1.5.6/zhousflib/web/logger.py
+-rw-rw-rw-   0        0        0     1340 2024-01-23 07:44:48.000000 zhousf-lib-1.5.6/zhousflib/web/response.py
+-rw-rw-rw-   0        0        0     6913 2024-04-01 08:27:11.000000 zhousf-lib-1.5.6/zhousflib/web/web.py
```

### Comparing `zhousf-lib-1.5.5/LICENSE` & `zhousf-lib-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/PKG-INFO` & `zhousf-lib-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.5
+Version: 1.5.6
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.5/README.md` & `zhousf-lib-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/setup.py` & `zhousf-lib-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 # 打包：python setup.py upload
 NAME = 'zhousf-lib'
 DESCRIPTION = 'a python library of zhousf'
 URL = 'https://github.com/MrZhousf/ZhousfLib'
 EMAIL = '442553199@qq.com'
 AUTHOR = 'zhousf'
 REQUIRES_PYTHON = '>=3.6.13'
-VERSION = '1.5.5'
+VERSION = '1.5.6'
 PACKAGE_DATA = {'': ['*.yaml', '*.ttf', '*.txt', '*.md']}
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 # What packages are required for this module to be executed?
```

### Comparing `zhousf-lib-1.5.5/zhousf_lib.egg-info/PKG-INFO` & `zhousf-lib-1.5.6/zhousf_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhousf-lib
-Version: 1.5.5
+Version: 1.5.6
 Summary: a python library of zhousf
 Home-page: https://github.com/MrZhousf/ZhousfLib
 Author: zhousf
 Author-email: 442553199@qq.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `zhousf-lib-1.5.5/zhousf_lib.egg-info/SOURCES.txt` & `zhousf-lib-1.5.6/zhousf_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/__init__.py` & `zhousf-lib-1.5.6/zhousflib/ann/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/onnx/__init__.py` & `zhousf-lib-1.5.6/zhousflib/ann/onnx/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/onnx/onnx_to_trt.py` & `zhousf-lib-1.5.6/zhousflib/ann/onnx/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/tensorrt/tensorrt_infer.py` & `zhousf-lib-1.5.6/zhousflib/ann/tensorrt/tensorrt_infer.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/torch/__init__.py` & `zhousf-lib-1.5.6/zhousflib/ann/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/torch/torch_to_onnx.py` & `zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_onnx.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/torch/torch_to_script.py` & `zhousf-lib-1.5.6/zhousflib/ann/torch/torch_to_script.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ann/transformers/__init__.py` & `zhousf-lib-1.5.6/zhousflib/ann/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/database/lmdb_master.py` & `zhousf-lib-1.5.6/zhousflib/database/lmdb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/database/tinydb_master.py` & `zhousf-lib-1.5.6/zhousflib/database/tinydb_master.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/classification/classification_dataset_split.py` & `zhousf-lib-1.5.6/zhousflib/datasets/classification/classification_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/__init__.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_extract.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_extract.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_update.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_bbox_vis.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_bbox_vis.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_dataset_merge.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/coco/coco_dataset_split.py` & `zhousf-lib-1.5.6/zhousflib/datasets/coco/coco_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/__init__.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_bbox_update.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_bbox_update.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_clip.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_coco.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_coco.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_seg.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_seg.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_convert_uiex.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_convert_uiex.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/labelme_dataset_clip.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/labelme_dataset_clip.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/labelme/shape_convert.py` & `zhousf-lib-1.5.6/zhousflib/datasets/labelme/shape_convert.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/datasets/segmentation/seg_dataset_split.py` & `zhousf-lib-1.5.6/zhousflib/datasets/segmentation/seg_dataset_split.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/decorator/interceptor_util.py` & `zhousf-lib-1.5.6/zhousflib/decorator/interceptor_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/file/__init__.py` & `zhousf-lib-1.5.6/zhousflib/file/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/file/delete_file.py` & `zhousf-lib-1.5.6/zhousflib/file/delete_file.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/file/download.py` & `zhousf-lib-1.5.6/zhousflib/file/download.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/file/zip_util.py` & `zhousf-lib-1.5.6/zhousflib/file/zip_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/font/SimSun.ttf` & `zhousf-lib-1.5.6/zhousflib/font/SimSun.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/font/Symbola.ttf` & `zhousf-lib-1.5.6/zhousflib/font/Symbola.ttf`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/font/__init__.py` & `zhousf-lib-1.5.6/zhousflib/font/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/__init__.py` & `zhousf-lib-1.5.6/zhousflib/image/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/cv.py` & `zhousf-lib-1.5.6/zhousflib/image/cv.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/cv_util.py` & `zhousf-lib-1.5.6/zhousflib/image/cv_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/img_util.py` & `zhousf-lib-1.5.6/zhousflib/image/img_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/nms_util.py` & `zhousf-lib-1.5.6/zhousflib/image/nms_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/op.py` & `zhousf-lib-1.5.6/zhousflib/image/op.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/pil_util.py` & `zhousf-lib-1.5.6/zhousflib/image/pil_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/image/similarity.py` & `zhousf-lib-1.5.6/zhousflib/image/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_http.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_http.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_onnx.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_onnx.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_original.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_original.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_tensorrt.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_tensorrt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/backend_torch_script.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/backend_torch_script.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/fast_infer/fast_infer.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/fast_infer/fast_infer.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/triton/__init__.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/infer_framework/triton/client_http.py` & `zhousf-lib-1.5.6/zhousflib/infer_framework/triton/client_http.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/locust/locust_demo.py` & `zhousf-lib-1.5.6/zhousflib/locust/locust_demo.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/metrics/f_score.py` & `zhousf-lib-1.5.6/zhousflib/metrics/f_score.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ml/feature_vector.py` & `zhousf-lib-1.5.6/zhousflib/ml/feature_vector.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ml/model_base.py` & `zhousf-lib-1.5.6/zhousflib/ml/model_base.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ml/model_cluster.py` & `zhousf-lib-1.5.6/zhousflib/ml/model_cluster.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ml/model_gbdt.py` & `zhousf-lib-1.5.6/zhousflib/ml/model_gbdt.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/ml/model_lr.py` & `zhousf-lib-1.5.6/zhousflib/ml/model_lr.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/pandas/openpyxl_util.py` & `zhousf-lib-1.5.6/zhousflib/pandas/openpyxl_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/pandas/pandas_util.py` & `zhousf-lib-1.5.6/zhousflib/pandas/pandas_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/pdf/export_image.py` & `zhousf-lib-1.5.6/zhousflib/pdf/export_image.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/pdf/pdfplumber_util.py` & `zhousf-lib-1.5.6/zhousflib/pdf/pdfplumber_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/so/project_to_so.py` & `zhousf-lib-1.5.6/zhousflib/so/project_to_so.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/text/similarity.py` & `zhousf-lib-1.5.6/zhousflib/text/similarity.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/thread/thread_util.py` & `zhousf-lib-1.5.6/zhousflib/thread/thread_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/thread/threadpool_util.py` & `zhousf-lib-1.5.6/zhousflib/thread/threadpool_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/time/__init__.py` & `zhousf-lib-1.5.6/zhousflib/time/__init__.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/time/time_util.py` & `zhousf-lib-1.5.6/zhousflib/time/time_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/calculater_util.py` & `zhousf-lib-1.5.6/zhousflib/util/calculater_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/char_util.py` & `zhousf-lib-1.5.6/zhousflib/util/char_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/dict_util.py` & `zhousf-lib-1.5.6/zhousflib/util/dict_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/encrypt_util.py` & `zhousf-lib-1.5.6/zhousflib/util/encrypt_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/iou_util.py` & `zhousf-lib-1.5.6/zhousflib/util/iou_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/json_util.py` & `zhousf-lib-1.5.6/zhousflib/util/json_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/list_util.py` & `zhousf-lib-1.5.6/zhousflib/util/list_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,11 +195,14 @@
     """
     if chunk_size <= 0:
         return data
     return [data[i * chunk_size:(i+1)*chunk_size] for i in range(0, ceil(len(data) / chunk_size))]
 
 
 def split_list(data: list, split_size=2) -> list:
+    """
+    等分分割
+    """
     splits = np.array_split(np.asarray(data), split_size, axis=0)
     filtered_arrays = [arr for arr in splits if arr.size > 0]
     return [filtered_arrays[i].tolist() for i in range(len(filtered_arrays))]
```

### Comparing `zhousf-lib-1.5.5/zhousflib/util/math_util.py` & `zhousf-lib-1.5.6/zhousflib/util/math_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/permission_util.py` & `zhousf-lib-1.5.6/zhousflib/util/permission_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/poly_util.py` & `zhousf-lib-1.5.6/zhousflib/util/poly_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/random_util.py` & `zhousf-lib-1.5.6/zhousflib/util/random_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/re_util.py` & `zhousf-lib-1.5.6/zhousflib/util/re_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/singleton.py` & `zhousf-lib-1.5.6/zhousflib/util/singleton.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/util/string_util.py` & `zhousf-lib-1.5.6/zhousflib/util/string_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/web/config.py` & `zhousf-lib-1.5.6/zhousflib/web/config.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/web/fast_api.py` & `zhousf-lib-1.5.6/zhousflib/web/fast_api.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/web/log_util.py` & `zhousf-lib-1.5.6/zhousflib/web/log_util.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/web/logger.py` & `zhousf-lib-1.5.6/zhousflib/web/logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -45,20 +45,20 @@
         day_time = time.strftime('%Y/%m/%d %H:%M:%S', time.localtime(time.time())) + '\n'
         if g is not None:
             if hasattr(g, "log"):
                 day_time = g.log
             g.logger = self
         # 日志信息-详细
         self.log_txt = day_time
-        self.title_first("日志路径")
-        self.log(log_dir)
         # 日志信息-仅标题
         self.__log_txt_level = []
         # 耗时
         self.elapsed_time_dict = {}
+        self.title_first("日志路径")
+        self.log(log_dir)
 
     def elapsed_time(self, k: str, start: float, end: float):
         """
         耗时记录
         :param k:
         :param start:
         :param end:
```

### Comparing `zhousf-lib-1.5.5/zhousflib/web/response.py` & `zhousf-lib-1.5.6/zhousflib/web/response.py`

 * *Files identical despite different names*

### Comparing `zhousf-lib-1.5.5/zhousflib/web/web.py` & `zhousf-lib-1.5.6/zhousflib/web/web.py`

 * *Files identical despite different names*

