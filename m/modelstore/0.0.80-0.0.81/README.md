# Comparing `tmp/modelstore-0.0.80.tar.gz` & `tmp/modelstore-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelstore-0.0.80.tar", last modified: Wed Oct 18 11:12:33 2023, max compression
+gzip compressed data, was "modelstore-0.0.81.tar", last modified: Tue May  7 23:53:08 2024, max compression
```

## Comparing `modelstore-0.0.80.tar` & `modelstore-0.0.81.tar`

### file list

```diff
@@ -1,269 +1,172 @@
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.339928 modelstore-0.0.80/
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.220251 modelstore-0.0.80/.github/
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.239355 modelstore-0.0.80/.github/workflows/
--rw-r--r--   0 neallathia   (501) staff       (20)     2296 2022-12-02 10:38:39.000000 modelstore-0.0.80/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 neallathia   (501) staff       (20)     2024 2022-12-03 00:48:26.000000 modelstore-0.0.80/.github/workflows/integration-tests.yml
--rw-r--r--   0 neallathia   (501) staff       (20)      716 2023-03-05 21:12:21.000000 modelstore-0.0.80/.github/workflows/unit-tests.yml
--rw-r--r--   0 neallathia   (501) staff       (20)      189 2023-03-05 21:12:21.000000 modelstore-0.0.80/.gitignore
--rw-r--r--   0 neallathia   (501) staff       (20)    14470 2023-10-16 21:12:19.000000 modelstore-0.0.80/CHANGELOG.md
--rw-r--r--   0 neallathia   (501) staff       (20)     5223 2022-01-13 15:38:40.000000 modelstore-0.0.80/CODE_OF_CONDUCT.md
--rw-r--r--   0 neallathia   (501) staff       (20)     4548 2023-03-19 19:25:32.000000 modelstore-0.0.80/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)    11342 2022-01-13 15:38:40.000000 modelstore-0.0.80/LICENSE
--rw-r--r--   0 neallathia   (501) staff       (20)      489 2023-10-16 21:07:03.000000 modelstore-0.0.80/Makefile
--rw-r--r--   0 neallathia   (501) staff       (20)      949 2023-10-18 11:12:33.339475 modelstore-0.0.80/PKG-INFO
--rw-r--r--   0 neallathia   (501) staff       (20)     6938 2023-09-30 22:46:37.000000 modelstore-0.0.80/README.md
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.246751 modelstore-0.0.80/bin/
--rwxr-xr-x   0 neallathia   (501) staff       (20)      684 2023-06-08 11:33:57.000000 modelstore-0.0.80/bin/_brew_install
--rwxr-xr-x   0 neallathia   (501) staff       (20)      277 2022-12-17 10:26:28.000000 modelstore-0.0.80/bin/_build_library
--rwxr-xr-x   0 neallathia   (501) staff       (20)      222 2022-12-17 10:26:28.000000 modelstore-0.0.80/bin/_cleanup
--rwxr-xr-x   0 neallathia   (501) staff       (20)      262 2023-10-16 21:06:59.000000 modelstore-0.0.80/bin/_pyenv_config
--rwxr-xr-x   0 neallathia   (501) staff       (20)      758 2023-03-12 00:03:54.000000 modelstore-0.0.80/bin/_pyenv_install
--rwxr-xr-x   0 neallathia   (501) staff       (20)      466 2023-02-11 15:06:42.000000 modelstore-0.0.80/bin/_pyenv_uninstall
--rwxr-xr-x   0 neallathia   (501) staff       (20)      225 2022-12-17 10:26:28.000000 modelstore-0.0.80/bin/_release_prod
--rwxr-xr-x   0 neallathia   (501) staff       (20)      251 2022-12-17 10:26:28.000000 modelstore-0.0.80/bin/_release_test
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.248247 modelstore-0.0.80/examples/
--rw-r--r--   0 neallathia   (501) staff       (20)     1055 2023-10-16 21:46:01.000000 modelstore-0.0.80/examples/Makefile-example
--rw-r--r--   0 neallathia   (501) staff       (20)     1720 2023-07-29 18:19:58.000000 modelstore-0.0.80/examples/README.md
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.254166 modelstore-0.0.80/examples/cli-examples/
--rw-r--r--   0 neallathia   (501) staff       (20)       32 2022-01-13 15:38:40.000000 modelstore-0.0.80/examples/cli-examples/.gitignore
--rw-r--r--   0 neallathia   (501) staff       (20)       61 2022-01-13 15:38:40.000000 modelstore-0.0.80/examples/cli-examples/Makefile
--rw-r--r--   0 neallathia   (501) staff       (20)     1614 2023-09-23 12:32:43.000000 modelstore-0.0.80/examples/cli-examples/model.py
--rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-17 13:52:20.000000 modelstore-0.0.80/examples/cli-examples/requirements.txt
--rwxr-xr-x   0 neallathia   (501) staff       (20)      497 2022-01-13 15:38:40.000000 modelstore-0.0.80/examples/cli-examples/run-all.sh
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.258885 modelstore-0.0.80/examples/examples-by-ml-library/
--rw-r--r--   0 neallathia   (501) staff       (20)       62 2022-04-15 16:06:05.000000 modelstore-0.0.80/examples/examples-by-ml-library/Makefile
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.268874 modelstore-0.0.80/examples/examples-by-ml-library/libraries/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2078 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/annoy_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2054 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/catboost_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1746 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/fastai_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1997 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/gensim_example.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.270976 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2023-05-06 22:45:07.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2223 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/distilbert.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1966 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/dpt.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1988 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/gpt2_pytorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1997 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/gpt2_tensorflow.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1889 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/sam.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2177 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/keras_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2216 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/lightgbm_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2261 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/mxnet_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3109 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/onnx_lightgbm_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2474 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/onnx_sklearn_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2039 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/prophet_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2893 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/pyspark_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2562 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/pytorch_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3434 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/pytorch_lightning_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1722 2023-03-19 20:28:18.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/raw_file_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2474 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/shap_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2396 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/sklearn_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2663 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/sklearn_with_explainer_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2689 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/sklearn_with_extras_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2416 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/skorch_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2241 2023-10-17 21:24:40.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/tensorflow_example.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.271743 modelstore-0.0.80/examples/examples-by-ml-library/libraries/util/
--rw-r--r--   0 neallathia   (501) staff       (20)     2368 2023-10-17 21:23:23.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/util/datasets.py
--rw-r--r--   0 neallathia   (501) staff       (20)      747 2023-03-19 20:28:18.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/util/domains.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2198 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/xgboost_booster_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2125 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/xgboost_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1517 2023-10-17 21:24:41.000000 modelstore-0.0.80/examples/examples-by-ml-library/libraries/yolo_example.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3928 2023-10-18 11:06:05.000000 modelstore-0.0.80/examples/examples-by-ml-library/main.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3596 2023-10-17 20:07:31.000000 modelstore-0.0.80/examples/examples-by-ml-library/modelstores.py
--rw-r--r--   0 neallathia   (501) staff       (20)      792 2023-10-17 20:10:43.000000 modelstore-0.0.80/examples/examples-by-ml-library/requirements.txt
--rwxr-xr-x   0 neallathia   (501) staff       (20)      683 2023-10-18 11:06:07.000000 modelstore-0.0.80/examples/examples-by-ml-library/run-all.sh
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.272949 modelstore-0.0.80/modelstore/
--rw-r--r--   0 neallathia   (501) staff       (20)      268 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2601 2022-09-08 11:52:33.000000 modelstore-0.0.80/modelstore/__main__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.275648 modelstore-0.0.80/modelstore/ids/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.80/modelstore/ids/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1638 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/ids/model_ids.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.276131 modelstore-0.0.80/modelstore/metadata/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/modelstore/metadata/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.277647 modelstore-0.0.80/modelstore/metadata/code/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/modelstore/metadata/code/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1938 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/code/code.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2157 2023-09-30 18:08:32.000000 modelstore-0.0.80/modelstore/metadata/code/dependencies.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1699 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/metadata/code/revision.py
--rw-r--r--   0 neallathia   (501) staff       (20)      936 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/metadata/code/runtime.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.278988 modelstore-0.0.80/modelstore/metadata/dataset/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.80/modelstore/metadata/dataset/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1667 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/dataset/dataset.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1761 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/metadata/dataset/features.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2720 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/metadata/dataset/labels.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1271 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/metadata/dataset/types.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2866 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/metadata/metadata.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.279750 modelstore-0.0.80/modelstore/metadata/model/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/modelstore/metadata/model/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1795 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/model/model.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2080 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/model/model_type.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.280217 modelstore-0.0.80/modelstore/metadata/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/modelstore/metadata/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2639 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/storage/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.280715 modelstore-0.0.80/modelstore/metadata/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/modelstore/metadata/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1544 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/metadata/utils/utils.py
--rw-r--r--   0 neallathia   (501) staff       (20)    14523 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/model_store.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.288277 modelstore-0.0.80/modelstore/models/
--rw-r--r--   0 neallathia   (501) staff       (20)     7775 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/models/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/models/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2830 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/models/annoy.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5348 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/models/catboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1119 2022-05-08 12:34:43.000000 modelstore-0.0.80/modelstore/models/common.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3895 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/models/fastai.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3246 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/gensim.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2965 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/lightgbm.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3956 2023-09-25 08:16:58.000000 modelstore-0.0.80/modelstore/models/managers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2241 2022-06-12 22:21:05.000000 modelstore-0.0.80/modelstore/models/missing_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3130 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/models/model_file.py
--rw-r--r--   0 neallathia   (501) staff       (20)     8815 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/models/model_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2903 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/models/multiple_models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3743 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/mxnet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2784 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/onnx.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3236 2023-02-11 15:06:42.000000 modelstore-0.0.80/modelstore/models/prophet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4218 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/models/pyspark.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4907 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/pytorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3659 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/models/pytorch_lightning.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2356 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/models/shap.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3764 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/models/sklearn.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3121 2022-07-03 11:35:08.000000 modelstore-0.0.80/modelstore/models/skorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3531 2023-07-30 20:49:43.000000 modelstore-0.0.80/modelstore/models/tensorflow.py
--rw-r--r--   0 neallathia   (501) staff       (20)     7840 2023-10-17 21:17:27.000000 modelstore-0.0.80/modelstore/models/transformers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1556 2022-05-08 13:46:10.000000 modelstore-0.0.80/modelstore/models/util.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4662 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/models/xgboost.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.291877 modelstore-0.0.80/modelstore/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)     3470 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/storage/CONTRIBUTING.md
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6039 2023-09-30 22:46:37.000000 modelstore-0.0.80/modelstore/storage/aws.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6814 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/storage/azure.py
--rw-r--r--   0 neallathia   (501) staff       (20)    17685 2023-10-17 21:24:39.000000 modelstore-0.0.80/modelstore/storage/blob_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     9823 2023-09-23 15:59:13.000000 modelstore-0.0.80/modelstore/storage/gcloud.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4794 2023-10-16 21:41:09.000000 modelstore-0.0.80/modelstore/storage/hdfs.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6660 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/storage/local.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6698 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/storage/minio.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.292358 modelstore-0.0.80/modelstore/storage/states/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.80/modelstore/storage/states/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1452 2023-07-01 09:48:47.000000 modelstore-0.0.80/modelstore/storage/states/model_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4311 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/storage/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.294256 modelstore-0.0.80/modelstore/storage/util/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/storage/util/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1382 2022-05-08 13:46:10.000000 modelstore-0.0.80/modelstore/storage/util/environment.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4456 2022-12-17 10:26:28.000000 modelstore-0.0.80/modelstore/storage/util/paths.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1147 2022-05-08 13:46:10.000000 modelstore-0.0.80/modelstore/storage/util/versions.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.295506 modelstore-0.0.80/modelstore/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/modelstore/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3555 2023-09-23 12:32:43.000000 modelstore-0.0.80/modelstore/utils/cli.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1917 2022-05-08 13:46:10.000000 modelstore-0.0.80/modelstore/utils/exceptions.py
--rw-r--r--   0 neallathia   (501) staff       (20)      982 2023-10-17 21:17:51.000000 modelstore-0.0.80/modelstore/utils/log.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.275119 modelstore-0.0.80/modelstore.egg-info/
--rw-r--r--   0 neallathia   (501) staff       (20)      949 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/PKG-INFO
--rw-r--r--   0 neallathia   (501) staff       (20)     7989 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/SOURCES.txt
--rw-r--r--   0 neallathia   (501) staff       (20)        1 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/dependency_links.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       55 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/entry_points.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      147 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/requires.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       17 2023-10-18 11:12:33.000000 modelstore-0.0.80/modelstore.egg-info/top_level.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      367 2022-01-13 15:38:40.000000 modelstore-0.0.80/pytest.ini
--rw-r--r--   0 neallathia   (501) staff       (20)      453 2023-10-16 21:07:03.000000 modelstore-0.0.80/requirements-dev0.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      818 2023-10-16 21:07:03.000000 modelstore-0.0.80/requirements-dev1.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      145 2023-10-16 21:07:03.000000 modelstore-0.0.80/requirements.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       38 2023-10-18 11:12:33.340023 modelstore-0.0.80/setup.cfg
--rw-r--r--   0 neallathia   (501) staff       (20)     1201 2023-10-16 21:09:26.000000 modelstore-0.0.80/setup.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.296683 modelstore-0.0.80/tests/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/tests/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.297206 modelstore-0.0.80/tests/ids/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-04-15 14:47:26.000000 modelstore-0.0.80/tests/ids/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1337 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/ids/test_model_ids.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.297727 modelstore-0.0.80/tests/metadata/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/tests/metadata/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.299599 modelstore-0.0.80/tests/metadata/code/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/tests/metadata/code/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1746 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/metadata/code/test_code.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1542 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/metadata/code/test_dependencies.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1711 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/metadata/code/test_revision.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1116 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/metadata/code/test_runtime.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.301194 modelstore-0.0.80/tests/metadata/dataset/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-12 22:21:05.000000 modelstore-0.0.80/tests/metadata/dataset/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1123 2022-06-12 22:21:05.000000 modelstore-0.0.80/tests/metadata/dataset/fixtures.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1497 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/metadata/dataset/test_dataset.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1384 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/metadata/dataset/test_features.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1575 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/metadata/dataset/test_labels.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1713 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/metadata/dataset/test_types.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.301965 modelstore-0.0.80/tests/metadata/model/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/tests/metadata/model/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1421 2022-12-17 10:26:28.000000 modelstore-0.0.80/tests/metadata/model/test_model.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2271 2022-12-17 10:26:28.000000 modelstore-0.0.80/tests/metadata/model/test_model_type.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.302449 modelstore-0.0.80/tests/metadata/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/tests/metadata/storage/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2069 2022-12-17 10:26:28.000000 modelstore-0.0.80/tests/metadata/storage/test_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2706 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/metadata/test_metadata.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.302943 modelstore-0.0.80/tests/metadata/utils/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-05-25 22:34:04.000000 modelstore-0.0.80/tests/metadata/utils/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1865 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/metadata/utils/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.317111 modelstore-0.0.80/tests/models/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/tests/models/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3567 2022-06-12 22:21:05.000000 modelstore-0.0.80/tests/models/test_annoy.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4215 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_catboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1425 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/models/test_common.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5092 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_fastai.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3449 2022-12-17 10:26:28.000000 modelstore-0.0.80/tests/models/test_gensim.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4245 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_lightgbm.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2571 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/models/test_managers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1303 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/models/test_missing_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2627 2022-06-12 22:21:05.000000 modelstore-0.0.80/tests/models/test_model_file.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6196 2023-09-30 22:46:40.000000 modelstore-0.0.80/tests/models/test_model_manager.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4992 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_multiple_models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3659 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/models/test_mxnet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4080 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_onnx.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3856 2022-06-12 22:21:05.000000 modelstore-0.0.80/tests/models/test_prophet.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4491 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_pyspark.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4647 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_pytorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5346 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_pytorch_lightning.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3661 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_shap.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4575 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_sklearn.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3941 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_skorch.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4663 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_tensorflow.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4769 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_transformers.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6211 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/models/test_xgboost.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1519 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/models/utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.324533 modelstore-0.0.80/tests/storage/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/tests/storage/__init__.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.325842 modelstore-0.0.80/tests/storage/states/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-02-20 17:43:37.000000 modelstore-0.0.80/tests/storage/states/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1281 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/states/test_model_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5980 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_aws.py
--rw-r--r--   0 neallathia   (501) staff       (20)     9260 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_azure.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1829 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/storage/test_blob_storage.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3158 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_blob_storage_artifacts.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3728 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_blob_storage_meta_data.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6775 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_blob_storage_states.py
--rw-r--r--   0 neallathia   (501) staff       (20)    10047 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_gcloud.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4138 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_hdfs.py
--rw-r--r--   0 neallathia   (501) staff       (20)     6348 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_local.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5516 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/storage/test_minio.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2504 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/storage/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.327217 modelstore-0.0.80/tests/storage/util/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-01-13 15:38:40.000000 modelstore-0.0.80/tests/storage/util/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     4362 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/storage/util/test_paths.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3803 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/test_model_store.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3333 2023-10-17 21:24:40.000000 modelstore-0.0.80/tests/test_model_store_filesystem.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2202 2023-09-23 12:32:43.000000 modelstore-0.0.80/tests/test_utils.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.330733 modelstore-0.0.80/workflows/
--rw-r--r--   0 neallathia   (501) staff       (20)      640 2023-02-19 11:42:44.000000 modelstore-0.0.80/workflows/Makefile
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.333644 modelstore-0.0.80/workflows/actions/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.80/workflows/actions/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1900 2023-10-17 21:24:40.000000 modelstore-0.0.80/workflows/actions/actions.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1910 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/actions/cli.py
--rw-r--r--   0 neallathia   (501) staff       (20)     5143 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/actions/models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1789 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/actions/storage.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.334982 modelstore-0.0.80/workflows/fixtures/
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.80/workflows/fixtures/__init__.py
--rw-r--r--   0 neallathia   (501) staff       (20)     1433 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/fixtures/extra.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2058 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/fixtures/models.py
--rw-r--r--   0 neallathia   (501) staff       (20)     3070 2022-12-17 10:26:28.000000 modelstore-0.0.80/workflows/fixtures/modelstores.py
--rw-r--r--   0 neallathia   (501) staff       (20)     2429 2023-09-23 12:32:43.000000 modelstore-0.0.80/workflows/main.py
-drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2023-10-18 11:12:33.337515 modelstore-0.0.80/workflows/requirements/
--rw-r--r--   0 neallathia   (501) staff       (20)       14 2022-09-08 11:52:33.000000 modelstore-0.0.80/workflows/requirements/aws-s3.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       45 2022-09-08 11:52:33.000000 modelstore-0.0.80/workflows/requirements/azure-container.txt
--rw-r--r--   0 neallathia   (501) staff       (20)        0 2022-06-25 18:07:50.000000 modelstore-0.0.80/workflows/requirements/filesystem.txt
--rw-r--r--   0 neallathia   (501) staff       (20)      104 2022-09-08 11:52:33.000000 modelstore-0.0.80/workflows/requirements/google-cloud-storage.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       13 2022-12-03 00:48:26.000000 modelstore-0.0.80/workflows/requirements/minio.txt
--rw-r--r--   0 neallathia   (501) staff       (20)       48 2023-02-11 15:06:42.000000 modelstore-0.0.80/workflows/requirements.txt
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.593852 modelstore-0.0.81/
+-rw-r--r--   0 neallathia   (501) staff       (20)    11342 2024-02-10 14:16:27.000000 modelstore-0.0.81/LICENSE
+-rw-r--r--   0 neallathia   (501) staff       (20)      949 2024-05-07 23:53:08.593660 modelstore-0.0.81/PKG-INFO
+-rw-r--r--   0 neallathia   (501) staff       (20)     7184 2024-05-07 14:14:50.000000 modelstore-0.0.81/README.md
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.576536 modelstore-0.0.81/modelstore/
+-rw-r--r--   0 neallathia   (501) staff       (20)      873 2024-05-01 16:43:37.000000 modelstore-0.0.81/modelstore/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2601 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/__main__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.577532 modelstore-0.0.81/modelstore/ids/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/ids/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1638 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/ids/model_ids.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.577887 modelstore-0.0.81/modelstore/metadata/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.578524 modelstore-0.0.81/modelstore/metadata/code/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/code/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1938 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/code/code.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2157 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/code/dependencies.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1699 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/code/revision.py
+-rw-r--r--   0 neallathia   (501) staff       (20)      936 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/code/runtime.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.579119 modelstore-0.0.81/modelstore/metadata/dataset/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/dataset/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1667 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/dataset/dataset.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1761 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/dataset/features.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2720 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/dataset/labels.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1271 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/dataset/types.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2866 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/metadata.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.579465 modelstore-0.0.81/modelstore/metadata/model/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/model/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1795 2024-02-11 23:26:40.000000 modelstore-0.0.81/modelstore/metadata/model/model.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2080 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/model/model_type.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.579685 modelstore-0.0.81/modelstore/metadata/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2639 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/storage/storage.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.579892 modelstore-0.0.81/modelstore/metadata/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1544 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/metadata/utils/utils.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    14523 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/model_store.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.582941 modelstore-0.0.81/modelstore/models/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2830 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/annoy.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5348 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/catboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2371 2024-05-07 14:17:08.000000 modelstore-0.0.81/modelstore/models/causalml.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1119 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/common.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3895 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/fastai.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3246 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/gensim.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2965 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/lightgbm.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3968 2024-05-07 14:17:08.000000 modelstore-0.0.81/modelstore/models/managers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2241 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/missing_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3130 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/model_file.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     8815 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/model_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2903 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/multiple_models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2784 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/onnx.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3236 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/prophet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4218 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/pyspark.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4907 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/pytorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3659 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/pytorch_lightning.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2356 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/shap.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3764 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/sklearn.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3121 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/skorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4705 2024-05-05 22:43:35.000000 modelstore-0.0.81/modelstore/models/tensorflow.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     7928 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/transformers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1556 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/util.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4662 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/models/xgboost.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.584116 modelstore-0.0.81/modelstore/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6039 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/aws.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6814 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/azure.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    17685 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/blob_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     9823 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/gcloud.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4794 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/hdfs.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6660 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/local.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6698 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/minio.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.584353 modelstore-0.0.81/modelstore/storage/states/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/states/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1452 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/states/model_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4311 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/storage.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.584813 modelstore-0.0.81/modelstore/storage/util/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/util/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1382 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/util/environment.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4456 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/util/paths.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1147 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/storage/util/versions.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.585257 modelstore-0.0.81/modelstore/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3555 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/utils/cli.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1917 2024-02-10 14:16:27.000000 modelstore-0.0.81/modelstore/utils/exceptions.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1194 2024-05-01 16:43:37.000000 modelstore-0.0.81/modelstore/utils/log.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.593425 modelstore-0.0.81/modelstore.egg-info/
+-rw-r--r--   0 neallathia   (501) staff       (20)      949 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/PKG-INFO
+-rw-r--r--   0 neallathia   (501) staff       (20)     4538 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/SOURCES.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)        1 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/dependency_links.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       55 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/entry_points.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)      147 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/requires.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       17 2024-05-07 23:53:08.000000 modelstore-0.0.81/modelstore.egg-info/top_level.txt
+-rw-r--r--   0 neallathia   (501) staff       (20)       38 2024-05-07 23:53:08.593895 modelstore-0.0.81/setup.cfg
+-rw-r--r--   0 neallathia   (501) staff       (20)     1201 2024-05-07 14:17:18.000000 modelstore-0.0.81/setup.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.585607 modelstore-0.0.81/tests/
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.585813 modelstore-0.0.81/tests/ids/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/ids/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1337 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/ids/test_model_ids.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.586029 modelstore-0.0.81/tests/metadata/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.586576 modelstore-0.0.81/tests/metadata/code/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/code/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1746 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/code/test_code.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1542 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/code/test_dependencies.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1795 2024-05-01 16:43:37.000000 modelstore-0.0.81/tests/metadata/code/test_revision.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1116 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/code/test_runtime.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.587256 modelstore-0.0.81/tests/metadata/dataset/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1123 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/fixtures.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1497 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/test_dataset.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1384 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/test_features.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1575 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/test_labels.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1713 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/dataset/test_types.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.587611 modelstore-0.0.81/tests/metadata/model/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/model/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1421 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/model/test_model.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2271 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/model/test_model_type.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.587856 modelstore-0.0.81/tests/metadata/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/storage/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2069 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/storage/test_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2706 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/test_metadata.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.588083 modelstore-0.0.81/tests/metadata/utils/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/utils/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1865 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/metadata/utils/test_utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.591344 modelstore-0.0.81/tests/models/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3567 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_annoy.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4215 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_catboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4731 2024-05-07 14:17:08.000000 modelstore-0.0.81/tests/models/test_causalml.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1425 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_common.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5092 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_fastai.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3449 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_gensim.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4245 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_lightgbm.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2571 2024-05-07 14:17:08.000000 modelstore-0.0.81/tests/models/test_managers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1303 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_missing_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2627 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_model_file.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6196 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_model_manager.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5001 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_multiple_models.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4080 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_onnx.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3856 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_prophet.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4491 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_pyspark.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4647 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_pytorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5346 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_pytorch_lightning.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3670 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_shap.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4575 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_sklearn.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3941 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_skorch.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6045 2024-05-05 22:43:35.000000 modelstore-0.0.81/tests/models/test_tensorflow.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4448 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_transformers.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6437 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/test_xgboost.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1519 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/models/utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.592831 modelstore-0.0.81/tests/storage/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/__init__.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.593040 modelstore-0.0.81/tests/storage/states/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/states/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1281 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/states/test_model_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5978 2024-05-01 16:43:37.000000 modelstore-0.0.81/tests/storage/test_aws.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     9260 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_azure.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     1829 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_blob_storage.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3158 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_blob_storage_artifacts.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3728 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_blob_storage_meta_data.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6775 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_blob_storage_states.py
+-rw-r--r--   0 neallathia   (501) staff       (20)    10047 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_gcloud.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4138 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_hdfs.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     6348 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_local.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     5516 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_minio.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2504 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/test_utils.py
+drwxr-xr-x   0 neallathia   (501) staff       (20)        0 2024-05-07 23:53:08.593248 modelstore-0.0.81/tests/storage/util/
+-rw-r--r--   0 neallathia   (501) staff       (20)        0 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/util/__init__.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     4362 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/storage/util/test_paths.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3803 2024-02-10 14:16:27.000000 modelstore-0.0.81/tests/test_model_store.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     3334 2024-05-01 16:43:37.000000 modelstore-0.0.81/tests/test_model_store_filesystem.py
+-rw-r--r--   0 neallathia   (501) staff       (20)     2202 2024-05-05 22:43:35.000000 modelstore-0.0.81/tests/test_utils.py
```

### Comparing `modelstore-0.0.80/LICENSE` & `modelstore-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/PKG-INFO` & `modelstore-0.0.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelstore
-Version: 0.0.80
+Version: 0.0.81
 Summary: modelstore is a library for versioning, exporting, storing, and loading machine learning models
 Home-page: https://github.com/operatorai/modelstore
 Author: Neal Lathia
 License: Please refer to the readme
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `modelstore-0.0.80/README.md` & `modelstore-0.0.81/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 * A filesystem directory ([example](https://github.com/operatorai/modelstore/blob/b096275018674243835d21102f75b6270dfa2c97/examples/examples-by-storage/modelstores.py#L44-L49))
 
 
 ## Supported machine learning libraries
 
 * [Annoy](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/annoy_example.py)
 * [Catboost](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/catboost_example.py)
+* [CausalML](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/causalml_example.py)
 * [Fast.AI](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/fastai_example.py)
 * [Gensim](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/gensim_example.py)
 * [Keras](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/keras_example.py)
 * [LightGBM](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/lightgbm_example.py)
 * [Mxnet](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/mxnet_example.py)
 * [Onnx](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/onnx_sklearn_example.py)
 * [Prophet](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/prophet_example.py)
@@ -73,14 +74,15 @@
 
 Is there a machine learning framework that is missing? 
 * Save your model and then upload it [as a raw file](https://github.com/operatorai/modelstore/blob/main/examples/examples-by-ml-library/libraries/raw_file_example.py).
 * Feel free to [open an issue](https://github.com/operatorai/modelstore/issues)
 
 ## Read more about modelstore
 
+* [35 Hidden Python Libraries That Are Absolute Gems](https://www.blog.dailydoseofds.com/p/35-gem-py-libs), March 2023
 * [Evidently.AI AMA with Neal Lathia](https://www.evidentlyai.com/blog/ama-neal-lathia), January 2023
 * [MLOps Model Stores: Definition, Functionality, Tools Review](https://neptune.ai/blog/mlops-model-stores), January 2023
 * [Monzo's machine learning stack](https://monzo.com/blog/2022/04/26/monzos-machine-learning-stack), April 2022
 * [Data Talks Club Minis: Model Store](https://www.youtube.com/watch?v=85BWnKmOZl8), July 2021
 * [Model arterfacts: the war stories](https://nlathia.github.io/2020/09/Model-artifacts-war-stories.html), September 2020
 
 ## Example Usage
```

