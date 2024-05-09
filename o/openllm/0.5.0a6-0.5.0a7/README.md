# Comparing `tmp/openllm-0.5.0a6.tar.gz` & `tmp/openllm-0.5.0a7.tar.gz`

## Comparing `openllm-0.5.0a6.tar` & `openllm-0.5.0a7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    42622 2020-02-02 00:00:00.000000 openllm-0.5.0a6/CHANGELOG.md
--rw-r--r--   0        0        0    40681 2020-02-02 00:00:00.000000 openllm-0.5.0a6/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a6/pyoxidizer.bzl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_service_vars.pyi
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/Dockerfile.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/__init__.pyi
--rw-r--r--   0        0        0    19278 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/_entrypoint.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/_helpers.py
--rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/_llm.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/_service.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/_service_vars.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/_openllm_tiny/bentofile.yaml
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/__init__.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/__main__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_deprecated.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_generation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_generation.pyi
--rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_llm.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_llm.pyi
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_quantisation.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_quantisation.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_runners.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_runners.pyi
--rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_strategies.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_strategies.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/_version.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/client.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/client.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/py.typed
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/utils.pyi
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/bundle/__init__.pyi
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/bundle/_package.pyi
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/__init__.pyi
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/_openapi.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/_openapi.pyi
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/hf.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/hf.pyi
--rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/openai.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/entrypoints/openai.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/__init__.pyi
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/_helpers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/ggml/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/transformers/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/transformers/_helpers.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/transformers/weights.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm/serialisation/vllm/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/__init__.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/_factory.py
--rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/_sdk.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/termui.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/dive_bentos.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/get_containerfile.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/get_prompt.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/list_bentos.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/list_models.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/extension/playground.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/_meta.yml
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/features.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a6/src/openllm_cli/playground/opt_tuned.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a6/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a6/LICENSE.md
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 openllm-0.5.0a6/pyproject.toml
--rw-r--r--   0        0        0    47179 2020-02-02 00:00:00.000000 openllm-0.5.0a6/PKG-INFO
+-rw-r--r--   0        0        0    42723 2020-02-02 00:00:00.000000 openllm-0.5.0a7/CHANGELOG.md
+-rw-r--r--   0        0        0    40681 2020-02-02 00:00:00.000000 openllm-0.5.0a7/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a7/pyoxidizer.bzl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_service_vars.pyi
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/Dockerfile.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/__init__.pyi
+-rw-r--r--   0        0        0    19157 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/_entrypoint.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/_helpers.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/_llm.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/_service.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/_service_vars.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/_openllm_tiny/bentofile.yaml
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/__init__.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/__main__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_deprecated.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_generation.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_generation.pyi
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_llm.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_llm.pyi
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_quantisation.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_runners.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_runners.pyi
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_strategies.pyi
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/_version.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/client.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/client.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/py.typed
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/utils.pyi
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/bundle/__init__.pyi
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/bundle/_package.pyi
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/__init__.pyi
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/_openapi.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/_openapi.pyi
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/hf.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/hf.pyi
+-rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/openai.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/entrypoints/openai.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/__init__.pyi
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/_helpers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/ggml/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/transformers/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/transformers/_helpers.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/transformers/weights.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm/serialisation/vllm/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/__init__.py
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/_factory.py
+-rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/_sdk.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/termui.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/dive_bentos.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/get_containerfile.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/get_prompt.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/list_bentos.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/list_models.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/extension/playground.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/__init__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/_meta.yml
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/features.py
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a7/src/openllm_cli/playground/opt_tuned.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a7/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a7/LICENSE.md
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 openllm-0.5.0a7/pyproject.toml
+-rw-r--r--   0        0        0    47179 2020-02-02 00:00:00.000000 openllm-0.5.0a7/PKG-INFO
```

### Comparing `openllm-0.5.0a6/CHANGELOG.md` & `openllm-0.5.0a7/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.5.0-alpha.7](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.7)
+No significant changes.
+
+
 ## [0.5.0-alpha.6](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.6)
 No significant changes.
 
 
 ## [0.5.0-alpha.5](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.5)
 No significant changes.
