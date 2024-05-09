# Comparing `tmp/danling-0.3.4.tar.gz` & `tmp/danling-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.3.4.tar", last modified: Wed May  8 06:30:34 2024, max compression
+gzip compressed data, was "danling-0.3.5.tar", last modified: Thu May  9 10:48:18 2024, max compression
```

## Comparing `danling-0.3.4.tar` & `danling-0.3.5.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.961465 danling-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 06:30:31.000000 danling-0.3.4/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-05-08 06:30:31.000000 danling-0.3.4/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-08 06:30:31.000000 danling-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-08 06:30:31.000000 danling-0.3.4/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.AGPL
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.Apache
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.BSD
--rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.GPLv2
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.GPLv3
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-08 06:30:31.000000 danling-0.3.4/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-08 06:30:34.961465 danling-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-08 06:30:31.000000 danling-0.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-08 06:30:31.000000 danling-0.3.4/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.933465 danling-0.3.4/danling/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-08 06:30:31.000000 danling-0.3.4/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 06:30:34.000000 danling-0.3.4/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/average_meters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 06:30:31.000000 danling-0.3.4/danling/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-08 06:30:31.000000 danling-0.3.4/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.937465 danling-0.3.4/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-08 06:30:31.000000 danling-0.3.4/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 06:30:31.000000 danling-0.3.4/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/accelerate_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    43863 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/state.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-08 06:30:31.000000 danling-0.3.4/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    41934 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-08 06:30:31.000000 danling-0.3.4/danling/tensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-08 06:30:31.000000 danling-0.3.4/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-05-08 06:30:31.000000 danling-0.3.4/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.961465 danling-0.3.4/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 06:30:34.000000 danling-0.3.4/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.925465 danling-0.3.4/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/demo/vision/
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-08 06:30:31.000000 danling-0.3.4/demo/vision/torch_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/average_meters.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/metrics/metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.941465 danling-0.3.4/docs/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/package.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/accelerate_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/state.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/contextmanagers.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 06:30:31.000000 danling-0.3.4/docs/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-05-08 06:30:31.000000 danling-0.3.4/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.945465 danling-0.3.4/docs/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/docs/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-08 06:30:31.000000 danling-0.3.4/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-08 06:30:31.000000 danling-0.3.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-08 06:30:31.000000 danling-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 06:30:31.000000 danling-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:30:34.961465 danling-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 06:30:31.000000 danling-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.929465 danling-0.3.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-08 06:30:31.000000 danling-0.3.4/tests/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-08 06:30:31.000000 danling-0.3.4/tests/optim/test_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-08 06:30:31.000000 danling-0.3.4/tests/runner/test_base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-08 06:30:31.000000 danling-0.3.4/tests/runner/test_torch_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-08 06:30:31.000000 danling-0.3.4/tests/tensors/test_nested_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 06:30:34.957466 danling-0.3.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 06:30:31.000000 danling-0.3.4/tests/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 06:30:31.000000 danling-0.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.411428 danling-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 10:48:14.000000 danling-0.3.5/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-09 10:48:14.000000 danling-0.3.5/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-09 10:48:14.000000 danling-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 10:48:14.000000 danling-0.3.5/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.AGPL
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.Apache
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.BSD
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.GPLv2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.GPLv3
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-09 10:48:18.411428 danling-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-09 10:48:14.000000 danling-0.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-09 10:48:14.000000 danling-0.3.5/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/danling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 10:48:14.000000 danling-0.3.5/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 10:48:18.000000 danling-0.3.5/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 10:48:14.000000 danling-0.3.5/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/accelerate_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44104 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44356 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 10:48:14.000000 danling-0.3.5/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/demo/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-09 10:48:14.000000 danling-0.3.5/demo/vision/torch_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/metrics/metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/package.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/accelerate_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/state.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/contextmanagers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-09 10:48:14.000000 danling-0.3.5/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 10:48:14.000000 danling-0.3.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-09 10:48:14.000000 danling-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 10:48:14.000000 danling-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:48:18.411428 danling-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:48:14.000000 danling-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-09 10:48:14.000000 danling-0.3.5/tests/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-09 10:48:14.000000 danling-0.3.5/tests/optim/test_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-09 10:48:14.000000 danling-0.3.5/tests/runner/test_base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-09 10:48:14.000000 danling-0.3.5/tests/runner/test_torch_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-09 10:48:14.000000 danling-0.3.5/tests/tensors/test_nested_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-09 10:48:14.000000 danling-0.3.5/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 10:48:14.000000 danling-0.3.5/tox.ini
```

### Comparing `danling-0.3.4/.github/workflows/push.yaml` & `danling-0.3.5/.github/workflows/push.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         id: pip-cache
         run: echo "::set-output name=dir::$(pip cache dir)"
       - uses: actions/cache@v3
         with:
           key: ${{ github.ref }}
           path: .cache
       - run: pip install -r docs/requirements.txt
+      - run: pip install -e .
       - name: Download coverage report
         uses: actions/download-artifact@v3
         with:
           name: coverage
           path: htmlcov
       - run: mkdocs build -v -f docs/mkdocs.yml
       - name: Deploy
@@ -103,15 +104,14 @@
       - name: publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
   develop:
     if: contains(fromJson('["refs/heads/master", "refs/heads/main"]'), github.ref)
     needs: [lint, test]
-    environment: pypi
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v4
         with:
```

### Comparing `danling-0.3.4/.gitignore` & `danling-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/.pre-commit-config.yaml` & `danling-0.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.AGPL` & `danling-0.3.5/LICENSES/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.Apache` & `danling-0.3.5/LICENSES/LICENSE.Apache`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.BSD` & `danling-0.3.5/LICENSES/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.GPLv2` & `danling-0.3.5/LICENSES/LICENSE.GPLv2`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.GPLv3` & `danling-0.3.5/LICENSES/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.MIT` & `danling-0.3.5/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/LICENSES/LICENSE.Unlicense` & `danling-0.3.5/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/PKG-INFO` & `danling-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.4
+Version: 0.3.5
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
```

### Comparing `danling-0.3.4/README.md` & `danling-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/anaconda-project.yml` & `danling-0.3.5/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/__init__.py` & `danling-0.3.5/danling/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from danling import metrics, modules, optim, registry, runner, tensors, typing, utils
 
-from .metrics import AverageMeter, AverageMeters
+from .metrics import AverageMeter, Metrics, MultiTaskAverageMeter, MultiTaskMetrics
 from .registry import GlobalRegistry, Registry
 from .runner import AccelerateRunner, BaseRunner, TorchRunner
-from .tensors import NestedTensor, PNTensor
-from .utils import catch, debug, ensure_dir, flexible_decorator, is_json_serializable, load, method_cache, save
+from .tensors import NestedTensor, PNTensor, tensor
+from .utils import (
+    catch,
+    debug,
+    ensure_dir,
+    flexible_decorator,
+    is_json_serializable,
+    load,
+    load_pandas,
+    method_cache,
+    save,
+)
 
 __all__ = [
     "metrics",
     "modules",
     "optim",
     "registry",
     "runner",
@@ -17,20 +27,23 @@
     "typing",
     "BaseRunner",
     "AccelerateRunner",
     "TorchRunner",
     "Registry",
     "GlobalRegistry",
     "Metrics",
+    "MultiTaskMetrics",
     "AverageMeter",
-    "AverageMeters",
+    "MultiTaskAverageMeter",
     "NestedTensor",
     "PNTensor",
+    "tensor",
     "save",
     "load",
+    "load_pandas",
     "catch",
     "debug",
     "flexible_decorator",
     "method_cache",
     "ensure_dir",
     "is_json_serializable",
 ]
```

### Comparing `danling-0.3.4/danling/metrics/__init__.py` & `danling-0.3.5/danling/metrics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from functools import partial
 
 from lazy_imports import try_import
 
-from .average_meters import AverageMeter, AverageMeters
+from .average_meter import AverageMeter, MultiTaskAverageMeter
 
 with try_import():
     from .functional import accuracy, auprc, auroc, matthews_corrcoef, pearson, r2_score, rmse, spearman
-    from .metrics import Metrics
+    from .metrics import Metrics, MultiTaskMetrics
 
 __all__ = [
     "Metrics",
+    "MultiTaskMetrics",
     "AverageMeter",
-    "AverageMeters",
+    "MultiTaskAverageMeter",
     "regression_metrics",
     "binary_metrics",
     "multiclass_metrics",
     "multilabel_metrics",
 ]