### Comparing `modelstore-0.0.80/examples/examples-by-ml-library/libraries/annoy_example.py` & `modelstore-0.0.81/modelstore/models/annoy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,93 @@
-#    Copyright 2023 Neal Lathia
+#    Copyright 2020 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-import random
+import os
+from functools import partial
+from typing import Any
 
-from annoy import AnnoyIndex
+from modelstore.metadata import metadata
+from modelstore.models.model_manager import ModelManager
+from modelstore.storage.storage import CloudStorage
+from modelstore.utils.log import logger
 
-from modelstore.model_store import ModelStore
+MODEL_FILE = "model.ann"
 
-_NUM_DIMENSIONS = 40
-_NUM_TREES = 10
-_METRIC = "angular"
-_DOMAIN_NAME = "example-annoy-index"
-
-
-def _train_example_model() -> AnnoyIndex:
-    # Create an index
-    print("🤖  Creating an Annoy index...")
-    model = AnnoyIndex(_NUM_DIMENSIONS, _METRIC)
-    for i in range(1000):
-        vector = [random.gauss(0, 1) for z in range(_NUM_DIMENSIONS)]
-        model.add_item(i, vector)
-    model.build(_NUM_TREES)
-
-    # Show some nearest neighbours
-    results = model.get_nns_by_item(0, 10)
-    print(f"🔍  Nearest neighbors = {results}.")
-    return model
-
-
-def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train an Annoy index
-    model = _train_example_model()
-
-    # Upload the model to the model store
-    print(f'⤴️  Uploading the Annoy model to the "{_DOMAIN_NAME}" domain.')
-    meta_data = modelstore.upload(
-        _DOMAIN_NAME,
-        model=model,
-        num_dimensions=_NUM_DIMENSIONS,
-        metric=_METRIC,
-        num_trees=_NUM_TREES,
-    )
-    return meta_data
-
-
-def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
-    # Load the model back into memory!
-    print(f'⤵️  Loading the Annoy "{model_domain}" domain model={model_id}')
-    model = modelstore.load(model_domain, model_id)
-
-    # Find some nearest neighbours
-    results = model.get_nns_by_item(0, 10)
-    print(f"🔍  Nearest neighbors = {results}.")
+
+class AnnoyManager(ModelManager):
+
+    """
+    Model persistence for Annoy models:
+    https://github.com/spotify/annoy
+    """
+
+    NAME = "annoy"
+
+    def __init__(self, storage: CloudStorage = None):
+        super().__init__(self.NAME, storage)
+
+    def required_dependencies(self) -> list:
+        return ["annoy"]
+
+    def _required_kwargs(self):
+        return ["model", "metric", "num_trees"]
+
+    def matches_with(self, **kwargs) -> bool:
+        # pylint: disable=import-outside-toplevel
+        from annoy import AnnoyIndex
+
+        return isinstance(kwargs.get("model"), AnnoyIndex)
+
+    def _get_functions(self, **kwargs) -> list:
+        if not self.matches_with(**kwargs):
+            raise TypeError("Model is not an AnnoyIndex!")
+
+        return [
+            partial(
+                save_model,
+                model=kwargs["model"],
+            ),
+        ]
+
+    def get_params(self, **kwargs) -> dict:
+        return {
+            "num_dimensions": kwargs["model"].f,
+            "num_trees": kwargs["num_trees"],
+            "metric": kwargs["metric"],
+        }
+
+    def load(self, model_path: str, meta_data: metadata.Summary) -> Any:
+        super().load(model_path, meta_data)
+
+        # pylint: disable=import-outside-toplevel
+        from annoy import AnnoyIndex
+
+        # Extract index size & metric from the meta_data
+        params = meta_data.model.parameters
+        num_dimensions = int(params["num_dimensions"])
+        metric = params["metric"]
+
+        model = AnnoyIndex(num_dimensions, metric)
+        model.load(_model_file_path(model_path))
+        return model
+
+
+def _model_file_path(tmp_dir: str) -> str:
+    return os.path.join(tmp_dir, MODEL_FILE)
+
+
+def save_model(tmp_dir: str, model: "annoy.AnnoyIndex") -> str:
+    """Saves an annoy index to file"""
+    file_path = _model_file_path(tmp_dir)
+    logger.debug("Saving annoy model to %s", file_path)
+    model.save(file_path)
+    return file_path
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modelstore-0.0.80/examples/examples-by-ml-library/libraries/huggingface/gpt2_pytorch.py` & `modelstore-0.0.81/modelstore/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,79 @@
-#    Copyright 2023 Neal Lathia
+#    Copyright 2021 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+import os
 