```

### Comparing `openllm-0.5.0a6/README.md` & `openllm-0.5.0a7/README.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/pyoxidizer.bzl` & `openllm-0.5.0a7/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_service_vars.pyi` & `openllm-0.5.0a7/src/_service_vars.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/__init__.pyi` & `openllm-0.5.0a7/src/_openllm_tiny/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/_entrypoint.py` & `openllm-0.5.0a7/src/_openllm_tiny/_entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,18 +457,15 @@
         version=bento_tag.version,
         build_ctx=llm_fs.getsyspath('/'),
         build_config=BentoBuildConfig(
           service=f"{llm_config['service_name']}:LLMService",
           name=bento_tag.name,
           labels=labels,
           models=models,
-          envs=[
-            EnvironmentEntry(name='OPENLLM_CONFIG', value=f"'{llm_config.model_dump_json()}'"),
-            EnvironmentEntry(name='NVIDIA_DRIVER_CAPABILITIES', value='compute,utility'),
-          ],
+          envs=[EnvironmentEntry(name='NVIDIA_DRIVER_CAPABILITIES', value='compute,utility')],
           description=f"OpenLLM service for {llm_config['start_name']}",
           include=list(llm_fs.walk.files()),
           exclude=['/venv', '/.venv', '__pycache__/', '*.py[cod]', '*$py.class'],
           python=construct_python_options(llm_config, llm_fs),
           docker=DockerOptions(python_version='3.11'),
         ),
       ).save(bento_store=BentoMLContainer.bento_store.get(), model_store=BentoMLContainer.model_store.get())