```

### Comparing `danling-0.3.4/danling/metrics/functional.py` & `danling-0.3.5/danling/metrics/functional.py`

 * *Files 24% similar despite different names*

```diff
@@ -90,34 +90,39 @@
     target: Tensor | NestedTensor,
 ):
     lazy_import.check()
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
         target = torch.cat(target.storage())
-    return tmf.pearson_corrcoef(input, target)
+    try:
+        return tmf.pearson_corrcoef(input, target)
+    except ValueError:
+        return torch.tensor(0, dtype=float).to(input.device)
 
 
 def spearman(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
 ):
     lazy_import.check()
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
         target = torch.cat(target.storage())
-    return tmf.spearman_corrcoef(input, target)
+    try:
+        return tmf.spearman_corrcoef(input, target)
+    except ValueError:
+        return torch.tensor(0, dtype=float).to(input.device)
 
 
 def matthews_corrcoef(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
     threshold: float = 0.5,
-    average: str | None = "micro",
     num_labels: int | None = None,
     num_classes: int | None = None,
 ):
     lazy_import.check()
     if num_classes and num_labels:
         raise ValueError("Only one of num_classes or num_labels can be specified, but not both")
     task = "binary"
@@ -125,28 +130,36 @@
         task = "multiclass"
     if num_labels:
         task = "multilabel"
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
         target = torch.cat(target.storage())
-    return tmf.matthews_corrcoef(
-        input, target, task, threshold=threshold, num_classes=num_classes, num_labels=num_labels
-    )
+    try:
+        return tmf.matthews_corrcoef(
+            input, target, task, threshold=threshold, num_classes=num_classes, num_labels=num_labels
+        )
+    except ValueError:
+        return torch.tensor(0, dtype=float).to(input.device)
 
 
 def r2_score(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
+    multioutput: str = "uniform_average",
+    num_regressors: int = 0,
 ):
     if isinstance(input, NestedTensor):
         input = torch.cat(input.storage())
     if isinstance(target, NestedTensor):
         target = torch.cat(target.storage())
-    return tef.r2_score(input, target)
+    try:
+        return tef.r2_score(input, target, multioutput=multioutput, num_regressors=num_regressors)
+    except ValueError:
+        return torch.tensor(0, dtype=float).to(input.device)
 
 
 def mse(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
 ):
     if isinstance(input, NestedTensor):
@@ -156,12 +169,8 @@
     return tef.mean_squared_error(input, target)
 
 
 def rmse(
     input: Tensor | NestedTensor,
     target: Tensor | NestedTensor,
 ):
-    if isinstance(input, NestedTensor):
-        input = torch.cat(input.storage())
-    if isinstance(target, NestedTensor):
-        target = torch.cat(target.storage())
-    return tef.mean_squared_error(input, target).sqrt()
+    return mse(input, target).sqrt()
```

### Comparing `danling-0.3.4/danling/metrics/metrics.py` & `danling-0.3.5/danling/metrics/metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 from chanfig import DefaultDict, FlatDict
 from torch import Tensor
 from torch import distributed as dist
 from torcheval.metrics import Metric
 
 from danling.tensors import NestedTensor
 
+from .multitask import MultiTaskDict
 from .utils import flist, get_world_size
 
 try:
     from typing import Self  # type: ignore[attr-defined]
 except ImportError:
     from typing_extensions import Self
 
 
 class Metrics(Metric):
     r"""
     Metric class wraps around multiple metrics that share the same states.
 
     Typically, there are many metrics that we want to compute for a single task.
-    For example, we usually needs to compute `accuracy`, `auroc`, `auprc` for a classification task.
-    Computing them one by one is inefficient, especially when evaluating in a distributed environment.
+    For example, we usually needs to compute `pearson` and `spearman` for a regression task.
+    Unlike `accuracy`, which can uses an average meter to compute the average accuracy,
+    `pearson` and `spearman` cannot be computed by averaging the results of multiple batches.
+    They need access to all the data to compute the correct results.
+    And saving all intermediate results for each tasks is quite inefficient.
 
-    To solve this problem, Metrics maintains a shared state for multiple metric functions.
+    `Metrics` solves this problem by maintaining a shared state for multiple metric functions.
 
     Attributes:
         metrics: A dictionary of metrics to be computed.
         val: Metric results of current batch on current device.
         bat: Metric results of current batch on all devices.
         avg: Metric results of all results on all devices.
         input: The input tensor of latest batch.
@@ -42,15 +46,15 @@
         targets: All target tensors.
 
     Args:
         *args: A single mapping of metrics.
         **metrics: Metrics.
 
     Examples:
-        >>> from danling.metrics import auroc, auprc
+        >>> from danling.metrics.functional import auroc, auprc
         >>> metrics = Metrics(auroc=auroc, auprc=auprc)
         >>> metrics
         Metrics('auroc', 'auprc')
         >>> metrics.update([0.2, 0.3, 0.5, 0.7], [0, 1, 0, 1])
         >>> metrics.input  # predicted values of current batch
         tensor([0.2000, 0.3000, 0.5000, 0.7000])
         >>> metrics.target  # ground truth of current batch
@@ -94,17 +98,16 @@
           ('auprc'): 0.5
         )
         >>> metrics.avg  # Metrics of all data on all devices
         FlatDict(
           ('auroc'): 0.6666666666666666
           ('auprc'): 0.5555555820465088
         )
-        >>> print(f"{metrics:.4f}")
-        auroc: 0.6667 (0.6667)
-        auprc: 0.5000 (0.5556)
+        >>> f"{metrics:.4f}"
+        'auroc: 0.6667 (0.6667)\tauprc: 0.5000 (0.5556)'
     """
 
     metrics: FlatDict[str, Callable]
     _input: Tensor
     _target: Tensor
     _inputs: flist
     _targets: flist
@@ -303,20 +306,20 @@
 
     def __repr__(self):
         keys = tuple(i for i in self.metrics.keys())
         return f"{self.__class__.__name__}{keys}"
 
     def __format__(self, format_spec):
         val, avg = self.value(), self.average()