-from transformers import GPT2LMHeadModel, GPT2Tokenizer
+import click
 
-from modelstore.model_store import ModelStore
+from modelstore.utils import cli as modelstorecli
 
-_DOMAIN_NAME = "example-gpt2-model"
 
+@click.group()
+def download_model():
+    pass
+
+
+@click.group()
+def upload_model():
+    pass
+
+
+@download_model.command()
+@click.argument("domain", type=str, required=True)
+@click.argument("model_id", type=str, required=True)
+@click.argument("parent_dir", type=str, required=False, default=None)
+def download(domain: str, model_id: str, parent_dir: str):
+    """Download a model from the modelstore. Usage:\n
+    ❯ python -m modelstore download <domain> <model-id> <parent-directory>
+    """
+    try:
+        target_dir = (
+            os.path.join(parent_dir, domain, model_id)
+            if parent_dir is not None
+            else os.path.join(domain, model_id)
+        )
+        os.makedirs(target_dir, exist_ok=True)
+
+        model_store = modelstorecli.model_store_from_env()
+        archive_path = model_store.download(target_dir, domain, model_id)
+        modelstorecli.success(f"✅  Downloaded: {domain}={model_id} to {archive_path}")
+    except Exception:
+        modelstorecli.failure("❌  Failed to download model:")
+        raise
+
+
+@upload_model.command()
+@click.argument("domain", type=str, required=True)
+@click.argument("model", type=click.Path(exists=True))
+def upload(domain: str, model: str):
+    """Upload a model to the modelstore. Usage:\n
+    ❯ python -m modelstore upload <domain> /path/to/file
+    """
+    try:
+        model_store = modelstorecli.model_store_from_env()
+        meta_data = model_store.upload(domain, model=model)
+        model_id = meta_data["model"]["model_id"]
+        modelstorecli.success(f"✅  Uploaded: {domain}={model_id}")
+        print(model_id)
+    except SystemExit:
+        # Failed to instantiate a model store from environment variables
+        pass
+    except Exception:
+        modelstorecli.failure("❌  Failed to upload model:")
+        raise
 