```

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/_helpers.py` & `openllm-0.5.0a7/src/_openllm_tiny/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/_llm.py` & `openllm-0.5.0a7/src/_openllm_tiny/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/_service.py` & `openllm-0.5.0a7/src/_openllm_tiny/_service.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/_openllm_tiny/_service_vars.py` & `openllm-0.5.0a7/src/_openllm_tiny/_service_vars.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/__init__.py` & `openllm-0.5.0a7/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/__init__.pyi` & `openllm-0.5.0a7/src/openllm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_deprecated.py` & `openllm-0.5.0a7/src/openllm/_deprecated.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_generation.py` & `openllm-0.5.0a7/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_llm.py` & `openllm-0.5.0a7/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_llm.pyi` & `openllm-0.5.0a7/src/openllm/_llm.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_quantisation.py` & `openllm-0.5.0a7/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_quantisation.pyi` & `openllm-0.5.0a7/src/openllm/_quantisation.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_runners.py` & `openllm-0.5.0a7/src/openllm/_runners.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_runners.pyi` & `openllm-0.5.0a7/src/openllm/_runners.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_strategies.py` & `openllm-0.5.0a7/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/_strategies.pyi` & `openllm-0.5.0a7/src/openllm/_strategies.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/utils.py` & `openllm-0.5.0a7/src/openllm/utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/utils.pyi` & `openllm-0.5.0a7/src/openllm/utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/bundle/__init__.py` & `openllm-0.5.0a7/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/bundle/__init__.pyi` & `openllm-0.5.0a7/src/openllm/bundle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/bundle/_package.py` & `openllm-0.5.0a7/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/bundle/_package.pyi` & `openllm-0.5.0a7/src/openllm/bundle/_package.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/entrypoints/_openapi.py` & `openllm-0.5.0a7/src/openllm/entrypoints/_openapi.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/entrypoints/_openapi.pyi` & `openllm-0.5.0a7/src/openllm/entrypoints/_openapi.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/entrypoints/hf.py` & `openllm-0.5.0a7/src/openllm/entrypoints/hf.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/entrypoints/openai.py` & `openllm-0.5.0a7/src/openllm/entrypoints/openai.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/entrypoints/openai.pyi` & `openllm-0.5.0a7/src/openllm/entrypoints/openai.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/__init__.py` & `openllm-0.5.0a7/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/__init__.pyi` & `openllm-0.5.0a7/src/openllm/serialisation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/_helpers.py` & `openllm-0.5.0a7/src/openllm/serialisation/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/transformers/__init__.py` & `openllm-0.5.0a7/src/openllm/serialisation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/transformers/_helpers.py` & `openllm-0.5.0a7/src/openllm/serialisation/transformers/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/transformers/weights.py` & `openllm-0.5.0a7/src/openllm/serialisation/transformers/weights.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm/serialisation/vllm/__init__.py` & `openllm-0.5.0a7/src/openllm/serialisation/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/_factory.py` & `openllm-0.5.0a7/src/openllm_cli/_factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/_sdk.py` & `openllm-0.5.0a7/src/openllm_cli/_sdk.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/termui.py` & `openllm-0.5.0a7/src/openllm_cli/termui.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/__init__.py` & `openllm-0.5.0a7/src/openllm_cli/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/dive_bentos.py` & `openllm-0.5.0a7/src/openllm_cli/extension/dive_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/get_containerfile.py` & `openllm-0.5.0a7/src/openllm_cli/extension/get_containerfile.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/get_prompt.py` & `openllm-0.5.0a7/src/openllm_cli/extension/get_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/list_bentos.py` & `openllm-0.5.0a7/src/openllm_cli/extension/list_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/list_models.py` & `openllm-0.5.0a7/src/openllm_cli/extension/list_models.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/extension/playground.py` & `openllm-0.5.0a7/src/openllm_cli/extension/playground.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/playground/_meta.yml` & `openllm-0.5.0a7/src/openllm_cli/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/playground/falcon_tuned.py` & `openllm-0.5.0a7/src/openllm_cli/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/playground/features.py` & `openllm-0.5.0a7/src/openllm_cli/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/playground/llama2_qlora.py` & `openllm-0.5.0a7/src/openllm_cli/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/src/openllm_cli/playground/opt_tuned.py` & `openllm-0.5.0a7/src/openllm_cli/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/.gitignore` & `openllm-0.5.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/LICENSE.md` & `openllm-0.5.0a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a6/pyproject.toml` & `openllm-0.5.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "bentoml[io]>=1.2",
     "transformers[torch,tokenizers]>=4.36.0",
-    "openllm-client>=0.5.0-alpha.6",
-    "openllm-core>=0.5.0-alpha.6",
+    "openllm-client>=0.5.0-alpha.7",
+    "openllm-core>=0.5.0-alpha.7",
     "safetensors",
     "vllm>=0.4.2",
     "optimum>=1.12.0",
     "accelerate",
     "ghapi",
     "einops",
     "sentencepiece",
```

### Comparing `openllm-0.5.0a6/PKG-INFO` & `openllm-0.5.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm
-Version: 0.5.0a6
+Version: 0.5.0a7
 Summary: OpenLLM: Run any open-source LLMs, such as Llama 2, Mistral, as OpenAI compatible API endpoint in the cloud.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://discord.gg/openllm
 Project-URL: Documentation, https://github.com/bentoml/openllm#readme
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -42,16 +42,16 @@
 Requires-Dist: bentoml[io]>=1.2
 Requires-Dist: bitsandbytes<0.42
 Requires-Dist: build[virtualenv]<1
 Requires-Dist: click>=8.1.3
 Requires-Dist: cuda-python; platform_system != 'Darwin'
 Requires-Dist: einops
 Requires-Dist: ghapi
-Requires-Dist: openllm-client>=0.5.0-alpha.6
-Requires-Dist: openllm-core>=0.5.0-alpha.6
+Requires-Dist: openllm-client>=0.5.0-alpha.7
+Requires-Dist: openllm-core>=0.5.0-alpha.7
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: safetensors
 Requires-Dist: scipy
 Requires-Dist: sentencepiece
 Requires-Dist: transformers[tokenizers,torch]>=4.36.0
 Requires-Dist: vllm>=0.4.2
 Provides-Extra: agents
```