-        return "\n".join(
+        return "\t".join(
             [f"{key}: {val[key].__format__(format_spec)} ({avg[key].__format__(format_spec)})" for key in self.metrics]
         )
 
     def reset(self: Self) -> Self:  # pragma: no cover
-        """
+        r"""
         Reset the metric state variables to their default value.
         The tensors in the default values are also moved to the device of
         the last ``self.to(device)`` call.
         """
         for state_name, default in self._state_name_to_default.items():
             if isinstance(default, torch.Tensor):
                 setattr(self, state_name, default.clone().to(self.device))
@@ -401,7 +404,90 @@
         return self._score_name
 
     @score_name.setter
     def score_name(self, name) -> None:
         if name not in self.metrics:
             raise ValueError(f"score_name must be in {self.metrics.keys()}, but got {name}")
         self._score_name = name
+
+
+class MultiTaskMetrics(MultiTaskDict):
+    r"""
+    Examples:
+        >>> from danling.metrics.functional import auroc, auprc, pearson, spearman, accuracy, matthews_corrcoef
+        >>> metrics = MultiTaskMetrics()
+        >>> metrics.dataset1.cls = Metrics(auroc=auroc, auprc=auprc)
+        >>> metrics.dataset1.reg = Metrics(pearson=pearson, spearman=spearman)
+        >>> metrics.dataset2 = Metrics(auroc=auroc, auprc=auprc)
+        >>> metrics
+        MultiTaskMetrics(<class 'danling.metrics.metrics.MultiTaskMetrics'>,
+          ('dataset1'): MultiTaskMetrics(<class 'danling.metrics.metrics.MultiTaskMetrics'>,
+            ('cls'): Metrics('auroc', 'auprc')
+            ('reg'): Metrics('pearson', 'spearman')
+          )
+          ('dataset2'): Metrics('auroc', 'auprc')
+        )
+        >>> metrics.update({"dataset1.cls": {"input": [0.2, 0.4, 0.5, 0.7], "target": [0, 1, 0, 1]}, "dataset1.reg": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0.2, 0.3, 0.5, 0.7]}, "dataset2": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0, 1, 0, 1]}})
+        >>> f"{metrics:.4f}"
+        'dataset1.cls: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)\ndataset1.reg: pearson: 0.9691 (0.9691)\tspearman: 1.0000 (1.0000)\ndataset2: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)'
+        >>> metrics.setattr("return_average", True)
+        >>> metrics.update({"dataset1.cls": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0, 0, 1, 0]}, "dataset1.reg": {"input": [0.2, 0.3, 0.5, 0.7], "target": [0.2, 0.4, 0.6, 0.8]}, "dataset2": {"input": [0.2, 0.3, 0.5, 0.7], "target": [0, 0, 1, 0]}})
+        >>> f"{metrics:.4f}"
+        'dataset1.cls: auroc: 0.6667 (0.7000)\tauprc: 0.5000 (0.5556)\ndataset1.reg: pearson: 0.9898 (0.9146)\tspearman: 1.0000 (0.9222)\ndataset2: auroc: 0.6667 (0.7333)\tauprc: 0.5000 (0.7000)'
+    """  # noqa: E501
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, default_factory=MultiTaskMetrics, **kwargs)
+
+    def update(self, values: Mapping[str, Mapping[str, Tensor]]) -> None:  # pylint: disable=W0237
+        r"""
+        Updates the average and current value in all metrics.
+
+        Args:
+            values: Dict of values to be added to the average.
+
+        Raises:
+            ValueError: If the value is not an instance of (Mapping).
+
+        Examples:
+            >>> from danling.metrics.functional import auroc, auprc, pearson, spearman
+            >>> metrics = MultiTaskMetrics()
+            >>> metrics.dataset1.cls = Metrics(auroc=auroc, auprc=auprc)
+            >>> metrics.dataset1.reg = Metrics(pearson=pearson, spearman=spearman)
+            >>> metrics.dataset2 = Metrics(auroc=auroc, auprc=auprc)
+            >>> metrics.update({"dataset1.cls": {"input": [0.2, 0.4, 0.5, 0.7], "target": [0, 1, 0, 1]}, "dataset1.reg": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0.2, 0.3, 0.5, 0.7]}})
+            >>> f"{metrics:.4f}"
+            'dataset1.cls: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)\ndataset1.reg: pearson: 0.9691 (0.9691)\tspearman: 1.0000 (1.0000)\ndataset2: auroc: nan (nan)\tauprc: nan (nan)'
+            >>> metrics.update({"dataset2": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0, 1, 0, 1]}})
+            >>> f"{metrics:.4f}"
+            'dataset1.cls: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)\ndataset1.reg: pearson: 0.9691 (0.9691)\tspearman: 1.0000 (1.0000)\ndataset2: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)'
+            >>> metrics.update({"dataset1.cls": {"input": [0.1, 0.4, 0.6, 0.8], "target": [0, 0, 1, 0]}})
+            >>> f"{metrics:.4f}"
+            'dataset1.cls: auroc: 0.6667 (0.7000)\tauprc: 0.5000 (0.5556)\ndataset1.reg: pearson: 0.9691 (0.9691)\tspearman: 1.0000 (1.0000)\ndataset2: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)'
+            >>> metrics.update({"dataset1.reg": {"input": [0.2, 0.3, 0.5, 0.7], "target": [0.2, 0.4, 0.6, 0.8]}})
+            >>> f"{metrics:.4f}"
+            'dataset1.cls: auroc: 0.6667 (0.7000)\tauprc: 0.5000 (0.5556)\ndataset1.reg: pearson: 0.9898 (0.9146)\tspearman: 1.0000 (0.9222)\ndataset2: auroc: 0.7500 (0.7500)\tauprc: 0.8333 (0.8333)'
+            >>> metrics.update({"dataset1": {"cls": {"input": [0.1, 0.4, 0.6, 0.8]}}})
+            Traceback (most recent call last):
+            ValueError: Expected values to be a flat dictionary, but got <class 'dict'>
+            This is likely due to nested dictionary in the values.
+            Nested dictionaries cannot be processed due to the method's design, which uses Mapping to pass both input and target. Ensure your input is a flat dictionary or a single value.
+            >>> metrics.update(dict(loss=""))
+            Traceback (most recent call last):
+            ValueError: Expected values to be a flat dictionary, but got <class 'str'>
+        """  # noqa: E501
+
+        for metric, value in values.items():
+            if isinstance(value, Mapping):
+                if metric not in self:
+                    raise ValueError(f"Metric {metric} not found in {self}")
+                try:
+                    self[metric].update(**value)
+                except TypeError:
+                    raise ValueError(
+                        f"Expected values to be a flat dictionary, but got {type(value)}\n"
+                        "This is likely due to nested dictionary in the values.\n"
+                        "Nested dictionaries cannot be processed due to the method's design, which uses Mapping "
+                        "to pass both input and target. Ensure your input is a flat dictionary or a single value."
+                    ) from None
+            else:
+                raise ValueError(f"Expected values to be a flat dictionary, but got {type(value)}")
```

### Comparing `danling-0.3.4/danling/metrics/utils.py` & `danling-0.3.5/danling/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/__init__.py` & `danling-0.3.5/danling/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/mlp/dense.py` & `danling-0.3.5/danling/modules/mlp/dense.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/mlp/mlp.py` & `danling-0.3.5/danling/modules/mlp/mlp.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/__init__.py` & `danling-0.3.5/danling/modules/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.3.5/danling/modules/transformer/attention/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/attention/simple_attention.py` & `danling-0.3.5/danling/modules/transformer/attention/simple_attention.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/decoder.py` & `danling-0.3.5/danling/modules/transformer/decoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/encoder.py` & `danling-0.3.5/danling/modules/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/ffn/fcn.py` & `danling-0.3.5/danling/modules/transformer/ffn/fcn.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.3.5/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.3.5/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/runner/README.md` & `danling-0.3.5/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/runner/accelerate_runner.py` & `danling-0.3.5/danling/runner/accelerate_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,23 +74,27 @@
         super().__init__(config)
 
     def __post_init__(self) -> None:
         self.model, self.criterion, self.optimizer = self.prepare(self.model, self.criterion, self.optimizer)
         self.scheduler = self.prepare(self.scheduler)
         if self.datasets:
             datasets = {k: d for k, d in self.datasets.items() if k not in self.dataloaders}
-            default_kwargs = self.state.get("dataloader", NestedDict)
+            default_kwargs = self.state.setdefault("dataloader", NestedDict())
             dataloader_kwargs = NestedDict({k: default_kwargs.pop(k) for k in self.datasets if k in default_kwargs})
             for k, d in datasets.items():
                 dataloader_kwargs.setdefault(k, NestedDict())
                 dataloader_kwargs[k].merge(default_kwargs, overwrite=False)
                 dataloader_kwargs[k].setdefault("shuffle", getattr(d, "train", True))
                 dataloader_kwargs[k].setdefault("drop_last", not getattr(d, "train", True))
-                self.dataloaders[k] = self.prepare(utils.data.DataLoader(d, **dataloader_kwargs[k]))
+                self.dataloaders[k] = utils.data.DataLoader(d, **dataloader_kwargs[k])
             default_kwargs.update(dataloader_kwargs)
+        for k, d in self.dataloaders.items():
+            self.dataloaders[k] = self.prepare(d)
+        if self.state.get("log_interval") is None:
+            self.state.log_interval = max(len(d) for d in self.dataloaders.values()) // 10
 
     @property
     def deepspeed(self) -> dict | None:
         if "accelerator" not in self:
             raise ValueError("accelerator is not used")
         if self.accelerator.state.deepspeed_plugin is not None:
             return self.accelerator.state.deepspeed_plugin.deepspeed_config
@@ -127,15 +131,16 @@
             for split in train_splits:
                 result[split] = self.train_epoch(split)
             for split in eval_splits:
                 result[split] = self.evaluate_epoch(split)
             self.append_result(result)
             print(self.format_epoch_result(result))
             self.save_result()
-            self.save_checkpoint()
+            if self.state.save_interval is not None:
+                self.save_checkpoint(epochs)
             """@nni.report_intermediate_result(self.latest_score)"""
             early_stop_counter = 0 if self.is_best else early_stop_counter + 1
             if early_stop_counter > patience:
                 print("early stop")
                 break
         """@nni.report_final_result(self.latest_score)"""
         return self.results
@@ -152,14 +157,15 @@
         """
 
         self.mode = "train"  # type: ignore
         self.split = split
         loader = self.dataloaders[split]
         length = len(loader) - 1
         last_print_iteration = -1