-def _run_prediction(model: GPT2LMHeadModel, tokenizer: GPT2Tokenizer):
-    text = "What is MLOps, and why is it important?"
-    encoded_input = tokenizer(text, return_tensors="pt")
-    output = model.generate(**encoded_input)
-    decoded = tokenizer.decode(output[0])
-    print(f"🔍 Model output={decoded}.")
 
+cli = click.CommandCollection(sources=[download_model, upload_model])
 
-def _train_example_model():
-    # Returns a PyTorch model
-    tokenizer = GPT2Tokenizer.from_pretrained("gpt2")
-    model = GPT2LMHeadModel.from_pretrained("gpt2")
-
-    _run_prediction(model, tokenizer)
-    return model, tokenizer
-
-
-def train_and_upload(modelstore: ModelStore) -> dict:
-    # Train a model
-    model, tokenizer = _train_example_model()
-
-    # Upload the model to the model store
-    print(f'⤴️  Uploading the transformers model to the "{_DOMAIN_NAME}" domain.')
-    meta_data = modelstore.upload(
-        _DOMAIN_NAME,
-        model=model,
-        tokenizer=tokenizer,
-    )
-    return meta_data
-
-
-def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
-    # Load the model back into memory!
-    print(f'⤵️  Loading the transformers "{model_domain}" domain model={model_id}')
-    model, tokenizer, _ = modelstore.load(model_domain, model_id)
-    _run_prediction(model, tokenizer)
+if __name__ == "__main__":
+    cli()
```

### Comparing `modelstore-0.0.80/examples/examples-by-ml-library/libraries/util/domains.py` & `modelstore-0.0.81/modelstore/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-#    Copyright 2023 Neal Lathia
+#    Copyright 2024 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+from pkg_resources import DistributionNotFound, get_distribution
 
-DIABETES_DOMAIN = "diabetes-boosting-demo"
-NEWSGROUP_EMBEDDINGS_DOMAIN = "newsgroups-embeddings"
-BREAST_CANCER_DOMAIN = "breast-cancer-demo"
+# pylint: disable=unused-import
+from modelstore.model_store import ModelStore
+
+try:
+    __version__ = get_distribution("modelstore").version
+except DistributionNotFound:
+    __version__ = "unavailable"
```

### Comparing `modelstore-0.0.80/examples/examples-by-ml-library/libraries/yolo_example.py` & `modelstore-0.0.81/modelstore/models/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-#    Copyright 2023 Neal Lathia
+#    Copyright 2020 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+import json
+import os
+from typing import Any
 
-import torch
+import joblib
 
-from modelstore.model_store import ModelStore
 