+        log_interval = self.state.get("log_interval", -1)
         self.meters.reset()
         if self.metrics is not None:
             self.metrics.reset()
         batch_time = time()
         if hasattr(loader.batch_sampler, "set_epoch"):
             loader.batch_sampler.set_epoch(self.epochs)
         if hasattr(loader.sampler, "set_epoch"):
@@ -168,20 +174,18 @@
         for iteration, data in enumerate(loader):
             with self.autocast(), self.accumulate():
                 input = data["input"] if isinstance(data, Mapping) else data[0]
                 target = data["target"] if isinstance(data, Mapping) else data[1]
                 pred = self.model(**input) if isinstance(input, Mapping) else self.model(input)
                 loss = self.criterion(pred, target)
                 if self.metrics is not None:
-                    self.metrics.update(pred, target)
+                    self.metrics.update(pred.squeeze(-1), target)
                 self.step(loss)
 
-            if self.print_interval > 0 and (
-                iteration > 0 and iteration % self.print_interval == 0 or iteration == length
-            ):
+            if log_interval > 0 and (iteration > 0 and iteration % log_interval == 0 or iteration == length):
                 interval = iteration - last_print_iteration
                 if self.device == torch.device("cuda"):
                     torch.cuda.synchronize()
                 self.meters.time.update((time() - batch_time) / interval)
                 batch_time = time()
                 reduced_loss = self.reduce(loss).item()
                 self.meters.loss.update(reduced_loss)
@@ -230,30 +234,29 @@
         """
 
         self.mode = "eval"  # type: ignore
         self.split = split
         loader = self.dataloaders[split]
         length = len(loader) - 1
         last_print_iteration = -1
+        log_interval = self.state.get("log_interval", -1)
         self.meters.reset()
         if self.metrics is not None:
             self.metrics.reset()
         batch_time = time()
 
         for iteration, data in enumerate(loader):
             input = data["input"] if isinstance(data, Mapping) else data[0]
             target = data["target"] if isinstance(data, Mapping) else data[1]
             pred = self.model(**input) if isinstance(input, Mapping) else self.model(input)
             loss = self.criterion(pred, target)
             if self.metrics is not None:
-                self.metrics.update(pred, target)
+                self.metrics.update(pred.squeeze(-1), target)
 
-            if self.print_interval > 0 and (
-                iteration > 0 and iteration % self.print_interval == 0 or iteration == length
-            ):
+            if log_interval > 0 and (iteration > 0 and iteration % log_interval == 0 or iteration == length):
                 interval = iteration - last_print_iteration
                 if self.device == torch.device("cuda"):
                     torch.cuda.synchronize()
                 self.meters.time.update((time() - batch_time) / interval)
                 batch_time = time()
                 reduced_loss = self.reduce(loss).item()
                 self.meters.loss.update(reduced_loss)
@@ -282,15 +285,15 @@
         self.mode = "inf"  # type: ignore
         loader = self.dataloaders[split]
         self.meters.reset()
         output = []
         for _, data in tqdm(enumerate(loader), total=len(loader)):
             input = data["input"] if isinstance(data, Mapping) else data[0]
             pred = self.model(**input) if isinstance(input, Mapping) else self.model(input)
-            output.extend(pred.tolist())
+            output.extend(pred.squeeze(-1).tolist())
 
         if self.distributed:
             torch.cuda.synchronize()
             output = self.gather_for_metrics(output)
         return output
 
     def init_distributed(self) -> None:
```

### Comparing `danling-0.3.4/danling/runner/base_runner.py` & `danling-0.3.5/danling/runner/base_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from sys import version_info
 from typing import Any, Dict
 from uuid import UUID, uuid5
 from warnings import warn
 
 from chanfig import Config, FlatDict, NestedDict, Variable
 
-from danling.metrics import AverageMeter, AverageMeters, Metrics
+from danling.metrics import AverageMeter, Metrics, MultiTaskAverageMeter
 from danling.typing import File, PathStr
 from danling.utils import catch, ensure_dir, load, save
 
 try:
     from functools import cached_property
 except ImportError:
     from cached_property import cached_property  # type: ignore
@@ -85,15 +85,15 @@
             Results should be in the form of `{epoch: {subset: {metric: score}}}`.
         latest_result (NestedDict, property): Most recent result, should be in the form of `{subset: {metric: score}}`.
         best_result (NestedDict, property): Best result, should be in the form of `{subset: {metric: score}}`.
         scores (List[float], property): Score is the core metric that is used to evaluate the performance of the model.
             Scores should be in the form of `{epoch: score}`.
         latest_score (float, property): Most recent score, should be in the form of `score`.
         best_score (float, property): Best score, should be in the form of `score`.
-        score_set (Optional[str]): The subset to calculate the score.
+        score_split (Optional[str]): The subset to calculate the score.
             If is `None`, will use the last set of the result.
         score_name (str): The metric name of score.
             Defaults to `"loss"`.
         is_best (bool, property): If `latest_score == best_score`.
 
     A `result` is a dict with the same `split` as keys, like `dataloaders`.
     A typical `result` shall look like this:
@@ -110,17 +110,17 @@
         "test": {
             "loss": 0.3,
             "accuracy": 0.7,
         },
     }
     ```
 
-    `scores` are dynamically extracted from `results` by `score_set` and `score_name`.
+    `scores` are dynamically extracted from `results` by `score_split` and `score_name`.
     They represent the core metric that is used in comparing the performance against different models and settings.
-    For the above `results`, If `score_set = "val"`, `score_name = "accuracy"`, then `scores = 0.9`.
+    For the above `results`, If `score_split = "val"`, `score_name = "accuracy"`, then `scores = 0.9`.
 
     Attributes: IO:
         dir (str, property): Directory of the run.
             Defaults to `${self.project_root}/${self.name}-${self.id}/${self.timestamp})`.
         checkpoint_dir (str, property): Directory of checkpoints.
         log_path (str, property):  Path of log file.
         checkpoint_dir_name (str): The name of the directory under `runner.dir` to save checkpoints.
@@ -131,16 +131,16 @@
         rank (int, property): Process index of all processes.
         local_rank (int, property): Process index of local processes.
         distributed (bool, property): If runner is running in distributed mode.
         is_main_process (bool, property): If current process is the main process of all processes.
         is_local_main_process (bool, property): If current process is the main process of local processes.
 
     Attributes: logging:
-        meters (AverageMeters): Average meters.
-            Initialised to `AverageMeters` by default.
+        meters (MultiTaskAverageMeter): Average meters.
+            Initialised to `MultiTaskAverageMeter` by default.
         metrics (Metrics): Metrics for evaluating.
         logger:
         writer:
 
     See Also:
         [`RunnerState`][danling.runner.runner_state.RunnerState]: The runeer base that stores runtime information.
         [`BaseRunner`][danling.runner.BaseRunner]: The base runner class.
@@ -161,30 +161,30 @@
 
     datasets: FlatDict
     datasamplers: FlatDict
     dataloaders: FlatDict
     split: str
 
     results: NestedDict
-    meters: AverageMeters
+    meters: MultiTaskAverageMeter
     metrics: Metrics | None = None
     logger: logging.Logger | None = None
     writer: Any | None = None
 
     def __init__(self, config: NestedDict) -> None:
         self.timestamp = get_time_str()
         if "datasets" not in self.__dict__:
             self.datasets = FlatDict()
         if "datasamplers" not in self.__dict__:
             self.datasamplers = FlatDict()
         if "dataloaders" not in self.__dict__:
             self.dataloaders = FlatDict()
         if "results" not in self.__dict__:
             self.results = NestedDict()
-        self.meters = AverageMeters()
+        self.meters = MultiTaskAverageMeter()
         self._mode = RunnerMode.train  # type: ignore[assignment]
         # must init state at last to avoid name conflicts
         self._state = RunnerState(config)
         self.inited = True
         self.init_distributed()
         if self.state.seed is not None:
             self.set_seed()
@@ -213,15 +213,15 @@
         if config is None:
             config = self.state.get("deepspeed")
         if config is None:
             return {}
         if isinstance(config, str):
             config = NestedDict.load(config)
         if config.get("steps_per_print", "auto") == "auto":
-            config["steps_per_print"] = self.print_interval
+            config["steps_per_print"] = self.state.log_interval
         if config.get("train_micro_batch_size_per_gpu", "auto") == "auto":
             config["train_micro_batch_size_per_gpu"] = self.batch_size
         if "amp" in config:
             amp = config["amp"]
             if amp.get("enabled", "auto") == "auto":
                 amp["enabled"] = "true"
             if amp.get("opt_level", "auto") == "auto":
@@ -570,34 +570,32 @@
             if action == "raise":
                 raise RuntimeError(f"Directory `{self.dir}` is not empty")
             return False
         return True
 
     @catch
     @on_main_process
-    def save_checkpoint(self) -> None:
+    def save_checkpoint(self, epochs: int | None = None) -> None:
         r"""
         Save checkpoint to `self.checkpoint_dir`.
 
         The checkpoint will be saved to `self.checkpoint_dir/latest.pth`.
 
         If `self.state.save_interval` is positive and `self.state.epochs + 1` is a multiple of `save_interval`,
         the checkpoint will also be copied to `self.checkpoint_dir/epoch-{self.state.epochs}.pth`.
 
         If `self.is_best` is `True`, the checkpoint will also be copied to `self.checkpoint_dir/best.pth`.
         """
 
+        epochs = epochs or self.state.epochs
+        save_interval = self.state.get("save_interval", -1)
         latest_path = os.path.join(self.checkpoint_dir, "latest.pth")
         self.save(self.state_dict(), latest_path)
-        if (
-            hasattr(self, "save_interval")
-            and self.save_interval > 0
-            and (self.state.epochs + 1) % self.save_interval == 0
-        ):
-            save_path = os.path.join(self.checkpoint_dir, f"epoch-{self.state.epochs}.pth")
+        if save_interval > 0 and (epochs + 1) % save_interval == 0:
+            save_path = os.path.join(self.checkpoint_dir, f"epoch-{epochs}.pth")
             shutil.copy(latest_path, save_path)
         if self.is_best:
             best_path = os.path.join(self.checkpoint_dir, "best.pth")
             shutil.copy(latest_path, best_path)
 
     def load_checkpoint(
         self,
@@ -763,52 +761,55 @@
             self.results[index] = result
 
     def print_result(self) -> None:
         r"""
         Print latest and best result.
         """
 
-        print(f"results: {self.results}")
         print(f"latest result: {self.latest_result}")
         print(f"best result: {self.best_result}")
 
     def step_log(self, split: str, iteration: int, length: int | None = None):
         if length is None:
             length = len(self.dataloaders[split]) - 1
         result = self.meters.val
         if self.metrics is not None:
             result.merge(self.metrics.val)
         print(self.format_step_result(result, split, iteration, length))
         if self.mode == "train":
             self.write_result(result, split)
         return result
 
-    def format_step_result(self, result: NestedDict, split: str, steps: int, length: int) -> str:
+    def format_step_result(
+        self, result: NestedDict, split: str, steps: int, length: int, format_spec: str = ".4f"
+    ) -> str:
         result = NestedDict(result).clone()
         repr_str = ""
         if split is not None:
             if self.mode == "train":
                 repr_str = f"training on {split} "
             elif self.mode == "eval":
                 repr_str = f"evaluating on {split} "
             else:
                 repr_str = f"running in {self.mode} mode on {split} "
         repr_str += f"[{steps}/{length}]\t"
-        return repr_str + self.format_result(result)
+        return repr_str + self.format_result(result, format_spec=format_spec)
 
-    def format_epoch_result(self, result: NestedDict, epochs: int | None = None, epoch_end: int | None = None) -> str:
+    def format_epoch_result(
+        self, result: NestedDict, epochs: int | None = None, epoch_end: int | None = None, format_spec: str = ".4f"
+    ) -> str:
         result = NestedDict(result).clone()
         epochs = epochs or self.state.epochs
         epoch_end = epoch_end or self.state.epoch_end
         repr_str = f"epoch [{epochs}/{epoch_end - 1}]\n" if epochs is not None and epoch_end else ""
-        repr_str += "\n".join([f"{k}:\t{self.format_result(v)}" for k, v in result.items()])
+        repr_str += "\n".join([f"{k}:\t{self.format_result(v, format_spec=format_spec)}" for k, v in result.items()])
         return repr_str
 
-    def format_result(self, result):
-        return "\t".join([f"{k}: {v}" for k, v in result.items()])
+    def format_result(self, result, format_spec: str = ".4f") -> str:
+        return "\t".join([f"{k}: {format(v, format_spec)}" for k, v in result.items()])
 
     def write_result(self, result: NestedDict, split: str, steps: int | None = None):
         if steps is None:
             steps = self.steps
         for name, score in result.all_items():
             name = name.replace(".", "/")
             if name == "loss" and isinstance(score, AverageMeter):
@@ -1072,39 +1073,39 @@
         return ret
 
     @property
     def scores(self) -> FlatDict | None:
         r"""
         All scores.
 
-        Scores are extracted from results by `score_set` and `runner.state.score_name`,
-        following `[r[score_set][self.state.score_name] for r in self.results]`.
+        Scores are extracted from results by `score_split` and `runner.state.score_name`,
+        following `[r[score_split][self.state.score_name] for r in self.results]`.
 
         Scores are considered as the index of the performance of the model.
         It is useful to determine the best model and the best hyper-parameters.
 
-        `score_set` is defined in `self.state.score_set`.
+        `score_split` is defined in `self.state.score_split`.
         If it is not set, `DanLing` will use `val` or `validate` if they appear in the `latest_result`.
         If `DanLing` still could not find, it will fall back to the second key in the `latest_result`
         if it contains more that one element, or the first key.
 
         Note that certain keys are ignored when falling back, they are defined in {IGNORED_SET_NAMES}.
         """
 
         if not self.results:
             return None
         subsets = [i for i in self.latest_result.keys() if i not in IGNORED_SET_NAMES]  # type: ignore
-        score_set = self.state.get("score_set")
-        if score_set is None and "val" in subsets:
-            score_set = "val"
-        if score_set is None and "validate" in subsets:
-            score_set = "validate"
-        if score_set is None:
-            score_set = subsets[1] if len(subsets) > 1 else subsets[0]
-        return FlatDict({k: v[score_set][self.state.score_name] for k, v in self.results.items()})
+        score_split = self.state.get("score_split")
+        if score_split is None and "val" in subsets:
+            score_split = "val"
+        if score_split is None and "validate" in subsets:
+            score_split = "validate"
+        if score_split is None:
+            score_split = subsets[1] if len(subsets) > 1 else subsets[0]
+        return FlatDict({k: v[score_split][self.state.score_name] for k, v in self.results.items()})
 
     @property
     def latest_score(self) -> float | None:
         r"""
         Latest score.
         """
 
@@ -1163,15 +1164,15 @@
     def checkpoint_dir(self) -> str:
         r"""
         Directory of checkpoints.
         """
 
         if "checkpoint_dir" in self.state:
             return self.state.checkpoint_dir
-        return os.path.join(self.dir, self.checkpoint_dir_name)
+        return os.path.join(self.dir, self.state.checkpoint_dir_name)
 
     # def __getattribute__(self, name) -> Any:
     #     if name in ("__class__", "__dict__"):
     #         return super().__getattribute__(name)
     #     if name in self.__dict__:
     #         return self.__dict__[name]
     #     if name in dir(self):
```

### Comparing `danling-0.3.4/danling/runner/state.py` & `danling-0.3.5/danling/runner/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,19 @@
     In practice, `checkpoint_dir_name` is rarely called.
 
     Attributes: logging:
         log (bool): Whether to log the outputs.
             Defaults to `True`.
         tensorboard (bool): Whether to use `tensorboard`.
             Defaults to `False`.
-        print_interval (int): Interval of printing logs.
-            Defaults to -1.
+        log_interval (int): Interval of printing logs.
+            Defaults to `None`, print logs every 1/10 of the longest split.
         save_interval (int): Interval of saving intermediate checkpoints.
-            Defaults to -1, never save intermediate checkpoints.
+            Defaults to `None`, never save checkpoints.
+            If <= 0, save only the latest and the best checkpoints.
 
     Notes:
         `RunnerState` is a `NestedDict`, so you can access its attributes by `state["name"]` or `state.name`.
 
     See Also:
         [`BaseRunner`][danling.runner.BaseRunner]: The base runner class.
     """