-_YOLO_DOMAIN = "yolov5"
+def save_json(tmp_dir: str, file_name: str, data: dict) -> str:
+    target = os.path.join(tmp_dir, file_name)
+    with open(target, "w") as out:
+        out.write(json.dumps(data))
+    return target
 
 
-def _predict(model):
-    model.eval()
-    img = "https://ultralytics.com/images/zidane.jpg"
-    results = model(img)
-    print(f"🔍  Prediction result: \n{results.pandas().xyxy[0]}.")
+def save_joblib(tmp_dir: str, model: Any, file_name: str) -> str:
+    model_path = os.path.join(tmp_dir, file_name)
+    joblib.dump(model, model_path)
+    return model_path
 
 
-def train_and_upload(modelstore: ModelStore) -> dict:
-    # Load the yolov5 model
-    model = torch.hub.load("ultralytics/yolov5", "yolov5s")
-    _predict(model)
-
-    # Upload the model to the model store
-    print(f'⤴️  Uploading the yolo model to the "{_YOLO_DOMAIN}" domain.')
-    meta_data = modelstore.upload(_YOLO_DOMAIN, model=model)
-    return meta_data
-
-
-def load_and_test(modelstore: ModelStore, model_domain: str, model_id: str):
-    # Load the model back into memory!
-    print(f'⤵️  Loading the yolo "{model_domain}" domain model={model_id}')
-    model = modelstore.load(model_domain, model_id)
-    _predict(model)
+def load_joblib(model_path: str) -> Any:
+    return joblib.load(model_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modelstore-0.0.80/examples/examples-by-ml-library/modelstores.py` & `modelstore-0.0.81/modelstore/utils/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,90 +8,99 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
+import sys
+from enum import Enum
+
+import click
 
 from modelstore import ModelStore
 from modelstore.storage.aws import AWSStorage
 from modelstore.storage.azure import AzureBlobStorage
 from modelstore.storage.gcloud import GoogleCloudStorage
-# from modelstore.storage.hdfs import HdfsStorage
 from modelstore.storage.local import FileSystemStorage
 from modelstore.storage.minio import MinIOStorage
 
+STORAGE_TYPES = {
+    AWSStorage.NAME: AWSStorage,
+    AzureBlobStorage.NAME: AzureBlobStorage,
+    GoogleCloudStorage.NAME: GoogleCloudStorage,
+    FileSystemStorage.NAME: FileSystemStorage,
+    MinIOStorage.NAME: MinIOStorage,
+}
 
-def create_aws_model_store() -> ModelStore:
-    """A model store that uses an s3 bucket"""
-    return ModelStore.from_aws_s3(
-        os.environ["MODEL_STORE_AWS_BUCKET"],
-        root_prefix="example-by-ml-library",
-    )
-
-
-def create_azure_model_store() -> ModelStore:
-    """A model store that uses an azure container"""
-    # A model store in an Azure Container
-    # The modelstore library assumes that:
-    # 1. You have already created an Azure container
-    # 2. You have an os environment variable called AZURE_STORAGE_CONNECTION_STRING
-    return ModelStore.from_azure(
-        container_name=os.environ["MODEL_STORE_AZURE_CONTAINER"],
-        root_prefix=os.environ.get("MODEL_STORE_AZURE_ROOT_PREFIX"),
-    )
-
-
-def create_file_system_model_store() -> ModelStore:
-    """A model store in a local file system"""
-    # Here, we create a new local model store in our home directory
-    root_dir = os.environ.get(
-        "MODEL_STORE_ROOT_PREFIX",
-        os.path.expanduser("~"),
-    )
-    print(f"🏦  Creating store in: {root_dir}")
-    return ModelStore.from_file_system(root_directory=root_dir)
-
-
-def create_gcloud_model_store() -> ModelStore:
-    """A model store in a Google Cloud bucket"""
-    # The modelstore library assumes you have already created
-    # a Cloud Storage bucket and will raise an exception if it doesn't exist
-    return ModelStore.from_gcloud(
-        os.environ["MODEL_STORE_GCP_PROJECT"],
-        os.environ["MODEL_STORE_GCP_BUCKET"],
-        root_prefix=os.environ.get("MODEL_STORE_GCP_ROOT_PREFIX"),
-    )
-
-
-# def create_hdfs_model_store() -> ModelStore:
-#     """A model store in HDFS storage"""
-#     return ModelStore.from_hdfs(
-#         root_prefix=os.environ["MODEL_STORE_HDFS_ROOT_PREFIX"],
-#         create_directory=True,
-#     )
-
-
-def create_minio_model_store() -> ModelStore:
-    """A model store that uses an s3 bucket with a MinIO client"""
-    return ModelStore.from_minio(
-        access_key=os.environ["AWS_ACCESS_KEY_ID"],
-        secret_key=os.environ["AWS_SECRET_ACCESS_KEY"],
-        bucket_name=os.environ["MODEL_STORE_AWS_BUCKET"],
-        root_prefix="example-by-ml-library",
-    )
-
-
-MODELSTORES = {
-    AWSStorage.NAME: create_aws_model_store,
-    AzureBlobStorage.NAME: create_azure_model_store,
-    FileSystemStorage.NAME: create_file_system_model_store,
-    GoogleCloudStorage.NAME: create_gcloud_model_store,
-    # HdfsStorage.NAME: create_hdfs_model_store,
-    MinIOStorage.NAME: create_minio_model_store,
+MODEL_STORE_TYPES = {
+    AWSStorage.NAME: ModelStore.from_aws_s3,
+    AzureBlobStorage.NAME: ModelStore.from_azure,
+    GoogleCloudStorage.NAME: ModelStore.from_gcloud,
+    FileSystemStorage.NAME: ModelStore.from_file_system,
+    MinIOStorage.NAME: ModelStore.from_minio,
 }
 
 
-def create_model_store(backend) -> ModelStore:
-    """Returns a modelstore instance with the required storage type"""
-    return MODELSTORES[backend]()
+class MessageStatus(Enum):
+
+    """
+    MessageStatus enumerates the different potential statuses
+    that we can print messages about in the CLI, and their
+    associated color
+    """
+
+    SUCCESS: str = "green"
+    FAILURE: str = "red"
+    INFO: str = "blue"
+
+
+def _echo(message: str, status: MessageStatus):
+    click.echo(click.style(message, fg=status.value), err=True)
+
+
+def success(message: str):
+    """Echos a message in green"""
+    _echo(message, MessageStatus.SUCCESS)
+
+
+def failure(message: str):
+    """Echos a message in red"""
+    _echo(message, MessageStatus.FAILURE)
+
+
+def info(message: str):
+    """Echos a message in blue"""
+    _echo(message, MessageStatus.INFO)
+
+
+def assert_environ_exists(storage_type: str, keys: dict):
+    """Checks that environment variables that are required to use the modelstore CLI
+    are set. If not, logs the failure and exits."""
+    missing_required_keys = [k for k in keys.get("required", []) if k not in os.environ]
+    missing_optional_keys = [k for k in keys.get("optional", []) if k not in os.environ]
+    if len(missing_required_keys) != 0:
+        failure(
+            f"❌ Failed to create {storage_type} modelstore.\nYour environment is missing:"
+        )
+        for k in missing_required_keys:
+            failure(f"- {k} (required)")
+        for k in missing_optional_keys:
+            failure(f"- {k} (optional)")
+        sys.exit(1)
+
+
+def model_store_from_env() -> ModelStore:
+    """Builds a modelstore instance from environment variables."""
+    if "MODEL_STORE_STORAGE" not in os.environ:
+        failure("❌  No value for MODEL_STORE_STORAGE set in os.environ")
+        sys.exit(1)
+
+    storage_name = os.environ["MODEL_STORE_STORAGE"]
+    if storage_name not in STORAGE_TYPES:
+        failure(f"❌  Unknown storage name in MODEL_STORE_STORAGE: {storage_name}")
+        sys.exit(1)
+
+    storage_type = STORAGE_TYPES[storage_name]
+    assert_environ_exists(storage_name, storage_type.BUILD_FROM_ENVIRONMENT)
+    info(f"Using model store with storage={storage_name}")
+    return MODEL_STORE_TYPES[storage_name]()
```

### Comparing `modelstore-0.0.80/modelstore/__main__.py` & `modelstore-0.0.81/tests/test_model_store_filesystem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,97 @@
-#    Copyright 2021 Neal Lathia
+#    Copyright 2022 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
+import shutil
+from pathlib import PosixPath
 
-import click
+import pytest
+from mock import patch
 
-from modelstore.utils import cli as modelstorecli
-
-
-@click.group()
-def download_model():
-    pass
-
-
-@click.group()
-def upload_model():
-    pass
-
-
-@download_model.command()
-@click.argument("domain", type=str, required=True)
-@click.argument("model_id", type=str, required=True)
-@click.argument("parent_dir", type=str, required=False, default=None)
-def download(domain: str, model_id: str, parent_dir: str):
-    """Download a model from the modelstore. Usage:\n
-    ❯ python -m modelstore download <domain> <model-id> <parent-directory>
-    """
-    try:
-        target_dir = (
-            os.path.join(parent_dir, domain, model_id)
-            if parent_dir is not None
-            else os.path.join(domain, model_id)
+from modelstore.model_store import ModelStore
+from modelstore.models.managers import _LIBRARIES
+from modelstore.storage.local import FileSystemStorage
+from modelstore.utils.exceptions import (
+    DomainNotFoundException,
+    ModelNotFoundException
+)
+# pylint: disable=unused-import
+from tests.test_utils import (
+    iter_only_sklearn,
+    libraries_without_sklearn,
+    model_file,
+    validate_library_attributes
+)
+
+# pylint: disable=missing-function-docstring
+
+
+@pytest.mark.parametrize(
+    "should_create",
+    [
+        True,
+        False,
+    ],
+)
+def test_from_file_system_existing_root(tmp_path: PosixPath, should_create: bool):
+    store = ModelStore.from_file_system(
+        root_directory=str(tmp_path), create_directory=should_create
+    )
+    assert isinstance(store.storage, FileSystemStorage)
+    validate_library_attributes(store, allowed=_LIBRARIES , not_allowed=[])
+
+
+@pytest.mark.parametrize(
+    "should_create",
+    [
+        True,
+        False,
+    ],
+)
+def test_from_file_system_missing_root(tmp_path: PosixPath, should_create: bool):
+    root_directory = os.path.join(tmp_path, "unit-test")
+    assert not os.path.exists(root_directory)
+    if should_create:
+        store = ModelStore.from_file_system(
+            root_directory=root_directory, create_directory=should_create
         )
-        os.makedirs(target_dir, exist_ok=True)
-
-        model_store = modelstorecli.model_store_from_env()
-        archive_path = model_store.download(target_dir, domain, model_id)
-        modelstorecli.success(f"✅  Downloaded: {domain}={model_id} to {archive_path}")
-    except Exception:
-        modelstorecli.failure("❌  Failed to download model:")
-        raise
-
-
-@upload_model.command()
-@click.argument("domain", type=str, required=True)
-@click.argument("model", type=click.Path(exists=True))
-def upload(domain: str, model: str):
-    """Upload a model to the modelstore. Usage:\n
-    ❯ python -m modelstore upload <domain> /path/to/file
-    """
-    try:
-        model_store = modelstorecli.model_store_from_env()
-        meta_data = model_store.upload(domain, model=model)
-        model_id = meta_data["model"]["model_id"]
-        modelstorecli.success(f"✅  Uploaded: {domain}={model_id}")
-        print(model_id)
-    except SystemExit:
-        # Failed to instantiate a model store from environment variables
-        pass
-    except Exception:
-        modelstorecli.failure("❌  Failed to upload model:")
-        raise
-
-
-cli = click.CommandCollection(sources=[download_model, upload_model])
-
-if __name__ == "__main__":
-    cli()
+        assert os.path.exists(root_directory)
+        assert os.path.isdir(root_directory)
+        assert isinstance(store.storage, FileSystemStorage)
+        validate_library_attributes(store, allowed=_LIBRARIES, not_allowed=[])
+        # Clean up
+        shutil.rmtree(root_directory)
+    else:
+        with pytest.raises(Exception):
+            _ = ModelStore.from_file_system(
+                root_directory=root_directory, create_directory=should_create
+            )
+
+
+@patch("modelstore.model_store.iter_libraries", side_effect=iter_only_sklearn)
+def test_from_file_system_only_sklearn(_mock_iter_libraries, tmp_path):
+    store = ModelStore.from_file_system(root_directory=str(tmp_path))
+    assert isinstance(store.storage, FileSystemStorage)
+    validate_library_attributes(
+        store, allowed=["sklearn"], not_allowed=libraries_without_sklearn()
+    )
+
+
+def test_model_not_found(tmp_path: PosixPath, model_file: str):
+    store = ModelStore.from_file_system(root_directory=str(tmp_path))
+    with pytest.raises(DomainNotFoundException):
+        store.get_model_info("missing-domain", "missing-model")
+
+    store.upload(domain="existing-domain", model_id="test-model-id-1", model=model_file)
+    with pytest.raises(ModelNotFoundException):
+        store.get_model_info("existing-domain", "missing-model")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `modelstore-0.0.80/modelstore/ids/model_ids.py` & `modelstore-0.0.81/modelstore/ids/model_ids.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/code/code.py` & `modelstore-0.0.81/modelstore/metadata/code/code.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/code/dependencies.py` & `modelstore-0.0.81/modelstore/metadata/code/dependencies.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/code/revision.py` & `modelstore-0.0.81/modelstore/metadata/code/revision.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/code/runtime.py` & `modelstore-0.0.81/modelstore/metadata/code/runtime.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/dataset/dataset.py` & `modelstore-0.0.81/modelstore/metadata/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/dataset/features.py` & `modelstore-0.0.81/modelstore/metadata/dataset/features.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/dataset/labels.py` & `modelstore-0.0.81/modelstore/metadata/dataset/labels.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/dataset/types.py` & `modelstore-0.0.81/modelstore/metadata/dataset/types.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/metadata.py` & `modelstore-0.0.81/modelstore/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/model/model.py` & `modelstore-0.0.81/modelstore/metadata/model/model.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/model/model_type.py` & `modelstore-0.0.81/modelstore/metadata/model/model_type.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/storage/storage.py` & `modelstore-0.0.81/modelstore/metadata/storage/storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/metadata/utils/utils.py` & `modelstore-0.0.81/modelstore/metadata/utils/utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/model_store.py` & `modelstore-0.0.81/modelstore/model_store.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/annoy.py` & `modelstore-0.0.81/modelstore/models/onnx.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2020 Neal Lathia
+#    Copyright 2021 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,78 +16,76 @@
 from typing import Any
 
 from modelstore.metadata import metadata
 from modelstore.models.model_manager import ModelManager
 from modelstore.storage.storage import CloudStorage
 from modelstore.utils.log import logger
 
-MODEL_FILE = "model.ann"
+MODEL_FILE = "model.onnx"
 
 
-class AnnoyManager(ModelManager):
+class OnnxManager(ModelManager):
 
     """
-    Model persistence for Annoy models:
-    https://github.com/spotify/annoy
+    Model persistence for ONNX models:
+    https://github.com/onnx/onnx/blob/master/docs/PythonAPIOverview.md
     """
 
-    NAME = "annoy"
+    NAME = "onnx"
 
     def __init__(self, storage: CloudStorage = None):
         super().__init__(self.NAME, storage)
 
     def required_dependencies(self) -> list:
-        return ["annoy"]
+        return ["onnx"]
+
+    def optional_dependencies(self) -> list:
+        return super().optional_dependencies() + [
+            "skl2onnx",
+            "onnxmltools",
+            "onnxruntime",
+            "onnxconverter-common",
+        ]
 
     def _required_kwargs(self):
-        return ["model", "metric", "num_trees"]
+        return ["model"]
 
     def matches_with(self, **kwargs) -> bool:
         # pylint: disable=import-outside-toplevel
-        from annoy import AnnoyIndex
+        from onnx import ModelProto
 
-        return isinstance(kwargs.get("model"), AnnoyIndex)
+        return isinstance(kwargs.get("model"), ModelProto)
 
     def _get_functions(self, **kwargs) -> list:
         if not self.matches_with(**kwargs):
-            raise TypeError("Model is not an AnnoyIndex!")
+            raise TypeError("Model is not an onnx.ModelProto!")
 
         return [
             partial(
                 save_model,
                 model=kwargs["model"],
             ),
         ]
 
-    def get_params(self, **kwargs) -> dict:
-        return {
-            "num_dimensions": kwargs["model"].f,
-            "num_trees": kwargs["num_trees"],
-            "metric": kwargs["metric"],
-        }
-
     def load(self, model_path: str, meta_data: metadata.Summary) -> Any:
         super().load(model_path, meta_data)
 
         # pylint: disable=import-outside-toplevel
-        from annoy import AnnoyIndex
+        import onnxruntime as rt
 
-        # Extract index size & metric from the meta_data
-        params = meta_data.model.parameters
-        num_dimensions = int(params["num_dimensions"])
-        metric = params["metric"]
-
-        model = AnnoyIndex(num_dimensions, metric)
-        model.load(_model_file_path(model_path))
-        return model
+        model_path = _model_file_path(model_path)
+        with open(model_path, "rb") as lines:
+            model = lines.read()
+        return rt.InferenceSession(model)
 
 
 def _model_file_path(tmp_dir: str) -> str:
     return os.path.join(tmp_dir, MODEL_FILE)
 
 
-def save_model(tmp_dir: str, model: "annoy.AnnoyIndex") -> str:
-    """Saves an annoy index to file"""
+def save_model(tmp_dir: str, model: "onnx.ModelProto") -> str:
+    """Saves the onnx model in tmp_dir"""
     file_path = _model_file_path(tmp_dir)
-    logger.debug("Saving annoy model to %s", file_path)
-    model.save(file_path)
+    logger.debug("Saving onnx model to %s", file_path)
+    with open(file_path, "wb") as model_file:
+        model_file.write(model.SerializeToString())
     return file_path
```

### Comparing `modelstore-0.0.80/modelstore/models/catboost.py` & `modelstore-0.0.81/modelstore/models/catboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/fastai.py` & `modelstore-0.0.81/modelstore/models/fastai.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/gensim.py` & `modelstore-0.0.81/modelstore/models/gensim.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/lightgbm.py` & `modelstore-0.0.81/modelstore/models/lightgbm.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/managers.py` & `modelstore-0.0.81/modelstore/models/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 from typing import Iterator, List
 
 from modelstore.metadata.code.dependencies import module_exists
 from modelstore.models.annoy import AnnoyManager
 from modelstore.models.catboost import CatBoostManager
+from modelstore.models.causalml import CausalMLManager
 from modelstore.models.fastai import FastAIManager
 from modelstore.models.gensim import GensimManager
 from modelstore.models.lightgbm import LightGbmManager
 from modelstore.models.missing_manager import MissingDepManager
 from modelstore.models.model_file import ModelFileManager
 from modelstore.models.model_manager import ModelManager
-from modelstore.models.mxnet import MxnetManager
 from modelstore.models.onnx import OnnxManager
 from modelstore.models.prophet import ProphetManager
 from modelstore.models.pyspark import PySparkManager
 from modelstore.models.pytorch import PyTorchManager
 from modelstore.models.pytorch_lightning import PyTorchLightningManager
 from modelstore.models.shap import ShapManager
 from modelstore.models.sklearn import SKLearnManager
@@ -38,19 +38,19 @@
 from modelstore.utils.log import logger
 
 _LIBRARIES = {
     m.NAME: m
     for m in [
         AnnoyManager,
         CatBoostManager,
+        CausalMLManager,
         FastAIManager,
         ModelFileManager,
         GensimManager,
         LightGbmManager,
-        MxnetManager,
         OnnxManager,
         ProphetManager,
         PySparkManager,
         PyTorchManager,
         PyTorchLightningManager,
         ShapManager,
         SKLearnManager,
@@ -91,10 +91,11 @@
     if name == "keras":
         # Older versions of modelstore (before 0.0.73) had separate
         # managers for Keras and Tensorflow. Setting this explicitly
         # here ensures that modelstore remains backward compatible
         manager = TensorflowManager(storage)
     else:
         manager = _LIBRARIES[name](storage)
-    if all(module_exists(x) for x in manager.required_dependencies()):
-        return manager
-    raise ValueError(f"could not create manager for {name}: dependencies not installed")
+    for x in manager.required_dependencies():
+        if not module_exists(x):
+            raise ValueError(f"could not create manager for {name}: {x} not installed")
+    return manager
```

### Comparing `modelstore-0.0.80/modelstore/models/missing_manager.py` & `modelstore-0.0.81/modelstore/models/missing_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/model_file.py` & `modelstore-0.0.81/modelstore/models/model_file.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/model_manager.py` & `modelstore-0.0.81/modelstore/models/model_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/multiple_models.py` & `modelstore-0.0.81/modelstore/models/multiple_models.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/mxnet.py` & `modelstore-0.0.81/modelstore/models/prophet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,102 @@
-#    Copyright 2021 Neal Lathia
+#    Copyright 2020 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
+import json
 import os
 from functools import partial
 from typing import Any
 
 from modelstore.metadata import metadata
 from modelstore.models.model_manager import ModelManager
 from modelstore.storage.storage import CloudStorage
+from modelstore.utils.log import logger
 
-MODEL_FILE = "model-symbol.json"
-PARAMS_FILE = "model-{}.params"
+MODEL_FILE = "prophet_model.json"
 
 
-class MxnetManager(ModelManager):
+class ProphetManager(ModelManager):
 
     """
-    Model persistence for Mxnet (Hybrid) Gluon models
-    https://mxnet.apache.org/versions/1.8.0/api/python/docs/tutorials/packages/gluon/blocks/save_load_params.html
+    Model persistence for Prophet models:
+    https://facebook.github.io/prophet/docs/additional_topics.html#saving-models
     """
 
-    NAME = "mxnet"
+    NAME = "prophet"
 
     def __init__(self, storage: CloudStorage = None):
         super().__init__(self.NAME, storage)
 
     def required_dependencies(self) -> list:
-        return ["mxnet"]
+        return ["prophet"]
 
     def optional_dependencies(self) -> list:
-        return super().optional_dependencies() + ["onnx"]
+        return super().optional_dependencies() + ["pystan"]
 
     def _required_kwargs(self):
-        return ["model", "epoch"]
+        return ["model"]
 
     def matches_with(self, **kwargs) -> bool:
         # pylint: disable=import-outside-toplevel
-        from mxnet.gluon import nn
+        from prophet import Prophet
 
-        # Using nn.HybridBlock instead of nn.Block because Hybrid
-        # blocks can be exported
-        return isinstance(kwargs.get("model"), nn.HybridBlock)
+        return isinstance(kwargs.get("model"), Prophet)
 
     def _get_functions(self, **kwargs) -> list:
         if not self.matches_with(**kwargs):
-            raise TypeError("Model is not an mxnet nn.HybridBlock!")
-        if "epoch" not in kwargs:
-            raise ValueError("Mxnet uploads require the 'epoch' kwarg to be set.")
+            raise TypeError("Model is not a Prophet model!")
 
         return [
             partial(
                 save_model,
                 model=kwargs["model"],
-                epoch=kwargs["epoch"],
             ),
         ]
 
     def get_params(self, **kwargs) -> dict:
-        return {
-            "epoch": kwargs["epoch"],
-        }
+        """
+        Reference:
+        https://facebook.github.io/prophet/docs/additional_topics.html#updating-fitted-models
+        """
+        model = kwargs["model"]
+        params = {}
+        for pname in ["k", "m", "sigma_obs"]:
+            params[pname] = model.params[pname][0][0]
+        for pname in ["delta", "beta", "trend"]:
+            params[pname] = model.params[pname][0].tolist()
+        return params
 
     def load(self, model_path: str, meta_data: metadata.Summary) -> Any:
         super().load(model_path, meta_data)
 
         # pylint: disable=import-outside-toplevel
-        from mxnet.gluon import SymbolBlock
+        from prophet.serialize import model_from_json
 
-        epoch = int(meta_data.model.parameters["epoch"])
-        return SymbolBlock.imports(
-            model_file_path(model_path),
-            ["data"],
-            params_file_path(model_path, epoch),
-        )
-
-
-def model_file_path(parent_dir: str) -> str:
-    """Returns the path to the model file in parent_dir"""
-    return os.path.join(parent_dir, MODEL_FILE)
-
-
-def params_file_path(parent_dir: str, epoch: int) -> str:
-    """Returns the path to the params file for #epoch in parent_dir"""
-    return os.path.join(parent_dir, PARAMS_FILE.format(f"{epoch:04d}"))
-
-
-def save_model(tmp_dir: str, model: "nn.HybridBlock", epoch: int) -> str:
-    """Saves the model in tmp_dir"""
-
-    # model.export() stores files in the current directory, so we chdir()
-    # to the target directory where we want the files saved
-    cwd = os.getcwd()
-    os.chdir(tmp_dir)
-    # Two files path-symbol.json and path-xxxx.params will be created,
-    # where xxxx is the 4 digits epoch number, in the current directory
-    model.export("model", epoch=epoch)
-    # Go back to the previous working directory
-    os.chdir(cwd)
-    return [
-        model_file_path(tmp_dir),
-        params_file_path(tmp_dir, epoch),
-    ]
+        file_path = _model_file_path(model_path)
+        with open(file_path, "r") as fin:
+            m_json = json.load(fin)
+        return model_from_json(m_json)
+
+
+def _model_file_path(tmp_dir: str) -> str:
+    return os.path.join(tmp_dir, MODEL_FILE)
+
+
+def save_model(tmp_dir: str, model: "prophet.Prophet") -> str:
+    # pylint: disable=import-outside-toplevel
+    from prophet.serialize import model_to_json
+
+    file_path = _model_file_path(tmp_dir)
+    logger.debug("Saving prophet model to %s", file_path)
+    with open(file_path, "w") as fout:
+        fout.write(json.dumps(model_to_json(model)))
+    return file_path
```

### Comparing `modelstore-0.0.80/modelstore/models/onnx.py` & `modelstore-0.0.81/modelstore/models/causalml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#    Copyright 2021 Neal Lathia
+#    Copyright 2024 Neal Lathia
 #
 #    Licensed under the Apache License, Version 2.0 (the "License");
 #    you may not use this file except in compliance with the License.
 #    You may obtain a copy of the License at
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,80 +12,60 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
 from functools import partial
 from typing import Any
 
 from modelstore.metadata import metadata
+from modelstore.models.common import load_joblib, save_joblib
 from modelstore.models.model_manager import ModelManager
 from modelstore.storage.storage import CloudStorage
-from modelstore.utils.log import logger
 
-MODEL_FILE = "model.onnx"
+MODEL_FILE = "model.joblib"
 
 
-class OnnxManager(ModelManager):
+class CausalMLManager(ModelManager):
 
     """
-    Model persistence for ONNX models:
-    https://github.com/onnx/onnx/blob/master/docs/PythonAPIOverview.md
+    Model persistence for Causal ML models:
+    https://causalml.readthedocs.io/en/latest/index.html
     """
 
-    NAME = "onnx"
+    NAME = "causalml"
 
     def __init__(self, storage: CloudStorage = None):
         super().__init__(self.NAME, storage)
 
     def required_dependencies(self) -> list:
-        return ["onnx"]
+        return ["causalml"]
 
     def optional_dependencies(self) -> list:
-        return super().optional_dependencies() + [
-            "skl2onnx",
-            "onnxmltools",
-            "onnxruntime",
-            "onnxconverter-common",
-        ]
+        deps = super().optional_dependencies()
+        return deps + ["Cython", "joblib"]
 
     def _required_kwargs(self):
         return ["model"]
 
     def matches_with(self, **kwargs) -> bool:
         # pylint: disable=import-outside-toplevel
-        from onnx import ModelProto
+        import causalml
 
-        return isinstance(kwargs.get("model"), ModelProto)
+        return any(
+            [
+                isinstance(kwargs.get("model"), causalml.inference.meta.base.BaseLearner),
+                isinstance(kwargs.get("model"), causalml.propensity.PropensityModel),
+            ]
+        )
 
     def _get_functions(self, **kwargs) -> list:
         if not self.matches_with(**kwargs):
-            raise TypeError("Model is not an onnx.ModelProto!")
+            raise TypeError("This model is not a Causal ML model!")
 
-        return [
-            partial(
-                save_model,
-                model=kwargs["model"],
-            ),
-        ]
+        return [partial(save_joblib, model=kwargs["model"], file_name=MODEL_FILE)]
 
     def load(self, model_path: str, meta_data: metadata.Summary) -> Any:
         super().load(model_path, meta_data)
 
-        # pylint: disable=import-outside-toplevel
-        import onnxruntime as rt
-
-        model_path = _model_file_path(model_path)
-        with open(model_path, "rb") as lines:
-            model = lines.read()
-        return rt.InferenceSession(model)
-
-
-def _model_file_path(tmp_dir: str) -> str:
-    return os.path.join(tmp_dir, MODEL_FILE)
-
-
-def save_model(tmp_dir: str, model: "onnx.ModelProto") -> str:
-    """Saves the onnx model in tmp_dir"""
-    file_path = _model_file_path(tmp_dir)
-    logger.debug("Saving onnx model to %s", file_path)
-    with open(file_path, "wb") as model_file:
-        model_file.write(model.SerializeToString())
-    return file_path
+        # @Future: check if loading into same version of joblib
+        # as was used for saving
+        file_name = os.path.join(model_path, MODEL_FILE)
+        return load_joblib(file_name)
```

### Comparing `modelstore-0.0.80/modelstore/models/pyspark.py` & `modelstore-0.0.81/modelstore/models/pyspark.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/pytorch.py` & `modelstore-0.0.81/modelstore/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/pytorch_lightning.py` & `modelstore-0.0.81/modelstore/models/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/shap.py` & `modelstore-0.0.81/modelstore/models/shap.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/sklearn.py` & `modelstore-0.0.81/modelstore/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/skorch.py` & `modelstore-0.0.81/modelstore/models/skorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/transformers.py` & `modelstore-0.0.81/modelstore/models/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,15 @@
         if "preprocessor_config.json" in model_files:
             from transformers import AutoProcessor
 
             processor = AutoProcessor.from_pretrained(model_dir)
             logger.debug("Loaded: %s...", type(processor))
 
         # Infer whether we're loading a PyTorch or Tensorflow model
+        # @TODO: this does not appear to hold with more recent versions of transformers
         is_pytorch = "pytorch_model.bin" in model_files
         logger.debug("Loading transformers model with pytorch=%s", is_pytorch)
 
         if is_pytorch:
             from transformers import AutoModel, GPT2LMHeadModel
 
             # In examples-by-ml-library/libraries/huggingface/gpt2*.py, we want
```

### Comparing `modelstore-0.0.80/modelstore/models/util.py` & `modelstore-0.0.81/modelstore/models/util.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/models/xgboost.py` & `modelstore-0.0.81/modelstore/models/xgboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/aws.py` & `modelstore-0.0.81/modelstore/storage/aws.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/azure.py` & `modelstore-0.0.81/modelstore/storage/azure.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/blob_storage.py` & `modelstore-0.0.81/modelstore/storage/blob_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/gcloud.py` & `modelstore-0.0.81/modelstore/storage/gcloud.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/hdfs.py` & `modelstore-0.0.81/modelstore/storage/hdfs.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/local.py` & `modelstore-0.0.81/modelstore/storage/local.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/minio.py` & `modelstore-0.0.81/modelstore/storage/minio.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/states/model_states.py` & `modelstore-0.0.81/modelstore/storage/states/model_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/storage.py` & `modelstore-0.0.81/modelstore/storage/storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/util/environment.py` & `modelstore-0.0.81/modelstore/storage/util/environment.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/util/paths.py` & `modelstore-0.0.81/modelstore/storage/util/paths.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/storage/util/versions.py` & `modelstore-0.0.81/modelstore/storage/util/versions.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/utils/exceptions.py` & `modelstore-0.0.81/modelstore/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/modelstore/utils/log.py` & `modelstore-0.0.81/modelstore/utils/log.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,20 +10,29 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import logging
 import sys
 
-
 def get_logger():
     """Builds the modelstore logger"""
     log = logging.getLogger(name="modelstore")
     formatter = logging.Formatter("%(asctime)s - %(message)s")
     handler = logging.StreamHandler(sys.stderr)
     handler.setFormatter(formatter)
     log.setLevel(logging.INFO)
     log.addHandler(handler)
     return log
 
 
 logger = get_logger()
+
+
+def debug_mode(on: bool):
+    global logger
+    logger = get_logger()
+    if not on:
+        return
+    logger.setLevel(logging.DEBUG)
+    for handler in logger.handlers:
+        handler.setLevel(logging.DEBUG)
```

### Comparing `modelstore-0.0.80/modelstore.egg-info/PKG-INFO` & `modelstore-0.0.81/modelstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelstore
-Version: 0.0.80
+Version: 0.0.81
 Summary: modelstore is a library for versioning, exporting, storing, and loading machine learning models
 Home-page: https://github.com/operatorai/modelstore
 Author: Neal Lathia
 License: Please refer to the readme
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `modelstore-0.0.80/setup.py` & `modelstore-0.0.81/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # pylint: disable=unspecified-encoding
 with open("requirements.txt", "r") as lines:
     requirements = lines.read().splitlines()
 
 
 setup(
     name="modelstore",
-    version="0.0.80",
+    version="0.0.81",
     packages=find_packages(exclude=["tests", "examples", "docs", "workflows"]),
     include_package_data=True,
     description="modelstore is a library for versioning, exporting, storing, and loading machine learning models",
     long_description="Please refer to: https://modelstore.readthedocs.io/en/latest/",
     long_description_content_type="text/markdown",
     url="https://github.com/operatorai/modelstore",
     author="Neal Lathia",
```

### Comparing `modelstore-0.0.80/tests/ids/test_model_ids.py` & `modelstore-0.0.81/tests/ids/test_model_ids.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/code/test_code.py` & `modelstore-0.0.81/tests/metadata/code/test_code.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/code/test_dependencies.py` & `modelstore-0.0.81/tests/metadata/code/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/code/test_revision.py` & `modelstore-0.0.81/tests/metadata/code/test_revision.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,24 +8,26 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
+import sys
 import subprocess
 
 import git
 import pytest
 
 from modelstore.metadata.code import revision
 
 # pylint: disable=missing-function-docstring
 
 
+@pytest.mark.skipif(sys.platform!="darwin", reason="skipping in ubuntu")
 def test_repo_name():
     # pylint: disable=protected-access
     repo = git.Repo(search_parent_directories=True)
     repo_name = revision._repo_name(repo)
     if repo_name == "":
         # Not a git repo
         return
```

### Comparing `modelstore-0.0.80/tests/metadata/code/test_runtime.py` & `modelstore-0.0.81/tests/metadata/code/test_runtime.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/dataset/fixtures.py` & `modelstore-0.0.81/tests/metadata/dataset/fixtures.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/dataset/test_dataset.py` & `modelstore-0.0.81/tests/metadata/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/dataset/test_features.py` & `modelstore-0.0.81/tests/metadata/dataset/test_features.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/dataset/test_labels.py` & `modelstore-0.0.81/tests/metadata/dataset/test_labels.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/dataset/test_types.py` & `modelstore-0.0.81/tests/metadata/dataset/test_types.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/model/test_model.py` & `modelstore-0.0.81/tests/metadata/model/test_model.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/model/test_model_type.py` & `modelstore-0.0.81/tests/metadata/model/test_model_type.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/storage/test_storage.py` & `modelstore-0.0.81/tests/metadata/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/test_metadata.py` & `modelstore-0.0.81/tests/metadata/test_metadata.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/metadata/utils/test_utils.py` & `modelstore-0.0.81/tests/metadata/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_annoy.py` & `modelstore-0.0.81/tests/models/test_annoy.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_catboost.py` & `modelstore-0.0.81/tests/models/test_catboost.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_common.py` & `modelstore-0.0.81/tests/models/test_common.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_fastai.py` & `modelstore-0.0.81/tests/models/test_fastai.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_gensim.py` & `modelstore-0.0.81/tests/models/test_gensim.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_lightgbm.py` & `modelstore-0.0.81/tests/models/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_managers.py` & `modelstore-0.0.81/tests/models/test_managers.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_missing_manager.py` & `modelstore-0.0.81/tests/models/test_missing_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_model_file.py` & `modelstore-0.0.81/tests/models/test_model_file.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_model_manager.py` & `modelstore-0.0.81/tests/models/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_multiple_models.py` & `modelstore-0.0.81/tests/models/test_multiple_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     expected = metadata.ModelType(
         library="multiple-models",
         type=None,
         models=[
             metadata.ModelType(
                 SKLearnManager.NAME, "RandomForestRegressor", models=None
             ),
-            metadata.ModelType(ShapManager.NAME, "Tree", models=None),
+            metadata.ModelType(ShapManager.NAME, "TreeExplainer", models=None),
         ],
     )
     res = multiple_model_manager.model_info(
         model=sklearn_tree,
         explainer=shap_explainer,
     )
     assert res == expected
```

### Comparing `modelstore-0.0.80/tests/models/test_onnx.py` & `modelstore-0.0.81/tests/models/test_onnx.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_prophet.py` & `modelstore-0.0.81/tests/models/test_prophet.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_pyspark.py` & `modelstore-0.0.81/tests/models/test_pyspark.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_pytorch.py` & `modelstore-0.0.81/tests/models/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_pytorch_lightning.py` & `modelstore-0.0.81/tests/models/test_pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_shap.py` & `modelstore-0.0.81/tests/models/test_shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 @pytest.fixture
 def shap_manager():
     return shap.ShapManager()
 
 
 def test_model_info(shap_manager, shap_explainer):
-    exp = metadata.ModelType("shap", "Tree", None)
+    exp = metadata.ModelType("shap", "TreeExplainer", None)
     res = shap_manager.model_info(explainer=shap_explainer)
     assert exp == res
 
 
 def test_model_data(shap_manager, shap_explainer):
     res = shap_manager.model_data(explainer=shap_explainer)
     assert res is None
```

### Comparing `modelstore-0.0.80/tests/models/test_sklearn.py` & `modelstore-0.0.81/tests/models/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_skorch.py` & `modelstore-0.0.81/tests/models/test_skorch.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/models/test_tensorflow.py` & `modelstore-0.0.81/tests/models/test_tensorflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from modelstore.metadata import metadata
 from modelstore.metadata.dataset.dataset import Features, Labels
 from modelstore.models.tensorflow import (
     MODEL_DIRECTORY,
     TensorflowManager,
     _save_model,
     _save_weights,
-    save_json
+    save_json,
+    _is_tensorflow_using_keras3_api,
 )
 
 # pylint: disable=protected-access
 # pylint: disable=redefined-outer-name
 # pylint: disable=missing-function-docstring
 tf.config.threading.set_inter_op_parallelism_threads(1)
 
@@ -101,23 +102,25 @@
 
 def test_get_params(tf_manager, tf_model):
     exp = tf_model.optimizer.get_config()
     res = tf_manager.get_params(model=tf_model)
     assert exp == res
 
 
+@pytest.mark.skipif(_is_tensorflow_using_keras3_api(), reason="Testing behaviour for Keras < 3.0")
 def test_save_model(tmp_path, tf_model):
     exp = os.path.join(tmp_path, "model")
     model_path = _save_model(tmp_path, tf_model)
     assert exp == model_path
     assert os.path.isdir(model_path)
     loaded_model = tf.keras.models.load_model(model_path)
     assert_models_equal(tf_model, loaded_model)
 
 
+@pytest.mark.skipif(_is_tensorflow_using_keras3_api(), reason="Testing behaviour for Keras < 3.0")
 def test_save_weights(tf_model, tmp_path):
     exp = os.path.join(tmp_path, "checkpoint")
     file_path = _save_weights(tmp_path, model=tf_model)
     assert file_path == exp
     assert os.path.isfile(file_path)
 
     loaded_model = tf.keras.models.Sequential(
@@ -127,27 +130,57 @@
             tf.keras.layers.Dense(1),
         ]
     )
     loaded_model.load_weights(file_path).expect_partial()
     assert_models_equal(tf_model, loaded_model)
 
 
+@pytest.mark.skipif(not _is_tensorflow_using_keras3_api(), reason="Testing behaviour for Keras >= 3.0")
+def test_save_model_keras_3_api(tmp_path, tf_model):
+    exp = f"{os.path.join(tmp_path, 'model')}.keras"
+    model_path = _save_model(tmp_path, tf_model)
+    assert exp == model_path
+    loaded_model = tf.keras.models.load_model(model_path)
+    assert_models_equal(tf_model, loaded_model)
+
+
+@pytest.mark.skipif(not _is_tensorflow_using_keras3_api(), reason="Testing behaviour for Keras >= 3.0")
+def test_save_weights_keras_3_api(tf_model, tmp_path):
+    exp = f"{os.path.join(tmp_path, 'checkpoint')}.weights.h5"
+    file_path = _save_weights(tmp_path, model=tf_model)
+    assert file_path == exp
+    assert os.path.isfile(file_path)
+
+    loaded_model = tf.keras.models.Sequential(
+        [
+            tf.keras.layers.Dense(5, activation="relu", input_shape=(10,)),
+            tf.keras.layers.Dropout(0.2),
+            tf.keras.layers.Dense(1),
+        ]
+    )
+    loaded_model.load_weights(file_path)
+    assert_models_equal(tf_model, loaded_model)
+
+
 def test_model_json(tf_model, tmp_path):
     exp = os.path.join(tmp_path, "model_config.json")
     file_path = save_json(tmp_path, "model_config.json", tf_model.to_json())
     assert file_path == exp
     with open(file_path, "r") as lines:
         model_json = json.loads(lines.read())
     model = tf.keras.models.model_from_json(model_json)
     assert_models_equal(model, tf_model, assert_predictions=False)
 
 
 def test_load_model(tmp_path, tf_manager, tf_model):
     # Save the model to a tmp directory
     model_path = os.path.join(tmp_path, MODEL_DIRECTORY)
+    if _is_tensorflow_using_keras3_api():
+        model_path = f"{model_path}.keras"
+
     tf_model.save(model_path)
 
     #  Load the model
     loaded_model = tf_manager.load(tmp_path, None)
 
     # Expect the two to be the same
     assert_models_equal(tf_model, loaded_model)
```

### Comparing `modelstore-0.0.80/tests/models/test_transformers.py` & `modelstore-0.0.81/tests/models/test_transformers.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-import json
 import os
 
 import pytest
 from transformers import (
     AutoConfig,
     AutoModelForSequenceClassification,
     AutoTokenizer,
     DistilBertForSequenceClassification,
-    DistilBertModel,
+    TFDistilBertModel,
     DistilBertTokenizerFast,
     PreTrainedTokenizerFast
 )
-from transformers.file_utils import CONFIG_NAME
 
 from modelstore.metadata import metadata
 from modelstore.models.transformers import (
     MODEL_DIRECTORY,
     TransformersManager,
     _save_transformers
 )
@@ -115,21 +113,14 @@
 def test_save_transformers(tr_config, tr_model, tr_tokenizer, tmp_path):
     exp = os.path.join(tmp_path, "transformers")
     file_path = _save_transformers(
         tmp_path, entities=[tr_config, tr_model, tr_tokenizer]
     )
     assert exp == file_path
 
-    # Validate config
-    config_file = os.path.join(exp, CONFIG_NAME)
-    assert os.path.exists(config_file)
-    with open(config_file, "r") as lines:
-        config_json = json.loads(lines.read())
-    assert config_json == json.loads(tr_config.to_json_string())
-
     # Validate model
     model = AutoModelForSequenceClassification.from_pretrained(
         exp,
         config=tr_config,
     )
     assert isinstance(model, DistilBertForSequenceClassification)
 
@@ -161,10 +152,10 @@
         code=None,
         storage=None,
         modelstore=None,
     )
     loaded_model, loaded_tokenizer, loaded_config = tr_manager.load(tmp_path, meta_data)
 
     # Expect the two to be the same
-    assert isinstance(loaded_model, DistilBertModel)
+    assert isinstance(loaded_model, TFDistilBertModel)
     assert isinstance(loaded_config, type(tr_config))
     assert isinstance(loaded_tokenizer, DistilBertTokenizerFast)
```

### Comparing `modelstore-0.0.80/tests/models/test_xgboost.py` & `modelstore-0.0.81/tests/models/test_xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,20 +153,30 @@
     loaded_model_params = loaded_model.get_params()
     assert_same_xgboost_params(xgb_model_params, loaded_model_params)
 
 
 def assert_same_xgboost_params(a_params: dict, b_params: dict):
     # Some fields in xgboost get_params change when loading
     # or are nans; we cannot compare them in this test
-    ignore_params = ["missing", "tree_method", "use_label_encoder", "n_jobs"]
+    # import pdb; pdb.set_trace()
+    ignore_params = [
+        "missing",
+        "tree_method",
+        "use_label_encoder",
+        "n_jobs",
+        "booster",
+        "base_score"
+    ]
     for param in ignore_params:
         if param in a_params:
             a_params.pop(param)
         if param in b_params:
             b_params.pop(param)
+    for key, param in a_params.items():
+        assert param == b_params[key], f"Params are different for {key}"
     assert a_params == b_params
 
 
 def test_load_booster(tmp_path, xgb_manager, xgb_booster, classification_data):
     # Get the model predictions
     X_train, _ = classification_data
     y_pred = xgb_booster.predict(xgb.DMatrix(X_train))
```

### Comparing `modelstore-0.0.80/tests/models/utils.py` & `modelstore-0.0.81/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/states/test_model_states.py` & `modelstore-0.0.81/tests/storage/states/test_model_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_aws.py` & `modelstore-0.0.81/tests/storage/test_aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 import os
 from tempfile import TemporaryDirectory
 
 import boto3
 import pytest
-from moto import mock_s3
+from moto import mock_aws
 
 from modelstore.metadata import metadata
 from modelstore.storage.aws import AWSStorage
 # pylint: disable=unused-import
 from tests.storage.test_utils import (
     TEST_FILE_CONTENTS,
     TEST_FILE_NAME,
@@ -36,15 +36,15 @@
 # pylint: disable=missing-function-docstring
 
 _MOCK_BUCKET_NAME = "existing-bucket"
 
 
 @pytest.fixture(autouse=True)
 def moto_boto():
-    with mock_s3():
+    with mock_aws():
         conn = boto3.resource("s3")
         conn.create_bucket(Bucket=_MOCK_BUCKET_NAME)
         yield conn
 
 
 def get_file_contents(moto_boto, prefix):
     return (
@@ -177,26 +177,26 @@
 
 
 @pytest.mark.parametrize(
     "meta_data,should_raise,result",
     [
         (
             metadata.Storage(
-                type=None,
+                type="",
                 path=None,
                 bucket=_MOCK_BUCKET_NAME,
                 container=None,
                 prefix="/path/to/file",
             ),
             False,
             "/path/to/file",
         ),
         (
             metadata.Storage(
-                type=None,
+                type="",
                 path=None,
                 bucket="a-different-bucket",
                 container=None,
                 prefix="/path/to/file",
             ),
             True,
             None,
```

### Comparing `modelstore-0.0.80/tests/storage/test_azure.py` & `modelstore-0.0.81/tests/storage/test_azure.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_blob_storage.py` & `modelstore-0.0.81/tests/storage/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_blob_storage_artifacts.py` & `modelstore-0.0.81/tests/storage/test_blob_storage_artifacts.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_blob_storage_meta_data.py` & `modelstore-0.0.81/tests/storage/test_blob_storage_meta_data.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_blob_storage_states.py` & `modelstore-0.0.81/tests/storage/test_blob_storage_states.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_gcloud.py` & `modelstore-0.0.81/tests/storage/test_gcloud.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_hdfs.py` & `modelstore-0.0.81/tests/storage/test_hdfs.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_local.py` & `modelstore-0.0.81/tests/storage/test_local.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_minio.py` & `modelstore-0.0.81/tests/storage/test_minio.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/test_utils.py` & `modelstore-0.0.81/tests/storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/storage/util/test_paths.py` & `modelstore-0.0.81/tests/storage/util/test_paths.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/test_model_store.py` & `modelstore-0.0.81/tests/test_model_store.py`

 * *Files identical despite different names*

### Comparing `modelstore-0.0.80/tests/test_utils.py` & `modelstore-0.0.81/tests/test_utils.py`

 * *Files identical despite different names*