@@ -100,23 +101,23 @@
     iter_begin: int = 0
     step_begin: int = 0
     epoch_begin: int = 0
     iter_end: Optional[int] = None
     step_end: Optional[int] = None
     epoch_end: Optional[int] = None
 
-    score_set: Optional[str] = None
+    score_split: Optional[str] = None
     score_name: str = "loss"
 
     project_root: str = "experiments"
     checkpoint_dir_name: str = "checkpoints"
     log: bool = True
     tensorboard: bool = False
-    print_interval: int = -1
-    save_interval: int = -1
+    log_interval: Optional[int] = None
+    save_interval: Optional[int] = None
 
     distributed: Optional[bool] = None
     dist_backend: Optional[str] = None
     init_method: Optional[str] = None
     master_addr: Optional[str] = None
     master_port: Optional[int] = None
```

### Comparing `danling-0.3.4/danling/runner/utils.py` & `danling-0.3.5/danling/runner/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/tensors/functional.py` & `danling-0.3.5/danling/tensors/functional.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/tensors/nested_tensor.py` & `danling-0.3.5/danling/tensors/nested_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 from torch.utils.data._utils.collate import default_collate_fn_map
 
 from ..utils import method_cache
 from .functional import mask_tensor, pad_tensor
 from .utils import TorchFuncRegistry
 
 
+def tensor(data: Any, dtype=None, device=None, requires_grad: bool = False, pin_memory: bool = False) -> PNTensor:
+    return PNTensor(torch.tensor(data, dtype=dtype, device=device, requires_grad=requires_grad, pin_memory=pin_memory))
+
+
 class PNTensor(Tensor):
     r"""
     Wrapper for tensors to be converted to `NestedTensor`.
 
     `PNTensor` is a subclass of `torch.Tensor`.
-    It implements two additional methods as `NestedTensor`: `tensor` and `mask`.
+    It implements three additional property as `NestedTensor`: `tensor`, `mask`, and `concat`.
 
     Although it is possible to directly construct `NestedTensor` in dataset,
     the best practice is to do so is in `collate_fn`.
-    `PNTensor` is introduced to smooth the process.
+    `PNTensor` is introduced to smoothen the process.
 
     Convert tensors that will be converted to `NestedTensor` to a `PNTensor`,
     and PyTorch Dataloader will automatically collate `PNTensor` to `NestedTensor`.
     """
 
     @property
     def tensor(self) -> Tensor:
@@ -59,14 +63,33 @@
             >>> pn_tensor = PNTensor([1, 2, 3])
             >>> bool((pn_tensor.mask == torch.ones_like(pn_tensor)).all().item())
             True
         """
 
         return torch.ones_like(self)
 
+    @property
+    def contact(self) -> Tensor:
+        r"""
+        Identical to `self`.
+
+        Returns:
+            (torch.Tensor):
+
+        Examples:
+            >>> tensor = torch.tensor([1, 2, 3])
+            >>> pn_tensor = PNTensor([1, 2, 3])
+            >>> bool((tensor == pn_tensor).all())
+            True
+            >>> bool((tensor == pn_tensor.contact).all())
+            True
+        """
+
+        return self
+
     def new_empty(self, *args, **kwargs):
         return PNTensor(super().new_empty(*args, **kwargs))
 
 
 class NestedTensor:
     r"""
     Wrap an iterable of tensors into a single tensor with a mask.
@@ -81,14 +104,15 @@
     1. if arg is `int` or `slice`, returns a tuple of two `tensor`s, representing data and padding mask.
     2. if arg is a `tuple`, return a new `NestedTensor` with specified shape.
 
     Attributes:
         _storage: The sequence of tensors.
         tensor: padded tensor.
         mask: mask tensor.
+        concat: concatenated tensor.
         batch_first:  Whether the first dimension of the tensors is the batch dimension.
 
             If `True`, the first dimension is the batch dimension, i.e., `B, N, *`.
 
             If `False`, the first dimension is the sequence dimension, i.e., `N, B, *`
         padding_value: The padding value used to in padded tensor.
         mask_value: The mask value used in mask tensor.
@@ -119,14 +143,16 @@
         torch.int64
         >>> nested_tensor.tensor
         tensor([[1, 2, 3],
                 [4, 5, 0]])
         >>> nested_tensor.mask
         tensor([[ True,  True,  True],
                 [ True,  True, False]])
+        >>> nested_tensor.concat
+        tensor([1, 2, 3, 4, 5])
         >>> nested_tensor.to(torch.float).tensor
         tensor([[1., 2., 3.],
                 [4., 5., 0.]])
         >>> nested_tensor.half().tensor
         tensor([[1., 2., 3.],
                 [4., 5., 0.]], dtype=torch.float16)
         >>> nested_tensor[:]
@@ -172,15 +198,15 @@
     def _storage(self, tensors: Sequence):
         if not isinstance(tensors, Iterable):
             raise ValueError(f"tensors must be an Iterable, bug got {type(tensors)}.")
         tensors = list(tensors)
         if len(tensors) == 0:
             raise ValueError("tensors must be a non-empty Iterable.")
         if not isinstance(tensors[0], Tensor):
-            tensors = [torch.tensor(tensor) for tensor in tensors]
+            tensors = [tensor(t) for t in tensors]
         self.__storage = tensors
 
     def storage(self):
         return self._storage
 
     @property
     def tensor(self) -> Tensor:
@@ -212,14 +238,53 @@
             >>> nested_tensor.mask
             tensor([[ True,  True,  True],
                     [ True,  True, False]])
         """
 
         return self._mask(tuple(self._storage), self.batch_first, self.mask_value)
 
+    @property
+    def concat(self) -> Tensor:
+        r"""
+        Concat `tensor` in padding dim.
+
+        This is particularly useful when calculating loss or passing `Linear` to avoid unnecessary computation.
+
+        Returns:
+            (torch.Tensor):
+
+        Examples:
+            >>> nested_tensor = NestedTensor([torch.randn(9, 8), torch.randn(11, 8)])
+            >>> nested_tensor.concat.shape
+            torch.Size([20, 8])
+            >>> nested_tensor = NestedTensor([torch.randn(9, 9, 8), torch.randn(11, 11, 8)])
+            >>> nested_tensor.concat.shape
+            torch.Size([202, 8])
+            >>> nested_tensor = NestedTensor([torch.randn(9, 9, 8, 6), torch.randn(11, 11, 8, 6)])
+            >>> nested_tensor.concat.shape
+            torch.Size([202, 8, 6])
+            >>> nested_tensor = NestedTensor([torch.randn(9, 9, 8, 7), torch.randn(11, 11, 8, 6)])
+            >>> nested_tensor.concat.shape
+            torch.Size([1293, 8])
+        """
+        shape = list(self.size())  # type: ignore[arg-type]
+        shape = shape[1:] if self.batch_first else shape[0] + shape[2:]
+        elem = self._storage[0]
+        if elem.shape == shape:
+            return torch.cat(self._storage, dim=1 if self.batch_first else 0)
+
+        static_dims = set(range(len(shape)))
+        for i, s in enumerate(shape):
+            if not all(t.shape[i] == s for t in self._storage):
+                shape[i] = -1
+                static_dims.remove(i)
+        target_shape = [-1] + [s for s in shape if s != -1]
+        storage = [i.view(target_shape) for i in self._storage]
+        return torch.cat(storage, dim=0 if self.batch_first else 1)
+
     @classmethod
     def from_tensor_mask(cls, tensor: Tensor, mask: Tensor):
         r"""
         Build a `NestedTensor` object from a padded `Tensor` and corresponding mask `Tensor`.
 
         Args:
             tensor: Padded Tensor.
```

### Comparing `danling-0.3.4/danling/tensors/utils.py` & `danling-0.3.5/danling/tensors/utils.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/utils/basex.py` & `danling-0.3.5/danling/utils/basex.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/utils/contextmanagers.py` & `danling-0.3.5/danling/utils/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/danling/utils/decorators.py` & `danling-0.3.5/danling/utils/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from weakref import ref
 
 from danling.typing import Exceptions
 
 
 def flexible_decorator(maybe_decorator: Optional[Callable] = None):
     r"""
-    Decorator to allow bracket-less when no arguments are passed.
+    Meta decorator to allow bracket-less decorator when no arguments are passed.
 
     Examples:
         For decorator defined as follows:
 
         >>> @flexible_decorator
         ... def decorator(*args, **kwargs):
         ...     def wrapper(func, *args, **kwargs):
@@ -33,15 +33,15 @@
 
         >>> @decorator()
         ... def func(*args, **kwargs):
         ...     pass
     """
 
     def decorator(func: Callable):
-        @wraps(decorator)
+        @wraps(func)
         def wrapper(*args, **kwargs):
             if len(args) == 1 and isfunction(args[0]):
                 return func(**kwargs)(args[0])
             return func(*args, **kwargs)
 
         return wrapper
 
@@ -100,19 +100,26 @@
             Additional arguments should be passed with `*callback_args` and `**callback_kwargs`.
         callback_args: Arguments to be passed to `callback`.
         callback_kwargs: Keyword arguments to be passed to `callback`.
 
     Examples:
         >>> def file_not_found(*args, **kwargs):
         ...     raise FileNotFoundError
-        >>> file_not_found()
+        >>> func = file_not_found
+        >>> func()
         Traceback (most recent call last):
         FileNotFoundError
         >>> func = catch(OSError)(file_not_found)
-        >>> file_not_found()
+        >>> func()
+        >>> func = catch(IOError)(file_not_found)
+        >>> func()
+        >>> func = catch(ZeroDivisionError)(file_not_found)
+        >>> func()
+        Traceback (most recent call last):
+        FileNotFoundError
     """
 
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):  # pylint: disable=inconsistent-return-statements
             try:
                 return func(*args, **kwargs)
```

### Comparing `danling-0.3.4/danling/utils/io.py` & `danling-0.3.5/danling/utils/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,21 +26,26 @@
     import pandas
 
     PANDAS_AVAILABLE = True
 except ImportError:
     PANDAS_AVAILABLE = False
 
 
-JSON = ("json",)
-YAML = ("yaml", "yml")
 PYTORCH = ("pt", "pth")
-CSV = ("csv",)
 NUMPY = ("numpy", "npy", "npz")
+JSON = ("json",)
+YAML = ("yaml", "yml")
+CSV = ("csv", "tsv")
 PANDAS = ("pandas", "pd")
 PICKLE = ("pickle", "pkl")
+H5 = ("h5", "hdf5")
+EXCEL = ("xlsx", "xls")
+XML = ("xml",)
+SQL = ("sql",)
+PANDAS_SUPPORTED = sum([JSON, YAML, CSV, PANDAS, PICKLE, H5, EXCEL, XML, SQL], ())
 
 
 def save(obj: Any, file: PathStr, *args: List[Any], **kwargs: Dict[str, Any]) -> File:
     r"""
     Save any file with supported extensions.
     """
     extension = os.path.splitext(file)[-1].lower()[1:]
@@ -92,31 +97,51 @@
         if not TORCH_AVAILABLE:
             raise ImportError(f"Trying to load {file!r} but torch is not installed.")
         return torch.load(file, *args, **kwargs)
     if extension in NUMPY:
         if not NUMPY_AVAILABLE:
             raise ImportError(f"Trying to load {file!r} but numpy is not installed.")
         return numpy.load(file, *args, **kwargs)
-    if extension in PANDAS:
-        if not PANDAS_AVAILABLE:
-            raise ImportError(f"Trying to load {file!r} but pandas is not installed.")
-        return pandas.read_pickle(file, *args, **kwargs)
-    if extension in CSV:
-        if not PANDAS_AVAILABLE:
-            raise ImportError(f"Trying to load {file!r} but pandas is not installed.")
-        return pandas.read_csv(file, *args, **kwargs)
     if extension in JSON:
         with open(file) as fp:
             return json.load(fp, *args, **kwargs)  # type: ignore
     if extension in YAML:
         with open(file) as fp:
             return yaml.load(fp, *args, **kwargs)  # type: ignore
     if extension in PICKLE:
         with open(file, "rb") as fp:
             return pickle.load(fp, *args, **kwargs)  # type: ignore
+    if extension in PANDAS_SUPPORTED:
+        load_pandas(file, *args, **kwargs)
+    raise ValueError(f"Tying to load {file!r} with unsupported extension={extension!r}")
+
+
+def load_pandas(file: PathStr, *args: List[Any], **kwargs: Dict[str, Any]) -> Any:
+    r"""
+    Load any pandas data file with supported extensions.
+    """
+    if not PANDAS_AVAILABLE:
+        raise ImportError(f"Trying to load {file!r} but pandas is not installed.")
+    if not os.path.isfile(file):
+        raise ValueError(f"Trying to load {file!r} but it is not a file.")
+    extension = os.path.splitext(file)[-1].lower()[1:]
+    if extension in PANDAS or extension in PICKLE:
+        return pandas.read_pickle(file, *args, **kwargs)
+    if extension in H5:
+        return pandas.read_hdf(file, *args, **kwargs)
+    if extension in CSV:
+        return pandas.read_csv(file, *args, **kwargs)
+    if extension in JSON:
+        return pandas.read_json(file, *args, **kwargs)
+    if extension in EXCEL:
+        return pandas.read_excel(file, *args, **kwargs)
+    if extension in XML:
+        return pandas.read_xml(file, *args, **kwargs)
+    if extension in SQL:
+        return pandas.read_sql(file, *args, **kwargs)
     raise ValueError(f"Tying to load {file!r} with unsupported extension={extension!r}")
 
 
 def is_json_serializable(obj: Any) -> bool:
     r"""
     Check if `obj` is JSON serializable.
     """
```

### Comparing `danling-0.3.4/danling.egg-info/PKG-INFO` & `danling-0.3.5/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.4
+Version: 0.3.5
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
```

### Comparing `danling-0.3.4/danling.egg-info/SOURCES.txt` & `danling-0.3.5/danling.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
 danling/typing.py
 danling.egg-info/PKG-INFO
 danling.egg-info/SOURCES.txt
 danling.egg-info/dependency_links.txt
 danling.egg-info/requires.txt
 danling.egg-info/top_level.txt
 danling/metrics/__init__.py
-danling/metrics/average_meters.py
+danling/metrics/average_meter.py
 danling/metrics/functional.py
 danling/metrics/metrics.py
+danling/metrics/multitask.py
 danling/metrics/utils.py
 danling/modules/__init__.py
 danling/modules/mlp/__init__.py
 danling/modules/mlp/dense.py
 danling/modules/mlp/mlp.py
 danling/modules/transformer/__init__.py
 danling/modules/transformer/decoder.py
@@ -70,15 +71,14 @@
 docs/requirements.txt
 docs/docs/CNAME
 docs/docs/index.md
 docs/docs/manifest.webmanifest
 docs/docs/package.md
 docs/docs/blog/index.md
 docs/docs/metrics/average_meter.md
-docs/docs/metrics/average_meters.md
 docs/docs/metrics/metrics.md
 docs/docs/optim/lr_scheduler.md
 docs/docs/runner/accelerate_runner.md
 docs/docs/runner/base_runner.md
 docs/docs/runner/index.md
 docs/docs/runner/state.md
 docs/docs/runner/utils.md
```

### Comparing `danling-0.3.4/demo/vision/torch_mnist.py` & `danling-0.3.5/demo/vision/torch_mnist.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 
 OPTIMIZERS = Registry()
 OPTIMIZERS.register(optim.AdamW, "adamw")
 OPTIMIZERS.register(optim.SGD, "sgd")
 
 
 class MNISTConfig(Config):
+    epoch_end = 2
+    log = False
+    tensorboard = False
+    log_interval = 1000
+    score_split = "val"
+    score_name = "loss"
+    debug = False
+    patience = 1
+
     def __init__(self):
         self.network.name = "resnet18"
         self.dataset.download = True
         self.dataset.root = "data"
         self.dataloader.batch_size = 8
-        self.epoch_end = 2
         self.optim.name = "adamw"
         self.optim.lr = 1e-3
         self.optim.weight_decay = 1e-4
-        self.log = False
-        self.tensorboard = False
-        self.print_interval = 1000
-        self.score_set = "val"
-        self.score_name = "loss"
-        self.debug = False
-        self.patience = 1
 
     def post(self):
         self.experiment_name = f"{self.network.name}_{self.optim.name}@{self.optim.lr}"
 
 
 class MNISTRunner(dl.TorchRunner):
     def __init__(self, config: Config):
```

### Comparing `danling-0.3.4/docs/mkdocs.yml` & `danling-0.3.5/docs/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
   - Tensors:
       - NestedTensor: tensors/nested_tensor.md
       - PNTensor: tensors/pn_tensor.md
       - TorchFuncRegistry: tensors/torch_func_registry.md
   - Optim:
       - LRScheduler: optim/lr_scheduler.md
   - Metrics:
-      - metrics: metrics/metrics.md
-      - AverageMeters: metrics/average_meters.md
+      - Metrics: metrics/metrics.md
+      - AverageMeter: metrics/average_meter.md
   - Utilities:
       - Decorator: utils/decorators.md
       - Context Manager: utils/contextmanagers.md
       - IO: utils/io.md
       - basex: utils/basex.md
   - package: package.md
   # - Blog: blog/index.md
```

#### html2text {}

```diff
@@ -3,25 +3,25 @@
 Researchers copyright: All rights reserved © 2021-2023, DanLing Contributors
 repo_name: DanLing repo_url: https://github.com/ZhiyuanChen/DanLing nav: -
 DanLing: index.md - Runner: - runner/index.md - RunnerState: runner/
 runner_state.md - BaseRunner: runner/base_runner.md - AccelerateRunner: runner/
 accelerate_runner.md - Utilities: runner/utils.md - Tensors: - NestedTensor:
 tensors/nested_tensor.md - PNTensor: tensors/pn_tensor.md - TorchFuncRegistry:
 tensors/torch_func_registry.md - Optim: - LRScheduler: optim/lr_scheduler.md -
-Metrics: - metrics: metrics/metrics.md - AverageMeters: metrics/
-average_meters.md - Utilities: - Decorator: utils/decorators.md - Context
-Manager: utils/contextmanagers.md - IO: utils/io.md - basex: utils/basex.md -
-package: package.md # - Blog: blog/index.md theme: name: material custom_dir:
-overrides language: "zh" palette: - media: "(prefers-color-scheme: dark)"
-scheme: slate primary: blue grey accent: teal toggle: icon: material/
-brightness-4 name: Switch to light mode - media: "(prefers-color-scheme:
-light)" scheme: default primary: blue grey accent: teal toggle: icon: material/
-brightness-7 name: Switch to dark mode logo: "assets/images/logo.png" favicon:
-"assets/images/logo.ico" features: - announce.dismiss # - content.action.edit #
-- content.action.view - content.code.annotate - content.code.copy -
+Metrics: - Metrics: metrics/metrics.md - AverageMeter: metrics/average_meter.md
+- Utilities: - Decorator: utils/decorators.md - Context Manager: utils/
+contextmanagers.md - IO: utils/io.md - basex: utils/basex.md - package:
+package.md # - Blog: blog/index.md theme: name: material custom_dir: overrides
+language: "zh" palette: - media: "(prefers-color-scheme: dark)" scheme: slate
+primary: blue grey accent: teal toggle: icon: material/brightness-4 name:
+Switch to light mode - media: "(prefers-color-scheme: light)" scheme: default
+primary: blue grey accent: teal toggle: icon: material/brightness-7 name:
+Switch to dark mode logo: "assets/images/logo.png" favicon: "assets/images/
+logo.ico" features: - announce.dismiss # - content.action.edit # -
+content.action.view - content.code.annotate - content.code.copy -
 content.tabs.link - content.tooltips - header.autohide - navigation.expand -
 navigation.footer - navigation.indexes # - navigation.instant -
 navigation.prune - navigation.sections - navigation.tabs -
 navigation.tabs.sticky - navigation.top - navigation.tracking -
 search.highlight - search.share - search.suggest - toc.follow - toc.integrate
 font: false extra: analytics: provider: google property: "G-RE7EKZ9T8D"
 consent: title: Cookie consent description: >- We use cookies to recognize your
```

### Comparing `danling-0.3.4/docs/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.3.5/docs/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.3.5/docs/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.3.5/docs/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.3.5/docs/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/assets/images/favicon.ico` & `danling-0.3.5/docs/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/assets/images/logo.png` & `danling-0.3.5/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/docs/overrides/main.html` & `danling-0.3.5/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/pyproject.toml` & `danling-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/tests/metrics/test_metrics.py` & `danling-0.3.5/tests/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/tests/optim/test_lr_scheduler.py` & `danling-0.3.5/tests/optim/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `danling-0.3.4/tests/runner/test_base_runner.py` & `danling-0.3.5/tests/runner/test_base_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,18 +22,19 @@
         self.epoch_end = 2
         self.optim.name = "adamw"
         self.optim.lr = 1e-3
         self.optim.weight_decay = 1e-4
         self.log = False
         self.tensorboard = False
         self.gradient_clip = False
-        self.print_interval = 10
+        self.log_interval = None
+        self.save_interval = None
         self.train_iterations_per_epoch = 64
         self.val_iterations_per_epoch = 16
-        self.score_set = "val"
+        self.score_split = "val"
         self.score = "loss"
         self.conflict = 1
 
 
 class Test:
     config = Config()
     runner = Runner(config)
```

### Comparing `danling-0.3.4/tests/runner/test_torch_runner.py` & `danling-0.3.5/tests/runner/test_torch_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,17 @@
         self.dataloader.batch_size = 8
         self.epoch_end = 2
         self.optim.name = "adamw"
         self.optim.lr = 1e-3
         self.optim.weight_decay = 1e-4
         self.log = False
         self.tensorboard = False
-        self.print_interval = 1000
-        self.score_set = "val"
+        self.log_interval = None
+        self.save_interval = None
+        self.score_split = "val"
         self.score_name = "loss"
 
     def post(self):
         self.experiment_name = f"{self.network.name}_{self.optim.name}@{self.optim.lr}"
 
 
 class MNISTRunner(dl.TorchRunner):
```

### Comparing `danling-0.3.4/tests/tensors/test_nested_tensor.py` & `danling-0.3.5/tests/tensors/test_nested_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         assert torch.sum(a * i - i / (1 / a)) < self.epsilon
         assert torch.sum(a / (1 / i) - i * a) < self.epsilon
         assert torch.sum(a * i - i * a) < self.epsilon
         a *= i
         b /= 1 / i
         assert torch.sum(a - b) < self.epsilon
 
+    @pytest.mark.skipif(not torch.cuda.is_available(), reason="requires PyTorch CUDA")
     @pytest.mark.skipif(torch.__version__ < "1.12", reason="requires PyTorch 1.12 or higher")
     @pytest.mark.parametrize(
         "i",
         [
             NestedTensor([[6, 5, 4], [3, 2]]),
             torch.tensor([[6, 5, 4], [3, 2, 1]]),
             torch.randn(2, 3),
@@ -104,14 +105,15 @@
     def test_pow_log(self, i):
         a = self.nested_tensor.clone().float()
         b = a.clone()
         assert torch.sum(torch.log(a**i) / torch.log(a) - i) < self.epsilon
         a **= i
         assert torch.sum(torch.log(a) / torch.log(b) - i) < self.epsilon
 
+    @pytest.mark.skipif(not torch.cuda.is_available(), reason="requires PyTorch CUDA")
     @pytest.mark.skipif(torch.__version__ < "2.1", reason="requires PyTorch 2.1 or higher")
     @pytest.mark.parametrize(
         "i",
         [
             NestedTensor([[6, 5, 4], [3, 2]]),
             torch.tensor([[6, 5, 4], [3, 2, 1]]),
             1,
@@ -123,14 +125,15 @@
         assert torch.sum(a >> i << i - a) < self.epsilon
         b = a.clone()
         b <<= i
         assert torch.sum(a << i - b) < self.epsilon
         b >>= i
         assert torch.sum(a - b) < self.epsilon
 
+    @pytest.mark.skipif(not torch.cuda.is_available(), reason="requires PyTorch CUDA")
     @pytest.mark.parametrize(
         "i",
         [
             NestedTensor([[6, 5, 4], [3, 2]]),
             torch.tensor([[6, 5, 4], [3, 2, 1]]),
             torch.randint(0, 9, (2, 3)),
             1,
```

### Comparing `danling-0.3.4/tests/utils/test_decorators.py` & `danling-0.3.5/tests/utils/test_decorators.py`

 * *Files identical despite different names*

