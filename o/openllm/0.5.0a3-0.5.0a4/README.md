# Comparing `tmp/openllm-0.5.0a3.tar.gz` & `tmp/openllm-0.5.0a4.tar.gz`

## Comparing `openllm-0.5.0a3.tar` & `openllm-0.5.0a4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    42319 2020-02-02 00:00:00.000000 openllm-0.5.0a3/CHANGELOG.md
--rw-r--r--   0        0        0    46908 2020-02-02 00:00:00.000000 openllm-0.5.0a3/README.md
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a3/pyoxidizer.bzl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_service_vars.pyi
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/Dockerfile.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/__init__.pyi
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/_entrypoint.py
--rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/_helpers.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/_llm.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/_service.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/_service_vars.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/_openllm_tiny/bentofile.yaml
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/__init__.pyi
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/__main__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_deprecated.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_generation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_generation.pyi
--rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_llm.py
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_llm.pyi
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_quantisation.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_quantisation.pyi
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_runners.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_runners.pyi
--rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_strategies.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_strategies.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/_version.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/client.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/client.pyi
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/py.typed
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/utils.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/utils.pyi
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/bundle/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/bundle/__init__.pyi
--rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/bundle/_package.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/bundle/_package.pyi
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/__init__.pyi
--rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/_openapi.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/_openapi.pyi
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/hf.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/hf.pyi
--rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/openai.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/entrypoints/openai.pyi
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/models/__init__.py
--rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/__init__.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/__init__.pyi
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/_helpers.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/constants.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/ggml/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/transformers/__init__.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/transformers/_helpers.py
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/transformers/weights.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm/serialisation/vllm/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/__init__.py
--rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/_factory.py
--rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/_sdk.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/termui.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/dive_bentos.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/get_containerfile.py
--rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/get_prompt.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/list_bentos.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/list_models.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/extension/playground.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/__init__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/_meta.yml
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/falcon_tuned.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/features.py
--rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/llama2_qlora.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a3/src/openllm_cli/playground/opt_tuned.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a3/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a3/LICENSE.md
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 openllm-0.5.0a3/pyproject.toml
--rw-r--r--   0        0        0    53335 2020-02-02 00:00:00.000000 openllm-0.5.0a3/PKG-INFO
+-rw-r--r--   0        0        0    42420 2020-02-02 00:00:00.000000 openllm-0.5.0a4/CHANGELOG.md
+-rw-r--r--   0        0        0    40681 2020-02-02 00:00:00.000000 openllm-0.5.0a4/README.md
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 openllm-0.5.0a4/pyoxidizer.bzl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_service_vars.pyi
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/Dockerfile.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/__init__.pyi
+-rw-r--r--   0        0        0    19286 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/_entrypoint.py
+-rw-r--r--   0        0        0    12945 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/_helpers.py
+-rw-r--r--   0        0        0     7733 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/_llm.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/_service.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/_service_vars.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/_openllm_tiny/bentofile.yaml
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/__init__.pyi
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/__main__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_deprecated.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_generation.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_generation.pyi
+-rw-r--r--   0        0        0    19732 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_llm.py
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_llm.pyi
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_quantisation.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_quantisation.pyi
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_runners.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_runners.pyi
+-rw-r--r--   0        0        0    12147 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_strategies.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_strategies.pyi
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/_version.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/client.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/client.pyi
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/py.typed
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/utils.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/utils.pyi
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/bundle/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/bundle/__init__.pyi
+-rw-r--r--   0        0        0     6054 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/bundle/_package.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/bundle/_package.pyi
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/__init__.pyi
+-rw-r--r--   0        0        0    20050 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/_openapi.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/_openapi.pyi
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/hf.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/hf.pyi
+-rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/openai.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/entrypoints/openai.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/models/__init__.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/__init__.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/__init__.pyi
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/_helpers.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/constants.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/ggml/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/transformers/__init__.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/transformers/_helpers.py
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/transformers/weights.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm/serialisation/vllm/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/__init__.py
+-rw-r--r--   0        0        0    12396 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/_factory.py
+-rw-r--r--   0        0        0    12850 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/_sdk.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/termui.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/dive_bentos.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/get_containerfile.py
+-rw-r--r--   0        0        0     6734 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/get_prompt.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/list_bentos.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/list_models.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/extension/playground.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/__init__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/_meta.yml
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/falcon_tuned.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/features.py
+-rw-r--r--   0        0        0     8315 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/llama2_qlora.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 openllm-0.5.0a4/src/openllm_cli/playground/opt_tuned.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm-0.5.0a4/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm-0.5.0a4/LICENSE.md
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 openllm-0.5.0a4/pyproject.toml
+-rw-r--r--   0        0        0    47179 2020-02-02 00:00:00.000000 openllm-0.5.0a4/PKG-INFO
```

### Comparing `openllm-0.5.0a3/CHANGELOG.md` & `openllm-0.5.0a4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 Do *NOT* add changelog entries here!
 
 This changelog is managed by towncrier and is compiled at release time.
 -->
 
 <!-- towncrier release notes start -->
 
+## [0.5.0-alpha.4](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.4)
+No significant changes.
+
+
 ## [0.5.0-alpha.3](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.3)
 No significant changes.
 
 
 ## [0.5.0-alpha.2](https://github.com/bentoml/openllm/tree/v0.5.0-alpha.2)
 No significant changes.
```

### Comparing `openllm-0.5.0a3/README.md` & `openllm-0.5.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,2932 +1,2949 @@
-00000000: 215b 4261 6e6e 6572 2066 6f72 204f 7065  ![Banner for Ope
-00000010: 6e4c 4c4d 5d28 2f2e 6769 7468 7562 2f61  nLLM](/.github/a
-00000020: 7373 6574 732f 6d61 696e 2d62 616e 6e65  ssets/main-banne
-00000030: 722e 706e 6729 0a0a 3c21 2d2d 2068 6174  r.png)..<!-- hat
-00000040: 6368 2d66 616e 6379 2d70 7970 692d 7265  ch-fancy-pypi-re
-00000050: 6164 6d65 2069 6e74 726f 2073 7461 7274  adme intro start
-00000060: 202d 2d3e 0a0a 3c64 6976 2061 6c69 676e   -->..<div align
-00000070: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
-00000080: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-00000090: 223e f09f a6be 204f 7065 6e4c 4c4d 3c2f  ">.... OpenLLM</
-000000a0: 6831 3e0a 2020 2020 3c61 2068 7265 663d  h1>.    <a href=
-000000b0: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-000000c0: 672f 7072 6f6a 6563 742f 6f70 656e 6c6c  g/project/openll
-000000d0: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
-000000e0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000000f0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000100: 692f 762f 6f70 656e 6c6c 6d2e 7376 673f  i/v/openllm.svg?
-00000110: 6c6f 676f 3d70 7970 6926 6c61 6265 6c3d  logo=pypi&label=
-00000120: 5079 5049 266c 6f67 6f43 6f6c 6f72 3d67  PyPI&logoColor=g
-00000130: 6f6c 6422 2061 6c74 3d22 7079 7069 5f73  old" alt="pypi_s
-00000140: 7461 7475 7322 202f 3e0a 2020 2020 3c2f  tatus" />.    </
-00000150: 613e 3c61 2068 7265 663d 2268 7474 7073  a><a href="https
-00000160: 3a2f 2f74 6573 742e 7079 7069 2e6f 7267  ://test.pypi.org
-00000170: 2f70 726f 6a65 6374 2f6f 7065 6e6c 6c6d  /project/openllm
-00000180: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
-00000190: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000001a0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000001b0: 6765 2f4e 6967 6874 6c79 2d50 7950 493f  ge/Nightly-PyPI?
-000001c0: 6c6f 676f 3d70 7970 6926 6c61 6265 6c3d  logo=pypi&label=
-000001d0: 5079 5049 2663 6f6c 6f72 3d67 7261 7926  PyPI&color=gray&
-000001e0: 6c69 6e6b 3d68 7474 7073 2533 4125 3246  link=https%3A%2F
-000001f0: 2532 4674 6573 742e 7079 7069 2e6f 7267  %2Ftest.pypi.org
-00000200: 2532 4670 726f 6a65 6374 2532 466f 7065  %2Fproject%2Fope
-00000210: 6e6c 6c6d 2532 4622 2061 6c74 3d22 7465  nllm%2F" alt="te
-00000220: 7374 5f70 7970 695f 7374 6174 7573 2220  st_pypi_status" 
-00000230: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-00000240: 6566 3d22 6874 7470 733a 2f2f 7477 6974  ef="https://twit
-00000250: 7465 722e 636f 6d2f 6265 6e74 6f6d 6c61  ter.com/bentomla
-00000260: 6922 3e0a 2020 2020 2020 2020 3c69 6d67  i">.        <img
-00000270: 2073 7263 3d22 6874 7470 733a 2f2f 6261   src="https://ba
-00000280: 6467 656e 2e6e 6574 2f62 6164 6765 2f69  dgen.net/badge/i
-00000290: 636f 6e2f 4062 656e 746f 6d6c 6169 2f31  con/@bentomlai/1
-000002a0: 4441 3146 323f 6963 6f6e 3d74 7769 7474  DA1F2?icon=twitt
-000002b0: 6572 266c 6162 656c 3d46 6f6c 6c6f 7725  er&label=Follow%
-000002c0: 3230 5573 2220 616c 743d 2254 7769 7474  20Us" alt="Twitt
-000002d0: 6572 2220 2f3e 0a20 2020 203c 2f61 3e3c  er" />.    </a><
-000002e0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000002f0: 6c2e 6265 6e74 6f6d 6c2e 636f 6d2f 6a6f  l.bentoml.com/jo
-00000300: 696e 2d6f 7065 6e6c 6c6d 2d64 6973 636f  in-openllm-disco
-00000310: 7264 223e 0a20 2020 2020 2020 203c 696d  rd">.        <im
-00000320: 6720 7372 633d 2268 7474 7073 3a2f 2f62  g src="https://b
-00000330: 6164 6765 6e2e 6e65 742f 6261 6467 652f  adgen.net/badge/
-00000340: 6963 6f6e 2f4f 7065 6e4c 4c4d 2f37 3238  icon/OpenLLM/728
-00000350: 3964 613f 6963 6f6e 3d64 6973 636f 7264  9da?icon=discord
-00000360: 266c 6162 656c 3d4a 6f69 6e25 3230 5573  &label=Join%20Us
-00000370: 2220 616c 743d 2244 6973 636f 7264 2220  " alt="Discord" 
-00000380: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-00000390: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-000003a0: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-000003b0: 7065 6e4c 4c4d 2f61 6374 696f 6e73 2f77  penLLM/actions/w
-000003c0: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c22  orkflows/ci.yml"
-000003d0: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-000003e0: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-000003f0: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-00000400: 7065 6e4c 4c4d 2f61 6374 696f 6e73 2f77  penLLM/actions/w
-00000410: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c2f  orkflows/ci.yml/
-00000420: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-00000430: 3d6d 6169 6e22 2061 6c74 3d22 6369 2220  =main" alt="ci" 
-00000440: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-00000450: 6566 3d22 6874 7470 733a 2f2f 7265 7375  ef="https://resu
-00000460: 6c74 732e 7072 652d 636f 6d6d 6974 2e63  lts.pre-commit.c
-00000470: 692f 6c61 7465 7374 2f67 6974 6875 622f  i/latest/github/
-00000480: 6265 6e74 6f6d 6c2f 4f70 656e 4c4c 4d2f  bentoml/OpenLLM/
-00000490: 6d61 696e 223e 0a20 2020 2020 2020 203c  main">.        <
-000004a0: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-000004b0: 2f72 6573 756c 7473 2e70 7265 2d63 6f6d  /results.pre-com
-000004c0: 6d69 742e 6369 2f62 6164 6765 2f67 6974  mit.ci/badge/git
-000004d0: 6875 622f 6265 6e74 6f6d 6c2f 4f70 656e  hub/bentoml/Open
-000004e0: 4c4c 4d2f 6d61 696e 2e73 7667 2220 616c  LLM/main.svg" al
-000004f0: 743d 2270 7265 2d63 6f6d 6d69 742e 6369  t="pre-commit.ci
-00000500: 2073 7461 7475 7322 202f 3e0a 2020 2020   status" />.    
-00000510: 3c2f 613e 3c62 723e 0a20 2020 203c 6120  </a><br>.    <a 
-00000520: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00000530: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6f  pi.org/project/o
-00000540: 7065 6e6c 6c6d 223e 0a20 2020 2020 2020  penllm">.       
-00000550: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000560: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000570: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00000580: 732f 6f70 656e 6c6c 6d2e 7376 673f 6c6f  s/openllm.svg?lo
-00000590: 676f 3d70 7974 686f 6e26 6c61 6265 6c3d  go=python&label=
-000005a0: 5079 7468 6f6e 266c 6f67 6f43 6f6c 6f72  Python&logoColor
-000005b0: 3d67 6f6c 6422 2061 6c74 3d22 7079 7468  =gold" alt="pyth
-000005c0: 6f6e 5f76 6572 7369 6f6e 2220 2f3e 0a20  on_version" />. 
-000005d0: 2020 203c 2f61 3e3c 6120 6872 6566 3d22     </a><a href="
-000005e0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000005f0: 6f6d 2f70 7970 612f 6861 7463 6822 3e0a  om/pypa/hatch">.
-00000600: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00000610: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00000620: 6965 6c64 732e 696f 2f62 6164 6765 2f25  ields.io/badge/%
-00000630: 4630 2539 4625 4135 2539 412d 4861 7463  F0%9F%A5%9A-Hatc
-00000640: 682d 3430 3531 6235 2e73 7667 2220 616c  h-4051b5.svg" al
-00000650: 743d 2248 6174 6368 2220 2f3e 0a20 2020  t="Hatch" />.   
-00000660: 203c 2f61 3e3c 6120 6872 6566 3d22 6874   </a><a href="ht
-00000670: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000680: 2f62 656e 746f 6d6c 2f4f 7065 6e4c 4c4d  /bentoml/OpenLLM
-00000690: 2f62 6c6f 622f 6d61 696e 2f53 5459 4c45  /blob/main/STYLE
-000006a0: 2e6d 6422 3e0a 2020 2020 2020 2020 3c69  .md">.        <i
-000006b0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000006c0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000006d0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-000006e0: 652d 476f 6f67 6c65 2d30 3030 3030 302e  e-Google-000000.
-000006f0: 7376 6722 2061 6c74 3d22 636f 6465 2073  svg" alt="code s
-00000700: 7479 6c65 2220 2f3e 0a20 2020 203c 2f61  tyle" />.    </a
-00000710: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00000720: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7374  //github.com/ast
-00000730: 7261 6c2d 7368 2f72 7566 6622 3e0a 2020  ral-sh/ruff">.  
-00000740: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
-00000750: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000760: 6c64 732e 696f 2f65 6e64 706f 696e 743f  lds.io/endpoint?
-00000770: 7572 6c3d 6874 7470 733a 2f2f 7261 772e  url=https://raw.
-00000780: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00000790: 742e 636f 6d2f 6368 6172 6c69 6572 6d61  t.com/charlierma
-000007a0: 7273 682f 7275 6666 2f6d 6169 6e2f 6173  rsh/ruff/main/as
-000007b0: 7365 7473 2f62 6164 6765 2f76 322e 6a73  sets/badge/v2.js
-000007c0: 6f6e 2220 616c 743d 2252 7566 6622 202f  on" alt="Ruff" /
-000007d0: 3e0a 2020 2020 3c2f 613e 3c61 2068 7265  >.    </a><a hre
-000007e0: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-000007f0: 622e 636f 6d2f 7079 7468 6f6e 2f6d 7970  b.com/python/myp
-00000800: 7922 3e0a 2020 2020 2020 2020 3c69 6d67  y">.        <img
-00000810: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000820: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000830: 6765 2f74 7970 6573 2d6d 7970 792d 626c  ge/types-mypy-bl
-00000840: 7565 2e73 7667 2220 616c 743d 2274 7970  ue.svg" alt="typ
-00000850: 6573 202d 206d 7970 7922 202f 3e0a 2020  es - mypy" />.  
-00000860: 2020 3c2f 613e 3c61 2068 7265 663d 2268    </a><a href="h
-00000870: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000880: 6d2f 6d69 6372 6f73 6f66 742f 7079 7269  m/microsoft/pyri
-00000890: 6768 7422 3e0a 2020 2020 2020 2020 3c69  ght">.        <i
-000008a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000008b0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-000008c0: 6164 6765 2f74 7970 6573 2d70 7972 6967  adge/types-pyrig
-000008d0: 6874 2d79 656c 6c6f 772e 7376 6722 2061  ht-yellow.svg" a
-000008e0: 6c74 3d22 7479 7065 7320 2d20 7079 7269  lt="types - pyri
-000008f0: 6768 7422 202f 3e0a 2020 2020 3c2f 613e  ght" />.    </a>
-00000900: 3c62 723e 0a20 2020 203c 703e 416e 206f  <br>.    <p>An o
-00000910: 7065 6e20 706c 6174 666f 726d 2066 6f72  pen platform for
-00000920: 206f 7065 7261 7469 6e67 206c 6172 6765   operating large
-00000930: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00000940: 2028 4c4c 4d73 2920 696e 2070 726f 6475   (LLMs) in produ
-00000950: 6374 696f 6e2e 3c2f 6272 3e0a 2020 2020  ction.</br>.    
-00000960: 4669 6e65 2d74 756e 652c 2073 6572 7665  Fine-tune, serve
-00000970: 2c20 6465 706c 6f79 2c20 616e 6420 6d6f  , deploy, and mo
-00000980: 6e69 746f 7220 616e 7920 4c4c 4d73 2077  nitor any LLMs w
-00000990: 6974 6820 6561 7365 2e3c 2f70 3e0a 2020  ith ease.</p>.  
-000009a0: 2020 3c69 3e3c 2f69 3e0a 3c2f 6469 763e    <i></i>.</div>
-000009b0: 0a0a 2323 20f0 9f93 9620 496e 7472 6f64  ..## .... Introd
-000009c0: 7563 7469 6f6e 0a0a 4f70 656e 4c4c 4d20  uction..OpenLLM 
-000009d0: 6973 2061 6e20 6f70 656e 2d73 6f75 7263  is an open-sourc
-000009e0: 6520 706c 6174 666f 726d 2064 6573 6967  e platform desig
-000009f0: 6e65 6420 746f 2066 6163 696c 6974 6174  ned to facilitat
-00000a00: 6520 7468 6520 6465 706c 6f79 6d65 6e74  e the deployment
-00000a10: 2061 6e64 206f 7065 7261 7469 6f6e 206f   and operation o
-00000a20: 6620 6c61 7267 6520 6c61 6e67 7561 6765  f large language
-00000a30: 206d 6f64 656c 7320 284c 4c4d 7329 2069   models (LLMs) i
-00000a40: 6e20 7265 616c 2d77 6f72 6c64 2061 7070  n real-world app
-00000a50: 6c69 6361 7469 6f6e 732e 2057 6974 6820  lications. With 
-00000a60: 4f70 656e 4c4c 4d2c 2079 6f75 2063 616e  OpenLLM, you can
-00000a70: 2072 756e 2069 6e66 6572 656e 6365 206f   run inference o
-00000a80: 6e20 616e 7920 6f70 656e 2d73 6f75 7263  n any open-sourc
-00000a90: 6520 4c4c 4d2c 2064 6570 6c6f 7920 7468  e LLM, deploy th
-00000aa0: 656d 206f 6e20 7468 6520 636c 6f75 6420  em on the cloud 
-00000ab0: 6f72 206f 6e2d 7072 656d 6973 6573 2c20  or on-premises, 
-00000ac0: 616e 6420 6275 696c 6420 706f 7765 7266  and build powerf
-00000ad0: 756c 2041 4920 6170 706c 6963 6174 696f  ul AI applicatio
-00000ae0: 6e73 2e0a 0a4b 6579 2066 6561 7475 7265  ns...Key feature
-00000af0: 7320 696e 636c 7564 653a 0a0a f09f 9a82  s include:......
-00000b00: 202a 2a53 7461 7465 2d6f 662d 7468 652d   **State-of-the-
-00000b10: 6172 7420 4c4c 4d73 2a2a 3a20 496e 7465  art LLMs**: Inte
-00000b20: 6772 6174 6564 2073 7570 706f 7274 2066  grated support f
-00000b30: 6f72 2061 2077 6964 6520 7261 6e67 6520  or a wide range 
-00000b40: 6f66 206f 7065 6e2d 736f 7572 6365 204c  of open-source L
-00000b50: 4c4d 7320 616e 6420 6d6f 6465 6c20 7275  LMs and model ru
-00000b60: 6e74 696d 6573 2c20 696e 636c 7564 696e  ntimes, includin
-00000b70: 6720 6275 7420 6e6f 7420 6c69 6d69 7465  g but not limite
-00000b80: 6420 746f 204c 6c61 6d61 2032 2c20 5374  d to Llama 2, St
-00000b90: 6162 6c65 4c4d 2c20 4661 6c63 6f6e 2c20  ableLM, Falcon, 
-00000ba0: 446f 6c6c 792c 2046 6c61 6e2d 5435 2c20  Dolly, Flan-T5, 
-00000bb0: 4368 6174 474c 4d2c 2061 6e64 2053 7461  ChatGLM, and Sta
-00000bc0: 7243 6f64 6572 2e0a 0af0 9f94 a520 2a2a  rCoder....... **
-00000bd0: 466c 6578 6962 6c65 2041 5049 732a 2a3a  Flexible APIs**:
-00000be0: 2053 6572 7665 204c 4c4d 7320 6f76 6572   Serve LLMs over
-00000bf0: 2061 2052 4553 5466 756c 2041 5049 206f   a RESTful API o
-00000c00: 7220 6752 5043 2077 6974 6820 6120 7369  r gRPC with a si
-00000c10: 6e67 6c65 2063 6f6d 6d61 6e64 2e20 596f  ngle command. Yo
-00000c20: 7520 6361 6e20 696e 7465 7261 6374 2077  u can interact w
-00000c30: 6974 6820 7468 6520 6d6f 6465 6c20 7573  ith the model us
-00000c40: 696e 6720 6120 5765 6220 5549 2c20 434c  ing a Web UI, CL
-00000c50: 492c 2050 7974 686f 6e2f 4a61 7661 5363  I, Python/JavaSc
-00000c60: 7269 7074 2063 6c69 656e 7473 2c20 6f72  ript clients, or
-00000c70: 2061 6e79 2048 5454 5020 636c 6965 6e74   any HTTP client
-00000c80: 206f 6620 796f 7572 2063 686f 6963 652e   of your choice.
-00000c90: 0a0a e29b 93ef b88f 202a 2a46 7265 6564  ........ **Freed
-00000ca0: 6f6d 2074 6f20 6275 696c 642a 2a3a 2046  om to build**: F
-00000cb0: 6972 7374 2d63 6c61 7373 2073 7570 706f  irst-class suppo
-00000cc0: 7274 2066 6f72 204c 616e 6743 6861 696e  rt for LangChain
-00000cd0: 2c20 4265 6e74 6f4d 4c2c 204c 6c61 6d61  , BentoML, Llama
-00000ce0: 496e 6465 782c 204f 7065 6e41 4920 656e  Index, OpenAI en
-00000cf0: 6470 6f69 6e74 732c 2061 6e64 2048 7567  dpoints, and Hug
-00000d00: 6769 6e67 2046 6163 652c 2061 6c6c 6f77  ging Face, allow
-00000d10: 696e 6720 796f 7520 746f 2065 6173 696c  ing you to easil
-00000d20: 7920 6372 6561 7465 2079 6f75 7220 6f77  y create your ow
-00000d30: 6e20 4149 2061 7070 6c69 6361 7469 6f6e  n AI application
-00000d40: 7320 6279 2063 6f6d 706f 7369 6e67 204c  s by composing L
-00000d50: 4c4d 7320 7769 7468 206f 7468 6572 206d  LMs with other m
-00000d60: 6f64 656c 7320 616e 6420 7365 7276 6963  odels and servic
-00000d70: 6573 2e0a 0af0 9f8e af20 2a2a 5374 7265  es....... **Stre
-00000d80: 616d 6c69 6e65 2064 6570 6c6f 796d 656e  amline deploymen
-00000d90: 742a 2a3a 2041 7574 6f6d 6174 6963 616c  t**: Automatical
-00000da0: 6c79 2067 656e 6572 6174 6520 796f 7572  ly generate your
-00000db0: 204c 4c4d 2073 6572 7665 7220 446f 636b   LLM server Dock
-00000dc0: 6572 2069 6d61 6765 7320 6f72 2064 6570  er images or dep
-00000dd0: 6c6f 7920 6173 2073 6572 7665 726c 6573  loy as serverles
-00000de0: 7320 656e 6470 6f69 6e74 7320 7669 610a  s endpoints via.
-00000df0: 5be2 9881 efb8 8f20 4265 6e74 6f43 6c6f  [...... BentoClo
-00000e00: 7564 5d28 6874 7470 733a 2f2f 6c2e 6265  ud](https://l.be
-00000e10: 6e74 6f6d 6c2e 636f 6d2f 6265 6e74 6f2d  ntoml.com/bento-
-00000e20: 636c 6f75 6429 2c20 7768 6963 6820 6566  cloud), which ef
-00000e30: 666f 7274 6c65 7373 6c79 206d 616e 6167  fortlessly manag
-00000e40: 6573 2047 5055 2072 6573 6f75 7263 6573  es GPU resources
-00000e50: 2c20 7363 616c 6573 2061 6363 6f72 6469  , scales accordi
-00000e60: 6e67 2074 6f20 7472 6166 6669 632c 2061  ng to traffic, a
-00000e70: 6e64 2065 6e73 7572 6573 2063 6f73 742d  nd ensures cost-
-00000e80: 6566 6665 6374 6976 656e 6573 732e 0a0a  effectiveness...
-00000e90: f09f a496 efb8 8f20 2a2a 4272 696e 6720  ....... **Bring 
-00000ea0: 796f 7572 206f 776e 204c 4c4d 2a2a 3a20  your own LLM**: 
-00000eb0: 4669 6e65 2d74 756e 6520 616e 7920 4c4c  Fine-tune any LL
-00000ec0: 4d20 746f 2073 7569 7420 796f 7572 206e  M to suit your n
-00000ed0: 6565 6473 2e20 596f 7520 6361 6e20 6c6f  eeds. You can lo
-00000ee0: 6164 204c 6f52 4120 6c61 7965 7273 2074  ad LoRA layers t
-00000ef0: 6f20 6669 6e65 2d74 756e 6520 6d6f 6465  o fine-tune mode
-00000f00: 6c73 2066 6f72 2068 6967 6865 7220 6163  ls for higher ac
-00000f10: 6375 7261 6379 2061 6e64 2070 6572 666f  curacy and perfo
-00000f20: 726d 616e 6365 2066 6f72 2073 7065 6369  rmance for speci
-00000f30: 6669 6320 7461 736b 732e 2041 2075 6e69  fic tasks. A uni
-00000f40: 6669 6564 2066 696e 652d 7475 6e69 6e67  fied fine-tuning
-00000f50: 2041 5049 2066 6f72 206d 6f64 656c 7320   API for models 
-00000f60: 2860 4c4c 4d2e 7475 6e69 6e67 2829 6029  (`LLM.tuning()`)
-00000f70: 2069 7320 636f 6d69 6e67 2073 6f6f 6e2e   is coming soon.
-00000f80: 0a0a e29a a1c2 a02a 2a51 7561 6e74 697a  .......**Quantiz
-00000f90: 6174 696f 6e2a 2a3a 2052 756e 2069 6e66  ation**: Run inf
-00000fa0: 6572 656e 6365 2077 6974 6820 6c65 7373  erence with less
-00000fb0: 2063 6f6d 7075 7461 7469 6f6e 616c 2061   computational a
-00000fc0: 6e64 206d 656d 6f72 7920 636f 7374 7320  nd memory costs 
-00000fd0: 7769 7468 2071 7561 6e74 697a 6174 696f  with quantizatio
-00000fe0: 6e20 7465 6368 6e69 7175 6573 2073 7563  n techniques suc
-00000ff0: 6820 6173 205b 4c4c 4d2e 696e 7438 5d28  h as [LLM.int8](
-00001000: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00001010: 672f 6162 732f 3232 3038 2e30 3733 3339  g/abs/2208.07339
-00001020: 292c 205b 5370 5152 2028 696e 7434 295d  ), [SpQR (int4)]
-00001030: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00001040: 7267 2f61 6273 2f32 3330 362e 3033 3037  rg/abs/2306.0307
-00001050: 3829 2c20 5b41 5751 5d28 6874 7470 733a  8), [AWQ](https:
-00001060: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-00001070: 3233 3036 2e30 3039 3738 2e70 6466 292c  2306.00978.pdf),
-00001080: c2a0 5b47 5054 515d 2868 7474 7073 3a2f  ..[GPTQ](https:/
-00001090: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-000010a0: 3231 302e 3137 3332 3329 2c20 616e 6420  210.17323), and 
-000010b0: 5b53 7175 6565 7a65 4c4c 4d5d 2868 7474  [SqueezeLLM](htt
-000010c0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
-000010d0: 6466 2f32 3330 362e 3037 3632 3976 322e  df/2306.07629v2.
-000010e0: 7064 6629 2e0a 0af0 9f93 a1c2 a02a 2a53  pdf).........**S
-000010f0: 7472 6561 6d69 6e67 2a2a 3a20 5375 7070  treaming**: Supp
-00001100: 6f72 7420 746f 6b65 6e20 7374 7265 616d  ort token stream
-00001110: 696e 6720 7468 726f 7567 6820 7365 7276  ing through serv
-00001120: 6572 2d73 656e 7420 6576 656e 7473 2028  er-sent events (
-00001130: 5353 4529 2e20 596f 7520 6361 6e20 7573  SSE). You can us
-00001140: 6520 7468 6520 602f 7631 2f67 656e 6572  e the `/v1/gener
-00001150: 6174 655f 7374 7265 616d 60c2 a065 6e64  ate_stream`..end
-00001160: 706f 696e 7420 666f 7220 7374 7265 616d  point for stream
-00001170: 696e 6720 7265 7370 6f6e 7365 7320 6672  ing responses fr
-00001180: 6f6d 204c 4c4d 732e 0a0a f09f 9484 c2a0  om LLMs.........
-00001190: 2a2a 436f 6e74 696e 756f 7573 2062 6174  **Continuous bat
-000011a0: 6368 696e 672a 2a3a 2053 7570 706f 7274  ching**: Support
-000011b0: 2063 6f6e 7469 6e75 6f75 7320 6261 7463   continuous batc
-000011c0: 6869 6e67 2076 6961 205b 764c 4c4d 5d28  hing via [vLLM](
-000011d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000011e0: 6f6d 2f76 6c6c 6d2d 7072 6f6a 6563 742f  om/vllm-project/
-000011f0: 766c 6c6d 2920 666f 7220 696e 6372 6561  vllm) for increa
-00001200: 7365 6420 746f 7461 6c20 7468 726f 7567  sed total throug
-00001210: 6870 7574 2e0a 0a4f 7065 6e4c 4c4d 2069  hput...OpenLLM i
-00001220: 7320 6465 7369 676e 6564 2066 6f72 2041  s designed for A
-00001230: 4920 6170 706c 6963 6174 696f 6e20 6465  I application de
-00001240: 7665 6c6f 7065 7273 2077 6f72 6b69 6e67  velopers working
-00001250: 2074 6f20 6275 696c 6420 7072 6f64 7563   to build produc
-00001260: 7469 6f6e 2d72 6561 6479 2061 7070 6c69  tion-ready appli
-00001270: 6361 7469 6f6e 7320 6261 7365 6420 6f6e  cations based on
-00001280: 204c 4c4d 732e 2049 7420 6465 6c69 7665   LLMs. It delive
-00001290: 7273 2061 2063 6f6d 7072 6568 656e 7369  rs a comprehensi
-000012a0: 7665 2073 7569 7465 206f 6620 746f 6f6c  ve suite of tool
-000012b0: 7320 616e 6420 6665 6174 7572 6573 2066  s and features f
-000012c0: 6f72 2066 696e 652d 7475 6e69 6e67 2c20  or fine-tuning, 
-000012d0: 7365 7276 696e 672c 2064 6570 6c6f 7969  serving, deployi
-000012e0: 6e67 2c20 616e 6420 6d6f 6e69 746f 7269  ng, and monitori
-000012f0: 6e67 2074 6865 7365 206d 6f64 656c 732c  ng these models,
-00001300: 2073 696d 706c 6966 7969 6e67 2074 6865   simplifying the
-00001310: 2065 6e64 2d74 6f2d 656e 6420 6465 706c   end-to-end depl
-00001320: 6f79 6d65 6e74 2077 6f72 6b66 6c6f 7720  oyment workflow 
-00001330: 666f 7220 4c4c 4d73 2e0a 0a3c 212d 2d20  for LLMs...<!-- 
-00001340: 6861 7463 682d 6661 6e63 792d 7079 7069  hatch-fancy-pypi
-00001350: 2d72 6561 646d 6520 696e 7472 6f20 7374  -readme intro st
-00001360: 6f70 202d 2d3e 0a0a 215b 4769 6620 7368  op -->..![Gif sh
-00001370: 6f77 696e 6720 4f70 656e 4c4c 4d20 496e  owing OpenLLM In
-00001380: 7472 6f5d 282f 2e67 6974 6875 622f 6173  tro](/.github/as
-00001390: 7365 7473 2f6f 7574 7075 742e 6769 6629  sets/output.gif)
-000013a0: 0a0a 3c62 722f 3e0a 0a3c 212d 2d20 6861  ..<br/>..<!-- ha
-000013b0: 7463 682d 6661 6e63 792d 7079 7069 2d72  tch-fancy-pypi-r
-000013c0: 6561 646d 6520 696e 7465 7269 6d20 7374  eadme interim st
-000013d0: 6172 7420 2d2d 3e0a 0a23 2320 f09f 92be  art -->..## ....
-000013e0: 2054 4c2f 4452 0a0a 466f 7220 7374 6172   TL/DR..For star
-000013f0: 7465 722c 2077 6520 7072 6f76 6964 6520  ter, we provide 
-00001400: 7477 6f20 7761 7973 2074 6f20 7175 6963  two ways to quic
-00001410: 6b6c 7920 7472 7920 6f75 7420 4f70 656e  kly try out Open
-00001420: 4c4c 4d3a 0a23 2323 204a 7570 7974 6572  LLM:.### Jupyter
-00001430: 204e 6f74 6562 6f6f 6b73 0a0a 5472 7920   Notebooks..Try 
-00001440: 7468 6973 205b 4f70 656e 4c4c 4d20 7475  this [OpenLLM tu
-00001450: 746f 7269 616c 2069 6e20 476f 6f67 6c65  torial in Google
-00001460: 2043 6f6c 6162 3a20 5365 7276 696e 6720   Colab: Serving 
-00001470: 4c6c 616d 6120 3220 7769 7468 204f 7065  Llama 2 with Ope
-00001480: 6e4c 4c4d 5d28 6874 7470 733a 2f2f 636f  nLLM](https://co
-00001490: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
-000014a0: 676c 652e 636f 6d2f 6769 7468 7562 2f62  gle.com/github/b
-000014b0: 656e 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62  entoml/OpenLLM/b
-000014c0: 6c6f 622f 6d61 696e 2f65 7861 6d70 6c65  lob/main/example
-000014d0: 732f 6c6c 616d 6132 2e69 7079 6e62 292e  s/llama2.ipynb).
-000014e0: 0a0a 2323 2320 446f 636b 6572 0a0a 5765  ..### Docker..We
-000014f0: 2070 726f 7669 6465 2061 2064 6f63 6b65   provide a docke
-00001500: 7220 636f 6e74 6169 6e65 7220 7468 6174  r container that
-00001510: 2068 656c 7073 2079 6f75 2073 7461 7274   helps you start
-00001520: 2072 756e 6e69 6e67 204f 7065 6e4c 4c4d   running OpenLLM
-00001530: 3a0a 0a60 6060 6261 7368 0a64 6f63 6b65  :..```bash.docke
-00001540: 7220 7275 6e20 2d2d 726d 202d 6974 202d  r run --rm -it -
-00001550: 7020 3330 3030 3a33 3030 3020 6768 6372  p 3000:3000 ghcr
-00001560: 2e69 6f2f 6265 6e74 6f6d 6c2f 6f70 656e  .io/bentoml/open
-00001570: 6c6c 6d20 7374 6172 7420 6661 6365 626f  llm start facebo
-00001580: 6f6b 2f6f 7074 2d31 2e33 6220 2d2d 6261  ok/opt-1.3b --ba
-00001590: 636b 656e 6420 7074 0a60 6060 0a0a 3e20  ckend pt.```..> 
-000015a0: 5b21 4e4f 5445 5d0a 3e20 4769 7665 6e20  [!NOTE].> Given 
-000015b0: 796f 7520 6861 7665 2061 6363 6573 7320  you have access 
-000015c0: 746f 2047 5055 7320 616e 6420 6861 7665  to GPUs and have
-000015d0: 2073 6574 7570 205b 6e76 6964 6961 2d64   setup [nvidia-d
-000015e0: 6f63 6b65 725d 2868 7474 7073 3a2f 2f67  ocker](https://g
-000015f0: 6974 6875 622e 636f 6d2f 4e56 4944 4941  ithub.com/NVIDIA
-00001600: 2f6e 7669 6469 612d 636f 6e74 6169 6e65  /nvidia-containe
-00001610: 722d 746f 6f6c 6b69 7429 2c20 2079 6f75  r-toolkit),  you
-00001620: 2063 616e 2061 6464 6974 696f 6e61 6c6c   can additionall
-00001630: 7920 7061 7373 2069 6e20 602d 2d67 7075  y pass in `--gpu
-00001640: 7360 0a3e 2074 6f20 7573 6520 4750 5520  s`.> to use GPU 
-00001650: 666f 7220 6661 7374 6572 2069 6e66 6572  for faster infer
-00001660: 656e 6365 2061 6e64 206f 7074 696d 697a  ence and optimiz
-00001670: 6174 696f 6e0a 3e60 6060 6261 7368 0a3e  ation.>```bash.>
-00001680: 2064 6f63 6b65 7220 7275 6e20 2d2d 726d   docker run --rm
-00001690: 202d 2d67 7075 7320 616c 6c20 2d70 2033   --gpus all -p 3
-000016a0: 3030 303a 3330 3030 202d 6974 2067 6863  000:3000 -it ghc
-000016b0: 722e 696f 2f62 656e 746f 6d6c 2f6f 7065  r.io/bentoml/ope
-000016c0: 6e6c 6c6d 2073 7461 7274 2048 7567 6769  nllm start Huggi
-000016d0: 6e67 4661 6365 4834 2f7a 6570 6879 722d  ngFaceH4/zephyr-
-000016e0: 3762 2d62 6574 6120 2d2d 6261 636b 656e  7b-beta --backen
-000016f0: 6420 766c 6c6d 0a3e 2060 6060 0a0a 0a23  d vllm.> ```...#
-00001700: 2320 f09f 8f83 2047 6574 2073 7461 7274  # .... Get start
-00001710: 6564 0a0a 5468 6520 666f 6c6c 6f77 696e  ed..The followin
-00001720: 6720 7072 6f76 6964 6573 2069 6e73 7472  g provides instr
-00001730: 7563 7469 6f6e 7320 666f 7220 686f 7720  uctions for how 
-00001740: 746f 2067 6574 2073 7461 7274 6564 2077  to get started w
-00001750: 6974 6820 4f70 656e 4c4c 4d20 6c6f 6361  ith OpenLLM loca
-00001760: 6c6c 792e 0a23 2323 2050 7265 7265 7175  lly..### Prerequ
-00001770: 6973 6974 6573 0a0a 596f 7520 6861 7665  isites..You have
-00001780: 2069 6e73 7461 6c6c 6564 2050 7974 686f   installed Pytho
-00001790: 6e20 332e 3820 286f 7220 6c61 7465 7229  n 3.8 (or later)
-000017a0: 2061 6e64 c2a0 6070 6970 602e 2057 6520   and..`pip`. We 
-000017b0: 6869 6768 6c79 2072 6563 6f6d 6d65 6e64  highly recommend
-000017c0: 2075 7369 6e67 2061 205b 5669 7274 7561   using a [Virtua
-000017d0: 6c20 456e 7669 726f 6e6d 656e 745d 2868  l Environment](h
-000017e0: 7474 7073 3a2f 2f64 6f63 732e 7079 7468  ttps://docs.pyth
-000017f0: 6f6e 2e6f 7267 2f33 2f6c 6962 7261 7279  on.org/3/library
-00001800: 2f76 656e 762e 6874 6d6c 2920 746f 2070  /venv.html) to p
-00001810: 7265 7665 6e74 2070 6163 6b61 6765 2063  revent package c
-00001820: 6f6e 666c 6963 7473 2e0a 0a23 2323 2049  onflicts...### I
-00001830: 6e73 7461 6c6c 204f 7065 6e4c 4c4d 0a0a  nstall OpenLLM..
-00001840: 496e 7374 616c 6c20 4f70 656e 4c4c 4d20  Install OpenLLM 
-00001850: 6279 2075 7369 6e67 2060 7069 7060 2061  by using `pip` a
-00001860: 7320 666f 6c6c 6f77 733a 0a0a 6060 6062  s follows:..```b
-00001870: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00001880: 6f70 656e 6c6c 6d0a 6060 600a 0a54 6f20  openllm.```..To 
-00001890: 7665 7269 6679 2074 6865 2069 6e73 7461  verify the insta
-000018a0: 6c6c 6174 696f 6e2c 2072 756e 3a0a 0a60  llation, run:..`
-000018b0: 6060 6261 7368 0a24 206f 7065 6e6c 6c6d  ``bash.$ openllm
-000018c0: 202d 680a 0a55 7361 6765 3a20 6f70 656e   -h..Usage: open
-000018d0: 6c6c 6d20 5b4f 5054 494f 4e53 5d20 434f  llm [OPTIONS] CO
-000018e0: 4d4d 414e 4420 5b41 5247 535d 2e2e 2e0a  MMAND [ARGS]....
-000018f0: 0a20 2020 e296 88e2 9688 e296 88e2 9688  .   ............
-00001900: e296 88e2 9688 e295 9720 e296 88e2 9688  ......... ......
-00001910: e296 88e2 9688 e296 88e2 9688 e295 9720  ............... 
-00001920: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00001930: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
-00001940: 88e2 9597 2020 20e2 9688 e296 88e2 9597  ....   .........
-00001950: e296 88e2 9688 e295 9720 2020 2020 e296  .........     ..
-00001960: 88e2 9688 e295 9720 2020 2020 e296 88e2  .......     ....
-00001970: 9688 e296 88e2 9597 2020 20e2 9688 e296  ........   .....
-00001980: 88e2 9688 e295 970a 2020 e296 88e2 9688  ........  ......
-00001990: e295 94e2 9590 e295 90e2 9590 e296 88e2  ................
-000019a0: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
-000019b0: 90e2 9590 e296 88e2 9688 e295 97e2 9688  ................
-000019c0: e296 88e2 9594 e295 90e2 9590 e295 90e2  ................
-000019d0: 9590 e295 9de2 9688 e296 88e2 9688 e296  ................
-000019e0: 88e2 9597 2020 e296 88e2 9688 e295 91e2  ....  ..........
-000019f0: 9688 e296 88e2 9591 2020 2020 20e2 9688  ........     ...
-00001a00: e296 88e2 9591 2020 2020 20e2 9688 e296  ......     .....
-00001a10: 88e2 9688 e296 88e2 9597 20e2 9688 e296  .......... .....
-00001a20: 88e2 9688 e296 88e2 9591 0a20 20e2 9688  ...........  ...
-00001a30: e296 88e2 9591 2020 20e2 9688 e296 88e2  ......   .......
-00001a40: 9591 e296 88e2 9688 e296 88e2 9688 e296  ................
-00001a50: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
-00001a60: e296 88e2 9688 e296 88e2 9597 2020 e296  ............  ..
-00001a70: 88e2 9688 e295 94e2 9688 e296 88e2 9597  ................
-00001a80: 20e2 9688 e296 88e2 9591 e296 88e2 9688   ...............
-00001a90: e295 9120 2020 2020 e296 88e2 9688 e295  ...     ........
-00001aa0: 9120 2020 2020 e296 88e2 9688 e295 94e2  .     ..........
-00001ab0: 9688 e296 88e2 9688 e296 88e2 9594 e296  ................
-00001ac0: 88e2 9688 e295 910a 2020 e296 88e2 9688  ........  ......
-00001ad0: e295 9120 2020 e296 88e2 9688 e295 91e2  ...   ..........
-00001ae0: 9688 e296 88e2 9594 e295 90e2 9590 e295  ................
-00001af0: 90e2 959d 20e2 9688 e296 88e2 9594 e295  .... ...........
-00001b00: 90e2 9590 e295 9d20 20e2 9688 e296 88e2  .......  .......
-00001b10: 9591 e295 9ae2 9688 e296 88e2 9597 e296  ................
-00001b20: 88e2 9688 e295 91e2 9688 e296 88e2 9591  ................
-00001b30: 2020 2020 20e2 9688 e296 88e2 9591 2020       .........  
-00001b40: 2020 20e2 9688 e296 88e2 9591 e295 9ae2     .............
-00001b50: 9688 e296 88e2 9594 e295 9de2 9688 e296  ................
-00001b60: 88e2 9591 0a20 20e2 959a e296 88e2 9688  .....  .........
-00001b70: e296 88e2 9688 e296 88e2 9688 e295 94e2  ................
-00001b80: 959d e296 88e2 9688 e295 9120 2020 2020  ...........     
-00001b90: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00001ba0: 9688 e296 88e2 9597 e296 88e2 9688 e295  ................
-00001bb0: 9120 e295 9ae2 9688 e296 88e2 9688 e296  . ..............
-00001bc0: 88e2 9591 e296 88e2 9688 e296 88e2 9688  ................
-00001bd0: e296 88e2 9688 e296 88e2 9597 e296 88e2  ................
-00001be0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00001bf0: 88e2 9597 e296 88e2 9688 e295 9120 e295  ............. ..
-00001c00: 9ae2 9590 e295 9d20 e296 88e2 9688 e295  ....... ........
-00001c10: 910a 2020 20e2 959a e295 90e2 9590 e295  ..   ...........
-00001c20: 90e2 9590 e295 90e2 959d 20e2 959a e295  .......... .....
-00001c30: 90e2 959d 2020 2020 20e2 959a e295 90e2  ....     .......
-00001c40: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00001c50: 9de2 959a e295 90e2 959d 2020 e295 9ae2  ..........  ....
-00001c60: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
-00001c70: 90e2 9590 e295 90e2 9590 e295 90e2 9590  ................
-00001c80: e295 9de2 959a e295 90e2 9590 e295 90e2  ................
-00001c90: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
-00001ca0: 90e2 959d 2020 2020 20e2 959a e295 90e2  ....     .......
-00001cb0: 959d 2e0a 0a20 2041 6e20 6f70 656e 2070  .....  An open p
-00001cc0: 6c61 7466 6f72 6d20 666f 7220 6f70 6572  latform for oper
-00001cd0: 6174 696e 6720 6c61 7267 6520 6c61 6e67  ating large lang
-00001ce0: 7561 6765 206d 6f64 656c 7320 696e 2070  uage models in p
-00001cf0: 726f 6475 6374 696f 6e2e 0a20 2046 696e  roduction..  Fin
-00001d00: 652d 7475 6e65 2c20 7365 7276 652c 2064  e-tune, serve, d
-00001d10: 6570 6c6f 792c 2061 6e64 206d 6f6e 6974  eploy, and monit
-00001d20: 6f72 2061 6e79 204c 4c4d 7320 7769 7468  or any LLMs with
-00001d30: 2065 6173 652e 0a0a 4f70 7469 6f6e 733a   ease...Options:
-00001d40: 0a20 202d 762c 202d 2d76 6572 7369 6f6e  .  -v, --version
-00001d50: 2020 5368 6f77 2074 6865 2076 6572 7369    Show the versi
-00001d60: 6f6e 2061 6e64 2065 7869 742e 0a20 202d  on and exit..  -
-00001d70: 682c 202d 2d68 656c 7020 2020 2020 5368  h, --help     Sh
-00001d80: 6f77 2074 6869 7320 6d65 7373 6167 6520  ow this message 
-00001d90: 616e 6420 6578 6974 2e0a 0a43 6f6d 6d61  and exit...Comma
-00001da0: 6e64 733a 0a20 2062 7569 6c64 2020 2020  nds:.  build    
-00001db0: 2020 2050 6163 6b61 6765 2061 2067 6976     Package a giv
-00001dc0: 656e 206d 6f64 656c 7320 696e 746f 2061  en models into a
-00001dd0: 2042 656e 746f 4c4c 4d2e 0a20 2069 6d70   BentoLLM..  imp
-00001de0: 6f72 7420 2020 2020 2053 6574 7570 204c  ort      Setup L
-00001df0: 4c4d 2069 6e74 6572 6163 7469 7665 6c79  LM interactively
-00001e00: 2e0a 2020 6d6f 6465 6c73 2020 2020 2020  ..  models      
-00001e10: 4c69 7374 2061 6c6c 2073 7570 706f 7274  List all support
-00001e20: 6564 206d 6f64 656c 732e 0a20 2070 7275  ed models..  pru
-00001e30: 6e65 2020 2020 2020 2052 656d 6f76 6520  ne       Remove 
-00001e40: 616c 6c20 7361 7665 6420 6d6f 6465 6c73  all saved models
-00001e50: 2c20 2861 6e64 206f 7074 696f 6e61 6c6c  , (and optionall
-00001e60: 7920 6265 6e74 6f73 2920 6275 696c 7420  y bentos) built 
-00001e70: 7769 7468 204f 7065 6e4c 4c4d 206c 6f63  with OpenLLM loc
-00001e80: 616c 6c79 2e0a 2020 7175 6572 7920 2020  ally..  query   
-00001e90: 2020 2020 5175 6572 7920 6120 4c4c 4d20      Query a LLM 
-00001ea0: 696e 7465 7261 6374 6976 656c 792c 2066  interactively, f
-00001eb0: 726f 6d20 6120 7465 726d 696e 616c 2e0a  rom a terminal..
-00001ec0: 2020 7374 6172 7420 2020 2020 2020 5374    start       St
-00001ed0: 6172 7420 6120 4c4c 4d53 6572 7665 7220  art a LLMServer 
-00001ee0: 666f 7220 616e 7920 7375 7070 6f72 7465  for any supporte
-00001ef0: 6420 4c4c 4d2e 0a20 2073 7461 7274 2d67  d LLM..  start-g
-00001f00: 7270 6320 2053 7461 7274 2061 2067 5250  rpc  Start a gRP
-00001f10: 4320 4c4c 4d53 6572 7665 7220 666f 7220  C LLMServer for 
-00001f20: 616e 7920 7375 7070 6f72 7465 6420 4c4c  any supported LL
-00001f30: 4d2e 0a0a 4578 7465 6e73 696f 6e73 3a0a  M...Extensions:.
-00001f40: 2020 6275 696c 642d 6261 7365 2d63 6f6e    build-base-con
-00001f50: 7461 696e 6572 2020 4261 7365 2069 6d61  tainer  Base ima
-00001f60: 6765 2062 7569 6c64 6572 2066 6f72 2042  ge builder for B
-00001f70: 656e 746f 4c4c 4d2e 0a20 2064 6976 652d  entoLLM..  dive-
-00001f80: 6265 6e74 6f73 2020 2020 2020 2020 2020  bentos          
-00001f90: 2044 6976 6520 696e 746f 2061 2042 656e   Dive into a Ben
-00001fa0: 746f 4c4c 4d2e 0a20 2067 6574 2d63 6f6e  toLLM..  get-con
-00001fb0: 7461 696e 6572 6669 6c65 2020 2020 2052  tainerfile     R
-00001fc0: 6574 7572 6e20 436f 6e74 6169 6e65 7266  eturn Containerf
-00001fd0: 696c 6520 6f66 2061 6e79 2067 6976 656e  ile of any given
-00001fe0: 2042 656e 746f 2e0a 2020 6765 742d 7072   Bento..  get-pr
-00001ff0: 6f6d 7074 2020 2020 2020 2020 2020 2020  ompt            
-00002000: 4765 7420 7468 6520 6465 6661 756c 7420  Get the default 
-00002010: 7072 6f6d 7074 2075 7365 6420 6279 204f  prompt used by O
-00002020: 7065 6e4c 4c4d 2e0a 2020 6c69 7374 2d62  penLLM..  list-b
-00002030: 656e 746f 7320 2020 2020 2020 2020 2020  entos           
-00002040: 4c69 7374 2061 7661 696c 6162 6c65 2062  List available b
-00002050: 656e 746f 7320 6275 696c 7420 6279 204f  entos built by O
-00002060: 7065 6e4c 4c4d 2e0a 2020 6c69 7374 2d6d  penLLM..  list-m
-00002070: 6f64 656c 7320 2020 2020 2020 2020 2020  odels           
-00002080: 5468 6973 2069 7320 6571 7569 7661 6c65  This is equivale
-00002090: 6e74 2074 6f20 6f70 656e 6c6c 6d20 6d6f  nt to openllm mo
-000020a0: 6465 6c73 2e2e 2e0a 2020 706c 6179 6772  dels....  playgr
-000020b0: 6f75 6e64 2020 2020 2020 2020 2020 2020  ound            
-000020c0: 4f70 656e 4c4c 4d20 506c 6179 6772 6f75  OpenLLM Playgrou
-000020d0: 6e64 2e0a 6060 600a 0a23 2323 2053 7461  nd..```..### Sta
-000020e0: 7274 2061 204c 4c4d 2073 6572 7665 720a  rt a LLM server.
-000020f0: 0a4f 7065 6e4c 4c4d 2061 6c6c 6f77 7320  .OpenLLM allows 
-00002100: 796f 7520 746f 2071 7569 636b 6c79 2073  you to quickly s
-00002110: 7069 6e20 7570 2061 6e20 4c4c 4d20 7365  pin up an LLM se
-00002120: 7276 6572 2075 7369 6e67 2060 6f70 656e  rver using `open
-00002130: 6c6c 6d20 7374 6172 7460 2e20 466f 7220  llm start`. For 
-00002140: 6578 616d 706c 652c 2074 6f20 7374 6172  example, to star
-00002150: 7420 61c2 a05b 7068 692d 325d 2868 7474  t a..[phi-2](htt
-00002160: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00002170: 2e63 6f2f 6d69 6372 6f73 6f66 742f 7068  .co/microsoft/ph
-00002180: 692d 3229 c2a0 7365 7276 6572 2c20 7275  i-2)..server, ru
-00002190: 6e20 7468 6520 666f 6c6c 6f77 696e 673a  n the following:
-000021a0: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
-000021b0: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
-000021c0: 206f 7065 6e6c 6c6d 2073 7461 7274 206d   openllm start m
-000021d0: 6963 726f 736f 6674 2f70 6869 2d32 0a60  icrosoft/phi-2.`
-000021e0: 6060 0a0a 5468 6973 2073 7461 7274 7320  ``..This starts 
-000021f0: 7468 6520 7365 7276 6572 2061 74c2 a05b  the server at..[
-00002200: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a33  http://0.0.0.0:3
-00002210: 3030 302f 5d28 6874 7470 3a2f 2f30 2e30  000/](http://0.0
-00002220: 2e30 2e30 3a33 3030 302f 292e 204f 7065  .0.0:3000/). Ope
-00002230: 6e4c 4c4d 2064 6f77 6e6c 6f61 6473 2074  nLLM downloads t
-00002240: 6865 206d 6f64 656c 2074 6f20 7468 6520  he model to the 
-00002250: 4265 6e74 6f4d 4c20 6c6f 6361 6c20 4d6f  BentoML local Mo
-00002260: 6465 6c20 5374 6f72 6520 6966 2069 7420  del Store if it 
-00002270: 6861 7320 6e6f 7420 6265 656e 2072 6567  has not been reg
-00002280: 6973 7465 7265 6420 6265 666f 7265 2e20  istered before. 
-00002290: 546f 2076 6965 7720 796f 7572 206c 6f63  To view your loc
-000022a0: 616c 206d 6f64 656c 732c 2072 756e 2060  al models, run `
-000022b0: 6265 6e74 6f6d 6c20 6d6f 6465 6c73 206c  bentoml models l
-000022c0: 6973 7460 2e0a 0a54 6f20 696e 7465 7261  ist`...To intera
-000022d0: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-000022e0: 6572 2c20 796f 7520 6361 6e20 7669 7369  er, you can visi
-000022f0: 7420 7468 6520 7765 6220 5549 2061 74c2  t the web UI at.
-00002300: a05b 6874 7470 3a2f 2f30 2e30 2e30 2e30  .[http://0.0.0.0
-00002310: 3a33 3030 302f 5d28 6874 7470 3a2f 2f30  :3000/](http://0
-00002320: 2e30 2e30 2e30 3a33 3030 302f 2920 6f72  .0.0.0:3000/) or
-00002330: 2073 656e 6420 6120 7265 7175 6573 7420   send a request 
-00002340: 7573 696e 67c2 a060 6375 726c 602e 2059  using..`curl`. Y
-00002350: 6f75 2063 616e 2061 6c73 6f20 7573 6520  ou can also use 
-00002360: 4f70 656e 4c4c 4de2 8099 7320 6275 696c  OpenLLM...s buil
-00002370: 742d 696e 2050 7974 686f 6e20 636c 6965  t-in Python clie
-00002380: 6e74 2074 6f20 696e 7465 7261 6374 2077  nt to interact w
-00002390: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-000023a0: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-000023b0: 7420 6f70 656e 6c6c 6d0a 0a63 6c69 656e  t openllm..clien
-000023c0: 7420 3d20 6f70 656e 6c6c 6d2e 636c 6965  t = openllm.clie
-000023d0: 6e74 2e48 5454 5043 6c69 656e 7428 2768  nt.HTTPClient('h
-000023e0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-000023f0: 3330 3030 2729 0a63 6c69 656e 742e 7175  3000').client.qu
-00002400: 6572 7928 2745 7870 6c61 696e 2074 6f20  ery('Explain to 
-00002410: 6d65 2074 6865 2064 6966 6665 7265 6e63  me the differenc
-00002420: 6520 6265 7477 6565 6e20 2266 7572 7468  e between "furth
-00002430: 6572 2220 616e 6420 2266 6172 7468 6572  er" and "farther
-00002440: 2227 290a 6060 600a 0a41 6c74 6572 6e61  "').```..Alterna
-00002450: 7469 7665 6c79 2c20 7573 6520 7468 65c2  tively, use the.
-00002460: a060 6f70 656e 6c6c 6d20 7175 6572 7960  .`openllm query`
-00002470: c2a0 636f 6d6d 616e 6420 746f 2071 7565  ..command to que
-00002480: 7279 2074 6865 206d 6f64 656c 3a0a 0a60  ry the model:..`
-00002490: 6060 6261 7368 0a65 7870 6f72 7420 4f50  ``bash.export OP
-000024a0: 454e 4c4c 4d5f 454e 4450 4f49 4e54 3d68  ENLLM_ENDPOINT=h
-000024b0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-000024c0: 3330 3030 0a6f 7065 6e6c 6c6d 2071 7565  3000.openllm que
-000024d0: 7279 2027 4578 706c 6169 6e20 746f 206d  ry 'Explain to m
-000024e0: 6520 7468 6520 6469 6666 6572 656e 6365  e the difference
-000024f0: 2062 6574 7765 656e 2022 6675 7274 6865   between "furthe
-00002500: 7222 2061 6e64 2022 6661 7274 6865 7222  r" and "farther"
-00002510: 270a 6060 600a 0a4f 7065 6e4c 4c4d 2073  '.```..OpenLLM s
-00002520: 6561 6d6c 6573 736c 7920 7375 7070 6f72  eamlessly suppor
-00002530: 7473 206d 616e 7920 6d6f 6465 6c73 2061  ts many models a
-00002540: 6e64 2074 6865 6972 2076 6172 6961 6e74  nd their variant
-00002550: 732e 2059 6f75 2063 616e 2073 7065 6369  s. You can speci
-00002560: 6679 2064 6966 6665 7265 6e74 2076 6172  fy different var
-00002570: 6961 6e74 7320 6f66 2074 6865 206d 6f64  iants of the mod
-00002580: 656c 2074 6f20 6265 2073 6572 7665 642e  el to be served.
-00002590: 2046 6f72 2065 7861 6d70 6c65 3a0a 0a60   For example:..`
-000025a0: 6060 6261 7368 0a6f 7065 6e6c 6c6d 2073  ``bash.openllm s
-000025b0: 7461 7274 203c 6d6f 6465 6c5f 6964 3e20  tart <model_id> 
-000025c0: 2d2d 3c6f 7074 696f 6e73 3e0a 6060 600a  --<options>.```.
-000025d0: 0a3e 205b 214e 4f54 455d 0a3e 204f 7065  .> [!NOTE].> Ope
-000025e0: 6e4c 4c4d 2073 7570 706f 7274 7320 7370  nLLM supports sp
-000025f0: 6563 6966 7969 6e67 2066 696e 652d 7475  ecifying fine-tu
-00002600: 6e69 6e67 2077 6569 6768 7473 2061 6e64  ning weights and
-00002610: 2071 7561 6e74 697a 6564 2077 6569 6768   quantized weigh
-00002620: 7473 0a3e 2066 6f72 2061 6e79 206f 6620  ts.> for any of 
-00002630: 7468 6520 7375 7070 6f72 7465 6420 6d6f  the supported mo
-00002640: 6465 6c73 2061 7320 6c6f 6e67 2061 7320  dels as long as 
-00002650: 7468 6579 2063 616e 2062 6520 6c6f 6164  they can be load
-00002660: 6564 2077 6974 6820 7468 6520 6d6f 6465  ed with the mode
-00002670: 6c0a 3e20 6172 6368 6974 6563 7475 7265  l.> architecture
-00002680: 2e20 5573 6520 7468 65c2 a060 6f70 656e  . Use the..`open
-00002690: 6c6c 6d20 6d6f 6465 6c73 60c2 a063 6f6d  llm models`..com
-000026a0: 6d61 6e64 2074 6f20 7365 6520 7468 6520  mand to see the 
-000026b0: 636f 6d70 6c65 7465 206c 6973 7420 6f66  complete list of
-000026c0: 2073 7570 706f 7274 6564 0a3e 206d 6f64   supported.> mod
-000026d0: 656c 732c 2074 6865 6972 2061 7263 6869  els, their archi
-000026e0: 7465 6374 7572 6573 2c20 616e 6420 7468  tectures, and th
-000026f0: 6569 7220 7661 7269 616e 7473 2e0a 0a3e  eir variants...>
-00002700: 205b 2149 4d50 4f52 5441 4e54 5d0a 3e20   [!IMPORTANT].> 
-00002710: 4966 2079 6f75 2061 7265 2074 6573 7469  If you are testi
-00002720: 6e67 204f 7065 6e4c 4c4d 206f 6e20 4350  ng OpenLLM on CP
-00002730: 552c 2079 6f75 206d 6967 6874 2077 616e  U, you might wan
-00002740: 7420 746f 2070 6173 7320 696e 2060 4454  t to pass in `DT
-00002750: 5950 453d 666c 6f61 7433 3260 2e20 4279  YPE=float32`. By
-00002760: 2064 6566 6175 6c74 2c0a 3e20 4f70 656e   default,.> Open
-00002770: 4c4c 4d20 7769 6c6c 2073 6574 206d 6f64  LLM will set mod
-00002780: 656c 2060 6474 7970 6560 2074 6f20 6062  el `dtype` to `b
-00002790: 666c 6f61 7431 3660 2066 6f72 2074 6865  float16` for the
-000027a0: 2062 6573 7420 7065 7266 6f72 6d61 6e63   best performanc
-000027b0: 652e 0a3e 2060 6060 6261 7368 0a3e 2044  e..> ```bash.> D
-000027c0: 5459 5045 3d66 6c6f 6174 3332 206f 7065  TYPE=float32 ope
-000027d0: 6e6c 6c6d 2073 7461 7274 206d 6963 726f  nllm start micro
-000027e0: 736f 6674 2f70 6869 2d32 0a3e 2060 6060  soft/phi-2.> ```
-000027f0: 0a3e 2054 6869 7320 7769 6c6c 2061 6c73  .> This will als
-00002800: 6f20 6170 706c 6965 7320 746f 206f 6c64  o applies to old
-00002810: 6572 2047 5055 732e 2049 6620 796f 7572  er GPUs. If your
-00002820: 2047 5055 7320 646f 6573 6e27 7420 7375   GPUs doesn't su
-00002830: 7070 6f72 7420 6062 666c 6f61 7431 3660  pport `bfloat16`
-00002840: 2c20 7468 656e 2079 6f75 2061 6c73 6f0a  , then you also.
-00002850: 3e20 7761 6e74 2074 6f20 7365 7420 6044  > want to set `D
-00002860: 5459 5045 3d66 6c6f 6174 3136 602e 0a0a  TYPE=float16`...
-00002870: 2323 20f0 9fa7 a920 5375 7070 6f72 7465  ## .... Supporte
-00002880: 6420 6d6f 6465 6c73 0a0a 4f70 656e 4c4c  d models..OpenLL
-00002890: 4d20 6375 7272 656e 746c 7920 7375 7070  M currently supp
-000028a0: 6f72 7473 2074 6865 2066 6f6c 6c6f 7769  orts the followi
-000028b0: 6e67 206d 6f64 656c 732e 2042 7920 6465  ng models. By de
-000028c0: 6661 756c 742c 204f 7065 6e4c 4c4d 2064  fault, OpenLLM d
-000028d0: 6f65 736e 2774 2069 6e63 6c75 6465 2064  oesn't include d
-000028e0: 6570 656e 6465 6e63 6965 7320 746f 2072  ependencies to r
-000028f0: 756e 2061 6c6c 206d 6f64 656c 732e 2054  un all models. T
-00002900: 6865 2065 7874 7261 206d 6f64 656c 2d73  he extra model-s
-00002910: 7065 6369 6669 6320 6465 7065 6e64 656e  pecific dependen
-00002920: 6369 6573 2063 616e 2062 6520 696e 7374  cies can be inst
-00002930: 616c 6c65 6420 7769 7468 2074 6865 2069  alled with the i
-00002940: 6e73 7472 7563 7469 6f6e 7320 6265 6c6f  nstructions belo
-00002950: 772e 0a0a 3c21 2d2d 2075 7064 6174 652d  w...<!-- update-
-00002960: 7265 6164 6d65 2e70 793a 2073 7461 7274  readme.py: start
-00002970: 202d 2d3e 0a3c 6465 7461 696c 733e 0a0a   -->.<details>..
-00002980: 3c73 756d 6d61 7279 3e42 6169 6368 7561  <summary>Baichua
-00002990: 6e3c 2f73 756d 6d61 7279 3e0a 0a0a 2323  n</summary>...##
-000029a0: 2320 5175 6963 6b73 7461 7274 0a0a 0a0a  # Quickstart....
-000029b0: 3e20 2a2a 4e6f 7465 3a2a 2a20 4261 6963  > **Note:** Baic
-000029c0: 6875 616e 2072 6571 7569 7265 7320 746f  huan requires to
-000029d0: 2069 6e73 7461 6c6c 2077 6974 683a 0a3e   install with:.>
-000029e0: 2060 6060 6261 7368 0a3e 2070 6970 2069   ```bash.> pip i
-000029f0: 6e73 7461 6c6c 2022 6f70 656e 6c6c 6d5b  nstall "openllm[
-00002a00: 6261 6963 6875 616e 5d22 0a3e 2060 6060  baichuan]".> ```
-00002a10: 0a0a 0a52 756e 2074 6865 2066 6f6c 6c6f  ...Run the follo
-00002a20: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00002a30: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
-00002a40: 6120 4261 6963 6875 616e 2073 6572 7665  a Baichuan serve
-00002a50: 723a 0a0a 6060 6062 6173 680a 5452 5553  r:..```bash.TRUS
-00002a60: 545f 5245 4d4f 5445 5f43 4f44 453d 5472  T_REMOTE_CODE=Tr
-00002a70: 7565 206f 7065 6e6c 6c6d 2073 7461 7274  ue openllm start
-00002a80: 2062 6169 6368 7561 6e2d 696e 632f 6261   baichuan-inc/ba
-00002a90: 6963 6875 616e 2d37 620a 6060 600a 496e  ichuan-7b.```.In
-00002aa0: 2061 2064 6966 6665 7265 6e74 2074 6572   a different ter
-00002ab0: 6d69 6e61 6c2c 2072 756e 2074 6865 2066  minal, run the f
-00002ac0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00002ad0: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
-00002ae0: 6820 7468 6520 7365 7276 6572 3a0a 0a60  h the server:..`
-00002af0: 6060 6261 7368 0a65 7870 6f72 7420 4f50  ``bash.export OP
-00002b00: 454e 4c4c 4d5f 454e 4450 4f49 4e54 3d68  ENLLM_ENDPOINT=h
-00002b10: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00002b20: 3330 3030 0a6f 7065 6e6c 6c6d 2071 7565  3000.openllm que
-00002b30: 7279 2027 5768 6174 2061 7265 206c 6172  ry 'What are lar
-00002b40: 6765 206c 616e 6775 6167 6520 6d6f 6465  ge language mode
-00002b50: 6c73 3f27 0a60 6060 0a0a 0a3e 202a 2a4e  ls?'.```...> **N
-00002b60: 6f74 653a 2a2a 2041 6e79 2042 6169 6368  ote:** Any Baich
-00002b70: 7561 6e20 7661 7269 616e 7473 2063 616e  uan variants can
-00002b80: 2062 6520 6465 706c 6f79 6564 2077 6974   be deployed wit
-00002b90: 6820 4f70 656e 4c4c 4d2e 2056 6973 6974  h OpenLLM. Visit
-00002ba0: 2074 6865 205b 4875 6767 696e 6746 6163   the [HuggingFac
-00002bb0: 6520 4d6f 6465 6c20 4875 625d 2868 7474  e Model Hub](htt
-00002bc0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00002bd0: 2e63 6f2f 6d6f 6465 6c73 3f73 6f72 743d  .co/models?sort=
-00002be0: 7472 656e 6469 6e67 2673 6561 7263 683d  trending&search=
-00002bf0: 6261 6963 6875 616e 2920 746f 2073 6565  baichuan) to see
-00002c00: 206d 6f72 6520 4261 6963 6875 616e 2d63   more Baichuan-c
-00002c10: 6f6d 7061 7469 626c 6520 6d6f 6465 6c73  ompatible models
-00002c20: 2e0a 0a0a 0a23 2323 2053 7570 706f 7274  .....### Support
-00002c30: 6564 206d 6f64 656c 730a 0a59 6f75 2063  ed models..You c
-00002c40: 616e 2073 7065 6369 6679 2061 6e79 206f  an specify any o
-00002c50: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
-00002c60: 4261 6963 6875 616e 206d 6f64 656c 7320  Baichuan models 
-00002c70: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
-00002c80: 7274 603a 0a0a 0a2d 205b 6261 6963 6875  rt`:...- [baichu
-00002c90: 616e 2d69 6e63 2f62 6169 6368 7561 6e32  an-inc/baichuan2
-00002ca0: 2d37 622d 6261 7365 5d28 6874 7470 733a  -7b-base](https:
-00002cb0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00002cc0: 2f62 6169 6368 7561 6e2d 696e 632f 6261  /baichuan-inc/ba
-00002cd0: 6963 6875 616e 322d 3762 2d62 6173 6529  ichuan2-7b-base)
-00002ce0: 0a2d 205b 6261 6963 6875 616e 2d69 6e63  .- [baichuan-inc
-00002cf0: 2f62 6169 6368 7561 6e32 2d37 622d 6368  /baichuan2-7b-ch
-00002d00: 6174 5d28 6874 7470 733a 2f2f 6875 6767  at](https://hugg
-00002d10: 696e 6766 6163 652e 636f 2f62 6169 6368  ingface.co/baich
-00002d20: 7561 6e2d 696e 632f 6261 6963 6875 616e  uan-inc/baichuan
-00002d30: 322d 3762 2d63 6861 7429 0a2d 205b 6261  2-7b-chat).- [ba
-00002d40: 6963 6875 616e 2d69 6e63 2f62 6169 6368  ichuan-inc/baich
-00002d50: 7561 6e32 2d31 3362 2d62 6173 655d 2868  uan2-13b-base](h
-00002d60: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00002d70: 6365 2e63 6f2f 6261 6963 6875 616e 2d69  ce.co/baichuan-i
-00002d80: 6e63 2f62 6169 6368 7561 6e32 2d31 3362  nc/baichuan2-13b
-00002d90: 2d62 6173 6529 0a2d 205b 6261 6963 6875  -base).- [baichu
-00002da0: 616e 2d69 6e63 2f62 6169 6368 7561 6e32  an-inc/baichuan2
-00002db0: 2d31 3362 2d63 6861 745d 2868 7474 7073  -13b-chat](https
-00002dc0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00002dd0: 6f2f 6261 6963 6875 616e 2d69 6e63 2f62  o/baichuan-inc/b
-00002de0: 6169 6368 7561 6e32 2d31 3362 2d63 6861  aichuan2-13b-cha
-00002df0: 7429 0a0a 3c2f 6465 7461 696c 733e 0a0a  t)..</details>..
-00002e00: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
-00002e10: 6172 793e 4368 6174 474c 4d3c 2f73 756d  ary>ChatGLM</sum
-00002e20: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
-00002e30: 6b73 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f  kstart....> **No
-00002e40: 7465 3a2a 2a20 4368 6174 474c 4d20 7265  te:** ChatGLM re
-00002e50: 7175 6972 6573 2074 6f20 696e 7374 616c  quires to instal
-00002e60: 6c20 7769 7468 3a0a 3e20 6060 6062 6173  l with:.> ```bas
-00002e70: 680a 3e20 7069 7020 696e 7374 616c 6c20  h.> pip install 
-00002e80: 226f 7065 6e6c 6c6d 5b63 6861 7467 6c6d  "openllm[chatglm
-00002e90: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
-00002ea0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00002eb0: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
-00002ec0: 7370 696e 2075 7020 6120 4368 6174 474c  spin up a ChatGL
-00002ed0: 4d20 7365 7276 6572 3a0a 0a60 6060 6261  M server:..```ba
-00002ee0: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
-00002ef0: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
-00002f00: 6d20 7374 6172 7420 7468 7564 6d2f 6368  m start thudm/ch
-00002f10: 6174 676c 6d2d 3662 0a60 6060 0a49 6e20  atglm-6b.```.In 
-00002f20: 6120 6469 6666 6572 656e 7420 7465 726d  a different term
-00002f30: 696e 616c 2c20 7275 6e20 7468 6520 666f  inal, run the fo
-00002f40: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
-00002f50: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
-00002f60: 2074 6865 2073 6572 7665 723a 0a0a 6060   the server:..``
-00002f70: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
-00002f80: 4e4c 4c4d 5f45 4e44 504f 494e 543d 6874  NLLM_ENDPOINT=ht
-00002f90: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
-00002fa0: 3030 300a 6f70 656e 6c6c 6d20 7175 6572  000.openllm quer
-00002fb0: 7920 2757 6861 7420 6172 6520 6c61 7267  y 'What are larg
-00002fc0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
-00002fd0: 733f 270a 6060 600a 0a0a 3e20 2a2a 4e6f  s?'.```...> **No
-00002fe0: 7465 3a2a 2a20 416e 7920 4368 6174 474c  te:** Any ChatGL
-00002ff0: 4d20 7661 7269 616e 7473 2063 616e 2062  M variants can b
-00003000: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
-00003010: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
-00003020: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
-00003030: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
-00003040: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00003050: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
-00003060: 656e 6469 6e67 2673 6561 7263 683d 6368  ending&search=ch
-00003070: 6174 676c 6d29 2074 6f20 7365 6520 6d6f  atglm) to see mo
-00003080: 7265 2043 6861 7447 4c4d 2d63 6f6d 7061  re ChatGLM-compa
-00003090: 7469 626c 6520 6d6f 6465 6c73 2e0a 0a0a  tible models....
-000030a0: 0a23 2323 2053 7570 706f 7274 6564 206d  .### Supported m
-000030b0: 6f64 656c 730a 0a59 6f75 2063 616e 2073  odels..You can s
-000030c0: 7065 6369 6679 2061 6e79 206f 6620 7468  pecify any of th
-000030d0: 6520 666f 6c6c 6f77 696e 6720 4368 6174  e following Chat
-000030e0: 474c 4d20 6d6f 6465 6c73 2076 6961 2060  GLM models via `
-000030f0: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
-00003100: 0a0a 2d20 5b74 6875 646d 2f63 6861 7467  ..- [thudm/chatg
-00003110: 6c6d 2d36 625d 2868 7474 7073 3a2f 2f68  lm-6b](https://h
-00003120: 7567 6769 6e67 6661 6365 2e63 6f2f 7468  uggingface.co/th
-00003130: 7564 6d2f 6368 6174 676c 6d2d 3662 290a  udm/chatglm-6b).
-00003140: 2d20 5b74 6875 646d 2f63 6861 7467 6c6d  - [thudm/chatglm
-00003150: 2d36 622d 696e 7438 5d28 6874 7470 733a  -6b-int8](https:
-00003160: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00003170: 2f74 6875 646d 2f63 6861 7467 6c6d 2d36  /thudm/chatglm-6
-00003180: 622d 696e 7438 290a 2d20 5b74 6875 646d  b-int8).- [thudm
-00003190: 2f63 6861 7467 6c6d 2d36 622d 696e 7434  /chatglm-6b-int4
-000031a0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000031b0: 6766 6163 652e 636f 2f74 6875 646d 2f63  gface.co/thudm/c
-000031c0: 6861 7467 6c6d 2d36 622d 696e 7434 290a  hatglm-6b-int4).
-000031d0: 2d20 5b74 6875 646d 2f63 6861 7467 6c6d  - [thudm/chatglm
-000031e0: 322d 3662 5d28 6874 7470 733a 2f2f 6875  2-6b](https://hu
-000031f0: 6767 696e 6766 6163 652e 636f 2f74 6875  ggingface.co/thu
-00003200: 646d 2f63 6861 7467 6c6d 322d 3662 290a  dm/chatglm2-6b).
-00003210: 2d20 5b74 6875 646d 2f63 6861 7467 6c6d  - [thudm/chatglm
-00003220: 322d 3662 2d69 6e74 345d 2868 7474 7073  2-6b-int4](https
-00003230: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00003240: 6f2f 7468 7564 6d2f 6368 6174 676c 6d32  o/thudm/chatglm2
-00003250: 2d36 622d 696e 7434 290a 2d20 5b74 6875  -6b-int4).- [thu
-00003260: 646d 2f63 6861 7467 6c6d 332d 3662 5d28  dm/chatglm3-6b](
-00003270: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00003280: 6163 652e 636f 2f74 6875 646d 2f63 6861  ace.co/thudm/cha
-00003290: 7467 6c6d 332d 3662 290a 0a3c 2f64 6574  tglm3-6b)..</det
-000032a0: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
-000032b0: 0a0a 3c73 756d 6d61 7279 3e44 6272 783c  ..<summary>Dbrx<
-000032c0: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
-000032d0: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
-000032e0: 2a2a 4e6f 7465 3a2a 2a20 4462 7278 2072  **Note:** Dbrx r
-000032f0: 6571 7569 7265 7320 746f 2069 6e73 7461  equires to insta
-00003300: 6c6c 2077 6974 683a 0a3e 2060 6060 6261  ll with:.> ```ba
-00003310: 7368 0a3e 2070 6970 2069 6e73 7461 6c6c  sh.> pip install
-00003320: 2022 6f70 656e 6c6c 6d5b 6462 7278 5d22   "openllm[dbrx]"
-00003330: 0a3e 2060 6060 0a0a 0a52 756e 2074 6865  .> ```...Run the
-00003340: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00003350: 6e64 2074 6f20 7175 6963 6b6c 7920 7370  nd to quickly sp
-00003360: 696e 2075 7020 6120 4462 7278 2073 6572  in up a Dbrx ser
-00003370: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
-00003380: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
-00003390: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
-000033a0: 7274 2064 6174 6162 7269 636b 732f 6462  rt databricks/db
-000033b0: 7278 2d69 6e73 7472 7563 740a 6060 600a  rx-instruct.```.
-000033c0: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-000033d0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-000033e0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-000033f0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-00003400: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-00003410: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00003420: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00003430: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00003440: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00003450: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00003460: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00003470: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00003480: 2a4e 6f74 653a 2a2a 2041 6e79 2044 6272  *Note:** Any Dbr
-00003490: 7820 7661 7269 616e 7473 2063 616e 2062  x variants can b
-000034a0: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
-000034b0: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
-000034c0: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
-000034d0: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
-000034e0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-000034f0: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
-00003500: 656e 6469 6e67 2673 6561 7263 683d 6462  ending&search=db
-00003510: 7278 2920 746f 2073 6565 206d 6f72 6520  rx) to see more 
-00003520: 4462 7278 2d63 6f6d 7061 7469 626c 6520  Dbrx-compatible 
-00003530: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
-00003540: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
-00003550: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
-00003560: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
-00003570: 6f77 696e 6720 4462 7278 206d 6f64 656c  owing Dbrx model
-00003580: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
-00003590: 7461 7274 603a 0a0a 0a2d 205b 6461 7461  tart`:...- [data
-000035a0: 6272 6963 6b73 2f64 6272 782d 696e 7374  bricks/dbrx-inst
-000035b0: 7275 6374 5d28 6874 7470 733a 2f2f 6875  ruct](https://hu
-000035c0: 6767 696e 6766 6163 652e 636f 2f64 6174  ggingface.co/dat
-000035d0: 6162 7269 636b 732f 6462 7278 2d69 6e73  abricks/dbrx-ins
-000035e0: 7472 7563 7429 0a2d 205b 6461 7461 6272  truct).- [databr
-000035f0: 6963 6b73 2f64 6272 782d 6261 7365 5d28  icks/dbrx-base](
-00003600: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00003610: 6163 652e 636f 2f64 6174 6162 7269 636b  ace.co/databrick
-00003620: 732f 6462 7278 2d62 6173 6529 0a0a 3c2f  s/dbrx-base)..</
-00003630: 6465 7461 696c 733e 0a0a 3c64 6574 6169  details>..<detai
-00003640: 6c73 3e0a 0a3c 7375 6d6d 6172 793e 446f  ls>..<summary>Do
-00003650: 6c6c 7956 323c 2f73 756d 6d61 7279 3e0a  llyV2</summary>.
-00003660: 0a0a 2323 2320 5175 6963 6b73 7461 7274  ..### Quickstart
-00003670: 0a0a 5275 6e20 7468 6520 666f 6c6c 6f77  ..Run the follow
-00003680: 696e 6720 636f 6d6d 616e 6420 746f 2071  ing command to q
-00003690: 7569 636b 6c79 2073 7069 6e20 7570 2061  uickly spin up a
-000036a0: 2044 6f6c 6c79 5632 2073 6572 7665 723a   DollyV2 server:
-000036b0: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
-000036c0: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
-000036d0: 206f 7065 6e6c 6c6d 2073 7461 7274 2064   openllm start d
-000036e0: 6174 6162 7269 636b 732f 646f 6c6c 792d  atabricks/dolly-
-000036f0: 7632 2d33 620a 6060 600a 496e 2061 2064  v2-3b.```.In a d
-00003700: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
-00003710: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
-00003720: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00003730: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
-00003740: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
-00003750: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-00003760: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
-00003770: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-00003780: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
-00003790: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
-000037a0: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
-000037b0: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
-000037c0: 2a2a 2041 6e79 2044 6f6c 6c79 5632 2076  ** Any DollyV2 v
-000037d0: 6172 6961 6e74 7320 6361 6e20 6265 2064  ariants can be d
-000037e0: 6570 6c6f 7965 6420 7769 7468 204f 7065  eployed with Ope
-000037f0: 6e4c 4c4d 2e20 5669 7369 7420 7468 6520  nLLM. Visit the 
-00003800: 5b48 7567 6769 6e67 4661 6365 204d 6f64  [HuggingFace Mod
-00003810: 656c 2048 7562 5d28 6874 7470 733a 2f2f  el Hub](https://
-00003820: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
-00003830: 6f64 656c 733f 736f 7274 3d74 7265 6e64  odels?sort=trend
-00003840: 696e 6726 7365 6172 6368 3d64 6f6c 6c79  ing&search=dolly
-00003850: 5f76 3229 2074 6f20 7365 6520 6d6f 7265  _v2) to see more
-00003860: 2044 6f6c 6c79 5632 2d63 6f6d 7061 7469   DollyV2-compati
-00003870: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-00003880: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00003890: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-000038a0: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-000038b0: 666f 6c6c 6f77 696e 6720 446f 6c6c 7956  following DollyV
-000038c0: 3220 6d6f 6465 6c73 2076 6961 2060 6f70  2 models via `op
-000038d0: 656e 6c6c 6d20 7374 6172 7460 3a0a 0a0a  enllm start`:...
-000038e0: 2d20 5b64 6174 6162 7269 636b 732f 646f  - [databricks/do
-000038f0: 6c6c 792d 7632 2d33 625d 2868 7474 7073  lly-v2-3b](https
-00003900: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00003910: 6f2f 6461 7461 6272 6963 6b73 2f64 6f6c  o/databricks/dol
-00003920: 6c79 2d76 322d 3362 290a 2d20 5b64 6174  ly-v2-3b).- [dat
-00003930: 6162 7269 636b 732f 646f 6c6c 792d 7632  abricks/dolly-v2
-00003940: 2d37 625d 2868 7474 7073 3a2f 2f68 7567  -7b](https://hug
-00003950: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
-00003960: 6272 6963 6b73 2f64 6f6c 6c79 2d76 322d  bricks/dolly-v2-
-00003970: 3762 290a 2d20 5b64 6174 6162 7269 636b  7b).- [databrick
-00003980: 732f 646f 6c6c 792d 7632 2d31 3262 5d28  s/dolly-v2-12b](
-00003990: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-000039a0: 6163 652e 636f 2f64 6174 6162 7269 636b  ace.co/databrick
-000039b0: 732f 646f 6c6c 792d 7632 2d31 3262 290a  s/dolly-v2-12b).
-000039c0: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
-000039d0: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
-000039e0: 3e46 616c 636f 6e3c 2f73 756d 6d61 7279  >Falcon</summary
-000039f0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
-00003a00: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
-00003a10: 2a20 4661 6c63 6f6e 2072 6571 7569 7265  * Falcon require
-00003a20: 7320 746f 2069 6e73 7461 6c6c 2077 6974  s to install wit
-00003a30: 683a 0a3e 2060 6060 6261 7368 0a3e 2070  h:.> ```bash.> p
-00003a40: 6970 2069 6e73 7461 6c6c 2022 6f70 656e  ip install "open
-00003a50: 6c6c 6d5b 6661 6c63 6f6e 5d22 0a3e 2060  llm[falcon]".> `
-00003a60: 6060 0a0a 0a52 756e 2074 6865 2066 6f6c  ``...Run the fol
-00003a70: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-00003a80: 6f20 7175 6963 6b6c 7920 7370 696e 2075  o quickly spin u
-00003a90: 7020 6120 4661 6c63 6f6e 2073 6572 7665  p a Falcon serve
-00003aa0: 723a 0a0a 6060 6062 6173 680a 5452 5553  r:..```bash.TRUS
-00003ab0: 545f 5245 4d4f 5445 5f43 4f44 453d 5472  T_REMOTE_CODE=Tr
-00003ac0: 7565 206f 7065 6e6c 6c6d 2073 7461 7274  ue openllm start
-00003ad0: 2074 6969 7561 652f 6661 6c63 6f6e 2d37   tiiuae/falcon-7
-00003ae0: 620a 6060 600a 496e 2061 2064 6966 6665  b.```.In a diffe
-00003af0: 7265 6e74 2074 6572 6d69 6e61 6c2c 2072  rent terminal, r
-00003b00: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00003b10: 2063 6f6d 6d61 6e64 2074 6f20 696e 7465   command to inte
-00003b20: 7261 6374 2077 6974 6820 7468 6520 7365  ract with the se
-00003b30: 7276 6572 3a0a 0a60 6060 6261 7368 0a65  rver:..```bash.e
-00003b40: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
-00003b50: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
-00003b60: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
-00003b70: 6e6c 6c6d 2071 7565 7279 2027 5768 6174  nllm query 'What
-00003b80: 2061 7265 206c 6172 6765 206c 616e 6775   are large langu
-00003b90: 6167 6520 6d6f 6465 6c73 3f27 0a60 6060  age models?'.```
-00003ba0: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2041  ...> **Note:** A
-00003bb0: 6e79 2046 616c 636f 6e20 7661 7269 616e  ny Falcon varian
-00003bc0: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
-00003bd0: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
-00003be0: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
-00003bf0: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
-00003c00: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-00003c10: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
-00003c20: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
-00003c30: 6561 7263 683d 6661 6c63 6f6e 2920 746f  earch=falcon) to
-00003c40: 2073 6565 206d 6f72 6520 4661 6c63 6f6e   see more Falcon
-00003c50: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
-00003c60: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
-00003c70: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
-00003c80: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
-00003c90: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00003ca0: 6720 4661 6c63 6f6e 206d 6f64 656c 7320  g Falcon models 
-00003cb0: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
-00003cc0: 7274 603a 0a0a 0a2d 205b 7469 6975 6165  rt`:...- [tiiuae
-00003cd0: 2f66 616c 636f 6e2d 3762 5d28 6874 7470  /falcon-7b](http
-00003ce0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00003cf0: 636f 2f74 6969 7561 652f 6661 6c63 6f6e  co/tiiuae/falcon
-00003d00: 2d37 6229 0a2d 205b 7469 6975 6165 2f66  -7b).- [tiiuae/f
-00003d10: 616c 636f 6e2d 3430 625d 2868 7474 7073  alcon-40b](https
-00003d20: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00003d30: 6f2f 7469 6975 6165 2f66 616c 636f 6e2d  o/tiiuae/falcon-
-00003d40: 3430 6229 0a2d 205b 7469 6975 6165 2f66  40b).- [tiiuae/f
-00003d50: 616c 636f 6e2d 3762 2d69 6e73 7472 7563  alcon-7b-instruc
-00003d60: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
-00003d70: 6e67 6661 6365 2e63 6f2f 7469 6975 6165  ngface.co/tiiuae
-00003d80: 2f66 616c 636f 6e2d 3762 2d69 6e73 7472  /falcon-7b-instr
-00003d90: 7563 7429 0a2d 205b 7469 6975 6165 2f66  uct).- [tiiuae/f
-00003da0: 616c 636f 6e2d 3430 622d 696e 7374 7275  alcon-40b-instru
-00003db0: 6374 5d28 6874 7470 733a 2f2f 6875 6767  ct](https://hugg
-00003dc0: 696e 6766 6163 652e 636f 2f74 6969 7561  ingface.co/tiiua
-00003dd0: 652f 6661 6c63 6f6e 2d34 3062 2d69 6e73  e/falcon-40b-ins
-00003de0: 7472 7563 7429 0a0a 3c2f 6465 7461 696c  truct)..</detail
-00003df0: 733e 0a0a 3c64 6574 6169 6c73 3e0a 0a3c  s>..<details>..<
-00003e00: 7375 6d6d 6172 793e 466c 616e 5435 3c2f  summary>FlanT5</
-00003e10: 7375 6d6d 6172 793e 0a0a 0a23 2323 2051  summary>...### Q
-00003e20: 7569 636b 7374 6172 740a 0a52 756e 2074  uickstart..Run t
-00003e30: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00003e40: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
-00003e50: 7370 696e 2075 7020 6120 466c 616e 5435  spin up a FlanT5
-00003e60: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
-00003e70: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
-00003e80: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
-00003e90: 2073 7461 7274 2067 6f6f 676c 652f 666c   start google/fl
-00003ea0: 616e 2d74 352d 6c61 7267 650a 6060 600a  an-t5-large.```.
-00003eb0: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-00003ec0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-00003ed0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00003ee0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-00003ef0: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-00003f00: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00003f10: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00003f20: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00003f30: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00003f40: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00003f50: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00003f60: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00003f70: 2a4e 6f74 653a 2a2a 2041 6e79 2046 6c61  *Note:** Any Fla
-00003f80: 6e54 3520 7661 7269 616e 7473 2063 616e  nT5 variants can
-00003f90: 2062 6520 6465 706c 6f79 6564 2077 6974   be deployed wit
-00003fa0: 6820 4f70 656e 4c4c 4d2e 2056 6973 6974  h OpenLLM. Visit
-00003fb0: 2074 6865 205b 4875 6767 696e 6746 6163   the [HuggingFac
-00003fc0: 6520 4d6f 6465 6c20 4875 625d 2868 7474  e Model Hub](htt
-00003fd0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00003fe0: 2e63 6f2f 6d6f 6465 6c73 3f73 6f72 743d  .co/models?sort=
-00003ff0: 7472 656e 6469 6e67 2673 6561 7263 683d  trending&search=
-00004000: 666c 616e 5f74 3529 2074 6f20 7365 6520  flan_t5) to see 
-00004010: 6d6f 7265 2046 6c61 6e54 352d 636f 6d70  more FlanT5-comp
-00004020: 6174 6962 6c65 206d 6f64 656c 732e 0a0a  atible models...
-00004030: 0a0a 2323 2320 5375 7070 6f72 7465 6420  ..### Supported 
-00004040: 6d6f 6465 6c73 0a0a 596f 7520 6361 6e20  models..You can 
-00004050: 7370 6563 6966 7920 616e 7920 6f66 2074  specify any of t
-00004060: 6865 2066 6f6c 6c6f 7769 6e67 2046 6c61  he following Fla
-00004070: 6e54 3520 6d6f 6465 6c73 2076 6961 2060  nT5 models via `
-00004080: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
-00004090: 0a0a 2d20 5b67 6f6f 676c 652f 666c 616e  ..- [google/flan
-000040a0: 2d74 352d 736d 616c 6c5d 2868 7474 7073  -t5-small](https
-000040b0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-000040c0: 6f2f 676f 6f67 6c65 2f66 6c61 6e2d 7435  o/google/flan-t5
-000040d0: 2d73 6d61 6c6c 290a 2d20 5b67 6f6f 676c  -small).- [googl
-000040e0: 652f 666c 616e 2d74 352d 6261 7365 5d28  e/flan-t5-base](
-000040f0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00004100: 6163 652e 636f 2f67 6f6f 676c 652f 666c  ace.co/google/fl
-00004110: 616e 2d74 352d 6261 7365 290a 2d20 5b67  an-t5-base).- [g
-00004120: 6f6f 676c 652f 666c 616e 2d74 352d 6c61  oogle/flan-t5-la
-00004130: 7267 655d 2868 7474 7073 3a2f 2f68 7567  rge](https://hug
-00004140: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
-00004150: 6c65 2f66 6c61 6e2d 7435 2d6c 6172 6765  le/flan-t5-large
-00004160: 290a 2d20 5b67 6f6f 676c 652f 666c 616e  ).- [google/flan
-00004170: 2d74 352d 786c 5d28 6874 7470 733a 2f2f  -t5-xl](https://
-00004180: 6875 6767 696e 6766 6163 652e 636f 2f67  huggingface.co/g
-00004190: 6f6f 676c 652f 666c 616e 2d74 352d 786c  oogle/flan-t5-xl
-000041a0: 290a 2d20 5b67 6f6f 676c 652f 666c 616e  ).- [google/flan
-000041b0: 2d74 352d 7878 6c5d 2868 7474 7073 3a2f  -t5-xxl](https:/
-000041c0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-000041d0: 676f 6f67 6c65 2f66 6c61 6e2d 7435 2d78  google/flan-t5-x
-000041e0: 786c 290a 0a3c 2f64 6574 6169 6c73 3e0a  xl)..</details>.
-000041f0: 0a3c 6465 7461 696c 733e 0a0a 3c73 756d  .<details>..<sum
-00004200: 6d61 7279 3e47 656d 6d61 3c2f 7375 6d6d  mary>Gemma</summ
-00004210: 6172 793e 0a0a 0a23 2323 2051 7569 636b  ary>...### Quick
-00004220: 7374 6172 740a 0a0a 0a3e 202a 2a4e 6f74  start....> **Not
-00004230: 653a 2a2a 2047 656d 6d61 2072 6571 7569  e:** Gemma requi
-00004240: 7265 7320 746f 2069 6e73 7461 6c6c 2077  res to install w
-00004250: 6974 683a 0a3e 2060 6060 6261 7368 0a3e  ith:.> ```bash.>
-00004260: 2070 6970 2069 6e73 7461 6c6c 2022 6f70   pip install "op
-00004270: 656e 6c6c 6d5b 6765 6d6d 615d 220a 3e20  enllm[gemma]".> 
-00004280: 6060 600a 0a0a 5275 6e20 7468 6520 666f  ```...Run the fo
-00004290: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
-000042a0: 746f 2071 7569 636b 6c79 2073 7069 6e20  to quickly spin 
-000042b0: 7570 2061 2047 656d 6d61 2073 6572 7665  up a Gemma serve
-000042c0: 723a 0a0a 6060 6062 6173 680a 5452 5553  r:..```bash.TRUS
-000042d0: 545f 5245 4d4f 5445 5f43 4f44 453d 5472  T_REMOTE_CODE=Tr
-000042e0: 7565 206f 7065 6e6c 6c6d 2073 7461 7274  ue openllm start
-000042f0: 2067 6f6f 676c 652f 6765 6d6d 612d 3762   google/gemma-7b
-00004300: 0a60 6060 0a49 6e20 6120 6469 6666 6572  .```.In a differ
-00004310: 656e 7420 7465 726d 696e 616c 2c20 7275  ent terminal, ru
-00004320: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-00004330: 636f 6d6d 616e 6420 746f 2069 6e74 6572  command to inter
-00004340: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
-00004350: 7665 723a 0a0a 6060 6062 6173 680a 6578  ver:..```bash.ex
-00004360: 706f 7274 204f 5045 4e4c 4c4d 5f45 4e44  port OPENLLM_END
-00004370: 504f 494e 543d 6874 7470 3a2f 2f6c 6f63  POINT=http://loc
-00004380: 616c 686f 7374 3a33 3030 300a 6f70 656e  alhost:3000.open
-00004390: 6c6c 6d20 7175 6572 7920 2757 6861 7420  llm query 'What 
-000043a0: 6172 6520 6c61 7267 6520 6c61 6e67 7561  are large langua
-000043b0: 6765 206d 6f64 656c 733f 270a 6060 600a  ge models?'.```.
-000043c0: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 416e  ..> **Note:** An
-000043d0: 7920 4765 6d6d 6120 7661 7269 616e 7473  y Gemma variants
-000043e0: 2063 616e 2062 6520 6465 706c 6f79 6564   can be deployed
-000043f0: 2077 6974 6820 4f70 656e 4c4c 4d2e 2056   with OpenLLM. V
-00004400: 6973 6974 2074 6865 205b 4875 6767 696e  isit the [Huggin
-00004410: 6746 6163 6520 4d6f 6465 6c20 4875 625d  gFace Model Hub]
-00004420: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00004430: 6661 6365 2e63 6f2f 6d6f 6465 6c73 3f73  face.co/models?s
-00004440: 6f72 743d 7472 656e 6469 6e67 2673 6561  ort=trending&sea
-00004450: 7263 683d 6765 6d6d 6129 2074 6f20 7365  rch=gemma) to se
-00004460: 6520 6d6f 7265 2047 656d 6d61 2d63 6f6d  e more Gemma-com
-00004470: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
-00004480: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
-00004490: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
-000044a0: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
-000044b0: 7468 6520 666f 6c6c 6f77 696e 6720 4765  the following Ge
-000044c0: 6d6d 6120 6d6f 6465 6c73 2076 6961 2060  mma models via `
-000044d0: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
-000044e0: 0a0a 2d20 5b67 6f6f 676c 652f 6765 6d6d  ..- [google/gemm
-000044f0: 612d 3762 5d28 6874 7470 733a 2f2f 6875  a-7b](https://hu
-00004500: 6767 696e 6766 6163 652e 636f 2f67 6f6f  ggingface.co/goo
-00004510: 676c 652f 6765 6d6d 612d 3762 290a 2d20  gle/gemma-7b).- 
-00004520: 5b67 6f6f 676c 652f 6765 6d6d 612d 3762  [google/gemma-7b
-00004530: 2d69 745d 2868 7474 7073 3a2f 2f68 7567  -it](https://hug
-00004540: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
-00004550: 6c65 2f67 656d 6d61 2d37 622d 6974 290a  le/gemma-7b-it).
-00004560: 2d20 5b67 6f6f 676c 652f 6765 6d6d 612d  - [google/gemma-
-00004570: 3262 5d28 6874 7470 733a 2f2f 6875 6767  2b](https://hugg
-00004580: 696e 6766 6163 652e 636f 2f67 6f6f 676c  ingface.co/googl
-00004590: 652f 6765 6d6d 612d 3262 290a 2d20 5b67  e/gemma-2b).- [g
-000045a0: 6f6f 676c 652f 6765 6d6d 612d 3262 2d69  oogle/gemma-2b-i
-000045b0: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
-000045c0: 6e67 6661 6365 2e63 6f2f 676f 6f67 6c65  ngface.co/google
-000045d0: 2f67 656d 6d61 2d32 622d 6974 290a 0a3c  /gemma-2b-it)..<
-000045e0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-000045f0: 696c 733e 0a0a 3c73 756d 6d61 7279 3e47  ils>..<summary>G
-00004600: 5054 4e65 6f58 3c2f 7375 6d6d 6172 793e  PTNeoX</summary>
-00004610: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
-00004620: 740a 0a52 756e 2074 6865 2066 6f6c 6c6f  t..Run the follo
-00004630: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00004640: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
-00004650: 6120 4750 544e 656f 5820 7365 7276 6572  a GPTNeoX server
-00004660: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
-00004670: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
-00004680: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
-00004690: 656c 6575 7468 6572 6169 2f67 7074 2d6e  eleutherai/gpt-n
-000046a0: 656f 782d 3230 620a 6060 600a 496e 2061  eox-20b.```.In a
-000046b0: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
-000046c0: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
-000046d0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-000046e0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-000046f0: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
-00004700: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
-00004710: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
-00004720: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-00004730: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
-00004740: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
-00004750: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00004760: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
-00004770: 653a 2a2a 2041 6e79 2047 5054 4e65 6f58  e:** Any GPTNeoX
-00004780: 2076 6172 6961 6e74 7320 6361 6e20 6265   variants can be
-00004790: 2064 6570 6c6f 7965 6420 7769 7468 204f   deployed with O
-000047a0: 7065 6e4c 4c4d 2e20 5669 7369 7420 7468  penLLM. Visit th
-000047b0: 6520 5b48 7567 6769 6e67 4661 6365 204d  e [HuggingFace M
-000047c0: 6f64 656c 2048 7562 5d28 6874 7470 733a  odel Hub](https:
-000047d0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000047e0: 2f6d 6f64 656c 733f 736f 7274 3d74 7265  /models?sort=tre
-000047f0: 6e64 696e 6726 7365 6172 6368 3d67 7074  nding&search=gpt
-00004800: 5f6e 656f 7829 2074 6f20 7365 6520 6d6f  _neox) to see mo
-00004810: 7265 2047 5054 4e65 6f58 2d63 6f6d 7061  re GPTNeoX-compa
-00004820: 7469 626c 6520 6d6f 6465 6c73 2e0a 0a0a  tible models....
-00004830: 0a23 2323 2053 7570 706f 7274 6564 206d  .### Supported m
-00004840: 6f64 656c 730a 0a59 6f75 2063 616e 2073  odels..You can s
-00004850: 7065 6369 6679 2061 6e79 206f 6620 7468  pecify any of th
-00004860: 6520 666f 6c6c 6f77 696e 6720 4750 544e  e following GPTN
-00004870: 656f 5820 6d6f 6465 6c73 2076 6961 2060  eoX models via `
-00004880: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
-00004890: 0a0a 2d20 5b65 6c65 7574 6865 7261 692f  ..- [eleutherai/
-000048a0: 6770 742d 6e65 6f78 2d32 3062 5d28 6874  gpt-neox-20b](ht
-000048b0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-000048c0: 652e 636f 2f65 6c65 7574 6865 7261 692f  e.co/eleutherai/
-000048d0: 6770 742d 6e65 6f78 2d32 3062 290a 0a3c  gpt-neox-20b)..<
-000048e0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
-000048f0: 696c 733e 0a0a 3c73 756d 6d61 7279 3e4c  ils>..<summary>L
-00004900: 6c61 6d61 3c2f 7375 6d6d 6172 793e 0a0a  lama</summary>..
-00004910: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
-00004920: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 204c  ...> **Note:** L
-00004930: 6c61 6d61 2072 6571 7569 7265 7320 746f  lama requires to
-00004940: 2069 6e73 7461 6c6c 2077 6974 683a 0a3e   install with:.>
-00004950: 2060 6060 6261 7368 0a3e 2070 6970 2069   ```bash.> pip i
-00004960: 6e73 7461 6c6c 2022 6f70 656e 6c6c 6d5b  nstall "openllm[
-00004970: 6c6c 616d 615d 220a 3e20 6060 600a 0a0a  llama]".> ```...
-00004980: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
-00004990: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
-000049a0: 636b 6c79 2073 7069 6e20 7570 2061 204c  ckly spin up a L
-000049b0: 6c61 6d61 2073 6572 7665 723a 0a0a 6060  lama server:..``
-000049c0: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
-000049d0: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
-000049e0: 6e6c 6c6d 2073 7461 7274 204e 6f75 7352  nllm start NousR
-000049f0: 6573 6561 7263 682f 6c6c 616d 612d 322d  esearch/llama-2-
-00004a00: 3762 2d68 660a 6060 600a 496e 2061 2064  7b-hf.```.In a d
-00004a10: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
-00004a20: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
-00004a30: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00004a40: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
-00004a50: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
-00004a60: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-00004a70: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
-00004a80: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-00004a90: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
-00004aa0: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
-00004ab0: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
-00004ac0: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
-00004ad0: 2a2a 2041 6e79 204c 6c61 6d61 2076 6172  ** Any Llama var
-00004ae0: 6961 6e74 7320 6361 6e20 6265 2064 6570  iants can be dep
-00004af0: 6c6f 7965 6420 7769 7468 204f 7065 6e4c  loyed with OpenL
-00004b00: 4c4d 2e20 5669 7369 7420 7468 6520 5b48  LM. Visit the [H
-00004b10: 7567 6769 6e67 4661 6365 204d 6f64 656c  uggingFace Model
-00004b20: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
-00004b30: 6767 696e 6766 6163 652e 636f 2f6d 6f64  ggingface.co/mod
-00004b40: 656c 733f 736f 7274 3d74 7265 6e64 696e  els?sort=trendin
-00004b50: 6726 7365 6172 6368 3d6c 6c61 6d61 2920  g&search=llama) 
-00004b60: 746f 2073 6565 206d 6f72 6520 4c6c 616d  to see more Llam
-00004b70: 612d 636f 6d70 6174 6962 6c65 206d 6f64  a-compatible mod
-00004b80: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
-00004b90: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
-00004ba0: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
-00004bb0: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
-00004bc0: 6e67 204c 6c61 6d61 206d 6f64 656c 7320  ng Llama models 
-00004bd0: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
-00004be0: 7274 603a 0a0a 0a2d 205b 6d65 7461 2d6c  rt`:...- [meta-l
-00004bf0: 6c61 6d61 2f4c 6c61 6d61 2d32 2d37 3062  lama/Llama-2-70b
-00004c00: 2d63 6861 742d 6866 5d28 6874 7470 733a  -chat-hf](https:
-00004c10: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00004c20: 2f6d 6574 612d 6c6c 616d 612f 4c6c 616d  /meta-llama/Llam
-00004c30: 612d 322d 3730 622d 6368 6174 2d68 6629  a-2-70b-chat-hf)
-00004c40: 0a2d 205b 6d65 7461 2d6c 6c61 6d61 2f4c  .- [meta-llama/L
-00004c50: 6c61 6d61 2d32 2d31 3362 2d63 6861 742d  lama-2-13b-chat-
-00004c60: 6866 5d28 6874 7470 733a 2f2f 6875 6767  hf](https://hugg
-00004c70: 696e 6766 6163 652e 636f 2f6d 6574 612d  ingface.co/meta-
-00004c80: 6c6c 616d 612f 4c6c 616d 612d 322d 3133  llama/Llama-2-13
-00004c90: 622d 6368 6174 2d68 6629 0a2d 205b 6d65  b-chat-hf).- [me
-00004ca0: 7461 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32  ta-llama/Llama-2
-00004cb0: 2d37 622d 6368 6174 2d68 665d 2868 7474  -7b-chat-hf](htt
-00004cc0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00004cd0: 2e63 6f2f 6d65 7461 2d6c 6c61 6d61 2f4c  .co/meta-llama/L
-00004ce0: 6c61 6d61 2d32 2d37 622d 6368 6174 2d68  lama-2-7b-chat-h
-00004cf0: 6629 0a2d 205b 6d65 7461 2d6c 6c61 6d61  f).- [meta-llama
-00004d00: 2f4c 6c61 6d61 2d32 2d37 3062 2d68 665d  /Llama-2-70b-hf]
-00004d10: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00004d20: 6661 6365 2e63 6f2f 6d65 7461 2d6c 6c61  face.co/meta-lla
-00004d30: 6d61 2f4c 6c61 6d61 2d32 2d37 3062 2d68  ma/Llama-2-70b-h
-00004d40: 6629 0a2d 205b 6d65 7461 2d6c 6c61 6d61  f).- [meta-llama
-00004d50: 2f4c 6c61 6d61 2d32 2d31 3362 2d68 665d  /Llama-2-13b-hf]
-00004d60: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00004d70: 6661 6365 2e63 6f2f 6d65 7461 2d6c 6c61  face.co/meta-lla
-00004d80: 6d61 2f4c 6c61 6d61 2d32 2d31 3362 2d68  ma/Llama-2-13b-h
-00004d90: 6629 0a2d 205b 6d65 7461 2d6c 6c61 6d61  f).- [meta-llama
-00004da0: 2f4c 6c61 6d61 2d32 2d37 622d 6866 5d28  /Llama-2-7b-hf](
-00004db0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00004dc0: 6163 652e 636f 2f6d 6574 612d 6c6c 616d  ace.co/meta-llam
-00004dd0: 612f 4c6c 616d 612d 322d 3762 2d68 6629  a/Llama-2-7b-hf)
-00004de0: 0a2d 205b 4e6f 7573 5265 7365 6172 6368  .- [NousResearch
-00004df0: 2f6c 6c61 6d61 2d32 2d37 3062 2d63 6861  /llama-2-70b-cha
-00004e00: 742d 6866 5d28 6874 7470 733a 2f2f 6875  t-hf](https://hu
-00004e10: 6767 696e 6766 6163 652e 636f 2f4e 6f75  ggingface.co/Nou
-00004e20: 7352 6573 6561 7263 682f 6c6c 616d 612d  sResearch/llama-
-00004e30: 322d 3730 622d 6368 6174 2d68 6629 0a2d  2-70b-chat-hf).-
-00004e40: 205b 4e6f 7573 5265 7365 6172 6368 2f6c   [NousResearch/l
-00004e50: 6c61 6d61 2d32 2d31 3362 2d63 6861 742d  lama-2-13b-chat-
-00004e60: 6866 5d28 6874 7470 733a 2f2f 6875 6767  hf](https://hugg
-00004e70: 696e 6766 6163 652e 636f 2f4e 6f75 7352  ingface.co/NousR
-00004e80: 6573 6561 7263 682f 6c6c 616d 612d 322d  esearch/llama-2-
-00004e90: 3133 622d 6368 6174 2d68 6629 0a2d 205b  13b-chat-hf).- [
-00004ea0: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-00004eb0: 6d61 2d32 2d37 622d 6368 6174 2d68 665d  ma-2-7b-chat-hf]
-00004ec0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00004ed0: 6661 6365 2e63 6f2f 4e6f 7573 5265 7365  face.co/NousRese
-00004ee0: 6172 6368 2f6c 6c61 6d61 2d32 2d37 622d  arch/llama-2-7b-
-00004ef0: 6368 6174 2d68 6629 0a2d 205b 4e6f 7573  chat-hf).- [Nous
-00004f00: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
-00004f10: 2d37 3062 2d68 665d 2868 7474 7073 3a2f  -70b-hf](https:/
-00004f20: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00004f30: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-00004f40: 6d61 2d32 2d37 3062 2d68 6629 0a2d 205b  ma-2-70b-hf).- [
-00004f50: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-00004f60: 6d61 2d32 2d31 3362 2d68 665d 2868 7474  ma-2-13b-hf](htt
-00004f70: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00004f80: 2e63 6f2f 4e6f 7573 5265 7365 6172 6368  .co/NousResearch
-00004f90: 2f6c 6c61 6d61 2d32 2d31 3362 2d68 6629  /llama-2-13b-hf)
-00004fa0: 0a2d 205b 4e6f 7573 5265 7365 6172 6368  .- [NousResearch
-00004fb0: 2f6c 6c61 6d61 2d32 2d37 622d 6866 5d28  /llama-2-7b-hf](
-00004fc0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00004fd0: 6163 652e 636f 2f4e 6f75 7352 6573 6561  ace.co/NousResea
-00004fe0: 7263 682f 6c6c 616d 612d 322d 3762 2d68  rch/llama-2-7b-h
-00004ff0: 6629 0a0a 3c2f 6465 7461 696c 733e 0a0a  f)..</details>..
-00005000: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
-00005010: 6172 793e 4d69 7374 7261 6c3c 2f73 756d  ary>Mistral</sum
-00005020: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
-00005030: 6b73 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f  kstart....> **No
-00005040: 7465 3a2a 2a20 4d69 7374 7261 6c20 7265  te:** Mistral re
-00005050: 7175 6972 6573 2074 6f20 696e 7374 616c  quires to instal
-00005060: 6c20 7769 7468 3a0a 3e20 6060 6062 6173  l with:.> ```bas
-00005070: 680a 3e20 7069 7020 696e 7374 616c 6c20  h.> pip install 
-00005080: 226f 7065 6e6c 6c6d 5b6d 6973 7472 616c  "openllm[mistral
-00005090: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
-000050a0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000050b0: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
-000050c0: 7370 696e 2075 7020 6120 4d69 7374 7261  spin up a Mistra
-000050d0: 6c20 7365 7276 6572 3a0a 0a60 6060 6261  l server:..```ba
-000050e0: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
-000050f0: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
-00005100: 6d20 7374 6172 7420 6d69 7374 7261 6c61  m start mistrala
-00005110: 692f 4d69 7374 7261 6c2d 3742 2d49 6e73  i/Mistral-7B-Ins
-00005120: 7472 7563 742d 7630 2e31 0a60 6060 0a49  truct-v0.1.```.I
-00005130: 6e20 6120 6469 6666 6572 656e 7420 7465  n a different te
-00005140: 726d 696e 616c 2c20 7275 6e20 7468 6520  rminal, run the 
-00005150: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
-00005160: 6420 746f 2069 6e74 6572 6163 7420 7769  d to interact wi
-00005170: 7468 2074 6865 2073 6572 7665 723a 0a0a  th the server:..
-00005180: 6060 6062 6173 680a 6578 706f 7274 204f  ```bash.export O
-00005190: 5045 4e4c 4c4d 5f45 4e44 504f 494e 543d  PENLLM_ENDPOINT=
-000051a0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
-000051b0: 3a33 3030 300a 6f70 656e 6c6c 6d20 7175  :3000.openllm qu
-000051c0: 6572 7920 2757 6861 7420 6172 6520 6c61  ery 'What are la
-000051d0: 7267 6520 6c61 6e67 7561 6765 206d 6f64  rge language mod
-000051e0: 656c 733f 270a 6060 600a 0a0a 3e20 2a2a  els?'.```...> **
-000051f0: 4e6f 7465 3a2a 2a20 416e 7920 4d69 7374  Note:** Any Mist
-00005200: 7261 6c20 7661 7269 616e 7473 2063 616e  ral variants can
-00005210: 2062 6520 6465 706c 6f79 6564 2077 6974   be deployed wit
-00005220: 6820 4f70 656e 4c4c 4d2e 2056 6973 6974  h OpenLLM. Visit
-00005230: 2074 6865 205b 4875 6767 696e 6746 6163   the [HuggingFac
-00005240: 6520 4d6f 6465 6c20 4875 625d 2868 7474  e Model Hub](htt
-00005250: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00005260: 2e63 6f2f 6d6f 6465 6c73 3f73 6f72 743d  .co/models?sort=
-00005270: 7472 656e 6469 6e67 2673 6561 7263 683d  trending&search=
-00005280: 6d69 7374 7261 6c29 2074 6f20 7365 6520  mistral) to see 
-00005290: 6d6f 7265 204d 6973 7472 616c 2d63 6f6d  more Mistral-com
-000052a0: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
-000052b0: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
-000052c0: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
-000052d0: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
-000052e0: 7468 6520 666f 6c6c 6f77 696e 6720 4d69  the following Mi
-000052f0: 7374 7261 6c20 6d6f 6465 6c73 2076 6961  stral models via
-00005300: 2060 6f70 656e 6c6c 6d20 7374 6172 7460   `openllm start`
-00005310: 3a0a 0a0a 2d20 5b48 7567 6769 6e67 4661  :...- [HuggingFa
-00005320: 6365 4834 2f7a 6570 6879 722d 3762 2d61  ceH4/zephyr-7b-a
-00005330: 6c70 6861 5d28 6874 7470 733a 2f2f 6875  lpha](https://hu
-00005340: 6767 696e 6766 6163 652e 636f 2f48 7567  ggingface.co/Hug
-00005350: 6769 6e67 4661 6365 4834 2f7a 6570 6879  gingFaceH4/zephy
-00005360: 722d 3762 2d61 6c70 6861 290a 2d20 5b48  r-7b-alpha).- [H
-00005370: 7567 6769 6e67 4661 6365 4834 2f7a 6570  uggingFaceH4/zep
-00005380: 6879 722d 3762 2d62 6574 615d 2868 7474  hyr-7b-beta](htt
-00005390: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-000053a0: 2e63 6f2f 4875 6767 696e 6746 6163 6548  .co/HuggingFaceH
-000053b0: 342f 7a65 7068 7972 2d37 622d 6265 7461  4/zephyr-7b-beta
-000053c0: 290a 2d20 5b6d 6973 7472 616c 6169 2f4d  ).- [mistralai/M
-000053d0: 6973 7472 616c 2d37 422d 496e 7374 7275  istral-7B-Instru
-000053e0: 6374 2d76 302e 325d 2868 7474 7073 3a2f  ct-v0.2](https:/
-000053f0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00005400: 6d69 7374 7261 6c61 692f 4d69 7374 7261  mistralai/Mistra
-00005410: 6c2d 3742 2d49 6e73 7472 7563 742d 7630  l-7B-Instruct-v0
-00005420: 2e32 290a 2d20 5b6d 6973 7472 616c 6169  .2).- [mistralai
-00005430: 2f4d 6973 7472 616c 2d37 422d 496e 7374  /Mistral-7B-Inst
-00005440: 7275 6374 2d76 302e 315d 2868 7474 7073  ruct-v0.1](https
-00005450: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00005460: 6f2f 6d69 7374 7261 6c61 692f 4d69 7374  o/mistralai/Mist
-00005470: 7261 6c2d 3742 2d49 6e73 7472 7563 742d  ral-7B-Instruct-
-00005480: 7630 2e31 290a 2d20 5b6d 6973 7472 616c  v0.1).- [mistral
-00005490: 6169 2f4d 6973 7472 616c 2d37 422d 7630  ai/Mistral-7B-v0
-000054a0: 2e31 5d28 6874 7470 733a 2f2f 6875 6767  .1](https://hugg
-000054b0: 696e 6766 6163 652e 636f 2f6d 6973 7472  ingface.co/mistr
-000054c0: 616c 6169 2f4d 6973 7472 616c 2d37 422d  alai/Mistral-7B-
-000054d0: 7630 2e31 290a 0a3c 2f64 6574 6169 6c73  v0.1)..</details
-000054e0: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
-000054f0: 756d 6d61 7279 3e4d 6978 7472 616c 3c2f  ummary>Mixtral</
-00005500: 7375 6d6d 6172 793e 0a0a 0a23 2323 2051  summary>...### Q
-00005510: 7569 636b 7374 6172 740a 0a0a 0a3e 202a  uickstart....> *
-00005520: 2a4e 6f74 653a 2a2a 204d 6978 7472 616c  *Note:** Mixtral
-00005530: 2072 6571 7569 7265 7320 746f 2069 6e73   requires to ins
-00005540: 7461 6c6c 2077 6974 683a 0a3e 2060 6060  tall with:.> ```
-00005550: 6261 7368 0a3e 2070 6970 2069 6e73 7461  bash.> pip insta
-00005560: 6c6c 2022 6f70 656e 6c6c 6d5b 6d69 7874  ll "openllm[mixt
-00005570: 7261 6c5d 220a 3e20 6060 600a 0a0a 5275  ral]".> ```...Ru
-00005580: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-00005590: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
-000055a0: 6c79 2073 7069 6e20 7570 2061 204d 6978  ly spin up a Mix
-000055b0: 7472 616c 2073 6572 7665 723a 0a0a 6060  tral server:..``
-000055c0: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
-000055d0: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
-000055e0: 6e6c 6c6d 2073 7461 7274 206d 6973 7472  nllm start mistr
-000055f0: 616c 6169 2f4d 6978 7472 616c 2d38 7837  alai/Mixtral-8x7
-00005600: 422d 496e 7374 7275 6374 2d76 302e 310a  B-Instruct-v0.1.
-00005610: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
-00005620: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
-00005630: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00005640: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
-00005650: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-00005660: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
-00005670: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
-00005680: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
-00005690: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
-000056a0: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
-000056b0: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
-000056c0: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
-000056d0: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
-000056e0: 204d 6978 7472 616c 2076 6172 6961 6e74   Mixtral variant
-000056f0: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
-00005700: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
-00005710: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
-00005720: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
-00005730: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00005740: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
-00005750: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
-00005760: 6172 6368 3d6d 6978 7472 616c 2920 746f  arch=mixtral) to
-00005770: 2073 6565 206d 6f72 6520 4d69 7874 7261   see more Mixtra
-00005780: 6c2d 636f 6d70 6174 6962 6c65 206d 6f64  l-compatible mod
-00005790: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
-000057a0: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
-000057b0: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
-000057c0: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
-000057d0: 6e67 204d 6978 7472 616c 206d 6f64 656c  ng Mixtral model
-000057e0: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
-000057f0: 7461 7274 603a 0a0a 0a2d 205b 6d69 7374  tart`:...- [mist
-00005800: 7261 6c61 692f 4d69 7874 7261 6c2d 3878  ralai/Mixtral-8x
-00005810: 3742 2d49 6e73 7472 7563 742d 7630 2e31  7B-Instruct-v0.1
-00005820: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00005830: 6766 6163 652e 636f 2f6d 6973 7472 616c  gface.co/mistral
-00005840: 6169 2f4d 6978 7472 616c 2d38 7837 422d  ai/Mixtral-8x7B-
-00005850: 496e 7374 7275 6374 2d76 302e 3129 0a2d  Instruct-v0.1).-
-00005860: 205b 6d69 7374 7261 6c61 692f 4d69 7874   [mistralai/Mixt
-00005870: 7261 6c2d 3878 3742 2d76 302e 315d 2868  ral-8x7B-v0.1](h
-00005880: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00005890: 6365 2e63 6f2f 6d69 7374 7261 6c61 692f  ce.co/mistralai/
-000058a0: 4d69 7874 7261 6c2d 3878 3742 2d76 302e  Mixtral-8x7B-v0.
-000058b0: 3129 0a0a 3c2f 6465 7461 696c 733e 0a0a  1)..</details>..
-000058c0: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
-000058d0: 6172 793e 4d50 543c 2f73 756d 6d61 7279  ary>MPT</summary
-000058e0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
-000058f0: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
-00005900: 2a20 4d50 5420 7265 7175 6972 6573 2074  * MPT requires t
-00005910: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
-00005920: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
-00005930: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
-00005940: 5b6d 7074 5d22 0a3e 2060 6060 0a0a 0a52  [mpt]".> ```...R
-00005950: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00005960: 2063 6f6d 6d61 6e64 2074 6f20 7175 6963   command to quic
-00005970: 6b6c 7920 7370 696e 2075 7020 6120 4d50  kly spin up a MP
-00005980: 5420 7365 7276 6572 3a0a 0a60 6060 6261  T server:..```ba
-00005990: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
-000059a0: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
-000059b0: 6d20 7374 6172 7420 6d6f 7361 6963 6d6c  m start mosaicml
-000059c0: 2f6d 7074 2d37 622d 696e 7374 7275 6374  /mpt-7b-instruct
-000059d0: 0a60 6060 0a49 6e20 6120 6469 6666 6572  .```.In a differ
-000059e0: 656e 7420 7465 726d 696e 616c 2c20 7275  ent terminal, ru
-000059f0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-00005a00: 636f 6d6d 616e 6420 746f 2069 6e74 6572  command to inter
-00005a10: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
-00005a20: 7665 723a 0a0a 6060 6062 6173 680a 6578  ver:..```bash.ex
-00005a30: 706f 7274 204f 5045 4e4c 4c4d 5f45 4e44  port OPENLLM_END
-00005a40: 504f 494e 543d 6874 7470 3a2f 2f6c 6f63  POINT=http://loc
-00005a50: 616c 686f 7374 3a33 3030 300a 6f70 656e  alhost:3000.open
-00005a60: 6c6c 6d20 7175 6572 7920 2757 6861 7420  llm query 'What 
-00005a70: 6172 6520 6c61 7267 6520 6c61 6e67 7561  are large langua
-00005a80: 6765 206d 6f64 656c 733f 270a 6060 600a  ge models?'.```.
-00005a90: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 416e  ..> **Note:** An
-00005aa0: 7920 4d50 5420 7661 7269 616e 7473 2063  y MPT variants c
-00005ab0: 616e 2062 6520 6465 706c 6f79 6564 2077  an be deployed w
-00005ac0: 6974 6820 4f70 656e 4c4c 4d2e 2056 6973  ith OpenLLM. Vis
-00005ad0: 6974 2074 6865 205b 4875 6767 696e 6746  it the [HuggingF
-00005ae0: 6163 6520 4d6f 6465 6c20 4875 625d 2868  ace Model Hub](h
-00005af0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00005b00: 6365 2e63 6f2f 6d6f 6465 6c73 3f73 6f72  ce.co/models?sor
-00005b10: 743d 7472 656e 6469 6e67 2673 6561 7263  t=trending&searc
-00005b20: 683d 6d70 7429 2074 6f20 7365 6520 6d6f  h=mpt) to see mo
-00005b30: 7265 204d 5054 2d63 6f6d 7061 7469 626c  re MPT-compatibl
-00005b40: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
-00005b50: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
-00005b60: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
-00005b70: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
-00005b80: 6c6c 6f77 696e 6720 4d50 5420 6d6f 6465  llowing MPT mode
-00005b90: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
-00005ba0: 7374 6172 7460 3a0a 0a0a 2d20 5b6d 6f73  start`:...- [mos
-00005bb0: 6169 636d 6c2f 6d70 742d 3762 5d28 6874  aicml/mpt-7b](ht
-00005bc0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00005bd0: 652e 636f 2f6d 6f73 6169 636d 6c2f 6d70  e.co/mosaicml/mp
-00005be0: 742d 3762 290a 2d20 5b6d 6f73 6169 636d  t-7b).- [mosaicm
-00005bf0: 6c2f 6d70 742d 3762 2d69 6e73 7472 7563  l/mpt-7b-instruc
-00005c00: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
-00005c10: 6e67 6661 6365 2e63 6f2f 6d6f 7361 6963  ngface.co/mosaic
-00005c20: 6d6c 2f6d 7074 2d37 622d 696e 7374 7275  ml/mpt-7b-instru
-00005c30: 6374 290a 2d20 5b6d 6f73 6169 636d 6c2f  ct).- [mosaicml/
-00005c40: 6d70 742d 3762 2d63 6861 745d 2868 7474  mpt-7b-chat](htt
-00005c50: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00005c60: 2e63 6f2f 6d6f 7361 6963 6d6c 2f6d 7074  .co/mosaicml/mpt
-00005c70: 2d37 622d 6368 6174 290a 2d20 5b6d 6f73  -7b-chat).- [mos
-00005c80: 6169 636d 6c2f 6d70 742d 3762 2d73 746f  aicml/mpt-7b-sto
-00005c90: 7279 7772 6974 6572 5d28 6874 7470 733a  rywriter](https:
-00005ca0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00005cb0: 2f6d 6f73 6169 636d 6c2f 6d70 742d 3762  /mosaicml/mpt-7b
-00005cc0: 2d73 746f 7279 7772 6974 6572 290a 2d20  -storywriter).- 
-00005cd0: 5b6d 6f73 6169 636d 6c2f 6d70 742d 3330  [mosaicml/mpt-30
-00005ce0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-00005cf0: 6e67 6661 6365 2e63 6f2f 6d6f 7361 6963  ngface.co/mosaic
-00005d00: 6d6c 2f6d 7074 2d33 3062 290a 2d20 5b6d  ml/mpt-30b).- [m
-00005d10: 6f73 6169 636d 6c2f 6d70 742d 3330 622d  osaicml/mpt-30b-
-00005d20: 696e 7374 7275 6374 5d28 6874 7470 733a  instruct](https:
-00005d30: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00005d40: 2f6d 6f73 6169 636d 6c2f 6d70 742d 3330  /mosaicml/mpt-30
-00005d50: 622d 696e 7374 7275 6374 290a 2d20 5b6d  b-instruct).- [m
-00005d60: 6f73 6169 636d 6c2f 6d70 742d 3330 622d  osaicml/mpt-30b-
-00005d70: 6368 6174 5d28 6874 7470 733a 2f2f 6875  chat](https://hu
-00005d80: 6767 696e 6766 6163 652e 636f 2f6d 6f73  ggingface.co/mos
-00005d90: 6169 636d 6c2f 6d70 742d 3330 622d 6368  aicml/mpt-30b-ch
-00005da0: 6174 290a 0a3c 2f64 6574 6169 6c73 3e0a  at)..</details>.
-00005db0: 0a3c 6465 7461 696c 733e 0a0a 3c73 756d  .<details>..<sum
-00005dc0: 6d61 7279 3e4f 5054 3c2f 7375 6d6d 6172  mary>OPT</summar
-00005dd0: 793e 0a0a 0a23 2323 2051 7569 636b 7374  y>...### Quickst
-00005de0: 6172 740a 0a0a 0a3e 202a 2a4e 6f74 653a  art....> **Note:
-00005df0: 2a2a 204f 5054 2072 6571 7569 7265 7320  ** OPT requires 
-00005e00: 746f 2069 6e73 7461 6c6c 2077 6974 683a  to install with:
-00005e10: 0a3e 2060 6060 6261 7368 0a3e 2070 6970  .> ```bash.> pip
-00005e20: 2069 6e73 7461 6c6c 2022 6f70 656e 6c6c   install "openll
-00005e30: 6d5b 6f70 745d 220a 3e20 6060 600a 0a0a  m[opt]".> ```...
-00005e40: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
-00005e50: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
-00005e60: 636b 6c79 2073 7069 6e20 7570 2061 204f  ckly spin up a O
-00005e70: 5054 2073 6572 7665 723a 0a0a 6060 6062  PT server:..```b
-00005e80: 6173 680a 6f70 656e 6c6c 6d20 7374 6172  ash.openllm star
-00005e90: 7420 6661 6365 626f 6f6b 2f6f 7074 2d31  t facebook/opt-1
-00005ea0: 2e33 620a 6060 600a 496e 2061 2064 6966  .3b.```.In a dif
-00005eb0: 6665 7265 6e74 2074 6572 6d69 6e61 6c2c  ferent terminal,
-00005ec0: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
-00005ed0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 696e  ng command to in
-00005ee0: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
-00005ef0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
-00005f00: 0a65 7870 6f72 7420 4f50 454e 4c4c 4d5f  .export OPENLLM_
-00005f10: 454e 4450 4f49 4e54 3d68 7474 703a 2f2f  ENDPOINT=http://
-00005f20: 6c6f 6361 6c68 6f73 743a 3330 3030 0a6f  localhost:3000.o
-00005f30: 7065 6e6c 6c6d 2071 7565 7279 2027 5768  penllm query 'Wh
-00005f40: 6174 2061 7265 206c 6172 6765 206c 616e  at are large lan
-00005f50: 6775 6167 6520 6d6f 6465 6c73 3f27 0a60  guage models?'.`
-00005f60: 6060 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  ``...> **Note:**
-00005f70: 2041 6e79 204f 5054 2076 6172 6961 6e74   Any OPT variant
-00005f80: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
-00005f90: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
-00005fa0: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
-00005fb0: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
-00005fc0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00005fd0: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
-00005fe0: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
-00005ff0: 6172 6368 3d6f 7074 2920 746f 2073 6565  arch=opt) to see
-00006000: 206d 6f72 6520 4f50 542d 636f 6d70 6174   more OPT-compat
-00006010: 6962 6c65 206d 6f64 656c 732e 0a0a 0a0a  ible models.....
-00006020: 2323 2320 5375 7070 6f72 7465 6420 6d6f  ### Supported mo
-00006030: 6465 6c73 0a0a 596f 7520 6361 6e20 7370  dels..You can sp
-00006040: 6563 6966 7920 616e 7920 6f66 2074 6865  ecify any of the
-00006050: 2066 6f6c 6c6f 7769 6e67 204f 5054 206d   following OPT m
-00006060: 6f64 656c 7320 7669 6120 606f 7065 6e6c  odels via `openl
-00006070: 6c6d 2073 7461 7274 603a 0a0a 0a2d 205b  lm start`:...- [
-00006080: 6661 6365 626f 6f6b 2f6f 7074 2d31 3235  facebook/opt-125
-00006090: 6d5d 2868 7474 7073 3a2f 2f68 7567 6769  m](https://huggi
-000060a0: 6e67 6661 6365 2e63 6f2f 6661 6365 626f  ngface.co/facebo
-000060b0: 6f6b 2f6f 7074 2d31 3235 6d29 0a2d 205b  ok/opt-125m).- [
-000060c0: 6661 6365 626f 6f6b 2f6f 7074 2d33 3530  facebook/opt-350
-000060d0: 6d5d 2868 7474 7073 3a2f 2f68 7567 6769  m](https://huggi
-000060e0: 6e67 6661 6365 2e63 6f2f 6661 6365 626f  ngface.co/facebo
-000060f0: 6f6b 2f6f 7074 2d33 3530 6d29 0a2d 205b  ok/opt-350m).- [
-00006100: 6661 6365 626f 6f6b 2f6f 7074 2d31 2e33  facebook/opt-1.3
-00006110: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-00006120: 6e67 6661 6365 2e63 6f2f 6661 6365 626f  ngface.co/facebo
-00006130: 6f6b 2f6f 7074 2d31 2e33 6229 0a2d 205b  ok/opt-1.3b).- [
-00006140: 6661 6365 626f 6f6b 2f6f 7074 2d32 2e37  facebook/opt-2.7
-00006150: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-00006160: 6e67 6661 6365 2e63 6f2f 6661 6365 626f  ngface.co/facebo
-00006170: 6f6b 2f6f 7074 2d32 2e37 6229 0a2d 205b  ok/opt-2.7b).- [
-00006180: 6661 6365 626f 6f6b 2f6f 7074 2d36 2e37  facebook/opt-6.7
-00006190: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-000061a0: 6e67 6661 6365 2e63 6f2f 6661 6365 626f  ngface.co/facebo
-000061b0: 6f6b 2f6f 7074 2d36 2e37 6229 0a2d 205b  ok/opt-6.7b).- [
-000061c0: 6661 6365 626f 6f6b 2f6f 7074 2d36 3662  facebook/opt-66b
-000061d0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000061e0: 6766 6163 652e 636f 2f66 6163 6562 6f6f  gface.co/faceboo
-000061f0: 6b2f 6f70 742d 3636 6229 0a0a 3c2f 6465  k/opt-66b)..</de
-00006200: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
-00006210: 3e0a 0a3c 7375 6d6d 6172 793e 5068 693c  >..<summary>Phi<
-00006220: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
-00006230: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
-00006240: 2a2a 4e6f 7465 3a2a 2a20 5068 6920 7265  **Note:** Phi re
-00006250: 7175 6972 6573 2074 6f20 696e 7374 616c  quires to instal
-00006260: 6c20 7769 7468 3a0a 3e20 6060 6062 6173  l with:.> ```bas
-00006270: 680a 3e20 7069 7020 696e 7374 616c 6c20  h.> pip install 
-00006280: 226f 7065 6e6c 6c6d 5b70 6869 5d22 0a3e  "openllm[phi]".>
-00006290: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
-000062a0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-000062b0: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
-000062c0: 2075 7020 6120 5068 6920 7365 7276 6572   up a Phi server
-000062d0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
-000062e0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
-000062f0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
-00006300: 6d69 6372 6f73 6f66 742f 7068 692d 320a  microsoft/phi-2.
-00006310: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
-00006320: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
-00006330: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00006340: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
-00006350: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-00006360: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
-00006370: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
-00006380: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
-00006390: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
-000063a0: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
-000063b0: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
-000063c0: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
-000063d0: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
-000063e0: 2050 6869 2076 6172 6961 6e74 7320 6361   Phi variants ca
-000063f0: 6e20 6265 2064 6570 6c6f 7965 6420 7769  n be deployed wi
-00006400: 7468 204f 7065 6e4c 4c4d 2e20 5669 7369  th OpenLLM. Visi
-00006410: 7420 7468 6520 5b48 7567 6769 6e67 4661  t the [HuggingFa
-00006420: 6365 204d 6f64 656c 2048 7562 5d28 6874  ce Model Hub](ht
-00006430: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00006440: 652e 636f 2f6d 6f64 656c 733f 736f 7274  e.co/models?sort
-00006450: 3d74 7265 6e64 696e 6726 7365 6172 6368  =trending&search
-00006460: 3d70 6869 2920 746f 2073 6565 206d 6f72  =phi) to see mor
-00006470: 6520 5068 692d 636f 6d70 6174 6962 6c65  e Phi-compatible
-00006480: 206d 6f64 656c 732e 0a0a 0a0a 2323 2320   models.....### 
-00006490: 5375 7070 6f72 7465 6420 6d6f 6465 6c73  Supported models
-000064a0: 0a0a 596f 7520 6361 6e20 7370 6563 6966  ..You can specif
-000064b0: 7920 616e 7920 6f66 2074 6865 2066 6f6c  y any of the fol
-000064c0: 6c6f 7769 6e67 2050 6869 206d 6f64 656c  lowing Phi model
-000064d0: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
-000064e0: 7461 7274 603a 0a0a 0a2d 205b 6d69 6372  tart`:...- [micr
-000064f0: 6f73 6f66 742f 7068 692d 325d 2868 7474  osoft/phi-2](htt
-00006500: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00006510: 2e63 6f2f 6d69 6372 6f73 6f66 742f 7068  .co/microsoft/ph
-00006520: 692d 3229 0a2d 205b 6d69 6372 6f73 6f66  i-2).- [microsof
-00006530: 742f 7068 692d 315f 355d 2868 7474 7073  t/phi-1_5](https
-00006540: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00006550: 6f2f 6d69 6372 6f73 6f66 742f 7068 692d  o/microsoft/phi-
-00006560: 315f 3529 0a0a 3c2f 6465 7461 696c 733e  1_5)..</details>
-00006570: 0a0a 3c64 6574 6169 6c73 3e0a 0a3c 7375  ..<details>..<su
-00006580: 6d6d 6172 793e 5177 656e 3c2f 7375 6d6d  mmary>Qwen</summ
-00006590: 6172 793e 0a0a 0a23 2323 2051 7569 636b  ary>...### Quick
-000065a0: 7374 6172 740a 0a0a 0a3e 202a 2a4e 6f74  start....> **Not
-000065b0: 653a 2a2a 2051 7765 6e20 7265 7175 6972  e:** Qwen requir
-000065c0: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
-000065d0: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
-000065e0: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
-000065f0: 6e6c 6c6d 5b71 7765 6e5d 220a 3e20 6060  nllm[qwen]".> ``
-00006600: 600a 0a0a 5275 6e20 7468 6520 666f 6c6c  `...Run the foll
-00006610: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
-00006620: 2071 7569 636b 6c79 2073 7069 6e20 7570   quickly spin up
-00006630: 2061 2051 7765 6e20 7365 7276 6572 3a0a   a Qwen server:.
-00006640: 0a60 6060 6261 7368 0a54 5255 5354 5f52  .```bash.TRUST_R
-00006650: 454d 4f54 455f 434f 4445 3d54 7275 6520  EMOTE_CODE=True 
-00006660: 6f70 656e 6c6c 6d20 7374 6172 7420 7177  openllm start qw
-00006670: 656e 2f51 7765 6e2d 3742 2d43 6861 740a  en/Qwen-7B-Chat.
-00006680: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
-00006690: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
-000066a0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-000066b0: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
-000066c0: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-000066d0: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
-000066e0: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
-000066f0: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
-00006700: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
-00006710: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
-00006720: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
-00006730: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
-00006740: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
-00006750: 2051 7765 6e20 7661 7269 616e 7473 2063   Qwen variants c
-00006760: 616e 2062 6520 6465 706c 6f79 6564 2077  an be deployed w
-00006770: 6974 6820 4f70 656e 4c4c 4d2e 2056 6973  ith OpenLLM. Vis
-00006780: 6974 2074 6865 205b 4875 6767 696e 6746  it the [HuggingF
-00006790: 6163 6520 4d6f 6465 6c20 4875 625d 2868  ace Model Hub](h
-000067a0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000067b0: 6365 2e63 6f2f 6d6f 6465 6c73 3f73 6f72  ce.co/models?sor
-000067c0: 743d 7472 656e 6469 6e67 2673 6561 7263  t=trending&searc
-000067d0: 683d 7177 656e 2920 746f 2073 6565 206d  h=qwen) to see m
-000067e0: 6f72 6520 5177 656e 2d63 6f6d 7061 7469  ore Qwen-compati
-000067f0: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-00006800: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00006810: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-00006820: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-00006830: 666f 6c6c 6f77 696e 6720 5177 656e 206d  following Qwen m
-00006840: 6f64 656c 7320 7669 6120 606f 7065 6e6c  odels via `openl
-00006850: 6c6d 2073 7461 7274 603a 0a0a 0a2d 205b  lm start`:...- [
-00006860: 7177 656e 2f51 7765 6e2d 3742 2d43 6861  qwen/Qwen-7B-Cha
-00006870: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
-00006880: 6e67 6661 6365 2e63 6f2f 7177 656e 2f51  ngface.co/qwen/Q
-00006890: 7765 6e2d 3742 2d43 6861 7429 0a2d 205b  wen-7B-Chat).- [
-000068a0: 7177 656e 2f51 7765 6e2d 3742 2d43 6861  qwen/Qwen-7B-Cha
-000068b0: 742d 496e 7438 5d28 6874 7470 733a 2f2f  t-Int8](https://
-000068c0: 6875 6767 696e 6766 6163 652e 636f 2f71  huggingface.co/q
-000068d0: 7765 6e2f 5177 656e 2d37 422d 4368 6174  wen/Qwen-7B-Chat
-000068e0: 2d49 6e74 3829 0a2d 205b 7177 656e 2f51  -Int8).- [qwen/Q
-000068f0: 7765 6e2d 3742 2d43 6861 742d 496e 7434  wen-7B-Chat-Int4
-00006900: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00006910: 6766 6163 652e 636f 2f71 7765 6e2f 5177  gface.co/qwen/Qw
-00006920: 656e 2d37 422d 4368 6174 2d49 6e74 3429  en-7B-Chat-Int4)
-00006930: 0a2d 205b 7177 656e 2f51 7765 6e2d 3134  .- [qwen/Qwen-14
-00006940: 422d 4368 6174 5d28 6874 7470 733a 2f2f  B-Chat](https://
-00006950: 6875 6767 696e 6766 6163 652e 636f 2f71  huggingface.co/q
-00006960: 7765 6e2f 5177 656e 2d31 3442 2d43 6861  wen/Qwen-14B-Cha
-00006970: 7429 0a2d 205b 7177 656e 2f51 7765 6e2d  t).- [qwen/Qwen-
-00006980: 3134 422d 4368 6174 2d49 6e74 385d 2868  14B-Chat-Int8](h
-00006990: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000069a0: 6365 2e63 6f2f 7177 656e 2f51 7765 6e2d  ce.co/qwen/Qwen-
-000069b0: 3134 422d 4368 6174 2d49 6e74 3829 0a2d  14B-Chat-Int8).-
-000069c0: 205b 7177 656e 2f51 7765 6e2d 3134 422d   [qwen/Qwen-14B-
-000069d0: 4368 6174 2d49 6e74 345d 2868 7474 7073  Chat-Int4](https
-000069e0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-000069f0: 6f2f 7177 656e 2f51 7765 6e2d 3134 422d  o/qwen/Qwen-14B-
-00006a00: 4368 6174 2d49 6e74 3429 0a0a 3c2f 6465  Chat-Int4)..</de
-00006a10: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
-00006a20: 3e0a 0a3c 7375 6d6d 6172 793e 5374 6162  >..<summary>Stab
-00006a30: 6c65 4c4d 3c2f 7375 6d6d 6172 793e 0a0a  leLM</summary>..
-00006a40: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
-00006a50: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2053  ...> **Note:** S
-00006a60: 7461 626c 654c 4d20 7265 7175 6972 6573  tableLM requires
-00006a70: 2074 6f20 696e 7374 616c 6c20 7769 7468   to install with
-00006a80: 3a0a 3e20 6060 6062 6173 680a 3e20 7069  :.> ```bash.> pi
-00006a90: 7020 696e 7374 616c 6c20 226f 7065 6e6c  p install "openl
-00006aa0: 6c6d 5b73 7461 626c 656c 6d5d 220a 3e20  lm[stablelm]".> 
-00006ab0: 6060 600a 0a0a 5275 6e20 7468 6520 666f  ```...Run the fo
-00006ac0: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
-00006ad0: 746f 2071 7569 636b 6c79 2073 7069 6e20  to quickly spin 
-00006ae0: 7570 2061 2053 7461 626c 654c 4d20 7365  up a StableLM se
-00006af0: 7276 6572 3a0a 0a60 6060 6261 7368 0a54  rver:..```bash.T
-00006b00: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
-00006b10: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
-00006b20: 6172 7420 7374 6162 696c 6974 7961 692f  art stabilityai/
-00006b30: 7374 6162 6c65 6c6d 2d74 756e 6564 2d61  stablelm-tuned-a
-00006b40: 6c70 6861 2d33 620a 6060 600a 496e 2061  lpha-3b.```.In a
-00006b50: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
-00006b60: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
-00006b70: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-00006b80: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-00006b90: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
-00006ba0: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
-00006bb0: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
-00006bc0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-00006bd0: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
-00006be0: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
-00006bf0: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00006c00: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
-00006c10: 653a 2a2a 2041 6e79 2053 7461 626c 654c  e:** Any StableL
-00006c20: 4d20 7661 7269 616e 7473 2063 616e 2062  M variants can b
-00006c30: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
-00006c40: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
-00006c50: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
-00006c60: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
-00006c70: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00006c80: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
-00006c90: 656e 6469 6e67 2673 6561 7263 683d 7374  ending&search=st
-00006ca0: 6162 6c65 6c6d 2920 746f 2073 6565 206d  ablelm) to see m
-00006cb0: 6f72 6520 5374 6162 6c65 4c4d 2d63 6f6d  ore StableLM-com
-00006cc0: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
-00006cd0: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
-00006ce0: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
-00006cf0: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
-00006d00: 7468 6520 666f 6c6c 6f77 696e 6720 5374  the following St
-00006d10: 6162 6c65 4c4d 206d 6f64 656c 7320 7669  ableLM models vi
-00006d20: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
-00006d30: 603a 0a0a 0a2d 205b 7374 6162 696c 6974  `:...- [stabilit
-00006d40: 7961 692f 7374 6162 6c65 6c6d 2d74 756e  yai/stablelm-tun
-00006d50: 6564 2d61 6c70 6861 2d33 625d 2868 7474  ed-alpha-3b](htt
-00006d60: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00006d70: 2e63 6f2f 7374 6162 696c 6974 7961 692f  .co/stabilityai/
-00006d80: 7374 6162 6c65 6c6d 2d74 756e 6564 2d61  stablelm-tuned-a
-00006d90: 6c70 6861 2d33 6229 0a2d 205b 7374 6162  lpha-3b).- [stab
-00006da0: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
-00006db0: 2d74 756e 6564 2d61 6c70 6861 2d37 625d  -tuned-alpha-7b]
-00006dc0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00006dd0: 6661 6365 2e63 6f2f 7374 6162 696c 6974  face.co/stabilit
-00006de0: 7961 692f 7374 6162 6c65 6c6d 2d74 756e  yai/stablelm-tun
-00006df0: 6564 2d61 6c70 6861 2d37 6229 0a2d 205b  ed-alpha-7b).- [
-00006e00: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
-00006e10: 6c65 6c6d 2d62 6173 652d 616c 7068 612d  lelm-base-alpha-
-00006e20: 3362 5d28 6874 7470 733a 2f2f 6875 6767  3b](https://hugg
-00006e30: 696e 6766 6163 652e 636f 2f73 7461 6269  ingface.co/stabi
-00006e40: 6c69 7479 6169 2f73 7461 626c 656c 6d2d  lityai/stablelm-
-00006e50: 6261 7365 2d61 6c70 6861 2d33 6229 0a2d  base-alpha-3b).-
-00006e60: 205b 7374 6162 696c 6974 7961 692f 7374   [stabilityai/st
-00006e70: 6162 6c65 6c6d 2d62 6173 652d 616c 7068  ablelm-base-alph
-00006e80: 612d 3762 5d28 6874 7470 733a 2f2f 6875  a-7b](https://hu
-00006e90: 6767 696e 6766 6163 652e 636f 2f73 7461  ggingface.co/sta
-00006ea0: 6269 6c69 7479 6169 2f73 7461 626c 656c  bilityai/stablel
-00006eb0: 6d2d 6261 7365 2d61 6c70 6861 2d37 6229  m-base-alpha-7b)
-00006ec0: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
-00006ed0: 6574 6169 6c73 3e0a 0a3c 7375 6d6d 6172  etails>..<summar
-00006ee0: 793e 5374 6172 436f 6465 723c 2f73 756d  y>StarCoder</sum
-00006ef0: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
-00006f00: 6b73 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f  kstart....> **No
-00006f10: 7465 3a2a 2a20 5374 6172 436f 6465 7220  te:** StarCoder 
-00006f20: 7265 7175 6972 6573 2074 6f20 696e 7374  requires to inst
-00006f30: 616c 6c20 7769 7468 3a0a 3e20 6060 6062  all with:.> ```b
-00006f40: 6173 680a 3e20 7069 7020 696e 7374 616c  ash.> pip instal
-00006f50: 6c20 226f 7065 6e6c 6c6d 5b73 7461 7263  l "openllm[starc
-00006f60: 6f64 6572 5d22 0a3e 2060 6060 0a0a 0a52  oder]".> ```...R
-00006f70: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00006f80: 2063 6f6d 6d61 6e64 2074 6f20 7175 6963   command to quic
-00006f90: 6b6c 7920 7370 696e 2075 7020 6120 5374  kly spin up a St
-00006fa0: 6172 436f 6465 7220 7365 7276 6572 3a0a  arCoder server:.
-00006fb0: 0a60 6060 6261 7368 0a54 5255 5354 5f52  .```bash.TRUST_R
-00006fc0: 454d 4f54 455f 434f 4445 3d54 7275 6520  EMOTE_CODE=True 
-00006fd0: 6f70 656e 6c6c 6d20 7374 6172 7420 6269  openllm start bi
-00006fe0: 6763 6f64 652f 7374 6172 636f 6465 720a  gcode/starcoder.
-00006ff0: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
-00007000: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
-00007010: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00007020: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
-00007030: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-00007040: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
-00007050: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
-00007060: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
-00007070: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
-00007080: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
-00007090: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
-000070a0: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
-000070b0: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
-000070c0: 2053 7461 7243 6f64 6572 2076 6172 6961   StarCoder varia
-000070d0: 6e74 7320 6361 6e20 6265 2064 6570 6c6f  nts can be deplo
-000070e0: 7965 6420 7769 7468 204f 7065 6e4c 4c4d  yed with OpenLLM
-000070f0: 2e20 5669 7369 7420 7468 6520 5b48 7567  . Visit the [Hug
-00007100: 6769 6e67 4661 6365 204d 6f64 656c 2048  gingFace Model H
-00007110: 7562 5d28 6874 7470 733a 2f2f 6875 6767  ub](https://hugg
-00007120: 696e 6766 6163 652e 636f 2f6d 6f64 656c  ingface.co/model
-00007130: 733f 736f 7274 3d74 7265 6e64 696e 6726  s?sort=trending&
-00007140: 7365 6172 6368 3d73 7461 7263 6f64 6572  search=starcoder
-00007150: 2920 746f 2073 6565 206d 6f72 6520 5374  ) to see more St
-00007160: 6172 436f 6465 722d 636f 6d70 6174 6962  arCoder-compatib
-00007170: 6c65 206d 6f64 656c 732e 0a0a 0a0a 2323  le models.....##
-00007180: 2320 5375 7070 6f72 7465 6420 6d6f 6465  # Supported mode
-00007190: 6c73 0a0a 596f 7520 6361 6e20 7370 6563  ls..You can spec
-000071a0: 6966 7920 616e 7920 6f66 2074 6865 2066  ify any of the f
-000071b0: 6f6c 6c6f 7769 6e67 2053 7461 7243 6f64  ollowing StarCod
-000071c0: 6572 206d 6f64 656c 7320 7669 6120 606f  er models via `o
-000071d0: 7065 6e6c 6c6d 2073 7461 7274 603a 0a0a  penllm start`:..
-000071e0: 0a2d 205b 6269 6763 6f64 652f 7374 6172  .- [bigcode/star
-000071f0: 636f 6465 725d 2868 7474 7073 3a2f 2f68  coder](https://h
-00007200: 7567 6769 6e67 6661 6365 2e63 6f2f 6269  uggingface.co/bi
-00007210: 6763 6f64 652f 7374 6172 636f 6465 7229  gcode/starcoder)
-00007220: 0a2d 205b 6269 6763 6f64 652f 7374 6172  .- [bigcode/star
-00007230: 636f 6465 7262 6173 655d 2868 7474 7073  coderbase](https
-00007240: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00007250: 6f2f 6269 6763 6f64 652f 7374 6172 636f  o/bigcode/starco
-00007260: 6465 7262 6173 6529 0a0a 3c2f 6465 7461  derbase)..</deta
-00007270: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
-00007280: 0a3c 7375 6d6d 6172 793e 5969 3c2f 7375  .<summary>Yi</su
-00007290: 6d6d 6172 793e 0a0a 0a23 2323 2051 7569  mmary>...### Qui
-000072a0: 636b 7374 6172 740a 0a0a 0a3e 202a 2a4e  ckstart....> **N
-000072b0: 6f74 653a 2a2a 2059 6920 7265 7175 6972  ote:** Yi requir
-000072c0: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
-000072d0: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
-000072e0: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
-000072f0: 6e6c 6c6d 5b79 695d 220a 3e20 6060 600a  nllm[yi]".> ```.
-00007300: 0a0a 5275 6e20 7468 6520 666f 6c6c 6f77  ..Run the follow
-00007310: 696e 6720 636f 6d6d 616e 6420 746f 2071  ing command to q
-00007320: 7569 636b 6c79 2073 7069 6e20 7570 2061  uickly spin up a
-00007330: 2059 6920 7365 7276 6572 3a0a 0a60 6060   Yi server:..```
-00007340: 6261 7368 0a54 5255 5354 5f52 454d 4f54  bash.TRUST_REMOT
-00007350: 455f 434f 4445 3d54 7275 6520 6f70 656e  E_CODE=True open
-00007360: 6c6c 6d20 7374 6172 7420 3031 2d61 692f  llm start 01-ai/
-00007370: 5969 2d36 420a 6060 600a 496e 2061 2064  Yi-6B.```.In a d
-00007380: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
-00007390: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
-000073a0: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-000073b0: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
-000073c0: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
-000073d0: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-000073e0: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
-000073f0: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-00007400: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
-00007410: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
-00007420: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
-00007430: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
-00007440: 2a2a 2041 6e79 2059 6920 7661 7269 616e  ** Any Yi varian
-00007450: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
-00007460: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
-00007470: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
-00007480: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
-00007490: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-000074a0: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
-000074b0: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
-000074c0: 6561 7263 683d 7969 2920 746f 2073 6565  earch=yi) to see
-000074d0: 206d 6f72 6520 5969 2d63 6f6d 7061 7469   more Yi-compati
-000074e0: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-000074f0: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00007500: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-00007510: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-00007520: 666f 6c6c 6f77 696e 6720 5969 206d 6f64  following Yi mod
-00007530: 656c 7320 7669 6120 606f 7065 6e6c 6c6d  els via `openllm
-00007540: 2073 7461 7274 603a 0a0a 0a2d 205b 3031   start`:...- [01
-00007550: 2d61 692f 5969 2d36 425d 2868 7474 7073  -ai/Yi-6B](https
-00007560: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00007570: 6f2f 3031 2d61 692f 5969 2d36 4229 0a2d  o/01-ai/Yi-6B).-
-00007580: 205b 3031 2d61 692f 5969 2d33 3442 5d28   [01-ai/Yi-34B](
-00007590: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-000075a0: 6163 652e 636f 2f30 312d 6169 2f59 692d  ace.co/01-ai/Yi-
-000075b0: 3334 4229 0a2d 205b 3031 2d61 692f 5969  34B).- [01-ai/Yi
-000075c0: 2d36 422d 3230 304b 5d28 6874 7470 733a  -6B-200K](https:
-000075d0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000075e0: 2f30 312d 6169 2f59 692d 3642 2d32 3030  /01-ai/Yi-6B-200
-000075f0: 4b29 0a2d 205b 3031 2d61 692f 5969 2d33  K).- [01-ai/Yi-3
-00007600: 3442 2d32 3030 4b5d 2868 7474 7073 3a2f  4B-200K](https:/
-00007610: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00007620: 3031 2d61 692f 5969 2d33 3442 2d32 3030  01-ai/Yi-34B-200
-00007630: 4b29 0a0a 3c2f 6465 7461 696c 733e 0a0a  K)..</details>..
-00007640: 3c21 2d2d 2075 7064 6174 652d 7265 6164  <!-- update-read
-00007650: 6d65 2e70 793a 2073 746f 7020 2d2d 3e0a  me.py: stop -->.
-00007660: 0a4d 6f72 6520 6d6f 6465 6c73 2077 696c  .More models wil
-00007670: 6c20 6265 2069 6e74 6567 7261 7465 6420  l be integrated 
-00007680: 7769 7468 204f 7065 6e4c 4c4d 2061 6e64  with OpenLLM and
-00007690: 2077 6520 7765 6c63 6f6d 6520 796f 7572   we welcome your
-000076a0: 2063 6f6e 7472 6962 7574 696f 6e73 2069   contributions i
-000076b0: 6620 796f 7520 7761 6e74 2074 6f20 696e  f you want to in
-000076c0: 636f 7270 6f72 6174 6520 796f 7572 2063  corporate your c
-000076d0: 7573 746f 6d20 4c4c 4d73 2069 6e74 6f20  ustom LLMs into 
-000076e0: 7468 6520 6563 6f73 7973 7465 6d2e 2043  the ecosystem. C
-000076f0: 6865 636b 206f 7574 205b 4164 6469 6e67  heck out [Adding
-00007700: 2061 204e 6577 204d 6f64 656c 2047 7569   a New Model Gui
-00007710: 6465 5d28 6874 7470 733a 2f2f 6769 7468  de](https://gith
-00007720: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-00007730: 7065 6e4c 4c4d 2f62 6c6f 622f 6d61 696e  penLLM/blob/main
-00007740: 2f41 4444 494e 475f 4e45 575f 4d4f 4445  /ADDING_NEW_MODE
-00007750: 4c2e 6d64 2920 746f 206c 6561 726e 206d  L.md) to learn m
-00007760: 6f72 652e 0a0a 2323 20f0 9f92 bb20 5275  ore...## .... Ru
-00007770: 6e20 796f 7572 206d 6f64 656c 206f 6e20  n your model on 
-00007780: 6d75 6c74 6970 6c65 2047 5055 730a 0a4f  multiple GPUs..O
-00007790: 7065 6e4c 4c4d 2061 6c6c 6f77 7320 796f  penLLM allows yo
-000077a0: 7520 746f 2073 7461 7274 2079 6f75 7220  u to start your 
-000077b0: 6d6f 6465 6c20 7365 7276 6572 206f 6e20  model server on 
-000077c0: 6d75 6c74 6970 6c65 2047 5055 7320 616e  multiple GPUs an
-000077d0: 6420 7370 6563 6966 7920 7468 6520 6e75  d specify the nu
-000077e0: 6d62 6572 206f 6620 776f 726b 6572 7320  mber of workers 
-000077f0: 7065 7220 7265 736f 7572 6365 2061 7373  per resource ass
-00007800: 6967 6e65 6420 7573 696e 6720 7468 6520  igned using the 
-00007810: 602d 2d77 6f72 6b65 7273 2d70 6572 2d72  `--workers-per-r
-00007820: 6573 6f75 7263 6560 206f 7074 696f 6e2e  esource` option.
-00007830: 2046 6f72 2065 7861 6d70 6c65 2c20 6966   For example, if
-00007840: 2079 6f75 2068 6176 6520 3420 6176 6169   you have 4 avai
-00007850: 6c61 626c 6520 4750 5573 2c20 796f 7520  lable GPUs, you 
-00007860: 7365 7420 7468 6520 7661 6c75 6520 6173  set the value as
-00007870: 206f 6e65 2064 6976 6964 6564 2062 7920   one divided by 
-00007880: 7468 6520 6e75 6d62 6572 2061 7320 6f6e  the number as on
-00007890: 6c79 206f 6e65 2069 6e73 7461 6e63 6520  ly one instance 
-000078a0: 6f66 2074 6865 2052 756e 6e65 7220 7365  of the Runner se
-000078b0: 7276 6572 2077 696c 6c20 6265 2073 7061  rver will be spa
-000078c0: 776e 6564 2e0a 0a60 6060 6261 7368 0a54  wned...```bash.T
-000078d0: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
-000078e0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
-000078f0: 6172 7420 6d69 6372 6f73 6f66 742f 7068  art microsoft/ph
-00007900: 692d 3220 2d2d 776f 726b 6572 732d 7065  i-2 --workers-pe
-00007910: 722d 7265 736f 7572 6365 2030 2e32 350a  r-resource 0.25.
-00007920: 6060 600a 0a3e 205b 214e 4f54 455d 0a3e  ```..> [!NOTE].>
-00007930: 2054 6865 2061 6d6f 756e 7420 6f66 2047   The amount of G
-00007940: 5055 7320 7265 7175 6972 6564 2064 6570  PUs required dep
-00007950: 656e 6473 206f 6e20 7468 6520 6d6f 6465  ends on the mode
-00007960: 6c20 7369 7a65 2069 7473 656c 662e 0a3e  l size itself..>
-00007970: 2059 6f75 2063 616e 2075 7365 205b 7468   You can use [th
-00007980: 6520 4d6f 6465 6c20 4d65 6d6f 7279 2043  e Model Memory C
-00007990: 616c 6375 6c61 746f 7220 6672 6f6d 2048  alculator from H
-000079a0: 7567 6769 6e67 2046 6163 655d 2868 7474  ugging Face](htt
-000079b0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-000079c0: 2e63 6f2f 7370 6163 6573 2f68 662d 6163  .co/spaces/hf-ac
-000079d0: 6365 6c65 7261 7465 2f6d 6f64 656c 2d6d  celerate/model-m
-000079e0: 656d 6f72 792d 7573 6167 6529 2074 6f0a  emory-usage) to.
-000079f0: 3e20 6361 6c63 756c 6174 6520 686f 7720  > calculate how 
-00007a00: 6d75 6368 2076 5241 4d20 6973 206e 6565  much vRAM is nee
-00007a10: 6465 6420 746f 2074 7261 696e 2061 6e64  ded to train and
-00007a20: 2070 6572 666f 726d 2062 6967 206d 6f64   perform big mod
-00007a30: 656c 0a3e 2069 6e66 6572 656e 6365 206f  el.> inference o
-00007a40: 6e20 6120 6d6f 6465 6c20 616e 6420 7468  n a model and th
-00007a50: 656e 2070 6c61 6e20 796f 7572 2047 5055  en plan your GPU
-00007a60: 2073 7472 6174 6567 7920 6261 7365 6420   strategy based 
-00007a70: 6f6e 2069 742e 0a0a 5768 656e 2075 7369  on it...When usi
-00007a80: 6e67 2074 6865 2060 2d2d 776f 726b 6572  ng the `--worker
-00007a90: 732d 7065 722d 7265 736f 7572 6365 6020  s-per-resource` 
-00007aa0: 6f70 7469 6f6e 2077 6974 6820 7468 6520  option with the 
-00007ab0: 606f 7065 6e6c 6c6d 2062 7569 6c64 6020  `openllm build` 
-00007ac0: 636f 6d6d 616e 642c 2074 6865 2065 6e76  command, the env
-00007ad0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00007ae0: 6520 6973 2073 6176 6564 2069 6e74 6f20  e is saved into 
-00007af0: 7468 6520 7265 7375 6c74 696e 6720 4265  the resulting Be
-00007b00: 6e74 6f2e 0a0a 466f 7220 6d6f 7265 2069  nto...For more i
-00007b10: 6e66 6f72 6d61 7469 6f6e 2c20 7365 6520  nformation, see 
-00007b20: 5b52 6573 6f75 7263 6520 7363 6865 6475  [Resource schedu
-00007b30: 6c69 6e67 2073 7472 6174 6567 795d 2868  ling strategy](h
-00007b40: 7474 7073 3a2f 2f64 6f63 732e 6265 6e74  ttps://docs.bent
-00007b50: 6f6d 6c2e 6f72 672f 656e 2f6c 6174 6573  oml.org/en/lates
-00007b60: 742f 6775 6964 6573 2f73 6368 6564 756c  t/guides/schedul
-00007b70: 696e 672e 6874 6d6c 2329 2e0a 0a23 2320  ing.html#)...## 
-00007b80: f09f 9b9e 2052 756e 7469 6d65 2069 6d70  .... Runtime imp
-00007b90: 6c65 6d65 6e74 6174 696f 6e73 0a0a 4469  lementations..Di
-00007ba0: 6666 6572 656e 7420 4c4c 4d73 206d 6179  fferent LLMs may
-00007bb0: 2073 7570 706f 7274 206d 756c 7469 706c   support multipl
-00007bc0: 6520 7275 6e74 696d 6520 696d 706c 656d  e runtime implem
-00007bd0: 656e 7461 7469 6f6e 732e 204d 6f64 656c  entations. Model
-00007be0: 7320 7468 6174 2068 6176 6520 6076 4c4c  s that have `vLL
-00007bf0: 4d60 2028 6076 6c6c 6d60 2920 7375 7070  M` (`vllm`) supp
-00007c00: 6f72 7473 2077 696c 6c20 7573 6520 764c  orts will use vL
-00007c10: 4c4d 2062 7920 6465 6661 756c 742c 206f  LM by default, o
-00007c20: 7468 6572 7769 7365 2069 7420 6661 6c6c  therwise it fall
-00007c30: 6261 636b 2074 6f20 7573 6520 6050 7954  back to use `PyT
-00007c40: 6f72 6368 6020 2860 7074 6029 2e0a 0a54  orch` (`pt`)...T
-00007c50: 6f20 7370 6563 6966 7920 6120 7370 6563  o specify a spec
-00007c60: 6966 6963 2072 756e 7469 6d65 2066 6f72  ific runtime for
-00007c70: 2079 6f75 7220 6368 6f73 656e 206d 6f64   your chosen mod
-00007c80: 656c 2c20 7573 6520 7468 6520 602d 2d62  el, use the `--b
-00007c90: 6163 6b65 6e64 6020 6f70 7469 6f6e 2e20  ackend` option. 
-00007ca0: 466f 7220 6578 616d 706c 653a 0a0a 6060  For example:..``
-00007cb0: 6062 6173 680a 6f70 656e 6c6c 6d20 7374  `bash.openllm st
-00007cc0: 6172 7420 6d65 7461 2d6c 6c61 6d61 2f4c  art meta-llama/L
-00007cd0: 6c61 6d61 2d32 2d37 622d 6368 6174 2d68  lama-2-7b-chat-h
-00007ce0: 6620 2d2d 6261 636b 656e 6420 766c 6c6d  f --backend vllm
-00007cf0: 0a60 6060 0a0a 4e6f 7465 3a0a 0a31 2e20  .```..Note:..1. 
-00007d00: 546f 2075 7365 2074 6865 2076 4c4c 4d20  To use the vLLM 
-00007d10: 6261 636b 656e 642c 2079 6f75 206e 6565  backend, you nee
-00007d20: 6420 6120 4750 5520 7769 7468 2061 7420  d a GPU with at 
-00007d30: 6c65 6173 7420 7468 6520 416d 7065 7265  least the Ampere
-00007d40: 2061 7263 6869 7465 6374 7572 6520 6f72   architecture or
-00007d50: 206e 6577 6572 2061 6e64 2043 5544 4120   newer and CUDA 
-00007d60: 7665 7273 696f 6e20 3131 2e38 2e0a 322e  version 11.8..2.
-00007d70: 2054 6f20 7365 6520 7468 6520 6261 636b   To see the back
-00007d80: 656e 6420 6f70 7469 6f6e 7320 6f66 2065  end options of e
-00007d90: 6163 6820 6d6f 6465 6c20 7375 7070 6f72  ach model suppor
-00007da0: 7465 6420 6279 204f 7065 6e4c 4c4d 2c20  ted by OpenLLM, 
-00007db0: 7365 6520 7468 6520 5375 7070 6f72 7465  see the Supporte
-00007dc0: 6420 6d6f 6465 6c73 2073 6563 7469 6f6e  d models section
-00007dd0: 206f 7220 7275 6e20 606f 7065 6e6c 6c6d   or run `openllm
-00007de0: 206d 6f64 656c 7360 2e0a 0a23 2320 f09f   models`...## ..
-00007df0: 9390 2051 7561 6e74 697a 6174 696f 6e0a  .. Quantization.
-00007e00: 0a51 7561 6e74 697a 6174 696f 6e20 6973  .Quantization is
-00007e10: 2061 2074 6563 686e 6971 7565 2074 6f20   a technique to 
-00007e20: 7265 6475 6365 2074 6865 2073 746f 7261  reduce the stora
-00007e30: 6765 2061 6e64 2063 6f6d 7075 7461 7469  ge and computati
-00007e40: 6f6e 2072 6571 7569 7265 6d65 6e74 7320  on requirements 
-00007e50: 666f 7220 6d61 6368 696e 6520 6c65 6172  for machine lear
-00007e60: 6e69 6e67 206d 6f64 656c 732c 2070 6172  ning models, par
-00007e70: 7469 6375 6c61 726c 7920 6475 7269 6e67  ticularly during
-00007e80: 2069 6e66 6572 656e 6365 2e20 4279 2061   inference. By a
-00007e90: 7070 726f 7869 6d61 7469 6e67 2066 6c6f  pproximating flo
-00007ea0: 6174 696e 672d 706f 696e 7420 6e75 6d62  ating-point numb
-00007eb0: 6572 7320 6173 2069 6e74 6567 6572 7320  ers as integers 
-00007ec0: 2871 7561 6e74 697a 6564 2076 616c 7565  (quantized value
-00007ed0: 7329 2c20 7175 616e 7469 7a61 7469 6f6e  s), quantization
-00007ee0: 2061 6c6c 6f77 7320 666f 7220 6661 7374   allows for fast
-00007ef0: 6572 2063 6f6d 7075 7461 7469 6f6e 732c  er computations,
-00007f00: 2072 6564 7563 6564 206d 656d 6f72 7920   reduced memory 
-00007f10: 666f 6f74 7072 696e 742c 2061 6e64 2063  footprint, and c
-00007f20: 616e 206d 616b 6520 6974 2066 6561 7369  an make it feasi
-00007f30: 626c 6520 746f 2064 6570 6c6f 7920 6c61  ble to deploy la
-00007f40: 7267 6520 6d6f 6465 6c73 206f 6e20 7265  rge models on re
-00007f50: 736f 7572 6365 2d63 6f6e 7374 7261 696e  source-constrain
-00007f60: 6564 2064 6576 6963 6573 2e0a 0a4f 7065  ed devices...Ope
-00007f70: 6e4c 4c4d 2073 7570 706f 7274 7320 7468  nLLM supports th
-00007f80: 6520 666f 6c6c 6f77 696e 6720 7175 616e  e following quan
-00007f90: 7469 7a61 7469 6f6e 2074 6563 686e 6971  tization techniq
-00007fa0: 7565 730a 0a2d 205b 4c4c 4d2e 696e 7438  ues..- [LLM.int8
-00007fb0: 2829 3a20 382d 6269 7420 4d61 7472 6978  (): 8-bit Matrix
-00007fc0: 204d 756c 7469 706c 6963 6174 696f 6e5d   Multiplication]
-00007fd0: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-00007fe0: 7267 2f61 6273 2f32 3230 382e 3037 3333  rg/abs/2208.0733
-00007ff0: 3929 2074 6872 6f75 6768 205b 6269 7473  9) through [bits
-00008000: 616e 6462 7974 6573 5d28 6874 7470 733a  andbytes](https:
-00008010: 2f2f 6769 7468 7562 2e63 6f6d 2f54 696d  //github.com/Tim
-00008020: 4465 7474 6d65 7273 2f62 6974 7361 6e64  Dettmers/bitsand
-00008030: 6279 7465 7329 0a2d 205b 5370 5152 3a20  bytes).- [SpQR: 
-00008040: 4120 5370 6172 7365 2d51 7561 6e74 697a  A Sparse-Quantiz
-00008050: 6564 2052 6570 7265 7365 6e74 6174 696f  ed Representatio
-00008060: 6e20 666f 7220 4e65 6172 2d4c 6f73 736c  n for Near-Lossl
-00008070: 6573 7320 4c4c 4d20 5765 6967 6874 2043  ess LLM Weight C
-00008080: 6f6d 7072 6573 7369 6f6e 0a20 205d 2868  ompression.  ](h
-00008090: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000080a0: 2f61 6273 2f32 3330 362e 3033 3037 3829  /abs/2306.03078)
-000080b0: 2074 6872 6f75 6768 205b 6269 7473 616e   through [bitsan
-000080c0: 6462 7974 6573 5d28 6874 7470 733a 2f2f  dbytes](https://
-000080d0: 6769 7468 7562 2e63 6f6d 2f54 696d 4465  github.com/TimDe
-000080e0: 7474 6d65 7273 2f62 6974 7361 6e64 6279  ttmers/bitsandby
-000080f0: 7465 7329 0a2d 205b 4157 513a 2041 6374  tes).- [AWQ: Act
-00008100: 6976 6174 696f 6e2d 6177 6172 6520 5765  ivation-aware We
-00008110: 6967 6874 2051 7561 6e74 697a 6174 696f  ight Quantizatio
-00008120: 6e5d 2868 7474 7073 3a2f 2f61 7278 6976  n](https://arxiv
-00008130: 2e6f 7267 2f61 6273 2f32 3330 362e 3030  .org/abs/2306.00
-00008140: 3937 3829 2c0a 2d20 5b47 5054 513a 2041  978),.- [GPTQ: A
-00008150: 6363 7572 6174 6520 506f 7374 2d54 7261  ccurate Post-Tra
-00008160: 696e 696e 6720 5175 616e 7469 7a61 7469  ining Quantizati
-00008170: 6f6e 5d28 6874 7470 733a 2f2f 6172 7869  on](https://arxi
-00008180: 762e 6f72 672f 6162 732f 3232 3130 2e31  v.org/abs/2210.1
-00008190: 3733 3233 290a 2d20 5b53 7175 6565 7a65  7323).- [Squeeze
-000081a0: 4c4c 4d3a 2044 656e 7365 2d61 6e64 2d53  LLM: Dense-and-S
-000081b0: 7061 7273 6520 5175 616e 7469 7a61 7469  parse Quantizati
-000081c0: 6f6e 5d28 6874 7470 733a 2f2f 6172 7869  on](https://arxi
-000081d0: 762e 6f72 672f 6162 732f 3233 3036 2e30  v.org/abs/2306.0
-000081e0: 3736 3239 292e 0a0a 2323 2320 5079 546f  7629)...### PyTo
-000081f0: 7263 6820 6261 636b 656e 640a 0a57 6974  rch backend..Wit
-00008200: 6820 5079 546f 7263 6820 6261 636b 656e  h PyTorch backen
-00008210: 642c 204f 7065 6e4c 4c4d 2073 7570 706f  d, OpenLLM suppo
-00008220: 7274 7320 6069 6e74 3860 2c20 6069 6e74  rts `int8`, `int
-00008230: 3460 2c20 616e 6420 6067 7074 7160 2e0a  4`, and `gptq`..
-00008240: 0a46 6f72 2075 7369 6e67 2069 6e74 3820  .For using int8 
-00008250: 616e 6420 696e 7434 2071 7561 6e74 697a  and int4 quantiz
-00008260: 6174 696f 6e20 7468 726f 7567 6820 6062  ation through `b
-00008270: 6974 7361 6e64 6279 7465 7360 2c20 796f  itsandbytes`, yo
-00008280: 7520 6361 6e20 7573 6520 7468 6520 666f  u can use the fo
-00008290: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-000082a0: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
-000082b0: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
-000082c0: 206f 7065 6e6c 6c6d 2073 7461 7274 206d   openllm start m
-000082d0: 6963 726f 736f 6674 2f70 6869 2d32 202d  icrosoft/phi-2 -
-000082e0: 2d71 7561 6e74 697a 6520 696e 7438 0a60  -quantize int8.`
-000082f0: 6060 0a0a 546f 2072 756e 2069 6e66 6572  ``..To run infer
-00008300: 656e 6365 2077 6974 68c2 a060 6770 7471  ence with..`gptq
-00008310: 602c 2073 696d 706c 7920 7061 7373 c2a0  `, simply pass..
-00008320: 602d 2d71 7561 6e74 697a 6520 6770 7471  `--quantize gptq
-00008330: 603a 0a0a 6060 6062 6173 680a 6f70 656e  `:..```bash.open
-00008340: 6c6c 6d20 7374 6172 7420 5468 6542 6c6f  llm start TheBlo
-00008350: 6b65 2f4c 6c61 6d61 2d32 2d37 422d 4368  ke/Llama-2-7B-Ch
-00008360: 6174 2d47 5054 5120 2d2d 7175 616e 7469  at-GPTQ --quanti
-00008370: 7a65 2067 7074 710a 6060 600a 0a3e 205b  ze gptq.```..> [
-00008380: 214e 4f54 455d 0a3e 2049 6e20 6f72 6465  !NOTE].> In orde
-00008390: 7220 746f 2072 756e 2047 5054 512c 206d  r to run GPTQ, m
-000083a0: 616b 6520 7375 7265 2079 6f75 2072 756e  ake sure you run
-000083b0: c2a0 6070 6970 2069 6e73 7461 6c6c 2022  ..`pip install "
-000083c0: 6f70 656e 6c6c 6d5b 6770 7471 5d22 600a  openllm[gptq]"`.
-000083d0: 3e20 6669 7273 7420 746f 2069 6e73 7461  > first to insta
-000083e0: 6c6c 2074 6865 2064 6570 656e 6465 6e63  ll the dependenc
-000083f0: 792e 2046 726f 6d20 7468 6520 4750 5451  y. From the GPTQ
-00008400: 2070 6170 6572 2c20 6974 2069 7320 7265   paper, it is re
-00008410: 636f 6d6d 656e 6465 6420 746f 2071 7561  commended to qua
-00008420: 6e74 697a 6564 2074 6865 2077 6569 6768  ntized the weigh
-00008430: 7473 2062 6566 6f72 6520 7365 7276 696e  ts before servin
-00008440: 672e 0a3e 2053 6565 c2a0 5b41 7574 6f47  g..> See..[AutoG
-00008450: 5054 515d 2868 7474 7073 3a2f 2f67 6974  PTQ](https://git
-00008460: 6875 622e 636f 6d2f 5061 6e51 6957 6569  hub.com/PanQiWei
-00008470: 2f41 7574 6f47 5054 5129 c2a0 666f 7220  /AutoGPTQ)..for 
-00008480: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
-00008490: 206f 6e20 4750 5451 2071 7561 6e74 697a   on GPTQ quantiz
-000084a0: 6174 696f 6e2e 0a0a 2323 2320 764c 4c4d  ation...### vLLM
-000084b0: 2062 6163 6b65 6e64 0a0a 5769 7468 2076   backend..With v
-000084c0: 4c4c 4d20 6261 636b 656e 642c 204f 7065  LLM backend, Ope
-000084d0: 6e4c 4c4d 2073 7570 706f 7274 7320 6061  nLLM supports `a
-000084e0: 7771 602c 2060 7371 7565 657a 656c 6c6d  wq`, `squeezellm
-000084f0: 600a 0a54 6f20 7275 6e20 696e 6665 7265  `..To run infere
-00008500: 6e63 6520 7769 7468 c2a0 6061 7771 602c  nce with..`awq`,
-00008510: 2073 696d 706c 7920 7061 7373 c2a0 602d   simply pass..`-
-00008520: 2d71 7561 6e74 697a 6520 6177 7160 3a0a  -quantize awq`:.
-00008530: 0a60 6060 6261 7368 0a6f 7065 6e6c 6c6d  .```bash.openllm
-00008540: 2073 7461 7274 2054 6865 426c 6f6b 652f   start TheBloke/
-00008550: 7a65 7068 7972 2d37 422d 616c 7068 612d  zephyr-7B-alpha-
-00008560: 4157 5120 2d2d 7175 616e 7469 7a65 2061  AWQ --quantize a
-00008570: 7771 0a60 6060 0a0a 546f 2072 756e 2069  wq.```..To run i
-00008580: 6e66 6572 656e 6365 2077 6974 6820 6073  nference with `s
-00008590: 7175 6565 7a65 6c6c 6d60 2c20 7369 6d70  queezellm`, simp
-000085a0: 6c79 2070 6173 7320 602d 2d71 7561 6e74  ly pass `--quant
-000085b0: 697a 6520 7371 7565 657a 656c 6c6d 603a  ize squeezellm`:
-000085c0: 0a0a 6060 6062 6173 680a 6f70 656e 6c6c  ..```bash.openll
-000085d0: 6d20 7374 6172 7420 7371 7565 657a 652d  m start squeeze-
-000085e0: 6169 2d6c 6162 2f73 712d 6c6c 616d 612d  ai-lab/sq-llama-
-000085f0: 322d 3762 2d77 342d 7330 202d 2d71 7561  2-7b-w4-s0 --qua
-00008600: 6e74 697a 6520 7371 7565 657a 656c 6c6d  ntize squeezellm
-00008610: 202d 2d73 6572 6961 6c69 7a61 7469 6f6e   --serialization
-00008620: 206c 6567 6163 790a 6060 600a 0a3e 205b   legacy.```..> [
-00008630: 2149 4d50 4f52 5441 4e54 5d0a 3e20 5369  !IMPORTANT].> Si
-00008640: 6e63 6520 626f 7468 2060 7371 7565 657a  nce both `squeez
-00008650: 656c 6c6d 6020 616e 6420 6061 7771 6020  ellm` and `awq` 
-00008660: 6172 6520 7765 6967 6874 2d61 7761 7265  are weight-aware
-00008670: 2071 7561 6e74 697a 6174 696f 6e20 6d65   quantization me
-00008680: 7468 6f64 732c 206d 6561 6e69 6e67 2074  thods, meaning t
-00008690: 6865 2071 7561 6e74 697a 6174 696f 6e20  he quantization 
-000086a0: 6973 2064 6f6e 6520 6475 7269 6e67 2074  is done during t
-000086b0: 7261 696e 696e 672c 2061 6c6c 2070 7265  raining, all pre
-000086c0: 2d74 7261 696e 6564 2077 6569 6768 7473  -trained weights
-000086d0: 206e 6565 6473 2074 6f20 6765 7420 7175   needs to get qu
-000086e0: 616e 7469 7a65 6420 6265 666f 7265 2069  antized before i
-000086f0: 6e66 6572 656e 6365 2074 696d 652e 204d  nference time. M
-00008700: 616b 6520 7375 7265 2074 6f20 6669 6e64  ake sure to find
-00008710: 2063 6f6d 7061 7469 626c 6520 7765 6967   compatible weig
-00008720: 6874 7320 6f6e 2048 7567 6769 6e67 4661  hts on HuggingFa
-00008730: 6365 2048 7562 2066 6f72 2079 6f75 7220  ce Hub for your 
-00008740: 6d6f 6465 6c20 6f66 2063 686f 6963 652e  model of choice.
-00008750: 0a0a 2323 20f0 9f9b a0ef b88f 2053 6572  ..## ....... Ser
-00008760: 7669 6e67 2066 696e 652d 7475 6e69 6e67  ving fine-tuning
-00008770: 206c 6179 6572 730a 0a5b 5045 4654 5d28   layers..[PEFT](
-00008780: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00008790: 6163 652e 636f 2f64 6f63 732f 7065 6674  ace.co/docs/peft
-000087a0: 2f69 6e64 6578 292c 206f 7220 5061 7261  /index), or Para
-000087b0: 6d65 7465 722d 4566 6669 6369 656e 7420  meter-Efficient 
-000087c0: 4669 6e65 2d54 756e 696e 672c 2069 7320  Fine-Tuning, is 
-000087d0: 6120 6d65 7468 6f64 6f6c 6f67 7920 6465  a methodology de
-000087e0: 7369 676e 6564 2074 6f20 6669 6e65 2d74  signed to fine-t
-000087f0: 756e 6520 7072 652d 7472 6169 6e65 6420  une pre-trained 
-00008800: 6d6f 6465 6c73 206d 6f72 6520 6566 6669  models more effi
-00008810: 6369 656e 746c 792e 2049 6e73 7465 6164  ciently. Instead
-00008820: 206f 6620 6164 6a75 7374 696e 6720 616c   of adjusting al
-00008830: 6c20 6d6f 6465 6c20 7061 7261 6d65 7465  l model paramete
-00008840: 7273 2c20 5045 4654 2066 6f63 7573 6573  rs, PEFT focuses
-00008850: 206f 6e20 7475 6e69 6e67 206f 6e6c 7920   on tuning only 
-00008860: 6120 7375 6273 6574 2c20 7265 6475 6369  a subset, reduci
-00008870: 6e67 2063 6f6d 7075 7461 7469 6f6e 616c  ng computational
-00008880: 2061 6e64 2073 746f 7261 6765 2063 6f73   and storage cos
-00008890: 7473 2e20 5b4c 6f52 415d 2868 7474 7073  ts. [LoRA](https
-000088a0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-000088b0: 6f2f 646f 6373 2f70 6566 742f 636f 6e63  o/docs/peft/conc
-000088c0: 6570 7475 616c 5f67 7569 6465 732f 6c6f  eptual_guides/lo
-000088d0: 7261 2920 284c 6f77 2d52 616e 6b20 4164  ra) (Low-Rank Ad
-000088e0: 6170 7461 7469 6f6e 2920 6973 206f 6e65  aptation) is one
-000088f0: 206f 6620 7468 6520 7465 6368 6e69 7175   of the techniqu
-00008900: 6573 2073 7570 706f 7274 6564 2062 7920  es supported by 
-00008910: 5045 4654 2e20 4974 2073 7472 6561 6d6c  PEFT. It streaml
-00008920: 696e 6573 2066 696e 652d 7475 6e69 6e67  ines fine-tuning
-00008930: 2062 7920 7573 696e 6720 6c6f 772d 7261   by using low-ra
-00008940: 6e6b 2064 6563 6f6d 706f 7369 7469 6f6e  nk decomposition
-00008950: 2074 6f20 7265 7072 6573 656e 7420 7765   to represent we
-00008960: 6967 6874 2075 7064 6174 6573 2c20 7468  ight updates, th
-00008970: 6572 6562 7920 6472 6173 7469 6361 6c6c  ereby drasticall
-00008980: 7920 7265 6475 6369 6e67 2074 6865 206e  y reducing the n
-00008990: 756d 6265 7220 6f66 2074 7261 696e 6162  umber of trainab
-000089a0: 6c65 2070 6172 616d 6574 6572 732e 0a0a  le parameters...
-000089b0: 5769 7468 204f 7065 6e4c 4c4d 2c20 796f  With OpenLLM, yo
-000089c0: 7520 6361 6e20 7461 6b65 2061 6476 616e  u can take advan
-000089d0: 7461 6765 206f 6620 7468 6520 6669 6e65  tage of the fine
-000089e0: 2d74 756e 696e 6720 6665 6174 7572 6520  -tuning feature 
-000089f0: 6279 2073 6572 7669 6e67 206d 6f64 656c  by serving model
-00008a00: 7320 7769 7468 2061 6e79 2050 4546 542d  s with any PEFT-
-00008a10: 636f 6d70 6174 6962 6c65 206c 6179 6572  compatible layer
-00008a20: 7320 7573 696e 6720 7468 6520 602d 2d61  s using the `--a
-00008a30: 6461 7074 6572 2d69 6460 206f 7074 696f  dapter-id` optio
-00008a40: 6e2e 2046 6f72 2065 7861 6d70 6c65 3a0a  n. For example:.
-00008a50: 0a60 6060 6261 7368 0a6f 7065 6e6c 6c6d  .```bash.openllm
-00008a60: 2073 7461 7274 2066 6163 6562 6f6f 6b2f   start facebook/
-00008a70: 6f70 742d 362e 3762 202d 2d61 6461 7074  opt-6.7b --adapt
-00008a80: 6572 2d69 6420 6161 726e 7068 6d2f 6f70  er-id aarnphm/op
-00008a90: 742d 362d 3762 2d71 756f 7465 733a 6465  t-6-7b-quotes:de
-00008aa0: 6661 756c 740a 6060 600a 0a4f 7065 6e4c  fault.```..OpenL
-00008ab0: 4c4d 2061 6c73 6f20 7072 6f76 6964 6573  LM also provides
-00008ac0: 2066 6c65 7869 6269 6c69 7479 2062 7920   flexibility by 
-00008ad0: 7375 7070 6f72 7469 6e67 2061 6461 7074  supporting adapt
-00008ae0: 6572 7320 6672 6f6d 2063 7573 746f 6d20  ers from custom 
-00008af0: 6669 6c65 2070 6174 6873 3a0a 0a60 6060  file paths:..```
-00008b00: 6261 7368 0a6f 7065 6e6c 6c6d 2073 7461  bash.openllm sta
-00008b10: 7274 2066 6163 6562 6f6f 6b2f 6f70 742d  rt facebook/opt-
-00008b20: 362e 3762 202d 2d61 6461 7074 6572 2d69  6.7b --adapter-i
-00008b30: 6420 2f70 6174 682f 746f 2f61 6461 7074  d /path/to/adapt
-00008b40: 6572 733a 6c6f 6361 6c5f 6164 6170 7465  ers:local_adapte
-00008b50: 720a 6060 600a 0a54 6f20 7573 6520 6d75  r.```..To use mu
-00008b60: 6c74 6970 6c65 2061 6461 7074 6572 732c  ltiple adapters,
-00008b70: 2075 7365 2074 6865 2066 6f6c 6c6f 7769   use the followi
-00008b80: 6e67 2066 6f72 6d61 743a 0a0a 6060 6062  ng format:..```b
-00008b90: 6173 680a 6f70 656e 6c6c 6d20 7374 6172  ash.openllm star
-00008ba0: 7420 6661 6365 626f 6f6b 2f6f 7074 2d36  t facebook/opt-6
-00008bb0: 2e37 6220 2d2d 6164 6170 7465 722d 6964  .7b --adapter-id
-00008bc0: 2061 6172 6e70 686d 2f6f 7074 2d36 2e37   aarnphm/opt-6.7
-00008bd0: 622d 6c6f 7261 3a64 6566 6175 6c74 202d  b-lora:default -
-00008be0: 2d61 6461 7074 6572 2d69 6420 6161 726e  -adapter-id aarn
-00008bf0: 7068 6d2f 6f70 742d 362e 3762 2d66 7265  phm/opt-6.7b-fre
-00008c00: 6e63 683a 6672 656e 6368 5f6c 6f72 610a  nch:french_lora.
-00008c10: 6060 600a 0a42 7920 6465 6661 756c 742c  ```..By default,
-00008c20: 2061 6c6c 2061 6461 7074 6572 7320 7769   all adapters wi
-00008c30: 6c6c 2062 6520 696e 6a65 6374 6564 2069  ll be injected i
-00008c40: 6e74 6f20 7468 6520 6d6f 6465 6c73 2064  nto the models d
-00008c50: 7572 696e 6720 7374 6172 7475 702e 2041  uring startup. A
-00008c60: 6461 7074 6572 7320 6361 6e20 6265 2073  dapters can be s
-00008c70: 7065 6369 6669 6564 2070 6572 2072 6571  pecified per req
-00008c80: 7565 7374 2076 6961 2060 6164 6170 7465  uest via `adapte
-00008c90: 725f 6e61 6d65 603a 0a0a 6060 6062 6173  r_name`:..```bas
-00008ca0: 680a 6375 726c 202d 5820 2750 4f53 5427  h.curl -X 'POST'
-00008cb0: 205c 0a20 2027 6874 7470 3a2f 2f6c 6f63   \.  'http://loc
-00008cc0: 616c 686f 7374 3a33 3030 302f 7631 2f67  alhost:3000/v1/g
-00008cd0: 656e 6572 6174 6527 205c 0a20 202d 4820  enerate' \.  -H 
-00008ce0: 2761 6363 6570 743a 2061 7070 6c69 6361  'accept: applica
-00008cf0: 7469 6f6e 2f6a 736f 6e27 205c 0a20 202d  tion/json' \.  -
-00008d00: 4820 2743 6f6e 7465 6e74 2d54 7970 653a  H 'Content-Type:
-00008d10: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
-00008d20: 6e27 205c 0a20 202d 6420 277b 0a20 2022  n' \.  -d '{.  "
-00008d30: 7072 6f6d 7074 223a 2022 5768 6174 2069  prompt": "What i
-00008d40: 7320 7468 6520 6d65 616e 696e 6720 6f66  s the meaning of
-00008d50: 206c 6966 653f 222c 0a20 2022 7374 6f70   life?",.  "stop
-00008d60: 223a 205b 0a20 2020 2022 7068 696c 6f73  ": [.    "philos
-00008d70: 6f70 6865 7222 0a20 205d 2c0a 2020 226c  opher".  ],.  "l
-00008d80: 6c6d 5f63 6f6e 6669 6722 3a20 7b0a 2020  lm_config": {.  
-00008d90: 2020 226d 6178 5f6e 6577 5f74 6f6b 656e    "max_new_token
-00008da0: 7322 3a20 3235 362c 0a20 2020 2022 7465  s": 256,.    "te
-00008db0: 6d70 6572 6174 7572 6522 3a20 302e 3735  mperature": 0.75
-00008dc0: 2c0a 2020 2020 2274 6f70 5f6b 223a 2031  ,.    "top_k": 1
-00008dd0: 352c 0a20 2020 2022 746f 705f 7022 3a20  5,.    "top_p": 
-00008de0: 310a 2020 7d2c 0a20 2022 6164 6170 7465  1.  },.  "adapte
-00008df0: 725f 6e61 6d65 223a 2022 6465 6661 756c  r_name": "defaul
-00008e00: 7422 0a7d 270a 6060 600a 0a54 6f20 696e  t".}'.```..To in
-00008e10: 636c 7564 6520 7468 6973 2069 6e74 6f20  clude this into 
-00008e20: 7468 6520 4265 6e74 6f2c 2079 6f75 2063  the Bento, you c
-00008e30: 616e 2073 7065 6369 6679 2074 6865 c2a0  an specify the..
-00008e40: 602d 2d61 6461 7074 6572 2d69 6460 c2a0  `--adapter-id`..
-00008e50: 6f70 7469 6f6e 2077 6865 6e20 7573 696e  option when usin
-00008e60: 6720 7468 65c2 a060 6f70 656e 6c6c 6d20  g the..`openllm 
-00008e70: 6275 696c 6460 2063 6f6d 6d61 6e64 3a0a  build` command:.
-00008e80: 0a60 6060 6261 7368 0a6f 7065 6e6c 6c6d  .```bash.openllm
-00008e90: 2062 7569 6c64 2066 6163 6562 6f6f 6b2f   build facebook/
-00008ea0: 6f70 742d 362e 3762 202d 2d61 6461 7074  opt-6.7b --adapt
-00008eb0: 6572 2d69 6420 2e2e 2e0a 6060 600a 0a49  er-id ....```..I
-00008ec0: 6620 796f 7520 7573 6520 6120 7265 6c61  f you use a rela
-00008ed0: 7469 7665 2070 6174 6820 666f 7220 602d  tive path for `-
-00008ee0: 2d61 6461 7074 6572 2d69 6460 2c20 796f  -adapter-id`, yo
-00008ef0: 7520 6e65 6564 2074 6f20 6164 6420 602d  u need to add `-
-00008f00: 2d62 7569 6c64 2d63 7478 602e 0a0a 6060  -build-ctx`...``
-00008f10: 6062 6173 680a 6f70 656e 6c6c 6d20 6275  `bash.openllm bu
-00008f20: 696c 6420 6661 6365 626f 6f6b 2f6f 7074  ild facebook/opt
-00008f30: 2d36 2e37 6220 2d2d 6164 6170 7465 722d  -6.7b --adapter-
-00008f40: 6964 202e 2f70 6174 682f 746f 2f61 6461  id ./path/to/ada
-00008f50: 7074 6572 5f69 6420 2d2d 6275 696c 642d  pter_id --build-
-00008f60: 6374 7820 2e0a 6060 600a 0a3e 205b 2149  ctx ..```..> [!I
-00008f70: 4d50 4f52 5441 4e54 5d0a 3e20 4669 6e65  MPORTANT].> Fine
-00008f80: 2d74 756e 696e 6720 7375 7070 6f72 7420  -tuning support 
-00008f90: 6973 2073 7469 6c6c 2065 7870 6572 696d  is still experim
-00008fa0: 656e 7461 6c20 616e 6420 6375 7272 656e  ental and curren
-00008fb0: 746c 7920 6f6e 6c79 2077 6f72 6b73 2077  tly only works w
-00008fc0: 6974 6820 5079 546f 7263 6820 6261 636b  ith PyTorch back
-00008fd0: 656e 642e 2076 4c4c 4d20 7375 7070 6f72  end. vLLM suppor
-00008fe0: 7420 6973 2063 6f6d 696e 6720 736f 6f6e  t is coming soon
-00008ff0: 2e0a 0a23 2320 f09f 908d 2050 7974 686f  ...## .... Pytho
-00009000: 6e20 5344 4b0a 0a45 6163 6820 4c4c 4d20  n SDK..Each LLM 
-00009010: 6361 6e20 6265 2069 6e73 7461 6e74 6961  can be instantia
-00009020: 7465 6420 7769 7468 2060 6f70 656e 6c6c  ted with `openll
-00009030: 6d2e 4c4c 4d60 3a0a 0a60 6060 7079 7468  m.LLM`:..```pyth
-00009040: 6f6e 0a69 6d70 6f72 7420 6f70 656e 6c6c  on.import openll
-00009050: 6d0a 0a6c 6c6d 203d 206f 7065 6e6c 6c6d  m..llm = openllm
-00009060: 2e4c 4c4d 2827 6d69 6372 6f73 6f66 742f  .LLM('microsoft/
-00009070: 7068 692d 3227 290a 6060 600a 0a54 6865  phi-2').```..The
-00009080: 206d 6169 6e20 696e 6665 7265 6e63 6520   main inference 
-00009090: 4150 4920 6973 2074 6865 2073 7472 6561  API is the strea
-000090a0: 6d69 6e67 2060 6765 6e65 7261 7465 5f69  ming `generate_i
-000090b0: 7465 7261 746f 7260 206d 6574 686f 643a  terator` method:
-000090c0: 0a0a 6060 6070 7974 686f 6e0a 6173 796e  ..```python.asyn
-000090d0: 6320 666f 7220 6765 6e65 7261 7469 6f6e  c for generation
-000090e0: 2069 6e20 6c6c 6d2e 6765 6e65 7261 7465   in llm.generate
-000090f0: 5f69 7465 7261 746f 7228 2757 6861 7420  _iterator('What 
-00009100: 6973 2074 6865 206d 6561 6e69 6e67 206f  is the meaning o
-00009110: 6620 6c69 6665 3f27 293a 0a20 2070 7269  f life?'):.  pri
-00009120: 6e74 2867 656e 6572 6174 696f 6e2e 6f75  nt(generation.ou
-00009130: 7470 7574 735b 305d 2e74 6578 7429 0a60  tputs[0].text).`
-00009140: 6060 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20  ``..> [!NOTE].> 
-00009150: 5468 6520 6d6f 7469 7661 7469 6f6e 2062  The motivation b
-00009160: 6568 696e 6420 6d61 6b69 6e67 2060 6c6c  ehind making `ll
-00009170: 6d2e 6765 6e65 7261 7465 5f69 7465 7261  m.generate_itera
-00009180: 746f 7260 2061 6e20 6173 796e 6320 6765  tor` an async ge
-00009190: 6e65 7261 746f 7220 6973 2074 6f20 7072  nerator is to pr
-000091a0: 6f76 6964 6520 7375 7070 6f72 7420 666f  ovide support fo
-000091b0: 7220 436f 6e74 696e 756f 7573 2062 6174  r Continuous bat
-000091c0: 6368 696e 6720 7769 7468 2076 4c4c 4d20  ching with vLLM 
-000091d0: 6261 636b 656e 642e 2042 7920 6861 7669  backend. By havi
-000091e0: 6e67 2074 6865 2061 7379 6e63 2065 6e64  ng the async end
-000091f0: 706f 696e 7473 2c20 6561 6368 2070 726f  points, each pro
-00009200: 6d70 740a 3e20 7769 6c6c 2062 6520 6164  mpt.> will be ad
-00009210: 6465 6420 636f 7272 6563 746c 7920 746f  ded correctly to
-00009220: 2074 6865 2072 6571 7565 7374 2071 7565   the request que
-00009230: 7565 2074 6f20 7072 6f63 6573 7320 7769  ue to process wi
-00009240: 7468 2076 4c4c 4d20 6261 636b 656e 642e  th vLLM backend.
-00009250: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
-00009260: 6120 5f6f 6e65 2d73 686f 745f 2060 6765  a _one-shot_ `ge
-00009270: 6e65 7261 7465 6020 6d65 7468 6f64 3a0a  nerate` method:.
-00009280: 0a60 6060 7079 7468 6f6e 0a61 7761 6974  .```python.await
-00009290: 206c 6c6d 2e67 656e 6572 6174 6528 2757   llm.generate('W
-000092a0: 6861 7420 6973 2074 6865 206d 6561 6e69  hat is the meani
-000092b0: 6e67 206f 6620 6c69 6665 3f27 290a 6060  ng of life?').``
-000092c0: 600a 0a54 6869 7320 6d65 7468 6f64 2069  `..This method i
-000092d0: 7320 6561 7379 2074 6f20 7573 6520 666f  s easy to use fo
-000092e0: 7220 6f6e 652d 7368 6f74 2067 656e 6572  r one-shot gener
-000092f0: 6174 696f 6e20 7573 6520 6361 7365 2c20  ation use case, 
-00009300: 6275 7420 6d65 7265 6c79 2073 6572 7665  but merely serve
-00009310: 6420 6173 2061 6e20 6578 616d 706c 6520  d as an example 
-00009320: 686f 7720 746f 2075 7365 2060 6c6c 6d2e  how to use `llm.
-00009330: 6765 6e65 7261 7465 5f69 7465 7261 746f  generate_iterato
-00009340: 7260 2061 7320 6974 2075 7365 7320 6067  r` as it uses `g
-00009350: 656e 6572 6174 655f 6974 6572 6174 6f72  enerate_iterator
-00009360: 6020 756e 6465 7220 7468 6520 686f 6f64  ` under the hood
-00009370: 2e0a 0a3e 205b 2149 4d50 4f52 5441 4e54  ...> [!IMPORTANT
-00009380: 5d0a 3e20 4966 2079 6f75 206e 6565 6420  ].> If you need 
-00009390: 746f 2063 616c 6c20 796f 7572 2063 6f64  to call your cod
-000093a0: 6520 696e 2061 2073 796e 6368 726f 6e6f  e in a synchrono
-000093b0: 7573 2063 6f6e 7465 7874 2c20 796f 7520  us context, you 
-000093c0: 6361 6e20 7573 6520 6061 7379 6e63 696f  can use `asyncio
-000093d0: 2e72 756e 6020 7468 6174 2077 7261 7073  .run` that wraps
-000093e0: 2061 6e20 6173 796e 6320 6675 6e63 7469   an async functi
-000093f0: 6f6e 3a0a 3e0a 3e20 6060 6070 7974 686f  on:.>.> ```pytho
-00009400: 6e0a 3e20 696d 706f 7274 2061 7379 6e63  n.> import async
-00009410: 696f 0a3e 2061 7379 6e63 2064 6566 2067  io.> async def g
-00009420: 656e 6572 6174 6528 7072 6f6d 7074 2c20  enerate(prompt, 
-00009430: 2a2a 6174 7472 7329 3a20 7265 7475 726e  **attrs): return
-00009440: 2061 7761 6974 206c 6c6d 2e67 656e 6572   await llm.gener
-00009450: 6174 6528 7072 6f6d 7074 2c20 2a2a 6174  ate(prompt, **at
-00009460: 7472 7329 0a3e 2061 7379 6e63 696f 2e72  trs).> asyncio.r
-00009470: 756e 2867 656e 6572 6174 6528 2254 6865  un(generate("The
-00009480: 206d 6561 6e69 6e67 206f 6620 6c69 6665   meaning of life
-00009490: 2069 7322 2c20 7465 6d70 6572 6174 7572   is", temperatur
-000094a0: 653d 302e 3233 2929 0a3e 2060 6060 0a0a  e=0.23)).> ```..
-000094b0: 2323 20e2 9a99 efb8 8f20 496e 7465 6772  ## ...... Integr
-000094c0: 6174 696f 6e73 0a0a 4f70 656e 4c4c 4d20  ations..OpenLLM 
-000094d0: 6973 206e 6f74 206a 7573 7420 6120 7374  is not just a st
-000094e0: 616e 6461 6c6f 6e65 2070 726f 6475 6374  andalone product
-000094f0: 3b20 6974 2773 2061 2062 7569 6c64 696e  ; it's a buildin
-00009500: 6720 626c 6f63 6b20 6465 7369 676e 6564  g block designed
-00009510: 2074 6f0a 696e 7465 6772 6174 6520 7769   to.integrate wi
-00009520: 7468 206f 7468 6572 2070 6f77 6572 6675  th other powerfu
-00009530: 6c20 746f 6f6c 7320 6561 7369 6c79 2e20  l tools easily. 
-00009540: 5765 2063 7572 7265 6e74 6c79 206f 6666  We currently off
-00009550: 6572 2069 6e74 6567 7261 7469 6f6e 2077  er integration w
-00009560: 6974 680a 5b42 656e 746f 4d4c 5d28 6874  ith.[BentoML](ht
-00009570: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00009580: 2f62 656e 746f 6d6c 2f42 656e 746f 4d4c  /bentoml/BentoML
-00009590: 292c 0a5b 4f70 656e 4149 2773 2043 6f6d  ),.[OpenAI's Com
-000095a0: 7061 7469 626c 6520 456e 6470 6f69 6e74  patible Endpoint
-000095b0: 735d 2868 7474 7073 3a2f 2f70 6c61 7466  s](https://platf
-000095c0: 6f72 6d2e 6f70 656e 6169 2e63 6f6d 2f64  orm.openai.com/d
-000095d0: 6f63 732f 6170 692d 7265 6665 7265 6e63  ocs/api-referenc
-000095e0: 652f 636f 6d70 6c65 7469 6f6e 732f 6f62  e/completions/ob
-000095f0: 6a65 6374 292c 0a5b 4c6c 616d 6149 6e64  ject),.[LlamaInd
-00009600: 6578 5d28 6874 7470 733a 2f2f 7777 772e  ex](https://www.
-00009610: 6c6c 616d 6169 6e64 6578 2e61 692f 292c  llamaindex.ai/),
-00009620: 0a5b 4c61 6e67 4368 6169 6e5d 2868 7474  .[LangChain](htt
-00009630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00009640: 6877 6368 6173 6531 372f 6c61 6e67 6368  hwchase17/langch
-00009650: 6169 6e29 2c20 616e 640a 5b54 7261 6e73  ain), and.[Trans
-00009660: 666f 726d 6572 7320 4167 656e 7473 5d28  formers Agents](
-00009670: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00009680: 6163 652e 636f 2f64 6f63 732f 7472 616e  ace.co/docs/tran
-00009690: 7366 6f72 6d65 7273 2f74 7261 6e73 666f  sformers/transfo
-000096a0: 726d 6572 735f 6167 656e 7473 292e 0a0a  rmers_agents)...
-000096b0: 2323 2320 4f70 656e 4149 2043 6f6d 7061  ### OpenAI Compa
-000096c0: 7469 626c 6520 456e 6470 6f69 6e74 730a  tible Endpoints.
-000096d0: 0a4f 7065 6e4c 4c4d 2053 6572 7665 7220  .OpenLLM Server 
-000096e0: 6361 6e20 6265 2075 7365 6420 6173 2061  can be used as a
-000096f0: 2064 726f 702d 696e 2072 6570 6c61 6365   drop-in replace
-00009700: 6d65 6e74 2066 6f72 204f 7065 6e41 4927  ment for OpenAI'
-00009710: 7320 4150 492e 2053 696d 706c 790a 7370  s API. Simply.sp
-00009720: 6563 6966 7920 7468 6520 6261 7365 5f75  ecify the base_u
-00009730: 726c 2074 6f20 606c 6c6d 2d65 6e64 706f  rl to `llm-endpo
-00009740: 696e 742f 7631 6020 616e 6420 796f 7520  int/v1` and you 
-00009750: 6172 6520 676f 6f64 2074 6f20 676f 3a0a  are good to go:.
-00009760: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00009770: 7420 6f70 656e 6169 0a0a 636c 6965 6e74  t openai..client
-00009780: 203d 206f 7065 6e61 692e 4f70 656e 4149   = openai.OpenAI
-00009790: 280a 2020 6261 7365 5f75 726c 3d27 6874  (.  base_url='ht
-000097a0: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
-000097b0: 3030 302f 7631 272c 2061 7069 5f6b 6579  000/v1', api_key
-000097c0: 3d27 6e61 270a 2920 2023 2048 6572 6520  ='na'.)  # Here 
-000097d0: 7468 6520 7365 7276 6572 2069 7320 7275  the server is ru
-000097e0: 6e6e 696e 6720 6f6e 206c 6f63 616c 686f  nning on localho
-000097f0: 7374 3a33 3030 300a 0a63 6f6d 706c 6574  st:3000..complet
-00009800: 696f 6e73 203d 2063 6c69 656e 742e 636f  ions = client.co
-00009810: 6d70 6c65 7469 6f6e 732e 6372 6561 7465  mpletions.create
-00009820: 280a 2020 7072 6f6d 7074 3d27 5772 6974  (.  prompt='Writ
-00009830: 6520 6d65 2061 2074 6167 206c 696e 6520  e me a tag line 
-00009840: 666f 7220 616e 2069 6365 2063 7265 616d  for an ice cream
-00009850: 2073 686f 702e 272c 206d 6f64 656c 3d6d   shop.', model=m
-00009860: 6f64 656c 2c20 6d61 785f 746f 6b65 6e73  odel, max_tokens
-00009870: 3d36 342c 2073 7472 6561 6d3d 7374 7265  =64, stream=stre
-00009880: 616d 0a29 0a60 6060 0a0a 5468 6520 636f  am.).```..The co
-00009890: 6d70 6174 6962 6c65 2065 6e64 706f 696e  mpatible endpoin
-000098a0: 7473 2073 7570 706f 7274 7320 602f 636f  ts supports `/co
-000098b0: 6d70 6c65 7469 6f6e 7360 2c20 602f 6368  mpletions`, `/ch
-000098c0: 6174 2f63 6f6d 706c 6574 696f 6e73 602c  at/completions`,
-000098d0: 2061 6e64 2060 2f6d 6f64 656c 7360 0a0a   and `/models`..
-000098e0: 3e20 5b21 4e4f 5445 5d0a 3e20 596f 7520  > [!NOTE].> You 
-000098f0: 6361 6e20 6669 6e64 206f 7574 204f 7065  can find out Ope
-00009900: 6e41 4920 6578 616d 706c 6520 636c 6965  nAI example clie
-00009910: 6e74 7320 756e 6465 7220 7468 650a 3e20  nts under the.> 
-00009920: 5b65 7861 6d70 6c65 735d 2868 7474 7073  [examples](https
-00009930: 3a2f 2f67 6974 6875 622e 636f 6d2f 6265  ://github.com/be
-00009940: 6e74 6f6d 6c2f 4f70 656e 4c4c 4d2f 7472  ntoml/OpenLLM/tr
-00009950: 6565 2f6d 6169 6e2f 6578 616d 706c 6573  ee/main/examples
-00009960: 2920 666f 6c64 6572 2e0a 0a23 2323 2042  ) folder...### B
-00009970: 656e 746f 4d4c 0a0a 4f70 656e 4c4c 4d20  entoML..OpenLLM 
-00009980: 4c4c 4d20 6361 6e20 6265 2069 6e74 6567  LLM can be integ
-00009990: 7261 7465 6420 6173 2061 0a5b 5275 6e6e  rated as a.[Runn
-000099a0: 6572 5d28 6874 7470 733a 2f2f 646f 6373  er](https://docs
-000099b0: 2e62 656e 746f 6d6c 2e63 6f6d 2f65 6e2f  .bentoml.com/en/
-000099c0: 6c61 7465 7374 2f63 6f6e 6365 7074 732f  latest/concepts/
-000099d0: 7275 6e6e 6572 2e68 746d 6c29 2069 6e20  runner.html) in 
-000099e0: 796f 7572 0a42 656e 746f 4d4c 2073 6572  your.BentoML ser
-000099f0: 7669 6365 2e20 5369 6d70 6c79 2063 616c  vice. Simply cal
-00009a00: 6c20 6061 7761 6974 206c 6c6d 2e67 656e  l `await llm.gen
-00009a10: 6572 6174 6560 2074 6f20 6765 6e65 7261  erate` to genera
-00009a20: 7465 2074 6578 742e 204e 6f74 6520 7468  te text. Note th
-00009a30: 6174 0a60 6c6c 6d2e 6765 6e65 7261 7465  at.`llm.generate
-00009a40: 6020 7573 6573 2060 7275 6e6e 6572 6020  ` uses `runner` 
-00009a50: 756e 6465 7220 7468 6520 686f 6f64 3a0a  under the hood:.
-00009a60: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
-00009a70: 7420 6265 6e74 6f6d 6c0a 696d 706f 7274  t bentoml.import
-00009a80: 206f 7065 6e6c 6c6d 0a0a 6c6c 6d20 3d20   openllm..llm = 
-00009a90: 6f70 656e 6c6c 6d2e 4c4c 4d28 276d 6963  openllm.LLM('mic
-00009aa0: 726f 736f 6674 2f70 6869 2d32 2729 0a0a  rosoft/phi-2')..
-00009ab0: 7376 6320 3d20 6265 6e74 6f6d 6c2e 5365  svc = bentoml.Se
-00009ac0: 7276 6963 6528 6e61 6d65 3d27 6c6c 6d2d  rvice(name='llm-
-00009ad0: 7068 692d 7365 7276 6963 6527 2c20 7275  phi-service', ru
-00009ae0: 6e6e 6572 733d 5b6c 6c6d 2e72 756e 6e65  nners=[llm.runne
-00009af0: 725d 290a 0a0a 4073 7663 2e61 7069 2869  r])...@svc.api(i
-00009b00: 6e70 7574 3d62 656e 746f 6d6c 2e69 6f2e  nput=bentoml.io.
-00009b10: 5465 7874 2829 2c20 6f75 7470 7574 3d62  Text(), output=b
-00009b20: 656e 746f 6d6c 2e69 6f2e 5465 7874 2829  entoml.io.Text()
-00009b30: 290a 6173 796e 6320 6465 6620 7072 6f6d  ).async def prom
-00009b40: 7074 2869 6e70 7574 5f74 6578 743a 2073  pt(input_text: s
-00009b50: 7472 2920 2d3e 2073 7472 3a0a 2020 6765  tr) -> str:.  ge
-00009b60: 6e65 7261 7469 6f6e 203d 2061 7761 6974  neration = await
-00009b70: 206c 6c6d 2e67 656e 6572 6174 6528 696e   llm.generate(in
-00009b80: 7075 745f 7465 7874 290a 2020 7265 7475  put_text).  retu
-00009b90: 726e 2067 656e 6572 6174 696f 6e2e 6f75  rn generation.ou
-00009ba0: 7470 7574 735b 305d 2e74 6578 740a 6060  tputs[0].text.``
-00009bb0: 600a 0a23 2323 205b 4c6c 616d 6149 6e64  `..### [LlamaInd
-00009bc0: 6578 5d28 6874 7470 733a 2f2f 646f 6373  ex](https://docs
-00009bd0: 2e6c 6c61 6d61 696e 6465 782e 6169 2f65  .llamaindex.ai/e
-00009be0: 6e2f 7374 6162 6c65 2f6d 6f64 756c 655f  n/stable/module_
-00009bf0: 6775 6964 6573 2f6d 6f64 656c 732f 6c6c  guides/models/ll
-00009c00: 6d73 2f6d 6f64 756c 6573 2e68 746d 6c23  ms/modules.html#
-00009c10: 6f70 656e 6c6c 6d29 0a0a 546f 2073 7461  openllm)..To sta
-00009c20: 7274 2061 206c 6f63 616c 204c 4c4d 2077  rt a local LLM w
-00009c30: 6974 6820 606c 6c61 6d61 5f69 6e64 6578  ith `llama_index
-00009c40: 602c 2073 696d 706c 7920 7573 6520 606c  `, simply use `l
-00009c50: 6c61 6d61 5f69 6e64 6578 2e6c 6c6d 732e  lama_index.llms.
-00009c60: 6f70 656e 6c6c 6d2e 4f70 656e 4c4c 4d60  openllm.OpenLLM`
-00009c70: 3a0a 0a60 6060 7079 7468 6f6e 0a69 6d70  :..```python.imp
-00009c80: 6f72 7420 6173 796e 6369 6f0a 6672 6f6d  ort asyncio.from
-00009c90: 206c 6c61 6d61 5f69 6e64 6578 2e6c 6c6d   llama_index.llm
-00009ca0: 732e 6f70 656e 6c6c 6d20 696d 706f 7274  s.openllm import
-00009cb0: 204f 7065 6e4c 4c4d 0a0a 6c6c 6d20 3d20   OpenLLM..llm = 
-00009cc0: 4f70 656e 4c4c 4d28 2748 7567 6769 6e67  OpenLLM('Hugging
-00009cd0: 4661 6365 4834 2f7a 6570 6879 722d 3762  FaceH4/zephyr-7b
-00009ce0: 2d61 6c70 6861 2729 0a0a 6c6c 6d2e 636f  -alpha')..llm.co
-00009cf0: 6d70 6c65 7465 2827 5468 6520 6d65 616e  mplete('The mean
-00009d00: 696e 6720 6f66 206c 6966 6520 6973 2729  ing of life is')
-00009d10: 0a0a 0a61 7379 6e63 2064 6566 206d 6169  ...async def mai
-00009d20: 6e28 7072 6f6d 7074 2c20 2a2a 6b77 6172  n(prompt, **kwar
-00009d30: 6773 293a 0a20 2061 7379 6e63 2066 6f72  gs):.  async for
-00009d40: 2069 7420 696e 206c 6c6d 2e61 7374 7265   it in llm.astre
-00009d50: 616d 5f63 6861 7428 7072 6f6d 7074 2c20  am_chat(prompt, 
-00009d60: 2a2a 6b77 6172 6773 293a 0a20 2020 2070  **kwargs):.    p
-00009d70: 7269 6e74 2869 7429 0a0a 0a61 7379 6e63  rint(it)...async
-00009d80: 696f 2e72 756e 286d 6169 6e28 2754 6865  io.run(main('The
-00009d90: 2074 696d 6520 6174 2053 616e 2046 7261   time at San Fra
-00009da0: 6e63 6973 636f 2069 7327 2929 0a60 6060  ncisco is')).```
-00009db0: 0a0a 4966 2074 6865 7265 2069 7320 6120  ..If there is a 
-00009dc0: 7265 6d6f 7465 204c 4c4d 2053 6572 7665  remote LLM Serve
-00009dd0: 7220 7275 6e6e 696e 6720 656c 7365 7768  r running elsewh
-00009de0: 6572 652c 2074 6865 6e20 796f 7520 6361  ere, then you ca
-00009df0: 6e20 7573 6520 606c 6c61 6d61 5f69 6e64  n use `llama_ind
-00009e00: 6578 2e6c 6c6d 732e 6f70 656e 6c6c 6d2e  ex.llms.openllm.
-00009e10: 4f70 656e 4c4c 4d41 5049 603a 0a0a 6060  OpenLLMAPI`:..``
-00009e20: 6070 7974 686f 6e0a 6672 6f6d 206c 6c61  `python.from lla
-00009e30: 6d61 5f69 6e64 6578 2e6c 6c6d 732e 6f70  ma_index.llms.op
-00009e40: 656e 6c6c 6d20 696d 706f 7274 204f 7065  enllm import Ope
-00009e50: 6e4c 4c4d 4150 490a 6060 600a 0a3e 205b  nLLMAPI.```..> [
-00009e60: 214e 4f54 455d 0a3e 2041 6c6c 2073 796e  !NOTE].> All syn
-00009e70: 6368 726f 6e6f 7573 2061 6e64 2061 7379  chronous and asy
-00009e80: 6e63 6872 6f6e 6f75 7320 4150 4920 6672  nchronous API fr
-00009e90: 6f6d 2060 6c6c 616d 615f 696e 6465 782e  om `llama_index.
-00009ea0: 6c6c 6d73 2e4c 4c4d 6020 6172 6520 7375  llms.LLM` are su
-00009eb0: 7070 6f72 7465 642e 0a0a 2323 2320 5b4c  pported...### [L
-00009ec0: 616e 6743 6861 696e 5d28 6874 7470 733a  angChain](https:
-00009ed0: 2f2f 7079 7468 6f6e 2e6c 616e 6763 6861  //python.langcha
-00009ee0: 696e 2e63 6f6d 2f64 6f63 732f 6563 6f73  in.com/docs/ecos
-00009ef0: 7973 7465 6d2f 696e 7465 6772 6174 696f  ystem/integratio
-00009f00: 6e73 2f6f 7065 6e6c 6c6d 290a 0a54 6f20  ns/openllm)..To 
-00009f10: 7175 6963 6b6c 7920 7374 6172 7420 6120  quickly start a 
-00009f20: 6c6f 6361 6c20 4c4c 4d20 7769 7468 2060  local LLM with `
-00009f30: 6c61 6e67 6368 6169 6e60 2c20 7369 6d70  langchain`, simp
-00009f40: 6c79 2064 6f20 7468 6520 666f 6c6c 6f77  ly do the follow
-00009f50: 696e 673a 0a0a 6060 6070 7974 686f 6e0a  ing:..```python.
-00009f60: 6672 6f6d 206c 616e 6763 6861 696e 2e6c  from langchain.l
-00009f70: 6c6d 7320 696d 706f 7274 204f 7065 6e4c  lms import OpenL
-00009f80: 4c4d 0a0a 6c6c 6d20 3d20 4f70 656e 4c4c  LM..llm = OpenLL
-00009f90: 4d28 6d6f 6465 6c5f 6e61 6d65 3d27 6c6c  M(model_name='ll
-00009fa0: 616d 6127 2c20 6d6f 6465 6c5f 6964 3d27  ama', model_id='
-00009fb0: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
-00009fc0: 2d32 2d37 622d 6866 2729 0a0a 6c6c 6d28  -2-7b-hf')..llm(
-00009fd0: 2757 6861 7420 6973 2074 6865 2064 6966  'What is the dif
-00009fe0: 6665 7265 6e63 6520 6265 7477 6565 6e20  ference between 
-00009ff0: 6120 6475 636b 2061 6e64 2061 2067 6f6f  a duck and a goo
-0000a000: 7365 3f20 416e 6420 7768 7920 7468 6572  se? And why ther
-0000a010: 6520 6172 6520 736f 206d 616e 7920 476f  e are so many Go
-0000a020: 6f73 6520 696e 2043 616e 6164 613f 2729  ose in Canada?')
-0000a030: 0a60 6060 0a0a 3e20 5b21 494d 504f 5254  .```..> [!IMPORT
-0000a040: 414e 545d 0a3e 2042 7920 6465 6661 756c  ANT].> By defaul
-0000a050: 742c 204f 7065 6e4c 4c4d 2075 7365 2060  t, OpenLLM use `
-0000a060: 7361 6665 7465 6e73 6f72 7360 2066 6f72  safetensors` for
-0000a070: 6d61 7420 666f 7220 7361 7669 6e67 206d  mat for saving m
-0000a080: 6f64 656c 732e 0a3e 2049 6620 7468 6520  odels..> If the 
-0000a090: 6d6f 6465 6c20 646f 6573 6e27 7420 7375  model doesn't su
-0000a0a0: 7070 6f72 7420 7361 6665 7465 6e73 6f72  pport safetensor
-0000a0b0: 732c 206d 616b 6520 7375 7265 2074 6f20  s, make sure to 
-0000a0c0: 7061 7373 0a3e 2060 7365 7269 616c 6973  pass.> `serialis
-0000a0d0: 6174 696f 6e3d 226c 6567 6163 7922 6020  ation="legacy"` 
-0000a0e0: 746f 2075 7365 2074 6865 206c 6567 6163  to use the legac
-0000a0f0: 7920 5079 546f 7263 6820 6269 6e20 666f  y PyTorch bin fo
-0000a100: 726d 6174 2e0a 0a60 6c61 6e67 6368 6169  rmat...`langchai
-0000a110: 6e2e 6c6c 6d73 2e4f 7065 6e4c 4c4d 6020  n.llms.OpenLLM` 
-0000a120: 6861 7320 7468 6520 6361 7061 6269 6c69  has the capabili
-0000a130: 7479 2074 6f20 696e 7465 7261 6374 2077  ty to interact w
-0000a140: 6974 6820 7265 6d6f 7465 204f 7065 6e4c  ith remote OpenL
-0000a150: 4c4d 0a53 6572 7665 722e 2047 6976 656e  LM.Server. Given
-0000a160: 2074 6865 7265 2069 7320 616e 204f 7065   there is an Ope
-0000a170: 6e4c 4c4d 2073 6572 7665 7220 6465 706c  nLLM server depl
-0000a180: 6f79 6564 2065 6c73 6577 6865 7265 2c20  oyed elsewhere, 
-0000a190: 796f 7520 6361 6e20 636f 6e6e 6563 7420  you can connect 
-0000a1a0: 746f 0a69 7420 6279 2073 7065 6369 6679  to.it by specify
-0000a1b0: 696e 6720 6974 7320 5552 4c3a 0a0a 6060  ing its URL:..``
-0000a1c0: 6070 7974 686f 6e0a 6672 6f6d 206c 616e  `python.from lan
-0000a1d0: 6763 6861 696e 2e6c 6c6d 7320 696d 706f  gchain.llms impo
-0000a1e0: 7274 204f 7065 6e4c 4c4d 0a0a 6c6c 6d20  rt OpenLLM..llm 
-0000a1f0: 3d20 4f70 656e 4c4c 4d28 7365 7276 6572  = OpenLLM(server
-0000a200: 5f75 726c 3d27 6874 7470 3a2f 2f34 342e  _url='http://44.
-0000a210: 3233 2e31 3233 2e31 3a33 3030 3027 2c20  23.123.1:3000', 
-0000a220: 7365 7276 6572 5f74 7970 653d 2768 7474  server_type='htt
-0000a230: 7027 290a 6c6c 6d28 2757 6861 7420 6973  p').llm('What is
-0000a240: 2074 6865 2064 6966 6665 7265 6e63 6520   the difference 
-0000a250: 6265 7477 6565 6e20 6120 6475 636b 2061  between a duck a
-0000a260: 6e64 2061 2067 6f6f 7365 3f20 416e 6420  nd a goose? And 
-0000a270: 7768 7920 7468 6572 6520 6172 6520 736f  why there are so
-0000a280: 206d 616e 7920 476f 6f73 6520 696e 2043   many Goose in C
-0000a290: 616e 6164 613f 2729 0a60 6060 0a0a 546f  anada?').```..To
-0000a2a0: 2069 6e74 6567 7261 7465 2061 204c 616e   integrate a Lan
-0000a2b0: 6743 6861 696e 2061 6765 6e74 2077 6974  gChain agent wit
-0000a2c0: 6820 4265 6e74 6f4d 4c2c 2079 6f75 2063  h BentoML, you c
-0000a2d0: 616e 2064 6f20 7468 6520 666f 6c6c 6f77  an do the follow
-0000a2e0: 696e 673a 0a0a 6060 6070 7974 686f 6e0a  ing:..```python.
-0000a2f0: 6c6c 6d20 3d20 4f70 656e 4c4c 4d28 6d6f  llm = OpenLLM(mo
-0000a300: 6465 6c5f 6964 3d27 676f 6f67 6c65 2f66  del_id='google/f
-0000a310: 6c61 6e2d 7435 2d6c 6172 6765 272c 2065  lan-t5-large', e
-0000a320: 6d62 6564 6465 643d 4661 6c73 652c 2073  mbedded=False, s
-0000a330: 6572 6961 6c69 7361 7469 6f6e 3d27 6c65  erialisation='le
-0000a340: 6761 6379 2729 0a74 6f6f 6c73 203d 206c  gacy').tools = l
-0000a350: 6f61 645f 746f 6f6c 7328 5b27 7365 7270  oad_tools(['serp
-0000a360: 6170 6927 2c20 276c 6c6d 2d6d 6174 6827  api', 'llm-math'
-0000a370: 5d2c 206c 6c6d 3d6c 6c6d 290a 6167 656e  ], llm=llm).agen
-0000a380: 7420 3d20 696e 6974 6961 6c69 7a65 5f61  t = initialize_a
-0000a390: 6765 6e74 2874 6f6f 6c73 2c20 6c6c 6d2c  gent(tools, llm,
-0000a3a0: 2061 6765 6e74 3d41 6765 6e74 5479 7065   agent=AgentType
-0000a3b0: 2e5a 4552 4f5f 5348 4f54 5f52 4541 4354  .ZERO_SHOT_REACT
-0000a3c0: 5f44 4553 4352 4950 5449 4f4e 290a 7376  _DESCRIPTION).sv
-0000a3d0: 6320 3d20 6265 6e74 6f6d 6c2e 5365 7276  c = bentoml.Serv
-0000a3e0: 6963 6528 276c 616e 6763 6861 696e 2d6f  ice('langchain-o
-0000a3f0: 7065 6e6c 6c6d 272c 2072 756e 6e65 7273  penllm', runners
-0000a400: 3d5b 6c6c 6d2e 7275 6e6e 6572 5d29 0a0a  =[llm.runner])..
-0000a410: 0a40 7376 632e 6170 6928 696e 7075 743d  .@svc.api(input=
-0000a420: 5465 7874 2829 2c20 6f75 7470 7574 3d54  Text(), output=T
-0000a430: 6578 7428 2929 0a64 6566 2063 6861 7428  ext()).def chat(
-0000a440: 696e 7075 745f 7465 7874 3a20 7374 7229  input_text: str)
-0000a450: 3a0a 2020 7265 7475 726e 2061 6765 6e74  :.  return agent
-0000a460: 2e72 756e 2869 6e70 7574 5f74 6578 7429  .run(input_text)
-0000a470: 0a60 6060 0a0a 3e20 5b21 4e4f 5445 5d0a  .```..> [!NOTE].
-0000a480: 3e20 596f 7520 6361 6e20 6669 6e64 206f  > You can find o
-0000a490: 7574 206d 6f72 6520 6578 616d 706c 6573  ut more examples
-0000a4a0: 2075 6e64 6572 2074 6865 0a3e 205b 6578   under the.> [ex
-0000a4b0: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
-0000a4c0: 6769 7468 7562 2e63 6f6d 2f62 656e 746f  github.com/bento
-0000a4d0: 6d6c 2f4f 7065 6e4c 4c4d 2f74 7265 652f  ml/OpenLLM/tree/
-0000a4e0: 6d61 696e 2f65 7861 6d70 6c65 7329 2066  main/examples) f
-0000a4f0: 6f6c 6465 722e 0a0a 2323 2320 5472 616e  older...### Tran
-0000a500: 7366 6f72 6d65 7273 2041 6765 6e74 730a  sformers Agents.
-0000a510: 0a4f 7065 6e4c 4c4d 2073 6561 6d6c 6573  .OpenLLM seamles
-0000a520: 736c 7920 696e 7465 6772 6174 6573 2077  sly integrates w
-0000a530: 6974 680a 5b54 7261 6e73 666f 726d 6572  ith.[Transformer
-0000a540: 7320 4167 656e 7473 5d28 6874 7470 733a  s Agents](https:
-0000a550: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-0000a560: 2f64 6f63 732f 7472 616e 7366 6f72 6d65  /docs/transforme
-0000a570: 7273 2f74 7261 6e73 666f 726d 6572 735f  rs/transformers_
-0000a580: 6167 656e 7473 292e 0a0a 3e20 5b21 5741  agents)...> [!WA
-0000a590: 524e 494e 475d 0a3e 2054 6865 2054 7261  RNING].> The Tra
-0000a5a0: 6e73 666f 726d 6572 7320 4167 656e 7420  nsformers Agent 
-0000a5b0: 6973 2073 7469 6c6c 2061 7420 616e 2065  is still at an e
-0000a5c0: 7870 6572 696d 656e 7461 6c20 7374 6167  xperimental stag
-0000a5d0: 652e 2049 7420 6973 0a3e 2072 6563 6f6d  e. It is.> recom
-0000a5e0: 6d65 6e64 6564 2074 6f20 696e 7374 616c  mended to instal
-0000a5f0: 6c20 4f70 656e 4c4c 4d20 7769 7468 2060  l OpenLLM with `
-0000a600: 7069 7020 696e 7374 616c 6c20 2d72 206e  pip install -r n
-0000a610: 6967 6874 6c79 2d72 6571 7569 7265 6d65  ightly-requireme
-0000a620: 6e74 732e 7478 7460 0a3e 2074 6f20 6765  nts.txt`.> to ge
-0000a630: 7420 7468 6520 6c61 7465 7374 2041 5049  t the latest API
-0000a640: 2075 7064 6174 6520 666f 7220 4875 6767   update for Hugg
-0000a650: 696e 6746 6163 6520 6167 656e 742e 0a0a  ingFace agent...
-0000a660: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-0000a670: 2074 7261 6e73 666f 726d 6572 730a 0a61   transformers..a
-0000a680: 6765 6e74 203d 2074 7261 6e73 666f 726d  gent = transform
-0000a690: 6572 732e 4866 4167 656e 7428 2768 7474  ers.HfAgent('htt
-0000a6a0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-0000a6b0: 3030 2f68 662f 6167 656e 7427 2920 2023  00/hf/agent')  #
-0000a6c0: 2055 524c 2074 6861 7420 7275 6e73 2074   URL that runs t
-0000a6d0: 6865 204f 7065 6e4c 4c4d 2073 6572 7665  he OpenLLM serve
-0000a6e0: 720a 0a61 6765 6e74 2e72 756e 2827 4973  r..agent.run('Is
-0000a6f0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2060   the following `
-0000a700: 7465 7874 6020 706f 7369 7469 7665 206f  text` positive o
-0000a710: 7220 6e65 6761 7469 7665 3f27 2c20 7465  r negative?', te
-0000a720: 7874 3d22 4920 646f 6e27 7420 6c69 6b65  xt="I don't like
-0000a730: 2068 6f77 2074 6869 7320 6d6f 6465 6c73   how this models
-0000a740: 2069 7320 6765 6e65 7261 7465 2069 6e70   is generate inp
-0000a750: 7574 7322 290a 6060 600a 0a3c 212d 2d20  uts").```..<!-- 
-0000a760: 6861 7463 682d 6661 6e63 792d 7079 7069  hatch-fancy-pypi
-0000a770: 2d72 6561 646d 6520 696e 7465 7269 6d20  -readme interim 
-0000a780: 7374 6f70 202d 2d3e 0a0a 215b 4769 6620  stop -->..![Gif 
-0000a790: 7368 6f77 696e 6720 4167 656e 7420 696e  showing Agent in
-0000a7a0: 7465 6772 6174 696f 6e5d 282f 2e67 6974  tegration](/.git
-0000a7b0: 6875 622f 6173 7365 7473 2f61 6765 6e74  hub/assets/agent
-0000a7c0: 2e67 6966 290a 0a3c 6272 2f3e 0a0a 3c21  .gif)..<br/>..<!
-0000a7d0: 2d2d 2068 6174 6368 2d66 616e 6379 2d70  -- hatch-fancy-p
-0000a7e0: 7970 692d 7265 6164 6d65 206d 6574 6120  ypi-readme meta 
-0000a7f0: 7374 6172 7420 2d2d 3e0a 0a23 2320 f09f  start -->..## ..
-0000a800: 9a80 2044 6570 6c6f 7969 6e67 206d 6f64  .. Deploying mod
-0000a810: 656c 7320 746f 2070 726f 6475 6374 696f  els to productio
-0000a820: 6e0a 0a54 6865 7265 2061 7265 2073 6576  n..There are sev
-0000a830: 6572 616c 2077 6179 7320 746f 2064 6570  eral ways to dep
-0000a840: 6c6f 7920 796f 7572 204c 4c4d 733a 0a0a  loy your LLMs:..
-0000a850: 2323 2320 f09f 90b3 2044 6f63 6b65 7220  ### .... Docker 
-0000a860: 636f 6e74 6169 6e65 720a 0a31 2e20 2a2a  container..1. **
-0000a870: 4275 696c 6469 6e67 2061 2042 656e 746f  Building a Bento
-0000a880: 2a2a 3a20 5769 7468 204f 7065 6e4c 4c4d  **: With OpenLLM
-0000a890: 2c20 796f 7520 6361 6e20 6561 7369 6c79  , you can easily
-0000a8a0: 2062 7569 6c64 2061 2042 656e 746f 2066   build a Bento f
-0000a8b0: 6f72 2061 0a20 2020 7370 6563 6966 6963  or a.   specific
-0000a8c0: 206d 6f64 656c 2c20 6c69 6b65 2060 6d69   model, like `mi
-0000a8d0: 7374 7261 6c61 692f 4d69 7374 7261 6c2d  stralai/Mistral-
-0000a8e0: 3742 2d49 6e73 7472 7563 742d 7630 2e31  7B-Instruct-v0.1
-0000a8f0: 602c 2075 7369 6e67 2074 6865 2060 6275  `, using the `bu
-0000a900: 696c 6460 2063 6f6d 6d61 6e64 2e3a 0a0a  ild` command.:..
-0000a910: 2020 2060 6060 6261 7368 0a20 2020 6f70     ```bash.   op
-0000a920: 656e 6c6c 6d20 6275 696c 6420 6d69 7374  enllm build mist
-0000a930: 7261 6c61 692f 4d69 7374 7261 6c2d 3742  ralai/Mistral-7B
-0000a940: 2d49 6e73 7472 7563 742d 7630 2e31 0a20  -Instruct-v0.1. 
-0000a950: 2020 6060 600a 0a20 2020 410a 2020 205b    ```..   A.   [
-0000a960: 4265 6e74 6f5d 2868 7474 7073 3a2f 2f64  Bento](https://d
-0000a970: 6f63 732e 6265 6e74 6f6d 6c2e 636f 6d2f  ocs.bentoml.com/
-0000a980: 656e 2f6c 6174 6573 742f 636f 6e63 6570  en/latest/concep
-0000a990: 7473 2f62 656e 746f 2e68 746d 6c23 7768  ts/bento.html#wh
-0000a9a0: 6174 2d69 732d 612d 6265 6e74 6f29 2c0a  at-is-a-bento),.
-0000a9b0: 2020 2069 6e20 4265 6e74 6f4d 4c2c 2069     in BentoML, i
-0000a9c0: 7320 7468 6520 756e 6974 206f 6620 6469  s the unit of di
-0000a9d0: 7374 7269 6275 7469 6f6e 2e20 4974 2070  stribution. It p
-0000a9e0: 6163 6b61 6765 7320 796f 7572 2070 726f  ackages your pro
-0000a9f0: 6772 616d 2773 2073 6f75 7263 650a 2020  gram's source.  
-0000aa00: 2063 6f64 652c 206d 6f64 656c 732c 2066   code, models, f
-0000aa10: 696c 6573 2c20 6172 7465 6661 6374 732c  iles, artefacts,
-0000aa20: 2061 6e64 2064 6570 656e 6465 6e63 6965   and dependencie
-0000aa30: 732e 0a0a 322e 202a 2a43 6f6e 7461 696e  s...2. **Contain
-0000aa40: 6572 697a 6520 796f 7572 2042 656e 746f  erize your Bento
-0000aa50: 2a2a 0a0a 2020 2060 6060 6261 7368 0a20  **..   ```bash. 
-0000aa60: 2020 6265 6e74 6f6d 6c20 636f 6e74 6169    bentoml contai
-0000aa70: 6e65 7269 7a65 203c 6e61 6d65 3a76 6572  nerize <name:ver
-0000aa80: 7369 6f6e 3e0a 2020 2060 6060 0a0a 2020  sion>.   ```..  
-0000aa90: 2054 6869 7320 6765 6e65 7261 7465 7320   This generates 
-0000aaa0: 6120 4f43 492d 636f 6d70 6174 6962 6c65  a OCI-compatible
-0000aab0: 2064 6f63 6b65 7220 696d 6167 6520 7468   docker image th
-0000aac0: 6174 2063 616e 2062 6520 6465 706c 6f79  at can be deploy
-0000aad0: 6564 2061 6e79 7768 6572 650a 2020 2064  ed anywhere.   d
-0000aae0: 6f63 6b65 7220 7275 6e73 2e20 466f 7220  ocker runs. For 
-0000aaf0: 6265 7374 2073 6361 6c61 6269 6c69 7479  best scalability
-0000ab00: 2061 6e64 2072 656c 6961 6269 6c69 7479   and reliability
-0000ab10: 206f 6620 796f 7572 204c 4c4d 2073 6572   of your LLM ser
-0000ab20: 7669 6365 2069 6e0a 2020 2070 726f 6475  vice in.   produ
-0000ab30: 6374 696f 6e2c 2077 6520 7265 636f 6d6d  ction, we recomm
-0000ab40: 656e 6420 6465 706c 6f79 2077 6974 6820  end deploy with 
-0000ab50: 4265 6e74 6f43 6c6f 7564 e380 820a 0a23  BentoCloud.....#
-0000ab60: 2323 20e2 9881 efb8 8f20 4265 6e74 6f43  ## ...... BentoC
-0000ab70: 6c6f 7564 0a0a 4465 706c 6f79 204f 7065  loud..Deploy Ope
-0000ab80: 6e4c 4c4d 2077 6974 6820 5b42 656e 746f  nLLM with [Bento
-0000ab90: 436c 6f75 645d 2868 7474 7073 3a2f 2f77  Cloud](https://w
-0000aba0: 7777 2e62 656e 746f 6d6c 2e63 6f6d 2f62  ww.bentoml.com/b
-0000abb0: 656e 746f 2d63 6c6f 7564 2f29 2c20 7468  ento-cloud/), th
-0000abc0: 650a 7365 7276 6572 6c65 7373 2063 6c6f  e.serverless clo
-0000abd0: 7564 2066 6f72 2073 6869 7070 696e 6720  ud for shipping 
-0000abe0: 616e 6420 7363 616c 696e 6720 4149 2061  and scaling AI a
-0000abf0: 7070 6c69 6361 7469 6f6e 732e 0a0a 312e  pplications...1.
-0000ac00: 202a 2a43 7265 6174 6520 6120 4265 6e74   **Create a Bent
-0000ac10: 6f43 6c6f 7564 2061 6363 6f75 6e74 3a2a  oCloud account:*
-0000ac20: 2a20 5b73 6967 6e20 7570 2068 6572 655d  * [sign up here]
-0000ac30: 2868 7474 7073 3a2f 2f62 656e 746f 6d6c  (https://bentoml
-0000ac40: 2e63 6f6d 2f63 6c6f 7564 290a 2020 2066  .com/cloud).   f
-0000ac50: 6f72 2065 6172 6c79 2061 6363 6573 730a  or early access.
-0000ac60: 0a32 2e20 2a2a 4c6f 6720 696e 746f 2079  .2. **Log into y
-0000ac70: 6f75 7220 4265 6e74 6f43 6c6f 7564 2061  our BentoCloud a
-0000ac80: 6363 6f75 6e74 3a2a 2a0a 0a20 2020 6060  ccount:**..   ``
-0000ac90: 6062 6173 680a 2020 2062 656e 746f 6d6c  `bash.   bentoml
-0000aca0: 2063 6c6f 7564 206c 6f67 696e 202d 2d61   cloud login --a
-0000acb0: 7069 2d74 6f6b 656e 203c 796f 7572 2d61  pi-token <your-a
-0000acc0: 7069 2d74 6f6b 656e 3e20 2d2d 656e 6470  pi-token> --endp
-0000acd0: 6f69 6e74 203c 6265 6e74 6f2d 636c 6f75  oint <bento-clou
-0000ace0: 642d 656e 6470 6f69 6e74 3e0a 2020 2060  d-endpoint>.   `
-0000acf0: 6060 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20  ``..> [!NOTE].> 
-0000ad00: 5265 706c 6163 6520 603c 796f 7572 2d61  Replace `<your-a
-0000ad10: 7069 2d74 6f6b 656e 3e60 2061 6e64 2060  pi-token>` and `
-0000ad20: 3c62 656e 746f 2d63 6c6f 7564 2d65 6e64  <bento-cloud-end
-0000ad30: 706f 696e 743e 6020 7769 7468 2079 6f75  point>` with you
-0000ad40: 720a 3e20 7370 6563 6966 6963 2041 5049  r.> specific API
-0000ad50: 2074 6f6b 656e 2061 6e64 2074 6865 2042   token and the B
-0000ad60: 656e 746f 436c 6f75 6420 656e 6470 6f69  entoCloud endpoi
-0000ad70: 6e74 2072 6573 7065 6374 6976 656c 792e  nt respectively.
-0000ad80: 0a0a 332e 202a 2a42 756c 6469 6e67 2061  ..3. **Bulding a
-0000ad90: 2042 656e 746f 2a2a 3a20 5769 7468 204f   Bento**: With O
-0000ada0: 7065 6e4c 4c4d 2c20 796f 7520 6361 6e20  penLLM, you can 
-0000adb0: 6561 7369 6c79 2062 7569 6c64 2061 2042  easily build a B
-0000adc0: 656e 746f 2066 6f72 2061 0a20 2020 7370  ento for a.   sp
-0000add0: 6563 6966 6963 206d 6f64 656c 2c20 7375  ecific model, su
-0000ade0: 6368 2061 7320 606d 6973 7472 616c 6169  ch as `mistralai
-0000adf0: 2f4d 6973 7472 616c 2d37 422d 496e 7374  /Mistral-7B-Inst
-0000ae00: 7275 6374 2d76 302e 3160 3a0a 0a20 2020  ruct-v0.1`:..   
-0000ae10: 6060 6062 6173 680a 2020 206f 7065 6e6c  ```bash.   openl
-0000ae20: 6c6d 2062 7569 6c64 206d 6973 7472 616c  lm build mistral
-0000ae30: 6169 2f4d 6973 7472 616c 2d37 422d 496e  ai/Mistral-7B-In
-0000ae40: 7374 7275 6374 2d76 302e 310a 2020 2060  struct-v0.1.   `
-0000ae50: 6060 0a0a 342e 202a 2a50 7573 6869 6e67  ``..4. **Pushing
-0000ae60: 2061 2042 656e 746f 2a2a 3a20 5075 7368   a Bento**: Push
-0000ae70: 2079 6f75 7220 6672 6573 686c 792d 6275   your freshly-bu
-0000ae80: 696c 7420 4265 6e74 6f20 7365 7276 6963  ilt Bento servic
-0000ae90: 6520 746f 2042 656e 746f 436c 6f75 6420  e to BentoCloud 
-0000aea0: 7669 610a 2020 2074 6865 2060 7075 7368  via.   the `push
-0000aeb0: 6020 636f 6d6d 616e 643a 0a0a 2020 2060  ` command:..   `
-0000aec0: 6060 6261 7368 0a20 2020 6265 6e74 6f6d  ``bash.   bentom
-0000aed0: 6c20 7075 7368 203c 6e61 6d65 3a76 6572  l push <name:ver
-0000aee0: 7369 6f6e 3e0a 2020 2060 6060 0a0a 352e  sion>.   ```..5.
-0000aef0: 202a 2a44 6570 6c6f 7969 6e67 2061 2042   **Deploying a B
-0000af00: 656e 746f 2a2a 3a20 4465 706c 6f79 2079  ento**: Deploy y
-0000af10: 6f75 7220 4c4c 4d73 2074 6f20 4265 6e74  our LLMs to Bent
-0000af20: 6f43 6c6f 7564 2077 6974 6820 6120 7369  oCloud with a si
-0000af30: 6e67 6c65 0a20 2020 6062 656e 746f 6d6c  ngle.   `bentoml
-0000af40: 2064 6570 6c6f 796d 656e 7420 6372 6561   deployment crea
-0000af50: 7465 6020 636f 6d6d 616e 6420 666f 6c6c  te` command foll
-0000af60: 6f77 696e 6720 7468 650a 2020 205b 6465  owing the.   [de
-0000af70: 706c 6f79 6d65 6e74 2069 6e73 7472 7563  ployment instruc
-0000af80: 7469 6f6e 735d 2868 7474 7073 3a2f 2f64  tions](https://d
-0000af90: 6f63 732e 6265 6e74 6f6d 6c2e 636f 6d2f  ocs.bentoml.com/
-0000afa0: 656e 2f6c 6174 6573 742f 7265 6665 7265  en/latest/refere
-0000afb0: 6e63 652f 636c 692e 6874 6d6c 2362 656e  nce/cli.html#ben
-0000afc0: 746f 6d6c 2d64 6570 6c6f 796d 656e 742d  toml-deployment-
-0000afd0: 6372 6561 7465 292e 0a0a 2323 20f0 9f91  create)...## ...
-0000afe0: a520 436f 6d6d 756e 6974 790a 0a45 6e67  . Community..Eng
-0000aff0: 6167 6520 7769 7468 206c 696b 652d 6d69  age with like-mi
-0000b000: 6e64 6564 2069 6e64 6976 6964 7561 6c73  nded individuals
-0000b010: 2070 6173 7369 6f6e 6174 6520 6162 6f75   passionate abou
-0000b020: 7420 4c4c 4d73 2c20 4149 2c20 616e 6420  t LLMs, AI, and 
-0000b030: 6d6f 7265 206f 6e20 6f75 720a 5b44 6973  more on our.[Dis
-0000b040: 636f 7264 5d28 6874 7470 733a 2f2f 6c2e  cord](https://l.
-0000b050: 6265 6e74 6f6d 6c2e 636f 6d2f 6a6f 696e  bentoml.com/join
-0000b060: 2d6f 7065 6e6c 6c6d 2d64 6973 636f 7264  -openllm-discord
-0000b070: 2921 0a0a 4f70 656e 4c4c 4d20 6973 2061  )!..OpenLLM is a
-0000b080: 6374 6976 656c 7920 6d61 696e 7461 696e  ctively maintain
-0000b090: 6564 2062 7920 7468 6520 4265 6e74 6f4d  ed by the BentoM
-0000b0a0: 4c20 7465 616d 2e20 4665 656c 2066 7265  L team. Feel fre
-0000b0b0: 6520 746f 2072 6561 6368 206f 7574 2061  e to reach out a
-0000b0c0: 6e64 0a6a 6f69 6e20 7573 2069 6e20 6f75  nd.join us in ou
-0000b0d0: 7220 7075 7273 7569 7420 746f 206d 616b  r pursuit to mak
-0000b0e0: 6520 4c4c 4d73 206d 6f72 6520 6163 6365  e LLMs more acce
-0000b0f0: 7373 6962 6c65 2061 6e64 2065 6173 7920  ssible and easy 
-0000b100: 746f 2075 7365 20f0 9f91 890a 5b4a 6f69  to use .....[Joi
-0000b110: 6e20 6f75 7220 536c 6163 6b20 636f 6d6d  n our Slack comm
-0000b120: 756e 6974 7921 5d28 6874 7470 733a 2f2f  unity!](https://
-0000b130: 6c2e 6265 6e74 6f6d 6c2e 636f 6d2f 6a6f  l.bentoml.com/jo
-0000b140: 696e 2d73 6c61 636b 290a 0a23 2320 f09f  in-slack)..## ..
-0000b150: 8e81 2043 6f6e 7472 6962 7574 696e 670a  .. Contributing.
-0000b160: 0a57 6520 7765 6c63 6f6d 6520 636f 6e74  .We welcome cont
-0000b170: 7269 6275 7469 6f6e 7321 2049 6620 796f  ributions! If yo
-0000b180: 7527 7265 2069 6e74 6572 6573 7465 6420  u're interested 
-0000b190: 696e 2065 6e68 616e 6369 6e67 204f 7065  in enhancing Ope
-0000b1a0: 6e4c 4c4d 2773 0a63 6170 6162 696c 6974  nLLM's.capabilit
-0000b1b0: 6965 7320 6f72 2068 6176 6520 616e 7920  ies or have any 
-0000b1c0: 7175 6573 7469 6f6e 732c 2064 6f6e 2774  questions, don't
-0000b1d0: 2068 6573 6974 6174 6520 746f 2072 6561   hesitate to rea
-0000b1e0: 6368 206f 7574 2069 6e20 6f75 720a 5b64  ch out in our.[d
-0000b1f0: 6973 636f 7264 2063 6861 6e6e 656c 5d28  iscord channel](
-0000b200: 6874 7470 733a 2f2f 6c2e 6265 6e74 6f6d  https://l.bentom
-0000b210: 6c2e 636f 6d2f 6a6f 696e 2d6f 7065 6e6c  l.com/join-openl
-0000b220: 6c6d 2d64 6973 636f 7264 292e 0a0a 4368  lm-discord)...Ch
-0000b230: 6563 6b6f 7574 206f 7572 0a5b 4465 7665  eckout our.[Deve
-0000b240: 6c6f 7065 7220 4775 6964 655d 2868 7474  loper Guide](htt
-0000b250: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000b260: 6265 6e74 6f6d 6c2f 4f70 656e 4c4c 4d2f  bentoml/OpenLLM/
-0000b270: 626c 6f62 2f6d 6169 6e2f 4445 5645 4c4f  blob/main/DEVELO
-0000b280: 504d 454e 542e 6d64 290a 6966 2079 6f75  PMENT.md).if you
-0000b290: 2077 6973 6820 746f 2063 6f6e 7472 6962   wish to contrib
-0000b2a0: 7574 6520 746f 204f 7065 6e4c 4c4d 2773  ute to OpenLLM's
-0000b2b0: 2063 6f64 6562 6173 652e 0a0a 2323 20f0   codebase...## .
-0000b2c0: 9f8d 8720 5465 6c65 6d65 7472 790a 0a4f  ... Telemetry..O
-0000b2d0: 7065 6e4c 4c4d 2063 6f6c 6c65 6374 7320  penLLM collects 
-0000b2e0: 7573 6167 6520 6461 7461 2074 6f20 656e  usage data to en
-0000b2f0: 6861 6e63 6520 7573 6572 2065 7870 6572  hance user exper
-0000b300: 6965 6e63 6520 616e 6420 696d 7072 6f76  ience and improv
-0000b310: 6520 7468 6520 7072 6f64 7563 742e 0a57  e the product..W
-0000b320: 6520 6f6e 6c79 2072 6570 6f72 7420 4f70  e only report Op
-0000b330: 656e 4c4c 4d27 7320 696e 7465 726e 616c  enLLM's internal
-0000b340: 2041 5049 2063 616c 6c73 2061 6e64 2065   API calls and e
-0000b350: 6e73 7572 6520 6d61 7869 6d75 6d20 7072  nsure maximum pr
-0000b360: 6976 6163 7920 6279 0a65 7863 6c75 6469  ivacy by.excludi
-0000b370: 6e67 2073 656e 7369 7469 7665 2069 6e66  ng sensitive inf
-0000b380: 6f72 6d61 7469 6f6e 2e20 5765 2077 696c  ormation. We wil
-0000b390: 6c20 6e65 7665 7220 636f 6c6c 6563 7420  l never collect 
-0000b3a0: 7573 6572 2063 6f64 652c 206d 6f64 656c  user code, model
-0000b3b0: 2064 6174 612c 206f 720a 7374 6163 6b20   data, or.stack 
-0000b3c0: 7472 6163 6573 2e20 466f 7220 7573 6167  traces. For usag
-0000b3d0: 6520 7472 6163 6b69 6e67 2c20 6368 6563  e tracking, chec
-0000b3e0: 6b20 6f75 7420 7468 650a 5b63 6f64 655d  k out the.[code]
-0000b3f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-0000b400: 636f 6d2f 6265 6e74 6f6d 6c2f 4f70 656e  com/bentoml/Open
-0000b410: 4c4c 4d2f 626c 6f62 2f6d 6169 6e2f 6f70  LLM/blob/main/op
-0000b420: 656e 6c6c 6d2d 636f 7265 2f73 7263 2f6f  enllm-core/src/o
-0000b430: 7065 6e6c 6c6d 5f63 6f72 652f 7574 696c  penllm_core/util
-0000b440: 732f 616e 616c 7974 6963 732e 7079 292e  s/analytics.py).
-0000b450: 0a0a 596f 7520 6361 6e20 6f70 7420 6f75  ..You can opt ou
-0000b460: 7420 6f66 2075 7361 6765 2074 7261 636b  t of usage track
-0000b470: 696e 6720 6279 2075 7369 6e67 2074 6865  ing by using the
-0000b480: 2060 2d2d 646f 2d6e 6f74 2d74 7261 636b   `--do-not-track
-0000b490: 6020 434c 4920 6f70 7469 6f6e 3a0a 0a60  ` CLI option:..`
-0000b4a0: 6060 6261 7368 0a6f 7065 6e6c 6c6d 205b  ``bash.openllm [
-0000b4b0: 636f 6d6d 616e 645d 202d 2d64 6f2d 6e6f  command] --do-no
-0000b4c0: 742d 7472 6163 6b0a 6060 600a 0a4f 7220  t-track.```..Or 
-0000b4d0: 6279 2073 6574 7469 6e67 2074 6865 2065  by setting the e
-0000b4e0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-0000b4f0: 626c 6520 604f 5045 4e4c 4c4d 5f44 4f5f  ble `OPENLLM_DO_
-0000b500: 4e4f 545f 5452 4143 4b3d 5472 7565 603a  NOT_TRACK=True`:
-0000b510: 0a0a 6060 6062 6173 680a 6578 706f 7274  ..```bash.export
-0000b520: 204f 5045 4e4c 4c4d 5f44 4f5f 4e4f 545f   OPENLLM_DO_NOT_
-0000b530: 5452 4143 4b3d 5472 7565 0a60 6060 0a0a  TRACK=True.```..
-0000b540: 2323 20f0 9f93 9420 4369 7461 7469 6f6e  ## .... Citation
-0000b550: 0a0a 4966 2079 6f75 2075 7365 204f 7065  ..If you use Ope
-0000b560: 6e4c 4c4d 2069 6e20 796f 7572 2072 6573  nLLM in your res
-0000b570: 6561 7263 682c 2077 6520 7072 6f76 6964  earch, we provid
-0000b580: 6520 6120 5b63 6974 6174 696f 6e5d 282e  e a [citation](.
-0000b590: 2f43 4954 4154 494f 4e2e 6366 6629 2074  /CITATION.cff) t
-0000b5a0: 6f0a 7573 653a 0a0a 6060 6062 6962 7465  o.use:..```bibte
-0000b5b0: 780a 4073 6f66 7477 6172 657b 5068 616d  x.@software{Pham
-0000b5c0: 5f4f 7065 6e4c 4c4d 5f4f 7065 7261 7469  _OpenLLM_Operati
-0000b5d0: 6e67 5f4c 4c4d 735f 3230 3233 2c0a 6175  ng_LLMs_2023,.au
-0000b5e0: 7468 6f72 203d 207b 5068 616d 2c20 4161  thor = {Pham, Aa
-0000b5f0: 726f 6e20 616e 6420 5961 6e67 2c20 4368  ron and Yang, Ch
-0000b600: 616f 7975 2061 6e64 2053 6865 6e67 2c20  aoyu and Sheng, 
-0000b610: 5365 616e 2061 6e64 2020 5a68 616f 2c20  Sean and  Zhao, 
-0000b620: 5368 656e 7961 6e67 2061 6e64 204c 6565  Shenyang and Lee
-0000b630: 2c20 5361 7579 6f6e 2061 6e64 204a 6961  , Sauyon and Jia
-0000b640: 6e67 2c20 426f 2061 6e64 2044 6f6e 672c  ng, Bo and Dong,
-0000b650: 2046 6f67 2061 6e64 2047 7561 6e2c 2058   Fog and Guan, X
-0000b660: 6970 656e 6720 616e 6420 4d69 6e67 2c20  ipeng and Ming, 
-0000b670: 4672 6f73 747d 2c0a 6c69 6365 6e73 6520  Frost},.license 
-0000b680: 3d20 7b41 7061 6368 652d 322e 307d 2c0a  = {Apache-2.0},.
-0000b690: 6d6f 6e74 6820 3d20 6a75 6e2c 0a74 6974  month = jun,.tit
-0000b6a0: 6c65 203d 207b 7b4f 7065 6e4c 4c4d 3a20  le = {{OpenLLM: 
-0000b6b0: 4f70 6572 6174 696e 6720 4c4c 4d73 2069  Operating LLMs i
-0000b6c0: 6e20 7072 6f64 7563 7469 6f6e 7d7d 2c0a  n production}},.
-0000b6d0: 7572 6c20 3d20 7b68 7474 7073 3a2f 2f67  url = {https://g
-0000b6e0: 6974 6875 622e 636f 6d2f 6265 6e74 6f6d  ithub.com/bentom
-0000b6f0: 6c2f 4f70 656e 4c4c 4d7d 2c0a 7965 6172  l/OpenLLM},.year
-0000b700: 203d 207b 3230 3233 7d0a 7d0a 6060 600a   = {2023}.}.```.
-0000b710: 0a3c 212d 2d20 6861 7463 682d 6661 6e63  .<!-- hatch-fanc
-0000b720: 792d 7079 7069 2d72 6561 646d 6520 6d65  y-pypi-readme me
-0000b730: 7461 2073 746f 7020 2d2d 3e0a            ta stop -->.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
+00000020: 6c6c 6d0a 5665 7273 696f 6e3a 2030 2e35  llm.Version: 0.5
+00000030: 2e30 6134 0a53 756d 6d61 7279 3a20 4f70  .0a4.Summary: Op
+00000040: 656e 4c4c 4d3a 2052 756e 2061 6e79 206f  enLLM: Run any o
+00000050: 7065 6e2d 736f 7572 6365 204c 4c4d 732c  pen-source LLMs,
+00000060: 2073 7563 6820 6173 204c 6c61 6d61 2032   such as Llama 2
+00000070: 2c20 4d69 7374 7261 6c2c 2061 7320 4f70  , Mistral, as Op
+00000080: 656e 4149 2063 6f6d 7061 7469 626c 6520  enAI compatible 
+00000090: 4150 4920 656e 6470 6f69 6e74 2069 6e20  API endpoint in 
+000000a0: 7468 6520 636c 6f75 642e 0a50 726f 6a65  the cloud..Proje
+000000b0: 6374 2d55 524c 3a20 426c 6f67 2c20 6874  ct-URL: Blog, ht
+000000c0: 7470 733a 2f2f 6d6f 6465 6c73 6572 7669  tps://modelservi
+000000d0: 6e67 2e63 6f6d 0a50 726f 6a65 6374 2d55  ng.com.Project-U
+000000e0: 524c 3a20 4368 6174 2c20 6874 7470 733a  RL: Chat, https:
+000000f0: 2f2f 6469 7363 6f72 642e 6767 2f6f 7065  //discord.gg/ope
+00000100: 6e6c 6c6d 0a50 726f 6a65 6374 2d55 524c  nllm.Project-URL
+00000110: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+00000120: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
+00000130: 636f 6d2f 6265 6e74 6f6d 6c2f 6f70 656e  com/bentoml/open
+00000140: 6c6c 6d23 7265 6164 6d65 0a50 726f 6a65  llm#readme.Proje
+00000150: 6374 2d55 524c 3a20 4769 7448 7562 2c20  ct-URL: GitHub, 
+00000160: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000170: 6f6d 2f62 656e 746f 6d6c 2f4f 7065 6e4c  om/bentoml/OpenL
+00000180: 4c4d 0a50 726f 6a65 6374 2d55 524c 3a20  LM.Project-URL: 
+00000190: 4869 7374 6f72 792c 2068 7474 7073 3a2f  History, https:/
+000001a0: 2f67 6974 6875 622e 636f 6d2f 6265 6e74  /github.com/bent
+000001b0: 6f6d 6c2f 4f70 656e 4c4c 4d2f 626c 6f62  oml/OpenLLM/blob
+000001c0: 2f6d 6169 6e2f 4348 414e 4745 4c4f 472e  /main/CHANGELOG.
+000001d0: 6d64 0a50 726f 6a65 6374 2d55 524c 3a20  md.Project-URL: 
+000001e0: 486f 6d65 7061 6765 2c20 6874 7470 733a  Homepage, https:
+000001f0: 2f2f 6265 6e74 6f6d 6c2e 636f 6d0a 5072  //bentoml.com.Pr
+00000200: 6f6a 6563 742d 5552 4c3a 2054 7261 636b  oject-URL: Track
+00000210: 6572 2c20 6874 7470 733a 2f2f 6769 7468  er, https://gith
+00000220: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
+00000230: 7065 6e4c 4c4d 2f69 7373 7565 730a 5072  penLLM/issues.Pr
+00000240: 6f6a 6563 742d 5552 4c3a 2054 7769 7474  oject-URL: Twitt
+00000250: 6572 2c20 6874 7470 733a 2f2f 7477 6974  er, https://twit
+00000260: 7465 722e 636f 6d2f 6265 6e74 6f6d 6c61  ter.com/bentomla
+00000270: 690a 4175 7468 6f72 2d65 6d61 696c 3a20  i.Author-email: 
+00000280: 4161 726f 6e20 5068 616d 203c 6161 726e  Aaron Pham <aarn
+00000290: 7068 6d40 6265 6e74 6f6d 6c2e 636f 6d3e  phm@bentoml.com>
+000002a0: 2c20 4265 6e74 6f4d 4c20 5465 616d 203c  , BentoML Team <
+000002b0: 636f 6e74 6163 7440 6265 6e74 6f6d 6c2e  contact@bentoml.
+000002c0: 636f 6d3e 0a4c 6963 656e 7365 2d45 7870  com>.License-Exp
+000002d0: 7265 7373 696f 6e3a 2041 7061 6368 652d  ression: Apache-
+000002e0: 322e 300a 4c69 6365 6e73 652d 4669 6c65  2.0.License-File
+000002f0: 3a20 4c49 4345 4e53 452e 6d64 0a4b 6579  : LICENSE.md.Key
+00000300: 776f 7264 733a 2041 492c 416c 7061 6361  words: AI,Alpaca
+00000310: 2c42 656e 746f 4d4c 2c46 616c 636f 6e2c  ,BentoML,Falcon,
+00000320: 4669 6e65 2074 756e 696e 672c 4765 6e65  Fine tuning,Gene
+00000330: 7261 7469 7665 2041 492c 4c4c 4d4f 7073  rative AI,LLMOps
+00000340: 2c4c 6172 6765 204c 616e 6775 6167 6520  ,Large Language 
+00000350: 4d6f 6465 6c2c 4c6c 616d 6120 322c 4d4c  Model,Llama 2,ML
+00000360: 4f70 732c 4d69 7374 7261 6c2c 4d6f 6465  Ops,Mistral,Mode
+00000370: 6c20 4465 706c 6f79 6d65 6e74 2c4d 6f64  l Deployment,Mod
+00000380: 656c 2053 6572 7669 6e67 2c50 7954 6f72  el Serving,PyTor
+00000390: 6368 2c53 6572 7665 726c 6573 732c 5374  ch,Serverless,St
+000003a0: 6162 6c65 4c4d 2c54 7261 6e73 666f 726d  ableLM,Transform
+000003b0: 6572 732c 5669 6375 6e61 2c76 4c4c 4d0a  ers,Vicuna,vLLM.
+000003c0: 436c 6173 7369 6669 6572 3a20 4465 7665  Classifier: Deve
+000003d0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+000003e0: 3a20 3520 2d20 5072 6f64 7563 7469 6f6e  : 5 - Production
+000003f0: 2f53 7461 626c 650a 436c 6173 7369 6669  /Stable.Classifi
+00000400: 6572 3a20 456e 7669 726f 6e6d 656e 7420  er: Environment 
+00000410: 3a3a 2047 5055 203a 3a20 4e56 4944 4941  :: GPU :: NVIDIA
+00000420: 2043 5544 410a 436c 6173 7369 6669 6572   CUDA.Classifier
+00000430: 3a20 456e 7669 726f 6e6d 656e 7420 3a3a  : Environment ::
+00000440: 2047 5055 203a 3a20 4e56 4944 4941 2043   GPU :: NVIDIA C
+00000450: 5544 4120 3a3a 2031 312e 370a 436c 6173  UDA :: 11.7.Clas
+00000460: 7369 6669 6572 3a20 456e 7669 726f 6e6d  sifier: Environm
+00000470: 656e 7420 3a3a 2047 5055 203a 3a20 4e56  ent :: GPU :: NV
+00000480: 4944 4941 2043 5544 4120 3a3a 2031 312e  IDIA CUDA :: 11.
+00000490: 380a 436c 6173 7369 6669 6572 3a20 456e  8.Classifier: En
+000004a0: 7669 726f 6e6d 656e 7420 3a3a 2047 5055  vironment :: GPU
+000004b0: 203a 3a20 4e56 4944 4941 2043 5544 4120   :: NVIDIA CUDA 
+000004c0: 3a3a 2031 320a 436c 6173 7369 6669 6572  :: 12.Classifier
+000004d0: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+000004e0: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+000004f0: 730a 436c 6173 7369 6669 6572 3a20 496e  s.Classifier: In
+00000500: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000510: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
+00000520: 7263 680a 436c 6173 7369 6669 6572 3a20  rch.Classifier: 
+00000530: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000540: 6520 3a3a 2053 7973 7465 6d20 4164 6d69  e :: System Admi
+00000550: 6e69 7374 7261 746f 7273 0a43 6c61 7373  nistrators.Class
+00000560: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
+00000570: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000580: 3a20 4170 6163 6865 2053 6f66 7477 6172  : Apache Softwar
+00000590: 6520 4c69 6365 6e73 650a 436c 6173 7369  e License.Classi
+000005a0: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+000005b0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000005c0: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+000005d0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000005e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000005f0: 686f 6e0a 436c 6173 7369 6669 6572 3a20  hon.Classifier: 
+00000600: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000610: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000620: 3a20 330a 436c 6173 7369 6669 6572 3a20  : 3.Classifier: 
+00000630: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000640: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000650: 3a20 3320 3a3a 204f 6e6c 790a 436c 6173  : 3 :: Only.Clas
+00000660: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
+00000670: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000680: 5079 7468 6f6e 203a 3a20 332e 380a 436c  Python :: 3.8.Cl
+00000690: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+000006a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000006b0: 3a20 5079 7468 6f6e 203a 3a20 332e 390a  : Python :: 3.9.
+000006c0: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+000006d0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000006e0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+000006f0: 3130 0a43 6c61 7373 6966 6965 723a 2050  10.Classifier: P
+00000700: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000710: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000720: 2033 2e31 310a 436c 6173 7369 6669 6572   3.11.Classifier
+00000730: 3a20 5072 6f67 7261 6d6d 696e 6720 4c61  : Programming La
+00000740: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000750: 203a 3a20 332e 3132 0a43 6c61 7373 6966   :: 3.12.Classif
+00000760: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000770: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000780: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+00000790: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
+000007a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000007b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000007c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2049  e :: Python :: I
+000007d0: 6d70 6c65 6d65 6e74 6174 696f 6e20 3a3a  mplementation ::
+000007e0: 2050 7950 790a 436c 6173 7369 6669 6572   PyPy.Classifier
+000007f0: 3a20 546f 7069 6320 3a3a 2053 6369 656e  : Topic :: Scien
+00000800: 7469 6669 632f 456e 6769 6e65 6572 696e  tific/Engineerin
+00000810: 6720 3a3a 2041 7274 6966 6963 6961 6c20  g :: Artificial 
+00000820: 496e 7465 6c6c 6967 656e 6365 0a43 6c61  Intelligence.Cla
+00000830: 7373 6966 6965 723a 2054 6f70 6963 203a  ssifier: Topic :
+00000840: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
+00000850: 6f70 6d65 6e74 203a 3a20 4c69 6272 6172  opment :: Librar
+00000860: 6965 730a 436c 6173 7369 6669 6572 3a20  ies.Classifier: 
+00000870: 5479 7069 6e67 203a 3a20 5479 7065 640a  Typing :: Typed.
+00000880: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000890: 203e 3d33 2e38 0a52 6571 7569 7265 732d   >=3.8.Requires-
+000008a0: 4469 7374 3a20 6163 6365 6c65 7261 7465  Dist: accelerate
+000008b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000008c0: 6265 6e74 6f6d 6c5b 696f 5d3e 3d31 2e32  bentoml[io]>=1.2
+000008d0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000008e0: 6269 7473 616e 6462 7974 6573 3c30 2e34  bitsandbytes<0.4
+000008f0: 320a 5265 7175 6972 6573 2d44 6973 743a  2.Requires-Dist:
+00000900: 2062 7569 6c64 5b76 6972 7475 616c 656e   build[virtualen
+00000910: 765d 3c31 0a52 6571 7569 7265 732d 4469  v]<1.Requires-Di
+00000920: 7374 3a20 636c 6963 6b3e 3d38 2e31 2e33  st: click>=8.1.3
+00000930: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000940: 6375 6461 2d70 7974 686f 6e3b 2070 6c61  cuda-python; pla
+00000950: 7466 6f72 6d5f 7379 7374 656d 2021 3d20  tform_system != 
+00000960: 2744 6172 7769 6e27 0a52 6571 7569 7265  'Darwin'.Require
+00000970: 732d 4469 7374 3a20 6569 6e6f 7073 0a52  s-Dist: einops.R
+00000980: 6571 7569 7265 732d 4469 7374 3a20 6768  equires-Dist: gh
+00000990: 6170 690a 5265 7175 6972 6573 2d44 6973  api.Requires-Dis
+000009a0: 743a 206f 7065 6e6c 6c6d 2d63 6c69 656e  t: openllm-clien
+000009b0: 743e 3d30 2e35 2e30 2d61 6c70 6861 2e34  t>=0.5.0-alpha.4
+000009c0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000009d0: 6f70 656e 6c6c 6d2d 636f 7265 3e3d 302e  openllm-core>=0.
+000009e0: 352e 302d 616c 7068 612e 340a 5265 7175  5.0-alpha.4.Requ
+000009f0: 6972 6573 2d44 6973 743a 206f 7074 696d  ires-Dist: optim
+00000a00: 756d 3e3d 312e 3132 2e30 0a52 6571 7569  um>=1.12.0.Requi
+00000a10: 7265 732d 4469 7374 3a20 7361 6665 7465  res-Dist: safete
+00000a20: 6e73 6f72 730a 5265 7175 6972 6573 2d44  nsors.Requires-D
+00000a30: 6973 743a 2073 6369 7079 0a52 6571 7569  ist: scipy.Requi
+00000a40: 7265 732d 4469 7374 3a20 7365 6e74 656e  res-Dist: senten
+00000a50: 6365 7069 6563 650a 5265 7175 6972 6573  cepiece.Requires
+00000a60: 2d44 6973 743a 2074 7261 6e73 666f 726d  -Dist: transform
+00000a70: 6572 735b 746f 6b65 6e69 7a65 7273 2c74  ers[tokenizers,t
+00000a80: 6f72 6368 5d3e 3d34 2e33 362e 300a 5265  orch]>=4.36.0.Re
+00000a90: 7175 6972 6573 2d44 6973 743a 2076 6c6c  quires-Dist: vll
+00000aa0: 6d3e 3d30 2e34 2e32 0a50 726f 7669 6465  m>=0.4.2.Provide
+00000ab0: 732d 4578 7472 613a 2061 6765 6e74 730a  s-Extra: agents.
+00000ac0: 5265 7175 6972 6573 2d44 6973 743a 2064  Requires-Dist: d
+00000ad0: 6966 6675 7365 7273 3b20 6578 7472 6120  iffusers; extra 
+00000ae0: 3d3d 2027 6167 656e 7473 270a 5265 7175  == 'agents'.Requ
+00000af0: 6972 6573 2d44 6973 743a 2073 6f75 6e64  ires-Dist: sound
+00000b00: 6669 6c65 3b20 6578 7472 6120 3d3d 2027  file; extra == '
+00000b10: 6167 656e 7473 270a 5265 7175 6972 6573  agents'.Requires
+00000b20: 2d44 6973 743a 2074 7261 6e73 666f 726d  -Dist: transform
+00000b30: 6572 735b 6167 656e 7473 5d3e 3d34 2e33  ers[agents]>=4.3
+00000b40: 362e 303b 2065 7874 7261 203d 3d20 2761  6.0; extra == 'a
+00000b50: 6765 6e74 7327 0a50 726f 7669 6465 732d  gents'.Provides-
+00000b60: 4578 7472 613a 2061 6c6c 0a52 6571 7569  Extra: all.Requi
+00000b70: 7265 732d 4469 7374 3a20 6f70 656e 6c6c  res-Dist: openll
+00000b80: 6d5b 6675 6c6c 5d3b 2065 7874 7261 203d  m[full]; extra =
+00000b90: 3d20 2761 6c6c 270a 5072 6f76 6964 6573  = 'all'.Provides
+00000ba0: 2d45 7874 7261 3a20 6177 710a 5265 7175  -Extra: awq.Requ
+00000bb0: 6972 6573 2d44 6973 743a 2061 7574 6f61  ires-Dist: autoa
+00000bc0: 7771 3b20 6578 7472 6120 3d3d 2027 6177  wq; extra == 'aw
+00000bd0: 7127 0a50 726f 7669 6465 732d 4578 7472  q'.Provides-Extr
+00000be0: 613a 2062 6169 6368 7561 6e0a 5265 7175  a: baichuan.Requ
+00000bf0: 6972 6573 2d44 6973 743a 2063 706d 2d6b  ires-Dist: cpm-k
+00000c00: 6572 6e65 6c73 3b20 6578 7472 6120 3d3d  ernels; extra ==
+00000c10: 2027 6261 6963 6875 616e 270a 5072 6f76   'baichuan'.Prov
+00000c20: 6964 6573 2d45 7874 7261 3a20 6368 6174  ides-Extra: chat
+00000c30: 676c 6d0a 5265 7175 6972 6573 2d44 6973  glm.Requires-Dis
+00000c40: 743a 2063 706d 2d6b 6572 6e65 6c73 3b20  t: cpm-kernels; 
+00000c50: 6578 7472 6120 3d3d 2027 6368 6174 676c  extra == 'chatgl
+00000c60: 6d27 0a50 726f 7669 6465 732d 4578 7472  m'.Provides-Extr
+00000c70: 613a 2064 6272 780a 5265 7175 6972 6573  a: dbrx.Requires
+00000c80: 2d44 6973 743a 2063 706d 2d6b 6572 6e65  -Dist: cpm-kerne
+00000c90: 6c73 3b20 6578 7472 6120 3d3d 2027 6462  ls; extra == 'db
+00000ca0: 7278 270a 5072 6f76 6964 6573 2d45 7874  rx'.Provides-Ext
+00000cb0: 7261 3a20 646f 6c6c 792d 7632 0a52 6571  ra: dolly-v2.Req
+00000cc0: 7569 7265 732d 4469 7374 3a20 6370 6d2d  uires-Dist: cpm-
+00000cd0: 6b65 726e 656c 733b 2065 7874 7261 203d  kernels; extra =
+00000ce0: 3d20 2764 6f6c 6c79 2d76 3227 0a50 726f  = 'dolly-v2'.Pro
+00000cf0: 7669 6465 732d 4578 7472 613a 2066 616c  vides-Extra: fal
+00000d00: 636f 6e0a 5265 7175 6972 6573 2d44 6973  con.Requires-Dis
+00000d10: 743a 2078 666f 726d 6572 733b 2065 7874  t: xformers; ext
+00000d20: 7261 203d 3d20 2766 616c 636f 6e27 0a50  ra == 'falcon'.P
+00000d30: 726f 7669 6465 732d 4578 7472 613a 2066  rovides-Extra: f
+00000d40: 696e 652d 7475 6e65 0a52 6571 7569 7265  ine-tune.Require
+00000d50: 732d 4469 7374 3a20 6461 7461 7365 7473  s-Dist: datasets
+00000d60: 3b20 6578 7472 6120 3d3d 2027 6669 6e65  ; extra == 'fine
+00000d70: 2d74 756e 6527 0a52 6571 7569 7265 732d  -tune'.Requires-
+00000d80: 4469 7374 3a20 6875 6767 696e 6766 6163  Dist: huggingfac
+00000d90: 652d 6875 623b 2065 7874 7261 203d 3d20  e-hub; extra == 
+00000da0: 2766 696e 652d 7475 6e65 270a 5265 7175  'fine-tune'.Requ
+00000db0: 6972 6573 2d44 6973 743a 2070 6566 743e  ires-Dist: peft>
+00000dc0: 3d30 2e36 2e30 3b20 6578 7472 6120 3d3d  =0.6.0; extra ==
+00000dd0: 2027 6669 6e65 2d74 756e 6527 0a52 6571   'fine-tune'.Req
+00000de0: 7569 7265 732d 4469 7374 3a20 7472 6c3b  uires-Dist: trl;
+00000df0: 2065 7874 7261 203d 3d20 2766 696e 652d   extra == 'fine-
+00000e00: 7475 6e65 270a 5072 6f76 6964 6573 2d45  tune'.Provides-E
+00000e10: 7874 7261 3a20 666c 616e 2d74 350a 5265  xtra: flan-t5.Re
+00000e20: 7175 6972 6573 2d44 6973 743a 2078 666f  quires-Dist: xfo
+00000e30: 726d 6572 733b 2065 7874 7261 203d 3d20  rmers; extra == 
+00000e40: 2766 6c61 6e2d 7435 270a 5072 6f76 6964  'flan-t5'.Provid
+00000e50: 6573 2d45 7874 7261 3a20 6675 6c6c 0a52  es-Extra: full.R
+00000e60: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+00000e70: 656e 6c6c 6d5b 6167 656e 7473 2c61 7771  enllm[agents,awq
+00000e80: 2c62 6169 6368 7561 6e2c 6368 6174 676c  ,baichuan,chatgl
+00000e90: 6d2c 6462 7278 2c64 6f6c 6c79 2d76 322c  m,dbrx,dolly-v2,
+00000ea0: 6661 6c63 6f6e 2c66 696e 652d 7475 6e65  falcon,fine-tune
+00000eb0: 2c66 6c61 6e2d 7435 2c67 656d 6d61 2c67  ,flan-t5,gemma,g
+00000ec0: 676d 6c2c 6770 742d 6e65 6f78 2c67 7074  gml,gpt-neox,gpt
+00000ed0: 712c 6772 7063 2c6c 6c61 6d61 2c6d 6973  q,grpc,llama,mis
+00000ee0: 7472 616c 2c6d 6978 7472 616c 2c6d 7074  tral,mixtral,mpt
+00000ef0: 2c6f 7065 6e61 692c 6f70 742c 7068 692c  ,openai,opt,phi,
+00000f00: 706c 6179 6772 6f75 6e64 2c71 7765 6e2c  playground,qwen,
+00000f10: 7374 6162 6c65 6c6d 2c73 7461 7263 6f64  stablelm,starcod
+00000f20: 6572 2c76 6c6c 6d2c 7969 5d3b 2065 7874  er,vllm,yi]; ext
+00000f30: 7261 203d 3d20 2766 756c 6c27 0a50 726f  ra == 'full'.Pro
+00000f40: 7669 6465 732d 4578 7472 613a 2067 656d  vides-Extra: gem
+00000f50: 6d61 0a52 6571 7569 7265 732d 4469 7374  ma.Requires-Dist
+00000f60: 3a20 7866 6f72 6d65 7273 3b20 6578 7472  : xformers; extr
+00000f70: 6120 3d3d 2027 6765 6d6d 6127 0a50 726f  a == 'gemma'.Pro
+00000f80: 7669 6465 732d 4578 7472 613a 2067 676d  vides-Extra: ggm
+00000f90: 6c0a 5265 7175 6972 6573 2d44 6973 743a  l.Requires-Dist:
+00000fa0: 2063 7472 616e 7366 6f72 6d65 7273 3b20   ctransformers; 
+00000fb0: 6578 7472 6120 3d3d 2027 6767 6d6c 270a  extra == 'ggml'.
+00000fc0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00000fd0: 6770 742d 6e65 6f78 0a52 6571 7569 7265  gpt-neox.Require
+00000fe0: 732d 4469 7374 3a20 7866 6f72 6d65 7273  s-Dist: xformers
+00000ff0: 3b20 6578 7472 6120 3d3d 2027 6770 742d  ; extra == 'gpt-
+00001000: 6e65 6f78 270a 5072 6f76 6964 6573 2d45  neox'.Provides-E
+00001010: 7874 7261 3a20 6770 7471 0a52 6571 7569  xtra: gptq.Requi
+00001020: 7265 732d 4469 7374 3a20 6175 746f 2d67  res-Dist: auto-g
+00001030: 7074 715b 7472 6974 6f6e 5d3e 3d30 2e34  ptq[triton]>=0.4
+00001040: 2e32 3b20 6578 7472 6120 3d3d 2027 6770  .2; extra == 'gp
+00001050: 7471 270a 5072 6f76 6964 6573 2d45 7874  tq'.Provides-Ext
+00001060: 7261 3a20 6772 7063 0a52 6571 7569 7265  ra: grpc.Require
+00001070: 732d 4469 7374 3a20 6265 6e74 6f6d 6c5b  s-Dist: bentoml[
+00001080: 6772 7063 5d3e 3d31 2e32 3b20 6578 7472  grpc]>=1.2; extr
+00001090: 6120 3d3d 2027 6772 7063 270a 5072 6f76  a == 'grpc'.Prov
+000010a0: 6964 6573 2d45 7874 7261 3a20 6c6c 616d  ides-Extra: llam
+000010b0: 610a 5265 7175 6972 6573 2d44 6973 743a  a.Requires-Dist:
+000010c0: 2078 666f 726d 6572 733b 2065 7874 7261   xformers; extra
+000010d0: 203d 3d20 276c 6c61 6d61 270a 5072 6f76   == 'llama'.Prov
+000010e0: 6964 6573 2d45 7874 7261 3a20 6d69 7374  ides-Extra: mist
+000010f0: 7261 6c0a 5265 7175 6972 6573 2d44 6973  ral.Requires-Dis
+00001100: 743a 2078 666f 726d 6572 733b 2065 7874  t: xformers; ext
+00001110: 7261 203d 3d20 276d 6973 7472 616c 270a  ra == 'mistral'.
+00001120: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+00001130: 6d69 7874 7261 6c0a 5265 7175 6972 6573  mixtral.Requires
+00001140: 2d44 6973 743a 2078 666f 726d 6572 733b  -Dist: xformers;
+00001150: 2065 7874 7261 203d 3d20 276d 6978 7472   extra == 'mixtr
+00001160: 616c 270a 5072 6f76 6964 6573 2d45 7874  al'.Provides-Ext
+00001170: 7261 3a20 6d70 740a 5265 7175 6972 6573  ra: mpt.Requires
+00001180: 2d44 6973 743a 2074 7269 746f 6e3b 2065  -Dist: triton; e
+00001190: 7874 7261 203d 3d20 276d 7074 270a 5072  xtra == 'mpt'.Pr
+000011a0: 6f76 6964 6573 2d45 7874 7261 3a20 6f70  ovides-Extra: op
+000011b0: 656e 6169 0a52 6571 7569 7265 732d 4469  enai.Requires-Di
+000011c0: 7374 3a20 6661 7374 6170 693b 2065 7874  st: fastapi; ext
+000011d0: 7261 203d 3d20 276f 7065 6e61 6927 0a52  ra == 'openai'.R
+000011e0: 6571 7569 7265 732d 4469 7374 3a20 6f70  equires-Dist: op
+000011f0: 656e 6169 5b64 6174 616c 6962 5d3e 3d31  enai[datalib]>=1
+00001200: 3b20 6578 7472 6120 3d3d 2027 6f70 656e  ; extra == 'open
+00001210: 6169 270a 5265 7175 6972 6573 2d44 6973  ai'.Requires-Dis
+00001220: 743a 2074 696b 746f 6b65 6e3b 2065 7874  t: tiktoken; ext
+00001230: 7261 203d 3d20 276f 7065 6e61 6927 0a50  ra == 'openai'.P
+00001240: 726f 7669 6465 732d 4578 7472 613a 206f  rovides-Extra: o
+00001250: 7074 0a52 6571 7569 7265 732d 4469 7374  pt.Requires-Dist
+00001260: 3a20 7472 6974 6f6e 3b20 6578 7472 6120  : triton; extra 
+00001270: 3d3d 2027 6f70 7427 0a50 726f 7669 6465  == 'opt'.Provide
+00001280: 732d 4578 7472 613a 2070 6869 0a52 6571  s-Extra: phi.Req
+00001290: 7569 7265 732d 4469 7374 3a20 7472 6974  uires-Dist: trit
+000012a0: 6f6e 3b20 6578 7472 6120 3d3d 2027 7068  on; extra == 'ph
+000012b0: 6927 0a50 726f 7669 6465 732d 4578 7472  i'.Provides-Extr
+000012c0: 613a 2070 6c61 7967 726f 756e 640a 5265  a: playground.Re
+000012d0: 7175 6972 6573 2d44 6973 743a 2069 7079  quires-Dist: ipy
+000012e0: 7468 6f6e 3b20 6578 7472 6120 3d3d 2027  thon; extra == '
+000012f0: 706c 6179 6772 6f75 6e64 270a 5265 7175  playground'.Requ
+00001300: 6972 6573 2d44 6973 743a 206a 7570 7974  ires-Dist: jupyt
+00001310: 6572 3b20 6578 7472 6120 3d3d 2027 706c  er; extra == 'pl
+00001320: 6179 6772 6f75 6e64 270a 5265 7175 6972  ayground'.Requir
+00001330: 6573 2d44 6973 743a 206a 7570 7974 6578  es-Dist: jupytex
+00001340: 743b 2065 7874 7261 203d 3d20 2770 6c61  t; extra == 'pla
+00001350: 7967 726f 756e 6427 0a52 6571 7569 7265  yground'.Require
+00001360: 732d 4469 7374 3a20 6e62 666f 726d 6174  s-Dist: nbformat
+00001370: 3b20 6578 7472 6120 3d3d 2027 706c 6179  ; extra == 'play
+00001380: 6772 6f75 6e64 270a 5265 7175 6972 6573  ground'.Requires
+00001390: 2d44 6973 743a 206e 6f74 6562 6f6f 6b3b  -Dist: notebook;
+000013a0: 2065 7874 7261 203d 3d20 2770 6c61 7967   extra == 'playg
+000013b0: 726f 756e 6427 0a50 726f 7669 6465 732d  round'.Provides-
+000013c0: 4578 7472 613a 2071 7765 6e0a 5265 7175  Extra: qwen.Requ
+000013d0: 6972 6573 2d44 6973 743a 2063 706d 2d6b  ires-Dist: cpm-k
+000013e0: 6572 6e65 6c73 3b20 6578 7472 6120 3d3d  ernels; extra ==
+000013f0: 2027 7177 656e 270a 5265 7175 6972 6573   'qwen'.Requires
+00001400: 2d44 6973 743a 2074 696b 746f 6b65 6e3b  -Dist: tiktoken;
+00001410: 2065 7874 7261 203d 3d20 2771 7765 6e27   extra == 'qwen'
+00001420: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00001430: 2073 7461 626c 656c 6d0a 5265 7175 6972   stablelm.Requir
+00001440: 6573 2d44 6973 743a 2063 706d 2d6b 6572  es-Dist: cpm-ker
+00001450: 6e65 6c73 3b20 6578 7472 6120 3d3d 2027  nels; extra == '
+00001460: 7374 6162 6c65 6c6d 270a 5265 7175 6972  stablelm'.Requir
+00001470: 6573 2d44 6973 743a 2074 696b 746f 6b65  es-Dist: tiktoke
+00001480: 6e3b 2065 7874 7261 203d 3d20 2773 7461  n; extra == 'sta
+00001490: 626c 656c 6d27 0a50 726f 7669 6465 732d  blelm'.Provides-
+000014a0: 4578 7472 613a 2073 7461 7263 6f64 6572  Extra: starcoder
+000014b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000014c0: 6269 7473 616e 6462 7974 6573 3b20 6578  bitsandbytes; ex
+000014d0: 7472 6120 3d3d 2027 7374 6172 636f 6465  tra == 'starcode
+000014e0: 7227 0a50 726f 7669 6465 732d 4578 7472  r'.Provides-Extr
+000014f0: 613a 2076 6c6c 6d0a 5265 7175 6972 6573  a: vllm.Requires
+00001500: 2d44 6973 743a 2076 6c6c 6d3d 3d30 2e34  -Dist: vllm==0.4
+00001510: 2e32 3b20 6578 7472 6120 3d3d 2027 766c  .2; extra == 'vl
+00001520: 6c6d 270a 5072 6f76 6964 6573 2d45 7874  lm'.Provides-Ext
+00001530: 7261 3a20 7969 0a52 6571 7569 7265 732d  ra: yi.Requires-
+00001540: 4469 7374 3a20 6269 7473 616e 6462 7974  Dist: bitsandbyt
+00001550: 6573 3b20 6578 7472 6120 3d3d 2027 7969  es; extra == 'yi
+00001560: 270a 4465 7363 7269 7074 696f 6e2d 436f  '.Description-Co
+00001570: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00001580: 2f6d 6172 6b64 6f77 6e0a 0a3c 7020 616c  /markdown..<p al
+00001590: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+000015a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000015b0: 2f67 6974 6875 622e 636f 6d2f 6265 6e74  /github.com/bent
+000015c0: 6f6d 6c2f 6f70 656e 6c6c 6d22 3e0a 2020  oml/openllm">.  
+000015d0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000015e0: 733a 2f2f 7261 772e 6769 7468 7562 7573  s://raw.githubus
+000015f0: 6572 636f 6e74 656e 742e 636f 6d2f 6265  ercontent.com/be
+00001600: 6e74 6f6d 6c2f 6f70 656e 6c6c 6d2f 6d61  ntoml/openllm/ma
+00001610: 696e 2f2e 6769 7468 7562 2f61 7373 6574  in/.github/asset
+00001620: 732f 6d61 696e 2d62 616e 6e65 722e 706e  s/main-banner.pn
+00001630: 6722 2061 6c74 3d22 4261 6e6e 6572 2066  g" alt="Banner f
+00001640: 6f72 204f 7065 6e4c 4c4d 2220 2f3e 0a20  or OpenLLM" />. 
+00001650: 203c 2f61 3e0a 3c2f 703e 0a0a 0a3c 6469   </a>.</p>...<di
+00001660: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
+00001670: 3e0a 2020 2020 3c68 3120 616c 6967 6e3d  >.    <h1 align=
+00001680: 2263 656e 7465 7222 3ef0 9fa6 be20 4f70  "center">.... Op
+00001690: 656e 4c4c 4d3a 2053 656c 662d 486f 7374  enLLM: Self-Host
+000016a0: 696e 6720 4c4c 4d73 204d 6164 6520 4561  ing LLMs Made Ea
+000016b0: 7379 3c2f 6831 3e0a 2020 2020 3c61 2068  sy</h1>.    <a h
+000016c0: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+000016d0: 692e 6f72 672f 7072 6f6a 6563 742f 6f70  i.org/project/op
+000016e0: 656e 6c6c 6d22 3e0a 2020 2020 2020 2020  enllm">.        
+000016f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001700: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001710: 2f70 7970 692f 762f 6f70 656e 6c6c 6d2e  /pypi/v/openllm.
+00001720: 7376 673f 6c6f 676f 3d70 7970 6926 6c61  svg?logo=pypi&la
+00001730: 6265 6c3d 5079 5049 266c 6f67 6f43 6f6c  bel=PyPI&logoCol
+00001740: 6f72 3d67 6f6c 6422 2061 6c74 3d22 7079  or=gold" alt="py
+00001750: 7069 5f73 7461 7475 7322 202f 3e0a 2020  pi_status" />.  
+00001760: 2020 3c2f 613e 3c61 2068 7265 663d 2268    </a><a href="h
+00001770: 7474 7073 3a2f 2f74 6573 742e 7079 7069  ttps://test.pypi
+00001780: 2e6f 7267 2f70 726f 6a65 6374 2f6f 7065  .org/project/ope
+00001790: 6e6c 6c6d 2f22 3e0a 2020 2020 2020 2020  nllm/">.        
+000017a0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000017b0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+000017c0: 2f62 6164 6765 2f4e 6967 6874 6c79 2d50  /badge/Nightly-P
+000017d0: 7950 493f 6c6f 676f 3d70 7970 6926 6c61  yPI?logo=pypi&la
+000017e0: 6265 6c3d 5079 5049 2663 6f6c 6f72 3d67  bel=PyPI&color=g
+000017f0: 7261 7926 6c69 6e6b 3d68 7474 7073 2533  ray&link=https%3
+00001800: 4125 3246 2532 4674 6573 742e 7079 7069  A%2F%2Ftest.pypi
+00001810: 2e6f 7267 2532 4670 726f 6a65 6374 2532  .org%2Fproject%2
+00001820: 466f 7065 6e6c 6c6d 2532 4622 2061 6c74  Fopenllm%2F" alt
+00001830: 3d22 7465 7374 5f70 7970 695f 7374 6174  ="test_pypi_stat
+00001840: 7573 2220 2f3e 0a20 2020 203c 2f61 3e3c  us" />.    </a><
+00001850: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001860: 6769 7468 7562 2e63 6f6d 2f62 656e 746f  github.com/bento
+00001870: 6d6c 2f4f 7065 6e4c 4c4d 2f61 6374 696f  ml/OpenLLM/actio
+00001880: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 692e  ns/workflows/ci.
+00001890: 796d 6c22 3e0a 2020 2020 2020 2020 3c69  yml">.        <i
+000018a0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000018b0: 6769 7468 7562 2e63 6f6d 2f62 656e 746f  github.com/bento
+000018c0: 6d6c 2f4f 7065 6e4c 4c4d 2f61 6374 696f  ml/OpenLLM/actio
+000018d0: 6e73 2f77 6f72 6b66 6c6f 7773 2f63 692e  ns/workflows/ci.
+000018e0: 796d 6c2f 6261 6467 652e 7376 673f 6272  yml/badge.svg?br
+000018f0: 616e 6368 3d6d 6169 6e22 2061 6c74 3d22  anch=main" alt="
+00001900: 6369 2220 2f3e 0a20 2020 203c 2f61 3e3c  ci" />.    </a><
+00001910: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001920: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00001930: 6974 2e63 692f 6c61 7465 7374 2f67 6974  it.ci/latest/git
+00001940: 6875 622f 6265 6e74 6f6d 6c2f 4f70 656e  hub/bentoml/Open
+00001950: 4c4c 4d2f 6d61 696e 223e 0a20 2020 2020  LLM/main">.     
+00001960: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
+00001970: 7073 3a2f 2f72 6573 756c 7473 2e70 7265  ps://results.pre
+00001980: 2d63 6f6d 6d69 742e 6369 2f62 6164 6765  -commit.ci/badge
+00001990: 2f67 6974 6875 622f 6265 6e74 6f6d 6c2f  /github/bentoml/
+000019a0: 4f70 656e 4c4c 4d2f 6d61 696e 2e73 7667  OpenLLM/main.svg
+000019b0: 2220 616c 743d 2270 7265 2d63 6f6d 6d69  " alt="pre-commi
+000019c0: 742e 6369 2073 7461 7475 7322 202f 3e0a  t.ci status" />.
+000019d0: 2020 2020 3c2f 613e 3c62 723e 3c61 2068      </a><br><a h
+000019e0: 7265 663d 2268 7474 7073 3a2f 2f74 7769  ref="https://twi
+000019f0: 7474 6572 2e63 6f6d 2f62 656e 746f 6d6c  tter.com/bentoml
+00001a00: 6169 223e 0a20 2020 2020 2020 203c 696d  ai">.        <im
+00001a10: 6720 7372 633d 2268 7474 7073 3a2f 2f62  g src="https://b
+00001a20: 6164 6765 6e2e 6e65 742f 6261 6467 652f  adgen.net/badge/
+00001a30: 6963 6f6e 2f40 6265 6e74 6f6d 6c61 692f  icon/@bentomlai/
+00001a40: 3144 4131 4632 3f69 636f 6e3d 7477 6974  1DA1F2?icon=twit
+00001a50: 7465 7226 6c61 6265 6c3d 466f 6c6c 6f77  ter&label=Follow
+00001a60: 2532 3055 7322 2061 6c74 3d22 5477 6974  %20Us" alt="Twit
+00001a70: 7465 7222 202f 3e0a 2020 2020 3c2f 613e  ter" />.    </a>
+00001a80: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001a90: 2f6c 2e62 656e 746f 6d6c 2e63 6f6d 2f6a  /l.bentoml.com/j
+00001aa0: 6f69 6e2d 6f70 656e 6c6c 6d2d 6469 7363  oin-openllm-disc
+00001ab0: 6f72 6422 3e0a 2020 2020 2020 2020 3c69  ord">.        <i
+00001ac0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00001ad0: 6261 6467 656e 2e6e 6574 2f62 6164 6765  badgen.net/badge
+00001ae0: 2f69 636f 6e2f 4f70 656e 4c4c 4d2f 3732  /icon/OpenLLM/72
+00001af0: 3839 6461 3f69 636f 6e3d 6469 7363 6f72  89da?icon=discor
+00001b00: 6426 6c61 6265 6c3d 4a6f 696e 2532 3055  d&label=Join%20U
+00001b10: 7322 2061 6c74 3d22 4469 7363 6f72 6422  s" alt="Discord"
+00001b20: 202f 3e0a 2020 2020 3c2f 613e 0a3c 2f64   />.    </a>.</d
+00001b30: 6976 3e0a 0a23 2320 f09f 9396 2049 6e74  iv>..## .... Int
+00001b40: 726f 6475 6374 696f 6e0a 0a4f 7065 6e4c  roduction..OpenL
+00001b50: 4c4d 2068 656c 7073 2064 6576 656c 6f70  LM helps develop
+00001b60: 6572 7320 2a2a 7275 6e20 616e 7920 6f70  ers **run any op
+00001b70: 656e 2d73 6f75 7263 6520 4c4c 4d73 2a2a  en-source LLMs**
+00001b80: 2c20 7375 6368 2061 7320 4c6c 616d 6120  , such as Llama 
+00001b90: 3220 616e 6420 4d69 7374 7261 6c2c 2061  2 and Mistral, a
+00001ba0: 7320 2a2a 4f70 656e 4149 2d63 6f6d 7061  s **OpenAI-compa
+00001bb0: 7469 626c 6520 4150 4920 656e 6470 6f69  tible API endpoi
+00001bc0: 6e74 732a 2a2c 206c 6f63 616c 6c79 2061  nts**, locally a
+00001bd0: 6e64 2069 6e20 7468 6520 636c 6f75 642c  nd in the cloud,
+00001be0: 206f 7074 696d 697a 6564 2066 6f72 2073   optimized for s
+00001bf0: 6572 7669 6e67 2074 6872 6f75 6768 7075  erving throughpu
+00001c00: 7420 616e 6420 7072 6f64 7563 7469 6f6e  t and production
+00001c10: 2064 6570 6c6f 796d 656e 742e 0a0a 0a2d   deployment....-
+00001c20: 20f0 9f9a 8220 5375 7070 6f72 7420 6120   .... Support a 
+00001c30: 7769 6465 2072 616e 6765 206f 6620 6f70  wide range of op
+00001c40: 656e 2d73 6f75 7263 6520 4c4c 4d73 2069  en-source LLMs i
+00001c50: 6e63 6c75 6469 6e67 204c 4c4d 7320 6669  ncluding LLMs fi
+00001c60: 6e65 2d74 756e 6564 2077 6974 6820 796f  ne-tuned with yo
+00001c70: 7572 206f 776e 2064 6174 610a 2d20 e29b  ur own data.- ..
+00001c80: 93ef b88f 204f 7065 6e41 4920 636f 6d70  .... OpenAI comp
+00001c90: 6174 6962 6c65 2041 5049 2065 6e64 706f  atible API endpo
+00001ca0: 696e 7473 2066 6f72 2073 6561 6d6c 6573  ints for seamles
+00001cb0: 7320 7472 616e 7369 7469 6f6e 2066 726f  s transition fro
+00001cc0: 6d20 796f 7572 204c 4c4d 2061 7070 2074  m your LLM app t
+00001cd0: 6f20 6f70 656e 2d73 6f75 7263 6520 4c4c  o open-source LL
+00001ce0: 4d73 0a2d 20f0 9f94 a520 5374 6174 652d  Ms.- .... State-
+00001cf0: 6f66 2d74 6865 2d61 7274 2073 6572 7669  of-the-art servi
+00001d00: 6e67 2061 6e64 2069 6e66 6572 656e 6365  ng and inference
+00001d10: 2070 6572 666f 726d 616e 6365 0a2d 20f0   performance.- .
+00001d20: 9f8e af20 5369 6d70 6c69 6669 6564 2063  ... Simplified c
+00001d30: 6c6f 7564 2064 6570 6c6f 796d 656e 7420  loud deployment 
+00001d40: 7669 6120 5b42 656e 746f 4d4c 5d28 7777  via [BentoML](ww
+00001d50: 772e 6265 6e74 6f6d 6c2e 636f 6d29 0a0a  w.bentoml.com)..
+00001d60: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+00001d70: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
+00001d80: 6874 7470 733a 2f2f 7261 772e 6769 7468  https://raw.gith
+00001d90: 7562 7573 6572 636f 6e74 656e 742e 636f  ubusercontent.co
+00001da0: 6d2f 6265 6e74 6f6d 6c2f 6f70 656e 6c6c  m/bentoml/openll
+00001db0: 6d2f 6d61 696e 2f2e 6769 7468 7562 2f61  m/main/.github/a
+00001dc0: 7373 6574 732f 6f75 7470 7574 2e67 6966  ssets/output.gif
+00001dd0: 2220 616c 743d 2247 6966 2073 686f 7769  " alt="Gif showi
+00001de0: 6e67 204f 7065 6e4c 4c4d 2049 6e74 726f  ng OpenLLM Intro
+00001df0: 2220 2f3e 0a3c 2f70 3e0a 0a23 2320 f09f  " />.</p>..## ..
+00001e00: 92be 2054 4c2f 4452 0a0a 466f 7220 7374  .. TL/DR..For st
+00001e10: 6172 7465 722c 2077 6520 7072 6f76 6964  arter, we provid
+00001e20: 6520 7477 6f20 7761 7973 2074 6f20 7175  e two ways to qu
+00001e30: 6963 6b6c 7920 7472 7920 6f75 7420 4f70  ickly try out Op
+00001e40: 656e 4c4c 4d3a 0a0a 2323 2320 4a75 7079  enLLM:..### Jupy
+00001e50: 7465 7220 4e6f 7465 626f 6f6b 730a 0a54  ter Notebooks..T
+00001e60: 7279 2074 6869 7320 5b4f 7065 6e4c 4c4d  ry this [OpenLLM
+00001e70: 2074 7574 6f72 6961 6c20 696e 2047 6f6f   tutorial in Goo
+00001e80: 676c 6520 436f 6c61 623a 2053 6572 7669  gle Colab: Servi
+00001e90: 6e67 204c 6c61 6d61 2032 2077 6974 6820  ng Llama 2 with 
+00001ea0: 4f70 656e 4c4c 4d5d 2868 7474 7073 3a2f  OpenLLM](https:/
+00001eb0: 2f63 6f6c 6162 2e72 6573 6561 7263 682e  /colab.research.
+00001ec0: 676f 6f67 6c65 2e63 6f6d 2f67 6974 6875  google.com/githu
+00001ed0: 622f 6265 6e74 6f6d 6c2f 4f70 656e 4c4c  b/bentoml/OpenLL
+00001ee0: 4d2f 626c 6f62 2f6d 6169 6e2f 6578 616d  M/blob/main/exam
+00001ef0: 706c 6573 2f6c 6c61 6d61 322e 6970 796e  ples/llama2.ipyn
+00001f00: 6229 2e0a 0a23 2323 2044 6f63 6b65 720a  b)...### Docker.
+00001f10: 0a57 6520 7072 6f76 6964 6520 6120 646f  .We provide a do
+00001f20: 636b 6572 2063 6f6e 7461 696e 6572 2074  cker container t
+00001f30: 6861 7420 6865 6c70 7320 796f 7520 7374  hat helps you st
+00001f40: 6172 7420 7275 6e6e 696e 6720 4f70 656e  art running Open
+00001f50: 4c4c 4d3a 0a0a 6060 6062 6173 680a 646f  LLM:..```bash.do
+00001f60: 636b 6572 2072 756e 202d 2d72 6d20 2d69  cker run --rm -i
+00001f70: 7420 2d70 2033 3030 303a 3330 3030 2067  t -p 3000:3000 g
+00001f80: 6863 722e 696f 2f62 656e 746f 6d6c 2f6f  hcr.io/bentoml/o
+00001f90: 7065 6e6c 6c6d 2073 7461 7274 2066 6163  penllm start fac
+00001fa0: 6562 6f6f 6b2f 6f70 742d 312e 3362 202d  ebook/opt-1.3b -
+00001fb0: 2d62 6163 6b65 6e64 2070 740a 6060 600a  -backend pt.```.
+00001fc0: 0a3e 205b 214e 4f54 455d 0a3e 2047 6976  .> [!NOTE].> Giv
+00001fd0: 656e 2079 6f75 2068 6176 6520 6163 6365  en you have acce
+00001fe0: 7373 2074 6f20 4750 5573 2061 6e64 2068  ss to GPUs and h
+00001ff0: 6176 6520 7365 7475 7020 5b6e 7669 6469  ave setup [nvidi
+00002000: 612d 646f 636b 6572 5d28 6874 7470 733a  a-docker](https:
+00002010: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 5649  //github.com/NVI
+00002020: 4449 412f 6e76 6964 6961 2d63 6f6e 7461  DIA/nvidia-conta
+00002030: 696e 6572 2d74 6f6f 6c6b 6974 292c 2020  iner-toolkit),  
+00002040: 796f 7520 6361 6e20 6164 6469 7469 6f6e  you can addition
+00002050: 616c 6c79 2070 6173 7320 696e 2060 2d2d  ally pass in `--
+00002060: 6770 7573 600a 3e20 746f 2075 7365 2047  gpus`.> to use G
+00002070: 5055 2066 6f72 2066 6173 7465 7220 696e  PU for faster in
+00002080: 6665 7265 6e63 6520 616e 6420 6f70 7469  ference and opti
+00002090: 6d69 7a61 7469 6f6e 0a3e 6060 6062 6173  mization.>```bas
+000020a0: 680a 3e20 646f 636b 6572 2072 756e 202d  h.> docker run -
+000020b0: 2d72 6d20 2d2d 6770 7573 2061 6c6c 202d  -rm --gpus all -
+000020c0: 7020 3330 3030 3a33 3030 3020 2d69 7420  p 3000:3000 -it 
+000020d0: 6768 6372 2e69 6f2f 6265 6e74 6f6d 6c2f  ghcr.io/bentoml/
+000020e0: 6f70 656e 6c6c 6d20 7374 6172 7420 4875  openllm start Hu
+000020f0: 6767 696e 6746 6163 6548 342f 7a65 7068  ggingFaceH4/zeph
+00002100: 7972 2d37 622d 6265 7461 202d 2d62 6163  yr-7b-beta --bac
+00002110: 6b65 6e64 2076 6c6c 6d0a 3e20 6060 600a  kend vllm.> ```.
+00002120: 0a0a 2323 20f0 9f8f 8320 4765 7420 7374  ..## .... Get st
+00002130: 6172 7465 640a 0a54 6865 2066 6f6c 6c6f  arted..The follo
+00002140: 7769 6e67 2070 726f 7669 6465 7320 696e  wing provides in
+00002150: 7374 7275 6374 696f 6e73 2066 6f72 2068  structions for h
+00002160: 6f77 2074 6f20 6765 7420 7374 6172 7465  ow to get starte
+00002170: 6420 7769 7468 204f 7065 6e4c 4c4d 206c  d with OpenLLM l
+00002180: 6f63 616c 6c79 2e0a 0a23 2323 2050 7265  ocally...### Pre
+00002190: 7265 7175 6973 6974 6573 0a0a 596f 7520  requisites..You 
+000021a0: 6861 7665 2069 6e73 7461 6c6c 6564 2050  have installed P
+000021b0: 7974 686f 6e20 332e 3820 286f 7220 6c61  ython 3.8 (or la
+000021c0: 7465 7229 2061 6e64 c2a0 6070 6970 602e  ter) and..`pip`.
+000021d0: 2057 6520 6869 6768 6c79 2072 6563 6f6d   We highly recom
+000021e0: 6d65 6e64 2075 7369 6e67 2061 205b 5669  mend using a [Vi
+000021f0: 7274 7561 6c20 456e 7669 726f 6e6d 656e  rtual Environmen
+00002200: 745d 2868 7474 7073 3a2f 2f64 6f63 732e  t](https://docs.
+00002210: 7079 7468 6f6e 2e6f 7267 2f33 2f6c 6962  python.org/3/lib
+00002220: 7261 7279 2f76 656e 762e 6874 6d6c 2920  rary/venv.html) 
+00002230: 746f 2070 7265 7665 6e74 2070 6163 6b61  to prevent packa
+00002240: 6765 2063 6f6e 666c 6963 7473 2e0a 0a23  ge conflicts...#
+00002250: 2323 2049 6e73 7461 6c6c 204f 7065 6e4c  ## Install OpenL
+00002260: 4c4d 0a0a 496e 7374 616c 6c20 4f70 656e  LM..Install Open
+00002270: 4c4c 4d20 6279 2075 7369 6e67 2060 7069  LLM by using `pi
+00002280: 7060 2061 7320 666f 6c6c 6f77 733a 0a0a  p` as follows:..
+00002290: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
+000022a0: 616c 6c20 6f70 656e 6c6c 6d0a 6060 600a  all openllm.```.
+000022b0: 0a54 6f20 7665 7269 6679 2074 6865 2069  .To verify the i
+000022c0: 6e73 7461 6c6c 6174 696f 6e2c 2072 756e  nstallation, run
+000022d0: 3a0a 0a60 6060 6261 7368 0a24 206f 7065  :..```bash.$ ope
+000022e0: 6e6c 6c6d 202d 680a 0a55 7361 6765 3a20  nllm -h..Usage: 
+000022f0: 6f70 656e 6c6c 6d20 5b4f 5054 494f 4e53  openllm [OPTIONS
+00002300: 5d20 434f 4d4d 414e 4420 5b41 5247 535d  ] COMMAND [ARGS]
+00002310: 2e2e 2e0a 0a20 2020 e296 88e2 9688 e296  .....   ........
+00002320: 88e2 9688 e296 88e2 9688 e295 9720 e296  ............. ..
+00002330: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
+00002340: e295 9720 e296 88e2 9688 e296 88e2 9688  ... ............
+00002350: e296 88e2 9688 e296 88e2 9597 e296 88e2  ................
+00002360: 9688 e296 88e2 9597 2020 20e2 9688 e296  ........   .....
+00002370: 88e2 9597 e296 88e2 9688 e295 9720 2020  .............   
+00002380: 2020 e296 88e2 9688 e295 9720 2020 2020    .........     
+00002390: e296 88e2 9688 e296 88e2 9597 2020 20e2  ............   .
+000023a0: 9688 e296 88e2 9688 e295 970a 2020 e296  ............  ..
+000023b0: 88e2 9688 e295 94e2 9590 e295 90e2 9590  ................
+000023c0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+000023d0: 9594 e295 90e2 9590 e296 88e2 9688 e295  ................
+000023e0: 97e2 9688 e296 88e2 9594 e295 90e2 9590  ................
+000023f0: e295 90e2 9590 e295 9de2 9688 e296 88e2  ................
+00002400: 9688 e296 88e2 9597 2020 e296 88e2 9688  ........  ......
+00002410: e295 91e2 9688 e296 88e2 9591 2020 2020  ............    
+00002420: 20e2 9688 e296 88e2 9591 2020 2020 20e2   .........     .
+00002430: 9688 e296 88e2 9688 e296 88e2 9597 20e2  .............. .
+00002440: 9688 e296 88e2 9688 e296 88e2 9591 0a20  ............... 
+00002450: 20e2 9688 e296 88e2 9591 2020 20e2 9688   .........   ...
+00002460: e296 88e2 9591 e296 88e2 9688 e296 88e2  ................
+00002470: 9688 e296 88e2 9688 e295 94e2 959d e296  ................
+00002480: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
+00002490: 2020 e296 88e2 9688 e295 94e2 9688 e296    ..............
+000024a0: 88e2 9597 20e2 9688 e296 88e2 9591 e296  .... ...........
+000024b0: 88e2 9688 e295 9120 2020 2020 e296 88e2  .......     ....
+000024c0: 9688 e295 9120 2020 2020 e296 88e2 9688  .....     ......
+000024d0: e295 94e2 9688 e296 88e2 9688 e296 88e2  ................
+000024e0: 9594 e296 88e2 9688 e295 910a 2020 e296  ............  ..
+000024f0: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
+00002500: e295 91e2 9688 e296 88e2 9594 e295 90e2  ................
+00002510: 9590 e295 90e2 959d 20e2 9688 e296 88e2  ........ .......
+00002520: 9594 e295 90e2 9590 e295 9d20 20e2 9688  ...........  ...
+00002530: e296 88e2 9591 e295 9ae2 9688 e296 88e2  ................
+00002540: 9597 e296 88e2 9688 e295 91e2 9688 e296  ................
+00002550: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
+00002560: 9591 2020 2020 20e2 9688 e296 88e2 9591  ..     .........
+00002570: e295 9ae2 9688 e296 88e2 9594 e295 9de2  ................
+00002580: 9688 e296 88e2 9591 0a20 20e2 959a e296  .........  .....
+00002590: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
+000025a0: e295 94e2 959d e296 88e2 9688 e295 9120  ............... 
+000025b0: 2020 2020 e296 88e2 9688 e296 88e2 9688      ............
+000025c0: e296 88e2 9688 e296 88e2 9597 e296 88e2  ................
+000025d0: 9688 e295 9120 e295 9ae2 9688 e296 88e2  ..... ..........
+000025e0: 9688 e296 88e2 9591 e296 88e2 9688 e296  ................
+000025f0: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
+00002600: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00002610: 9688 e296 88e2 9597 e296 88e2 9688 e295  ................
+00002620: 9120 e295 9ae2 9590 e295 9d20 e296 88e2  . ......... ....
+00002630: 9688 e295 910a 2020 20e2 959a e295 90e2  ......   .......
+00002640: 9590 e295 90e2 9590 e295 90e2 959d 20e2  .............. .
+00002650: 959a e295 90e2 959d 2020 2020 20e2 959a  ........     ...
+00002660: e295 90e2 9590 e295 90e2 9590 e295 90e2  ................
+00002670: 9590 e295 9de2 959a e295 90e2 959d 2020  ..............  
+00002680: e295 9ae2 9590 e295 90e2 9590 e295 9de2  ................
+00002690: 959a e295 90e2 9590 e295 90e2 9590 e295  ................
+000026a0: 90e2 9590 e295 9de2 959a e295 90e2 9590  ................
+000026b0: e295 90e2 9590 e295 90e2 9590 e295 9de2  ................
+000026c0: 959a e295 90e2 959d 2020 2020 20e2 959a  ........     ...
+000026d0: e295 90e2 959d 2e0a 0a20 2041 6e20 6f70  .........  An op
+000026e0: 656e 2070 6c61 7466 6f72 6d20 666f 7220  en platform for 
+000026f0: 6f70 6572 6174 696e 6720 6c61 7267 6520  operating large 
+00002700: 6c61 6e67 7561 6765 206d 6f64 656c 7320  language models 
+00002710: 696e 2070 726f 6475 6374 696f 6e2e 0a20  in production.. 
+00002720: 2046 696e 652d 7475 6e65 2c20 7365 7276   Fine-tune, serv
+00002730: 652c 2064 6570 6c6f 792c 2061 6e64 206d  e, deploy, and m
+00002740: 6f6e 6974 6f72 2061 6e79 204c 4c4d 7320  onitor any LLMs 
+00002750: 7769 7468 2065 6173 652e 0a0a 4f70 7469  with ease...Opti
+00002760: 6f6e 733a 0a20 202d 762c 202d 2d76 6572  ons:.  -v, --ver
+00002770: 7369 6f6e 2020 5368 6f77 2074 6865 2076  sion  Show the v
+00002780: 6572 7369 6f6e 2061 6e64 2065 7869 742e  ersion and exit.
+00002790: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
+000027a0: 2020 5368 6f77 2074 6869 7320 6d65 7373    Show this mess
+000027b0: 6167 6520 616e 6420 6578 6974 2e0a 0a43  age and exit...C
+000027c0: 6f6d 6d61 6e64 733a 0a20 2062 7569 6c64  ommands:.  build
+000027d0: 2020 2020 2020 2050 6163 6b61 6765 2061         Package a
+000027e0: 2067 6976 656e 206d 6f64 656c 7320 696e   given models in
+000027f0: 746f 2061 2042 656e 746f 4c4c 4d2e 0a20  to a BentoLLM.. 
+00002800: 2069 6d70 6f72 7420 2020 2020 2053 6574   import      Set
+00002810: 7570 204c 4c4d 2069 6e74 6572 6163 7469  up LLM interacti
+00002820: 7665 6c79 2e0a 2020 6d6f 6465 6c73 2020  vely..  models  
+00002830: 2020 2020 4c69 7374 2061 6c6c 2073 7570      List all sup
+00002840: 706f 7274 6564 206d 6f64 656c 732e 0a20  ported models.. 
+00002850: 2070 7275 6e65 2020 2020 2020 2052 656d   prune       Rem
+00002860: 6f76 6520 616c 6c20 7361 7665 6420 6d6f  ove all saved mo
+00002870: 6465 6c73 2c20 2861 6e64 206f 7074 696f  dels, (and optio
+00002880: 6e61 6c6c 7920 6265 6e74 6f73 2920 6275  nally bentos) bu
+00002890: 696c 7420 7769 7468 204f 7065 6e4c 4c4d  ilt with OpenLLM
+000028a0: 206c 6f63 616c 6c79 2e0a 2020 7175 6572   locally..  quer
+000028b0: 7920 2020 2020 2020 5175 6572 7920 6120  y       Query a 
+000028c0: 4c4c 4d20 696e 7465 7261 6374 6976 656c  LLM interactivel
+000028d0: 792c 2066 726f 6d20 6120 7465 726d 696e  y, from a termin
+000028e0: 616c 2e0a 2020 7374 6172 7420 2020 2020  al..  start     
+000028f0: 2020 5374 6172 7420 6120 4c4c 4d53 6572    Start a LLMSer
+00002900: 7665 7220 666f 7220 616e 7920 7375 7070  ver for any supp
+00002910: 6f72 7465 6420 4c4c 4d2e 0a0a 4578 7465  orted LLM...Exte
+00002920: 6e73 696f 6e73 3a0a 2020 6275 696c 642d  nsions:.  build-
+00002930: 6261 7365 2d63 6f6e 7461 696e 6572 2020  base-container  
+00002940: 4261 7365 2069 6d61 6765 2062 7569 6c64  Base image build
+00002950: 6572 2066 6f72 2042 656e 746f 4c4c 4d2e  er for BentoLLM.
+00002960: 0a20 2064 6976 652d 6265 6e74 6f73 2020  .  dive-bentos  
+00002970: 2020 2020 2020 2020 2044 6976 6520 696e           Dive in
+00002980: 746f 2061 2042 656e 746f 4c4c 4d2e 0a20  to a BentoLLM.. 
+00002990: 2067 6574 2d63 6f6e 7461 696e 6572 6669   get-containerfi
+000029a0: 6c65 2020 2020 2052 6574 7572 6e20 436f  le     Return Co
+000029b0: 6e74 6169 6e65 7266 696c 6520 6f66 2061  ntainerfile of a
+000029c0: 6e79 2067 6976 656e 2042 656e 746f 2e0a  ny given Bento..
+000029d0: 2020 6765 742d 7072 6f6d 7074 2020 2020    get-prompt    
+000029e0: 2020 2020 2020 2020 4765 7420 7468 6520          Get the 
+000029f0: 6465 6661 756c 7420 7072 6f6d 7074 2075  default prompt u
+00002a00: 7365 6420 6279 204f 7065 6e4c 4c4d 2e0a  sed by OpenLLM..
+00002a10: 2020 6c69 7374 2d62 656e 746f 7320 2020    list-bentos   
+00002a20: 2020 2020 2020 2020 4c69 7374 2061 7661          List ava
+00002a30: 696c 6162 6c65 2062 656e 746f 7320 6275  ilable bentos bu
+00002a40: 696c 7420 6279 204f 7065 6e4c 4c4d 2e0a  ilt by OpenLLM..
+00002a50: 2020 6c69 7374 2d6d 6f64 656c 7320 2020    list-models   
+00002a60: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00002a70: 6571 7569 7661 6c65 6e74 2074 6f20 6f70  equivalent to op
+00002a80: 656e 6c6c 6d20 6d6f 6465 6c73 2e2e 2e0a  enllm models....
+00002a90: 2020 706c 6179 6772 6f75 6e64 2020 2020    playground    
+00002aa0: 2020 2020 2020 2020 4f70 656e 4c4c 4d20          OpenLLM 
+00002ab0: 506c 6179 6772 6f75 6e64 2e0a 6060 600a  Playground..```.
+00002ac0: 0a23 2323 2053 7461 7274 2061 204c 4c4d  .### Start a LLM
+00002ad0: 2073 6572 7665 720a 0a4f 7065 6e4c 4c4d   server..OpenLLM
+00002ae0: 2061 6c6c 6f77 7320 796f 7520 746f 2071   allows you to q
+00002af0: 7569 636b 6c79 2073 7069 6e20 7570 2061  uickly spin up a
+00002b00: 6e20 4c4c 4d20 7365 7276 6572 2075 7369  n LLM server usi
+00002b10: 6e67 2060 6f70 656e 6c6c 6d20 7374 6172  ng `openllm star
+00002b20: 7460 2e20 466f 7220 6578 616d 706c 652c  t`. For example,
+00002b30: 2074 6f20 7374 6172 7420 61c2 a05b 7068   to start a..[ph
+00002b40: 692d 325d 2868 7474 7073 3a2f 2f68 7567  i-2](https://hug
+00002b50: 6769 6e67 6661 6365 2e63 6f2f 6d69 6372  gingface.co/micr
+00002b60: 6f73 6f66 742f 7068 692d 3229 c2a0 7365  osoft/phi-2)..se
+00002b70: 7276 6572 2c20 7275 6e20 7468 6520 666f  rver, run the fo
+00002b80: 6c6c 6f77 696e 673a 0a0a 6060 6062 6173  llowing:..```bas
+00002b90: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
+00002ba0: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
+00002bb0: 2073 7461 7274 206d 6963 726f 736f 6674   start microsoft
+00002bc0: 2f70 6869 2d32 0a60 6060 0a0a 5468 6973  /phi-2.```..This
+00002bd0: 2073 7461 7274 7320 7468 6520 7365 7276   starts the serv
+00002be0: 6572 2061 74c2 a05b 6874 7470 3a2f 2f30  er at..[http://0
+00002bf0: 2e30 2e30 2e30 3a33 3030 302f 5d28 6874  .0.0.0:3000/](ht
+00002c00: 7470 3a2f 2f30 2e30 2e30 2e30 3a33 3030  tp://0.0.0.0:300
+00002c10: 302f 292e 204f 7065 6e4c 4c4d 2064 6f77  0/). OpenLLM dow
+00002c20: 6e6c 6f61 6473 2074 6865 206d 6f64 656c  nloads the model
+00002c30: 2074 6f20 7468 6520 4265 6e74 6f4d 4c20   to the BentoML 
+00002c40: 6c6f 6361 6c20 4d6f 6465 6c20 5374 6f72  local Model Stor
+00002c50: 6520 6966 2069 7420 6861 7320 6e6f 7420  e if it has not 
+00002c60: 6265 656e 2072 6567 6973 7465 7265 6420  been registered 
+00002c70: 6265 666f 7265 2e20 546f 2076 6965 7720  before. To view 
+00002c80: 796f 7572 206c 6f63 616c 206d 6f64 656c  your local model
+00002c90: 732c 2072 756e 2060 6265 6e74 6f6d 6c20  s, run `bentoml 
+00002ca0: 6d6f 6465 6c73 206c 6973 7460 2e0a 0a54  models list`...T
+00002cb0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00002cc0: 7468 6520 7365 7276 6572 2c20 796f 7520  the server, you 
+00002cd0: 6361 6e20 7669 7369 7420 7468 6520 7765  can visit the we
+00002ce0: 6220 5549 2061 74c2 a05b 6874 7470 3a2f  b UI at..[http:/
+00002cf0: 2f30 2e30 2e30 2e30 3a33 3030 302f 5d28  /0.0.0.0:3000/](
+00002d00: 6874 7470 3a2f 2f30 2e30 2e30 2e30 3a33  http://0.0.0.0:3
+00002d10: 3030 302f 2920 6f72 2073 656e 6420 6120  000/) or send a 
+00002d20: 7265 7175 6573 7420 7573 696e 67c2 a060  request using..`
+00002d30: 6375 726c 602e 2059 6f75 2063 616e 2061  curl`. You can a
+00002d40: 6c73 6f20 7573 6520 4f70 656e 4c4c 4de2  lso use OpenLLM.
+00002d50: 8099 7320 6275 696c 742d 696e 2050 7974  ..s built-in Pyt
+00002d60: 686f 6e20 636c 6965 6e74 2074 6f20 696e  hon client to in
+00002d70: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
+00002d80: 7365 7276 6572 3a0a 0a60 6060 7079 7468  server:..```pyth
+00002d90: 6f6e 0a69 6d70 6f72 7420 6f70 656e 6c6c  on.import openll
+00002da0: 6d0a 0a63 6c69 656e 7420 3d20 6f70 656e  m..client = open
+00002db0: 6c6c 6d2e 636c 6965 6e74 2e48 5454 5043  llm.client.HTTPC
+00002dc0: 6c69 656e 7428 2768 7474 703a 2f2f 6c6f  lient('http://lo
+00002dd0: 6361 6c68 6f73 743a 3330 3030 2729 0a63  calhost:3000').c
+00002de0: 6c69 656e 742e 7175 6572 7928 2745 7870  lient.query('Exp
+00002df0: 6c61 696e 2074 6f20 6d65 2074 6865 2064  lain to me the d
+00002e00: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+00002e10: 6e20 2266 7572 7468 6572 2220 616e 6420  n "further" and 
+00002e20: 2266 6172 7468 6572 2227 290a 6060 600a  "farther"').```.
+00002e30: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+00002e40: 7573 6520 7468 65c2 a060 6f70 656e 6c6c  use the..`openll
+00002e50: 6d20 7175 6572 7960 c2a0 636f 6d6d 616e  m query`..comman
+00002e60: 6420 746f 2071 7565 7279 2074 6865 206d  d to query the m
+00002e70: 6f64 656c 3a0a 0a60 6060 6261 7368 0a65  odel:..```bash.e
+00002e80: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
+00002e90: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
+00002ea0: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
+00002eb0: 6e6c 6c6d 2071 7565 7279 2027 4578 706c  nllm query 'Expl
+00002ec0: 6169 6e20 746f 206d 6520 7468 6520 6469  ain to me the di
+00002ed0: 6666 6572 656e 6365 2062 6574 7765 656e  fference between
+00002ee0: 2022 6675 7274 6865 7222 2061 6e64 2022   "further" and "
+00002ef0: 6661 7274 6865 7222 270a 6060 600a 0a4f  farther"'.```..O
+00002f00: 7065 6e4c 4c4d 2073 6561 6d6c 6573 736c  penLLM seamlessl
+00002f10: 7920 7375 7070 6f72 7473 206d 616e 7920  y supports many 
+00002f20: 6d6f 6465 6c73 2061 6e64 2074 6865 6972  models and their
+00002f30: 2076 6172 6961 6e74 732e 2059 6f75 2063   variants. You c
+00002f40: 616e 2073 7065 6369 6679 2064 6966 6665  an specify diffe
+00002f50: 7265 6e74 2076 6172 6961 6e74 7320 6f66  rent variants of
+00002f60: 2074 6865 206d 6f64 656c 2074 6f20 6265   the model to be
+00002f70: 2073 6572 7665 642e 2046 6f72 2065 7861   served. For exa
+00002f80: 6d70 6c65 3a0a 0a60 6060 6261 7368 0a6f  mple:..```bash.o
+00002f90: 7065 6e6c 6c6d 2073 7461 7274 203c 6d6f  penllm start <mo
+00002fa0: 6465 6c5f 6964 3e20 2d2d 3c6f 7074 696f  del_id> --<optio
+00002fb0: 6e73 3e0a 6060 600a 0a3e 205b 214e 4f54  ns>.```..> [!NOT
+00002fc0: 455d 0a3e 204f 7065 6e4c 4c4d 2073 7570  E].> OpenLLM sup
+00002fd0: 706f 7274 7320 7370 6563 6966 7969 6e67  ports specifying
+00002fe0: 2066 696e 652d 7475 6e69 6e67 2077 6569   fine-tuning wei
+00002ff0: 6768 7473 2061 6e64 2071 7561 6e74 697a  ghts and quantiz
+00003000: 6564 2077 6569 6768 7473 0a3e 2066 6f72  ed weights.> for
+00003010: 2061 6e79 206f 6620 7468 6520 7375 7070   any of the supp
+00003020: 6f72 7465 6420 6d6f 6465 6c73 2061 7320  orted models as 
+00003030: 6c6f 6e67 2061 7320 7468 6579 2063 616e  long as they can
+00003040: 2062 6520 6c6f 6164 6564 2077 6974 6820   be loaded with 
+00003050: 7468 6520 6d6f 6465 6c0a 3e20 6172 6368  the model.> arch
+00003060: 6974 6563 7475 7265 2e20 5573 6520 7468  itecture. Use th
+00003070: 65c2 a060 6f70 656e 6c6c 6d20 6d6f 6465  e..`openllm mode
+00003080: 6c73 60c2 a063 6f6d 6d61 6e64 2074 6f20  ls`..command to 
+00003090: 7365 6520 7468 6520 636f 6d70 6c65 7465  see the complete
+000030a0: 206c 6973 7420 6f66 2073 7570 706f 7274   list of support
+000030b0: 6564 0a3e 206d 6f64 656c 732c 2074 6865  ed.> models, the
+000030c0: 6972 2061 7263 6869 7465 6374 7572 6573  ir architectures
+000030d0: 2c20 616e 6420 7468 6569 7220 7661 7269  , and their vari
+000030e0: 616e 7473 2e0a 0a3e 205b 2149 4d50 4f52  ants...> [!IMPOR
+000030f0: 5441 4e54 5d0a 3e20 4966 2079 6f75 2061  TANT].> If you a
+00003100: 7265 2074 6573 7469 6e67 204f 7065 6e4c  re testing OpenL
+00003110: 4c4d 206f 6e20 4350 552c 2079 6f75 206d  LM on CPU, you m
+00003120: 6967 6874 2077 616e 7420 746f 2070 6173  ight want to pas
+00003130: 7320 696e 2060 4454 5950 453d 666c 6f61  s in `DTYPE=floa
+00003140: 7433 3260 2e20 4279 2064 6566 6175 6c74  t32`. By default
+00003150: 2c0a 3e20 4f70 656e 4c4c 4d20 7769 6c6c  ,.> OpenLLM will
+00003160: 2073 6574 206d 6f64 656c 2060 6474 7970   set model `dtyp
+00003170: 6560 2074 6f20 6062 666c 6f61 7431 3660  e` to `bfloat16`
+00003180: 2066 6f72 2074 6865 2062 6573 7420 7065   for the best pe
+00003190: 7266 6f72 6d61 6e63 652e 0a3e 2060 6060  rformance..> ```
+000031a0: 6261 7368 0a3e 2044 5459 5045 3d66 6c6f  bash.> DTYPE=flo
+000031b0: 6174 3332 206f 7065 6e6c 6c6d 2073 7461  at32 openllm sta
+000031c0: 7274 206d 6963 726f 736f 6674 2f70 6869  rt microsoft/phi
+000031d0: 2d32 0a3e 2060 6060 0a3e 2054 6869 7320  -2.> ```.> This 
+000031e0: 7769 6c6c 2061 6c73 6f20 6170 706c 6965  will also applie
+000031f0: 7320 746f 206f 6c64 6572 2047 5055 732e  s to older GPUs.
+00003200: 2049 6620 796f 7572 2047 5055 7320 646f   If your GPUs do
+00003210: 6573 6e27 7420 7375 7070 6f72 7420 6062  esn't support `b
+00003220: 666c 6f61 7431 3660 2c20 7468 656e 2079  float16`, then y
+00003230: 6f75 2061 6c73 6f0a 3e20 7761 6e74 2074  ou also.> want t
+00003240: 6f20 7365 7420 6044 5459 5045 3d66 6c6f  o set `DTYPE=flo
+00003250: 6174 3136 602e 0a0a 2323 20f0 9fa7 a920  at16`...## .... 
+00003260: 5375 7070 6f72 7465 6420 6d6f 6465 6c73  Supported models
+00003270: 0a0a 4f70 656e 4c4c 4d20 6375 7272 656e  ..OpenLLM curren
+00003280: 746c 7920 7375 7070 6f72 7473 2074 6865  tly supports the
+00003290: 2066 6f6c 6c6f 7769 6e67 206d 6f64 656c   following model
+000032a0: 732e 2042 7920 6465 6661 756c 742c 204f  s. By default, O
+000032b0: 7065 6e4c 4c4d 2064 6f65 736e 2774 2069  penLLM doesn't i
+000032c0: 6e63 6c75 6465 2064 6570 656e 6465 6e63  nclude dependenc
+000032d0: 6965 7320 746f 2072 756e 2061 6c6c 206d  ies to run all m
+000032e0: 6f64 656c 732e 2054 6865 2065 7874 7261  odels. The extra
+000032f0: 206d 6f64 656c 2d73 7065 6369 6669 6320   model-specific 
+00003300: 6465 7065 6e64 656e 6369 6573 2063 616e  dependencies can
+00003310: 2062 6520 696e 7374 616c 6c65 6420 7769   be installed wi
+00003320: 7468 2074 6865 2069 6e73 7472 7563 7469  th the instructi
+00003330: 6f6e 7320 6265 6c6f 772e 0a0a 3c21 2d2d  ons below...<!--
+00003340: 2075 7064 6174 652d 7265 6164 6d65 2e70   update-readme.p
+00003350: 793a 2073 7461 7274 202d 2d3e 0a3c 6465  y: start -->.<de
+00003360: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
+00003370: 3e42 6169 6368 7561 6e3c 2f73 756d 6d61  >Baichuan</summa
+00003380: 7279 3e0a 0a0a 2323 2320 5175 6963 6b73  ry>...### Quicks
+00003390: 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465  tart....> **Note
+000033a0: 3a2a 2a20 4261 6963 6875 616e 2072 6571  :** Baichuan req
+000033b0: 7569 7265 7320 746f 2069 6e73 7461 6c6c  uires to install
+000033c0: 2077 6974 683a 0a3e 2060 6060 6261 7368   with:.> ```bash
+000033d0: 0a3e 2070 6970 2069 6e73 7461 6c6c 2022  .> pip install "
+000033e0: 6f70 656e 6c6c 6d5b 6261 6963 6875 616e  openllm[baichuan
+000033f0: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
+00003400: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00003410: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
+00003420: 7370 696e 2075 7020 6120 4261 6963 6875  spin up a Baichu
+00003430: 616e 2073 6572 7665 723a 0a0a 6060 6062  an server:..```b
+00003440: 6173 680a 5452 5553 545f 5245 4d4f 5445  ash.TRUST_REMOTE
+00003450: 5f43 4f44 453d 5472 7565 206f 7065 6e6c  _CODE=True openl
+00003460: 6c6d 2073 7461 7274 2062 6169 6368 7561  lm start baichua
+00003470: 6e2d 696e 632f 6261 6963 6875 616e 2d37  n-inc/baichuan-7
+00003480: 620a 6060 600a 496e 2061 2064 6966 6665  b.```.In a diffe
+00003490: 7265 6e74 2074 6572 6d69 6e61 6c2c 2072  rent terminal, r
+000034a0: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
+000034b0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7465   command to inte
+000034c0: 7261 6374 2077 6974 6820 7468 6520 7365  ract with the se
+000034d0: 7276 6572 3a0a 0a60 6060 6261 7368 0a65  rver:..```bash.e
+000034e0: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
+000034f0: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
+00003500: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
+00003510: 6e6c 6c6d 2071 7565 7279 2027 5768 6174  nllm query 'What
+00003520: 2061 7265 206c 6172 6765 206c 616e 6775   are large langu
+00003530: 6167 6520 6d6f 6465 6c73 3f27 0a60 6060  age models?'.```
+00003540: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2041  ...> **Note:** A
+00003550: 6e79 2042 6169 6368 7561 6e20 7661 7269  ny Baichuan vari
+00003560: 616e 7473 2063 616e 2062 6520 6465 706c  ants can be depl
+00003570: 6f79 6564 2077 6974 6820 4f70 656e 4c4c  oyed with OpenLL
+00003580: 4d2e 2056 6973 6974 2074 6865 205b 4875  M. Visit the [Hu
+00003590: 6767 696e 6746 6163 6520 4d6f 6465 6c20  ggingFace Model 
+000035a0: 4875 625d 2868 7474 7073 3a2f 2f68 7567  Hub](https://hug
+000035b0: 6769 6e67 6661 6365 2e63 6f2f 6d6f 6465  gingface.co/mode
+000035c0: 6c73 3f73 6f72 743d 7472 656e 6469 6e67  ls?sort=trending
+000035d0: 2673 6561 7263 683d 6261 6963 6875 616e  &search=baichuan
+000035e0: 2920 746f 2073 6565 206d 6f72 6520 4261  ) to see more Ba
+000035f0: 6963 6875 616e 2d63 6f6d 7061 7469 626c  ichuan-compatibl
+00003600: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
+00003610: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
+00003620: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
+00003630: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
+00003640: 6c6c 6f77 696e 6720 4261 6963 6875 616e  llowing Baichuan
+00003650: 206d 6f64 656c 7320 7669 6120 606f 7065   models via `ope
+00003660: 6e6c 6c6d 2073 7461 7274 603a 0a0a 0a2d  nllm start`:...-
+00003670: 205b 6261 6963 6875 616e 2d69 6e63 2f62   [baichuan-inc/b
+00003680: 6169 6368 7561 6e32 2d37 622d 6261 7365  aichuan2-7b-base
+00003690: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+000036a0: 6766 6163 652e 636f 2f62 6169 6368 7561  gface.co/baichua
+000036b0: 6e2d 696e 632f 6261 6963 6875 616e 322d  n-inc/baichuan2-
+000036c0: 3762 2d62 6173 6529 0a2d 205b 6261 6963  7b-base).- [baic
+000036d0: 6875 616e 2d69 6e63 2f62 6169 6368 7561  huan-inc/baichua
+000036e0: 6e32 2d37 622d 6368 6174 5d28 6874 7470  n2-7b-chat](http
+000036f0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00003700: 636f 2f62 6169 6368 7561 6e2d 696e 632f  co/baichuan-inc/
+00003710: 6261 6963 6875 616e 322d 3762 2d63 6861  baichuan2-7b-cha
+00003720: 7429 0a2d 205b 6261 6963 6875 616e 2d69  t).- [baichuan-i
+00003730: 6e63 2f62 6169 6368 7561 6e32 2d31 3362  nc/baichuan2-13b
+00003740: 2d62 6173 655d 2868 7474 7073 3a2f 2f68  -base](https://h
+00003750: 7567 6769 6e67 6661 6365 2e63 6f2f 6261  uggingface.co/ba
+00003760: 6963 6875 616e 2d69 6e63 2f62 6169 6368  ichuan-inc/baich
+00003770: 7561 6e32 2d31 3362 2d62 6173 6529 0a2d  uan2-13b-base).-
+00003780: 205b 6261 6963 6875 616e 2d69 6e63 2f62   [baichuan-inc/b
+00003790: 6169 6368 7561 6e32 2d31 3362 2d63 6861  aichuan2-13b-cha
+000037a0: 745d 2868 7474 7073 3a2f 2f68 7567 6769  t](https://huggi
+000037b0: 6e67 6661 6365 2e63 6f2f 6261 6963 6875  ngface.co/baichu
+000037c0: 616e 2d69 6e63 2f62 6169 6368 7561 6e32  an-inc/baichuan2
+000037d0: 2d31 3362 2d63 6861 7429 0a0a 3c2f 6465  -13b-chat)..</de
+000037e0: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
+000037f0: 3e0a 0a3c 7375 6d6d 6172 793e 4368 6174  >..<summary>Chat
+00003800: 474c 4d3c 2f73 756d 6d61 7279 3e0a 0a0a  GLM</summary>...
+00003810: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
+00003820: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 4368  ..> **Note:** Ch
+00003830: 6174 474c 4d20 7265 7175 6972 6573 2074  atGLM requires t
+00003840: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
+00003850: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
+00003860: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
+00003870: 5b63 6861 7467 6c6d 5d22 0a3e 2060 6060  [chatglm]".> ```
+00003880: 0a0a 0a52 756e 2074 6865 2066 6f6c 6c6f  ...Run the follo
+00003890: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+000038a0: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
+000038b0: 6120 4368 6174 474c 4d20 7365 7276 6572  a ChatGLM server
+000038c0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
+000038d0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
+000038e0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
+000038f0: 7468 7564 6d2f 6368 6174 676c 6d2d 3662  thudm/chatglm-6b
+00003900: 0a60 6060 0a49 6e20 6120 6469 6666 6572  .```.In a differ
+00003910: 656e 7420 7465 726d 696e 616c 2c20 7275  ent terminal, ru
+00003920: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00003930: 636f 6d6d 616e 6420 746f 2069 6e74 6572  command to inter
+00003940: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
+00003950: 7665 723a 0a0a 6060 6062 6173 680a 6578  ver:..```bash.ex
+00003960: 706f 7274 204f 5045 4e4c 4c4d 5f45 4e44  port OPENLLM_END
+00003970: 504f 494e 543d 6874 7470 3a2f 2f6c 6f63  POINT=http://loc
+00003980: 616c 686f 7374 3a33 3030 300a 6f70 656e  alhost:3000.open
+00003990: 6c6c 6d20 7175 6572 7920 2757 6861 7420  llm query 'What 
+000039a0: 6172 6520 6c61 7267 6520 6c61 6e67 7561  are large langua
+000039b0: 6765 206d 6f64 656c 733f 270a 6060 600a  ge models?'.```.
+000039c0: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 416e  ..> **Note:** An
+000039d0: 7920 4368 6174 474c 4d20 7661 7269 616e  y ChatGLM varian
+000039e0: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
+000039f0: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
+00003a00: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
+00003a10: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
+00003a20: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00003a30: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
+00003a40: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
+00003a50: 6561 7263 683d 6368 6174 676c 6d29 2074  earch=chatglm) t
+00003a60: 6f20 7365 6520 6d6f 7265 2043 6861 7447  o see more ChatG
+00003a70: 4c4d 2d63 6f6d 7061 7469 626c 6520 6d6f  LM-compatible mo
+00003a80: 6465 6c73 2e0a 0a0a 0a23 2323 2053 7570  dels.....### Sup
+00003a90: 706f 7274 6564 206d 6f64 656c 730a 0a59  ported models..Y
+00003aa0: 6f75 2063 616e 2073 7065 6369 6679 2061  ou can specify a
+00003ab0: 6e79 206f 6620 7468 6520 666f 6c6c 6f77  ny of the follow
+00003ac0: 696e 6720 4368 6174 474c 4d20 6d6f 6465  ing ChatGLM mode
+00003ad0: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
+00003ae0: 7374 6172 7460 3a0a 0a0a 2d20 5b74 6875  start`:...- [thu
+00003af0: 646d 2f63 6861 7467 6c6d 2d36 625d 2868  dm/chatglm-6b](h
+00003b00: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00003b10: 6365 2e63 6f2f 7468 7564 6d2f 6368 6174  ce.co/thudm/chat
+00003b20: 676c 6d2d 3662 290a 2d20 5b74 6875 646d  glm-6b).- [thudm
+00003b30: 2f63 6861 7467 6c6d 2d36 622d 696e 7438  /chatglm-6b-int8
+00003b40: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00003b50: 6766 6163 652e 636f 2f74 6875 646d 2f63  gface.co/thudm/c
+00003b60: 6861 7467 6c6d 2d36 622d 696e 7438 290a  hatglm-6b-int8).
+00003b70: 2d20 5b74 6875 646d 2f63 6861 7467 6c6d  - [thudm/chatglm
+00003b80: 2d36 622d 696e 7434 5d28 6874 7470 733a  -6b-int4](https:
+00003b90: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00003ba0: 2f74 6875 646d 2f63 6861 7467 6c6d 2d36  /thudm/chatglm-6
+00003bb0: 622d 696e 7434 290a 2d20 5b74 6875 646d  b-int4).- [thudm
+00003bc0: 2f63 6861 7467 6c6d 322d 3662 5d28 6874  /chatglm2-6b](ht
+00003bd0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00003be0: 652e 636f 2f74 6875 646d 2f63 6861 7467  e.co/thudm/chatg
+00003bf0: 6c6d 322d 3662 290a 2d20 5b74 6875 646d  lm2-6b).- [thudm
+00003c00: 2f63 6861 7467 6c6d 322d 3662 2d69 6e74  /chatglm2-6b-int
+00003c10: 345d 2868 7474 7073 3a2f 2f68 7567 6769  4](https://huggi
+00003c20: 6e67 6661 6365 2e63 6f2f 7468 7564 6d2f  ngface.co/thudm/
+00003c30: 6368 6174 676c 6d32 2d36 622d 696e 7434  chatglm2-6b-int4
+00003c40: 290a 2d20 5b74 6875 646d 2f63 6861 7467  ).- [thudm/chatg
+00003c50: 6c6d 332d 3662 5d28 6874 7470 733a 2f2f  lm3-6b](https://
+00003c60: 6875 6767 696e 6766 6163 652e 636f 2f74  huggingface.co/t
+00003c70: 6875 646d 2f63 6861 7467 6c6d 332d 3662  hudm/chatglm3-6b
+00003c80: 290a 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  )..</details>..<
+00003c90: 6465 7461 696c 733e 0a0a 3c73 756d 6d61  details>..<summa
+00003ca0: 7279 3e44 6272 783c 2f73 756d 6d61 7279  ry>Dbrx</summary
+00003cb0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
+00003cc0: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
+00003cd0: 2a20 4462 7278 2072 6571 7569 7265 7320  * Dbrx requires 
+00003ce0: 746f 2069 6e73 7461 6c6c 2077 6974 683a  to install with:
+00003cf0: 0a3e 2060 6060 6261 7368 0a3e 2070 6970  .> ```bash.> pip
+00003d00: 2069 6e73 7461 6c6c 2022 6f70 656e 6c6c   install "openll
+00003d10: 6d5b 6462 7278 5d22 0a3e 2060 6060 0a0a  m[dbrx]".> ```..
+00003d20: 0a52 756e 2074 6865 2066 6f6c 6c6f 7769  .Run the followi
+00003d30: 6e67 2063 6f6d 6d61 6e64 2074 6f20 7175  ng command to qu
+00003d40: 6963 6b6c 7920 7370 696e 2075 7020 6120  ickly spin up a 
+00003d50: 4462 7278 2073 6572 7665 723a 0a0a 6060  Dbrx server:..``
+00003d60: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
+00003d70: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
+00003d80: 6e6c 6c6d 2073 7461 7274 2064 6174 6162  nllm start datab
+00003d90: 7269 636b 732f 6462 7278 2d69 6e73 7472  ricks/dbrx-instr
+00003da0: 7563 740a 6060 600a 496e 2061 2064 6966  uct.```.In a dif
+00003db0: 6665 7265 6e74 2074 6572 6d69 6e61 6c2c  ferent terminal,
+00003dc0: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+00003dd0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 696e  ng command to in
+00003de0: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
+00003df0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+00003e00: 0a65 7870 6f72 7420 4f50 454e 4c4c 4d5f  .export OPENLLM_
+00003e10: 454e 4450 4f49 4e54 3d68 7474 703a 2f2f  ENDPOINT=http://
+00003e20: 6c6f 6361 6c68 6f73 743a 3330 3030 0a6f  localhost:3000.o
+00003e30: 7065 6e6c 6c6d 2071 7565 7279 2027 5768  penllm query 'Wh
+00003e40: 6174 2061 7265 206c 6172 6765 206c 616e  at are large lan
+00003e50: 6775 6167 6520 6d6f 6465 6c73 3f27 0a60  guage models?'.`
+00003e60: 6060 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  ``...> **Note:**
+00003e70: 2041 6e79 2044 6272 7820 7661 7269 616e   Any Dbrx varian
+00003e80: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
+00003e90: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
+00003ea0: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
+00003eb0: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
+00003ec0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00003ed0: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
+00003ee0: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
+00003ef0: 6561 7263 683d 6462 7278 2920 746f 2073  earch=dbrx) to s
+00003f00: 6565 206d 6f72 6520 4462 7278 2d63 6f6d  ee more Dbrx-com
+00003f10: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
+00003f20: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
+00003f30: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
+00003f40: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
+00003f50: 7468 6520 666f 6c6c 6f77 696e 6720 4462  the following Db
+00003f60: 7278 206d 6f64 656c 7320 7669 6120 606f  rx models via `o
+00003f70: 7065 6e6c 6c6d 2073 7461 7274 603a 0a0a  penllm start`:..
+00003f80: 0a2d 205b 6461 7461 6272 6963 6b73 2f64  .- [databricks/d
+00003f90: 6272 782d 696e 7374 7275 6374 5d28 6874  brx-instruct](ht
+00003fa0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00003fb0: 652e 636f 2f64 6174 6162 7269 636b 732f  e.co/databricks/
+00003fc0: 6462 7278 2d69 6e73 7472 7563 7429 0a2d  dbrx-instruct).-
+00003fd0: 205b 6461 7461 6272 6963 6b73 2f64 6272   [databricks/dbr
+00003fe0: 782d 6261 7365 5d28 6874 7470 733a 2f2f  x-base](https://
+00003ff0: 6875 6767 696e 6766 6163 652e 636f 2f64  huggingface.co/d
+00004000: 6174 6162 7269 636b 732f 6462 7278 2d62  atabricks/dbrx-b
+00004010: 6173 6529 0a0a 3c2f 6465 7461 696c 733e  ase)..</details>
+00004020: 0a0a 3c64 6574 6169 6c73 3e0a 0a3c 7375  ..<details>..<su
+00004030: 6d6d 6172 793e 446f 6c6c 7956 323c 2f73  mmary>DollyV2</s
+00004040: 756d 6d61 7279 3e0a 0a0a 2323 2320 5175  ummary>...### Qu
+00004050: 6963 6b73 7461 7274 0a0a 5275 6e20 7468  ickstart..Run th
+00004060: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00004070: 616e 6420 746f 2071 7569 636b 6c79 2073  and to quickly s
+00004080: 7069 6e20 7570 2061 2044 6f6c 6c79 5632  pin up a DollyV2
+00004090: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
+000040a0: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
+000040b0: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
+000040c0: 2073 7461 7274 2064 6174 6162 7269 636b   start databrick
+000040d0: 732f 646f 6c6c 792d 7632 2d33 620a 6060  s/dolly-v2-3b.``
+000040e0: 600a 496e 2061 2064 6966 6665 7265 6e74  `.In a different
+000040f0: 2074 6572 6d69 6e61 6c2c 2072 756e 2074   terminal, run t
+00004100: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00004110: 6d61 6e64 2074 6f20 696e 7465 7261 6374  mand to interact
+00004120: 2077 6974 6820 7468 6520 7365 7276 6572   with the server
+00004130: 3a0a 0a60 6060 6261 7368 0a65 7870 6f72  :..```bash.expor
+00004140: 7420 4f50 454e 4c4c 4d5f 454e 4450 4f49  t OPENLLM_ENDPOI
+00004150: 4e54 3d68 7474 703a 2f2f 6c6f 6361 6c68  NT=http://localh
+00004160: 6f73 743a 3330 3030 0a6f 7065 6e6c 6c6d  ost:3000.openllm
+00004170: 2071 7565 7279 2027 5768 6174 2061 7265   query 'What are
+00004180: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
+00004190: 6d6f 6465 6c73 3f27 0a60 6060 0a0a 0a3e  models?'.```...>
+000041a0: 202a 2a4e 6f74 653a 2a2a 2041 6e79 2044   **Note:** Any D
+000041b0: 6f6c 6c79 5632 2076 6172 6961 6e74 7320  ollyV2 variants 
+000041c0: 6361 6e20 6265 2064 6570 6c6f 7965 6420  can be deployed 
+000041d0: 7769 7468 204f 7065 6e4c 4c4d 2e20 5669  with OpenLLM. Vi
+000041e0: 7369 7420 7468 6520 5b48 7567 6769 6e67  sit the [Hugging
+000041f0: 4661 6365 204d 6f64 656c 2048 7562 5d28  Face Model Hub](
+00004200: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00004210: 6163 652e 636f 2f6d 6f64 656c 733f 736f  ace.co/models?so
+00004220: 7274 3d74 7265 6e64 696e 6726 7365 6172  rt=trending&sear
+00004230: 6368 3d64 6f6c 6c79 5f76 3229 2074 6f20  ch=dolly_v2) to 
+00004240: 7365 6520 6d6f 7265 2044 6f6c 6c79 5632  see more DollyV2
+00004250: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
+00004260: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
+00004270: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
+00004280: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
+00004290: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+000042a0: 6720 446f 6c6c 7956 3220 6d6f 6465 6c73  g DollyV2 models
+000042b0: 2076 6961 2060 6f70 656e 6c6c 6d20 7374   via `openllm st
+000042c0: 6172 7460 3a0a 0a0a 2d20 5b64 6174 6162  art`:...- [datab
+000042d0: 7269 636b 732f 646f 6c6c 792d 7632 2d33  ricks/dolly-v2-3
+000042e0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+000042f0: 6e67 6661 6365 2e63 6f2f 6461 7461 6272  ngface.co/databr
+00004300: 6963 6b73 2f64 6f6c 6c79 2d76 322d 3362  icks/dolly-v2-3b
+00004310: 290a 2d20 5b64 6174 6162 7269 636b 732f  ).- [databricks/
+00004320: 646f 6c6c 792d 7632 2d37 625d 2868 7474  dolly-v2-7b](htt
+00004330: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00004340: 2e63 6f2f 6461 7461 6272 6963 6b73 2f64  .co/databricks/d
+00004350: 6f6c 6c79 2d76 322d 3762 290a 2d20 5b64  olly-v2-7b).- [d
+00004360: 6174 6162 7269 636b 732f 646f 6c6c 792d  atabricks/dolly-
+00004370: 7632 2d31 3262 5d28 6874 7470 733a 2f2f  v2-12b](https://
+00004380: 6875 6767 696e 6766 6163 652e 636f 2f64  huggingface.co/d
+00004390: 6174 6162 7269 636b 732f 646f 6c6c 792d  atabricks/dolly-
+000043a0: 7632 2d31 3262 290a 0a3c 2f64 6574 6169  v2-12b)..</detai
+000043b0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a0a  ls>..<details>..
+000043c0: 3c73 756d 6d61 7279 3e46 616c 636f 6e3c  <summary>Falcon<
+000043d0: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
+000043e0: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
+000043f0: 2a2a 4e6f 7465 3a2a 2a20 4661 6c63 6f6e  **Note:** Falcon
+00004400: 2072 6571 7569 7265 7320 746f 2069 6e73   requires to ins
+00004410: 7461 6c6c 2077 6974 683a 0a3e 2060 6060  tall with:.> ```
+00004420: 6261 7368 0a3e 2070 6970 2069 6e73 7461  bash.> pip insta
+00004430: 6c6c 2022 6f70 656e 6c6c 6d5b 6661 6c63  ll "openllm[falc
+00004440: 6f6e 5d22 0a3e 2060 6060 0a0a 0a52 756e  on]".> ```...Run
+00004450: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00004460: 6f6d 6d61 6e64 2074 6f20 7175 6963 6b6c  ommand to quickl
+00004470: 7920 7370 696e 2075 7020 6120 4661 6c63  y spin up a Falc
+00004480: 6f6e 2073 6572 7665 723a 0a0a 6060 6062  on server:..```b
+00004490: 6173 680a 5452 5553 545f 5245 4d4f 5445  ash.TRUST_REMOTE
+000044a0: 5f43 4f44 453d 5472 7565 206f 7065 6e6c  _CODE=True openl
+000044b0: 6c6d 2073 7461 7274 2074 6969 7561 652f  lm start tiiuae/
+000044c0: 6661 6c63 6f6e 2d37 620a 6060 600a 496e  falcon-7b.```.In
+000044d0: 2061 2064 6966 6665 7265 6e74 2074 6572   a different ter
+000044e0: 6d69 6e61 6c2c 2072 756e 2074 6865 2066  minal, run the f
+000044f0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00004500: 2074 6f20 696e 7465 7261 6374 2077 6974   to interact wit
+00004510: 6820 7468 6520 7365 7276 6572 3a0a 0a60  h the server:..`
+00004520: 6060 6261 7368 0a65 7870 6f72 7420 4f50  ``bash.export OP
+00004530: 454e 4c4c 4d5f 454e 4450 4f49 4e54 3d68  ENLLM_ENDPOINT=h
+00004540: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00004550: 3330 3030 0a6f 7065 6e6c 6c6d 2071 7565  3000.openllm que
+00004560: 7279 2027 5768 6174 2061 7265 206c 6172  ry 'What are lar
+00004570: 6765 206c 616e 6775 6167 6520 6d6f 6465  ge language mode
+00004580: 6c73 3f27 0a60 6060 0a0a 0a3e 202a 2a4e  ls?'.```...> **N
+00004590: 6f74 653a 2a2a 2041 6e79 2046 616c 636f  ote:** Any Falco
+000045a0: 6e20 7661 7269 616e 7473 2063 616e 2062  n variants can b
+000045b0: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
+000045c0: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
+000045d0: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
+000045e0: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
+000045f0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00004600: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
+00004610: 656e 6469 6e67 2673 6561 7263 683d 6661  ending&search=fa
+00004620: 6c63 6f6e 2920 746f 2073 6565 206d 6f72  lcon) to see mor
+00004630: 6520 4661 6c63 6f6e 2d63 6f6d 7061 7469  e Falcon-compati
+00004640: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
+00004650: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
+00004660: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
+00004670: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
+00004680: 666f 6c6c 6f77 696e 6720 4661 6c63 6f6e  following Falcon
+00004690: 206d 6f64 656c 7320 7669 6120 606f 7065   models via `ope
+000046a0: 6e6c 6c6d 2073 7461 7274 603a 0a0a 0a2d  nllm start`:...-
+000046b0: 205b 7469 6975 6165 2f66 616c 636f 6e2d   [tiiuae/falcon-
+000046c0: 3762 5d28 6874 7470 733a 2f2f 6875 6767  7b](https://hugg
+000046d0: 696e 6766 6163 652e 636f 2f74 6969 7561  ingface.co/tiiua
+000046e0: 652f 6661 6c63 6f6e 2d37 6229 0a2d 205b  e/falcon-7b).- [
+000046f0: 7469 6975 6165 2f66 616c 636f 6e2d 3430  tiiuae/falcon-40
+00004700: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00004710: 6e67 6661 6365 2e63 6f2f 7469 6975 6165  ngface.co/tiiuae
+00004720: 2f66 616c 636f 6e2d 3430 6229 0a2d 205b  /falcon-40b).- [
+00004730: 7469 6975 6165 2f66 616c 636f 6e2d 3762  tiiuae/falcon-7b
+00004740: 2d69 6e73 7472 7563 745d 2868 7474 7073  -instruct](https
+00004750: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00004760: 6f2f 7469 6975 6165 2f66 616c 636f 6e2d  o/tiiuae/falcon-
+00004770: 3762 2d69 6e73 7472 7563 7429 0a2d 205b  7b-instruct).- [
+00004780: 7469 6975 6165 2f66 616c 636f 6e2d 3430  tiiuae/falcon-40
+00004790: 622d 696e 7374 7275 6374 5d28 6874 7470  b-instruct](http
+000047a0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+000047b0: 636f 2f74 6969 7561 652f 6661 6c63 6f6e  co/tiiuae/falcon
+000047c0: 2d34 3062 2d69 6e73 7472 7563 7429 0a0a  -40b-instruct)..
+000047d0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+000047e0: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
+000047f0: 466c 616e 5435 3c2f 7375 6d6d 6172 793e  FlanT5</summary>
+00004800: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
+00004810: 740a 0a52 756e 2074 6865 2066 6f6c 6c6f  t..Run the follo
+00004820: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+00004830: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
+00004840: 6120 466c 616e 5435 2073 6572 7665 723a  a FlanT5 server:
+00004850: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
+00004860: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
+00004870: 206f 7065 6e6c 6c6d 2073 7461 7274 2067   openllm start g
+00004880: 6f6f 676c 652f 666c 616e 2d74 352d 6c61  oogle/flan-t5-la
+00004890: 7267 650a 6060 600a 496e 2061 2064 6966  rge.```.In a dif
+000048a0: 6665 7265 6e74 2074 6572 6d69 6e61 6c2c  ferent terminal,
+000048b0: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
+000048c0: 6e67 2063 6f6d 6d61 6e64 2074 6f20 696e  ng command to in
+000048d0: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
+000048e0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+000048f0: 0a65 7870 6f72 7420 4f50 454e 4c4c 4d5f  .export OPENLLM_
+00004900: 454e 4450 4f49 4e54 3d68 7474 703a 2f2f  ENDPOINT=http://
+00004910: 6c6f 6361 6c68 6f73 743a 3330 3030 0a6f  localhost:3000.o
+00004920: 7065 6e6c 6c6d 2071 7565 7279 2027 5768  penllm query 'Wh
+00004930: 6174 2061 7265 206c 6172 6765 206c 616e  at are large lan
+00004940: 6775 6167 6520 6d6f 6465 6c73 3f27 0a60  guage models?'.`
+00004950: 6060 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  ``...> **Note:**
+00004960: 2041 6e79 2046 6c61 6e54 3520 7661 7269   Any FlanT5 vari
+00004970: 616e 7473 2063 616e 2062 6520 6465 706c  ants can be depl
+00004980: 6f79 6564 2077 6974 6820 4f70 656e 4c4c  oyed with OpenLL
+00004990: 4d2e 2056 6973 6974 2074 6865 205b 4875  M. Visit the [Hu
+000049a0: 6767 696e 6746 6163 6520 4d6f 6465 6c20  ggingFace Model 
+000049b0: 4875 625d 2868 7474 7073 3a2f 2f68 7567  Hub](https://hug
+000049c0: 6769 6e67 6661 6365 2e63 6f2f 6d6f 6465  gingface.co/mode
+000049d0: 6c73 3f73 6f72 743d 7472 656e 6469 6e67  ls?sort=trending
+000049e0: 2673 6561 7263 683d 666c 616e 5f74 3529  &search=flan_t5)
+000049f0: 2074 6f20 7365 6520 6d6f 7265 2046 6c61   to see more Fla
+00004a00: 6e54 352d 636f 6d70 6174 6962 6c65 206d  nT5-compatible m
+00004a10: 6f64 656c 732e 0a0a 0a0a 2323 2320 5375  odels.....### Su
+00004a20: 7070 6f72 7465 6420 6d6f 6465 6c73 0a0a  pported models..
+00004a30: 596f 7520 6361 6e20 7370 6563 6966 7920  You can specify 
+00004a40: 616e 7920 6f66 2074 6865 2066 6f6c 6c6f  any of the follo
+00004a50: 7769 6e67 2046 6c61 6e54 3520 6d6f 6465  wing FlanT5 mode
+00004a60: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
+00004a70: 7374 6172 7460 3a0a 0a0a 2d20 5b67 6f6f  start`:...- [goo
+00004a80: 676c 652f 666c 616e 2d74 352d 736d 616c  gle/flan-t5-smal
+00004a90: 6c5d 2868 7474 7073 3a2f 2f68 7567 6769  l](https://huggi
+00004aa0: 6e67 6661 6365 2e63 6f2f 676f 6f67 6c65  ngface.co/google
+00004ab0: 2f66 6c61 6e2d 7435 2d73 6d61 6c6c 290a  /flan-t5-small).
+00004ac0: 2d20 5b67 6f6f 676c 652f 666c 616e 2d74  - [google/flan-t
+00004ad0: 352d 6261 7365 5d28 6874 7470 733a 2f2f  5-base](https://
+00004ae0: 6875 6767 696e 6766 6163 652e 636f 2f67  huggingface.co/g
+00004af0: 6f6f 676c 652f 666c 616e 2d74 352d 6261  oogle/flan-t5-ba
+00004b00: 7365 290a 2d20 5b67 6f6f 676c 652f 666c  se).- [google/fl
+00004b10: 616e 2d74 352d 6c61 7267 655d 2868 7474  an-t5-large](htt
+00004b20: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00004b30: 2e63 6f2f 676f 6f67 6c65 2f66 6c61 6e2d  .co/google/flan-
+00004b40: 7435 2d6c 6172 6765 290a 2d20 5b67 6f6f  t5-large).- [goo
+00004b50: 676c 652f 666c 616e 2d74 352d 786c 5d28  gle/flan-t5-xl](
+00004b60: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00004b70: 6163 652e 636f 2f67 6f6f 676c 652f 666c  ace.co/google/fl
+00004b80: 616e 2d74 352d 786c 290a 2d20 5b67 6f6f  an-t5-xl).- [goo
+00004b90: 676c 652f 666c 616e 2d74 352d 7878 6c5d  gle/flan-t5-xxl]
+00004ba0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+00004bb0: 6661 6365 2e63 6f2f 676f 6f67 6c65 2f66  face.co/google/f
+00004bc0: 6c61 6e2d 7435 2d78 786c 290a 0a3c 2f64  lan-t5-xxl)..</d
+00004bd0: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
+00004be0: 733e 0a0a 3c73 756d 6d61 7279 3e47 656d  s>..<summary>Gem
+00004bf0: 6d61 3c2f 7375 6d6d 6172 793e 0a0a 0a23  ma</summary>...#
+00004c00: 2323 2051 7569 636b 7374 6172 740a 0a0a  ## Quickstart...
+00004c10: 0a3e 202a 2a4e 6f74 653a 2a2a 2047 656d  .> **Note:** Gem
+00004c20: 6d61 2072 6571 7569 7265 7320 746f 2069  ma requires to i
+00004c30: 6e73 7461 6c6c 2077 6974 683a 0a3e 2060  nstall with:.> `
+00004c40: 6060 6261 7368 0a3e 2070 6970 2069 6e73  ``bash.> pip ins
+00004c50: 7461 6c6c 2022 6f70 656e 6c6c 6d5b 6765  tall "openllm[ge
+00004c60: 6d6d 615d 220a 3e20 6060 600a 0a0a 5275  mma]".> ```...Ru
+00004c70: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00004c80: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
+00004c90: 6c79 2073 7069 6e20 7570 2061 2047 656d  ly spin up a Gem
+00004ca0: 6d61 2073 6572 7665 723a 0a0a 6060 6062  ma server:..```b
+00004cb0: 6173 680a 5452 5553 545f 5245 4d4f 5445  ash.TRUST_REMOTE
+00004cc0: 5f43 4f44 453d 5472 7565 206f 7065 6e6c  _CODE=True openl
+00004cd0: 6c6d 2073 7461 7274 2067 6f6f 676c 652f  lm start google/
+00004ce0: 6765 6d6d 612d 3762 0a60 6060 0a49 6e20  gemma-7b.```.In 
+00004cf0: 6120 6469 6666 6572 656e 7420 7465 726d  a different term
+00004d00: 696e 616c 2c20 7275 6e20 7468 6520 666f  inal, run the fo
+00004d10: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+00004d20: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
+00004d30: 2074 6865 2073 6572 7665 723a 0a0a 6060   the server:..``
+00004d40: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
+00004d50: 4e4c 4c4d 5f45 4e44 504f 494e 543d 6874  NLLM_ENDPOINT=ht
+00004d60: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
+00004d70: 3030 300a 6f70 656e 6c6c 6d20 7175 6572  000.openllm quer
+00004d80: 7920 2757 6861 7420 6172 6520 6c61 7267  y 'What are larg
+00004d90: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
+00004da0: 733f 270a 6060 600a 0a0a 3e20 2a2a 4e6f  s?'.```...> **No
+00004db0: 7465 3a2a 2a20 416e 7920 4765 6d6d 6120  te:** Any Gemma 
+00004dc0: 7661 7269 616e 7473 2063 616e 2062 6520  variants can be 
+00004dd0: 6465 706c 6f79 6564 2077 6974 6820 4f70  deployed with Op
+00004de0: 656e 4c4c 4d2e 2056 6973 6974 2074 6865  enLLM. Visit the
+00004df0: 205b 4875 6767 696e 6746 6163 6520 4d6f   [HuggingFace Mo
+00004e00: 6465 6c20 4875 625d 2868 7474 7073 3a2f  del Hub](https:/
+00004e10: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00004e20: 6d6f 6465 6c73 3f73 6f72 743d 7472 656e  models?sort=tren
+00004e30: 6469 6e67 2673 6561 7263 683d 6765 6d6d  ding&search=gemm
+00004e40: 6129 2074 6f20 7365 6520 6d6f 7265 2047  a) to see more G
+00004e50: 656d 6d61 2d63 6f6d 7061 7469 626c 6520  emma-compatible 
+00004e60: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
+00004e70: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
+00004e80: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
+00004e90: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
+00004ea0: 6f77 696e 6720 4765 6d6d 6120 6d6f 6465  owing Gemma mode
+00004eb0: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
+00004ec0: 7374 6172 7460 3a0a 0a0a 2d20 5b67 6f6f  start`:...- [goo
+00004ed0: 676c 652f 6765 6d6d 612d 3762 5d28 6874  gle/gemma-7b](ht
+00004ee0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00004ef0: 652e 636f 2f67 6f6f 676c 652f 6765 6d6d  e.co/google/gemm
+00004f00: 612d 3762 290a 2d20 5b67 6f6f 676c 652f  a-7b).- [google/
+00004f10: 6765 6d6d 612d 3762 2d69 745d 2868 7474  gemma-7b-it](htt
+00004f20: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00004f30: 2e63 6f2f 676f 6f67 6c65 2f67 656d 6d61  .co/google/gemma
+00004f40: 2d37 622d 6974 290a 2d20 5b67 6f6f 676c  -7b-it).- [googl
+00004f50: 652f 6765 6d6d 612d 3262 5d28 6874 7470  e/gemma-2b](http
+00004f60: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00004f70: 636f 2f67 6f6f 676c 652f 6765 6d6d 612d  co/google/gemma-
+00004f80: 3262 290a 2d20 5b67 6f6f 676c 652f 6765  2b).- [google/ge
+00004f90: 6d6d 612d 3262 2d69 745d 2868 7474 7073  mma-2b-it](https
+00004fa0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00004fb0: 6f2f 676f 6f67 6c65 2f67 656d 6d61 2d32  o/google/gemma-2
+00004fc0: 622d 6974 290a 0a3c 2f64 6574 6169 6c73  b-it)..</details
+00004fd0: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
+00004fe0: 756d 6d61 7279 3e47 5054 4e65 6f58 3c2f  ummary>GPTNeoX</
+00004ff0: 7375 6d6d 6172 793e 0a0a 0a23 2323 2051  summary>...### Q
+00005000: 7569 636b 7374 6172 740a 0a52 756e 2074  uickstart..Run t
+00005010: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00005020: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
+00005030: 7370 696e 2075 7020 6120 4750 544e 656f  spin up a GPTNeo
+00005040: 5820 7365 7276 6572 3a0a 0a60 6060 6261  X server:..```ba
+00005050: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
+00005060: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
+00005070: 6d20 7374 6172 7420 656c 6575 7468 6572  m start eleuther
+00005080: 6169 2f67 7074 2d6e 656f 782d 3230 620a  ai/gpt-neox-20b.
+00005090: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
+000050a0: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
+000050b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+000050c0: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
+000050d0: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
+000050e0: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
+000050f0: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
+00005100: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
+00005110: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
+00005120: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
+00005130: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
+00005140: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
+00005150: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
+00005160: 2047 5054 4e65 6f58 2076 6172 6961 6e74   GPTNeoX variant
+00005170: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
+00005180: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
+00005190: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
+000051a0: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
+000051b0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+000051c0: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
+000051d0: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
+000051e0: 6172 6368 3d67 7074 5f6e 656f 7829 2074  arch=gpt_neox) t
+000051f0: 6f20 7365 6520 6d6f 7265 2047 5054 4e65  o see more GPTNe
+00005200: 6f58 2d63 6f6d 7061 7469 626c 6520 6d6f  oX-compatible mo
+00005210: 6465 6c73 2e0a 0a0a 0a23 2323 2053 7570  dels.....### Sup
+00005220: 706f 7274 6564 206d 6f64 656c 730a 0a59  ported models..Y
+00005230: 6f75 2063 616e 2073 7065 6369 6679 2061  ou can specify a
+00005240: 6e79 206f 6620 7468 6520 666f 6c6c 6f77  ny of the follow
+00005250: 696e 6720 4750 544e 656f 5820 6d6f 6465  ing GPTNeoX mode
+00005260: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
+00005270: 7374 6172 7460 3a0a 0a0a 2d20 5b65 6c65  start`:...- [ele
+00005280: 7574 6865 7261 692f 6770 742d 6e65 6f78  utherai/gpt-neox
+00005290: 2d32 3062 5d28 6874 7470 733a 2f2f 6875  -20b](https://hu
+000052a0: 6767 696e 6766 6163 652e 636f 2f65 6c65  ggingface.co/ele
+000052b0: 7574 6865 7261 692f 6770 742d 6e65 6f78  utherai/gpt-neox
+000052c0: 2d32 3062 290a 0a3c 2f64 6574 6169 6c73  -20b)..</details
+000052d0: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
+000052e0: 756d 6d61 7279 3e4c 6c61 6d61 3c2f 7375  ummary>Llama</su
+000052f0: 6d6d 6172 793e 0a0a 0a23 2323 2051 7569  mmary>...### Qui
+00005300: 636b 7374 6172 740a 0a0a 0a3e 202a 2a4e  ckstart....> **N
+00005310: 6f74 653a 2a2a 204c 6c61 6d61 2072 6571  ote:** Llama req
+00005320: 7569 7265 7320 746f 2069 6e73 7461 6c6c  uires to install
+00005330: 2077 6974 683a 0a3e 2060 6060 6261 7368   with:.> ```bash
+00005340: 0a3e 2070 6970 2069 6e73 7461 6c6c 2022  .> pip install "
+00005350: 6f70 656e 6c6c 6d5b 6c6c 616d 615d 220a  openllm[llama]".
+00005360: 3e20 6060 600a 0a0a 5275 6e20 7468 6520  > ```...Run the 
+00005370: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00005380: 6420 746f 2071 7569 636b 6c79 2073 7069  d to quickly spi
+00005390: 6e20 7570 2061 204c 6c61 6d61 2073 6572  n up a Llama ser
+000053a0: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
+000053b0: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
+000053c0: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
+000053d0: 7274 204e 6f75 7352 6573 6561 7263 682f  rt NousResearch/
+000053e0: 6c6c 616d 612d 322d 3762 2d68 660a 6060  llama-2-7b-hf.``
+000053f0: 600a 496e 2061 2064 6966 6665 7265 6e74  `.In a different
+00005400: 2074 6572 6d69 6e61 6c2c 2072 756e 2074   terminal, run t
+00005410: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00005420: 6d61 6e64 2074 6f20 696e 7465 7261 6374  mand to interact
+00005430: 2077 6974 6820 7468 6520 7365 7276 6572   with the server
+00005440: 3a0a 0a60 6060 6261 7368 0a65 7870 6f72  :..```bash.expor
+00005450: 7420 4f50 454e 4c4c 4d5f 454e 4450 4f49  t OPENLLM_ENDPOI
+00005460: 4e54 3d68 7474 703a 2f2f 6c6f 6361 6c68  NT=http://localh
+00005470: 6f73 743a 3330 3030 0a6f 7065 6e6c 6c6d  ost:3000.openllm
+00005480: 2071 7565 7279 2027 5768 6174 2061 7265   query 'What are
+00005490: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
+000054a0: 6d6f 6465 6c73 3f27 0a60 6060 0a0a 0a3e  models?'.```...>
+000054b0: 202a 2a4e 6f74 653a 2a2a 2041 6e79 204c   **Note:** Any L
+000054c0: 6c61 6d61 2076 6172 6961 6e74 7320 6361  lama variants ca
+000054d0: 6e20 6265 2064 6570 6c6f 7965 6420 7769  n be deployed wi
+000054e0: 7468 204f 7065 6e4c 4c4d 2e20 5669 7369  th OpenLLM. Visi
+000054f0: 7420 7468 6520 5b48 7567 6769 6e67 4661  t the [HuggingFa
+00005500: 6365 204d 6f64 656c 2048 7562 5d28 6874  ce Model Hub](ht
+00005510: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00005520: 652e 636f 2f6d 6f64 656c 733f 736f 7274  e.co/models?sort
+00005530: 3d74 7265 6e64 696e 6726 7365 6172 6368  =trending&search
+00005540: 3d6c 6c61 6d61 2920 746f 2073 6565 206d  =llama) to see m
+00005550: 6f72 6520 4c6c 616d 612d 636f 6d70 6174  ore Llama-compat
+00005560: 6962 6c65 206d 6f64 656c 732e 0a0a 0a0a  ible models.....
+00005570: 2323 2320 5375 7070 6f72 7465 6420 6d6f  ### Supported mo
+00005580: 6465 6c73 0a0a 596f 7520 6361 6e20 7370  dels..You can sp
+00005590: 6563 6966 7920 616e 7920 6f66 2074 6865  ecify any of the
+000055a0: 2066 6f6c 6c6f 7769 6e67 204c 6c61 6d61   following Llama
+000055b0: 206d 6f64 656c 7320 7669 6120 606f 7065   models via `ope
+000055c0: 6e6c 6c6d 2073 7461 7274 603a 0a0a 0a2d  nllm start`:...-
+000055d0: 205b 6d65 7461 2d6c 6c61 6d61 2f4c 6c61   [meta-llama/Lla
+000055e0: 6d61 2d32 2d37 3062 2d63 6861 742d 6866  ma-2-70b-chat-hf
+000055f0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00005600: 6766 6163 652e 636f 2f6d 6574 612d 6c6c  gface.co/meta-ll
+00005610: 616d 612f 4c6c 616d 612d 322d 3730 622d  ama/Llama-2-70b-
+00005620: 6368 6174 2d68 6629 0a2d 205b 6d65 7461  chat-hf).- [meta
+00005630: 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32 2d31  -llama/Llama-2-1
+00005640: 3362 2d63 6861 742d 6866 5d28 6874 7470  3b-chat-hf](http
+00005650: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00005660: 636f 2f6d 6574 612d 6c6c 616d 612f 4c6c  co/meta-llama/Ll
+00005670: 616d 612d 322d 3133 622d 6368 6174 2d68  ama-2-13b-chat-h
+00005680: 6629 0a2d 205b 6d65 7461 2d6c 6c61 6d61  f).- [meta-llama
+00005690: 2f4c 6c61 6d61 2d32 2d37 622d 6368 6174  /Llama-2-7b-chat
+000056a0: 2d68 665d 2868 7474 7073 3a2f 2f68 7567  -hf](https://hug
+000056b0: 6769 6e67 6661 6365 2e63 6f2f 6d65 7461  gingface.co/meta
+000056c0: 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32 2d37  -llama/Llama-2-7
+000056d0: 622d 6368 6174 2d68 6629 0a2d 205b 6d65  b-chat-hf).- [me
+000056e0: 7461 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32  ta-llama/Llama-2
+000056f0: 2d37 3062 2d68 665d 2868 7474 7073 3a2f  -70b-hf](https:/
+00005700: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00005710: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
+00005720: 2d32 2d37 3062 2d68 6629 0a2d 205b 6d65  -2-70b-hf).- [me
+00005730: 7461 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32  ta-llama/Llama-2
+00005740: 2d31 3362 2d68 665d 2868 7474 7073 3a2f  -13b-hf](https:/
+00005750: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00005760: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
+00005770: 2d32 2d31 3362 2d68 6629 0a2d 205b 6d65  -2-13b-hf).- [me
+00005780: 7461 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32  ta-llama/Llama-2
+00005790: 2d37 622d 6866 5d28 6874 7470 733a 2f2f  -7b-hf](https://
+000057a0: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
+000057b0: 6574 612d 6c6c 616d 612f 4c6c 616d 612d  eta-llama/Llama-
+000057c0: 322d 3762 2d68 6629 0a2d 205b 4e6f 7573  2-7b-hf).- [Nous
+000057d0: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
+000057e0: 2d37 3062 2d63 6861 742d 6866 5d28 6874  -70b-chat-hf](ht
+000057f0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00005800: 652e 636f 2f4e 6f75 7352 6573 6561 7263  e.co/NousResearc
+00005810: 682f 6c6c 616d 612d 322d 3730 622d 6368  h/llama-2-70b-ch
+00005820: 6174 2d68 6629 0a2d 205b 4e6f 7573 5265  at-hf).- [NousRe
+00005830: 7365 6172 6368 2f6c 6c61 6d61 2d32 2d31  search/llama-2-1
+00005840: 3362 2d63 6861 742d 6866 5d28 6874 7470  3b-chat-hf](http
+00005850: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00005860: 636f 2f4e 6f75 7352 6573 6561 7263 682f  co/NousResearch/
+00005870: 6c6c 616d 612d 322d 3133 622d 6368 6174  llama-2-13b-chat
+00005880: 2d68 6629 0a2d 205b 4e6f 7573 5265 7365  -hf).- [NousRese
+00005890: 6172 6368 2f6c 6c61 6d61 2d32 2d37 622d  arch/llama-2-7b-
+000058a0: 6368 6174 2d68 665d 2868 7474 7073 3a2f  chat-hf](https:/
+000058b0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+000058c0: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
+000058d0: 6d61 2d32 2d37 622d 6368 6174 2d68 6629  ma-2-7b-chat-hf)
+000058e0: 0a2d 205b 4e6f 7573 5265 7365 6172 6368  .- [NousResearch
+000058f0: 2f6c 6c61 6d61 2d32 2d37 3062 2d68 665d  /llama-2-70b-hf]
+00005900: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+00005910: 6661 6365 2e63 6f2f 4e6f 7573 5265 7365  face.co/NousRese
+00005920: 6172 6368 2f6c 6c61 6d61 2d32 2d37 3062  arch/llama-2-70b
+00005930: 2d68 6629 0a2d 205b 4e6f 7573 5265 7365  -hf).- [NousRese
+00005940: 6172 6368 2f6c 6c61 6d61 2d32 2d31 3362  arch/llama-2-13b
+00005950: 2d68 665d 2868 7474 7073 3a2f 2f68 7567  -hf](https://hug
+00005960: 6769 6e67 6661 6365 2e63 6f2f 4e6f 7573  gingface.co/Nous
+00005970: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
+00005980: 2d31 3362 2d68 6629 0a2d 205b 4e6f 7573  -13b-hf).- [Nous
+00005990: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
+000059a0: 2d37 622d 6866 5d28 6874 7470 733a 2f2f  -7b-hf](https://
+000059b0: 6875 6767 696e 6766 6163 652e 636f 2f4e  huggingface.co/N
+000059c0: 6f75 7352 6573 6561 7263 682f 6c6c 616d  ousResearch/llam
+000059d0: 612d 322d 3762 2d68 6629 0a0a 3c2f 6465  a-2-7b-hf)..</de
+000059e0: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
+000059f0: 3e0a 0a3c 7375 6d6d 6172 793e 4d69 7374  >..<summary>Mist
+00005a00: 7261 6c3c 2f73 756d 6d61 7279 3e0a 0a0a  ral</summary>...
+00005a10: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
+00005a20: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 4d69  ..> **Note:** Mi
+00005a30: 7374 7261 6c20 7265 7175 6972 6573 2074  stral requires t
+00005a40: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
+00005a50: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
+00005a60: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
+00005a70: 5b6d 6973 7472 616c 5d22 0a3e 2060 6060  [mistral]".> ```
+00005a80: 0a0a 0a52 756e 2074 6865 2066 6f6c 6c6f  ...Run the follo
+00005a90: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+00005aa0: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
+00005ab0: 6120 4d69 7374 7261 6c20 7365 7276 6572  a Mistral server
+00005ac0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
+00005ad0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
+00005ae0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
+00005af0: 6d69 7374 7261 6c61 692f 4d69 7374 7261  mistralai/Mistra
+00005b00: 6c2d 3742 2d49 6e73 7472 7563 742d 7630  l-7B-Instruct-v0
+00005b10: 2e31 0a60 6060 0a49 6e20 6120 6469 6666  .1.```.In a diff
+00005b20: 6572 656e 7420 7465 726d 696e 616c 2c20  erent terminal, 
+00005b30: 7275 6e20 7468 6520 666f 6c6c 6f77 696e  run the followin
+00005b40: 6720 636f 6d6d 616e 6420 746f 2069 6e74  g command to int
+00005b50: 6572 6163 7420 7769 7468 2074 6865 2073  eract with the s
+00005b60: 6572 7665 723a 0a0a 6060 6062 6173 680a  erver:..```bash.
+00005b70: 6578 706f 7274 204f 5045 4e4c 4c4d 5f45  export OPENLLM_E
+00005b80: 4e44 504f 494e 543d 6874 7470 3a2f 2f6c  NDPOINT=http://l
+00005b90: 6f63 616c 686f 7374 3a33 3030 300a 6f70  ocalhost:3000.op
+00005ba0: 656e 6c6c 6d20 7175 6572 7920 2757 6861  enllm query 'Wha
+00005bb0: 7420 6172 6520 6c61 7267 6520 6c61 6e67  t are large lang
+00005bc0: 7561 6765 206d 6f64 656c 733f 270a 6060  uage models?'.``
+00005bd0: 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20  `...> **Note:** 
+00005be0: 416e 7920 4d69 7374 7261 6c20 7661 7269  Any Mistral vari
+00005bf0: 616e 7473 2063 616e 2062 6520 6465 706c  ants can be depl
+00005c00: 6f79 6564 2077 6974 6820 4f70 656e 4c4c  oyed with OpenLL
+00005c10: 4d2e 2056 6973 6974 2074 6865 205b 4875  M. Visit the [Hu
+00005c20: 6767 696e 6746 6163 6520 4d6f 6465 6c20  ggingFace Model 
+00005c30: 4875 625d 2868 7474 7073 3a2f 2f68 7567  Hub](https://hug
+00005c40: 6769 6e67 6661 6365 2e63 6f2f 6d6f 6465  gingface.co/mode
+00005c50: 6c73 3f73 6f72 743d 7472 656e 6469 6e67  ls?sort=trending
+00005c60: 2673 6561 7263 683d 6d69 7374 7261 6c29  &search=mistral)
+00005c70: 2074 6f20 7365 6520 6d6f 7265 204d 6973   to see more Mis
+00005c80: 7472 616c 2d63 6f6d 7061 7469 626c 6520  tral-compatible 
+00005c90: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
+00005ca0: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
+00005cb0: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
+00005cc0: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
+00005cd0: 6f77 696e 6720 4d69 7374 7261 6c20 6d6f  owing Mistral mo
+00005ce0: 6465 6c73 2076 6961 2060 6f70 656e 6c6c  dels via `openll
+00005cf0: 6d20 7374 6172 7460 3a0a 0a0a 2d20 5b48  m start`:...- [H
+00005d00: 7567 6769 6e67 4661 6365 4834 2f7a 6570  uggingFaceH4/zep
+00005d10: 6879 722d 3762 2d61 6c70 6861 5d28 6874  hyr-7b-alpha](ht
+00005d20: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00005d30: 652e 636f 2f48 7567 6769 6e67 4661 6365  e.co/HuggingFace
+00005d40: 4834 2f7a 6570 6879 722d 3762 2d61 6c70  H4/zephyr-7b-alp
+00005d50: 6861 290a 2d20 5b48 7567 6769 6e67 4661  ha).- [HuggingFa
+00005d60: 6365 4834 2f7a 6570 6879 722d 3762 2d62  ceH4/zephyr-7b-b
+00005d70: 6574 615d 2868 7474 7073 3a2f 2f68 7567  eta](https://hug
+00005d80: 6769 6e67 6661 6365 2e63 6f2f 4875 6767  gingface.co/Hugg
+00005d90: 696e 6746 6163 6548 342f 7a65 7068 7972  ingFaceH4/zephyr
+00005da0: 2d37 622d 6265 7461 290a 2d20 5b6d 6973  -7b-beta).- [mis
+00005db0: 7472 616c 6169 2f4d 6973 7472 616c 2d37  tralai/Mistral-7
+00005dc0: 422d 496e 7374 7275 6374 2d76 302e 325d  B-Instruct-v0.2]
+00005dd0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+00005de0: 6661 6365 2e63 6f2f 6d69 7374 7261 6c61  face.co/mistrala
+00005df0: 692f 4d69 7374 7261 6c2d 3742 2d49 6e73  i/Mistral-7B-Ins
+00005e00: 7472 7563 742d 7630 2e32 290a 2d20 5b6d  truct-v0.2).- [m
+00005e10: 6973 7472 616c 6169 2f4d 6973 7472 616c  istralai/Mistral
+00005e20: 2d37 422d 496e 7374 7275 6374 2d76 302e  -7B-Instruct-v0.
+00005e30: 315d 2868 7474 7073 3a2f 2f68 7567 6769  1](https://huggi
+00005e40: 6e67 6661 6365 2e63 6f2f 6d69 7374 7261  ngface.co/mistra
+00005e50: 6c61 692f 4d69 7374 7261 6c2d 3742 2d49  lai/Mistral-7B-I
+00005e60: 6e73 7472 7563 742d 7630 2e31 290a 2d20  nstruct-v0.1).- 
+00005e70: 5b6d 6973 7472 616c 6169 2f4d 6973 7472  [mistralai/Mistr
+00005e80: 616c 2d37 422d 7630 2e31 5d28 6874 7470  al-7B-v0.1](http
+00005e90: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00005ea0: 636f 2f6d 6973 7472 616c 6169 2f4d 6973  co/mistralai/Mis
+00005eb0: 7472 616c 2d37 422d 7630 2e31 290a 0a3c  tral-7B-v0.1)..<
+00005ec0: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+00005ed0: 696c 733e 0a0a 3c73 756d 6d61 7279 3e4d  ils>..<summary>M
+00005ee0: 6978 7472 616c 3c2f 7375 6d6d 6172 793e  ixtral</summary>
+00005ef0: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
+00005f00: 740a 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  t....> **Note:**
+00005f10: 204d 6978 7472 616c 2072 6571 7569 7265   Mixtral require
+00005f20: 7320 746f 2069 6e73 7461 6c6c 2077 6974  s to install wit
+00005f30: 683a 0a3e 2060 6060 6261 7368 0a3e 2070  h:.> ```bash.> p
+00005f40: 6970 2069 6e73 7461 6c6c 2022 6f70 656e  ip install "open
+00005f50: 6c6c 6d5b 6d69 7874 7261 6c5d 220a 3e20  llm[mixtral]".> 
+00005f60: 6060 600a 0a0a 5275 6e20 7468 6520 666f  ```...Run the fo
+00005f70: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+00005f80: 746f 2071 7569 636b 6c79 2073 7069 6e20  to quickly spin 
+00005f90: 7570 2061 204d 6978 7472 616c 2073 6572  up a Mixtral ser
+00005fa0: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
+00005fb0: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
+00005fc0: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
+00005fd0: 7274 206d 6973 7472 616c 6169 2f4d 6978  rt mistralai/Mix
+00005fe0: 7472 616c 2d38 7837 422d 496e 7374 7275  tral-8x7B-Instru
+00005ff0: 6374 2d76 302e 310a 6060 600a 496e 2061  ct-v0.1.```.In a
+00006000: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
+00006010: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
+00006020: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+00006030: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00006040: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
+00006050: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
+00006060: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
+00006070: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+00006080: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
+00006090: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
+000060a0: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+000060b0: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
+000060c0: 653a 2a2a 2041 6e79 204d 6978 7472 616c  e:** Any Mixtral
+000060d0: 2076 6172 6961 6e74 7320 6361 6e20 6265   variants can be
+000060e0: 2064 6570 6c6f 7965 6420 7769 7468 204f   deployed with O
+000060f0: 7065 6e4c 4c4d 2e20 5669 7369 7420 7468  penLLM. Visit th
+00006100: 6520 5b48 7567 6769 6e67 4661 6365 204d  e [HuggingFace M
+00006110: 6f64 656c 2048 7562 5d28 6874 7470 733a  odel Hub](https:
+00006120: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00006130: 2f6d 6f64 656c 733f 736f 7274 3d74 7265  /models?sort=tre
+00006140: 6e64 696e 6726 7365 6172 6368 3d6d 6978  nding&search=mix
+00006150: 7472 616c 2920 746f 2073 6565 206d 6f72  tral) to see mor
+00006160: 6520 4d69 7874 7261 6c2d 636f 6d70 6174  e Mixtral-compat
+00006170: 6962 6c65 206d 6f64 656c 732e 0a0a 0a0a  ible models.....
+00006180: 2323 2320 5375 7070 6f72 7465 6420 6d6f  ### Supported mo
+00006190: 6465 6c73 0a0a 596f 7520 6361 6e20 7370  dels..You can sp
+000061a0: 6563 6966 7920 616e 7920 6f66 2074 6865  ecify any of the
+000061b0: 2066 6f6c 6c6f 7769 6e67 204d 6978 7472   following Mixtr
+000061c0: 616c 206d 6f64 656c 7320 7669 6120 606f  al models via `o
+000061d0: 7065 6e6c 6c6d 2073 7461 7274 603a 0a0a  penllm start`:..
+000061e0: 0a2d 205b 6d69 7374 7261 6c61 692f 4d69  .- [mistralai/Mi
+000061f0: 7874 7261 6c2d 3878 3742 2d49 6e73 7472  xtral-8x7B-Instr
+00006200: 7563 742d 7630 2e31 5d28 6874 7470 733a  uct-v0.1](https:
+00006210: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00006220: 2f6d 6973 7472 616c 6169 2f4d 6978 7472  /mistralai/Mixtr
+00006230: 616c 2d38 7837 422d 496e 7374 7275 6374  al-8x7B-Instruct
+00006240: 2d76 302e 3129 0a2d 205b 6d69 7374 7261  -v0.1).- [mistra
+00006250: 6c61 692f 4d69 7874 7261 6c2d 3878 3742  lai/Mixtral-8x7B
+00006260: 2d76 302e 315d 2868 7474 7073 3a2f 2f68  -v0.1](https://h
+00006270: 7567 6769 6e67 6661 6365 2e63 6f2f 6d69  uggingface.co/mi
+00006280: 7374 7261 6c61 692f 4d69 7874 7261 6c2d  stralai/Mixtral-
+00006290: 3878 3742 2d76 302e 3129 0a0a 3c2f 6465  8x7B-v0.1)..</de
+000062a0: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
+000062b0: 3e0a 0a3c 7375 6d6d 6172 793e 4d50 543c  >..<summary>MPT<
+000062c0: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
+000062d0: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
+000062e0: 2a2a 4e6f 7465 3a2a 2a20 4d50 5420 7265  **Note:** MPT re
+000062f0: 7175 6972 6573 2074 6f20 696e 7374 616c  quires to instal
+00006300: 6c20 7769 7468 3a0a 3e20 6060 6062 6173  l with:.> ```bas
+00006310: 680a 3e20 7069 7020 696e 7374 616c 6c20  h.> pip install 
+00006320: 226f 7065 6e6c 6c6d 5b6d 7074 5d22 0a3e  "openllm[mpt]".>
+00006330: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
+00006340: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00006350: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
+00006360: 2075 7020 6120 4d50 5420 7365 7276 6572   up a MPT server
+00006370: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
+00006380: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
+00006390: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
+000063a0: 6d6f 7361 6963 6d6c 2f6d 7074 2d37 622d  mosaicml/mpt-7b-
+000063b0: 696e 7374 7275 6374 0a60 6060 0a49 6e20  instruct.```.In 
+000063c0: 6120 6469 6666 6572 656e 7420 7465 726d  a different term
+000063d0: 696e 616c 2c20 7275 6e20 7468 6520 666f  inal, run the fo
+000063e0: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+000063f0: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
+00006400: 2074 6865 2073 6572 7665 723a 0a0a 6060   the server:..``
+00006410: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
+00006420: 4e4c 4c4d 5f45 4e44 504f 494e 543d 6874  NLLM_ENDPOINT=ht
+00006430: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
+00006440: 3030 300a 6f70 656e 6c6c 6d20 7175 6572  000.openllm quer
+00006450: 7920 2757 6861 7420 6172 6520 6c61 7267  y 'What are larg
+00006460: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
+00006470: 733f 270a 6060 600a 0a0a 3e20 2a2a 4e6f  s?'.```...> **No
+00006480: 7465 3a2a 2a20 416e 7920 4d50 5420 7661  te:** Any MPT va
+00006490: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
+000064a0: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
+000064b0: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
+000064c0: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
+000064d0: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
+000064e0: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
+000064f0: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
+00006500: 6e67 2673 6561 7263 683d 6d70 7429 2074  ng&search=mpt) t
+00006510: 6f20 7365 6520 6d6f 7265 204d 5054 2d63  o see more MPT-c
+00006520: 6f6d 7061 7469 626c 6520 6d6f 6465 6c73  ompatible models
+00006530: 2e0a 0a0a 0a23 2323 2053 7570 706f 7274  .....### Support
+00006540: 6564 206d 6f64 656c 730a 0a59 6f75 2063  ed models..You c
+00006550: 616e 2073 7065 6369 6679 2061 6e79 206f  an specify any o
+00006560: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+00006570: 4d50 5420 6d6f 6465 6c73 2076 6961 2060  MPT models via `
+00006580: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
+00006590: 0a0a 2d20 5b6d 6f73 6169 636d 6c2f 6d70  ..- [mosaicml/mp
+000065a0: 742d 3762 5d28 6874 7470 733a 2f2f 6875  t-7b](https://hu
+000065b0: 6767 696e 6766 6163 652e 636f 2f6d 6f73  ggingface.co/mos
+000065c0: 6169 636d 6c2f 6d70 742d 3762 290a 2d20  aicml/mpt-7b).- 
+000065d0: 5b6d 6f73 6169 636d 6c2f 6d70 742d 3762  [mosaicml/mpt-7b
+000065e0: 2d69 6e73 7472 7563 745d 2868 7474 7073  -instruct](https
+000065f0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006600: 6f2f 6d6f 7361 6963 6d6c 2f6d 7074 2d37  o/mosaicml/mpt-7
+00006610: 622d 696e 7374 7275 6374 290a 2d20 5b6d  b-instruct).- [m
+00006620: 6f73 6169 636d 6c2f 6d70 742d 3762 2d63  osaicml/mpt-7b-c
+00006630: 6861 745d 2868 7474 7073 3a2f 2f68 7567  hat](https://hug
+00006640: 6769 6e67 6661 6365 2e63 6f2f 6d6f 7361  gingface.co/mosa
+00006650: 6963 6d6c 2f6d 7074 2d37 622d 6368 6174  icml/mpt-7b-chat
+00006660: 290a 2d20 5b6d 6f73 6169 636d 6c2f 6d70  ).- [mosaicml/mp
+00006670: 742d 3762 2d73 746f 7279 7772 6974 6572  t-7b-storywriter
+00006680: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00006690: 6766 6163 652e 636f 2f6d 6f73 6169 636d  gface.co/mosaicm
+000066a0: 6c2f 6d70 742d 3762 2d73 746f 7279 7772  l/mpt-7b-storywr
+000066b0: 6974 6572 290a 2d20 5b6d 6f73 6169 636d  iter).- [mosaicm
+000066c0: 6c2f 6d70 742d 3330 625d 2868 7474 7073  l/mpt-30b](https
+000066d0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+000066e0: 6f2f 6d6f 7361 6963 6d6c 2f6d 7074 2d33  o/mosaicml/mpt-3
+000066f0: 3062 290a 2d20 5b6d 6f73 6169 636d 6c2f  0b).- [mosaicml/
+00006700: 6d70 742d 3330 622d 696e 7374 7275 6374  mpt-30b-instruct
+00006710: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00006720: 6766 6163 652e 636f 2f6d 6f73 6169 636d  gface.co/mosaicm
+00006730: 6c2f 6d70 742d 3330 622d 696e 7374 7275  l/mpt-30b-instru
+00006740: 6374 290a 2d20 5b6d 6f73 6169 636d 6c2f  ct).- [mosaicml/
+00006750: 6d70 742d 3330 622d 6368 6174 5d28 6874  mpt-30b-chat](ht
+00006760: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00006770: 652e 636f 2f6d 6f73 6169 636d 6c2f 6d70  e.co/mosaicml/mp
+00006780: 742d 3330 622d 6368 6174 290a 0a3c 2f64  t-30b-chat)..</d
+00006790: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
+000067a0: 733e 0a0a 3c73 756d 6d61 7279 3e4f 5054  s>..<summary>OPT
+000067b0: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
+000067c0: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
+000067d0: 202a 2a4e 6f74 653a 2a2a 204f 5054 2072   **Note:** OPT r
+000067e0: 6571 7569 7265 7320 746f 2069 6e73 7461  equires to insta
+000067f0: 6c6c 2077 6974 683a 0a3e 2060 6060 6261  ll with:.> ```ba
+00006800: 7368 0a3e 2070 6970 2069 6e73 7461 6c6c  sh.> pip install
+00006810: 2022 6f70 656e 6c6c 6d5b 6f70 745d 220a   "openllm[opt]".
+00006820: 3e20 6060 600a 0a0a 5275 6e20 7468 6520  > ```...Run the 
+00006830: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00006840: 6420 746f 2071 7569 636b 6c79 2073 7069  d to quickly spi
+00006850: 6e20 7570 2061 204f 5054 2073 6572 7665  n up a OPT serve
+00006860: 723a 0a0a 6060 6062 6173 680a 6f70 656e  r:..```bash.open
+00006870: 6c6c 6d20 7374 6172 7420 6661 6365 626f  llm start facebo
+00006880: 6f6b 2f6f 7074 2d31 2e33 620a 6060 600a  ok/opt-1.3b.```.
+00006890: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
+000068a0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
+000068b0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+000068c0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
+000068d0: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
+000068e0: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
+000068f0: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
+00006900: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
+00006910: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
+00006920: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
+00006930: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
+00006940: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
+00006950: 2a4e 6f74 653a 2a2a 2041 6e79 204f 5054  *Note:** Any OPT
+00006960: 2076 6172 6961 6e74 7320 6361 6e20 6265   variants can be
+00006970: 2064 6570 6c6f 7965 6420 7769 7468 204f   deployed with O
+00006980: 7065 6e4c 4c4d 2e20 5669 7369 7420 7468  penLLM. Visit th
+00006990: 6520 5b48 7567 6769 6e67 4661 6365 204d  e [HuggingFace M
+000069a0: 6f64 656c 2048 7562 5d28 6874 7470 733a  odel Hub](https:
+000069b0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+000069c0: 2f6d 6f64 656c 733f 736f 7274 3d74 7265  /models?sort=tre
+000069d0: 6e64 696e 6726 7365 6172 6368 3d6f 7074  nding&search=opt
+000069e0: 2920 746f 2073 6565 206d 6f72 6520 4f50  ) to see more OP
+000069f0: 542d 636f 6d70 6174 6962 6c65 206d 6f64  T-compatible mod
+00006a00: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
+00006a10: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
+00006a20: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
+00006a30: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
+00006a40: 6e67 204f 5054 206d 6f64 656c 7320 7669  ng OPT models vi
+00006a50: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
+00006a60: 603a 0a0a 0a2d 205b 6661 6365 626f 6f6b  `:...- [facebook
+00006a70: 2f6f 7074 2d31 3235 6d5d 2868 7474 7073  /opt-125m](https
+00006a80: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006a90: 6f2f 6661 6365 626f 6f6b 2f6f 7074 2d31  o/facebook/opt-1
+00006aa0: 3235 6d29 0a2d 205b 6661 6365 626f 6f6b  25m).- [facebook
+00006ab0: 2f6f 7074 2d33 3530 6d5d 2868 7474 7073  /opt-350m](https
+00006ac0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006ad0: 6f2f 6661 6365 626f 6f6b 2f6f 7074 2d33  o/facebook/opt-3
+00006ae0: 3530 6d29 0a2d 205b 6661 6365 626f 6f6b  50m).- [facebook
+00006af0: 2f6f 7074 2d31 2e33 625d 2868 7474 7073  /opt-1.3b](https
+00006b00: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006b10: 6f2f 6661 6365 626f 6f6b 2f6f 7074 2d31  o/facebook/opt-1
+00006b20: 2e33 6229 0a2d 205b 6661 6365 626f 6f6b  .3b).- [facebook
+00006b30: 2f6f 7074 2d32 2e37 625d 2868 7474 7073  /opt-2.7b](https
+00006b40: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006b50: 6f2f 6661 6365 626f 6f6b 2f6f 7074 2d32  o/facebook/opt-2
+00006b60: 2e37 6229 0a2d 205b 6661 6365 626f 6f6b  .7b).- [facebook
+00006b70: 2f6f 7074 2d36 2e37 625d 2868 7474 7073  /opt-6.7b](https
+00006b80: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006b90: 6f2f 6661 6365 626f 6f6b 2f6f 7074 2d36  o/facebook/opt-6
+00006ba0: 2e37 6229 0a2d 205b 6661 6365 626f 6f6b  .7b).- [facebook
+00006bb0: 2f6f 7074 2d36 3662 5d28 6874 7470 733a  /opt-66b](https:
+00006bc0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00006bd0: 2f66 6163 6562 6f6f 6b2f 6f70 742d 3636  /facebook/opt-66
+00006be0: 6229 0a0a 3c2f 6465 7461 696c 733e 0a0a  b)..</details>..
+00006bf0: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+00006c00: 6172 793e 5068 693c 2f73 756d 6d61 7279  ary>Phi</summary
+00006c10: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
+00006c20: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
+00006c30: 2a20 5068 6920 7265 7175 6972 6573 2074  * Phi requires t
+00006c40: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
+00006c50: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
+00006c60: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
+00006c70: 5b70 6869 5d22 0a3e 2060 6060 0a0a 0a52  [phi]".> ```...R
+00006c80: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
+00006c90: 2063 6f6d 6d61 6e64 2074 6f20 7175 6963   command to quic
+00006ca0: 6b6c 7920 7370 696e 2075 7020 6120 5068  kly spin up a Ph
+00006cb0: 6920 7365 7276 6572 3a0a 0a60 6060 6261  i server:..```ba
+00006cc0: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
+00006cd0: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
+00006ce0: 6d20 7374 6172 7420 6d69 6372 6f73 6f66  m start microsof
+00006cf0: 742f 7068 692d 320a 6060 600a 496e 2061  t/phi-2.```.In a
+00006d00: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
+00006d10: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
+00006d20: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+00006d30: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00006d40: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
+00006d50: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
+00006d60: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
+00006d70: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+00006d80: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
+00006d90: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
+00006da0: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+00006db0: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
+00006dc0: 653a 2a2a 2041 6e79 2050 6869 2076 6172  e:** Any Phi var
+00006dd0: 6961 6e74 7320 6361 6e20 6265 2064 6570  iants can be dep
+00006de0: 6c6f 7965 6420 7769 7468 204f 7065 6e4c  loyed with OpenL
+00006df0: 4c4d 2e20 5669 7369 7420 7468 6520 5b48  LM. Visit the [H
+00006e00: 7567 6769 6e67 4661 6365 204d 6f64 656c  uggingFace Model
+00006e10: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
+00006e20: 6767 696e 6766 6163 652e 636f 2f6d 6f64  ggingface.co/mod
+00006e30: 656c 733f 736f 7274 3d74 7265 6e64 696e  els?sort=trendin
+00006e40: 6726 7365 6172 6368 3d70 6869 2920 746f  g&search=phi) to
+00006e50: 2073 6565 206d 6f72 6520 5068 692d 636f   see more Phi-co
+00006e60: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
+00006e70: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
+00006e80: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
+00006e90: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
+00006ea0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2050   the following P
+00006eb0: 6869 206d 6f64 656c 7320 7669 6120 606f  hi models via `o
+00006ec0: 7065 6e6c 6c6d 2073 7461 7274 603a 0a0a  penllm start`:..
+00006ed0: 0a2d 205b 6d69 6372 6f73 6f66 742f 7068  .- [microsoft/ph
+00006ee0: 692d 325d 2868 7474 7073 3a2f 2f68 7567  i-2](https://hug
+00006ef0: 6769 6e67 6661 6365 2e63 6f2f 6d69 6372  gingface.co/micr
+00006f00: 6f73 6f66 742f 7068 692d 3229 0a2d 205b  osoft/phi-2).- [
+00006f10: 6d69 6372 6f73 6f66 742f 7068 692d 315f  microsoft/phi-1_
+00006f20: 355d 2868 7474 7073 3a2f 2f68 7567 6769  5](https://huggi
+00006f30: 6e67 6661 6365 2e63 6f2f 6d69 6372 6f73  ngface.co/micros
+00006f40: 6f66 742f 7068 692d 315f 3529 0a0a 3c2f  oft/phi-1_5)..</
+00006f50: 6465 7461 696c 733e 0a0a 3c64 6574 6169  details>..<detai
+00006f60: 6c73 3e0a 0a3c 7375 6d6d 6172 793e 5177  ls>..<summary>Qw
+00006f70: 656e 3c2f 7375 6d6d 6172 793e 0a0a 0a23  en</summary>...#
+00006f80: 2323 2051 7569 636b 7374 6172 740a 0a0a  ## Quickstart...
+00006f90: 0a3e 202a 2a4e 6f74 653a 2a2a 2051 7765  .> **Note:** Qwe
+00006fa0: 6e20 7265 7175 6972 6573 2074 6f20 696e  n requires to in
+00006fb0: 7374 616c 6c20 7769 7468 3a0a 3e20 6060  stall with:.> ``
+00006fc0: 6062 6173 680a 3e20 7069 7020 696e 7374  `bash.> pip inst
+00006fd0: 616c 6c20 226f 7065 6e6c 6c6d 5b71 7765  all "openllm[qwe
+00006fe0: 6e5d 220a 3e20 6060 600a 0a0a 5275 6e20  n]".> ```...Run 
+00006ff0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00007000: 6d6d 616e 6420 746f 2071 7569 636b 6c79  mmand to quickly
+00007010: 2073 7069 6e20 7570 2061 2051 7765 6e20   spin up a Qwen 
+00007020: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+00007030: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
+00007040: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
+00007050: 7374 6172 7420 7177 656e 2f51 7765 6e2d  start qwen/Qwen-
+00007060: 3742 2d43 6861 740a 6060 600a 496e 2061  7B-Chat.```.In a
+00007070: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
+00007080: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
+00007090: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+000070a0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+000070b0: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
+000070c0: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
+000070d0: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
+000070e0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+000070f0: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
+00007100: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
+00007110: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+00007120: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
+00007130: 653a 2a2a 2041 6e79 2051 7765 6e20 7661  e:** Any Qwen va
+00007140: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
+00007150: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
+00007160: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
+00007170: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
+00007180: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
+00007190: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
+000071a0: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
+000071b0: 6e67 2673 6561 7263 683d 7177 656e 2920  ng&search=qwen) 
+000071c0: 746f 2073 6565 206d 6f72 6520 5177 656e  to see more Qwen
+000071d0: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
+000071e0: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
+000071f0: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
+00007200: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
+00007210: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00007220: 6720 5177 656e 206d 6f64 656c 7320 7669  g Qwen models vi
+00007230: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
+00007240: 603a 0a0a 0a2d 205b 7177 656e 2f51 7765  `:...- [qwen/Qwe
+00007250: 6e2d 3742 2d43 6861 745d 2868 7474 7073  n-7B-Chat](https
+00007260: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00007270: 6f2f 7177 656e 2f51 7765 6e2d 3742 2d43  o/qwen/Qwen-7B-C
+00007280: 6861 7429 0a2d 205b 7177 656e 2f51 7765  hat).- [qwen/Qwe
+00007290: 6e2d 3742 2d43 6861 742d 496e 7438 5d28  n-7B-Chat-Int8](
+000072a0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+000072b0: 6163 652e 636f 2f71 7765 6e2f 5177 656e  ace.co/qwen/Qwen
+000072c0: 2d37 422d 4368 6174 2d49 6e74 3829 0a2d  -7B-Chat-Int8).-
+000072d0: 205b 7177 656e 2f51 7765 6e2d 3742 2d43   [qwen/Qwen-7B-C
+000072e0: 6861 742d 496e 7434 5d28 6874 7470 733a  hat-Int4](https:
+000072f0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00007300: 2f71 7765 6e2f 5177 656e 2d37 422d 4368  /qwen/Qwen-7B-Ch
+00007310: 6174 2d49 6e74 3429 0a2d 205b 7177 656e  at-Int4).- [qwen
+00007320: 2f51 7765 6e2d 3134 422d 4368 6174 5d28  /Qwen-14B-Chat](
+00007330: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00007340: 6163 652e 636f 2f71 7765 6e2f 5177 656e  ace.co/qwen/Qwen
+00007350: 2d31 3442 2d43 6861 7429 0a2d 205b 7177  -14B-Chat).- [qw
+00007360: 656e 2f51 7765 6e2d 3134 422d 4368 6174  en/Qwen-14B-Chat
+00007370: 2d49 6e74 385d 2868 7474 7073 3a2f 2f68  -Int8](https://h
+00007380: 7567 6769 6e67 6661 6365 2e63 6f2f 7177  uggingface.co/qw
+00007390: 656e 2f51 7765 6e2d 3134 422d 4368 6174  en/Qwen-14B-Chat
+000073a0: 2d49 6e74 3829 0a2d 205b 7177 656e 2f51  -Int8).- [qwen/Q
+000073b0: 7765 6e2d 3134 422d 4368 6174 2d49 6e74  wen-14B-Chat-Int
+000073c0: 345d 2868 7474 7073 3a2f 2f68 7567 6769  4](https://huggi
+000073d0: 6e67 6661 6365 2e63 6f2f 7177 656e 2f51  ngface.co/qwen/Q
+000073e0: 7765 6e2d 3134 422d 4368 6174 2d49 6e74  wen-14B-Chat-Int
+000073f0: 3429 0a0a 3c2f 6465 7461 696c 733e 0a0a  4)..</details>..
+00007400: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+00007410: 6172 793e 5374 6162 6c65 4c4d 3c2f 7375  ary>StableLM</su
+00007420: 6d6d 6172 793e 0a0a 0a23 2323 2051 7569  mmary>...### Qui
+00007430: 636b 7374 6172 740a 0a0a 0a3e 202a 2a4e  ckstart....> **N
+00007440: 6f74 653a 2a2a 2053 7461 626c 654c 4d20  ote:** StableLM 
+00007450: 7265 7175 6972 6573 2074 6f20 696e 7374  requires to inst
+00007460: 616c 6c20 7769 7468 3a0a 3e20 6060 6062  all with:.> ```b
+00007470: 6173 680a 3e20 7069 7020 696e 7374 616c  ash.> pip instal
+00007480: 6c20 226f 7065 6e6c 6c6d 5b73 7461 626c  l "openllm[stabl
+00007490: 656c 6d5d 220a 3e20 6060 600a 0a0a 5275  elm]".> ```...Ru
+000074a0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000074b0: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
+000074c0: 6c79 2073 7069 6e20 7570 2061 2053 7461  ly spin up a Sta
+000074d0: 626c 654c 4d20 7365 7276 6572 3a0a 0a60  bleLM server:..`
+000074e0: 6060 6261 7368 0a54 5255 5354 5f52 454d  ``bash.TRUST_REM
+000074f0: 4f54 455f 434f 4445 3d54 7275 6520 6f70  OTE_CODE=True op
+00007500: 656e 6c6c 6d20 7374 6172 7420 7374 6162  enllm start stab
+00007510: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
+00007520: 2d74 756e 6564 2d61 6c70 6861 2d33 620a  -tuned-alpha-3b.
+00007530: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
+00007540: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
+00007550: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00007560: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
+00007570: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
+00007580: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
+00007590: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
+000075a0: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
+000075b0: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
+000075c0: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
+000075d0: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
+000075e0: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
+000075f0: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
+00007600: 2053 7461 626c 654c 4d20 7661 7269 616e   StableLM varian
+00007610: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
+00007620: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
+00007630: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
+00007640: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
+00007650: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00007660: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
+00007670: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
+00007680: 6561 7263 683d 7374 6162 6c65 6c6d 2920  earch=stablelm) 
+00007690: 746f 2073 6565 206d 6f72 6520 5374 6162  to see more Stab
+000076a0: 6c65 4c4d 2d63 6f6d 7061 7469 626c 6520  leLM-compatible 
+000076b0: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
+000076c0: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
+000076d0: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
+000076e0: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
+000076f0: 6f77 696e 6720 5374 6162 6c65 4c4d 206d  owing StableLM m
+00007700: 6f64 656c 7320 7669 6120 606f 7065 6e6c  odels via `openl
+00007710: 6c6d 2073 7461 7274 603a 0a0a 0a2d 205b  lm start`:...- [
+00007720: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
+00007730: 6c65 6c6d 2d74 756e 6564 2d61 6c70 6861  lelm-tuned-alpha
+00007740: 2d33 625d 2868 7474 7073 3a2f 2f68 7567  -3b](https://hug
+00007750: 6769 6e67 6661 6365 2e63 6f2f 7374 6162  gingface.co/stab
+00007760: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
+00007770: 2d74 756e 6564 2d61 6c70 6861 2d33 6229  -tuned-alpha-3b)
+00007780: 0a2d 205b 7374 6162 696c 6974 7961 692f  .- [stabilityai/
+00007790: 7374 6162 6c65 6c6d 2d74 756e 6564 2d61  stablelm-tuned-a
+000077a0: 6c70 6861 2d37 625d 2868 7474 7073 3a2f  lpha-7b](https:/
+000077b0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+000077c0: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
+000077d0: 6c65 6c6d 2d74 756e 6564 2d61 6c70 6861  lelm-tuned-alpha
+000077e0: 2d37 6229 0a2d 205b 7374 6162 696c 6974  -7b).- [stabilit
+000077f0: 7961 692f 7374 6162 6c65 6c6d 2d62 6173  yai/stablelm-bas
+00007800: 652d 616c 7068 612d 3362 5d28 6874 7470  e-alpha-3b](http
+00007810: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00007820: 636f 2f73 7461 6269 6c69 7479 6169 2f73  co/stabilityai/s
+00007830: 7461 626c 656c 6d2d 6261 7365 2d61 6c70  tablelm-base-alp
+00007840: 6861 2d33 6229 0a2d 205b 7374 6162 696c  ha-3b).- [stabil
+00007850: 6974 7961 692f 7374 6162 6c65 6c6d 2d62  ityai/stablelm-b
+00007860: 6173 652d 616c 7068 612d 3762 5d28 6874  ase-alpha-7b](ht
+00007870: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00007880: 652e 636f 2f73 7461 6269 6c69 7479 6169  e.co/stabilityai
+00007890: 2f73 7461 626c 656c 6d2d 6261 7365 2d61  /stablelm-base-a
+000078a0: 6c70 6861 2d37 6229 0a0a 3c2f 6465 7461  lpha-7b)..</deta
+000078b0: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
+000078c0: 0a3c 7375 6d6d 6172 793e 5374 6172 436f  .<summary>StarCo
+000078d0: 6465 723c 2f73 756d 6d61 7279 3e0a 0a0a  der</summary>...
+000078e0: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
+000078f0: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 5374  ..> **Note:** St
+00007900: 6172 436f 6465 7220 7265 7175 6972 6573  arCoder requires
+00007910: 2074 6f20 696e 7374 616c 6c20 7769 7468   to install with
+00007920: 3a0a 3e20 6060 6062 6173 680a 3e20 7069  :.> ```bash.> pi
+00007930: 7020 696e 7374 616c 6c20 226f 7065 6e6c  p install "openl
+00007940: 6c6d 5b73 7461 7263 6f64 6572 5d22 0a3e  lm[starcoder]".>
+00007950: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
+00007960: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00007970: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
+00007980: 2075 7020 6120 5374 6172 436f 6465 7220   up a StarCoder 
+00007990: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+000079a0: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
+000079b0: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
+000079c0: 7374 6172 7420 6269 6763 6f64 652f 7374  start bigcode/st
+000079d0: 6172 636f 6465 720a 6060 600a 496e 2061  arcoder.```.In a
+000079e0: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
+000079f0: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
+00007a00: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+00007a10: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
+00007a20: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
+00007a30: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
+00007a40: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
+00007a50: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+00007a60: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
+00007a70: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
+00007a80: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
+00007a90: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
+00007aa0: 653a 2a2a 2041 6e79 2053 7461 7243 6f64  e:** Any StarCod
+00007ab0: 6572 2076 6172 6961 6e74 7320 6361 6e20  er variants can 
+00007ac0: 6265 2064 6570 6c6f 7965 6420 7769 7468  be deployed with
+00007ad0: 204f 7065 6e4c 4c4d 2e20 5669 7369 7420   OpenLLM. Visit 
+00007ae0: 7468 6520 5b48 7567 6769 6e67 4661 6365  the [HuggingFace
+00007af0: 204d 6f64 656c 2048 7562 5d28 6874 7470   Model Hub](http
+00007b00: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00007b10: 636f 2f6d 6f64 656c 733f 736f 7274 3d74  co/models?sort=t
+00007b20: 7265 6e64 696e 6726 7365 6172 6368 3d73  rending&search=s
+00007b30: 7461 7263 6f64 6572 2920 746f 2073 6565  tarcoder) to see
+00007b40: 206d 6f72 6520 5374 6172 436f 6465 722d   more StarCoder-
+00007b50: 636f 6d70 6174 6962 6c65 206d 6f64 656c  compatible model
+00007b60: 732e 0a0a 0a0a 2323 2320 5375 7070 6f72  s.....### Suppor
+00007b70: 7465 6420 6d6f 6465 6c73 0a0a 596f 7520  ted models..You 
+00007b80: 6361 6e20 7370 6563 6966 7920 616e 7920  can specify any 
+00007b90: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
+00007ba0: 2053 7461 7243 6f64 6572 206d 6f64 656c   StarCoder model
+00007bb0: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
+00007bc0: 7461 7274 603a 0a0a 0a2d 205b 6269 6763  tart`:...- [bigc
+00007bd0: 6f64 652f 7374 6172 636f 6465 725d 2868  ode/starcoder](h
+00007be0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00007bf0: 6365 2e63 6f2f 6269 6763 6f64 652f 7374  ce.co/bigcode/st
+00007c00: 6172 636f 6465 7229 0a2d 205b 6269 6763  arcoder).- [bigc
+00007c10: 6f64 652f 7374 6172 636f 6465 7262 6173  ode/starcoderbas
+00007c20: 655d 2868 7474 7073 3a2f 2f68 7567 6769  e](https://huggi
+00007c30: 6e67 6661 6365 2e63 6f2f 6269 6763 6f64  ngface.co/bigcod
+00007c40: 652f 7374 6172 636f 6465 7262 6173 6529  e/starcoderbase)
+00007c50: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
+00007c60: 6574 6169 6c73 3e0a 0a3c 7375 6d6d 6172  etails>..<summar
+00007c70: 793e 5969 3c2f 7375 6d6d 6172 793e 0a0a  y>Yi</summary>..
+00007c80: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
+00007c90: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2059  ...> **Note:** Y
+00007ca0: 6920 7265 7175 6972 6573 2074 6f20 696e  i requires to in
+00007cb0: 7374 616c 6c20 7769 7468 3a0a 3e20 6060  stall with:.> ``
+00007cc0: 6062 6173 680a 3e20 7069 7020 696e 7374  `bash.> pip inst
+00007cd0: 616c 6c20 226f 7065 6e6c 6c6d 5b79 695d  all "openllm[yi]
+00007ce0: 220a 3e20 6060 600a 0a0a 5275 6e20 7468  ".> ```...Run th
+00007cf0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00007d00: 616e 6420 746f 2071 7569 636b 6c79 2073  and to quickly s
+00007d10: 7069 6e20 7570 2061 2059 6920 7365 7276  pin up a Yi serv
+00007d20: 6572 3a0a 0a60 6060 6261 7368 0a54 5255  er:..```bash.TRU
+00007d30: 5354 5f52 454d 4f54 455f 434f 4445 3d54  ST_REMOTE_CODE=T
+00007d40: 7275 6520 6f70 656e 6c6c 6d20 7374 6172  rue openllm star
+00007d50: 7420 3031 2d61 692f 5969 2d36 420a 6060  t 01-ai/Yi-6B.``
+00007d60: 600a 496e 2061 2064 6966 6665 7265 6e74  `.In a different
+00007d70: 2074 6572 6d69 6e61 6c2c 2072 756e 2074   terminal, run t
+00007d80: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00007d90: 6d61 6e64 2074 6f20 696e 7465 7261 6374  mand to interact
+00007da0: 2077 6974 6820 7468 6520 7365 7276 6572   with the server
+00007db0: 3a0a 0a60 6060 6261 7368 0a65 7870 6f72  :..```bash.expor
+00007dc0: 7420 4f50 454e 4c4c 4d5f 454e 4450 4f49  t OPENLLM_ENDPOI
+00007dd0: 4e54 3d68 7474 703a 2f2f 6c6f 6361 6c68  NT=http://localh
+00007de0: 6f73 743a 3330 3030 0a6f 7065 6e6c 6c6d  ost:3000.openllm
+00007df0: 2071 7565 7279 2027 5768 6174 2061 7265   query 'What are
+00007e00: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
+00007e10: 6d6f 6465 6c73 3f27 0a60 6060 0a0a 0a3e  models?'.```...>
+00007e20: 202a 2a4e 6f74 653a 2a2a 2041 6e79 2059   **Note:** Any Y
+00007e30: 6920 7661 7269 616e 7473 2063 616e 2062  i variants can b
+00007e40: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
+00007e50: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
+00007e60: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
+00007e70: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
+00007e80: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00007e90: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
+00007ea0: 656e 6469 6e67 2673 6561 7263 683d 7969  ending&search=yi
+00007eb0: 2920 746f 2073 6565 206d 6f72 6520 5969  ) to see more Yi
+00007ec0: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
+00007ed0: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
+00007ee0: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
+00007ef0: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
+00007f00: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00007f10: 6720 5969 206d 6f64 656c 7320 7669 6120  g Yi models via 
+00007f20: 606f 7065 6e6c 6c6d 2073 7461 7274 603a  `openllm start`:
+00007f30: 0a0a 0a2d 205b 3031 2d61 692f 5969 2d36  ...- [01-ai/Yi-6
+00007f40: 425d 2868 7474 7073 3a2f 2f68 7567 6769  B](https://huggi
+00007f50: 6e67 6661 6365 2e63 6f2f 3031 2d61 692f  ngface.co/01-ai/
+00007f60: 5969 2d36 4229 0a2d 205b 3031 2d61 692f  Yi-6B).- [01-ai/
+00007f70: 5969 2d33 3442 5d28 6874 7470 733a 2f2f  Yi-34B](https://
+00007f80: 6875 6767 696e 6766 6163 652e 636f 2f30  huggingface.co/0
+00007f90: 312d 6169 2f59 692d 3334 4229 0a2d 205b  1-ai/Yi-34B).- [
+00007fa0: 3031 2d61 692f 5969 2d36 422d 3230 304b  01-ai/Yi-6B-200K
+00007fb0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00007fc0: 6766 6163 652e 636f 2f30 312d 6169 2f59  gface.co/01-ai/Y
+00007fd0: 692d 3642 2d32 3030 4b29 0a2d 205b 3031  i-6B-200K).- [01
+00007fe0: 2d61 692f 5969 2d33 3442 2d32 3030 4b5d  -ai/Yi-34B-200K]
+00007ff0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+00008000: 6661 6365 2e63 6f2f 3031 2d61 692f 5969  face.co/01-ai/Yi
+00008010: 2d33 3442 2d32 3030 4b29 0a0a 3c2f 6465  -34B-200K)..</de
+00008020: 7461 696c 733e 0a0a 3c21 2d2d 2075 7064  tails>..<!-- upd
+00008030: 6174 652d 7265 6164 6d65 2e70 793a 2073  ate-readme.py: s
+00008040: 746f 7020 2d2d 3e0a 0a4d 6f72 6520 6d6f  top -->..More mo
+00008050: 6465 6c73 2077 696c 6c20 6265 2069 6e74  dels will be int
+00008060: 6567 7261 7465 6420 7769 7468 204f 7065  egrated with Ope
+00008070: 6e4c 4c4d 2061 6e64 2077 6520 7765 6c63  nLLM and we welc
+00008080: 6f6d 6520 796f 7572 2063 6f6e 7472 6962  ome your contrib
+00008090: 7574 696f 6e73 2069 6620 796f 7520 7761  utions if you wa
+000080a0: 6e74 2074 6f20 696e 636f 7270 6f72 6174  nt to incorporat
+000080b0: 6520 796f 7572 2063 7573 746f 6d20 4c4c  e your custom LL
+000080c0: 4d73 2069 6e74 6f20 7468 6520 6563 6f73  Ms into the ecos
+000080d0: 7973 7465 6d2e 2043 6865 636b 206f 7574  ystem. Check out
+000080e0: 205b 4164 6469 6e67 2061 204e 6577 204d   [Adding a New M
+000080f0: 6f64 656c 2047 7569 6465 5d28 6874 7470  odel Guide](http
+00008100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+00008110: 656e 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62  entoml/OpenLLM/b
+00008120: 6c6f 622f 6d61 696e 2f41 4444 494e 475f  lob/main/ADDING_
+00008130: 4e45 575f 4d4f 4445 4c2e 6d64 2920 746f  NEW_MODEL.md) to
+00008140: 206c 6561 726e 206d 6f72 652e 0a0a 2323   learn more...##
+00008150: 20f0 9f92 bb20 5275 6e20 796f 7572 206d   .... Run your m
+00008160: 6f64 656c 206f 6e20 6d75 6c74 6970 6c65  odel on multiple
+00008170: 2047 5055 730a 0a4f 7065 6e4c 4c4d 2061   GPUs..OpenLLM a
+00008180: 6c6c 6f77 7320 796f 7520 746f 2073 7461  llows you to sta
+00008190: 7274 2079 6f75 7220 6d6f 6465 6c20 7365  rt your model se
+000081a0: 7276 6572 206f 6e20 6d75 6c74 6970 6c65  rver on multiple
+000081b0: 2047 5055 7320 616e 6420 7370 6563 6966   GPUs and specif
+000081c0: 7920 7468 6520 6e75 6d62 6572 206f 6620  y the number of 
+000081d0: 776f 726b 6572 7320 7065 7220 7265 736f  workers per reso
+000081e0: 7572 6365 2061 7373 6967 6e65 6420 7573  urce assigned us
+000081f0: 696e 6720 7468 6520 602d 2d77 6f72 6b65  ing the `--worke
+00008200: 7273 2d70 6572 2d72 6573 6f75 7263 6560  rs-per-resource`
+00008210: 206f 7074 696f 6e2e 2046 6f72 2065 7861   option. For exa
+00008220: 6d70 6c65 2c20 6966 2079 6f75 2068 6176  mple, if you hav
+00008230: 6520 3420 6176 6169 6c61 626c 6520 4750  e 4 available GP
+00008240: 5573 2c20 796f 7520 7365 7420 7468 6520  Us, you set the 
+00008250: 7661 6c75 6520 6173 206f 6e65 2064 6976  value as one div
+00008260: 6964 6564 2062 7920 7468 6520 6e75 6d62  ided by the numb
+00008270: 6572 2061 7320 6f6e 6c79 206f 6e65 2069  er as only one i
+00008280: 6e73 7461 6e63 6520 6f66 2074 6865 2052  nstance of the R
+00008290: 756e 6e65 7220 7365 7276 6572 2077 696c  unner server wil
+000082a0: 6c20 6265 2073 7061 776e 6564 2e0a 0a60  l be spawned...`
+000082b0: 6060 6261 7368 0a54 5255 5354 5f52 454d  ``bash.TRUST_REM
+000082c0: 4f54 455f 434f 4445 3d54 7275 6520 6f70  OTE_CODE=True op
+000082d0: 656e 6c6c 6d20 7374 6172 7420 6d69 6372  enllm start micr
+000082e0: 6f73 6f66 742f 7068 692d 3220 2d2d 776f  osoft/phi-2 --wo
+000082f0: 726b 6572 732d 7065 722d 7265 736f 7572  rkers-per-resour
+00008300: 6365 2030 2e32 350a 6060 600a 0a3e 205b  ce 0.25.```..> [
+00008310: 214e 4f54 455d 0a3e 2054 6865 2061 6d6f  !NOTE].> The amo
+00008320: 756e 7420 6f66 2047 5055 7320 7265 7175  unt of GPUs requ
+00008330: 6972 6564 2064 6570 656e 6473 206f 6e20  ired depends on 
+00008340: 7468 6520 6d6f 6465 6c20 7369 7a65 2069  the model size i
+00008350: 7473 656c 662e 0a3e 2059 6f75 2063 616e  tself..> You can
+00008360: 2075 7365 205b 7468 6520 4d6f 6465 6c20   use [the Model 
+00008370: 4d65 6d6f 7279 2043 616c 6375 6c61 746f  Memory Calculato
+00008380: 7220 6672 6f6d 2048 7567 6769 6e67 2046  r from Hugging F
+00008390: 6163 655d 2868 7474 7073 3a2f 2f68 7567  ace](https://hug
+000083a0: 6769 6e67 6661 6365 2e63 6f2f 7370 6163  gingface.co/spac
+000083b0: 6573 2f68 662d 6163 6365 6c65 7261 7465  es/hf-accelerate
+000083c0: 2f6d 6f64 656c 2d6d 656d 6f72 792d 7573  /model-memory-us
+000083d0: 6167 6529 2074 6f0a 3e20 6361 6c63 756c  age) to.> calcul
+000083e0: 6174 6520 686f 7720 6d75 6368 2076 5241  ate how much vRA
+000083f0: 4d20 6973 206e 6565 6465 6420 746f 2074  M is needed to t
+00008400: 7261 696e 2061 6e64 2070 6572 666f 726d  rain and perform
+00008410: 2062 6967 206d 6f64 656c 0a3e 2069 6e66   big model.> inf
+00008420: 6572 656e 6365 206f 6e20 6120 6d6f 6465  erence on a mode
+00008430: 6c20 616e 6420 7468 656e 2070 6c61 6e20  l and then plan 
+00008440: 796f 7572 2047 5055 2073 7472 6174 6567  your GPU strateg
+00008450: 7920 6261 7365 6420 6f6e 2069 742e 0a0a  y based on it...
+00008460: 5768 656e 2075 7369 6e67 2074 6865 2060  When using the `
+00008470: 2d2d 776f 726b 6572 732d 7065 722d 7265  --workers-per-re
+00008480: 736f 7572 6365 6020 6f70 7469 6f6e 2077  source` option w
+00008490: 6974 6820 7468 6520 606f 7065 6e6c 6c6d  ith the `openllm
+000084a0: 2062 7569 6c64 6020 636f 6d6d 616e 642c   build` command,
+000084b0: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
+000084c0: 2076 6172 6961 626c 6520 6973 2073 6176   variable is sav
+000084d0: 6564 2069 6e74 6f20 7468 6520 7265 7375  ed into the resu
+000084e0: 6c74 696e 6720 4265 6e74 6f2e 0a0a 466f  lting Bento...Fo
+000084f0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+00008500: 6f6e 2c20 7365 6520 5b52 6573 6f75 7263  on, see [Resourc
+00008510: 6520 7363 6865 6475 6c69 6e67 2073 7472  e scheduling str
+00008520: 6174 6567 795d 2868 7474 7073 3a2f 2f64  ategy](https://d
+00008530: 6f63 732e 6265 6e74 6f6d 6c2e 6f72 672f  ocs.bentoml.org/
+00008540: 656e 2f6c 6174 6573 742f 6775 6964 6573  en/latest/guides
+00008550: 2f73 6368 6564 756c 696e 672e 6874 6d6c  /scheduling.html
+00008560: 2329 2e0a 0a23 2320 f09f 9b9e 2052 756e  #)...## .... Run
+00008570: 7469 6d65 2069 6d70 6c65 6d65 6e74 6174  time implementat
+00008580: 696f 6e73 0a0a 4469 6666 6572 656e 7420  ions..Different 
+00008590: 4c4c 4d73 206d 6179 2073 7570 706f 7274  LLMs may support
+000085a0: 206d 756c 7469 706c 6520 7275 6e74 696d   multiple runtim
+000085b0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000085c0: 732e 204d 6f64 656c 7320 7468 6174 2068  s. Models that h
+000085d0: 6176 6520 6076 4c4c 4d60 2028 6076 6c6c  ave `vLLM` (`vll
+000085e0: 6d60 2920 7375 7070 6f72 7473 2077 696c  m`) supports wil
+000085f0: 6c20 7573 6520 764c 4c4d 2062 7920 6465  l use vLLM by de
+00008600: 6661 756c 742c 206f 7468 6572 7769 7365  fault, otherwise
+00008610: 2069 7420 6661 6c6c 6261 636b 2074 6f20   it fallback to 
+00008620: 7573 6520 6050 7954 6f72 6368 6020 2860  use `PyTorch` (`
+00008630: 7074 6029 2e0a 0a54 6f20 7370 6563 6966  pt`)...To specif
+00008640: 7920 6120 7370 6563 6966 6963 2072 756e  y a specific run
+00008650: 7469 6d65 2066 6f72 2079 6f75 7220 6368  time for your ch
+00008660: 6f73 656e 206d 6f64 656c 2c20 7573 6520  osen model, use 
+00008670: 7468 6520 602d 2d62 6163 6b65 6e64 6020  the `--backend` 
+00008680: 6f70 7469 6f6e 2e20 466f 7220 6578 616d  option. For exam
+00008690: 706c 653a 0a0a 6060 6062 6173 680a 6f70  ple:..```bash.op
+000086a0: 656e 6c6c 6d20 7374 6172 7420 6d65 7461  enllm start meta
+000086b0: 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32 2d37  -llama/Llama-2-7
+000086c0: 622d 6368 6174 2d68 6620 2d2d 6261 636b  b-chat-hf --back
+000086d0: 656e 6420 766c 6c6d 0a60 6060 0a0a 4e6f  end vllm.```..No
+000086e0: 7465 3a0a 0a31 2e20 546f 2075 7365 2074  te:..1. To use t
+000086f0: 6865 2076 4c4c 4d20 6261 636b 656e 642c  he vLLM backend,
+00008700: 2079 6f75 206e 6565 6420 6120 4750 5520   you need a GPU 
+00008710: 7769 7468 2061 7420 6c65 6173 7420 7468  with at least th
+00008720: 6520 416d 7065 7265 2061 7263 6869 7465  e Ampere archite
+00008730: 6374 7572 6520 6f72 206e 6577 6572 2061  cture or newer a
+00008740: 6e64 2043 5544 4120 7665 7273 696f 6e20  nd CUDA version 
+00008750: 3131 2e38 2e0a 322e 2054 6f20 7365 6520  11.8..2. To see 
+00008760: 7468 6520 6261 636b 656e 6420 6f70 7469  the backend opti
+00008770: 6f6e 7320 6f66 2065 6163 6820 6d6f 6465  ons of each mode
+00008780: 6c20 7375 7070 6f72 7465 6420 6279 204f  l supported by O
+00008790: 7065 6e4c 4c4d 2c20 7365 6520 7468 6520  penLLM, see the 
+000087a0: 5375 7070 6f72 7465 6420 6d6f 6465 6c73  Supported models
+000087b0: 2073 6563 7469 6f6e 206f 7220 7275 6e20   section or run 
+000087c0: 606f 7065 6e6c 6c6d 206d 6f64 656c 7360  `openllm models`
+000087d0: 2e0a 0a23 2320 f09f 9390 2051 7561 6e74  ...## .... Quant
+000087e0: 697a 6174 696f 6e0a 0a51 7561 6e74 697a  ization..Quantiz
+000087f0: 6174 696f 6e20 6973 2061 2074 6563 686e  ation is a techn
+00008800: 6971 7565 2074 6f20 7265 6475 6365 2074  ique to reduce t
+00008810: 6865 2073 746f 7261 6765 2061 6e64 2063  he storage and c
+00008820: 6f6d 7075 7461 7469 6f6e 2072 6571 7569  omputation requi
+00008830: 7265 6d65 6e74 7320 666f 7220 6d61 6368  rements for mach
+00008840: 696e 6520 6c65 6172 6e69 6e67 206d 6f64  ine learning mod
+00008850: 656c 732c 2070 6172 7469 6375 6c61 726c  els, particularl
+00008860: 7920 6475 7269 6e67 2069 6e66 6572 656e  y during inferen
+00008870: 6365 2e20 4279 2061 7070 726f 7869 6d61  ce. By approxima
+00008880: 7469 6e67 2066 6c6f 6174 696e 672d 706f  ting floating-po
+00008890: 696e 7420 6e75 6d62 6572 7320 6173 2069  int numbers as i
+000088a0: 6e74 6567 6572 7320 2871 7561 6e74 697a  ntegers (quantiz
+000088b0: 6564 2076 616c 7565 7329 2c20 7175 616e  ed values), quan
+000088c0: 7469 7a61 7469 6f6e 2061 6c6c 6f77 7320  tization allows 
+000088d0: 666f 7220 6661 7374 6572 2063 6f6d 7075  for faster compu
+000088e0: 7461 7469 6f6e 732c 2072 6564 7563 6564  tations, reduced
+000088f0: 206d 656d 6f72 7920 666f 6f74 7072 696e   memory footprin
+00008900: 742c 2061 6e64 2063 616e 206d 616b 6520  t, and can make 
+00008910: 6974 2066 6561 7369 626c 6520 746f 2064  it feasible to d
+00008920: 6570 6c6f 7920 6c61 7267 6520 6d6f 6465  eploy large mode
+00008930: 6c73 206f 6e20 7265 736f 7572 6365 2d63  ls on resource-c
+00008940: 6f6e 7374 7261 696e 6564 2064 6576 6963  onstrained devic
+00008950: 6573 2e0a 0a4f 7065 6e4c 4c4d 2073 7570  es...OpenLLM sup
+00008960: 706f 7274 7320 7468 6520 666f 6c6c 6f77  ports the follow
+00008970: 696e 6720 7175 616e 7469 7a61 7469 6f6e  ing quantization
+00008980: 2074 6563 686e 6971 7565 730a 0a2d 205b   techniques..- [
+00008990: 4c4c 4d2e 696e 7438 2829 3a20 382d 6269  LLM.int8(): 8-bi
+000089a0: 7420 4d61 7472 6978 204d 756c 7469 706c  t Matrix Multipl
+000089b0: 6963 6174 696f 6e5d 2868 7474 7073 3a2f  ication](https:/
+000089c0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+000089d0: 3230 382e 3037 3333 3929 2074 6872 6f75  208.07339) throu
+000089e0: 6768 205b 6269 7473 616e 6462 7974 6573  gh [bitsandbytes
+000089f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00008a00: 2e63 6f6d 2f54 696d 4465 7474 6d65 7273  .com/TimDettmers
+00008a10: 2f62 6974 7361 6e64 6279 7465 7329 0a2d  /bitsandbytes).-
+00008a20: 205b 5370 5152 3a20 4120 5370 6172 7365   [SpQR: A Sparse
+00008a30: 2d51 7561 6e74 697a 6564 2052 6570 7265  -Quantized Repre
+00008a40: 7365 6e74 6174 696f 6e20 666f 7220 4e65  sentation for Ne
+00008a50: 6172 2d4c 6f73 736c 6573 7320 4c4c 4d20  ar-Lossless LLM 
+00008a60: 5765 6967 6874 2043 6f6d 7072 6573 7369  Weight Compressi
+00008a70: 6f6e 0a20 205d 2868 7474 7073 3a2f 2f61  on.  ](https://a
+00008a80: 7278 6976 2e6f 7267 2f61 6273 2f32 3330  rxiv.org/abs/230
+00008a90: 362e 3033 3037 3829 2074 6872 6f75 6768  6.03078) through
+00008aa0: 205b 6269 7473 616e 6462 7974 6573 5d28   [bitsandbytes](
+00008ab0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00008ac0: 6f6d 2f54 696d 4465 7474 6d65 7273 2f62  om/TimDettmers/b
+00008ad0: 6974 7361 6e64 6279 7465 7329 0a2d 205b  itsandbytes).- [
+00008ae0: 4157 513a 2041 6374 6976 6174 696f 6e2d  AWQ: Activation-
+00008af0: 6177 6172 6520 5765 6967 6874 2051 7561  aware Weight Qua
+00008b00: 6e74 697a 6174 696f 6e5d 2868 7474 7073  ntization](https
+00008b10: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
+00008b20: 2f32 3330 362e 3030 3937 3829 2c0a 2d20  /2306.00978),.- 
+00008b30: 5b47 5054 513a 2041 6363 7572 6174 6520  [GPTQ: Accurate 
+00008b40: 506f 7374 2d54 7261 696e 696e 6720 5175  Post-Training Qu
+00008b50: 616e 7469 7a61 7469 6f6e 5d28 6874 7470  antization](http
+00008b60: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00008b70: 732f 3232 3130 2e31 3733 3233 290a 2d20  s/2210.17323).- 
+00008b80: 5b53 7175 6565 7a65 4c4c 4d3a 2044 656e  [SqueezeLLM: Den
+00008b90: 7365 2d61 6e64 2d53 7061 7273 6520 5175  se-and-Sparse Qu
+00008ba0: 616e 7469 7a61 7469 6f6e 5d28 6874 7470  antization](http
+00008bb0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00008bc0: 732f 3233 3036 2e30 3736 3239 292e 0a0a  s/2306.07629)...
+00008bd0: 2323 2320 5079 546f 7263 6820 6261 636b  ### PyTorch back
+00008be0: 656e 640a 0a57 6974 6820 5079 546f 7263  end..With PyTorc
+00008bf0: 6820 6261 636b 656e 642c 204f 7065 6e4c  h backend, OpenL
+00008c00: 4c4d 2073 7570 706f 7274 7320 6069 6e74  LM supports `int
+00008c10: 3860 2c20 6069 6e74 3460 2c20 616e 6420  8`, `int4`, and 
+00008c20: 6067 7074 7160 2e0a 0a46 6f72 2075 7369  `gptq`...For usi
+00008c30: 6e67 2069 6e74 3820 616e 6420 696e 7434  ng int8 and int4
+00008c40: 2071 7561 6e74 697a 6174 696f 6e20 7468   quantization th
+00008c50: 726f 7567 6820 6062 6974 7361 6e64 6279  rough `bitsandby
+00008c60: 7465 7360 2c20 796f 7520 6361 6e20 7573  tes`, you can us
+00008c70: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+00008c80: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
+00008c90: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
+00008ca0: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
+00008cb0: 2073 7461 7274 206d 6963 726f 736f 6674   start microsoft
+00008cc0: 2f70 6869 2d32 202d 2d71 7561 6e74 697a  /phi-2 --quantiz
+00008cd0: 6520 696e 7438 0a60 6060 0a0a 546f 2072  e int8.```..To r
+00008ce0: 756e 2069 6e66 6572 656e 6365 2077 6974  un inference wit
+00008cf0: 68c2 a060 6770 7471 602c 2073 696d 706c  h..`gptq`, simpl
+00008d00: 7920 7061 7373 c2a0 602d 2d71 7561 6e74  y pass..`--quant
+00008d10: 697a 6520 6770 7471 603a 0a0a 6060 6062  ize gptq`:..```b
+00008d20: 6173 680a 6f70 656e 6c6c 6d20 7374 6172  ash.openllm star
+00008d30: 7420 5468 6542 6c6f 6b65 2f4c 6c61 6d61  t TheBloke/Llama
+00008d40: 2d32 2d37 422d 4368 6174 2d47 5054 5120  -2-7B-Chat-GPTQ 
+00008d50: 2d2d 7175 616e 7469 7a65 2067 7074 710a  --quantize gptq.
+00008d60: 6060 600a 0a3e 205b 214e 4f54 455d 0a3e  ```..> [!NOTE].>
+00008d70: 2049 6e20 6f72 6465 7220 746f 2072 756e   In order to run
+00008d80: 2047 5054 512c 206d 616b 6520 7375 7265   GPTQ, make sure
+00008d90: 2079 6f75 2072 756e c2a0 6070 6970 2069   you run..`pip i
+00008da0: 6e73 7461 6c6c 2022 6f70 656e 6c6c 6d5b  nstall "openllm[
+00008db0: 6770 7471 5d22 600a 3e20 6669 7273 7420  gptq]"`.> first 
+00008dc0: 746f 2069 6e73 7461 6c6c 2074 6865 2064  to install the d
+00008dd0: 6570 656e 6465 6e63 792e 2046 726f 6d20  ependency. From 
+00008de0: 7468 6520 4750 5451 2070 6170 6572 2c20  the GPTQ paper, 
+00008df0: 6974 2069 7320 7265 636f 6d6d 656e 6465  it is recommende
+00008e00: 6420 746f 2071 7561 6e74 697a 6564 2074  d to quantized t
+00008e10: 6865 2077 6569 6768 7473 2062 6566 6f72  he weights befor
+00008e20: 6520 7365 7276 696e 672e 0a3e 2053 6565  e serving..> See
+00008e30: c2a0 5b41 7574 6f47 5054 515d 2868 7474  ..[AutoGPTQ](htt
+00008e40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008e50: 5061 6e51 6957 6569 2f41 7574 6f47 5054  PanQiWei/AutoGPT
+00008e60: 5129 c2a0 666f 7220 6d6f 7265 2069 6e66  Q)..for more inf
+00008e70: 6f72 6d61 7469 6f6e 206f 6e20 4750 5451  ormation on GPTQ
+00008e80: 2071 7561 6e74 697a 6174 696f 6e2e 0a0a   quantization...
+00008e90: 2323 2320 764c 4c4d 2062 6163 6b65 6e64  ### vLLM backend
+00008ea0: 0a0a 5769 7468 2076 4c4c 4d20 6261 636b  ..With vLLM back
+00008eb0: 656e 642c 204f 7065 6e4c 4c4d 2073 7570  end, OpenLLM sup
+00008ec0: 706f 7274 7320 6061 7771 602c 2060 7371  ports `awq`, `sq
+00008ed0: 7565 657a 656c 6c6d 600a 0a54 6f20 7275  ueezellm`..To ru
+00008ee0: 6e20 696e 6665 7265 6e63 6520 7769 7468  n inference with
+00008ef0: c2a0 6061 7771 602c 2073 696d 706c 7920  ..`awq`, simply 
+00008f00: 7061 7373 c2a0 602d 2d71 7561 6e74 697a  pass..`--quantiz
+00008f10: 6520 6177 7160 3a0a 0a60 6060 6261 7368  e awq`:..```bash
+00008f20: 0a6f 7065 6e6c 6c6d 2073 7461 7274 2054  .openllm start T
+00008f30: 6865 426c 6f6b 652f 7a65 7068 7972 2d37  heBloke/zephyr-7
+00008f40: 422d 616c 7068 612d 4157 5120 2d2d 7175  B-alpha-AWQ --qu
+00008f50: 616e 7469 7a65 2061 7771 0a60 6060 0a0a  antize awq.```..
+00008f60: 546f 2072 756e 2069 6e66 6572 656e 6365  To run inference
+00008f70: 2077 6974 6820 6073 7175 6565 7a65 6c6c   with `squeezell
+00008f80: 6d60 2c20 7369 6d70 6c79 2070 6173 7320  m`, simply pass 
+00008f90: 602d 2d71 7561 6e74 697a 6520 7371 7565  `--quantize sque
+00008fa0: 657a 656c 6c6d 603a 0a0a 6060 6062 6173  ezellm`:..```bas
+00008fb0: 680a 6f70 656e 6c6c 6d20 7374 6172 7420  h.openllm start 
+00008fc0: 7371 7565 657a 652d 6169 2d6c 6162 2f73  squeeze-ai-lab/s
+00008fd0: 712d 6c6c 616d 612d 322d 3762 2d77 342d  q-llama-2-7b-w4-
+00008fe0: 7330 202d 2d71 7561 6e74 697a 6520 7371  s0 --quantize sq
+00008ff0: 7565 657a 656c 6c6d 202d 2d73 6572 6961  ueezellm --seria
+00009000: 6c69 7a61 7469 6f6e 206c 6567 6163 790a  lization legacy.
+00009010: 6060 600a 0a3e 205b 2149 4d50 4f52 5441  ```..> [!IMPORTA
+00009020: 4e54 5d0a 3e20 5369 6e63 6520 626f 7468  NT].> Since both
+00009030: 2060 7371 7565 657a 656c 6c6d 6020 616e   `squeezellm` an
+00009040: 6420 6061 7771 6020 6172 6520 7765 6967  d `awq` are weig
+00009050: 6874 2d61 7761 7265 2071 7561 6e74 697a  ht-aware quantiz
+00009060: 6174 696f 6e20 6d65 7468 6f64 732c 206d  ation methods, m
+00009070: 6561 6e69 6e67 2074 6865 2071 7561 6e74  eaning the quant
+00009080: 697a 6174 696f 6e20 6973 2064 6f6e 6520  ization is done 
+00009090: 6475 7269 6e67 2074 7261 696e 696e 672c  during training,
+000090a0: 2061 6c6c 2070 7265 2d74 7261 696e 6564   all pre-trained
+000090b0: 2077 6569 6768 7473 206e 6565 6473 2074   weights needs t
+000090c0: 6f20 6765 7420 7175 616e 7469 7a65 6420  o get quantized 
+000090d0: 6265 666f 7265 2069 6e66 6572 656e 6365  before inference
+000090e0: 2074 696d 652e 204d 616b 6520 7375 7265   time. Make sure
+000090f0: 2074 6f20 6669 6e64 2063 6f6d 7061 7469   to find compati
+00009100: 626c 6520 7765 6967 6874 7320 6f6e 2048  ble weights on H
+00009110: 7567 6769 6e67 4661 6365 2048 7562 2066  uggingFace Hub f
+00009120: 6f72 2079 6f75 7220 6d6f 6465 6c20 6f66  or your model of
+00009130: 2063 686f 6963 652e 0a0a 2323 20f0 9f9b   choice...## ...
+00009140: a0ef b88f 2053 6572 7669 6e67 2066 696e  .... Serving fin
+00009150: 652d 7475 6e69 6e67 206c 6179 6572 730a  e-tuning layers.
+00009160: 0a5b 5045 4654 5d28 6874 7470 733a 2f2f  .[PEFT](https://
+00009170: 6875 6767 696e 6766 6163 652e 636f 2f64  huggingface.co/d
+00009180: 6f63 732f 7065 6674 2f69 6e64 6578 292c  ocs/peft/index),
+00009190: 206f 7220 5061 7261 6d65 7465 722d 4566   or Parameter-Ef
+000091a0: 6669 6369 656e 7420 4669 6e65 2d54 756e  ficient Fine-Tun
+000091b0: 696e 672c 2069 7320 6120 6d65 7468 6f64  ing, is a method
+000091c0: 6f6c 6f67 7920 6465 7369 676e 6564 2074  ology designed t
+000091d0: 6f20 6669 6e65 2d74 756e 6520 7072 652d  o fine-tune pre-
+000091e0: 7472 6169 6e65 6420 6d6f 6465 6c73 206d  trained models m
+000091f0: 6f72 6520 6566 6669 6369 656e 746c 792e  ore efficiently.
+00009200: 2049 6e73 7465 6164 206f 6620 6164 6a75   Instead of adju
+00009210: 7374 696e 6720 616c 6c20 6d6f 6465 6c20  sting all model 
+00009220: 7061 7261 6d65 7465 7273 2c20 5045 4654  parameters, PEFT
+00009230: 2066 6f63 7573 6573 206f 6e20 7475 6e69   focuses on tuni
+00009240: 6e67 206f 6e6c 7920 6120 7375 6273 6574  ng only a subset
+00009250: 2c20 7265 6475 6369 6e67 2063 6f6d 7075  , reducing compu
+00009260: 7461 7469 6f6e 616c 2061 6e64 2073 746f  tational and sto
+00009270: 7261 6765 2063 6f73 7473 2e20 5b4c 6f52  rage costs. [LoR
+00009280: 415d 2868 7474 7073 3a2f 2f68 7567 6769  A](https://huggi
+00009290: 6e67 6661 6365 2e63 6f2f 646f 6373 2f70  ngface.co/docs/p
+000092a0: 6566 742f 636f 6e63 6570 7475 616c 5f67  eft/conceptual_g
+000092b0: 7569 6465 732f 6c6f 7261 2920 284c 6f77  uides/lora) (Low
+000092c0: 2d52 616e 6b20 4164 6170 7461 7469 6f6e  -Rank Adaptation
+000092d0: 2920 6973 206f 6e65 206f 6620 7468 6520  ) is one of the 
+000092e0: 7465 6368 6e69 7175 6573 2073 7570 706f  techniques suppo
+000092f0: 7274 6564 2062 7920 5045 4654 2e20 4974  rted by PEFT. It
+00009300: 2073 7472 6561 6d6c 696e 6573 2066 696e   streamlines fin
+00009310: 652d 7475 6e69 6e67 2062 7920 7573 696e  e-tuning by usin
+00009320: 6720 6c6f 772d 7261 6e6b 2064 6563 6f6d  g low-rank decom
+00009330: 706f 7369 7469 6f6e 2074 6f20 7265 7072  position to repr
+00009340: 6573 656e 7420 7765 6967 6874 2075 7064  esent weight upd
+00009350: 6174 6573 2c20 7468 6572 6562 7920 6472  ates, thereby dr
+00009360: 6173 7469 6361 6c6c 7920 7265 6475 6369  astically reduci
+00009370: 6e67 2074 6865 206e 756d 6265 7220 6f66  ng the number of
+00009380: 2074 7261 696e 6162 6c65 2070 6172 616d   trainable param
+00009390: 6574 6572 732e 0a0a 5769 7468 204f 7065  eters...With Ope
+000093a0: 6e4c 4c4d 2c20 796f 7520 6361 6e20 7461  nLLM, you can ta
+000093b0: 6b65 2061 6476 616e 7461 6765 206f 6620  ke advantage of 
+000093c0: 7468 6520 6669 6e65 2d74 756e 696e 6720  the fine-tuning 
+000093d0: 6665 6174 7572 6520 6279 2073 6572 7669  feature by servi
+000093e0: 6e67 206d 6f64 656c 7320 7769 7468 2061  ng models with a
+000093f0: 6e79 2050 4546 542d 636f 6d70 6174 6962  ny PEFT-compatib
+00009400: 6c65 206c 6179 6572 7320 7573 696e 6720  le layers using 
+00009410: 7468 6520 602d 2d61 6461 7074 6572 2d69  the `--adapter-i
+00009420: 6460 206f 7074 696f 6e2e 2046 6f72 2065  d` option. For e
+00009430: 7861 6d70 6c65 3a0a 0a60 6060 6261 7368  xample:..```bash
+00009440: 0a6f 7065 6e6c 6c6d 2073 7461 7274 2066  .openllm start f
+00009450: 6163 6562 6f6f 6b2f 6f70 742d 362e 3762  acebook/opt-6.7b
+00009460: 202d 2d61 6461 7074 6572 2d69 6420 6161   --adapter-id aa
+00009470: 726e 7068 6d2f 6f70 742d 362d 3762 2d71  rnphm/opt-6-7b-q
+00009480: 756f 7465 733a 6465 6661 756c 740a 6060  uotes:default.``
+00009490: 600a 0a4f 7065 6e4c 4c4d 2061 6c73 6f20  `..OpenLLM also 
+000094a0: 7072 6f76 6964 6573 2066 6c65 7869 6269  provides flexibi
+000094b0: 6c69 7479 2062 7920 7375 7070 6f72 7469  lity by supporti
+000094c0: 6e67 2061 6461 7074 6572 7320 6672 6f6d  ng adapters from
+000094d0: 2063 7573 746f 6d20 6669 6c65 2070 6174   custom file pat
+000094e0: 6873 3a0a 0a60 6060 6261 7368 0a6f 7065  hs:..```bash.ope
+000094f0: 6e6c 6c6d 2073 7461 7274 2066 6163 6562  nllm start faceb
+00009500: 6f6f 6b2f 6f70 742d 362e 3762 202d 2d61  ook/opt-6.7b --a
+00009510: 6461 7074 6572 2d69 6420 2f70 6174 682f  dapter-id /path/
+00009520: 746f 2f61 6461 7074 6572 733a 6c6f 6361  to/adapters:loca
+00009530: 6c5f 6164 6170 7465 720a 6060 600a 0a54  l_adapter.```..T
+00009540: 6f20 7573 6520 6d75 6c74 6970 6c65 2061  o use multiple a
+00009550: 6461 7074 6572 732c 2075 7365 2074 6865  dapters, use the
+00009560: 2066 6f6c 6c6f 7769 6e67 2066 6f72 6d61   following forma
+00009570: 743a 0a0a 6060 6062 6173 680a 6f70 656e  t:..```bash.open
+00009580: 6c6c 6d20 7374 6172 7420 6661 6365 626f  llm start facebo
+00009590: 6f6b 2f6f 7074 2d36 2e37 6220 2d2d 6164  ok/opt-6.7b --ad
+000095a0: 6170 7465 722d 6964 2061 6172 6e70 686d  apter-id aarnphm
+000095b0: 2f6f 7074 2d36 2e37 622d 6c6f 7261 3a64  /opt-6.7b-lora:d
+000095c0: 6566 6175 6c74 202d 2d61 6461 7074 6572  efault --adapter
+000095d0: 2d69 6420 6161 726e 7068 6d2f 6f70 742d  -id aarnphm/opt-
+000095e0: 362e 3762 2d66 7265 6e63 683a 6672 656e  6.7b-french:fren
+000095f0: 6368 5f6c 6f72 610a 6060 600a 0a42 7920  ch_lora.```..By 
+00009600: 6465 6661 756c 742c 2061 6c6c 2061 6461  default, all ada
+00009610: 7074 6572 7320 7769 6c6c 2062 6520 696e  pters will be in
+00009620: 6a65 6374 6564 2069 6e74 6f20 7468 6520  jected into the 
+00009630: 6d6f 6465 6c73 2064 7572 696e 6720 7374  models during st
+00009640: 6172 7475 702e 2041 6461 7074 6572 7320  artup. Adapters 
+00009650: 6361 6e20 6265 2073 7065 6369 6669 6564  can be specified
+00009660: 2070 6572 2072 6571 7565 7374 2076 6961   per request via
+00009670: 2060 6164 6170 7465 725f 6e61 6d65 603a   `adapter_name`:
+00009680: 0a0a 6060 6062 6173 680a 6375 726c 202d  ..```bash.curl -
+00009690: 5820 2750 4f53 5427 205c 0a20 2027 6874  X 'POST' \.  'ht
+000096a0: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
+000096b0: 3030 302f 7631 2f67 656e 6572 6174 6527  000/v1/generate'
+000096c0: 205c 0a20 202d 4820 2761 6363 6570 743a   \.  -H 'accept:
+000096d0: 2061 7070 6c69 6361 7469 6f6e 2f6a 736f   application/jso
+000096e0: 6e27 205c 0a20 202d 4820 2743 6f6e 7465  n' \.  -H 'Conte
+000096f0: 6e74 2d54 7970 653a 2061 7070 6c69 6361  nt-Type: applica
+00009700: 7469 6f6e 2f6a 736f 6e27 205c 0a20 202d  tion/json' \.  -
+00009710: 6420 277b 0a20 2022 7072 6f6d 7074 223a  d '{.  "prompt":
+00009720: 2022 5768 6174 2069 7320 7468 6520 6d65   "What is the me
+00009730: 616e 696e 6720 6f66 206c 6966 653f 222c  aning of life?",
+00009740: 0a20 2022 7374 6f70 223a 205b 0a20 2020  .  "stop": [.   
+00009750: 2022 7068 696c 6f73 6f70 6865 7222 0a20   "philosopher". 
+00009760: 205d 2c0a 2020 226c 6c6d 5f63 6f6e 6669   ],.  "llm_confi
+00009770: 6722 3a20 7b0a 2020 2020 226d 6178 5f6e  g": {.    "max_n
+00009780: 6577 5f74 6f6b 656e 7322 3a20 3235 362c  ew_tokens": 256,
+00009790: 0a20 2020 2022 7465 6d70 6572 6174 7572  .    "temperatur
+000097a0: 6522 3a20 302e 3735 2c0a 2020 2020 2274  e": 0.75,.    "t
+000097b0: 6f70 5f6b 223a 2031 352c 0a20 2020 2022  op_k": 15,.    "
+000097c0: 746f 705f 7022 3a20 310a 2020 7d2c 0a20  top_p": 1.  },. 
+000097d0: 2022 6164 6170 7465 725f 6e61 6d65 223a   "adapter_name":
+000097e0: 2022 6465 6661 756c 7422 0a7d 270a 6060   "default".}'.``
+000097f0: 600a 0a54 6f20 696e 636c 7564 6520 7468  `..To include th
+00009800: 6973 2069 6e74 6f20 7468 6520 4265 6e74  is into the Bent
+00009810: 6f2c 2079 6f75 2063 616e 2073 7065 6369  o, you can speci
+00009820: 6679 2074 6865 c2a0 602d 2d61 6461 7074  fy the..`--adapt
+00009830: 6572 2d69 6460 c2a0 6f70 7469 6f6e 2077  er-id`..option w
+00009840: 6865 6e20 7573 696e 6720 7468 65c2 a060  hen using the..`
+00009850: 6f70 656e 6c6c 6d20 6275 696c 6460 2063  openllm build` c
+00009860: 6f6d 6d61 6e64 3a0a 0a60 6060 6261 7368  ommand:..```bash
+00009870: 0a6f 7065 6e6c 6c6d 2062 7569 6c64 2066  .openllm build f
+00009880: 6163 6562 6f6f 6b2f 6f70 742d 362e 3762  acebook/opt-6.7b
+00009890: 202d 2d61 6461 7074 6572 2d69 6420 2e2e   --adapter-id ..
+000098a0: 2e0a 6060 600a 0a49 6620 796f 7520 7573  ..```..If you us
+000098b0: 6520 6120 7265 6c61 7469 7665 2070 6174  e a relative pat
+000098c0: 6820 666f 7220 602d 2d61 6461 7074 6572  h for `--adapter
+000098d0: 2d69 6460 2c20 796f 7520 6e65 6564 2074  -id`, you need t
+000098e0: 6f20 6164 6420 602d 2d62 7569 6c64 2d63  o add `--build-c
+000098f0: 7478 602e 0a0a 6060 6062 6173 680a 6f70  tx`...```bash.op
+00009900: 656e 6c6c 6d20 6275 696c 6420 6661 6365  enllm build face
+00009910: 626f 6f6b 2f6f 7074 2d36 2e37 6220 2d2d  book/opt-6.7b --
+00009920: 6164 6170 7465 722d 6964 202e 2f70 6174  adapter-id ./pat
+00009930: 682f 746f 2f61 6461 7074 6572 5f69 6420  h/to/adapter_id 
+00009940: 2d2d 6275 696c 642d 6374 7820 2e0a 6060  --build-ctx ..``
+00009950: 600a 0a3e 205b 2149 4d50 4f52 5441 4e54  `..> [!IMPORTANT
+00009960: 5d0a 3e20 4669 6e65 2d74 756e 696e 6720  ].> Fine-tuning 
+00009970: 7375 7070 6f72 7420 6973 2073 7469 6c6c  support is still
+00009980: 2065 7870 6572 696d 656e 7461 6c20 616e   experimental an
+00009990: 6420 6375 7272 656e 746c 7920 6f6e 6c79  d currently only
+000099a0: 2077 6f72 6b73 2077 6974 6820 5079 546f   works with PyTo
+000099b0: 7263 6820 6261 636b 656e 642e 2076 4c4c  rch backend. vLL
+000099c0: 4d20 7375 7070 6f72 7420 6973 2063 6f6d  M support is com
+000099d0: 696e 6720 736f 6f6e 2e0a 0a0a 2323 20e2  ing soon....## .
+000099e0: 9a99 efb8 8f20 496e 7465 6772 6174 696f  ..... Integratio
+000099f0: 6e73 0a0a 4f70 656e 4c4c 4d20 6973 206e  ns..OpenLLM is n
+00009a00: 6f74 206a 7573 7420 6120 7374 616e 6461  ot just a standa
+00009a10: 6c6f 6e65 2070 726f 6475 6374 3b20 6974  lone product; it
+00009a20: 2773 2061 2062 7569 6c64 696e 6720 626c  's a building bl
+00009a30: 6f63 6b20 6465 7369 676e 6564 2074 6f0a  ock designed to.
+00009a40: 696e 7465 6772 6174 6520 7769 7468 206f  integrate with o
+00009a50: 7468 6572 2070 6f77 6572 6675 6c20 746f  ther powerful to
+00009a60: 6f6c 7320 6561 7369 6c79 2e20 5765 2063  ols easily. We c
+00009a70: 7572 7265 6e74 6c79 206f 6666 6572 2069  urrently offer i
+00009a80: 6e74 6567 7261 7469 6f6e 2077 6974 680a  ntegration with.
+00009a90: 5b4f 7065 6e41 4927 7320 436f 6d70 6174  [OpenAI's Compat
+00009aa0: 6962 6c65 2045 6e64 706f 696e 7473 5d28  ible Endpoints](
+00009ab0: 6874 7470 733a 2f2f 706c 6174 666f 726d  https://platform
+00009ac0: 2e6f 7065 6e61 692e 636f 6d2f 646f 6373  .openai.com/docs
+00009ad0: 2f61 7069 2d72 6566 6572 656e 6365 2f63  /api-reference/c
+00009ae0: 6f6d 706c 6574 696f 6e73 2f6f 626a 6563  ompletions/objec
+00009af0: 7429 2c0a 5b4c 6c61 6d61 496e 6465 785d  t),.[LlamaIndex]
+00009b00: 2868 7474 7073 3a2f 2f77 7777 2e6c 6c61  (https://www.lla
+00009b10: 6d61 696e 6465 782e 6169 2f29 2c0a 5b4c  maindex.ai/),.[L
+00009b20: 616e 6743 6861 696e 5d28 6874 7470 733a  angChain](https:
+00009b30: 2f2f 6769 7468 7562 2e63 6f6d 2f68 7763  //github.com/hwc
+00009b40: 6861 7365 3137 2f6c 616e 6763 6861 696e  hase17/langchain
+00009b50: 292c 2061 6e64 0a5b 5472 616e 7366 6f72  ), and.[Transfor
+00009b60: 6d65 7273 2041 6765 6e74 735d 2868 7474  mers Agents](htt
+00009b70: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00009b80: 2e63 6f2f 646f 6373 2f74 7261 6e73 666f  .co/docs/transfo
+00009b90: 726d 6572 732f 7472 616e 7366 6f72 6d65  rmers/transforme
+00009ba0: 7273 5f61 6765 6e74 7329 2e0a 0a23 2323  rs_agents)...###
+00009bb0: 204f 7065 6e41 4920 436f 6d70 6174 6962   OpenAI Compatib
+00009bc0: 6c65 2045 6e64 706f 696e 7473 0a0a 4f70  le Endpoints..Op
+00009bd0: 656e 4c4c 4d20 5365 7276 6572 2063 616e  enLLM Server can
+00009be0: 2062 6520 7573 6564 2061 7320 6120 6472   be used as a dr
+00009bf0: 6f70 2d69 6e20 7265 706c 6163 656d 656e  op-in replacemen
+00009c00: 7420 666f 7220 4f70 656e 4149 2773 2041  t for OpenAI's A
+00009c10: 5049 2e20 5369 6d70 6c79 0a73 7065 6369  PI. Simply.speci
+00009c20: 6679 2074 6865 2062 6173 655f 7572 6c20  fy the base_url 
+00009c30: 746f 2060 6c6c 6d2d 656e 6470 6f69 6e74  to `llm-endpoint
+00009c40: 2f76 3160 2061 6e64 2079 6f75 2061 7265  /v1` and you are
+00009c50: 2067 6f6f 6420 746f 2067 6f3a 0a0a 6060   good to go:..``
+00009c60: 6070 7974 686f 6e0a 696d 706f 7274 206f  `python.import o
+00009c70: 7065 6e61 690a 0a63 6c69 656e 7420 3d20  penai..client = 
+00009c80: 6f70 656e 6169 2e4f 7065 6e41 4928 0a20  openai.OpenAI(. 
+00009c90: 2062 6173 655f 7572 6c3d 2768 7474 703a   base_url='http:
+00009ca0: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
+00009cb0: 2f76 3127 2c20 6170 695f 6b65 793d 276e  /v1', api_key='n
+00009cc0: 6127 0a29 2020 2320 4865 7265 2074 6865  a'.)  # Here the
+00009cd0: 2073 6572 7665 7220 6973 2072 756e 6e69   server is runni
+00009ce0: 6e67 206f 6e20 6c6f 6361 6c68 6f73 743a  ng on localhost:
+00009cf0: 3330 3030 0a0a 636f 6d70 6c65 7469 6f6e  3000..completion
+00009d00: 7320 3d20 636c 6965 6e74 2e63 6f6d 706c  s = client.compl
+00009d10: 6574 696f 6e73 2e63 7265 6174 6528 0a20  etions.create(. 
+00009d20: 2070 726f 6d70 743d 2757 7269 7465 206d   prompt='Write m
+00009d30: 6520 6120 7461 6720 6c69 6e65 2066 6f72  e a tag line for
+00009d40: 2061 6e20 6963 6520 6372 6561 6d20 7368   an ice cream sh
+00009d50: 6f70 2e27 2c20 6d6f 6465 6c3d 6d6f 6465  op.', model=mode
+00009d60: 6c2c 206d 6178 5f74 6f6b 656e 733d 3634  l, max_tokens=64
+00009d70: 2c20 7374 7265 616d 3d73 7472 6561 6d0a  , stream=stream.
+00009d80: 290a 6060 600a 0a54 6865 2063 6f6d 7061  ).```..The compa
+00009d90: 7469 626c 6520 656e 6470 6f69 6e74 7320  tible endpoints 
+00009da0: 7375 7070 6f72 7473 2060 2f63 6f6d 706c  supports `/compl
+00009db0: 6574 696f 6e73 602c 2060 2f63 6861 742f  etions`, `/chat/
+00009dc0: 636f 6d70 6c65 7469 6f6e 7360 2c20 616e  completions`, an
+00009dd0: 6420 602f 6d6f 6465 6c73 600a 0a3e 205b  d `/models`..> [
+00009de0: 214e 4f54 455d 0a3e 2059 6f75 2063 616e  !NOTE].> You can
+00009df0: 2066 696e 6420 6f75 7420 4f70 656e 4149   find out OpenAI
+00009e00: 2065 7861 6d70 6c65 2063 6c69 656e 7473   example clients
+00009e10: 2075 6e64 6572 2074 6865 0a3e 205b 6578   under the.> [ex
+00009e20: 616d 706c 6573 5d28 6874 7470 733a 2f2f  amples](https://
+00009e30: 6769 7468 7562 2e63 6f6d 2f62 656e 746f  github.com/bento
+00009e40: 6d6c 2f4f 7065 6e4c 4c4d 2f74 7265 652f  ml/OpenLLM/tree/
+00009e50: 6d61 696e 2f65 7861 6d70 6c65 7329 2066  main/examples) f
+00009e60: 6f6c 6465 722e 0a0a 0a23 2323 205b 4c6c  older....### [Ll
+00009e70: 616d 6149 6e64 6578 5d28 6874 7470 733a  amaIndex](https:
+00009e80: 2f2f 646f 6373 2e6c 6c61 6d61 696e 6465  //docs.llamainde
+00009e90: 782e 6169 2f65 6e2f 7374 6162 6c65 2f65  x.ai/en/stable/e
+00009ea0: 7861 6d70 6c65 732f 6c6c 6d2f 6f70 656e  xamples/llm/open
+00009eb0: 6c6c 6d2f 290a 0a54 6f20 7374 6172 7420  llm/)..To start 
+00009ec0: 6120 6c6f 6361 6c20 4c4c 4d20 7769 7468  a local LLM with
+00009ed0: 2060 6c6c 616d 615f 696e 6465 7860 2c20   `llama_index`, 
+00009ee0: 7369 6d70 6c79 2075 7365 2060 6c6c 616d  simply use `llam
+00009ef0: 615f 696e 6465 782e 6c6c 6d73 2e6f 7065  a_index.llms.ope
+00009f00: 6e6c 6c6d 2e4f 7065 6e4c 4c4d 603a 0a0a  nllm.OpenLLM`:..
+00009f10: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00009f20: 2061 7379 6e63 696f 0a66 726f 6d20 6c6c   asyncio.from ll
+00009f30: 616d 615f 696e 6465 782e 6c6c 6d73 2e6f  ama_index.llms.o
+00009f40: 7065 6e6c 6c6d 2069 6d70 6f72 7420 4f70  penllm import Op
+00009f50: 656e 4c4c 4d0a 0a6c 6c6d 203d 204f 7065  enLLM..llm = Ope
+00009f60: 6e4c 4c4d 2827 4875 6767 696e 6746 6163  nLLM('HuggingFac
+00009f70: 6548 342f 7a65 7068 7972 2d37 622d 616c  eH4/zephyr-7b-al
+00009f80: 7068 6127 290a 0a6c 6c6d 2e63 6f6d 706c  pha')..llm.compl
+00009f90: 6574 6528 2754 6865 206d 6561 6e69 6e67  ete('The meaning
+00009fa0: 206f 6620 6c69 6665 2069 7327 290a 0a0a   of life is')...
+00009fb0: 6173 796e 6320 6465 6620 6d61 696e 2870  async def main(p
+00009fc0: 726f 6d70 742c 202a 2a6b 7761 7267 7329  rompt, **kwargs)
+00009fd0: 3a0a 2020 6173 796e 6320 666f 7220 6974  :.  async for it
+00009fe0: 2069 6e20 6c6c 6d2e 6173 7472 6561 6d5f   in llm.astream_
+00009ff0: 6368 6174 2870 726f 6d70 742c 202a 2a6b  chat(prompt, **k
+0000a000: 7761 7267 7329 3a0a 2020 2020 7072 696e  wargs):.    prin
+0000a010: 7428 6974 290a 0a0a 6173 796e 6369 6f2e  t(it)...asyncio.
+0000a020: 7275 6e28 6d61 696e 2827 5468 6520 7469  run(main('The ti
+0000a030: 6d65 2061 7420 5361 6e20 4672 616e 6369  me at San Franci
+0000a040: 7363 6f20 6973 2729 290a 6060 600a 0a49  sco is')).```..I
+0000a050: 6620 7468 6572 6520 6973 2061 2072 656d  f there is a rem
+0000a060: 6f74 6520 4c4c 4d20 5365 7276 6572 2072  ote LLM Server r
+0000a070: 756e 6e69 6e67 2065 6c73 6577 6865 7265  unning elsewhere
+0000a080: 2c20 7468 656e 2079 6f75 2063 616e 2075  , then you can u
+0000a090: 7365 2060 6c6c 616d 615f 696e 6465 782e  se `llama_index.
+0000a0a0: 6c6c 6d73 2e6f 7065 6e6c 6c6d 2e4f 7065  llms.openllm.Ope
+0000a0b0: 6e4c 4c4d 4150 4960 3a0a 0a60 6060 7079  nLLMAPI`:..```py
+0000a0c0: 7468 6f6e 0a66 726f 6d20 6c6c 616d 615f  thon.from llama_
+0000a0d0: 696e 6465 782e 6c6c 6d73 2e6f 7065 6e6c  index.llms.openl
+0000a0e0: 6c6d 2069 6d70 6f72 7420 4f70 656e 4c4c  lm import OpenLL
+0000a0f0: 4d41 5049 0a60 6060 0a0a 3e20 5b21 4e4f  MAPI.```..> [!NO
+0000a100: 5445 5d0a 3e20 416c 6c20 7379 6e63 6872  TE].> All synchr
+0000a110: 6f6e 6f75 7320 616e 6420 6173 796e 6368  onous and asynch
+0000a120: 726f 6e6f 7573 2041 5049 2066 726f 6d20  ronous API from 
+0000a130: 606c 6c61 6d61 5f69 6e64 6578 2e6c 6c6d  `llama_index.llm
+0000a140: 732e 4c4c 4d60 2061 7265 2073 7570 706f  s.LLM` are suppo
+0000a150: 7274 6564 2e0a 0a23 2323 205b 4c61 6e67  rted...### [Lang
+0000a160: 4368 6169 6e5d 2868 7474 7073 3a2f 2f70  Chain](https://p
+0000a170: 7974 686f 6e2e 6c61 6e67 6368 6169 6e2e  ython.langchain.
+0000a180: 636f 6d2f 646f 6373 2f69 6e74 6567 7261  com/docs/integra
+0000a190: 7469 6f6e 732f 6c6c 6d73 2f6f 7065 6e6c  tions/llms/openl
+0000a1a0: 6c6d 2f29 0a0a 5370 696e 2075 7020 616e  lm/)..Spin up an
+0000a1b0: 204f 7065 6e4c 4c4d 2073 6572 7665 722c   OpenLLM server,
+0000a1c0: 2061 6e64 2063 6f6e 6e65 6374 2074 6f20   and connect to 
+0000a1d0: 6974 2062 7920 7370 6563 6966 7969 6e67  it by specifying
+0000a1e0: 2069 7473 2055 524c 3a0a 0a60 6060 7079   its URL:..```py
+0000a1f0: 7468 6f6e 0a66 726f 6d20 6c61 6e67 6368  thon.from langch
+0000a200: 6169 6e2e 6c6c 6d73 2069 6d70 6f72 7420  ain.llms import 
+0000a210: 4f70 656e 4c4c 4d0a 0a6c 6c6d 203d 204f  OpenLLM..llm = O
+0000a220: 7065 6e4c 4c4d 2873 6572 7665 725f 7572  penLLM(server_ur
+0000a230: 6c3d 2768 7474 703a 2f2f 3434 2e32 332e  l='http://44.23.
+0000a240: 3132 332e 313a 3330 3030 272c 2073 6572  123.1:3000', ser
+0000a250: 7665 725f 7479 7065 3d27 6874 7470 2729  ver_type='http')
+0000a260: 0a6c 6c6d 2827 5768 6174 2069 7320 7468  .llm('What is th
+0000a270: 6520 6469 6666 6572 656e 6365 2062 6574  e difference bet
+0000a280: 7765 656e 2061 2064 7563 6b20 616e 6420  ween a duck and 
+0000a290: 6120 676f 6f73 653f 2041 6e64 2077 6879  a goose? And why
+0000a2a0: 2074 6865 7265 2061 7265 2073 6f20 6d61   there are so ma
+0000a2b0: 6e79 2047 6f6f 7365 2069 6e20 4361 6e61  ny Goose in Cana
+0000a2c0: 6461 3f27 290a 6060 600a 0a23 2323 2054  da?').```..### T
+0000a2d0: 7261 6e73 666f 726d 6572 7320 4167 656e  ransformers Agen
+0000a2e0: 7473 0a0a 4f70 656e 4c4c 4d20 7365 616d  ts..OpenLLM seam
+0000a2f0: 6c65 7373 6c79 2069 6e74 6567 7261 7465  lessly integrate
+0000a300: 7320 7769 7468 0a5b 5472 616e 7366 6f72  s with.[Transfor
+0000a310: 6d65 7273 2041 6765 6e74 735d 2868 7474  mers Agents](htt
+0000a320: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+0000a330: 2e63 6f2f 646f 6373 2f74 7261 6e73 666f  .co/docs/transfo
+0000a340: 726d 6572 732f 7472 616e 7366 6f72 6d65  rmers/transforme
+0000a350: 7273 5f61 6765 6e74 7329 2e0a 0a3e 205b  rs_agents)...> [
+0000a360: 2157 4152 4e49 4e47 5d0a 3e20 5468 6520  !WARNING].> The 
+0000a370: 5472 616e 7366 6f72 6d65 7273 2041 6765  Transformers Age
+0000a380: 6e74 2069 7320 7374 696c 6c20 6174 2061  nt is still at a
+0000a390: 6e20 6578 7065 7269 6d65 6e74 616c 2073  n experimental s
+0000a3a0: 7461 6765 2e20 4974 2069 730a 3e20 7265  tage. It is.> re
+0000a3b0: 636f 6d6d 656e 6465 6420 746f 2069 6e73  commended to ins
+0000a3c0: 7461 6c6c 204f 7065 6e4c 4c4d 2077 6974  tall OpenLLM wit
+0000a3d0: 6820 6070 6970 2069 6e73 7461 6c6c 202d  h `pip install -
+0000a3e0: 7220 6e69 6768 746c 792d 7265 7175 6972  r nightly-requir
+0000a3f0: 656d 656e 7473 2e74 7874 600a 3e20 746f  ements.txt`.> to
+0000a400: 2067 6574 2074 6865 206c 6174 6573 7420   get the latest 
+0000a410: 4150 4920 7570 6461 7465 2066 6f72 2048  API update for H
+0000a420: 7567 6769 6e67 4661 6365 2061 6765 6e74  uggingFace agent
+0000a430: 2e0a 0a60 6060 7079 7468 6f6e 0a69 6d70  ...```python.imp
+0000a440: 6f72 7420 7472 616e 7366 6f72 6d65 7273  ort transformers
+0000a450: 0a0a 6167 656e 7420 3d20 7472 616e 7366  ..agent = transf
+0000a460: 6f72 6d65 7273 2e48 6641 6765 6e74 2827  ormers.HfAgent('
+0000a470: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+0000a480: 3a33 3030 302f 6866 2f61 6765 6e74 2729  :3000/hf/agent')
+0000a490: 2020 2320 5552 4c20 7468 6174 2072 756e    # URL that run
+0000a4a0: 7320 7468 6520 4f70 656e 4c4c 4d20 7365  s the OpenLLM se
+0000a4b0: 7276 6572 0a0a 6167 656e 742e 7275 6e28  rver..agent.run(
+0000a4c0: 2749 7320 7468 6520 666f 6c6c 6f77 696e  'Is the followin
+0000a4d0: 6720 6074 6578 7460 2070 6f73 6974 6976  g `text` positiv
+0000a4e0: 6520 6f72 206e 6567 6174 6976 653f 272c  e or negative?',
+0000a4f0: 2074 6578 743d 2249 2064 6f6e 2774 206c   text="I don't l
+0000a500: 696b 6520 686f 7720 7468 6973 206d 6f64  ike how this mod
+0000a510: 656c 7320 6973 2067 656e 6572 6174 6520  els is generate 
+0000a520: 696e 7075 7473 2229 0a60 6060 0a0a 3c70  inputs").```..<p
+0000a530: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
+0000a540: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
+0000a550: 7073 3a2f 2f72 6177 2e67 6974 6875 6275  ps://raw.githubu
+0000a560: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f62  sercontent.com/b
+0000a570: 656e 746f 6d6c 2f6f 7065 6e6c 6c6d 2f6d  entoml/openllm/m
+0000a580: 6169 6e2f 2e67 6974 6875 622f 6173 7365  ain/.github/asse
+0000a590: 7473 2f61 6765 6e74 2e67 6966 2220 616c  ts/agent.gif" al
+0000a5a0: 743d 2247 6966 2073 686f 7769 6e67 2041  t="Gif showing A
+0000a5b0: 6765 6e74 2069 6e74 6567 7261 7469 6f6e  gent integration
+0000a5c0: 2220 2f3e 0a3c 2f70 3e0a 0a23 2320 f09f  " />.</p>..## ..
+0000a5d0: 9a80 2044 6570 6c6f 7969 6e67 206d 6f64  .. Deploying mod
+0000a5e0: 656c 7320 746f 2070 726f 6475 6374 696f  els to productio
+0000a5f0: 6e0a 0a54 6865 7265 2061 7265 2073 6576  n..There are sev
+0000a600: 6572 616c 2077 6179 7320 746f 2064 6570  eral ways to dep
+0000a610: 6c6f 7920 796f 7572 204c 4c4d 733a 0a0a  loy your LLMs:..
+0000a620: 2323 2320 f09f 90b3 2044 6f63 6b65 7220  ### .... Docker 
+0000a630: 636f 6e74 6169 6e65 720a 0a31 2e20 2a2a  container..1. **
+0000a640: 4275 696c 6469 6e67 2061 2042 656e 746f  Building a Bento
+0000a650: 2a2a 3a20 5769 7468 204f 7065 6e4c 4c4d  **: With OpenLLM
+0000a660: 2c20 796f 7520 6361 6e20 6561 7369 6c79  , you can easily
+0000a670: 2062 7569 6c64 2061 2042 656e 746f 2066   build a Bento f
+0000a680: 6f72 2061 0a20 2020 7370 6563 6966 6963  or a.   specific
+0000a690: 206d 6f64 656c 2c20 6c69 6b65 2060 6d69   model, like `mi
+0000a6a0: 7374 7261 6c61 692f 4d69 7374 7261 6c2d  stralai/Mistral-
+0000a6b0: 3742 2d49 6e73 7472 7563 742d 7630 2e31  7B-Instruct-v0.1
+0000a6c0: 602c 2075 7369 6e67 2074 6865 2060 6275  `, using the `bu
+0000a6d0: 696c 6460 2063 6f6d 6d61 6e64 2e3a 0a0a  ild` command.:..
+0000a6e0: 2020 2060 6060 6261 7368 0a20 2020 6f70     ```bash.   op
+0000a6f0: 656e 6c6c 6d20 6275 696c 6420 6d69 7374  enllm build mist
+0000a700: 7261 6c61 692f 4d69 7374 7261 6c2d 3742  ralai/Mistral-7B
+0000a710: 2d49 6e73 7472 7563 742d 7630 2e31 0a20  -Instruct-v0.1. 
+0000a720: 2020 6060 600a 0a20 2020 410a 2020 205b    ```..   A.   [
+0000a730: 4265 6e74 6f5d 2868 7474 7073 3a2f 2f64  Bento](https://d
+0000a740: 6f63 732e 6265 6e74 6f6d 6c2e 636f 6d2f  ocs.bentoml.com/
+0000a750: 656e 2f6c 6174 6573 742f 636f 6e63 6570  en/latest/concep
+0000a760: 7473 2f62 656e 746f 2e68 746d 6c23 7768  ts/bento.html#wh
+0000a770: 6174 2d69 732d 612d 6265 6e74 6f29 2c0a  at-is-a-bento),.
+0000a780: 2020 2069 6e20 4265 6e74 6f4d 4c2c 2069     in BentoML, i
+0000a790: 7320 7468 6520 756e 6974 206f 6620 6469  s the unit of di
+0000a7a0: 7374 7269 6275 7469 6f6e 2e20 4974 2070  stribution. It p
+0000a7b0: 6163 6b61 6765 7320 796f 7572 2070 726f  ackages your pro
+0000a7c0: 6772 616d 2773 2073 6f75 7263 650a 2020  gram's source.  
+0000a7d0: 2063 6f64 652c 206d 6f64 656c 732c 2066   code, models, f
+0000a7e0: 696c 6573 2c20 6172 7465 6661 6374 732c  iles, artefacts,
+0000a7f0: 2061 6e64 2064 6570 656e 6465 6e63 6965   and dependencie
+0000a800: 732e 0a0a 322e 202a 2a43 6f6e 7461 696e  s...2. **Contain
+0000a810: 6572 697a 6520 796f 7572 2042 656e 746f  erize your Bento
+0000a820: 2a2a 0a0a 2020 2060 6060 6261 7368 0a20  **..   ```bash. 
+0000a830: 2020 6265 6e74 6f6d 6c20 636f 6e74 6169    bentoml contai
+0000a840: 6e65 7269 7a65 203c 6e61 6d65 3a76 6572  nerize <name:ver
+0000a850: 7369 6f6e 3e0a 2020 2060 6060 0a0a 2020  sion>.   ```..  
+0000a860: 2054 6869 7320 6765 6e65 7261 7465 7320   This generates 
+0000a870: 6120 4f43 492d 636f 6d70 6174 6962 6c65  a OCI-compatible
+0000a880: 2064 6f63 6b65 7220 696d 6167 6520 7468   docker image th
+0000a890: 6174 2063 616e 2062 6520 6465 706c 6f79  at can be deploy
+0000a8a0: 6564 2061 6e79 7768 6572 650a 2020 2064  ed anywhere.   d
+0000a8b0: 6f63 6b65 7220 7275 6e73 2e20 466f 7220  ocker runs. For 
+0000a8c0: 6265 7374 2073 6361 6c61 6269 6c69 7479  best scalability
+0000a8d0: 2061 6e64 2072 656c 6961 6269 6c69 7479   and reliability
+0000a8e0: 206f 6620 796f 7572 204c 4c4d 2073 6572   of your LLM ser
+0000a8f0: 7669 6365 2069 6e0a 2020 2070 726f 6475  vice in.   produ
+0000a900: 6374 696f 6e2c 2077 6520 7265 636f 6d6d  ction, we recomm
+0000a910: 656e 6420 6465 706c 6f79 2077 6974 6820  end deploy with 
+0000a920: 4265 6e74 6f43 6c6f 7564 e380 820a 0a23  BentoCloud.....#
+0000a930: 2323 20e2 9881 efb8 8f20 4265 6e74 6f43  ## ...... BentoC
+0000a940: 6c6f 7564 0a0a 4465 706c 6f79 204f 7065  loud..Deploy Ope
+0000a950: 6e4c 4c4d 2077 6974 6820 5b42 656e 746f  nLLM with [Bento
+0000a960: 436c 6f75 645d 2868 7474 7073 3a2f 2f77  Cloud](https://w
+0000a970: 7777 2e62 656e 746f 6d6c 2e63 6f6d 2f29  ww.bentoml.com/)
+0000a980: 2c20 7468 6520 696e 6665 7265 6e63 6520  , the inference 
+0000a990: 706c 6174 666f 726d 0a66 6f72 2066 6173  platform.for fas
+0000a9a0: 7420 6d6f 7669 6e67 2041 4920 7465 616d  t moving AI team
+0000a9b0: 732e 0a0a 312e 202a 2a43 7265 6174 6520  s...1. **Create 
+0000a9c0: 6120 4265 6e74 6f43 6c6f 7564 2061 6363  a BentoCloud acc
+0000a9d0: 6f75 6e74 3a2a 2a20 5b73 6967 6e20 7570  ount:** [sign up
+0000a9e0: 2068 6572 655d 2868 7474 7073 3a2f 2f62   here](https://b
+0000a9f0: 656e 746f 6d6c 2e63 6f6d 2f29 0a0a 322e  entoml.com/)..2.
+0000aa00: 202a 2a4c 6f67 2069 6e74 6f20 796f 7572   **Log into your
+0000aa10: 2042 656e 746f 436c 6f75 6420 6163 636f   BentoCloud acco
+0000aa20: 756e 743a 2a2a 0a0a 2020 2060 6060 6261  unt:**..   ```ba
+0000aa30: 7368 0a20 2020 6265 6e74 6f6d 6c20 636c  sh.   bentoml cl
+0000aa40: 6f75 6420 6c6f 6769 6e20 2d2d 6170 692d  oud login --api-
+0000aa50: 746f 6b65 6e20 3c79 6f75 722d 6170 692d  token <your-api-
+0000aa60: 746f 6b65 6e3e 202d 2d65 6e64 706f 696e  token> --endpoin
+0000aa70: 7420 3c62 656e 746f 2d63 6c6f 7564 2d65  t <bento-cloud-e
+0000aa80: 6e64 706f 696e 743e 0a20 2020 6060 600a  ndpoint>.   ```.
+0000aa90: 0a3e 205b 214e 4f54 455d 0a3e 2052 6570  .> [!NOTE].> Rep
+0000aaa0: 6c61 6365 2060 3c79 6f75 722d 6170 692d  lace `<your-api-
+0000aab0: 746f 6b65 6e3e 6020 616e 6420 603c 6265  token>` and `<be
+0000aac0: 6e74 6f2d 636c 6f75 642d 656e 6470 6f69  nto-cloud-endpoi
+0000aad0: 6e74 3e60 2077 6974 6820 796f 7572 0a3e  nt>` with your.>
+0000aae0: 2073 7065 6369 6669 6320 4150 4920 746f   specific API to
+0000aaf0: 6b65 6e20 616e 6420 7468 6520 4265 6e74  ken and the Bent
+0000ab00: 6f43 6c6f 7564 2065 6e64 706f 696e 7420  oCloud endpoint 
+0000ab10: 7265 7370 6563 7469 7665 6c79 2e0a 0a33  respectively...3
+0000ab20: 2e20 2a2a 4275 6c64 696e 6720 6120 4265  . **Bulding a Be
+0000ab30: 6e74 6f2a 2a3a 2057 6974 6820 4f70 656e  nto**: With Open
+0000ab40: 4c4c 4d2c 2079 6f75 2063 616e 2065 6173  LLM, you can eas
+0000ab50: 696c 7920 6275 696c 6420 6120 4265 6e74  ily build a Bent
+0000ab60: 6f20 666f 7220 610a 2020 2073 7065 6369  o for a.   speci
+0000ab70: 6669 6320 6d6f 6465 6c2c 2073 7563 6820  fic model, such 
+0000ab80: 6173 2060 6d69 7374 7261 6c61 692f 4d69  as `mistralai/Mi
+0000ab90: 7374 7261 6c2d 3742 2d49 6e73 7472 7563  stral-7B-Instruc
+0000aba0: 742d 7630 2e31 603a 0a0a 2020 2060 6060  t-v0.1`:..   ```
+0000abb0: 6261 7368 0a20 2020 6f70 656e 6c6c 6d20  bash.   openllm 
+0000abc0: 6275 696c 6420 6d69 7374 7261 6c61 692f  build mistralai/
+0000abd0: 4d69 7374 7261 6c2d 3742 2d49 6e73 7472  Mistral-7B-Instr
+0000abe0: 7563 742d 7630 2e31 0a20 2020 6060 600a  uct-v0.1.   ```.
+0000abf0: 0a34 2e20 2a2a 5075 7368 696e 6720 6120  .4. **Pushing a 
+0000ac00: 4265 6e74 6f2a 2a3a 2050 7573 6820 796f  Bento**: Push yo
+0000ac10: 7572 2066 7265 7368 6c79 2d62 7569 6c74  ur freshly-built
+0000ac20: 2042 656e 746f 2073 6572 7669 6365 2074   Bento service t
+0000ac30: 6f20 4265 6e74 6f43 6c6f 7564 2076 6961  o BentoCloud via
+0000ac40: 0a20 2020 7468 6520 6070 7573 6860 2063  .   the `push` c
+0000ac50: 6f6d 6d61 6e64 3a0a 0a20 2020 6060 6062  ommand:..   ```b
+0000ac60: 6173 680a 2020 2062 656e 746f 6d6c 2070  ash.   bentoml p
+0000ac70: 7573 6820 3c6e 616d 653a 7665 7273 696f  ush <name:versio
+0000ac80: 6e3e 0a20 2020 6060 600a 0a35 2e20 2a2a  n>.   ```..5. **
+0000ac90: 4465 706c 6f79 696e 6720 6120 4265 6e74  Deploying a Bent
+0000aca0: 6f2a 2a3a 2044 6570 6c6f 7920 796f 7572  o**: Deploy your
+0000acb0: 204c 4c4d 7320 746f 2042 656e 746f 436c   LLMs to BentoCl
+0000acc0: 6f75 6420 7769 7468 2061 2073 696e 676c  oud with a singl
+0000acd0: 650a 2020 2060 6265 6e74 6f6d 6c20 6465  e.   `bentoml de
+0000ace0: 706c 6f79 6d65 6e74 2063 7265 6174 6560  ployment create`
+0000acf0: 2063 6f6d 6d61 6e64 2066 6f6c 6c6f 7769   command followi
+0000ad00: 6e67 2074 6865 0a20 2020 5b64 6570 6c6f  ng the.   [deplo
+0000ad10: 796d 656e 7420 696e 7374 7275 6374 696f  yment instructio
+0000ad20: 6e73 5d28 6874 7470 733a 2f2f 646f 6373  ns](https://docs
+0000ad30: 2e62 656e 746f 6d6c 2e63 6f6d 2f65 6e2f  .bentoml.com/en/
+0000ad40: 6c61 7465 7374 2f72 6566 6572 656e 6365  latest/reference
+0000ad50: 2f63 6c69 2e68 746d 6c23 6265 6e74 6f6d  /cli.html#bentom
+0000ad60: 6c2d 6465 706c 6f79 6d65 6e74 2d63 7265  l-deployment-cre
+0000ad70: 6174 6529 2e0a 0a23 2320 f09f 91a5 2043  ate)...## .... C
+0000ad80: 6f6d 6d75 6e69 7479 0a0a 456e 6761 6765  ommunity..Engage
+0000ad90: 2077 6974 6820 6c69 6b65 2d6d 696e 6465   with like-minde
+0000ada0: 6420 696e 6469 7669 6475 616c 7320 7061  d individuals pa
+0000adb0: 7373 696f 6e61 7465 2061 626f 7574 204c  ssionate about L
+0000adc0: 4c4d 732c 2041 492c 2061 6e64 206d 6f72  LMs, AI, and mor
+0000add0: 6520 6f6e 206f 7572 0a5b 4469 7363 6f72  e on our.[Discor
+0000ade0: 645d 2868 7474 7073 3a2f 2f6c 2e62 656e  d](https://l.ben
+0000adf0: 746f 6d6c 2e63 6f6d 2f6a 6f69 6e2d 6f70  toml.com/join-op
+0000ae00: 656e 6c6c 6d2d 6469 7363 6f72 6429 210a  enllm-discord)!.
+0000ae10: 0a4f 7065 6e4c 4c4d 2069 7320 6163 7469  .OpenLLM is acti
+0000ae20: 7665 6c79 206d 6169 6e74 6169 6e65 6420  vely maintained 
+0000ae30: 6279 2074 6865 2042 656e 746f 4d4c 2074  by the BentoML t
+0000ae40: 6561 6d2e 2046 6565 6c20 6672 6565 2074  eam. Feel free t
+0000ae50: 6f20 7265 6163 6820 6f75 7420 616e 640a  o reach out and.
+0000ae60: 6a6f 696e 2075 7320 696e 206f 7572 2070  join us in our p
+0000ae70: 7572 7375 6974 2074 6f20 6d61 6b65 204c  ursuit to make L
+0000ae80: 4c4d 7320 6d6f 7265 2061 6363 6573 7369  LMs more accessi
+0000ae90: 626c 6520 616e 6420 6561 7379 2074 6f20  ble and easy to 
+0000aea0: 7573 6520 f09f 9189 0a5b 4a6f 696e 206f  use .....[Join o
+0000aeb0: 7572 2053 6c61 636b 2063 6f6d 6d75 6e69  ur Slack communi
+0000aec0: 7479 215d 2868 7474 7073 3a2f 2f6c 2e62  ty!](https://l.b
+0000aed0: 656e 746f 6d6c 2e63 6f6d 2f6a 6f69 6e2d  entoml.com/join-
+0000aee0: 736c 6163 6b29 0a0a 2323 20f0 9f8e 8120  slack)..## .... 
+0000aef0: 436f 6e74 7269 6275 7469 6e67 0a0a 5765  Contributing..We
+0000af00: 2077 656c 636f 6d65 2063 6f6e 7472 6962   welcome contrib
+0000af10: 7574 696f 6e73 2120 4966 2079 6f75 2772  utions! If you'r
+0000af20: 6520 696e 7465 7265 7374 6564 2069 6e20  e interested in 
+0000af30: 656e 6861 6e63 696e 6720 4f70 656e 4c4c  enhancing OpenLL
+0000af40: 4d27 730a 6361 7061 6269 6c69 7469 6573  M's.capabilities
+0000af50: 206f 7220 6861 7665 2061 6e79 2071 7565   or have any que
+0000af60: 7374 696f 6e73 2c20 646f 6e27 7420 6865  stions, don't he
+0000af70: 7369 7461 7465 2074 6f20 7265 6163 6820  sitate to reach 
+0000af80: 6f75 7420 696e 206f 7572 0a5b 6469 7363  out in our.[disc
+0000af90: 6f72 6420 6368 616e 6e65 6c5d 2868 7474  ord channel](htt
+0000afa0: 7073 3a2f 2f6c 2e62 656e 746f 6d6c 2e63  ps://l.bentoml.c
+0000afb0: 6f6d 2f6a 6f69 6e2d 6f70 656e 6c6c 6d2d  om/join-openllm-
+0000afc0: 6469 7363 6f72 6429 2e0a 0a43 6865 636b  discord)...Check
+0000afd0: 6f75 7420 6f75 720a 5b44 6576 656c 6f70  out our.[Develop
+0000afe0: 6572 2047 7569 6465 5d28 6874 7470 733a  er Guide](https:
+0000aff0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
+0000b000: 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62 6c6f  toml/OpenLLM/blo
+0000b010: 622f 6d61 696e 2f44 4556 454c 4f50 4d45  b/main/DEVELOPME
+0000b020: 4e54 2e6d 6429 0a69 6620 796f 7520 7769  NT.md).if you wi
+0000b030: 7368 2074 6f20 636f 6e74 7269 6275 7465  sh to contribute
+0000b040: 2074 6f20 4f70 656e 4c4c 4d27 7320 636f   to OpenLLM's co
+0000b050: 6465 6261 7365 2e0a 0a23 2320 f09f 8d87  debase...## ....
+0000b060: 2054 656c 656d 6574 7279 0a0a 4f70 656e   Telemetry..Open
+0000b070: 4c4c 4d20 636f 6c6c 6563 7473 2075 7361  LLM collects usa
+0000b080: 6765 2064 6174 6120 746f 2065 6e68 616e  ge data to enhan
+0000b090: 6365 2075 7365 7220 6578 7065 7269 656e  ce user experien
+0000b0a0: 6365 2061 6e64 2069 6d70 726f 7665 2074  ce and improve t
+0000b0b0: 6865 2070 726f 6475 6374 2e0a 5765 206f  he product..We o
+0000b0c0: 6e6c 7920 7265 706f 7274 204f 7065 6e4c  nly report OpenL
+0000b0d0: 4c4d 2773 2069 6e74 6572 6e61 6c20 4150  LM's internal AP
+0000b0e0: 4920 6361 6c6c 7320 616e 6420 656e 7375  I calls and ensu
+0000b0f0: 7265 206d 6178 696d 756d 2070 7269 7661  re maximum priva
+0000b100: 6379 2062 790a 6578 636c 7564 696e 6720  cy by.excluding 
+0000b110: 7365 6e73 6974 6976 6520 696e 666f 726d  sensitive inform
+0000b120: 6174 696f 6e2e 2057 6520 7769 6c6c 206e  ation. We will n
+0000b130: 6576 6572 2063 6f6c 6c65 6374 2075 7365  ever collect use
+0000b140: 7220 636f 6465 2c20 6d6f 6465 6c20 6461  r code, model da
+0000b150: 7461 2c20 6f72 0a73 7461 636b 2074 7261  ta, or.stack tra
+0000b160: 6365 732e 2046 6f72 2075 7361 6765 2074  ces. For usage t
+0000b170: 7261 636b 696e 672c 2063 6865 636b 206f  racking, check o
+0000b180: 7574 2074 6865 0a5b 636f 6465 5d28 6874  ut the.[code](ht
+0000b190: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0000b1a0: 2f62 656e 746f 6d6c 2f4f 7065 6e4c 4c4d  /bentoml/OpenLLM
+0000b1b0: 2f62 6c6f 622f 6d61 696e 2f6f 7065 6e6c  /blob/main/openl
+0000b1c0: 6c6d 2d63 6f72 652f 7372 632f 6f70 656e  lm-core/src/open
+0000b1d0: 6c6c 6d5f 636f 7265 2f75 7469 6c73 2f61  llm_core/utils/a
+0000b1e0: 6e61 6c79 7469 6373 2e70 7929 2e0a 0a59  nalytics.py)...Y
+0000b1f0: 6f75 2063 616e 206f 7074 206f 7574 206f  ou can opt out o
+0000b200: 6620 7573 6167 6520 7472 6163 6b69 6e67  f usage tracking
+0000b210: 2062 7920 7573 696e 6720 7468 6520 602d   by using the `-
+0000b220: 2d64 6f2d 6e6f 742d 7472 6163 6b60 2043  -do-not-track` C
+0000b230: 4c49 206f 7074 696f 6e3a 0a0a 6060 6062  LI option:..```b
+0000b240: 6173 680a 6f70 656e 6c6c 6d20 5b63 6f6d  ash.openllm [com
+0000b250: 6d61 6e64 5d20 2d2d 646f 2d6e 6f74 2d74  mand] --do-not-t
+0000b260: 7261 636b 0a60 6060 0a0a 4f72 2062 7920  rack.```..Or by 
+0000b270: 7365 7474 696e 6720 7468 6520 656e 7669  setting the envi
+0000b280: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+0000b290: 2060 4f50 454e 4c4c 4d5f 444f 5f4e 4f54   `OPENLLM_DO_NOT
+0000b2a0: 5f54 5241 434b 3d54 7275 6560 3a0a 0a60  _TRACK=True`:..`
+0000b2b0: 6060 6261 7368 0a65 7870 6f72 7420 4f50  ``bash.export OP
+0000b2c0: 454e 4c4c 4d5f 444f 5f4e 4f54 5f54 5241  ENLLM_DO_NOT_TRA
+0000b2d0: 434b 3d54 7275 650a 6060 600a 0a23 2320  CK=True.```..## 
+0000b2e0: f09f 9394 2043 6974 6174 696f 6e0a 0a49  .... Citation..I
+0000b2f0: 6620 796f 7520 7573 6520 4f70 656e 4c4c  f you use OpenLL
+0000b300: 4d20 696e 2079 6f75 7220 7265 7365 6172  M in your resear
+0000b310: 6368 2c20 7765 2070 726f 7669 6465 2061  ch, we provide a
+0000b320: 205b 6369 7461 7469 6f6e 5d28 2e2f 4349   [citation](./CI
+0000b330: 5441 5449 4f4e 2e63 6666 2920 746f 0a75  TATION.cff) to.u
+0000b340: 7365 3a0a 0a60 6060 6269 6274 6578 0a40  se:..```bibtex.@
+0000b350: 736f 6674 7761 7265 7b50 6861 6d5f 4f70  software{Pham_Op
+0000b360: 656e 4c4c 4d5f 4f70 6572 6174 696e 675f  enLLM_Operating_
+0000b370: 4c4c 4d73 5f32 3032 332c 0a61 7574 686f  LLMs_2023,.autho
+0000b380: 7220 3d20 7b50 6861 6d2c 2041 6172 6f6e  r = {Pham, Aaron
+0000b390: 2061 6e64 2059 616e 672c 2043 6861 6f79   and Yang, Chaoy
+0000b3a0: 7520 616e 6420 5368 656e 672c 2053 6561  u and Sheng, Sea
+0000b3b0: 6e20 616e 6420 205a 6861 6f2c 2053 6865  n and  Zhao, She
+0000b3c0: 6e79 616e 6720 616e 6420 4c65 652c 2053  nyang and Lee, S
+0000b3d0: 6175 796f 6e20 616e 6420 4a69 616e 672c  auyon and Jiang,
+0000b3e0: 2042 6f20 616e 6420 446f 6e67 2c20 466f   Bo and Dong, Fo
+0000b3f0: 6720 616e 6420 4775 616e 2c20 5869 7065  g and Guan, Xipe
+0000b400: 6e67 2061 6e64 204d 696e 672c 2046 726f  ng and Ming, Fro
+0000b410: 7374 7d2c 0a6c 6963 656e 7365 203d 207b  st},.license = {
+0000b420: 4170 6163 6865 2d32 2e30 7d2c 0a6d 6f6e  Apache-2.0},.mon
+0000b430: 7468 203d 206a 756e 2c0a 7469 746c 6520  th = jun,.title 
+0000b440: 3d20 7b7b 4f70 656e 4c4c 4d3a 204f 7065  = {{OpenLLM: Ope
+0000b450: 7261 7469 6e67 204c 4c4d 7320 696e 2070  rating LLMs in p
+0000b460: 726f 6475 6374 696f 6e7d 7d2c 0a75 726c  roduction}},.url
+0000b470: 203d 207b 6874 7470 733a 2f2f 6769 7468   = {https://gith
+0000b480: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
+0000b490: 7065 6e4c 4c4d 7d2c 0a79 6561 7220 3d20  penLLM},.year = 
+0000b4a0: 7b32 3032 337d 0a7d 0a60 6060 0a0a 2323  {2023}.}.```..##
+0000b4b0: 2052 656c 6561 7365 2049 6e66 6f72 6d61   Release Informa
+0000b4c0: 7469 6f6e 0a0a 2323 2320 4261 636b 7761  tion..### Backwa
+0000b4d0: 7264 732d 696e 636f 6d70 6174 6962 6c65  rds-incompatible
+0000b4e0: 2043 6861 6e67 6573 0a0a 2d20 2323 2320   Changes..- ### 
+0000b4f0: 6f70 656e 6c6c 6d2d 636f 7265 0a0a 2020  openllm-core..  
+0000b500: 4275 6d70 2060 6174 7472 7360 2074 6f20  Bump `attrs` to 
+0000b510: 6032 332e 322e 3060 0a0a 2020 4164 6465  `23.2.0`..  Adde
+0000b520: 6420 6578 7065 7269 6d65 6e74 616c 2068  d experimental h
+0000b530: 656c 7065 7273 2060 2e70 7964 616e 7469  elpers `.pydanti
+0000b540: 635f 6d6f 6465 6c28 2960 2066 756e 6374  c_model()` funct
+0000b550: 696f 6e73 2074 6f20 636f 6e76 6572 7420  ions to convert 
+0000b560: 6375 7272 656e 7420 6174 7472 732d 6261  current attrs-ba
+0000b570: 7365 6420 636c 6173 7320 746f 2069 7473  sed class to its
+0000b580: 2063 6f6d 7061 7469 626c 6520 7079 6461   compatible pyda
+0000b590: 6e74 6963 2063 6c61 7373 2e0a 0a20 2023  ntic class...  #
+0000b5a0: 2323 206f 7065 6e6c 6c6d 0a0a 2020 5570  ## openllm..  Up
+0000b5b0: 6461 7465 6420 4f70 656e 4c4c 4d20 6172  dated OpenLLM ar
+0000b5c0: 6368 6974 6563 7475 7265 2074 6f20 6e65  chitecture to ne
+0000b5d0: 7720 312e 3220 4265 6e74 6f4d 4c2e 0a0a  w 1.2 BentoML...
+0000b5e0: 2020 606f 7065 6e6c 6c6d 2e52 756e 6e65    `openllm.Runne
+0000b5f0: 7260 2072 656d 6169 6e73 2074 6865 206f  r` remains the o
+0000b600: 6c64 2052 756e 6e61 626c 6520 696d 706c  ld Runnable impl
+0000b610: 656d 656e 7461 7469 6f6e 2e20 5468 6572  ementation. Ther
+0000b620: 6566 6f72 652c 2069 6620 796f 7520 7374  efore, if you st
+0000b630: 696c 6c20 6465 7065 6e64 7320 6f6e 2074  ill depends on t
+0000b640: 6865 206f 6c64 2061 7263 6869 7465 6374  he old architect
+0000b650: 7572 652c 206d 616b 6520 7375 7265 2074  ure, make sure t
+0000b660: 6f20 7573 6520 606f 7065 6e6c 6c6d 2e52  o use `openllm.R
+0000b670: 756e 6e65 7260 2069 6e73 7465 6164 206f  unner` instead o
+0000b680: 6620 606c 6c6d 2e72 756e 6e65 7260 2e0a  f `llm.runner`..
+0000b690: 0a20 2060 6c6c 6d2e 7275 6e6e 6572 6020  .  `llm.runner` 
+0000b6a0: 7769 6c6c 206e 6f77 2062 6563 6f6d 6520  will now become 
+0000b6b0: 616e 2060 6265 6e74 6f6d 6c2e 6465 7065  an `bentoml.depe
+0000b6c0: 6e64 7328 2960 2073 696e 676c 6574 6f6e  nds()` singleton
+0000b6d0: 2c20 7468 6572 6566 6f72 652c 2074 6f20  , therefore, to 
+0000b6e0: 6176 6f69 6420 6272 6561 6b69 6e67 2063  avoid breaking c
+0000b6f0: 6861 6e67 652c 206d 616b 6520 7375 7265  hange, make sure
+0000b700: 2074 6f20 7365 7420 604f 5045 4e4c 4c4d   to set `OPENLLM
+0000b710: 5f52 554e 4e45 525f 4245 4841 5649 4f55  _RUNNER_BEHAVIOU
+0000b720: 523d 6465 7072 6563 6174 6564 6020 696e  R=deprecated` in
+0000b730: 2079 6f75 7220 656e 7669 726f 6e6d 656e   your environmen
+0000b740: 7420 7661 7269 6162 6c65 2e20 5468 6973  t variable. This
+0000b750: 2069 7320 7468 6520 6465 6661 756c 7420   is the default 
+0000b760: 6265 6861 7669 6f75 722e 2054 6f20 6f70  behaviour. To op
+0000b770: 742d 696e 2074 6865 206e 6577 2061 7263  t-in the new arc
+0000b780: 6869 7465 6374 7572 652c 2073 6574 2060  hitecture, set `
+0000b790: 4f50 454e 4c4c 4d5f 5255 4e4e 4552 5f42  OPENLLM_RUNNER_B
+0000b7a0: 4548 4156 494f 5552 3d6e 6577 5f69 6d70  EHAVIOUR=new_imp
+0000b7b0: 6c60 0a20 205b 2338 3231 5d28 6874 7470  l`.  [#821](http
+0000b7c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
+0000b7d0: 656e 746f 6d6c 2f6f 7065 6e6c 6c6d 2f69  entoml/openllm/i
+0000b7e0: 7373 7565 732f 3832 3129 0a0a 0a2d 2d2d  ssues/821)...---
+0000b7f0: 0a0a 5b43 6c69 636b 206d 6520 666f 7220  ..[Click me for 
+0000b800: 6675 6c6c 2063 6861 6e67 656c 6f67 5d28  full changelog](
+0000b810: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000b820: 6f6d 2f62 656e 746f 6d6c 2f6f 7065 6e6c  om/bentoml/openl
+0000b830: 6c6d 2f62 6c6f 622f 6d61 696e 2f43 4841  lm/blob/main/CHA
+0000b840: 4e47 454c 4f47 2e6d 6429 0a              NGELOG.md).
```

### Comparing `openllm-0.5.0a3/pyoxidizer.bzl` & `openllm-0.5.0a4/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/_service_vars.pyi` & `openllm-0.5.0a4/src/_service_vars.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/__init__.pyi` & `openllm-0.5.0a4/src/_openllm_tiny/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/_entrypoint.py` & `openllm-0.5.0a4/src/_openllm_tiny/_entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
 
 def construct_python_options(llm_config, llm_fs):
   from bentoml._internal.bento.build_config import PythonOptions
   from openllm.bundle._package import build_editable
 
   # TODO: Add this line back once 0.5 is out, for now depends on OPENLLM_DEV_BUILD
   # packages = ['scipy', 'bentoml[tracing]>=1.2.8', 'openllm[vllm]>0.4', 'vllm>=0.3']
-  packages = ['scipy', 'bentoml[tracing]>=1.2.8', 'vllm>=0.3']
+  packages = ['scipy', 'bentoml[tracing]>=1.2.8', 'vllm==0.4.2']
   if llm_config['requirements'] is not None:
     packages.extend(llm_config['requirements'])
   built_wheels = [build_editable(llm_fs.getsyspath('/'), p) for p in ('openllm_core', 'openllm_client', 'openllm')]
   return PythonOptions(
     packages=packages,
     wheels=[llm_fs.getsyspath(f"/{i.split('/')[-1]}") for i in built_wheels] if all(i for i in built_wheels) else None,
     lock_packages=False,
@@ -458,15 +458,15 @@
         build_ctx=llm_fs.getsyspath('/'),
         build_config=BentoBuildConfig(
           service=f"{llm_config['service_name']}:LLMService",
           name=bento_tag.name,
           labels=labels,
           models=models,
           envs=[
-            EnvironmentEntry(name='OPENLLM_CONFIG', value=llm_config.model_dump_json()),
+            EnvironmentEntry(name='OPENLLM_CONFIG', value=f"'{llm_config.model_dump_json()}'"),
             EnvironmentEntry(name='NVIDIA_DRIVER_CAPABILITIES', value='compute,utility'),
           ],
           description=f"OpenLLM service for {llm_config['start_name']}",
           include=list(llm_fs.walk.files()),
           exclude=['/venv', '/.venv', '__pycache__/', '*.py[cod]', '*$py.class'],
           python=construct_python_options(llm_config, llm_fs),
           docker=DockerOptions(python_version='3.11'),
```

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/_helpers.py` & `openllm-0.5.0a4/src/_openllm_tiny/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/_llm.py` & `openllm-0.5.0a4/src/_openllm_tiny/_llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   get_debug_mode,
   is_vllm_available,
   normalise_model_name,
   gen_random_uuid,
   dict_filter_none,
 )
 from openllm_core._typing_compat import LiteralQuantise, LiteralSerialisation, LiteralDtype
-from openllm_core._schemas import GenerationOutput, GenerationInput
+from openllm_core._schemas import GenerationOutput
 
 Dtype = t.Union[LiteralDtype, t.Literal['auto', 'half', 'float']]
 
 if t.TYPE_CHECKING:
   from vllm import RequestOutput
 
 
@@ -145,15 +145,15 @@
     stop_token_ids: list[int] | None = None,
     request_id: str | None = None,
     adapter_name: str | None = None,
     **attrs: t.Any,
   ) -> t.AsyncGenerator[RequestOutput, None]:
     from vllm import SamplingParams
 
-    config = self.config.generation_config.model_copy(update=dict_filter_none(attrs))
+    config = self.config.model_construct_env(**dict_filter_none(attrs))
 
     stop_token_ids = stop_token_ids or []
     eos_token_id = attrs.get('eos_token_id', config['eos_token_id'])
     if eos_token_id and not isinstance(eos_token_id, list):
       eos_token_id = [eos_token_id]
     stop_token_ids.extend(eos_token_id or [])
     if (config_eos := config['eos_token_id']) and config_eos not in stop_token_ids:
@@ -168,57 +168,58 @@
       stop = set(stop)
 
     request_id = gen_random_uuid() if request_id is None else request_id
 
     top_p = 1.0 if config['temperature'] <= 1e-5 else config['top_p']
     config = config.model_copy(update=dict(stop=list(stop), stop_token_ids=stop_token_ids, top_p=top_p))
 
-    params = {k: getattr(config, k, None) for k in set(inspect.signature(SamplingParams).parameters.keys())}
-    sampling_params = SamplingParams(**{k: v for k, v in params.items() if v is not None})
-
     try:
       async for it in self._model.generate(
-        prompt, sampling_params=sampling_params, request_id=request_id, prompt_token_ids=prompt_token_ids
+        prompt,
+        sampling_params=SamplingParams(**{
+          k: config.__getitem__(k) for k in set(inspect.signature(SamplingParams).parameters.keys())
+        }),
+        request_id=request_id,
+        prompt_token_ids=prompt_token_ids,
       ):
         yield it
     except Exception as err:
       raise RuntimeError(f'Failed to start generation task: {err}') from err
 
   async def generate(
     self,
     prompt: str | None,
     prompt_token_ids: list[int] | None = None,
     stop: str | t.Iterable[str] | None = None,
     stop_token_ids: list[int] | None = None,
     request_id: str | None = None,
     adapter_name: str | None = None,
-    *,
-    _generated: GenerationInput | None = None,
     **attrs: t.Any,
   ) -> GenerationOutput:
     if stop is not None:
       attrs.update({'stop': stop})
     if stop_token_ids is not None:
       attrs.update({'stop_token_ids': stop_token_ids})
-    config = self.config.model_copy(update=attrs)
+    config = self.config.model_construct_env(**attrs)
     texts, token_ids = [[]] * config['n'], [[]] * config['n']
     async for result in self.generate_iterator(
       prompt,
       prompt_token_ids=prompt_token_ids,
       request_id=request_id,
       adapter_name=adapter_name,
       **config.model_dump(),
     ):
       for output in result.outputs:
         texts[output.index].append(output.text)
         token_ids[output.index].extend(output.token_ids)
     if (final_result := result) is None:
       raise RuntimeError('No result is returned.')
-    return GenerationOutput.from_vllm(final_result).model_copy(
+    converted = GenerationOutput.from_vllm(final_result)
+    return converted.model_copy(
       update=dict(
         prompt=prompt,
         outputs=[
           output.model_copy(update=dict(text=''.join(texts[output.index]), token_ids=token_ids[output.index]))
-          for output in final_result.outputs
+          for output in converted.outputs
         ],
       )
     )
```

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/_service.py` & `openllm-0.5.0a4/src/_openllm_tiny/_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-import importlib.metadata
+import openllm, bentoml, logging, pydantic, importlib.metadata
+import openllm_core as core, _service_vars as svars, typing as t
+
 from http import HTTPStatus
 from starlette.requests import Request
 from starlette.responses import JSONResponse, StreamingResponse
-import openllm, bentoml, logging, openllm_core as core
-import _service_vars as svars, typing as t
 from openllm_core._typing_compat import Annotated
 from openllm_core._schemas import MessageParam, MessagesConverterInput
 from openllm_core.protocol.openai import ModelCard, ModelList, ChatCompletionRequest
 from _openllm_tiny._helpers import OpenAI, Error
 
 try:
   from fastapi import FastAPI
@@ -54,47 +54,39 @@
       gpu_memory_utilization=svars.gpu_memory_utilization,
     )
     self.openai = OpenAI(self.llm)
 
   @core.utils.api(route='/v1/generate')
   async def generate_v1(
     self,
-    llm_config: t.Dict[str, t.Any],
-    prompt: str = 'What is the meaning of life?',
+    prompt: str = pydantic.Field(default='What is the meaning of life?', description='Given prompt to generate from'),
     prompt_token_ids: t.Optional[t.List[int]] = None,
     stop: t.Optional[t.List[str]] = None,
     stop_token_ids: t.Optional[t.List[int]] = None,
     request_id: t.Optional[str] = None,
+    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=llm_config, description='LLM Config'),
   ) -> core.GenerationOutput:
+    llm_config.update(stop=stop, stop_token_ids=stop_token_ids)
     return await self.llm.generate(
-      prompt=prompt,
-      prompt_token_ids=prompt_token_ids,
-      llm_config=llm_config,
-      stop=stop,
-      stop_token_ids=stop_token_ids,
-      request_id=request_id,
+      prompt=prompt, prompt_token_ids=prompt_token_ids, request_id=request_id, **llm_config
     )
 
   @core.utils.api(route='/v1/generate_stream')
   async def generate_stream_v1(
     self,
-    llm_config: t.Dict[str, t.Any],
-    prompt: str = 'What is the meaning of life?',
+    prompt: str = pydantic.Field(default='What is the meaning of life?', description='Given prompt to generate from'),
     prompt_token_ids: t.Optional[t.List[int]] = None,
     stop: t.Optional[t.List[str]] = None,
     stop_token_ids: t.Optional[t.List[int]] = None,
     request_id: t.Optional[str] = None,
+    llm_config: t.Dict[str, t.Any] = pydantic.Field(default=llm_config, description='LLM Config'),
   ) -> t.AsyncGenerator[str, None]:
+    llm_config.update(stop=stop, stop_token_ids=stop_token_ids)
     async for generated in self.llm.generate_iterator(
-      prompt=prompt,
-      prompt_token_ids=prompt_token_ids,
-      llm_config=llm_config,
-      stop=stop,
-      stop_token_ids=stop_token_ids,
-      request_id=request_id,
+      prompt=prompt, prompt_token_ids=prompt_token_ids, request_id=request_id, **llm_config
     ):
       yield f'data: {core.GenerationOutput.from_vllm(generated).model_dump_json()}\n\n'
     yield 'data: [DONE]\n\n'
 
   @core.utils.api(route='/v1/metadata')
   async def metadata_v1(self) -> core.MetadataOutput:
     return core.MetadataOutput(
@@ -104,21 +96,23 @@
       model_id=self.llm.model_id,
       configuration=self.llm.config.model_dump_json(),
     )
 
   @core.utils.api(route='/v1/helpers/messages')
   def helpers_messages_v1(
     self,
-    message: Annotated[t.Dict[str, t.Any], MessagesConverterInput] = MessagesConverterInput(
-      add_generation_prompt=False,
-      messages=[
-        MessageParam(role='system', content='You are acting as Ernest Hemmingway.'),
-        MessageParam(role='user', content='Hi there!'),
-        MessageParam(role='assistant', content='Yes?'),
-      ],
+    message: Annotated[t.Dict[str, t.Any], MessagesConverterInput] = pydantic.Field(
+      default=MessagesConverterInput(
+        add_generation_prompt=False,
+        messages=[
+          MessageParam(role='system', content='You are acting as Ernest Hemmingway.'),
+          MessageParam(role='user', content='Hi there!'),
+          MessageParam(role='assistant', content='Yes?'),
+        ],
+      )
     ),
   ) -> str:
     return self.llm._tokenizer.apply_chat_template(
       message['messages'], add_generation_prompt=message['add_generation_prompt'], tokenize=False
     )
 
   @app_v1.post(
@@ -132,14 +126,15 @@
     self,
     raw_request: Request,
     request: ChatCompletionRequest = ChatCompletionRequest(
       messages=[
         MessageParam(role='system', content='You are acting as Ernest Hemmingway.'),
         MessageParam(role='user', content='Hi there!'),
         MessageParam(role='assistant', content='Yes?'),
+        MessageParam(role='user', content='What is the meaning of life?'),
       ],
       model=core.utils.normalise_model_name(model_id),
       n=1,
       stream=True,
     ),
   ):
     generator = await self.openai.chat_completions(request, raw_request)
```

### Comparing `openllm-0.5.0a3/src/_openllm_tiny/_service_vars.py` & `openllm-0.5.0a4/src/_openllm_tiny/_service_vars.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/__init__.py` & `openllm-0.5.0a4/src/openllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/__init__.pyi` & `openllm-0.5.0a4/src/openllm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_deprecated.py` & `openllm-0.5.0a4/src/openllm/_deprecated.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_generation.py` & `openllm-0.5.0a4/src/openllm/_generation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_llm.py` & `openllm-0.5.0a4/src/openllm/_llm.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_llm.pyi` & `openllm-0.5.0a4/src/openllm/_llm.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_quantisation.py` & `openllm-0.5.0a4/src/openllm/_quantisation.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_quantisation.pyi` & `openllm-0.5.0a4/src/openllm/_quantisation.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_runners.py` & `openllm-0.5.0a4/src/openllm/_runners.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_runners.pyi` & `openllm-0.5.0a4/src/openllm/_runners.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_strategies.py` & `openllm-0.5.0a4/src/openllm/_strategies.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/_strategies.pyi` & `openllm-0.5.0a4/src/openllm/_strategies.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/utils.py` & `openllm-0.5.0a4/src/openllm/utils.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/utils.pyi` & `openllm-0.5.0a4/src/openllm/utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/bundle/__init__.py` & `openllm-0.5.0a4/src/openllm/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/bundle/__init__.pyi` & `openllm-0.5.0a4/src/openllm/bundle/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/bundle/_package.py` & `openllm-0.5.0a4/src/openllm/bundle/_package.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/bundle/_package.pyi` & `openllm-0.5.0a4/src/openllm/bundle/_package.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/entrypoints/_openapi.py` & `openllm-0.5.0a4/src/openllm/entrypoints/_openapi.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/entrypoints/_openapi.pyi` & `openllm-0.5.0a4/src/openllm/entrypoints/_openapi.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/entrypoints/hf.py` & `openllm-0.5.0a4/src/openllm/entrypoints/hf.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/entrypoints/openai.py` & `openllm-0.5.0a4/src/openllm/entrypoints/openai.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/entrypoints/openai.pyi` & `openllm-0.5.0a4/src/openllm/entrypoints/openai.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/__init__.py` & `openllm-0.5.0a4/src/openllm/serialisation/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/__init__.pyi` & `openllm-0.5.0a4/src/openllm/serialisation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/_helpers.py` & `openllm-0.5.0a4/src/openllm/serialisation/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/transformers/__init__.py` & `openllm-0.5.0a4/src/openllm/serialisation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/transformers/_helpers.py` & `openllm-0.5.0a4/src/openllm/serialisation/transformers/_helpers.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/transformers/weights.py` & `openllm-0.5.0a4/src/openllm/serialisation/transformers/weights.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm/serialisation/vllm/__init__.py` & `openllm-0.5.0a4/src/openllm/serialisation/vllm/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/_factory.py` & `openllm-0.5.0a4/src/openllm_cli/_factory.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/_sdk.py` & `openllm-0.5.0a4/src/openllm_cli/_sdk.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/termui.py` & `openllm-0.5.0a4/src/openllm_cli/termui.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/__init__.py` & `openllm-0.5.0a4/src/openllm_cli/extension/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/dive_bentos.py` & `openllm-0.5.0a4/src/openllm_cli/extension/dive_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/get_containerfile.py` & `openllm-0.5.0a4/src/openllm_cli/extension/get_containerfile.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/get_prompt.py` & `openllm-0.5.0a4/src/openllm_cli/extension/get_prompt.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/list_bentos.py` & `openllm-0.5.0a4/src/openllm_cli/extension/list_bentos.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/list_models.py` & `openllm-0.5.0a4/src/openllm_cli/extension/list_models.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/extension/playground.py` & `openllm-0.5.0a4/src/openllm_cli/extension/playground.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/playground/_meta.yml` & `openllm-0.5.0a4/src/openllm_cli/playground/_meta.yml`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/playground/falcon_tuned.py` & `openllm-0.5.0a4/src/openllm_cli/playground/falcon_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/playground/features.py` & `openllm-0.5.0a4/src/openllm_cli/playground/features.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/playground/llama2_qlora.py` & `openllm-0.5.0a4/src/openllm_cli/playground/llama2_qlora.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/src/openllm_cli/playground/opt_tuned.py` & `openllm-0.5.0a4/src/openllm_cli/playground/opt_tuned.py`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/.gitignore` & `openllm-0.5.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/LICENSE.md` & `openllm-0.5.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm-0.5.0a3/pyproject.toml` & `openllm-0.5.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,30 +36,30 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "bentoml[io]>=1.2",
     "transformers[torch,tokenizers]>=4.36.0",
-    "openllm-client>=0.5.0-alpha.3",
-    "openllm-core>=0.5.0-alpha.3",
+    "openllm-client>=0.5.0-alpha.4",
+    "openllm-core>=0.5.0-alpha.4",
     "safetensors",
-    "vllm>=0.4.0",
+    "vllm>=0.4.2",
     "optimum>=1.12.0",
     "accelerate",
     "ghapi",
     "einops",
     "sentencepiece",
     "scipy",
     "build[virtualenv]<1",
     "click>=8.1.3",
     "cuda-python;platform_system!=\"Darwin\"",
     "bitsandbytes<0.42",
 ]
-description = "OpenLLM: Operating LLMs in production"
+description = "OpenLLM: Run any open-source LLMs, such as Llama 2, Mistral, as OpenAI compatible API endpoint in the cloud."
 dynamic = ["version", "readme"]
 keywords = [
     "MLOps",
     "AI",
     "BentoML",
     "Model Serving",
     "Model Deployment",
@@ -120,15 +120,15 @@
 openai = ["openai[datalib]>=1", "tiktoken", "fastapi"]
 opt = ["triton"]
 phi = ["triton"]
 playground = ["jupyter", "notebook", "ipython", "jupytext", "nbformat"]
 qwen = ["cpm-kernels", "tiktoken"]
 stablelm = ["cpm-kernels", "tiktoken"]
 starcoder = ["bitsandbytes"]
-vllm = ["vllm==0.4.0"]
+vllm = ["vllm==0.4.2"]
 yi = ["bitsandbytes"]
 
 [tool.hatch.version]
 fallback-version = "0.0.0"
 source = "vcs"
 [tool.hatch.build.hooks.vcs]
 version-file = "src/openllm/_version.py"
```

### Comparing `openllm-0.5.0a3/PKG-INFO` & `openllm-0.5.0a4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,3334 +1,2543 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6f70 656e  : 2.1.Name: open
-00000020: 6c6c 6d0a 5665 7273 696f 6e3a 2030 2e35  llm.Version: 0.5
-00000030: 2e30 6133 0a53 756d 6d61 7279 3a20 4f70  .0a3.Summary: Op
-00000040: 656e 4c4c 4d3a 204f 7065 7261 7469 6e67  enLLM: Operating
-00000050: 204c 4c4d 7320 696e 2070 726f 6475 6374   LLMs in product
-00000060: 696f 6e0a 5072 6f6a 6563 742d 5552 4c3a  ion.Project-URL:
-00000070: 2042 6c6f 672c 2068 7474 7073 3a2f 2f6d   Blog, https://m
-00000080: 6f64 656c 7365 7276 696e 672e 636f 6d0a  odelserving.com.
-00000090: 5072 6f6a 6563 742d 5552 4c3a 2043 6861  Project-URL: Cha
-000000a0: 742c 2068 7474 7073 3a2f 2f64 6973 636f  t, https://disco
-000000b0: 7264 2e67 672f 6f70 656e 6c6c 6d0a 5072  rd.gg/openllm.Pr
-000000c0: 6f6a 6563 742d 5552 4c3a 2044 6f63 756d  oject-URL: Docum
-000000d0: 656e 7461 7469 6f6e 2c20 6874 7470 733a  entation, https:
-000000e0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
-000000f0: 746f 6d6c 2f6f 7065 6e6c 6c6d 2372 6561  toml/openllm#rea
-00000100: 646d 650a 5072 6f6a 6563 742d 5552 4c3a  dme.Project-URL:
-00000110: 2047 6974 4875 622c 2068 7474 7073 3a2f   GitHub, https:/
-00000120: 2f67 6974 6875 622e 636f 6d2f 6265 6e74  /github.com/bent
-00000130: 6f6d 6c2f 4f70 656e 4c4c 4d0a 5072 6f6a  oml/OpenLLM.Proj
-00000140: 6563 742d 5552 4c3a 2048 6973 746f 7279  ect-URL: History
-00000150: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000160: 2e63 6f6d 2f62 656e 746f 6d6c 2f4f 7065  .com/bentoml/Ope
-00000170: 6e4c 4c4d 2f62 6c6f 622f 6d61 696e 2f43  nLLM/blob/main/C
-00000180: 4841 4e47 454c 4f47 2e6d 640a 5072 6f6a  HANGELOG.md.Proj
-00000190: 6563 742d 5552 4c3a 2048 6f6d 6570 6167  ect-URL: Homepag
-000001a0: 652c 2068 7474 7073 3a2f 2f62 656e 746f  e, https://bento
-000001b0: 6d6c 2e63 6f6d 0a50 726f 6a65 6374 2d55  ml.com.Project-U
-000001c0: 524c 3a20 5472 6163 6b65 722c 2068 7474  RL: Tracker, htt
-000001d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001e0: 6265 6e74 6f6d 6c2f 4f70 656e 4c4c 4d2f  bentoml/OpenLLM/
-000001f0: 6973 7375 6573 0a50 726f 6a65 6374 2d55  issues.Project-U
-00000200: 524c 3a20 5477 6974 7465 722c 2068 7474  RL: Twitter, htt
-00000210: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00000220: 2f62 656e 746f 6d6c 6169 0a41 7574 686f  /bentomlai.Autho
-00000230: 722d 656d 6169 6c3a 2041 6172 6f6e 2050  r-email: Aaron P
-00000240: 6861 6d20 3c61 6172 6e70 686d 4062 656e  ham <aarnphm@ben
-00000250: 746f 6d6c 2e63 6f6d 3e2c 2042 656e 746f  toml.com>, Bento
-00000260: 4d4c 2054 6561 6d20 3c63 6f6e 7461 6374  ML Team <contact
-00000270: 4062 656e 746f 6d6c 2e63 6f6d 3e0a 4c69  @bentoml.com>.Li
-00000280: 6365 6e73 652d 4578 7072 6573 7369 6f6e  cense-Expression
-00000290: 3a20 4170 6163 6865 2d32 2e30 0a4c 6963  : Apache-2.0.Lic
-000002a0: 656e 7365 2d46 696c 653a 204c 4943 454e  ense-File: LICEN
-000002b0: 5345 2e6d 640a 4b65 7977 6f72 6473 3a20  SE.md.Keywords: 
-000002c0: 4149 2c41 6c70 6163 612c 4265 6e74 6f4d  AI,Alpaca,BentoM
-000002d0: 4c2c 4661 6c63 6f6e 2c46 696e 6520 7475  L,Falcon,Fine tu
-000002e0: 6e69 6e67 2c47 656e 6572 6174 6976 6520  ning,Generative 
-000002f0: 4149 2c4c 4c4d 4f70 732c 4c61 7267 6520  AI,LLMOps,Large 
-00000300: 4c61 6e67 7561 6765 204d 6f64 656c 2c4c  Language Model,L
-00000310: 6c61 6d61 2032 2c4d 4c4f 7073 2c4d 6973  lama 2,MLOps,Mis
-00000320: 7472 616c 2c4d 6f64 656c 2044 6570 6c6f  tral,Model Deplo
-00000330: 796d 656e 742c 4d6f 6465 6c20 5365 7276  yment,Model Serv
-00000340: 696e 672c 5079 546f 7263 682c 5365 7276  ing,PyTorch,Serv
-00000350: 6572 6c65 7373 2c53 7461 626c 654c 4d2c  erless,StableLM,
-00000360: 5472 616e 7366 6f72 6d65 7273 2c56 6963  Transformers,Vic
-00000370: 756e 612c 764c 4c4d 0a43 6c61 7373 6966  una,vLLM.Classif
-00000380: 6965 723a 2044 6576 656c 6f70 6d65 6e74  ier: Development
-00000390: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
-000003a0: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
-000003b0: 0a43 6c61 7373 6966 6965 723a 2045 6e76  .Classifier: Env
-000003c0: 6972 6f6e 6d65 6e74 203a 3a20 4750 5520  ironment :: GPU 
-000003d0: 3a3a 204e 5649 4449 4120 4355 4441 0a43  :: NVIDIA CUDA.C
-000003e0: 6c61 7373 6966 6965 723a 2045 6e76 6972  lassifier: Envir
-000003f0: 6f6e 6d65 6e74 203a 3a20 4750 5520 3a3a  onment :: GPU ::
-00000400: 204e 5649 4449 4120 4355 4441 203a 3a20   NVIDIA CUDA :: 
-00000410: 3131 2e37 0a43 6c61 7373 6966 6965 723a  11.7.Classifier:
-00000420: 2045 6e76 6972 6f6e 6d65 6e74 203a 3a20   Environment :: 
-00000430: 4750 5520 3a3a 204e 5649 4449 4120 4355  GPU :: NVIDIA CU
-00000440: 4441 203a 3a20 3131 2e38 0a43 6c61 7373  DA :: 11.8.Class
-00000450: 6966 6965 723a 2045 6e76 6972 6f6e 6d65  ifier: Environme
-00000460: 6e74 203a 3a20 4750 5520 3a3a 204e 5649  nt :: GPU :: NVI
-00000470: 4449 4120 4355 4441 203a 3a20 3132 0a43  DIA CUDA :: 12.C
-00000480: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000490: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000004a0: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
-000004b0: 6966 6965 723a 2049 6e74 656e 6465 6420  ifier: Intended 
-000004c0: 4175 6469 656e 6365 203a 3a20 5363 6965  Audience :: Scie
-000004d0: 6e63 652f 5265 7365 6172 6368 0a43 6c61  nce/Research.Cla
-000004e0: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-000004f0: 6420 4175 6469 656e 6365 203a 3a20 5379  d Audience :: Sy
-00000500: 7374 656d 2041 646d 696e 6973 7472 6174  stem Administrat
-00000510: 6f72 730a 436c 6173 7369 6669 6572 3a20  ors.Classifier: 
-00000520: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000530: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000540: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000550: 7365 0a43 6c61 7373 6966 6965 723a 204f  se.Classifier: O
-00000560: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000570: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000580: 740a 436c 6173 7369 6669 6572 3a20 5072  t.Classifier: Pr
-00000590: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000005a0: 6765 203a 3a20 5079 7468 6f6e 0a43 6c61  ge :: Python.Cla
-000005b0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000005c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000005d0: 2050 7974 686f 6e20 3a3a 2033 0a43 6c61   Python :: 3.Cla
-000005e0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-000005f0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000600: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-00000610: 4f6e 6c79 0a43 6c61 7373 6966 6965 723a  Only.Classifier:
-00000620: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000630: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000640: 3a3a 2033 2e38 0a43 6c61 7373 6966 6965  :: 3.8.Classifie
-00000650: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000660: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000670: 6e20 3a3a 2033 2e39 0a43 6c61 7373 6966  n :: 3.9.Classif
-00000680: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000690: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000006a0: 686f 6e20 3a3a 2033 2e31 300a 436c 6173  hon :: 3.10.Clas
-000006b0: 7369 6669 6572 3a20 5072 6f67 7261 6d6d  sifier: Programm
-000006c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000006d0: 5079 7468 6f6e 203a 3a20 332e 3131 0a43  Python :: 3.11.C
-000006e0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
-000006f0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-00000700: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000710: 320a 436c 6173 7369 6669 6572 3a20 5072  2.Classifier: Pr
-00000720: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000730: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000740: 496d 706c 656d 656e 7461 7469 6f6e 203a  Implementation :
-00000750: 3a20 4350 7974 686f 6e0a 436c 6173 7369  : CPython.Classi
-00000760: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000770: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000780: 7468 6f6e 203a 3a20 496d 706c 656d 656e  thon :: Implemen
-00000790: 7461 7469 6f6e 203a 3a20 5079 5079 0a43  tation :: PyPy.C
-000007a0: 6c61 7373 6966 6965 723a 2054 6f70 6963  lassifier: Topic
-000007b0: 203a 3a20 5363 6965 6e74 6966 6963 2f45   :: Scientific/E
-000007c0: 6e67 696e 6565 7269 6e67 203a 3a20 4172  ngineering :: Ar
-000007d0: 7469 6669 6369 616c 2049 6e74 656c 6c69  tificial Intelli
-000007e0: 6765 6e63 650a 436c 6173 7369 6669 6572  gence.Classifier
-000007f0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
-00000800: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-00000810: 3a3a 204c 6962 7261 7269 6573 0a43 6c61  :: Libraries.Cla
-00000820: 7373 6966 6965 723a 2054 7970 696e 6720  ssifier: Typing 
-00000830: 3a3a 2054 7970 6564 0a52 6571 7569 7265  :: Typed.Require
-00000840: 732d 5079 7468 6f6e 3a20 3e3d 332e 380a  s-Python: >=3.8.
-00000850: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
-00000860: 6363 656c 6572 6174 650a 5265 7175 6972  ccelerate.Requir
-00000870: 6573 2d44 6973 743a 2062 656e 746f 6d6c  es-Dist: bentoml
-00000880: 5b69 6f5d 3e3d 312e 320a 5265 7175 6972  [io]>=1.2.Requir
-00000890: 6573 2d44 6973 743a 2062 6974 7361 6e64  es-Dist: bitsand
-000008a0: 6279 7465 733c 302e 3432 0a52 6571 7569  bytes<0.42.Requi
-000008b0: 7265 732d 4469 7374 3a20 6275 696c 645b  res-Dist: build[
-000008c0: 7669 7274 7561 6c65 6e76 5d3c 310a 5265  virtualenv]<1.Re
-000008d0: 7175 6972 6573 2d44 6973 743a 2063 6c69  quires-Dist: cli
-000008e0: 636b 3e3d 382e 312e 330a 5265 7175 6972  ck>=8.1.3.Requir
-000008f0: 6573 2d44 6973 743a 2063 7564 612d 7079  es-Dist: cuda-py
-00000900: 7468 6f6e 3b20 706c 6174 666f 726d 5f73  thon; platform_s
-00000910: 7973 7465 6d20 213d 2027 4461 7277 696e  ystem != 'Darwin
-00000920: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00000930: 2065 696e 6f70 730a 5265 7175 6972 6573   einops.Requires
-00000940: 2d44 6973 743a 2067 6861 7069 0a52 6571  -Dist: ghapi.Req
-00000950: 7569 7265 732d 4469 7374 3a20 6f70 656e  uires-Dist: open
-00000960: 6c6c 6d2d 636c 6965 6e74 3e3d 302e 352e  llm-client>=0.5.
-00000970: 302d 616c 7068 612e 330a 5265 7175 6972  0-alpha.3.Requir
-00000980: 6573 2d44 6973 743a 206f 7065 6e6c 6c6d  es-Dist: openllm
-00000990: 2d63 6f72 653e 3d30 2e35 2e30 2d61 6c70  -core>=0.5.0-alp
-000009a0: 6861 2e33 0a52 6571 7569 7265 732d 4469  ha.3.Requires-Di
-000009b0: 7374 3a20 6f70 7469 6d75 6d3e 3d31 2e31  st: optimum>=1.1
-000009c0: 322e 300a 5265 7175 6972 6573 2d44 6973  2.0.Requires-Dis
-000009d0: 743a 2073 6166 6574 656e 736f 7273 0a52  t: safetensors.R
-000009e0: 6571 7569 7265 732d 4469 7374 3a20 7363  equires-Dist: sc
-000009f0: 6970 790a 5265 7175 6972 6573 2d44 6973  ipy.Requires-Dis
-00000a00: 743a 2073 656e 7465 6e63 6570 6965 6365  t: sentencepiece
-00000a10: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000a20: 7472 616e 7366 6f72 6d65 7273 5b74 6f6b  transformers[tok
-00000a30: 656e 697a 6572 732c 746f 7263 685d 3e3d  enizers,torch]>=
-00000a40: 342e 3336 2e30 0a52 6571 7569 7265 732d  4.36.0.Requires-
-00000a50: 4469 7374 3a20 766c 6c6d 3e3d 302e 342e  Dist: vllm>=0.4.
-00000a60: 300a 5072 6f76 6964 6573 2d45 7874 7261  0.Provides-Extra
-00000a70: 3a20 6167 656e 7473 0a52 6571 7569 7265  : agents.Require
-00000a80: 732d 4469 7374 3a20 6469 6666 7573 6572  s-Dist: diffuser
-00000a90: 733b 2065 7874 7261 203d 3d20 2761 6765  s; extra == 'age
-00000aa0: 6e74 7327 0a52 6571 7569 7265 732d 4469  nts'.Requires-Di
-00000ab0: 7374 3a20 736f 756e 6466 696c 653b 2065  st: soundfile; e
-00000ac0: 7874 7261 203d 3d20 2761 6765 6e74 7327  xtra == 'agents'
-00000ad0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000ae0: 7472 616e 7366 6f72 6d65 7273 5b61 6765  transformers[age
-00000af0: 6e74 735d 3e3d 342e 3336 2e30 3b20 6578  nts]>=4.36.0; ex
-00000b00: 7472 6120 3d3d 2027 6167 656e 7473 270a  tra == 'agents'.
-00000b10: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00000b20: 616c 6c0a 5265 7175 6972 6573 2d44 6973  all.Requires-Dis
-00000b30: 743a 206f 7065 6e6c 6c6d 5b66 756c 6c5d  t: openllm[full]
-00000b40: 3b20 6578 7472 6120 3d3d 2027 616c 6c27  ; extra == 'all'
-00000b50: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000b60: 2061 7771 0a52 6571 7569 7265 732d 4469   awq.Requires-Di
-00000b70: 7374 3a20 6175 746f 6177 713b 2065 7874  st: autoawq; ext
-00000b80: 7261 203d 3d20 2761 7771 270a 5072 6f76  ra == 'awq'.Prov
-00000b90: 6964 6573 2d45 7874 7261 3a20 6261 6963  ides-Extra: baic
-00000ba0: 6875 616e 0a52 6571 7569 7265 732d 4469  huan.Requires-Di
-00000bb0: 7374 3a20 6370 6d2d 6b65 726e 656c 733b  st: cpm-kernels;
-00000bc0: 2065 7874 7261 203d 3d20 2762 6169 6368   extra == 'baich
-00000bd0: 7561 6e27 0a50 726f 7669 6465 732d 4578  uan'.Provides-Ex
-00000be0: 7472 613a 2063 6861 7467 6c6d 0a52 6571  tra: chatglm.Req
-00000bf0: 7569 7265 732d 4469 7374 3a20 6370 6d2d  uires-Dist: cpm-
-00000c00: 6b65 726e 656c 733b 2065 7874 7261 203d  kernels; extra =
-00000c10: 3d20 2763 6861 7467 6c6d 270a 5072 6f76  = 'chatglm'.Prov
-00000c20: 6964 6573 2d45 7874 7261 3a20 6462 7278  ides-Extra: dbrx
-00000c30: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000c40: 6370 6d2d 6b65 726e 656c 733b 2065 7874  cpm-kernels; ext
-00000c50: 7261 203d 3d20 2764 6272 7827 0a50 726f  ra == 'dbrx'.Pro
-00000c60: 7669 6465 732d 4578 7472 613a 2064 6f6c  vides-Extra: dol
-00000c70: 6c79 2d76 320a 5265 7175 6972 6573 2d44  ly-v2.Requires-D
-00000c80: 6973 743a 2063 706d 2d6b 6572 6e65 6c73  ist: cpm-kernels
-00000c90: 3b20 6578 7472 6120 3d3d 2027 646f 6c6c  ; extra == 'doll
-00000ca0: 792d 7632 270a 5072 6f76 6964 6573 2d45  y-v2'.Provides-E
-00000cb0: 7874 7261 3a20 6661 6c63 6f6e 0a52 6571  xtra: falcon.Req
-00000cc0: 7569 7265 732d 4469 7374 3a20 7866 6f72  uires-Dist: xfor
-00000cd0: 6d65 7273 3b20 6578 7472 6120 3d3d 2027  mers; extra == '
-00000ce0: 6661 6c63 6f6e 270a 5072 6f76 6964 6573  falcon'.Provides
-00000cf0: 2d45 7874 7261 3a20 6669 6e65 2d74 756e  -Extra: fine-tun
-00000d00: 650a 5265 7175 6972 6573 2d44 6973 743a  e.Requires-Dist:
-00000d10: 2064 6174 6173 6574 733b 2065 7874 7261   datasets; extra
-00000d20: 203d 3d20 2766 696e 652d 7475 6e65 270a   == 'fine-tune'.
-00000d30: 5265 7175 6972 6573 2d44 6973 743a 2068  Requires-Dist: h
-00000d40: 7567 6769 6e67 6661 6365 2d68 7562 3b20  uggingface-hub; 
-00000d50: 6578 7472 6120 3d3d 2027 6669 6e65 2d74  extra == 'fine-t
-00000d60: 756e 6527 0a52 6571 7569 7265 732d 4469  une'.Requires-Di
-00000d70: 7374 3a20 7065 6674 3e3d 302e 362e 303b  st: peft>=0.6.0;
-00000d80: 2065 7874 7261 203d 3d20 2766 696e 652d   extra == 'fine-
-00000d90: 7475 6e65 270a 5265 7175 6972 6573 2d44  tune'.Requires-D
-00000da0: 6973 743a 2074 726c 3b20 6578 7472 6120  ist: trl; extra 
-00000db0: 3d3d 2027 6669 6e65 2d74 756e 6527 0a50  == 'fine-tune'.P
-00000dc0: 726f 7669 6465 732d 4578 7472 613a 2066  rovides-Extra: f
-00000dd0: 6c61 6e2d 7435 0a52 6571 7569 7265 732d  lan-t5.Requires-
-00000de0: 4469 7374 3a20 7866 6f72 6d65 7273 3b20  Dist: xformers; 
-00000df0: 6578 7472 6120 3d3d 2027 666c 616e 2d74  extra == 'flan-t
-00000e00: 3527 0a50 726f 7669 6465 732d 4578 7472  5'.Provides-Extr
-00000e10: 613a 2066 756c 6c0a 5265 7175 6972 6573  a: full.Requires
-00000e20: 2d44 6973 743a 206f 7065 6e6c 6c6d 5b61  -Dist: openllm[a
-00000e30: 6765 6e74 732c 6177 712c 6261 6963 6875  gents,awq,baichu
-00000e40: 616e 2c63 6861 7467 6c6d 2c64 6272 782c  an,chatglm,dbrx,
-00000e50: 646f 6c6c 792d 7632 2c66 616c 636f 6e2c  dolly-v2,falcon,
-00000e60: 6669 6e65 2d74 756e 652c 666c 616e 2d74  fine-tune,flan-t
-00000e70: 352c 6765 6d6d 612c 6767 6d6c 2c67 7074  5,gemma,ggml,gpt
-00000e80: 2d6e 656f 782c 6770 7471 2c67 7270 632c  -neox,gptq,grpc,
-00000e90: 6c6c 616d 612c 6d69 7374 7261 6c2c 6d69  llama,mistral,mi
-00000ea0: 7874 7261 6c2c 6d70 742c 6f70 656e 6169  xtral,mpt,openai
-00000eb0: 2c6f 7074 2c70 6869 2c70 6c61 7967 726f  ,opt,phi,playgro
-00000ec0: 756e 642c 7177 656e 2c73 7461 626c 656c  und,qwen,stablel
-00000ed0: 6d2c 7374 6172 636f 6465 722c 766c 6c6d  m,starcoder,vllm
-00000ee0: 2c79 695d 3b20 6578 7472 6120 3d3d 2027  ,yi]; extra == '
-00000ef0: 6675 6c6c 270a 5072 6f76 6964 6573 2d45  full'.Provides-E
-00000f00: 7874 7261 3a20 6765 6d6d 610a 5265 7175  xtra: gemma.Requ
-00000f10: 6972 6573 2d44 6973 743a 2078 666f 726d  ires-Dist: xform
-00000f20: 6572 733b 2065 7874 7261 203d 3d20 2767  ers; extra == 'g
-00000f30: 656d 6d61 270a 5072 6f76 6964 6573 2d45  emma'.Provides-E
-00000f40: 7874 7261 3a20 6767 6d6c 0a52 6571 7569  xtra: ggml.Requi
-00000f50: 7265 732d 4469 7374 3a20 6374 7261 6e73  res-Dist: ctrans
-00000f60: 666f 726d 6572 733b 2065 7874 7261 203d  formers; extra =
-00000f70: 3d20 2767 676d 6c27 0a50 726f 7669 6465  = 'ggml'.Provide
-00000f80: 732d 4578 7472 613a 2067 7074 2d6e 656f  s-Extra: gpt-neo
-00000f90: 780a 5265 7175 6972 6573 2d44 6973 743a  x.Requires-Dist:
-00000fa0: 2078 666f 726d 6572 733b 2065 7874 7261   xformers; extra
-00000fb0: 203d 3d20 2767 7074 2d6e 656f 7827 0a50   == 'gpt-neox'.P
-00000fc0: 726f 7669 6465 732d 4578 7472 613a 2067  rovides-Extra: g
-00000fd0: 7074 710a 5265 7175 6972 6573 2d44 6973  ptq.Requires-Dis
-00000fe0: 743a 2061 7574 6f2d 6770 7471 5b74 7269  t: auto-gptq[tri
-00000ff0: 746f 6e5d 3e3d 302e 342e 323b 2065 7874  ton]>=0.4.2; ext
-00001000: 7261 203d 3d20 2767 7074 7127 0a50 726f  ra == 'gptq'.Pro
-00001010: 7669 6465 732d 4578 7472 613a 2067 7270  vides-Extra: grp
-00001020: 630a 5265 7175 6972 6573 2d44 6973 743a  c.Requires-Dist:
-00001030: 2062 656e 746f 6d6c 5b67 7270 635d 3e3d   bentoml[grpc]>=
-00001040: 312e 323b 2065 7874 7261 203d 3d20 2767  1.2; extra == 'g
-00001050: 7270 6327 0a50 726f 7669 6465 732d 4578  rpc'.Provides-Ex
-00001060: 7472 613a 206c 6c61 6d61 0a52 6571 7569  tra: llama.Requi
-00001070: 7265 732d 4469 7374 3a20 7866 6f72 6d65  res-Dist: xforme
-00001080: 7273 3b20 6578 7472 6120 3d3d 2027 6c6c  rs; extra == 'll
-00001090: 616d 6127 0a50 726f 7669 6465 732d 4578  ama'.Provides-Ex
-000010a0: 7472 613a 206d 6973 7472 616c 0a52 6571  tra: mistral.Req
-000010b0: 7569 7265 732d 4469 7374 3a20 7866 6f72  uires-Dist: xfor
-000010c0: 6d65 7273 3b20 6578 7472 6120 3d3d 2027  mers; extra == '
-000010d0: 6d69 7374 7261 6c27 0a50 726f 7669 6465  mistral'.Provide
-000010e0: 732d 4578 7472 613a 206d 6978 7472 616c  s-Extra: mixtral
-000010f0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00001100: 7866 6f72 6d65 7273 3b20 6578 7472 6120  xformers; extra 
-00001110: 3d3d 2027 6d69 7874 7261 6c27 0a50 726f  == 'mixtral'.Pro
-00001120: 7669 6465 732d 4578 7472 613a 206d 7074  vides-Extra: mpt
-00001130: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00001140: 7472 6974 6f6e 3b20 6578 7472 6120 3d3d  triton; extra ==
-00001150: 2027 6d70 7427 0a50 726f 7669 6465 732d   'mpt'.Provides-
-00001160: 4578 7472 613a 206f 7065 6e61 690a 5265  Extra: openai.Re
-00001170: 7175 6972 6573 2d44 6973 743a 2066 6173  quires-Dist: fas
-00001180: 7461 7069 3b20 6578 7472 6120 3d3d 2027  tapi; extra == '
-00001190: 6f70 656e 6169 270a 5265 7175 6972 6573  openai'.Requires
-000011a0: 2d44 6973 743a 206f 7065 6e61 695b 6461  -Dist: openai[da
-000011b0: 7461 6c69 625d 3e3d 313b 2065 7874 7261  talib]>=1; extra
-000011c0: 203d 3d20 276f 7065 6e61 6927 0a52 6571   == 'openai'.Req
-000011d0: 7569 7265 732d 4469 7374 3a20 7469 6b74  uires-Dist: tikt
-000011e0: 6f6b 656e 3b20 6578 7472 6120 3d3d 2027  oken; extra == '
-000011f0: 6f70 656e 6169 270a 5072 6f76 6964 6573  openai'.Provides
-00001200: 2d45 7874 7261 3a20 6f70 740a 5265 7175  -Extra: opt.Requ
-00001210: 6972 6573 2d44 6973 743a 2074 7269 746f  ires-Dist: trito
-00001220: 6e3b 2065 7874 7261 203d 3d20 276f 7074  n; extra == 'opt
-00001230: 270a 5072 6f76 6964 6573 2d45 7874 7261  '.Provides-Extra
-00001240: 3a20 7068 690a 5265 7175 6972 6573 2d44  : phi.Requires-D
-00001250: 6973 743a 2074 7269 746f 6e3b 2065 7874  ist: triton; ext
-00001260: 7261 203d 3d20 2770 6869 270a 5072 6f76  ra == 'phi'.Prov
-00001270: 6964 6573 2d45 7874 7261 3a20 706c 6179  ides-Extra: play
-00001280: 6772 6f75 6e64 0a52 6571 7569 7265 732d  ground.Requires-
-00001290: 4469 7374 3a20 6970 7974 686f 6e3b 2065  Dist: ipython; e
-000012a0: 7874 7261 203d 3d20 2770 6c61 7967 726f  xtra == 'playgro
-000012b0: 756e 6427 0a52 6571 7569 7265 732d 4469  und'.Requires-Di
-000012c0: 7374 3a20 6a75 7079 7465 723b 2065 7874  st: jupyter; ext
-000012d0: 7261 203d 3d20 2770 6c61 7967 726f 756e  ra == 'playgroun
-000012e0: 6427 0a52 6571 7569 7265 732d 4469 7374  d'.Requires-Dist
-000012f0: 3a20 6a75 7079 7465 7874 3b20 6578 7472  : jupytext; extr
-00001300: 6120 3d3d 2027 706c 6179 6772 6f75 6e64  a == 'playground
-00001310: 270a 5265 7175 6972 6573 2d44 6973 743a  '.Requires-Dist:
-00001320: 206e 6266 6f72 6d61 743b 2065 7874 7261   nbformat; extra
-00001330: 203d 3d20 2770 6c61 7967 726f 756e 6427   == 'playground'
-00001340: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00001350: 6e6f 7465 626f 6f6b 3b20 6578 7472 6120  notebook; extra 
-00001360: 3d3d 2027 706c 6179 6772 6f75 6e64 270a  == 'playground'.
-00001370: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00001380: 7177 656e 0a52 6571 7569 7265 732d 4469  qwen.Requires-Di
-00001390: 7374 3a20 6370 6d2d 6b65 726e 656c 733b  st: cpm-kernels;
-000013a0: 2065 7874 7261 203d 3d20 2771 7765 6e27   extra == 'qwen'
-000013b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000013c0: 7469 6b74 6f6b 656e 3b20 6578 7472 6120  tiktoken; extra 
-000013d0: 3d3d 2027 7177 656e 270a 5072 6f76 6964  == 'qwen'.Provid
-000013e0: 6573 2d45 7874 7261 3a20 7374 6162 6c65  es-Extra: stable
-000013f0: 6c6d 0a52 6571 7569 7265 732d 4469 7374  lm.Requires-Dist
-00001400: 3a20 6370 6d2d 6b65 726e 656c 733b 2065  : cpm-kernels; e
-00001410: 7874 7261 203d 3d20 2773 7461 626c 656c  xtra == 'stablel
-00001420: 6d27 0a52 6571 7569 7265 732d 4469 7374  m'.Requires-Dist
-00001430: 3a20 7469 6b74 6f6b 656e 3b20 6578 7472  : tiktoken; extr
-00001440: 6120 3d3d 2027 7374 6162 6c65 6c6d 270a  a == 'stablelm'.
-00001450: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00001460: 7374 6172 636f 6465 720a 5265 7175 6972  starcoder.Requir
-00001470: 6573 2d44 6973 743a 2062 6974 7361 6e64  es-Dist: bitsand
-00001480: 6279 7465 733b 2065 7874 7261 203d 3d20  bytes; extra == 
-00001490: 2773 7461 7263 6f64 6572 270a 5072 6f76  'starcoder'.Prov
-000014a0: 6964 6573 2d45 7874 7261 3a20 766c 6c6d  ides-Extra: vllm
-000014b0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-000014c0: 766c 6c6d 3d3d 302e 342e 303b 2065 7874  vllm==0.4.0; ext
-000014d0: 7261 203d 3d20 2776 6c6c 6d27 0a50 726f  ra == 'vllm'.Pro
-000014e0: 7669 6465 732d 4578 7472 613a 2079 690a  vides-Extra: yi.
-000014f0: 5265 7175 6972 6573 2d44 6973 743a 2062  Requires-Dist: b
-00001500: 6974 7361 6e64 6279 7465 733b 2065 7874  itsandbytes; ext
-00001510: 7261 203d 3d20 2779 6927 0a44 6573 6372  ra == 'yi'.Descr
-00001520: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00001530: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00001540: 776e 0a0a 3c70 2061 6c69 676e 3d22 6365  wn..<p align="ce
-00001550: 6e74 6572 223e 0a20 203c 6120 6872 6566  nter">.  <a href
-00001560: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00001570: 2e63 6f6d 2f62 656e 746f 6d6c 2f6f 7065  .com/bentoml/ope
-00001580: 6e6c 6c6d 223e 0a20 2020 203c 696d 6720  nllm">.    <img 
-00001590: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-000015a0: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-000015b0: 6e74 2e63 6f6d 2f62 656e 746f 6d6c 2f6f  nt.com/bentoml/o
-000015c0: 7065 6e6c 6c6d 2f6d 6169 6e2f 2e67 6974  penllm/main/.git
-000015d0: 6875 622f 6173 7365 7473 2f6d 6169 6e2d  hub/assets/main-
-000015e0: 6261 6e6e 6572 2e70 6e67 2220 616c 743d  banner.png" alt=
-000015f0: 2242 616e 6e65 7220 666f 7220 4f70 656e  "Banner for Open
-00001600: 4c4c 4d22 202f 3e0a 2020 3c2f 613e 0a3c  LLM" />.  </a>.<
-00001610: 2f70 3e0a 0a0a 3c64 6976 2061 6c69 676e  /p>...<div align
-00001620: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
-00001630: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
-00001640: 223e f09f a6be 204f 7065 6e4c 4c4d 3c2f  ">.... OpenLLM</
-00001650: 6831 3e0a 2020 2020 3c61 2068 7265 663d  h1>.    <a href=
-00001660: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-00001670: 672f 7072 6f6a 6563 742f 6f70 656e 6c6c  g/project/openll
-00001680: 6d22 3e0a 2020 2020 2020 2020 3c69 6d67  m">.        <img
-00001690: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000016a0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000016b0: 692f 762f 6f70 656e 6c6c 6d2e 7376 673f  i/v/openllm.svg?
-000016c0: 6c6f 676f 3d70 7970 6926 6c61 6265 6c3d  logo=pypi&label=
-000016d0: 5079 5049 266c 6f67 6f43 6f6c 6f72 3d67  PyPI&logoColor=g
-000016e0: 6f6c 6422 2061 6c74 3d22 7079 7069 5f73  old" alt="pypi_s
-000016f0: 7461 7475 7322 202f 3e0a 2020 2020 3c2f  tatus" />.    </
-00001700: 613e 3c61 2068 7265 663d 2268 7474 7073  a><a href="https
-00001710: 3a2f 2f74 6573 742e 7079 7069 2e6f 7267  ://test.pypi.org
-00001720: 2f70 726f 6a65 6374 2f6f 7065 6e6c 6c6d  /project/openllm
-00001730: 2f22 3e0a 2020 2020 2020 2020 3c69 6d67  /">.        <img
-00001740: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00001750: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00001760: 6765 2f4e 6967 6874 6c79 2d50 7950 493f  ge/Nightly-PyPI?
-00001770: 6c6f 676f 3d70 7970 6926 6c61 6265 6c3d  logo=pypi&label=
-00001780: 5079 5049 2663 6f6c 6f72 3d67 7261 7926  PyPI&color=gray&
-00001790: 6c69 6e6b 3d68 7474 7073 2533 4125 3246  link=https%3A%2F
-000017a0: 2532 4674 6573 742e 7079 7069 2e6f 7267  %2Ftest.pypi.org
-000017b0: 2532 4670 726f 6a65 6374 2532 466f 7065  %2Fproject%2Fope
-000017c0: 6e6c 6c6d 2532 4622 2061 6c74 3d22 7465  nllm%2F" alt="te
-000017d0: 7374 5f70 7970 695f 7374 6174 7573 2220  st_pypi_status" 
-000017e0: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-000017f0: 6566 3d22 6874 7470 733a 2f2f 7477 6974  ef="https://twit
-00001800: 7465 722e 636f 6d2f 6265 6e74 6f6d 6c61  ter.com/bentomla
-00001810: 6922 3e0a 2020 2020 2020 2020 3c69 6d67  i">.        <img
-00001820: 2073 7263 3d22 6874 7470 733a 2f2f 6261   src="https://ba
-00001830: 6467 656e 2e6e 6574 2f62 6164 6765 2f69  dgen.net/badge/i
-00001840: 636f 6e2f 4062 656e 746f 6d6c 6169 2f31  con/@bentomlai/1
-00001850: 4441 3146 323f 6963 6f6e 3d74 7769 7474  DA1F2?icon=twitt
-00001860: 6572 266c 6162 656c 3d46 6f6c 6c6f 7725  er&label=Follow%
-00001870: 3230 5573 2220 616c 743d 2254 7769 7474  20Us" alt="Twitt
-00001880: 6572 2220 2f3e 0a20 2020 203c 2f61 3e3c  er" />.    </a><
-00001890: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-000018a0: 6c2e 6265 6e74 6f6d 6c2e 636f 6d2f 6a6f  l.bentoml.com/jo
-000018b0: 696e 2d6f 7065 6e6c 6c6d 2d64 6973 636f  in-openllm-disco
-000018c0: 7264 223e 0a20 2020 2020 2020 203c 696d  rd">.        <im
-000018d0: 6720 7372 633d 2268 7474 7073 3a2f 2f62  g src="https://b
-000018e0: 6164 6765 6e2e 6e65 742f 6261 6467 652f  adgen.net/badge/
-000018f0: 6963 6f6e 2f4f 7065 6e4c 4c4d 2f37 3238  icon/OpenLLM/728
-00001900: 3964 613f 6963 6f6e 3d64 6973 636f 7264  9da?icon=discord
-00001910: 266c 6162 656c 3d4a 6f69 6e25 3230 5573  &label=Join%20Us
-00001920: 2220 616c 743d 2244 6973 636f 7264 2220  " alt="Discord" 
-00001930: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-00001940: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00001950: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-00001960: 7065 6e4c 4c4d 2f61 6374 696f 6e73 2f77  penLLM/actions/w
-00001970: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c22  orkflows/ci.yml"
-00001980: 3e0a 2020 2020 2020 2020 3c69 6d67 2073  >.        <img s
-00001990: 7263 3d22 6874 7470 733a 2f2f 6769 7468  rc="https://gith
-000019a0: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-000019b0: 7065 6e4c 4c4d 2f61 6374 696f 6e73 2f77  penLLM/actions/w
-000019c0: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c2f  orkflows/ci.yml/
-000019d0: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-000019e0: 3d6d 6169 6e22 2061 6c74 3d22 6369 2220  =main" alt="ci" 
-000019f0: 2f3e 0a20 2020 203c 2f61 3e3c 6120 6872  />.    </a><a hr
-00001a00: 6566 3d22 6874 7470 733a 2f2f 7265 7375  ef="https://resu
-00001a10: 6c74 732e 7072 652d 636f 6d6d 6974 2e63  lts.pre-commit.c
-00001a20: 692f 6c61 7465 7374 2f67 6974 6875 622f  i/latest/github/
-00001a30: 6265 6e74 6f6d 6c2f 4f70 656e 4c4c 4d2f  bentoml/OpenLLM/
-00001a40: 6d61 696e 223e 0a20 2020 2020 2020 203c  main">.        <
-00001a50: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00001a60: 2f72 6573 756c 7473 2e70 7265 2d63 6f6d  /results.pre-com
-00001a70: 6d69 742e 6369 2f62 6164 6765 2f67 6974  mit.ci/badge/git
-00001a80: 6875 622f 6265 6e74 6f6d 6c2f 4f70 656e  hub/bentoml/Open
-00001a90: 4c4c 4d2f 6d61 696e 2e73 7667 2220 616c  LLM/main.svg" al
-00001aa0: 743d 2270 7265 2d63 6f6d 6d69 742e 6369  t="pre-commit.ci
-00001ab0: 2073 7461 7475 7322 202f 3e0a 2020 2020   status" />.    
-00001ac0: 3c2f 613e 3c62 723e 0a20 2020 203c 6120  </a><br>.    <a 
-00001ad0: 6872 6566 3d22 6874 7470 733a 2f2f 7079  href="https://py
-00001ae0: 7069 2e6f 7267 2f70 726f 6a65 6374 2f6f  pi.org/project/o
-00001af0: 7065 6e6c 6c6d 223e 0a20 2020 2020 2020  penllm">.       
-00001b00: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00001b10: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00001b20: 6f2f 7079 7069 2f70 7976 6572 7369 6f6e  o/pypi/pyversion
-00001b30: 732f 6f70 656e 6c6c 6d2e 7376 673f 6c6f  s/openllm.svg?lo
-00001b40: 676f 3d70 7974 686f 6e26 6c61 6265 6c3d  go=python&label=
-00001b50: 5079 7468 6f6e 266c 6f67 6f43 6f6c 6f72  Python&logoColor
-00001b60: 3d67 6f6c 6422 2061 6c74 3d22 7079 7468  =gold" alt="pyth
-00001b70: 6f6e 5f76 6572 7369 6f6e 2220 2f3e 0a20  on_version" />. 
-00001b80: 2020 203c 2f61 3e3c 6120 6872 6566 3d22     </a><a href="
-00001b90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001ba0: 6f6d 2f70 7970 612f 6861 7463 6822 3e0a  om/pypa/hatch">.
-00001bb0: 2020 2020 2020 2020 3c69 6d67 2073 7263          <img src
-00001bc0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00001bd0: 6965 6c64 732e 696f 2f62 6164 6765 2f25  ields.io/badge/%
-00001be0: 4630 2539 4625 4135 2539 412d 4861 7463  F0%9F%A5%9A-Hatc
-00001bf0: 682d 3430 3531 6235 2e73 7667 2220 616c  h-4051b5.svg" al
-00001c00: 743d 2248 6174 6368 2220 2f3e 0a20 2020  t="Hatch" />.   
-00001c10: 203c 2f61 3e3c 6120 6872 6566 3d22 6874   </a><a href="ht
-00001c20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001c30: 2f62 656e 746f 6d6c 2f4f 7065 6e4c 4c4d  /bentoml/OpenLLM
-00001c40: 2f62 6c6f 622f 6d61 696e 2f53 5459 4c45  /blob/main/STYLE
-00001c50: 2e6d 6422 3e0a 2020 2020 2020 2020 3c69  .md">.        <i
-00001c60: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001c70: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00001c80: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
-00001c90: 652d 476f 6f67 6c65 2d30 3030 3030 302e  e-Google-000000.
-00001ca0: 7376 6722 2061 6c74 3d22 636f 6465 2073  svg" alt="code s
-00001cb0: 7479 6c65 2220 2f3e 0a20 2020 203c 2f61  tyle" />.    </a
-00001cc0: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001cd0: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7374  //github.com/ast
-00001ce0: 7261 6c2d 7368 2f72 7566 6622 3e0a 2020  ral-sh/ruff">.  
-00001cf0: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
-00001d00: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00001d10: 6c64 732e 696f 2f65 6e64 706f 696e 743f  lds.io/endpoint?
-00001d20: 7572 6c3d 6874 7470 733a 2f2f 7261 772e  url=https://raw.
-00001d30: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00001d40: 742e 636f 6d2f 6368 6172 6c69 6572 6d61  t.com/charlierma
-00001d50: 7273 682f 7275 6666 2f6d 6169 6e2f 6173  rsh/ruff/main/as
-00001d60: 7365 7473 2f62 6164 6765 2f76 322e 6a73  sets/badge/v2.js
-00001d70: 6f6e 2220 616c 743d 2252 7566 6622 202f  on" alt="Ruff" /
-00001d80: 3e0a 2020 2020 3c2f 613e 3c61 2068 7265  >.    </a><a hre
-00001d90: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00001da0: 622e 636f 6d2f 7079 7468 6f6e 2f6d 7970  b.com/python/myp
-00001db0: 7922 3e0a 2020 2020 2020 2020 3c69 6d67  y">.        <img
-00001dc0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00001dd0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00001de0: 6765 2f74 7970 6573 2d6d 7970 792d 626c  ge/types-mypy-bl
-00001df0: 7565 2e73 7667 2220 616c 743d 2274 7970  ue.svg" alt="typ
-00001e00: 6573 202d 206d 7970 7922 202f 3e0a 2020  es - mypy" />.  
-00001e10: 2020 3c2f 613e 3c61 2068 7265 663d 2268    </a><a href="h
-00001e20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001e30: 6d2f 6d69 6372 6f73 6f66 742f 7079 7269  m/microsoft/pyri
-00001e40: 6768 7422 3e0a 2020 2020 2020 2020 3c69  ght">.        <i
-00001e50: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00001e60: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00001e70: 6164 6765 2f74 7970 6573 2d70 7972 6967  adge/types-pyrig
-00001e80: 6874 2d79 656c 6c6f 772e 7376 6722 2061  ht-yellow.svg" a
-00001e90: 6c74 3d22 7479 7065 7320 2d20 7079 7269  lt="types - pyri
-00001ea0: 6768 7422 202f 3e0a 2020 2020 3c2f 613e  ght" />.    </a>
-00001eb0: 3c62 723e 0a20 2020 203c 703e 416e 206f  <br>.    <p>An o
-00001ec0: 7065 6e20 706c 6174 666f 726d 2066 6f72  pen platform for
-00001ed0: 206f 7065 7261 7469 6e67 206c 6172 6765   operating large
-00001ee0: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00001ef0: 2028 4c4c 4d73 2920 696e 2070 726f 6475   (LLMs) in produ
-00001f00: 6374 696f 6e2e 3c2f 6272 3e0a 2020 2020  ction.</br>.    
-00001f10: 4669 6e65 2d74 756e 652c 2073 6572 7665  Fine-tune, serve
-00001f20: 2c20 6465 706c 6f79 2c20 616e 6420 6d6f  , deploy, and mo
-00001f30: 6e69 746f 7220 616e 7920 4c4c 4d73 2077  nitor any LLMs w
-00001f40: 6974 6820 6561 7365 2e3c 2f70 3e0a 2020  ith ease.</p>.  
-00001f50: 2020 3c69 3e3c 2f69 3e0a 3c2f 6469 763e    <i></i>.</div>
-00001f60: 0a0a 2323 20f0 9f93 9620 496e 7472 6f64  ..## .... Introd
-00001f70: 7563 7469 6f6e 0a0a 4f70 656e 4c4c 4d20  uction..OpenLLM 
-00001f80: 6973 2061 6e20 6f70 656e 2d73 6f75 7263  is an open-sourc
-00001f90: 6520 706c 6174 666f 726d 2064 6573 6967  e platform desig
-00001fa0: 6e65 6420 746f 2066 6163 696c 6974 6174  ned to facilitat
-00001fb0: 6520 7468 6520 6465 706c 6f79 6d65 6e74  e the deployment
-00001fc0: 2061 6e64 206f 7065 7261 7469 6f6e 206f   and operation o
-00001fd0: 6620 6c61 7267 6520 6c61 6e67 7561 6765  f large language
-00001fe0: 206d 6f64 656c 7320 284c 4c4d 7329 2069   models (LLMs) i
-00001ff0: 6e20 7265 616c 2d77 6f72 6c64 2061 7070  n real-world app
-00002000: 6c69 6361 7469 6f6e 732e 2057 6974 6820  lications. With 
-00002010: 4f70 656e 4c4c 4d2c 2079 6f75 2063 616e  OpenLLM, you can
-00002020: 2072 756e 2069 6e66 6572 656e 6365 206f   run inference o
-00002030: 6e20 616e 7920 6f70 656e 2d73 6f75 7263  n any open-sourc
-00002040: 6520 4c4c 4d2c 2064 6570 6c6f 7920 7468  e LLM, deploy th
-00002050: 656d 206f 6e20 7468 6520 636c 6f75 6420  em on the cloud 
-00002060: 6f72 206f 6e2d 7072 656d 6973 6573 2c20  or on-premises, 
-00002070: 616e 6420 6275 696c 6420 706f 7765 7266  and build powerf
-00002080: 756c 2041 4920 6170 706c 6963 6174 696f  ul AI applicatio
-00002090: 6e73 2e0a 0a4b 6579 2066 6561 7475 7265  ns...Key feature
-000020a0: 7320 696e 636c 7564 653a 0a0a f09f 9a82  s include:......
-000020b0: 202a 2a53 7461 7465 2d6f 662d 7468 652d   **State-of-the-
-000020c0: 6172 7420 4c4c 4d73 2a2a 3a20 496e 7465  art LLMs**: Inte
-000020d0: 6772 6174 6564 2073 7570 706f 7274 2066  grated support f
-000020e0: 6f72 2061 2077 6964 6520 7261 6e67 6520  or a wide range 
-000020f0: 6f66 206f 7065 6e2d 736f 7572 6365 204c  of open-source L
-00002100: 4c4d 7320 616e 6420 6d6f 6465 6c20 7275  LMs and model ru
-00002110: 6e74 696d 6573 2c20 696e 636c 7564 696e  ntimes, includin
-00002120: 6720 6275 7420 6e6f 7420 6c69 6d69 7465  g but not limite
-00002130: 6420 746f 204c 6c61 6d61 2032 2c20 5374  d to Llama 2, St
-00002140: 6162 6c65 4c4d 2c20 4661 6c63 6f6e 2c20  ableLM, Falcon, 
-00002150: 446f 6c6c 792c 2046 6c61 6e2d 5435 2c20  Dolly, Flan-T5, 
-00002160: 4368 6174 474c 4d2c 2061 6e64 2053 7461  ChatGLM, and Sta
-00002170: 7243 6f64 6572 2e0a 0af0 9f94 a520 2a2a  rCoder....... **
-00002180: 466c 6578 6962 6c65 2041 5049 732a 2a3a  Flexible APIs**:
-00002190: 2053 6572 7665 204c 4c4d 7320 6f76 6572   Serve LLMs over
-000021a0: 2061 2052 4553 5466 756c 2041 5049 206f   a RESTful API o
-000021b0: 7220 6752 5043 2077 6974 6820 6120 7369  r gRPC with a si
-000021c0: 6e67 6c65 2063 6f6d 6d61 6e64 2e20 596f  ngle command. Yo
-000021d0: 7520 6361 6e20 696e 7465 7261 6374 2077  u can interact w
-000021e0: 6974 6820 7468 6520 6d6f 6465 6c20 7573  ith the model us
-000021f0: 696e 6720 6120 5765 6220 5549 2c20 434c  ing a Web UI, CL
-00002200: 492c 2050 7974 686f 6e2f 4a61 7661 5363  I, Python/JavaSc
-00002210: 7269 7074 2063 6c69 656e 7473 2c20 6f72  ript clients, or
-00002220: 2061 6e79 2048 5454 5020 636c 6965 6e74   any HTTP client
-00002230: 206f 6620 796f 7572 2063 686f 6963 652e   of your choice.
-00002240: 0a0a e29b 93ef b88f 202a 2a46 7265 6564  ........ **Freed
-00002250: 6f6d 2074 6f20 6275 696c 642a 2a3a 2046  om to build**: F
-00002260: 6972 7374 2d63 6c61 7373 2073 7570 706f  irst-class suppo
-00002270: 7274 2066 6f72 204c 616e 6743 6861 696e  rt for LangChain
-00002280: 2c20 4265 6e74 6f4d 4c2c 204c 6c61 6d61  , BentoML, Llama
-00002290: 496e 6465 782c 204f 7065 6e41 4920 656e  Index, OpenAI en
-000022a0: 6470 6f69 6e74 732c 2061 6e64 2048 7567  dpoints, and Hug
-000022b0: 6769 6e67 2046 6163 652c 2061 6c6c 6f77  ging Face, allow
-000022c0: 696e 6720 796f 7520 746f 2065 6173 696c  ing you to easil
-000022d0: 7920 6372 6561 7465 2079 6f75 7220 6f77  y create your ow
-000022e0: 6e20 4149 2061 7070 6c69 6361 7469 6f6e  n AI application
-000022f0: 7320 6279 2063 6f6d 706f 7369 6e67 204c  s by composing L
-00002300: 4c4d 7320 7769 7468 206f 7468 6572 206d  LMs with other m
-00002310: 6f64 656c 7320 616e 6420 7365 7276 6963  odels and servic
-00002320: 6573 2e0a 0af0 9f8e af20 2a2a 5374 7265  es....... **Stre
-00002330: 616d 6c69 6e65 2064 6570 6c6f 796d 656e  amline deploymen
-00002340: 742a 2a3a 2041 7574 6f6d 6174 6963 616c  t**: Automatical
-00002350: 6c79 2067 656e 6572 6174 6520 796f 7572  ly generate your
-00002360: 204c 4c4d 2073 6572 7665 7220 446f 636b   LLM server Dock
-00002370: 6572 2069 6d61 6765 7320 6f72 2064 6570  er images or dep
-00002380: 6c6f 7920 6173 2073 6572 7665 726c 6573  loy as serverles
-00002390: 7320 656e 6470 6f69 6e74 7320 7669 610a  s endpoints via.
-000023a0: 5be2 9881 efb8 8f20 4265 6e74 6f43 6c6f  [...... BentoClo
-000023b0: 7564 5d28 6874 7470 733a 2f2f 6c2e 6265  ud](https://l.be
-000023c0: 6e74 6f6d 6c2e 636f 6d2f 6265 6e74 6f2d  ntoml.com/bento-
-000023d0: 636c 6f75 6429 2c20 7768 6963 6820 6566  cloud), which ef
-000023e0: 666f 7274 6c65 7373 6c79 206d 616e 6167  fortlessly manag
-000023f0: 6573 2047 5055 2072 6573 6f75 7263 6573  es GPU resources
-00002400: 2c20 7363 616c 6573 2061 6363 6f72 6469  , scales accordi
-00002410: 6e67 2074 6f20 7472 6166 6669 632c 2061  ng to traffic, a
-00002420: 6e64 2065 6e73 7572 6573 2063 6f73 742d  nd ensures cost-
-00002430: 6566 6665 6374 6976 656e 6573 732e 0a0a  effectiveness...
-00002440: f09f a496 efb8 8f20 2a2a 4272 696e 6720  ....... **Bring 
-00002450: 796f 7572 206f 776e 204c 4c4d 2a2a 3a20  your own LLM**: 
-00002460: 4669 6e65 2d74 756e 6520 616e 7920 4c4c  Fine-tune any LL
-00002470: 4d20 746f 2073 7569 7420 796f 7572 206e  M to suit your n
-00002480: 6565 6473 2e20 596f 7520 6361 6e20 6c6f  eeds. You can lo
-00002490: 6164 204c 6f52 4120 6c61 7965 7273 2074  ad LoRA layers t
-000024a0: 6f20 6669 6e65 2d74 756e 6520 6d6f 6465  o fine-tune mode
-000024b0: 6c73 2066 6f72 2068 6967 6865 7220 6163  ls for higher ac
-000024c0: 6375 7261 6379 2061 6e64 2070 6572 666f  curacy and perfo
-000024d0: 726d 616e 6365 2066 6f72 2073 7065 6369  rmance for speci
-000024e0: 6669 6320 7461 736b 732e 2041 2075 6e69  fic tasks. A uni
-000024f0: 6669 6564 2066 696e 652d 7475 6e69 6e67  fied fine-tuning
-00002500: 2041 5049 2066 6f72 206d 6f64 656c 7320   API for models 
-00002510: 2860 4c4c 4d2e 7475 6e69 6e67 2829 6029  (`LLM.tuning()`)
-00002520: 2069 7320 636f 6d69 6e67 2073 6f6f 6e2e   is coming soon.
-00002530: 0a0a e29a a1c2 a02a 2a51 7561 6e74 697a  .......**Quantiz
-00002540: 6174 696f 6e2a 2a3a 2052 756e 2069 6e66  ation**: Run inf
-00002550: 6572 656e 6365 2077 6974 6820 6c65 7373  erence with less
-00002560: 2063 6f6d 7075 7461 7469 6f6e 616c 2061   computational a
-00002570: 6e64 206d 656d 6f72 7920 636f 7374 7320  nd memory costs 
-00002580: 7769 7468 2071 7561 6e74 697a 6174 696f  with quantizatio
-00002590: 6e20 7465 6368 6e69 7175 6573 2073 7563  n techniques suc
-000025a0: 6820 6173 205b 4c4c 4d2e 696e 7438 5d28  h as [LLM.int8](
-000025b0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-000025c0: 672f 6162 732f 3232 3038 2e30 3733 3339  g/abs/2208.07339
-000025d0: 292c 205b 5370 5152 2028 696e 7434 295d  ), [SpQR (int4)]
-000025e0: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
-000025f0: 7267 2f61 6273 2f32 3330 362e 3033 3037  rg/abs/2306.0307
-00002600: 3829 2c20 5b41 5751 5d28 6874 7470 733a  8), [AWQ](https:
-00002610: 2f2f 6172 7869 762e 6f72 672f 7064 662f  //arxiv.org/pdf/
-00002620: 3233 3036 2e30 3039 3738 2e70 6466 292c  2306.00978.pdf),
-00002630: c2a0 5b47 5054 515d 2868 7474 7073 3a2f  ..[GPTQ](https:/
-00002640: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00002650: 3231 302e 3137 3332 3329 2c20 616e 6420  210.17323), and 
-00002660: 5b53 7175 6565 7a65 4c4c 4d5d 2868 7474  [SqueezeLLM](htt
-00002670: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f70  ps://arxiv.org/p
-00002680: 6466 2f32 3330 362e 3037 3632 3976 322e  df/2306.07629v2.
-00002690: 7064 6629 2e0a 0af0 9f93 a1c2 a02a 2a53  pdf).........**S
-000026a0: 7472 6561 6d69 6e67 2a2a 3a20 5375 7070  treaming**: Supp
-000026b0: 6f72 7420 746f 6b65 6e20 7374 7265 616d  ort token stream
-000026c0: 696e 6720 7468 726f 7567 6820 7365 7276  ing through serv
-000026d0: 6572 2d73 656e 7420 6576 656e 7473 2028  er-sent events (
-000026e0: 5353 4529 2e20 596f 7520 6361 6e20 7573  SSE). You can us
-000026f0: 6520 7468 6520 602f 7631 2f67 656e 6572  e the `/v1/gener
-00002700: 6174 655f 7374 7265 616d 60c2 a065 6e64  ate_stream`..end
-00002710: 706f 696e 7420 666f 7220 7374 7265 616d  point for stream
-00002720: 696e 6720 7265 7370 6f6e 7365 7320 6672  ing responses fr
-00002730: 6f6d 204c 4c4d 732e 0a0a f09f 9484 c2a0  om LLMs.........
-00002740: 2a2a 436f 6e74 696e 756f 7573 2062 6174  **Continuous bat
-00002750: 6368 696e 672a 2a3a 2053 7570 706f 7274  ching**: Support
-00002760: 2063 6f6e 7469 6e75 6f75 7320 6261 7463   continuous batc
-00002770: 6869 6e67 2076 6961 205b 764c 4c4d 5d28  hing via [vLLM](
-00002780: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002790: 6f6d 2f76 6c6c 6d2d 7072 6f6a 6563 742f  om/vllm-project/
-000027a0: 766c 6c6d 2920 666f 7220 696e 6372 6561  vllm) for increa
-000027b0: 7365 6420 746f 7461 6c20 7468 726f 7567  sed total throug
-000027c0: 6870 7574 2e0a 0a4f 7065 6e4c 4c4d 2069  hput...OpenLLM i
-000027d0: 7320 6465 7369 676e 6564 2066 6f72 2041  s designed for A
-000027e0: 4920 6170 706c 6963 6174 696f 6e20 6465  I application de
-000027f0: 7665 6c6f 7065 7273 2077 6f72 6b69 6e67  velopers working
-00002800: 2074 6f20 6275 696c 6420 7072 6f64 7563   to build produc
-00002810: 7469 6f6e 2d72 6561 6479 2061 7070 6c69  tion-ready appli
-00002820: 6361 7469 6f6e 7320 6261 7365 6420 6f6e  cations based on
-00002830: 204c 4c4d 732e 2049 7420 6465 6c69 7665   LLMs. It delive
-00002840: 7273 2061 2063 6f6d 7072 6568 656e 7369  rs a comprehensi
-00002850: 7665 2073 7569 7465 206f 6620 746f 6f6c  ve suite of tool
-00002860: 7320 616e 6420 6665 6174 7572 6573 2066  s and features f
-00002870: 6f72 2066 696e 652d 7475 6e69 6e67 2c20  or fine-tuning, 
-00002880: 7365 7276 696e 672c 2064 6570 6c6f 7969  serving, deployi
-00002890: 6e67 2c20 616e 6420 6d6f 6e69 746f 7269  ng, and monitori
-000028a0: 6e67 2074 6865 7365 206d 6f64 656c 732c  ng these models,
-000028b0: 2073 696d 706c 6966 7969 6e67 2074 6865   simplifying the
-000028c0: 2065 6e64 2d74 6f2d 656e 6420 6465 706c   end-to-end depl
-000028d0: 6f79 6d65 6e74 2077 6f72 6b66 6c6f 7720  oyment workflow 
-000028e0: 666f 7220 4c4c 4d73 2e0a 0a3c 7020 616c  for LLMs...<p al
-000028f0: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
-00002900: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00002910: 2f2f 7261 772e 6769 7468 7562 7573 6572  //raw.githubuser
-00002920: 636f 6e74 656e 742e 636f 6d2f 6265 6e74  content.com/bent
-00002930: 6f6d 6c2f 6f70 656e 6c6c 6d2f 6d61 696e  oml/openllm/main
-00002940: 2f2e 6769 7468 7562 2f61 7373 6574 732f  /.github/assets/
-00002950: 6f75 7470 7574 2e67 6966 2220 616c 743d  output.gif" alt=
-00002960: 2247 6966 2073 686f 7769 6e67 204f 7065  "Gif showing Ope
-00002970: 6e4c 4c4d 2049 6e74 726f 2220 2f3e 0a3c  nLLM Intro" />.<
-00002980: 2f70 3e0a 0a23 2320 f09f 92be 2054 4c2f  /p>..## .... TL/
-00002990: 4452 0a0a 466f 7220 7374 6172 7465 722c  DR..For starter,
-000029a0: 2077 6520 7072 6f76 6964 6520 7477 6f20   we provide two 
-000029b0: 7761 7973 2074 6f20 7175 6963 6b6c 7920  ways to quickly 
-000029c0: 7472 7920 6f75 7420 4f70 656e 4c4c 4d3a  try out OpenLLM:
-000029d0: 0a23 2323 204a 7570 7974 6572 204e 6f74  .### Jupyter Not
-000029e0: 6562 6f6f 6b73 0a0a 5472 7920 7468 6973  ebooks..Try this
-000029f0: 205b 4f70 656e 4c4c 4d20 7475 746f 7269   [OpenLLM tutori
-00002a00: 616c 2069 6e20 476f 6f67 6c65 2043 6f6c  al in Google Col
-00002a10: 6162 3a20 5365 7276 696e 6720 4c6c 616d  ab: Serving Llam
-00002a20: 6120 3220 7769 7468 204f 7065 6e4c 4c4d  a 2 with OpenLLM
-00002a30: 5d28 6874 7470 733a 2f2f 636f 6c61 622e  ](https://colab.
-00002a40: 7265 7365 6172 6368 2e67 6f6f 676c 652e  research.google.
-00002a50: 636f 6d2f 6769 7468 7562 2f62 656e 746f  com/github/bento
-00002a60: 6d6c 2f4f 7065 6e4c 4c4d 2f62 6c6f 622f  ml/OpenLLM/blob/
-00002a70: 6d61 696e 2f65 7861 6d70 6c65 732f 6c6c  main/examples/ll
-00002a80: 616d 6132 2e69 7079 6e62 292e 0a0a 2323  ama2.ipynb)...##
-00002a90: 2320 446f 636b 6572 0a0a 5765 2070 726f  # Docker..We pro
-00002aa0: 7669 6465 2061 2064 6f63 6b65 7220 636f  vide a docker co
-00002ab0: 6e74 6169 6e65 7220 7468 6174 2068 656c  ntainer that hel
-00002ac0: 7073 2079 6f75 2073 7461 7274 2072 756e  ps you start run
-00002ad0: 6e69 6e67 204f 7065 6e4c 4c4d 3a0a 0a60  ning OpenLLM:..`
-00002ae0: 6060 6261 7368 0a64 6f63 6b65 7220 7275  ``bash.docker ru
-00002af0: 6e20 2d2d 726d 202d 6974 202d 7020 3330  n --rm -it -p 30
-00002b00: 3030 3a33 3030 3020 6768 6372 2e69 6f2f  00:3000 ghcr.io/
-00002b10: 6265 6e74 6f6d 6c2f 6f70 656e 6c6c 6d20  bentoml/openllm 
-00002b20: 7374 6172 7420 6661 6365 626f 6f6b 2f6f  start facebook/o
-00002b30: 7074 2d31 2e33 6220 2d2d 6261 636b 656e  pt-1.3b --backen
-00002b40: 6420 7074 0a60 6060 0a0a 3e20 5b21 4e4f  d pt.```..> [!NO
-00002b50: 5445 5d0a 3e20 4769 7665 6e20 796f 7520  TE].> Given you 
-00002b60: 6861 7665 2061 6363 6573 7320 746f 2047  have access to G
-00002b70: 5055 7320 616e 6420 6861 7665 2073 6574  PUs and have set
-00002b80: 7570 205b 6e76 6964 6961 2d64 6f63 6b65  up [nvidia-docke
-00002b90: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-00002ba0: 622e 636f 6d2f 4e56 4944 4941 2f6e 7669  b.com/NVIDIA/nvi
-00002bb0: 6469 612d 636f 6e74 6169 6e65 722d 746f  dia-container-to
-00002bc0: 6f6c 6b69 7429 2c20 2079 6f75 2063 616e  olkit),  you can
-00002bd0: 2061 6464 6974 696f 6e61 6c6c 7920 7061   additionally pa
-00002be0: 7373 2069 6e20 602d 2d67 7075 7360 0a3e  ss in `--gpus`.>
-00002bf0: 2074 6f20 7573 6520 4750 5520 666f 7220   to use GPU for 
-00002c00: 6661 7374 6572 2069 6e66 6572 656e 6365  faster inference
-00002c10: 2061 6e64 206f 7074 696d 697a 6174 696f   and optimizatio
-00002c20: 6e0a 3e60 6060 6261 7368 0a3e 2064 6f63  n.>```bash.> doc
-00002c30: 6b65 7220 7275 6e20 2d2d 726d 202d 2d67  ker run --rm --g
-00002c40: 7075 7320 616c 6c20 2d70 2033 3030 303a  pus all -p 3000:
-00002c50: 3330 3030 202d 6974 2067 6863 722e 696f  3000 -it ghcr.io
-00002c60: 2f62 656e 746f 6d6c 2f6f 7065 6e6c 6c6d  /bentoml/openllm
-00002c70: 2073 7461 7274 2048 7567 6769 6e67 4661   start HuggingFa
-00002c80: 6365 4834 2f7a 6570 6879 722d 3762 2d62  ceH4/zephyr-7b-b
-00002c90: 6574 6120 2d2d 6261 636b 656e 6420 766c  eta --backend vl
-00002ca0: 6c6d 0a3e 2060 6060 0a0a 0a23 2320 f09f  lm.> ```...## ..
-00002cb0: 8f83 2047 6574 2073 7461 7274 6564 0a0a  .. Get started..
-00002cc0: 5468 6520 666f 6c6c 6f77 696e 6720 7072  The following pr
-00002cd0: 6f76 6964 6573 2069 6e73 7472 7563 7469  ovides instructi
-00002ce0: 6f6e 7320 666f 7220 686f 7720 746f 2067  ons for how to g
-00002cf0: 6574 2073 7461 7274 6564 2077 6974 6820  et started with 
-00002d00: 4f70 656e 4c4c 4d20 6c6f 6361 6c6c 792e  OpenLLM locally.
-00002d10: 0a23 2323 2050 7265 7265 7175 6973 6974  .### Prerequisit
-00002d20: 6573 0a0a 596f 7520 6861 7665 2069 6e73  es..You have ins
-00002d30: 7461 6c6c 6564 2050 7974 686f 6e20 332e  talled Python 3.
-00002d40: 3820 286f 7220 6c61 7465 7229 2061 6e64  8 (or later) and
-00002d50: c2a0 6070 6970 602e 2057 6520 6869 6768  ..`pip`. We high
-00002d60: 6c79 2072 6563 6f6d 6d65 6e64 2075 7369  ly recommend usi
-00002d70: 6e67 2061 205b 5669 7274 7561 6c20 456e  ng a [Virtual En
-00002d80: 7669 726f 6e6d 656e 745d 2868 7474 7073  vironment](https
-00002d90: 3a2f 2f64 6f63 732e 7079 7468 6f6e 2e6f  ://docs.python.o
-00002da0: 7267 2f33 2f6c 6962 7261 7279 2f76 656e  rg/3/library/ven
-00002db0: 762e 6874 6d6c 2920 746f 2070 7265 7665  v.html) to preve
-00002dc0: 6e74 2070 6163 6b61 6765 2063 6f6e 666c  nt package confl
-00002dd0: 6963 7473 2e0a 0a23 2323 2049 6e73 7461  icts...### Insta
-00002de0: 6c6c 204f 7065 6e4c 4c4d 0a0a 496e 7374  ll OpenLLM..Inst
-00002df0: 616c 6c20 4f70 656e 4c4c 4d20 6279 2075  all OpenLLM by u
-00002e00: 7369 6e67 2060 7069 7060 2061 7320 666f  sing `pip` as fo
-00002e10: 6c6c 6f77 733a 0a0a 6060 6062 6173 680a  llows:..```bash.
-00002e20: 7069 7020 696e 7374 616c 6c20 6f70 656e  pip install open
-00002e30: 6c6c 6d0a 6060 600a 0a54 6f20 7665 7269  llm.```..To veri
-00002e40: 6679 2074 6865 2069 6e73 7461 6c6c 6174  fy the installat
-00002e50: 696f 6e2c 2072 756e 3a0a 0a60 6060 6261  ion, run:..```ba
-00002e60: 7368 0a24 206f 7065 6e6c 6c6d 202d 680a  sh.$ openllm -h.
-00002e70: 0a55 7361 6765 3a20 6f70 656e 6c6c 6d20  .Usage: openllm 
-00002e80: 5b4f 5054 494f 4e53 5d20 434f 4d4d 414e  [OPTIONS] COMMAN
-00002e90: 4420 5b41 5247 535d 2e2e 2e0a 0a20 2020  D [ARGS].....   
-00002ea0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00002eb0: 9688 e295 9720 e296 88e2 9688 e296 88e2  ..... ..........
-00002ec0: 9688 e296 88e2 9688 e295 9720 e296 88e2  ........... ....
-00002ed0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00002ee0: 88e2 9597 e296 88e2 9688 e296 88e2 9597  ................
-00002ef0: 2020 20e2 9688 e296 88e2 9597 e296 88e2     .............
-00002f00: 9688 e295 9720 2020 2020 e296 88e2 9688  .....     ......
-00002f10: e295 9720 2020 2020 e296 88e2 9688 e296  ...     ........
-00002f20: 88e2 9597 2020 20e2 9688 e296 88e2 9688  ....   .........
-00002f30: e295 970a 2020 e296 88e2 9688 e295 94e2  ....  ..........
-00002f40: 9590 e295 90e2 9590 e296 88e2 9688 e295  ................
-00002f50: 97e2 9688 e296 88e2 9594 e295 90e2 9590  ................
-00002f60: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
-00002f70: 9594 e295 90e2 9590 e295 90e2 9590 e295  ................
-00002f80: 9de2 9688 e296 88e2 9688 e296 88e2 9597  ................
-00002f90: 2020 e296 88e2 9688 e295 91e2 9688 e296    ..............
-00002fa0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
-00002fb0: 9591 2020 2020 20e2 9688 e296 88e2 9688  ..     .........
-00002fc0: e296 88e2 9597 20e2 9688 e296 88e2 9688  ...... .........
-00002fd0: e296 88e2 9591 0a20 20e2 9688 e296 88e2  .......  .......
-00002fe0: 9591 2020 20e2 9688 e296 88e2 9591 e296  ..   ...........
-00002ff0: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
-00003000: e295 94e2 959d e296 88e2 9688 e296 88e2  ................
-00003010: 9688 e296 88e2 9597 2020 e296 88e2 9688  ........  ......
-00003020: e295 94e2 9688 e296 88e2 9597 20e2 9688  ............ ...
-00003030: e296 88e2 9591 e296 88e2 9688 e295 9120  ............... 
-00003040: 2020 2020 e296 88e2 9688 e295 9120 2020      .........   
-00003050: 2020 e296 88e2 9688 e295 94e2 9688 e296    ..............
-00003060: 88e2 9688 e296 88e2 9594 e296 88e2 9688  ................
-00003070: e295 910a 2020 e296 88e2 9688 e295 9120  ....  ......... 
-00003080: 2020 e296 88e2 9688 e295 91e2 9688 e296    ..............
-00003090: 88e2 9594 e295 90e2 9590 e295 90e2 959d  ................
-000030a0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
-000030b0: e295 9d20 20e2 9688 e296 88e2 9591 e295  ...  ...........
-000030c0: 9ae2 9688 e296 88e2 9597 e296 88e2 9688  ................
-000030d0: e295 91e2 9688 e296 88e2 9591 2020 2020  ............    
-000030e0: 20e2 9688 e296 88e2 9591 2020 2020 20e2   .........     .
-000030f0: 9688 e296 88e2 9591 e295 9ae2 9688 e296  ................
-00003100: 88e2 9594 e295 9de2 9688 e296 88e2 9591  ................
-00003110: 0a20 20e2 959a e296 88e2 9688 e296 88e2  .  .............
-00003120: 9688 e296 88e2 9688 e295 94e2 959d e296  ................
-00003130: 88e2 9688 e295 9120 2020 2020 e296 88e2  .......     ....
-00003140: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00003150: 88e2 9597 e296 88e2 9688 e295 9120 e295  ............. ..
-00003160: 9ae2 9688 e296 88e2 9688 e296 88e2 9591  ................
-00003170: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00003180: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
-00003190: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
-000031a0: e296 88e2 9688 e295 9120 e295 9ae2 9590  ......... ......
-000031b0: e295 9d20 e296 88e2 9688 e295 910a 2020  ... ..........  
-000031c0: 20e2 959a e295 90e2 9590 e295 90e2 9590   ...............
-000031d0: e295 90e2 959d 20e2 959a e295 90e2 959d  ...... .........
-000031e0: 2020 2020 20e2 959a e295 90e2 9590 e295       ...........
-000031f0: 90e2 9590 e295 90e2 9590 e295 9de2 959a  ................
-00003200: e295 90e2 959d 2020 e295 9ae2 9590 e295  ......  ........
-00003210: 90e2 9590 e295 9de2 959a e295 90e2 9590  ................
-00003220: e295 90e2 9590 e295 90e2 9590 e295 9de2  ................
-00003230: 959a e295 90e2 9590 e295 90e2 9590 e295  ................
-00003240: 90e2 9590 e295 9de2 959a e295 90e2 959d  ................
-00003250: 2020 2020 20e2 959a e295 90e2 959d 2e0a       ...........
-00003260: 0a20 2041 6e20 6f70 656e 2070 6c61 7466  .  An open platf
-00003270: 6f72 6d20 666f 7220 6f70 6572 6174 696e  orm for operatin
-00003280: 6720 6c61 7267 6520 6c61 6e67 7561 6765  g large language
-00003290: 206d 6f64 656c 7320 696e 2070 726f 6475   models in produ
-000032a0: 6374 696f 6e2e 0a20 2046 696e 652d 7475  ction..  Fine-tu
-000032b0: 6e65 2c20 7365 7276 652c 2064 6570 6c6f  ne, serve, deplo
-000032c0: 792c 2061 6e64 206d 6f6e 6974 6f72 2061  y, and monitor a
-000032d0: 6e79 204c 4c4d 7320 7769 7468 2065 6173  ny LLMs with eas
-000032e0: 652e 0a0a 4f70 7469 6f6e 733a 0a20 202d  e...Options:.  -
-000032f0: 762c 202d 2d76 6572 7369 6f6e 2020 5368  v, --version  Sh
-00003300: 6f77 2074 6865 2076 6572 7369 6f6e 2061  ow the version a
-00003310: 6e64 2065 7869 742e 0a20 202d 682c 202d  nd exit..  -h, -
-00003320: 2d68 656c 7020 2020 2020 5368 6f77 2074  -help     Show t
-00003330: 6869 7320 6d65 7373 6167 6520 616e 6420  his message and 
-00003340: 6578 6974 2e0a 0a43 6f6d 6d61 6e64 733a  exit...Commands:
-00003350: 0a20 2062 7569 6c64 2020 2020 2020 2050  .  build       P
-00003360: 6163 6b61 6765 2061 2067 6976 656e 206d  ackage a given m
-00003370: 6f64 656c 7320 696e 746f 2061 2042 656e  odels into a Ben
-00003380: 746f 4c4c 4d2e 0a20 2069 6d70 6f72 7420  toLLM..  import 
-00003390: 2020 2020 2053 6574 7570 204c 4c4d 2069       Setup LLM i
-000033a0: 6e74 6572 6163 7469 7665 6c79 2e0a 2020  nteractively..  
-000033b0: 6d6f 6465 6c73 2020 2020 2020 4c69 7374  models      List
-000033c0: 2061 6c6c 2073 7570 706f 7274 6564 206d   all supported m
-000033d0: 6f64 656c 732e 0a20 2070 7275 6e65 2020  odels..  prune  
-000033e0: 2020 2020 2052 656d 6f76 6520 616c 6c20       Remove all 
-000033f0: 7361 7665 6420 6d6f 6465 6c73 2c20 2861  saved models, (a
-00003400: 6e64 206f 7074 696f 6e61 6c6c 7920 6265  nd optionally be
-00003410: 6e74 6f73 2920 6275 696c 7420 7769 7468  ntos) built with
-00003420: 204f 7065 6e4c 4c4d 206c 6f63 616c 6c79   OpenLLM locally
-00003430: 2e0a 2020 7175 6572 7920 2020 2020 2020  ..  query       
-00003440: 5175 6572 7920 6120 4c4c 4d20 696e 7465  Query a LLM inte
-00003450: 7261 6374 6976 656c 792c 2066 726f 6d20  ractively, from 
-00003460: 6120 7465 726d 696e 616c 2e0a 2020 7374  a terminal..  st
-00003470: 6172 7420 2020 2020 2020 5374 6172 7420  art       Start 
-00003480: 6120 4c4c 4d53 6572 7665 7220 666f 7220  a LLMServer for 
-00003490: 616e 7920 7375 7070 6f72 7465 6420 4c4c  any supported LL
-000034a0: 4d2e 0a20 2073 7461 7274 2d67 7270 6320  M..  start-grpc 
-000034b0: 2053 7461 7274 2061 2067 5250 4320 4c4c   Start a gRPC LL
-000034c0: 4d53 6572 7665 7220 666f 7220 616e 7920  MServer for any 
-000034d0: 7375 7070 6f72 7465 6420 4c4c 4d2e 0a0a  supported LLM...
-000034e0: 4578 7465 6e73 696f 6e73 3a0a 2020 6275  Extensions:.  bu
-000034f0: 696c 642d 6261 7365 2d63 6f6e 7461 696e  ild-base-contain
-00003500: 6572 2020 4261 7365 2069 6d61 6765 2062  er  Base image b
-00003510: 7569 6c64 6572 2066 6f72 2042 656e 746f  uilder for Bento
-00003520: 4c4c 4d2e 0a20 2064 6976 652d 6265 6e74  LLM..  dive-bent
-00003530: 6f73 2020 2020 2020 2020 2020 2044 6976  os           Div
-00003540: 6520 696e 746f 2061 2042 656e 746f 4c4c  e into a BentoLL
-00003550: 4d2e 0a20 2067 6574 2d63 6f6e 7461 696e  M..  get-contain
-00003560: 6572 6669 6c65 2020 2020 2052 6574 7572  erfile     Retur
-00003570: 6e20 436f 6e74 6169 6e65 7266 696c 6520  n Containerfile 
-00003580: 6f66 2061 6e79 2067 6976 656e 2042 656e  of any given Ben
-00003590: 746f 2e0a 2020 6765 742d 7072 6f6d 7074  to..  get-prompt
-000035a0: 2020 2020 2020 2020 2020 2020 4765 7420              Get 
-000035b0: 7468 6520 6465 6661 756c 7420 7072 6f6d  the default prom
-000035c0: 7074 2075 7365 6420 6279 204f 7065 6e4c  pt used by OpenL
-000035d0: 4c4d 2e0a 2020 6c69 7374 2d62 656e 746f  LM..  list-bento
-000035e0: 7320 2020 2020 2020 2020 2020 4c69 7374  s           List
-000035f0: 2061 7661 696c 6162 6c65 2062 656e 746f   available bento
-00003600: 7320 6275 696c 7420 6279 204f 7065 6e4c  s built by OpenL
-00003610: 4c4d 2e0a 2020 6c69 7374 2d6d 6f64 656c  LM..  list-model
-00003620: 7320 2020 2020 2020 2020 2020 5468 6973  s           This
-00003630: 2069 7320 6571 7569 7661 6c65 6e74 2074   is equivalent t
-00003640: 6f20 6f70 656e 6c6c 6d20 6d6f 6465 6c73  o openllm models
-00003650: 2e2e 2e0a 2020 706c 6179 6772 6f75 6e64  ....  playground
-00003660: 2020 2020 2020 2020 2020 2020 4f70 656e              Open
-00003670: 4c4c 4d20 506c 6179 6772 6f75 6e64 2e0a  LLM Playground..
-00003680: 6060 600a 0a23 2323 2053 7461 7274 2061  ```..### Start a
-00003690: 204c 4c4d 2073 6572 7665 720a 0a4f 7065   LLM server..Ope
-000036a0: 6e4c 4c4d 2061 6c6c 6f77 7320 796f 7520  nLLM allows you 
-000036b0: 746f 2071 7569 636b 6c79 2073 7069 6e20  to quickly spin 
-000036c0: 7570 2061 6e20 4c4c 4d20 7365 7276 6572  up an LLM server
-000036d0: 2075 7369 6e67 2060 6f70 656e 6c6c 6d20   using `openllm 
-000036e0: 7374 6172 7460 2e20 466f 7220 6578 616d  start`. For exam
-000036f0: 706c 652c 2074 6f20 7374 6172 7420 61c2  ple, to start a.
-00003700: a05b 7068 692d 325d 2868 7474 7073 3a2f  .[phi-2](https:/
-00003710: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00003720: 6d69 6372 6f73 6f66 742f 7068 692d 3229  microsoft/phi-2)
-00003730: c2a0 7365 7276 6572 2c20 7275 6e20 7468  ..server, run th
-00003740: 6520 666f 6c6c 6f77 696e 673a 0a0a 6060  e following:..``
-00003750: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
-00003760: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
-00003770: 6e6c 6c6d 2073 7461 7274 206d 6963 726f  nllm start micro
-00003780: 736f 6674 2f70 6869 2d32 0a60 6060 0a0a  soft/phi-2.```..
-00003790: 5468 6973 2073 7461 7274 7320 7468 6520  This starts the 
-000037a0: 7365 7276 6572 2061 74c2 a05b 6874 7470  server at..[http
-000037b0: 3a2f 2f30 2e30 2e30 2e30 3a33 3030 302f  ://0.0.0.0:3000/
-000037c0: 5d28 6874 7470 3a2f 2f30 2e30 2e30 2e30  ](http://0.0.0.0
-000037d0: 3a33 3030 302f 292e 204f 7065 6e4c 4c4d  :3000/). OpenLLM
-000037e0: 2064 6f77 6e6c 6f61 6473 2074 6865 206d   downloads the m
-000037f0: 6f64 656c 2074 6f20 7468 6520 4265 6e74  odel to the Bent
-00003800: 6f4d 4c20 6c6f 6361 6c20 4d6f 6465 6c20  oML local Model 
-00003810: 5374 6f72 6520 6966 2069 7420 6861 7320  Store if it has 
-00003820: 6e6f 7420 6265 656e 2072 6567 6973 7465  not been registe
-00003830: 7265 6420 6265 666f 7265 2e20 546f 2076  red before. To v
-00003840: 6965 7720 796f 7572 206c 6f63 616c 206d  iew your local m
-00003850: 6f64 656c 732c 2072 756e 2060 6265 6e74  odels, run `bent
-00003860: 6f6d 6c20 6d6f 6465 6c73 206c 6973 7460  oml models list`
-00003870: 2e0a 0a54 6f20 696e 7465 7261 6374 2077  ...To interact w
-00003880: 6974 6820 7468 6520 7365 7276 6572 2c20  ith the server, 
-00003890: 796f 7520 6361 6e20 7669 7369 7420 7468  you can visit th
-000038a0: 6520 7765 6220 5549 2061 74c2 a05b 6874  e web UI at..[ht
-000038b0: 7470 3a2f 2f30 2e30 2e30 2e30 3a33 3030  tp://0.0.0.0:300
-000038c0: 302f 5d28 6874 7470 3a2f 2f30 2e30 2e30  0/](http://0.0.0
-000038d0: 2e30 3a33 3030 302f 2920 6f72 2073 656e  .0:3000/) or sen
-000038e0: 6420 6120 7265 7175 6573 7420 7573 696e  d a request usin
-000038f0: 67c2 a060 6375 726c 602e 2059 6f75 2063  g..`curl`. You c
-00003900: 616e 2061 6c73 6f20 7573 6520 4f70 656e  an also use Open
-00003910: 4c4c 4de2 8099 7320 6275 696c 742d 696e  LLM...s built-in
-00003920: 2050 7974 686f 6e20 636c 6965 6e74 2074   Python client t
-00003930: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-00003940: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
-00003950: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f70  python.import op
-00003960: 656e 6c6c 6d0a 0a63 6c69 656e 7420 3d20  enllm..client = 
-00003970: 6f70 656e 6c6c 6d2e 636c 6965 6e74 2e48  openllm.client.H
-00003980: 5454 5043 6c69 656e 7428 2768 7474 703a  TTPClient('http:
-00003990: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-000039a0: 2729 0a63 6c69 656e 742e 7175 6572 7928  ').client.query(
-000039b0: 2745 7870 6c61 696e 2074 6f20 6d65 2074  'Explain to me t
-000039c0: 6865 2064 6966 6665 7265 6e63 6520 6265  he difference be
-000039d0: 7477 6565 6e20 2266 7572 7468 6572 2220  tween "further" 
-000039e0: 616e 6420 2266 6172 7468 6572 2227 290a  and "farther"').
-000039f0: 6060 600a 0a41 6c74 6572 6e61 7469 7665  ```..Alternative
-00003a00: 6c79 2c20 7573 6520 7468 65c2 a060 6f70  ly, use the..`op
-00003a10: 656e 6c6c 6d20 7175 6572 7960 c2a0 636f  enllm query`..co
-00003a20: 6d6d 616e 6420 746f 2071 7565 7279 2074  mmand to query t
-00003a30: 6865 206d 6f64 656c 3a0a 0a60 6060 6261  he model:..```ba
-00003a40: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-00003a50: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
-00003a60: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-00003a70: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
-00003a80: 4578 706c 6169 6e20 746f 206d 6520 7468  Explain to me th
-00003a90: 6520 6469 6666 6572 656e 6365 2062 6574  e difference bet
-00003aa0: 7765 656e 2022 6675 7274 6865 7222 2061  ween "further" a
-00003ab0: 6e64 2022 6661 7274 6865 7222 270a 6060  nd "farther"'.``
-00003ac0: 600a 0a4f 7065 6e4c 4c4d 2073 6561 6d6c  `..OpenLLM seaml
-00003ad0: 6573 736c 7920 7375 7070 6f72 7473 206d  essly supports m
-00003ae0: 616e 7920 6d6f 6465 6c73 2061 6e64 2074  any models and t
-00003af0: 6865 6972 2076 6172 6961 6e74 732e 2059  heir variants. Y
-00003b00: 6f75 2063 616e 2073 7065 6369 6679 2064  ou can specify d
-00003b10: 6966 6665 7265 6e74 2076 6172 6961 6e74  ifferent variant
-00003b20: 7320 6f66 2074 6865 206d 6f64 656c 2074  s of the model t
-00003b30: 6f20 6265 2073 6572 7665 642e 2046 6f72  o be served. For
-00003b40: 2065 7861 6d70 6c65 3a0a 0a60 6060 6261   example:..```ba
-00003b50: 7368 0a6f 7065 6e6c 6c6d 2073 7461 7274  sh.openllm start
-00003b60: 203c 6d6f 6465 6c5f 6964 3e20 2d2d 3c6f   <model_id> --<o
-00003b70: 7074 696f 6e73 3e0a 6060 600a 0a3e 205b  ptions>.```..> [
-00003b80: 214e 4f54 455d 0a3e 204f 7065 6e4c 4c4d  !NOTE].> OpenLLM
-00003b90: 2073 7570 706f 7274 7320 7370 6563 6966   supports specif
-00003ba0: 7969 6e67 2066 696e 652d 7475 6e69 6e67  ying fine-tuning
-00003bb0: 2077 6569 6768 7473 2061 6e64 2071 7561   weights and qua
-00003bc0: 6e74 697a 6564 2077 6569 6768 7473 0a3e  ntized weights.>
-00003bd0: 2066 6f72 2061 6e79 206f 6620 7468 6520   for any of the 
-00003be0: 7375 7070 6f72 7465 6420 6d6f 6465 6c73  supported models
-00003bf0: 2061 7320 6c6f 6e67 2061 7320 7468 6579   as long as they
-00003c00: 2063 616e 2062 6520 6c6f 6164 6564 2077   can be loaded w
-00003c10: 6974 6820 7468 6520 6d6f 6465 6c0a 3e20  ith the model.> 
-00003c20: 6172 6368 6974 6563 7475 7265 2e20 5573  architecture. Us
-00003c30: 6520 7468 65c2 a060 6f70 656e 6c6c 6d20  e the..`openllm 
-00003c40: 6d6f 6465 6c73 60c2 a063 6f6d 6d61 6e64  models`..command
-00003c50: 2074 6f20 7365 6520 7468 6520 636f 6d70   to see the comp
-00003c60: 6c65 7465 206c 6973 7420 6f66 2073 7570  lete list of sup
-00003c70: 706f 7274 6564 0a3e 206d 6f64 656c 732c  ported.> models,
-00003c80: 2074 6865 6972 2061 7263 6869 7465 6374   their architect
-00003c90: 7572 6573 2c20 616e 6420 7468 6569 7220  ures, and their 
-00003ca0: 7661 7269 616e 7473 2e0a 0a3e 205b 2149  variants...> [!I
-00003cb0: 4d50 4f52 5441 4e54 5d0a 3e20 4966 2079  MPORTANT].> If y
-00003cc0: 6f75 2061 7265 2074 6573 7469 6e67 204f  ou are testing O
-00003cd0: 7065 6e4c 4c4d 206f 6e20 4350 552c 2079  penLLM on CPU, y
-00003ce0: 6f75 206d 6967 6874 2077 616e 7420 746f  ou might want to
-00003cf0: 2070 6173 7320 696e 2060 4454 5950 453d   pass in `DTYPE=
-00003d00: 666c 6f61 7433 3260 2e20 4279 2064 6566  float32`. By def
-00003d10: 6175 6c74 2c0a 3e20 4f70 656e 4c4c 4d20  ault,.> OpenLLM 
-00003d20: 7769 6c6c 2073 6574 206d 6f64 656c 2060  will set model `
-00003d30: 6474 7970 6560 2074 6f20 6062 666c 6f61  dtype` to `bfloa
-00003d40: 7431 3660 2066 6f72 2074 6865 2062 6573  t16` for the bes
-00003d50: 7420 7065 7266 6f72 6d61 6e63 652e 0a3e  t performance..>
-00003d60: 2060 6060 6261 7368 0a3e 2044 5459 5045   ```bash.> DTYPE
-00003d70: 3d66 6c6f 6174 3332 206f 7065 6e6c 6c6d  =float32 openllm
-00003d80: 2073 7461 7274 206d 6963 726f 736f 6674   start microsoft
-00003d90: 2f70 6869 2d32 0a3e 2060 6060 0a3e 2054  /phi-2.> ```.> T
-00003da0: 6869 7320 7769 6c6c 2061 6c73 6f20 6170  his will also ap
-00003db0: 706c 6965 7320 746f 206f 6c64 6572 2047  plies to older G
-00003dc0: 5055 732e 2049 6620 796f 7572 2047 5055  PUs. If your GPU
-00003dd0: 7320 646f 6573 6e27 7420 7375 7070 6f72  s doesn't suppor
-00003de0: 7420 6062 666c 6f61 7431 3660 2c20 7468  t `bfloat16`, th
-00003df0: 656e 2079 6f75 2061 6c73 6f0a 3e20 7761  en you also.> wa
-00003e00: 6e74 2074 6f20 7365 7420 6044 5459 5045  nt to set `DTYPE
-00003e10: 3d66 6c6f 6174 3136 602e 0a0a 2323 20f0  =float16`...## .
-00003e20: 9fa7 a920 5375 7070 6f72 7465 6420 6d6f  ... Supported mo
-00003e30: 6465 6c73 0a0a 4f70 656e 4c4c 4d20 6375  dels..OpenLLM cu
-00003e40: 7272 656e 746c 7920 7375 7070 6f72 7473  rrently supports
-00003e50: 2074 6865 2066 6f6c 6c6f 7769 6e67 206d   the following m
-00003e60: 6f64 656c 732e 2042 7920 6465 6661 756c  odels. By defaul
-00003e70: 742c 204f 7065 6e4c 4c4d 2064 6f65 736e  t, OpenLLM doesn
-00003e80: 2774 2069 6e63 6c75 6465 2064 6570 656e  't include depen
-00003e90: 6465 6e63 6965 7320 746f 2072 756e 2061  dencies to run a
-00003ea0: 6c6c 206d 6f64 656c 732e 2054 6865 2065  ll models. The e
-00003eb0: 7874 7261 206d 6f64 656c 2d73 7065 6369  xtra model-speci
-00003ec0: 6669 6320 6465 7065 6e64 656e 6369 6573  fic dependencies
-00003ed0: 2063 616e 2062 6520 696e 7374 616c 6c65   can be installe
-00003ee0: 6420 7769 7468 2074 6865 2069 6e73 7472  d with the instr
-00003ef0: 7563 7469 6f6e 7320 6265 6c6f 772e 0a0a  uctions below...
-00003f00: 3c21 2d2d 2075 7064 6174 652d 7265 6164  <!-- update-read
-00003f10: 6d65 2e70 793a 2073 7461 7274 202d 2d3e  me.py: start -->
-00003f20: 0a3c 6465 7461 696c 733e 0a0a 3c73 756d  .<details>..<sum
-00003f30: 6d61 7279 3e42 6169 6368 7561 6e3c 2f73  mary>Baichuan</s
-00003f40: 756d 6d61 7279 3e0a 0a0a 2323 2320 5175  ummary>...### Qu
-00003f50: 6963 6b73 7461 7274 0a0a 0a0a 3e20 2a2a  ickstart....> **
-00003f60: 4e6f 7465 3a2a 2a20 4261 6963 6875 616e  Note:** Baichuan
-00003f70: 2072 6571 7569 7265 7320 746f 2069 6e73   requires to ins
-00003f80: 7461 6c6c 2077 6974 683a 0a3e 2060 6060  tall with:.> ```
-00003f90: 6261 7368 0a3e 2070 6970 2069 6e73 7461  bash.> pip insta
-00003fa0: 6c6c 2022 6f70 656e 6c6c 6d5b 6261 6963  ll "openllm[baic
-00003fb0: 6875 616e 5d22 0a3e 2060 6060 0a0a 0a52  huan]".> ```...R
-00003fc0: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00003fd0: 2063 6f6d 6d61 6e64 2074 6f20 7175 6963   command to quic
-00003fe0: 6b6c 7920 7370 696e 2075 7020 6120 4261  kly spin up a Ba
-00003ff0: 6963 6875 616e 2073 6572 7665 723a 0a0a  ichuan server:..
-00004000: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
-00004010: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
-00004020: 7065 6e6c 6c6d 2073 7461 7274 2062 6169  penllm start bai
-00004030: 6368 7561 6e2d 696e 632f 6261 6963 6875  chuan-inc/baichu
-00004040: 616e 2d37 620a 6060 600a 496e 2061 2064  an-7b.```.In a d
-00004050: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
-00004060: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
-00004070: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00004080: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
-00004090: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
-000040a0: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-000040b0: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
-000040c0: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
-000040d0: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
-000040e0: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
-000040f0: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
-00004100: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
-00004110: 2a2a 2041 6e79 2042 6169 6368 7561 6e20  ** Any Baichuan 
-00004120: 7661 7269 616e 7473 2063 616e 2062 6520  variants can be 
-00004130: 6465 706c 6f79 6564 2077 6974 6820 4f70  deployed with Op
-00004140: 656e 4c4c 4d2e 2056 6973 6974 2074 6865  enLLM. Visit the
-00004150: 205b 4875 6767 696e 6746 6163 6520 4d6f   [HuggingFace Mo
-00004160: 6465 6c20 4875 625d 2868 7474 7073 3a2f  del Hub](https:/
-00004170: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00004180: 6d6f 6465 6c73 3f73 6f72 743d 7472 656e  models?sort=tren
-00004190: 6469 6e67 2673 6561 7263 683d 6261 6963  ding&search=baic
-000041a0: 6875 616e 2920 746f 2073 6565 206d 6f72  huan) to see mor
-000041b0: 6520 4261 6963 6875 616e 2d63 6f6d 7061  e Baichuan-compa
-000041c0: 7469 626c 6520 6d6f 6465 6c73 2e0a 0a0a  tible models....
-000041d0: 0a23 2323 2053 7570 706f 7274 6564 206d  .### Supported m
-000041e0: 6f64 656c 730a 0a59 6f75 2063 616e 2073  odels..You can s
-000041f0: 7065 6369 6679 2061 6e79 206f 6620 7468  pecify any of th
-00004200: 6520 666f 6c6c 6f77 696e 6720 4261 6963  e following Baic
-00004210: 6875 616e 206d 6f64 656c 7320 7669 6120  huan models via 
-00004220: 606f 7065 6e6c 6c6d 2073 7461 7274 603a  `openllm start`:
-00004230: 0a0a 0a2d 205b 6261 6963 6875 616e 2d69  ...- [baichuan-i
-00004240: 6e63 2f62 6169 6368 7561 6e32 2d37 622d  nc/baichuan2-7b-
-00004250: 6261 7365 5d28 6874 7470 733a 2f2f 6875  base](https://hu
-00004260: 6767 696e 6766 6163 652e 636f 2f62 6169  ggingface.co/bai
-00004270: 6368 7561 6e2d 696e 632f 6261 6963 6875  chuan-inc/baichu
-00004280: 616e 322d 3762 2d62 6173 6529 0a2d 205b  an2-7b-base).- [
-00004290: 6261 6963 6875 616e 2d69 6e63 2f62 6169  baichuan-inc/bai
-000042a0: 6368 7561 6e32 2d37 622d 6368 6174 5d28  chuan2-7b-chat](
-000042b0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-000042c0: 6163 652e 636f 2f62 6169 6368 7561 6e2d  ace.co/baichuan-
-000042d0: 696e 632f 6261 6963 6875 616e 322d 3762  inc/baichuan2-7b
-000042e0: 2d63 6861 7429 0a2d 205b 6261 6963 6875  -chat).- [baichu
-000042f0: 616e 2d69 6e63 2f62 6169 6368 7561 6e32  an-inc/baichuan2
-00004300: 2d31 3362 2d62 6173 655d 2868 7474 7073  -13b-base](https
-00004310: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00004320: 6f2f 6261 6963 6875 616e 2d69 6e63 2f62  o/baichuan-inc/b
-00004330: 6169 6368 7561 6e32 2d31 3362 2d62 6173  aichuan2-13b-bas
-00004340: 6529 0a2d 205b 6261 6963 6875 616e 2d69  e).- [baichuan-i
-00004350: 6e63 2f62 6169 6368 7561 6e32 2d31 3362  nc/baichuan2-13b
-00004360: 2d63 6861 745d 2868 7474 7073 3a2f 2f68  -chat](https://h
-00004370: 7567 6769 6e67 6661 6365 2e63 6f2f 6261  uggingface.co/ba
-00004380: 6963 6875 616e 2d69 6e63 2f62 6169 6368  ichuan-inc/baich
-00004390: 7561 6e32 2d31 3362 2d63 6861 7429 0a0a  uan2-13b-chat)..
-000043a0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-000043b0: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-000043c0: 4368 6174 474c 4d3c 2f73 756d 6d61 7279  ChatGLM</summary
-000043d0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
-000043e0: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
-000043f0: 2a20 4368 6174 474c 4d20 7265 7175 6972  * ChatGLM requir
-00004400: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
-00004410: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
-00004420: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
-00004430: 6e6c 6c6d 5b63 6861 7467 6c6d 5d22 0a3e  nllm[chatglm]".>
-00004440: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
-00004450: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00004460: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
-00004470: 2075 7020 6120 4368 6174 474c 4d20 7365   up a ChatGLM se
-00004480: 7276 6572 3a0a 0a60 6060 6261 7368 0a54  rver:..```bash.T
-00004490: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
-000044a0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
-000044b0: 6172 7420 7468 7564 6d2f 6368 6174 676c  art thudm/chatgl
-000044c0: 6d2d 3662 0a60 6060 0a49 6e20 6120 6469  m-6b.```.In a di
-000044d0: 6666 6572 656e 7420 7465 726d 696e 616c  fferent terminal
-000044e0: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
-000044f0: 696e 6720 636f 6d6d 616e 6420 746f 2069  ing command to i
-00004500: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
-00004510: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
-00004520: 680a 6578 706f 7274 204f 5045 4e4c 4c4d  h.export OPENLLM
-00004530: 5f45 4e44 504f 494e 543d 6874 7470 3a2f  _ENDPOINT=http:/
-00004540: 2f6c 6f63 616c 686f 7374 3a33 3030 300a  /localhost:3000.
-00004550: 6f70 656e 6c6c 6d20 7175 6572 7920 2757  openllm query 'W
-00004560: 6861 7420 6172 6520 6c61 7267 6520 6c61  hat are large la
-00004570: 6e67 7561 6765 206d 6f64 656c 733f 270a  nguage models?'.
-00004580: 6060 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a  ```...> **Note:*
-00004590: 2a20 416e 7920 4368 6174 474c 4d20 7661  * Any ChatGLM va
-000045a0: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
-000045b0: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
-000045c0: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
-000045d0: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
-000045e0: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
-000045f0: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
-00004600: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
-00004610: 6e67 2673 6561 7263 683d 6368 6174 676c  ng&search=chatgl
-00004620: 6d29 2074 6f20 7365 6520 6d6f 7265 2043  m) to see more C
-00004630: 6861 7447 4c4d 2d63 6f6d 7061 7469 626c  hatGLM-compatibl
-00004640: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
-00004650: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
-00004660: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
-00004670: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
-00004680: 6c6c 6f77 696e 6720 4368 6174 474c 4d20  llowing ChatGLM 
-00004690: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
-000046a0: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
-000046b0: 5b74 6875 646d 2f63 6861 7467 6c6d 2d36  [thudm/chatglm-6
-000046c0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
-000046d0: 6e67 6661 6365 2e63 6f2f 7468 7564 6d2f  ngface.co/thudm/
-000046e0: 6368 6174 676c 6d2d 3662 290a 2d20 5b74  chatglm-6b).- [t
-000046f0: 6875 646d 2f63 6861 7467 6c6d 2d36 622d  hudm/chatglm-6b-
-00004700: 696e 7438 5d28 6874 7470 733a 2f2f 6875  int8](https://hu
-00004710: 6767 696e 6766 6163 652e 636f 2f74 6875  ggingface.co/thu
-00004720: 646d 2f63 6861 7467 6c6d 2d36 622d 696e  dm/chatglm-6b-in
-00004730: 7438 290a 2d20 5b74 6875 646d 2f63 6861  t8).- [thudm/cha
-00004740: 7467 6c6d 2d36 622d 696e 7434 5d28 6874  tglm-6b-int4](ht
-00004750: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00004760: 652e 636f 2f74 6875 646d 2f63 6861 7467  e.co/thudm/chatg
-00004770: 6c6d 2d36 622d 696e 7434 290a 2d20 5b74  lm-6b-int4).- [t
-00004780: 6875 646d 2f63 6861 7467 6c6d 322d 3662  hudm/chatglm2-6b
-00004790: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000047a0: 6766 6163 652e 636f 2f74 6875 646d 2f63  gface.co/thudm/c
-000047b0: 6861 7467 6c6d 322d 3662 290a 2d20 5b74  hatglm2-6b).- [t
-000047c0: 6875 646d 2f63 6861 7467 6c6d 322d 3662  hudm/chatglm2-6b
-000047d0: 2d69 6e74 345d 2868 7474 7073 3a2f 2f68  -int4](https://h
-000047e0: 7567 6769 6e67 6661 6365 2e63 6f2f 7468  uggingface.co/th
-000047f0: 7564 6d2f 6368 6174 676c 6d32 2d36 622d  udm/chatglm2-6b-
-00004800: 696e 7434 290a 2d20 5b74 6875 646d 2f63  int4).- [thudm/c
-00004810: 6861 7467 6c6d 332d 3662 5d28 6874 7470  hatglm3-6b](http
-00004820: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00004830: 636f 2f74 6875 646d 2f63 6861 7467 6c6d  co/thudm/chatglm
-00004840: 332d 3662 290a 0a3c 2f64 6574 6169 6c73  3-6b)..</details
-00004850: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
-00004860: 756d 6d61 7279 3e44 6272 783c 2f73 756d  ummary>Dbrx</sum
-00004870: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
-00004880: 6b73 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f  kstart....> **No
-00004890: 7465 3a2a 2a20 4462 7278 2072 6571 7569  te:** Dbrx requi
-000048a0: 7265 7320 746f 2069 6e73 7461 6c6c 2077  res to install w
-000048b0: 6974 683a 0a3e 2060 6060 6261 7368 0a3e  ith:.> ```bash.>
-000048c0: 2070 6970 2069 6e73 7461 6c6c 2022 6f70   pip install "op
-000048d0: 656e 6c6c 6d5b 6462 7278 5d22 0a3e 2060  enllm[dbrx]".> `
-000048e0: 6060 0a0a 0a52 756e 2074 6865 2066 6f6c  ``...Run the fol
-000048f0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-00004900: 6f20 7175 6963 6b6c 7920 7370 696e 2075  o quickly spin u
-00004910: 7020 6120 4462 7278 2073 6572 7665 723a  p a Dbrx server:
-00004920: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
-00004930: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
-00004940: 206f 7065 6e6c 6c6d 2073 7461 7274 2064   openllm start d
-00004950: 6174 6162 7269 636b 732f 6462 7278 2d69  atabricks/dbrx-i
-00004960: 6e73 7472 7563 740a 6060 600a 496e 2061  nstruct.```.In a
-00004970: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
-00004980: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
-00004990: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-000049a0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-000049b0: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
-000049c0: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
-000049d0: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
-000049e0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-000049f0: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
-00004a00: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
-00004a10: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00004a20: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
-00004a30: 653a 2a2a 2041 6e79 2044 6272 7820 7661  e:** Any Dbrx va
-00004a40: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
-00004a50: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
-00004a60: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
-00004a70: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
-00004a80: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
-00004a90: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
-00004aa0: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
-00004ab0: 6e67 2673 6561 7263 683d 6462 7278 2920  ng&search=dbrx) 
-00004ac0: 746f 2073 6565 206d 6f72 6520 4462 7278  to see more Dbrx
-00004ad0: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
-00004ae0: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
-00004af0: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
-00004b00: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
-00004b10: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-00004b20: 6720 4462 7278 206d 6f64 656c 7320 7669  g Dbrx models vi
-00004b30: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
-00004b40: 603a 0a0a 0a2d 205b 6461 7461 6272 6963  `:...- [databric
-00004b50: 6b73 2f64 6272 782d 696e 7374 7275 6374  ks/dbrx-instruct
-00004b60: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00004b70: 6766 6163 652e 636f 2f64 6174 6162 7269  gface.co/databri
-00004b80: 636b 732f 6462 7278 2d69 6e73 7472 7563  cks/dbrx-instruc
-00004b90: 7429 0a2d 205b 6461 7461 6272 6963 6b73  t).- [databricks
-00004ba0: 2f64 6272 782d 6261 7365 5d28 6874 7470  /dbrx-base](http
-00004bb0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00004bc0: 636f 2f64 6174 6162 7269 636b 732f 6462  co/databricks/db
-00004bd0: 7278 2d62 6173 6529 0a0a 3c2f 6465 7461  rx-base)..</deta
-00004be0: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
-00004bf0: 0a3c 7375 6d6d 6172 793e 446f 6c6c 7956  .<summary>DollyV
-00004c00: 323c 2f73 756d 6d61 7279 3e0a 0a0a 2323  2</summary>...##
-00004c10: 2320 5175 6963 6b73 7461 7274 0a0a 5275  # Quickstart..Ru
-00004c20: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-00004c30: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
-00004c40: 6c79 2073 7069 6e20 7570 2061 2044 6f6c  ly spin up a Dol
-00004c50: 6c79 5632 2073 6572 7665 723a 0a0a 6060  lyV2 server:..``
-00004c60: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
-00004c70: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
-00004c80: 6e6c 6c6d 2073 7461 7274 2064 6174 6162  nllm start datab
-00004c90: 7269 636b 732f 646f 6c6c 792d 7632 2d33  ricks/dolly-v2-3
-00004ca0: 620a 6060 600a 496e 2061 2064 6966 6665  b.```.In a diffe
-00004cb0: 7265 6e74 2074 6572 6d69 6e61 6c2c 2072  rent terminal, r
-00004cc0: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00004cd0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7465   command to inte
-00004ce0: 7261 6374 2077 6974 6820 7468 6520 7365  ract with the se
-00004cf0: 7276 6572 3a0a 0a60 6060 6261 7368 0a65  rver:..```bash.e
-00004d00: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
-00004d10: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
-00004d20: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
-00004d30: 6e6c 6c6d 2071 7565 7279 2027 5768 6174  nllm query 'What
-00004d40: 2061 7265 206c 6172 6765 206c 616e 6775   are large langu
-00004d50: 6167 6520 6d6f 6465 6c73 3f27 0a60 6060  age models?'.```
-00004d60: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2041  ...> **Note:** A
-00004d70: 6e79 2044 6f6c 6c79 5632 2076 6172 6961  ny DollyV2 varia
-00004d80: 6e74 7320 6361 6e20 6265 2064 6570 6c6f  nts can be deplo
-00004d90: 7965 6420 7769 7468 204f 7065 6e4c 4c4d  yed with OpenLLM
-00004da0: 2e20 5669 7369 7420 7468 6520 5b48 7567  . Visit the [Hug
-00004db0: 6769 6e67 4661 6365 204d 6f64 656c 2048  gingFace Model H
-00004dc0: 7562 5d28 6874 7470 733a 2f2f 6875 6767  ub](https://hugg
-00004dd0: 696e 6766 6163 652e 636f 2f6d 6f64 656c  ingface.co/model
-00004de0: 733f 736f 7274 3d74 7265 6e64 696e 6726  s?sort=trending&
-00004df0: 7365 6172 6368 3d64 6f6c 6c79 5f76 3229  search=dolly_v2)
-00004e00: 2074 6f20 7365 6520 6d6f 7265 2044 6f6c   to see more Dol
-00004e10: 6c79 5632 2d63 6f6d 7061 7469 626c 6520  lyV2-compatible 
-00004e20: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
-00004e30: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
-00004e40: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
-00004e50: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
-00004e60: 6f77 696e 6720 446f 6c6c 7956 3220 6d6f  owing DollyV2 mo
-00004e70: 6465 6c73 2076 6961 2060 6f70 656e 6c6c  dels via `openll
-00004e80: 6d20 7374 6172 7460 3a0a 0a0a 2d20 5b64  m start`:...- [d
-00004e90: 6174 6162 7269 636b 732f 646f 6c6c 792d  atabricks/dolly-
-00004ea0: 7632 2d33 625d 2868 7474 7073 3a2f 2f68  v2-3b](https://h
-00004eb0: 7567 6769 6e67 6661 6365 2e63 6f2f 6461  uggingface.co/da
-00004ec0: 7461 6272 6963 6b73 2f64 6f6c 6c79 2d76  tabricks/dolly-v
-00004ed0: 322d 3362 290a 2d20 5b64 6174 6162 7269  2-3b).- [databri
-00004ee0: 636b 732f 646f 6c6c 792d 7632 2d37 625d  cks/dolly-v2-7b]
-00004ef0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00004f00: 6661 6365 2e63 6f2f 6461 7461 6272 6963  face.co/databric
-00004f10: 6b73 2f64 6f6c 6c79 2d76 322d 3762 290a  ks/dolly-v2-7b).
-00004f20: 2d20 5b64 6174 6162 7269 636b 732f 646f  - [databricks/do
-00004f30: 6c6c 792d 7632 2d31 3262 5d28 6874 7470  lly-v2-12b](http
-00004f40: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00004f50: 636f 2f64 6174 6162 7269 636b 732f 646f  co/databricks/do
-00004f60: 6c6c 792d 7632 2d31 3262 290a 0a3c 2f64  lly-v2-12b)..</d
-00004f70: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
-00004f80: 733e 0a0a 3c73 756d 6d61 7279 3e46 616c  s>..<summary>Fal
-00004f90: 636f 6e3c 2f73 756d 6d61 7279 3e0a 0a0a  con</summary>...
-00004fa0: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
-00004fb0: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 4661  ..> **Note:** Fa
-00004fc0: 6c63 6f6e 2072 6571 7569 7265 7320 746f  lcon requires to
-00004fd0: 2069 6e73 7461 6c6c 2077 6974 683a 0a3e   install with:.>
-00004fe0: 2060 6060 6261 7368 0a3e 2070 6970 2069   ```bash.> pip i
-00004ff0: 6e73 7461 6c6c 2022 6f70 656e 6c6c 6d5b  nstall "openllm[
-00005000: 6661 6c63 6f6e 5d22 0a3e 2060 6060 0a0a  falcon]".> ```..
-00005010: 0a52 756e 2074 6865 2066 6f6c 6c6f 7769  .Run the followi
-00005020: 6e67 2063 6f6d 6d61 6e64 2074 6f20 7175  ng command to qu
-00005030: 6963 6b6c 7920 7370 696e 2075 7020 6120  ickly spin up a 
-00005040: 4661 6c63 6f6e 2073 6572 7665 723a 0a0a  Falcon server:..
-00005050: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
-00005060: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
-00005070: 7065 6e6c 6c6d 2073 7461 7274 2074 6969  penllm start tii
-00005080: 7561 652f 6661 6c63 6f6e 2d37 620a 6060  uae/falcon-7b.``
-00005090: 600a 496e 2061 2064 6966 6665 7265 6e74  `.In a different
-000050a0: 2074 6572 6d69 6e61 6c2c 2072 756e 2074   terminal, run t
-000050b0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-000050c0: 6d61 6e64 2074 6f20 696e 7465 7261 6374  mand to interact
-000050d0: 2077 6974 6820 7468 6520 7365 7276 6572   with the server
-000050e0: 3a0a 0a60 6060 6261 7368 0a65 7870 6f72  :..```bash.expor
-000050f0: 7420 4f50 454e 4c4c 4d5f 454e 4450 4f49  t OPENLLM_ENDPOI
-00005100: 4e54 3d68 7474 703a 2f2f 6c6f 6361 6c68  NT=http://localh
-00005110: 6f73 743a 3330 3030 0a6f 7065 6e6c 6c6d  ost:3000.openllm
-00005120: 2071 7565 7279 2027 5768 6174 2061 7265   query 'What are
-00005130: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
-00005140: 6d6f 6465 6c73 3f27 0a60 6060 0a0a 0a3e  models?'.```...>
-00005150: 202a 2a4e 6f74 653a 2a2a 2041 6e79 2046   **Note:** Any F
-00005160: 616c 636f 6e20 7661 7269 616e 7473 2063  alcon variants c
-00005170: 616e 2062 6520 6465 706c 6f79 6564 2077  an be deployed w
-00005180: 6974 6820 4f70 656e 4c4c 4d2e 2056 6973  ith OpenLLM. Vis
-00005190: 6974 2074 6865 205b 4875 6767 696e 6746  it the [HuggingF
-000051a0: 6163 6520 4d6f 6465 6c20 4875 625d 2868  ace Model Hub](h
-000051b0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000051c0: 6365 2e63 6f2f 6d6f 6465 6c73 3f73 6f72  ce.co/models?sor
-000051d0: 743d 7472 656e 6469 6e67 2673 6561 7263  t=trending&searc
-000051e0: 683d 6661 6c63 6f6e 2920 746f 2073 6565  h=falcon) to see
-000051f0: 206d 6f72 6520 4661 6c63 6f6e 2d63 6f6d   more Falcon-com
-00005200: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
-00005210: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
-00005220: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
-00005230: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
-00005240: 7468 6520 666f 6c6c 6f77 696e 6720 4661  the following Fa
-00005250: 6c63 6f6e 206d 6f64 656c 7320 7669 6120  lcon models via 
-00005260: 606f 7065 6e6c 6c6d 2073 7461 7274 603a  `openllm start`:
-00005270: 0a0a 0a2d 205b 7469 6975 6165 2f66 616c  ...- [tiiuae/fal
-00005280: 636f 6e2d 3762 5d28 6874 7470 733a 2f2f  con-7b](https://
-00005290: 6875 6767 696e 6766 6163 652e 636f 2f74  huggingface.co/t
-000052a0: 6969 7561 652f 6661 6c63 6f6e 2d37 6229  iiuae/falcon-7b)
-000052b0: 0a2d 205b 7469 6975 6165 2f66 616c 636f  .- [tiiuae/falco
-000052c0: 6e2d 3430 625d 2868 7474 7073 3a2f 2f68  n-40b](https://h
-000052d0: 7567 6769 6e67 6661 6365 2e63 6f2f 7469  uggingface.co/ti
-000052e0: 6975 6165 2f66 616c 636f 6e2d 3430 6229  iuae/falcon-40b)
-000052f0: 0a2d 205b 7469 6975 6165 2f66 616c 636f  .- [tiiuae/falco
-00005300: 6e2d 3762 2d69 6e73 7472 7563 745d 2868  n-7b-instruct](h
-00005310: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00005320: 6365 2e63 6f2f 7469 6975 6165 2f66 616c  ce.co/tiiuae/fal
-00005330: 636f 6e2d 3762 2d69 6e73 7472 7563 7429  con-7b-instruct)
-00005340: 0a2d 205b 7469 6975 6165 2f66 616c 636f  .- [tiiuae/falco
-00005350: 6e2d 3430 622d 696e 7374 7275 6374 5d28  n-40b-instruct](
-00005360: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00005370: 6163 652e 636f 2f74 6969 7561 652f 6661  ace.co/tiiuae/fa
-00005380: 6c63 6f6e 2d34 3062 2d69 6e73 7472 7563  lcon-40b-instruc
-00005390: 7429 0a0a 3c2f 6465 7461 696c 733e 0a0a  t)..</details>..
-000053a0: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
-000053b0: 6172 793e 466c 616e 5435 3c2f 7375 6d6d  ary>FlanT5</summ
-000053c0: 6172 793e 0a0a 0a23 2323 2051 7569 636b  ary>...### Quick
-000053d0: 7374 6172 740a 0a52 756e 2074 6865 2066  start..Run the f
-000053e0: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-000053f0: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
-00005400: 2075 7020 6120 466c 616e 5435 2073 6572   up a FlanT5 ser
-00005410: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
-00005420: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
-00005430: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
-00005440: 7274 2067 6f6f 676c 652f 666c 616e 2d74  rt google/flan-t
-00005450: 352d 6c61 7267 650a 6060 600a 496e 2061  5-large.```.In a
-00005460: 2064 6966 6665 7265 6e74 2074 6572 6d69   different termi
-00005470: 6e61 6c2c 2072 756e 2074 6865 2066 6f6c  nal, run the fol
-00005480: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
-00005490: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-000054a0: 7468 6520 7365 7276 6572 3a0a 0a60 6060  the server:..```
-000054b0: 6261 7368 0a65 7870 6f72 7420 4f50 454e  bash.export OPEN
-000054c0: 4c4c 4d5f 454e 4450 4f49 4e54 3d68 7474  LLM_ENDPOINT=htt
-000054d0: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
-000054e0: 3030 0a6f 7065 6e6c 6c6d 2071 7565 7279  00.openllm query
-000054f0: 2027 5768 6174 2061 7265 206c 6172 6765   'What are large
-00005500: 206c 616e 6775 6167 6520 6d6f 6465 6c73   language models
-00005510: 3f27 0a60 6060 0a0a 0a3e 202a 2a4e 6f74  ?'.```...> **Not
-00005520: 653a 2a2a 2041 6e79 2046 6c61 6e54 3520  e:** Any FlanT5 
-00005530: 7661 7269 616e 7473 2063 616e 2062 6520  variants can be 
-00005540: 6465 706c 6f79 6564 2077 6974 6820 4f70  deployed with Op
-00005550: 656e 4c4c 4d2e 2056 6973 6974 2074 6865  enLLM. Visit the
-00005560: 205b 4875 6767 696e 6746 6163 6520 4d6f   [HuggingFace Mo
-00005570: 6465 6c20 4875 625d 2868 7474 7073 3a2f  del Hub](https:/
-00005580: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00005590: 6d6f 6465 6c73 3f73 6f72 743d 7472 656e  models?sort=tren
-000055a0: 6469 6e67 2673 6561 7263 683d 666c 616e  ding&search=flan
-000055b0: 5f74 3529 2074 6f20 7365 6520 6d6f 7265  _t5) to see more
-000055c0: 2046 6c61 6e54 352d 636f 6d70 6174 6962   FlanT5-compatib
-000055d0: 6c65 206d 6f64 656c 732e 0a0a 0a0a 2323  le models.....##
-000055e0: 2320 5375 7070 6f72 7465 6420 6d6f 6465  # Supported mode
-000055f0: 6c73 0a0a 596f 7520 6361 6e20 7370 6563  ls..You can spec
-00005600: 6966 7920 616e 7920 6f66 2074 6865 2066  ify any of the f
-00005610: 6f6c 6c6f 7769 6e67 2046 6c61 6e54 3520  ollowing FlanT5 
-00005620: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
-00005630: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
-00005640: 5b67 6f6f 676c 652f 666c 616e 2d74 352d  [google/flan-t5-
-00005650: 736d 616c 6c5d 2868 7474 7073 3a2f 2f68  small](https://h
-00005660: 7567 6769 6e67 6661 6365 2e63 6f2f 676f  uggingface.co/go
-00005670: 6f67 6c65 2f66 6c61 6e2d 7435 2d73 6d61  ogle/flan-t5-sma
-00005680: 6c6c 290a 2d20 5b67 6f6f 676c 652f 666c  ll).- [google/fl
-00005690: 616e 2d74 352d 6261 7365 5d28 6874 7470  an-t5-base](http
-000056a0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-000056b0: 636f 2f67 6f6f 676c 652f 666c 616e 2d74  co/google/flan-t
-000056c0: 352d 6261 7365 290a 2d20 5b67 6f6f 676c  5-base).- [googl
-000056d0: 652f 666c 616e 2d74 352d 6c61 7267 655d  e/flan-t5-large]
-000056e0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-000056f0: 6661 6365 2e63 6f2f 676f 6f67 6c65 2f66  face.co/google/f
-00005700: 6c61 6e2d 7435 2d6c 6172 6765 290a 2d20  lan-t5-large).- 
-00005710: 5b67 6f6f 676c 652f 666c 616e 2d74 352d  [google/flan-t5-
-00005720: 786c 5d28 6874 7470 733a 2f2f 6875 6767  xl](https://hugg
-00005730: 696e 6766 6163 652e 636f 2f67 6f6f 676c  ingface.co/googl
-00005740: 652f 666c 616e 2d74 352d 786c 290a 2d20  e/flan-t5-xl).- 
-00005750: 5b67 6f6f 676c 652f 666c 616e 2d74 352d  [google/flan-t5-
-00005760: 7878 6c5d 2868 7474 7073 3a2f 2f68 7567  xxl](https://hug
-00005770: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
-00005780: 6c65 2f66 6c61 6e2d 7435 2d78 786c 290a  le/flan-t5-xxl).
-00005790: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
-000057a0: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
-000057b0: 3e47 656d 6d61 3c2f 7375 6d6d 6172 793e  >Gemma</summary>
-000057c0: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
-000057d0: 740a 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  t....> **Note:**
-000057e0: 2047 656d 6d61 2072 6571 7569 7265 7320   Gemma requires 
-000057f0: 746f 2069 6e73 7461 6c6c 2077 6974 683a  to install with:
-00005800: 0a3e 2060 6060 6261 7368 0a3e 2070 6970  .> ```bash.> pip
-00005810: 2069 6e73 7461 6c6c 2022 6f70 656e 6c6c   install "openll
-00005820: 6d5b 6765 6d6d 615d 220a 3e20 6060 600a  m[gemma]".> ```.
-00005830: 0a0a 5275 6e20 7468 6520 666f 6c6c 6f77  ..Run the follow
-00005840: 696e 6720 636f 6d6d 616e 6420 746f 2071  ing command to q
-00005850: 7569 636b 6c79 2073 7069 6e20 7570 2061  uickly spin up a
-00005860: 2047 656d 6d61 2073 6572 7665 723a 0a0a   Gemma server:..
-00005870: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
-00005880: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
-00005890: 7065 6e6c 6c6d 2073 7461 7274 2067 6f6f  penllm start goo
-000058a0: 676c 652f 6765 6d6d 612d 3762 0a60 6060  gle/gemma-7b.```
-000058b0: 0a49 6e20 6120 6469 6666 6572 656e 7420  .In a different 
-000058c0: 7465 726d 696e 616c 2c20 7275 6e20 7468  terminal, run th
-000058d0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-000058e0: 616e 6420 746f 2069 6e74 6572 6163 7420  and to interact 
-000058f0: 7769 7468 2074 6865 2073 6572 7665 723a  with the server:
-00005900: 0a0a 6060 6062 6173 680a 6578 706f 7274  ..```bash.export
-00005910: 204f 5045 4e4c 4c4d 5f45 4e44 504f 494e   OPENLLM_ENDPOIN
-00005920: 543d 6874 7470 3a2f 2f6c 6f63 616c 686f  T=http://localho
-00005930: 7374 3a33 3030 300a 6f70 656e 6c6c 6d20  st:3000.openllm 
-00005940: 7175 6572 7920 2757 6861 7420 6172 6520  query 'What are 
-00005950: 6c61 7267 6520 6c61 6e67 7561 6765 206d  large language m
-00005960: 6f64 656c 733f 270a 6060 600a 0a0a 3e20  odels?'.```...> 
-00005970: 2a2a 4e6f 7465 3a2a 2a20 416e 7920 4765  **Note:** Any Ge
-00005980: 6d6d 6120 7661 7269 616e 7473 2063 616e  mma variants can
-00005990: 2062 6520 6465 706c 6f79 6564 2077 6974   be deployed wit
-000059a0: 6820 4f70 656e 4c4c 4d2e 2056 6973 6974  h OpenLLM. Visit
-000059b0: 2074 6865 205b 4875 6767 696e 6746 6163   the [HuggingFac
-000059c0: 6520 4d6f 6465 6c20 4875 625d 2868 7474  e Model Hub](htt
-000059d0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-000059e0: 2e63 6f2f 6d6f 6465 6c73 3f73 6f72 743d  .co/models?sort=
-000059f0: 7472 656e 6469 6e67 2673 6561 7263 683d  trending&search=
-00005a00: 6765 6d6d 6129 2074 6f20 7365 6520 6d6f  gemma) to see mo
-00005a10: 7265 2047 656d 6d61 2d63 6f6d 7061 7469  re Gemma-compati
-00005a20: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-00005a30: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00005a40: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-00005a50: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-00005a60: 666f 6c6c 6f77 696e 6720 4765 6d6d 6120  following Gemma 
-00005a70: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
-00005a80: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
-00005a90: 5b67 6f6f 676c 652f 6765 6d6d 612d 3762  [google/gemma-7b
-00005aa0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00005ab0: 6766 6163 652e 636f 2f67 6f6f 676c 652f  gface.co/google/
-00005ac0: 6765 6d6d 612d 3762 290a 2d20 5b67 6f6f  gemma-7b).- [goo
-00005ad0: 676c 652f 6765 6d6d 612d 3762 2d69 745d  gle/gemma-7b-it]
-00005ae0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
-00005af0: 6661 6365 2e63 6f2f 676f 6f67 6c65 2f67  face.co/google/g
-00005b00: 656d 6d61 2d37 622d 6974 290a 2d20 5b67  emma-7b-it).- [g
-00005b10: 6f6f 676c 652f 6765 6d6d 612d 3262 5d28  oogle/gemma-2b](
-00005b20: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00005b30: 6163 652e 636f 2f67 6f6f 676c 652f 6765  ace.co/google/ge
-00005b40: 6d6d 612d 3262 290a 2d20 5b67 6f6f 676c  mma-2b).- [googl
-00005b50: 652f 6765 6d6d 612d 3262 2d69 745d 2868  e/gemma-2b-it](h
-00005b60: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00005b70: 6365 2e63 6f2f 676f 6f67 6c65 2f67 656d  ce.co/google/gem
-00005b80: 6d61 2d32 622d 6974 290a 0a3c 2f64 6574  ma-2b-it)..</det
-00005b90: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
-00005ba0: 0a0a 3c73 756d 6d61 7279 3e47 5054 4e65  ..<summary>GPTNe
-00005bb0: 6f58 3c2f 7375 6d6d 6172 793e 0a0a 0a23  oX</summary>...#
-00005bc0: 2323 2051 7569 636b 7374 6172 740a 0a52  ## Quickstart..R
-00005bd0: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00005be0: 2063 6f6d 6d61 6e64 2074 6f20 7175 6963   command to quic
-00005bf0: 6b6c 7920 7370 696e 2075 7020 6120 4750  kly spin up a GP
-00005c00: 544e 656f 5820 7365 7276 6572 3a0a 0a60  TNeoX server:..`
-00005c10: 6060 6261 7368 0a54 5255 5354 5f52 454d  ``bash.TRUST_REM
-00005c20: 4f54 455f 434f 4445 3d54 7275 6520 6f70  OTE_CODE=True op
-00005c30: 656e 6c6c 6d20 7374 6172 7420 656c 6575  enllm start eleu
-00005c40: 7468 6572 6169 2f67 7074 2d6e 656f 782d  therai/gpt-neox-
-00005c50: 3230 620a 6060 600a 496e 2061 2064 6966  20b.```.In a dif
-00005c60: 6665 7265 6e74 2074 6572 6d69 6e61 6c2c  ferent terminal,
-00005c70: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
-00005c80: 6e67 2063 6f6d 6d61 6e64 2074 6f20 696e  ng command to in
-00005c90: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
-00005ca0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
-00005cb0: 0a65 7870 6f72 7420 4f50 454e 4c4c 4d5f  .export OPENLLM_
-00005cc0: 454e 4450 4f49 4e54 3d68 7474 703a 2f2f  ENDPOINT=http://
-00005cd0: 6c6f 6361 6c68 6f73 743a 3330 3030 0a6f  localhost:3000.o
-00005ce0: 7065 6e6c 6c6d 2071 7565 7279 2027 5768  penllm query 'Wh
-00005cf0: 6174 2061 7265 206c 6172 6765 206c 616e  at are large lan
-00005d00: 6775 6167 6520 6d6f 6465 6c73 3f27 0a60  guage models?'.`
-00005d10: 6060 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  ``...> **Note:**
-00005d20: 2041 6e79 2047 5054 4e65 6f58 2076 6172   Any GPTNeoX var
-00005d30: 6961 6e74 7320 6361 6e20 6265 2064 6570  iants can be dep
-00005d40: 6c6f 7965 6420 7769 7468 204f 7065 6e4c  loyed with OpenL
-00005d50: 4c4d 2e20 5669 7369 7420 7468 6520 5b48  LM. Visit the [H
-00005d60: 7567 6769 6e67 4661 6365 204d 6f64 656c  uggingFace Model
-00005d70: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
-00005d80: 6767 696e 6766 6163 652e 636f 2f6d 6f64  ggingface.co/mod
-00005d90: 656c 733f 736f 7274 3d74 7265 6e64 696e  els?sort=trendin
-00005da0: 6726 7365 6172 6368 3d67 7074 5f6e 656f  g&search=gpt_neo
-00005db0: 7829 2074 6f20 7365 6520 6d6f 7265 2047  x) to see more G
-00005dc0: 5054 4e65 6f58 2d63 6f6d 7061 7469 626c  PTNeoX-compatibl
-00005dd0: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
-00005de0: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
-00005df0: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
-00005e00: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
-00005e10: 6c6c 6f77 696e 6720 4750 544e 656f 5820  llowing GPTNeoX 
-00005e20: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
-00005e30: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
-00005e40: 5b65 6c65 7574 6865 7261 692f 6770 742d  [eleutherai/gpt-
-00005e50: 6e65 6f78 2d32 3062 5d28 6874 7470 733a  neox-20b](https:
-00005e60: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00005e70: 2f65 6c65 7574 6865 7261 692f 6770 742d  /eleutherai/gpt-
-00005e80: 6e65 6f78 2d32 3062 290a 0a3c 2f64 6574  neox-20b)..</det
-00005e90: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
-00005ea0: 0a0a 3c73 756d 6d61 7279 3e4c 6c61 6d61  ..<summary>Llama
-00005eb0: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
-00005ec0: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
-00005ed0: 202a 2a4e 6f74 653a 2a2a 204c 6c61 6d61   **Note:** Llama
-00005ee0: 2072 6571 7569 7265 7320 746f 2069 6e73   requires to ins
-00005ef0: 7461 6c6c 2077 6974 683a 0a3e 2060 6060  tall with:.> ```
-00005f00: 6261 7368 0a3e 2070 6970 2069 6e73 7461  bash.> pip insta
-00005f10: 6c6c 2022 6f70 656e 6c6c 6d5b 6c6c 616d  ll "openllm[llam
-00005f20: 615d 220a 3e20 6060 600a 0a0a 5275 6e20  a]".> ```...Run 
-00005f30: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00005f40: 6d6d 616e 6420 746f 2071 7569 636b 6c79  mmand to quickly
-00005f50: 2073 7069 6e20 7570 2061 204c 6c61 6d61   spin up a Llama
-00005f60: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
-00005f70: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
-00005f80: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
-00005f90: 2073 7461 7274 204e 6f75 7352 6573 6561   start NousResea
-00005fa0: 7263 682f 6c6c 616d 612d 322d 3762 2d68  rch/llama-2-7b-h
-00005fb0: 660a 6060 600a 496e 2061 2064 6966 6665  f.```.In a diffe
-00005fc0: 7265 6e74 2074 6572 6d69 6e61 6c2c 2072  rent terminal, r
-00005fd0: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00005fe0: 2063 6f6d 6d61 6e64 2074 6f20 696e 7465   command to inte
-00005ff0: 7261 6374 2077 6974 6820 7468 6520 7365  ract with the se
-00006000: 7276 6572 3a0a 0a60 6060 6261 7368 0a65  rver:..```bash.e
-00006010: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
-00006020: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
-00006030: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
-00006040: 6e6c 6c6d 2071 7565 7279 2027 5768 6174  nllm query 'What
-00006050: 2061 7265 206c 6172 6765 206c 616e 6775   are large langu
-00006060: 6167 6520 6d6f 6465 6c73 3f27 0a60 6060  age models?'.```
-00006070: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2041  ...> **Note:** A
-00006080: 6e79 204c 6c61 6d61 2076 6172 6961 6e74  ny Llama variant
-00006090: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
-000060a0: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
-000060b0: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
-000060c0: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
-000060d0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000060e0: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
-000060f0: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
-00006100: 6172 6368 3d6c 6c61 6d61 2920 746f 2073  arch=llama) to s
-00006110: 6565 206d 6f72 6520 4c6c 616d 612d 636f  ee more Llama-co
-00006120: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
-00006130: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
-00006140: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
-00006150: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
-00006160: 2074 6865 2066 6f6c 6c6f 7769 6e67 204c   the following L
-00006170: 6c61 6d61 206d 6f64 656c 7320 7669 6120  lama models via 
-00006180: 606f 7065 6e6c 6c6d 2073 7461 7274 603a  `openllm start`:
-00006190: 0a0a 0a2d 205b 6d65 7461 2d6c 6c61 6d61  ...- [meta-llama
-000061a0: 2f4c 6c61 6d61 2d32 2d37 3062 2d63 6861  /Llama-2-70b-cha
-000061b0: 742d 6866 5d28 6874 7470 733a 2f2f 6875  t-hf](https://hu
-000061c0: 6767 696e 6766 6163 652e 636f 2f6d 6574  ggingface.co/met
-000061d0: 612d 6c6c 616d 612f 4c6c 616d 612d 322d  a-llama/Llama-2-
-000061e0: 3730 622d 6368 6174 2d68 6629 0a2d 205b  70b-chat-hf).- [
-000061f0: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
-00006200: 2d32 2d31 3362 2d63 6861 742d 6866 5d28  -2-13b-chat-hf](
-00006210: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00006220: 6163 652e 636f 2f6d 6574 612d 6c6c 616d  ace.co/meta-llam
-00006230: 612f 4c6c 616d 612d 322d 3133 622d 6368  a/Llama-2-13b-ch
-00006240: 6174 2d68 6629 0a2d 205b 6d65 7461 2d6c  at-hf).- [meta-l
-00006250: 6c61 6d61 2f4c 6c61 6d61 2d32 2d37 622d  lama/Llama-2-7b-
-00006260: 6368 6174 2d68 665d 2868 7474 7073 3a2f  chat-hf](https:/
-00006270: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00006280: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
-00006290: 2d32 2d37 622d 6368 6174 2d68 6629 0a2d  -2-7b-chat-hf).-
-000062a0: 205b 6d65 7461 2d6c 6c61 6d61 2f4c 6c61   [meta-llama/Lla
-000062b0: 6d61 2d32 2d37 3062 2d68 665d 2868 7474  ma-2-70b-hf](htt
-000062c0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-000062d0: 2e63 6f2f 6d65 7461 2d6c 6c61 6d61 2f4c  .co/meta-llama/L
-000062e0: 6c61 6d61 2d32 2d37 3062 2d68 6629 0a2d  lama-2-70b-hf).-
-000062f0: 205b 6d65 7461 2d6c 6c61 6d61 2f4c 6c61   [meta-llama/Lla
-00006300: 6d61 2d32 2d31 3362 2d68 665d 2868 7474  ma-2-13b-hf](htt
-00006310: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00006320: 2e63 6f2f 6d65 7461 2d6c 6c61 6d61 2f4c  .co/meta-llama/L
-00006330: 6c61 6d61 2d32 2d31 3362 2d68 6629 0a2d  lama-2-13b-hf).-
-00006340: 205b 6d65 7461 2d6c 6c61 6d61 2f4c 6c61   [meta-llama/Lla
-00006350: 6d61 2d32 2d37 622d 6866 5d28 6874 7470  ma-2-7b-hf](http
-00006360: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00006370: 636f 2f6d 6574 612d 6c6c 616d 612f 4c6c  co/meta-llama/Ll
-00006380: 616d 612d 322d 3762 2d68 6629 0a2d 205b  ama-2-7b-hf).- [
-00006390: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-000063a0: 6d61 2d32 2d37 3062 2d63 6861 742d 6866  ma-2-70b-chat-hf
-000063b0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000063c0: 6766 6163 652e 636f 2f4e 6f75 7352 6573  gface.co/NousRes
-000063d0: 6561 7263 682f 6c6c 616d 612d 322d 3730  earch/llama-2-70
-000063e0: 622d 6368 6174 2d68 6629 0a2d 205b 4e6f  b-chat-hf).- [No
-000063f0: 7573 5265 7365 6172 6368 2f6c 6c61 6d61  usResearch/llama
-00006400: 2d32 2d31 3362 2d63 6861 742d 6866 5d28  -2-13b-chat-hf](
-00006410: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00006420: 6163 652e 636f 2f4e 6f75 7352 6573 6561  ace.co/NousResea
-00006430: 7263 682f 6c6c 616d 612d 322d 3133 622d  rch/llama-2-13b-
-00006440: 6368 6174 2d68 6629 0a2d 205b 4e6f 7573  chat-hf).- [Nous
-00006450: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
-00006460: 2d37 622d 6368 6174 2d68 665d 2868 7474  -7b-chat-hf](htt
-00006470: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00006480: 2e63 6f2f 4e6f 7573 5265 7365 6172 6368  .co/NousResearch
-00006490: 2f6c 6c61 6d61 2d32 2d37 622d 6368 6174  /llama-2-7b-chat
-000064a0: 2d68 6629 0a2d 205b 4e6f 7573 5265 7365  -hf).- [NousRese
-000064b0: 6172 6368 2f6c 6c61 6d61 2d32 2d37 3062  arch/llama-2-70b
-000064c0: 2d68 665d 2868 7474 7073 3a2f 2f68 7567  -hf](https://hug
-000064d0: 6769 6e67 6661 6365 2e63 6f2f 4e6f 7573  gingface.co/Nous
-000064e0: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
-000064f0: 2d37 3062 2d68 6629 0a2d 205b 4e6f 7573  -70b-hf).- [Nous
-00006500: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
-00006510: 2d31 3362 2d68 665d 2868 7474 7073 3a2f  -13b-hf](https:/
-00006520: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00006530: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-00006540: 6d61 2d32 2d31 3362 2d68 6629 0a2d 205b  ma-2-13b-hf).- [
-00006550: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
-00006560: 6d61 2d32 2d37 622d 6866 5d28 6874 7470  ma-2-7b-hf](http
-00006570: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00006580: 636f 2f4e 6f75 7352 6573 6561 7263 682f  co/NousResearch/
-00006590: 6c6c 616d 612d 322d 3762 2d68 6629 0a0a  llama-2-7b-hf)..
-000065a0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-000065b0: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-000065c0: 4d69 7374 7261 6c3c 2f73 756d 6d61 7279  Mistral</summary
-000065d0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
-000065e0: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
-000065f0: 2a20 4d69 7374 7261 6c20 7265 7175 6972  * Mistral requir
-00006600: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
-00006610: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
-00006620: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
-00006630: 6e6c 6c6d 5b6d 6973 7472 616c 5d22 0a3e  nllm[mistral]".>
-00006640: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
-00006650: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00006660: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
-00006670: 2075 7020 6120 4d69 7374 7261 6c20 7365   up a Mistral se
-00006680: 7276 6572 3a0a 0a60 6060 6261 7368 0a54  rver:..```bash.T
-00006690: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
-000066a0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
-000066b0: 6172 7420 6d69 7374 7261 6c61 692f 4d69  art mistralai/Mi
-000066c0: 7374 7261 6c2d 3742 2d49 6e73 7472 7563  stral-7B-Instruc
-000066d0: 742d 7630 2e31 0a60 6060 0a49 6e20 6120  t-v0.1.```.In a 
-000066e0: 6469 6666 6572 656e 7420 7465 726d 696e  different termin
-000066f0: 616c 2c20 7275 6e20 7468 6520 666f 6c6c  al, run the foll
-00006700: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
-00006710: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
-00006720: 6865 2073 6572 7665 723a 0a0a 6060 6062  he server:..```b
-00006730: 6173 680a 6578 706f 7274 204f 5045 4e4c  ash.export OPENL
-00006740: 4c4d 5f45 4e44 504f 494e 543d 6874 7470  LM_ENDPOINT=http
-00006750: 3a2f 2f6c 6f63 616c 686f 7374 3a33 3030  ://localhost:300
-00006760: 300a 6f70 656e 6c6c 6d20 7175 6572 7920  0.openllm query 
-00006770: 2757 6861 7420 6172 6520 6c61 7267 6520  'What are large 
-00006780: 6c61 6e67 7561 6765 206d 6f64 656c 733f  language models?
-00006790: 270a 6060 600a 0a0a 3e20 2a2a 4e6f 7465  '.```...> **Note
-000067a0: 3a2a 2a20 416e 7920 4d69 7374 7261 6c20  :** Any Mistral 
-000067b0: 7661 7269 616e 7473 2063 616e 2062 6520  variants can be 
-000067c0: 6465 706c 6f79 6564 2077 6974 6820 4f70  deployed with Op
-000067d0: 656e 4c4c 4d2e 2056 6973 6974 2074 6865  enLLM. Visit the
-000067e0: 205b 4875 6767 696e 6746 6163 6520 4d6f   [HuggingFace Mo
-000067f0: 6465 6c20 4875 625d 2868 7474 7073 3a2f  del Hub](https:/
-00006800: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00006810: 6d6f 6465 6c73 3f73 6f72 743d 7472 656e  models?sort=tren
-00006820: 6469 6e67 2673 6561 7263 683d 6d69 7374  ding&search=mist
-00006830: 7261 6c29 2074 6f20 7365 6520 6d6f 7265  ral) to see more
-00006840: 204d 6973 7472 616c 2d63 6f6d 7061 7469   Mistral-compati
-00006850: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-00006860: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00006870: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-00006880: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-00006890: 666f 6c6c 6f77 696e 6720 4d69 7374 7261  following Mistra
-000068a0: 6c20 6d6f 6465 6c73 2076 6961 2060 6f70  l models via `op
-000068b0: 656e 6c6c 6d20 7374 6172 7460 3a0a 0a0a  enllm start`:...
-000068c0: 2d20 5b48 7567 6769 6e67 4661 6365 4834  - [HuggingFaceH4
-000068d0: 2f7a 6570 6879 722d 3762 2d61 6c70 6861  /zephyr-7b-alpha
-000068e0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-000068f0: 6766 6163 652e 636f 2f48 7567 6769 6e67  gface.co/Hugging
-00006900: 4661 6365 4834 2f7a 6570 6879 722d 3762  FaceH4/zephyr-7b
-00006910: 2d61 6c70 6861 290a 2d20 5b48 7567 6769  -alpha).- [Huggi
-00006920: 6e67 4661 6365 4834 2f7a 6570 6879 722d  ngFaceH4/zephyr-
-00006930: 3762 2d62 6574 615d 2868 7474 7073 3a2f  7b-beta](https:/
-00006940: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00006950: 4875 6767 696e 6746 6163 6548 342f 7a65  HuggingFaceH4/ze
-00006960: 7068 7972 2d37 622d 6265 7461 290a 2d20  phyr-7b-beta).- 
-00006970: 5b6d 6973 7472 616c 6169 2f4d 6973 7472  [mistralai/Mistr
-00006980: 616c 2d37 422d 496e 7374 7275 6374 2d76  al-7B-Instruct-v
-00006990: 302e 325d 2868 7474 7073 3a2f 2f68 7567  0.2](https://hug
-000069a0: 6769 6e67 6661 6365 2e63 6f2f 6d69 7374  gingface.co/mist
-000069b0: 7261 6c61 692f 4d69 7374 7261 6c2d 3742  ralai/Mistral-7B
-000069c0: 2d49 6e73 7472 7563 742d 7630 2e32 290a  -Instruct-v0.2).
-000069d0: 2d20 5b6d 6973 7472 616c 6169 2f4d 6973  - [mistralai/Mis
-000069e0: 7472 616c 2d37 422d 496e 7374 7275 6374  tral-7B-Instruct
-000069f0: 2d76 302e 315d 2868 7474 7073 3a2f 2f68  -v0.1](https://h
-00006a00: 7567 6769 6e67 6661 6365 2e63 6f2f 6d69  uggingface.co/mi
-00006a10: 7374 7261 6c61 692f 4d69 7374 7261 6c2d  stralai/Mistral-
-00006a20: 3742 2d49 6e73 7472 7563 742d 7630 2e31  7B-Instruct-v0.1
-00006a30: 290a 2d20 5b6d 6973 7472 616c 6169 2f4d  ).- [mistralai/M
-00006a40: 6973 7472 616c 2d37 422d 7630 2e31 5d28  istral-7B-v0.1](
-00006a50: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-00006a60: 6163 652e 636f 2f6d 6973 7472 616c 6169  ace.co/mistralai
-00006a70: 2f4d 6973 7472 616c 2d37 422d 7630 2e31  /Mistral-7B-v0.1
-00006a80: 290a 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  )..</details>..<
-00006a90: 6465 7461 696c 733e 0a0a 3c73 756d 6d61  details>..<summa
-00006aa0: 7279 3e4d 6978 7472 616c 3c2f 7375 6d6d  ry>Mixtral</summ
-00006ab0: 6172 793e 0a0a 0a23 2323 2051 7569 636b  ary>...### Quick
-00006ac0: 7374 6172 740a 0a0a 0a3e 202a 2a4e 6f74  start....> **Not
-00006ad0: 653a 2a2a 204d 6978 7472 616c 2072 6571  e:** Mixtral req
-00006ae0: 7569 7265 7320 746f 2069 6e73 7461 6c6c  uires to install
-00006af0: 2077 6974 683a 0a3e 2060 6060 6261 7368   with:.> ```bash
-00006b00: 0a3e 2070 6970 2069 6e73 7461 6c6c 2022  .> pip install "
-00006b10: 6f70 656e 6c6c 6d5b 6d69 7874 7261 6c5d  openllm[mixtral]
-00006b20: 220a 3e20 6060 600a 0a0a 5275 6e20 7468  ".> ```...Run th
-00006b30: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-00006b40: 616e 6420 746f 2071 7569 636b 6c79 2073  and to quickly s
-00006b50: 7069 6e20 7570 2061 204d 6978 7472 616c  pin up a Mixtral
-00006b60: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
-00006b70: 680a 5452 5553 545f 5245 4d4f 5445 5f43  h.TRUST_REMOTE_C
-00006b80: 4f44 453d 5472 7565 206f 7065 6e6c 6c6d  ODE=True openllm
-00006b90: 2073 7461 7274 206d 6973 7472 616c 6169   start mistralai
-00006ba0: 2f4d 6978 7472 616c 2d38 7837 422d 496e  /Mixtral-8x7B-In
-00006bb0: 7374 7275 6374 2d76 302e 310a 6060 600a  struct-v0.1.```.
-00006bc0: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-00006bd0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-00006be0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00006bf0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-00006c00: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-00006c10: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00006c20: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00006c30: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00006c40: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00006c50: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00006c60: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00006c70: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00006c80: 2a4e 6f74 653a 2a2a 2041 6e79 204d 6978  *Note:** Any Mix
-00006c90: 7472 616c 2076 6172 6961 6e74 7320 6361  tral variants ca
-00006ca0: 6e20 6265 2064 6570 6c6f 7965 6420 7769  n be deployed wi
-00006cb0: 7468 204f 7065 6e4c 4c4d 2e20 5669 7369  th OpenLLM. Visi
-00006cc0: 7420 7468 6520 5b48 7567 6769 6e67 4661  t the [HuggingFa
-00006cd0: 6365 204d 6f64 656c 2048 7562 5d28 6874  ce Model Hub](ht
-00006ce0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00006cf0: 652e 636f 2f6d 6f64 656c 733f 736f 7274  e.co/models?sort
-00006d00: 3d74 7265 6e64 696e 6726 7365 6172 6368  =trending&search
-00006d10: 3d6d 6978 7472 616c 2920 746f 2073 6565  =mixtral) to see
-00006d20: 206d 6f72 6520 4d69 7874 7261 6c2d 636f   more Mixtral-co
-00006d30: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
-00006d40: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
-00006d50: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
-00006d60: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
-00006d70: 2074 6865 2066 6f6c 6c6f 7769 6e67 204d   the following M
-00006d80: 6978 7472 616c 206d 6f64 656c 7320 7669  ixtral models vi
-00006d90: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
-00006da0: 603a 0a0a 0a2d 205b 6d69 7374 7261 6c61  `:...- [mistrala
-00006db0: 692f 4d69 7874 7261 6c2d 3878 3742 2d49  i/Mixtral-8x7B-I
-00006dc0: 6e73 7472 7563 742d 7630 2e31 5d28 6874  nstruct-v0.1](ht
-00006dd0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00006de0: 652e 636f 2f6d 6973 7472 616c 6169 2f4d  e.co/mistralai/M
-00006df0: 6978 7472 616c 2d38 7837 422d 496e 7374  ixtral-8x7B-Inst
-00006e00: 7275 6374 2d76 302e 3129 0a2d 205b 6d69  ruct-v0.1).- [mi
-00006e10: 7374 7261 6c61 692f 4d69 7874 7261 6c2d  stralai/Mixtral-
-00006e20: 3878 3742 2d76 302e 315d 2868 7474 7073  8x7B-v0.1](https
-00006e30: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00006e40: 6f2f 6d69 7374 7261 6c61 692f 4d69 7874  o/mistralai/Mixt
-00006e50: 7261 6c2d 3878 3742 2d76 302e 3129 0a0a  ral-8x7B-v0.1)..
-00006e60: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
-00006e70: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
-00006e80: 4d50 543c 2f73 756d 6d61 7279 3e0a 0a0a  MPT</summary>...
-00006e90: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
-00006ea0: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 4d50  ..> **Note:** MP
-00006eb0: 5420 7265 7175 6972 6573 2074 6f20 696e  T requires to in
-00006ec0: 7374 616c 6c20 7769 7468 3a0a 3e20 6060  stall with:.> ``
-00006ed0: 6062 6173 680a 3e20 7069 7020 696e 7374  `bash.> pip inst
-00006ee0: 616c 6c20 226f 7065 6e6c 6c6d 5b6d 7074  all "openllm[mpt
-00006ef0: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
-00006f00: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00006f10: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
-00006f20: 7370 696e 2075 7020 6120 4d50 5420 7365  spin up a MPT se
-00006f30: 7276 6572 3a0a 0a60 6060 6261 7368 0a54  rver:..```bash.T
-00006f40: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
-00006f50: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
-00006f60: 6172 7420 6d6f 7361 6963 6d6c 2f6d 7074  art mosaicml/mpt
-00006f70: 2d37 622d 696e 7374 7275 6374 0a60 6060  -7b-instruct.```
-00006f80: 0a49 6e20 6120 6469 6666 6572 656e 7420  .In a different 
-00006f90: 7465 726d 696e 616c 2c20 7275 6e20 7468  terminal, run th
-00006fa0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-00006fb0: 616e 6420 746f 2069 6e74 6572 6163 7420  and to interact 
-00006fc0: 7769 7468 2074 6865 2073 6572 7665 723a  with the server:
-00006fd0: 0a0a 6060 6062 6173 680a 6578 706f 7274  ..```bash.export
-00006fe0: 204f 5045 4e4c 4c4d 5f45 4e44 504f 494e   OPENLLM_ENDPOIN
-00006ff0: 543d 6874 7470 3a2f 2f6c 6f63 616c 686f  T=http://localho
-00007000: 7374 3a33 3030 300a 6f70 656e 6c6c 6d20  st:3000.openllm 
-00007010: 7175 6572 7920 2757 6861 7420 6172 6520  query 'What are 
-00007020: 6c61 7267 6520 6c61 6e67 7561 6765 206d  large language m
-00007030: 6f64 656c 733f 270a 6060 600a 0a0a 3e20  odels?'.```...> 
-00007040: 2a2a 4e6f 7465 3a2a 2a20 416e 7920 4d50  **Note:** Any MP
-00007050: 5420 7661 7269 616e 7473 2063 616e 2062  T variants can b
-00007060: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
-00007070: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
-00007080: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
-00007090: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
-000070a0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-000070b0: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
-000070c0: 656e 6469 6e67 2673 6561 7263 683d 6d70  ending&search=mp
-000070d0: 7429 2074 6f20 7365 6520 6d6f 7265 204d  t) to see more M
-000070e0: 5054 2d63 6f6d 7061 7469 626c 6520 6d6f  PT-compatible mo
-000070f0: 6465 6c73 2e0a 0a0a 0a23 2323 2053 7570  dels.....### Sup
-00007100: 706f 7274 6564 206d 6f64 656c 730a 0a59  ported models..Y
-00007110: 6f75 2063 616e 2073 7065 6369 6679 2061  ou can specify a
-00007120: 6e79 206f 6620 7468 6520 666f 6c6c 6f77  ny of the follow
-00007130: 696e 6720 4d50 5420 6d6f 6465 6c73 2076  ing MPT models v
-00007140: 6961 2060 6f70 656e 6c6c 6d20 7374 6172  ia `openllm star
-00007150: 7460 3a0a 0a0a 2d20 5b6d 6f73 6169 636d  t`:...- [mosaicm
-00007160: 6c2f 6d70 742d 3762 5d28 6874 7470 733a  l/mpt-7b](https:
-00007170: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-00007180: 2f6d 6f73 6169 636d 6c2f 6d70 742d 3762  /mosaicml/mpt-7b
-00007190: 290a 2d20 5b6d 6f73 6169 636d 6c2f 6d70  ).- [mosaicml/mp
-000071a0: 742d 3762 2d69 6e73 7472 7563 745d 2868  t-7b-instruct](h
-000071b0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000071c0: 6365 2e63 6f2f 6d6f 7361 6963 6d6c 2f6d  ce.co/mosaicml/m
-000071d0: 7074 2d37 622d 696e 7374 7275 6374 290a  pt-7b-instruct).
-000071e0: 2d20 5b6d 6f73 6169 636d 6c2f 6d70 742d  - [mosaicml/mpt-
-000071f0: 3762 2d63 6861 745d 2868 7474 7073 3a2f  7b-chat](https:/
-00007200: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00007210: 6d6f 7361 6963 6d6c 2f6d 7074 2d37 622d  mosaicml/mpt-7b-
-00007220: 6368 6174 290a 2d20 5b6d 6f73 6169 636d  chat).- [mosaicm
-00007230: 6c2f 6d70 742d 3762 2d73 746f 7279 7772  l/mpt-7b-storywr
-00007240: 6974 6572 5d28 6874 7470 733a 2f2f 6875  iter](https://hu
-00007250: 6767 696e 6766 6163 652e 636f 2f6d 6f73  ggingface.co/mos
-00007260: 6169 636d 6c2f 6d70 742d 3762 2d73 746f  aicml/mpt-7b-sto
-00007270: 7279 7772 6974 6572 290a 2d20 5b6d 6f73  rywriter).- [mos
-00007280: 6169 636d 6c2f 6d70 742d 3330 625d 2868  aicml/mpt-30b](h
-00007290: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000072a0: 6365 2e63 6f2f 6d6f 7361 6963 6d6c 2f6d  ce.co/mosaicml/m
-000072b0: 7074 2d33 3062 290a 2d20 5b6d 6f73 6169  pt-30b).- [mosai
-000072c0: 636d 6c2f 6d70 742d 3330 622d 696e 7374  cml/mpt-30b-inst
-000072d0: 7275 6374 5d28 6874 7470 733a 2f2f 6875  ruct](https://hu
-000072e0: 6767 696e 6766 6163 652e 636f 2f6d 6f73  ggingface.co/mos
-000072f0: 6169 636d 6c2f 6d70 742d 3330 622d 696e  aicml/mpt-30b-in
-00007300: 7374 7275 6374 290a 2d20 5b6d 6f73 6169  struct).- [mosai
-00007310: 636d 6c2f 6d70 742d 3330 622d 6368 6174  cml/mpt-30b-chat
-00007320: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00007330: 6766 6163 652e 636f 2f6d 6f73 6169 636d  gface.co/mosaicm
-00007340: 6c2f 6d70 742d 3330 622d 6368 6174 290a  l/mpt-30b-chat).
-00007350: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
-00007360: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
-00007370: 3e4f 5054 3c2f 7375 6d6d 6172 793e 0a0a  >OPT</summary>..
-00007380: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
-00007390: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 204f  ...> **Note:** O
-000073a0: 5054 2072 6571 7569 7265 7320 746f 2069  PT requires to i
-000073b0: 6e73 7461 6c6c 2077 6974 683a 0a3e 2060  nstall with:.> `
-000073c0: 6060 6261 7368 0a3e 2070 6970 2069 6e73  ``bash.> pip ins
-000073d0: 7461 6c6c 2022 6f70 656e 6c6c 6d5b 6f70  tall "openllm[op
-000073e0: 745d 220a 3e20 6060 600a 0a0a 5275 6e20  t]".> ```...Run 
-000073f0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00007400: 6d6d 616e 6420 746f 2071 7569 636b 6c79  mmand to quickly
-00007410: 2073 7069 6e20 7570 2061 204f 5054 2073   spin up a OPT s
-00007420: 6572 7665 723a 0a0a 6060 6062 6173 680a  erver:..```bash.
-00007430: 6f70 656e 6c6c 6d20 7374 6172 7420 6661  openllm start fa
-00007440: 6365 626f 6f6b 2f6f 7074 2d31 2e33 620a  cebook/opt-1.3b.
-00007450: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
-00007460: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
-00007470: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
-00007480: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
-00007490: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
-000074a0: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
-000074b0: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
-000074c0: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
-000074d0: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
-000074e0: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
-000074f0: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
-00007500: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
-00007510: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
-00007520: 204f 5054 2076 6172 6961 6e74 7320 6361   OPT variants ca
-00007530: 6e20 6265 2064 6570 6c6f 7965 6420 7769  n be deployed wi
-00007540: 7468 204f 7065 6e4c 4c4d 2e20 5669 7369  th OpenLLM. Visi
-00007550: 7420 7468 6520 5b48 7567 6769 6e67 4661  t the [HuggingFa
-00007560: 6365 204d 6f64 656c 2048 7562 5d28 6874  ce Model Hub](ht
-00007570: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00007580: 652e 636f 2f6d 6f64 656c 733f 736f 7274  e.co/models?sort
-00007590: 3d74 7265 6e64 696e 6726 7365 6172 6368  =trending&search
-000075a0: 3d6f 7074 2920 746f 2073 6565 206d 6f72  =opt) to see mor
-000075b0: 6520 4f50 542d 636f 6d70 6174 6962 6c65  e OPT-compatible
-000075c0: 206d 6f64 656c 732e 0a0a 0a0a 2323 2320   models.....### 
-000075d0: 5375 7070 6f72 7465 6420 6d6f 6465 6c73  Supported models
-000075e0: 0a0a 596f 7520 6361 6e20 7370 6563 6966  ..You can specif
-000075f0: 7920 616e 7920 6f66 2074 6865 2066 6f6c  y any of the fol
-00007600: 6c6f 7769 6e67 204f 5054 206d 6f64 656c  lowing OPT model
-00007610: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
-00007620: 7461 7274 603a 0a0a 0a2d 205b 6661 6365  tart`:...- [face
-00007630: 626f 6f6b 2f6f 7074 2d31 3235 6d5d 2868  book/opt-125m](h
-00007640: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00007650: 6365 2e63 6f2f 6661 6365 626f 6f6b 2f6f  ce.co/facebook/o
-00007660: 7074 2d31 3235 6d29 0a2d 205b 6661 6365  pt-125m).- [face
-00007670: 626f 6f6b 2f6f 7074 2d33 3530 6d5d 2868  book/opt-350m](h
-00007680: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00007690: 6365 2e63 6f2f 6661 6365 626f 6f6b 2f6f  ce.co/facebook/o
-000076a0: 7074 2d33 3530 6d29 0a2d 205b 6661 6365  pt-350m).- [face
-000076b0: 626f 6f6b 2f6f 7074 2d31 2e33 625d 2868  book/opt-1.3b](h
-000076c0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-000076d0: 6365 2e63 6f2f 6661 6365 626f 6f6b 2f6f  ce.co/facebook/o
-000076e0: 7074 2d31 2e33 6229 0a2d 205b 6661 6365  pt-1.3b).- [face
-000076f0: 626f 6f6b 2f6f 7074 2d32 2e37 625d 2868  book/opt-2.7b](h
-00007700: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00007710: 6365 2e63 6f2f 6661 6365 626f 6f6b 2f6f  ce.co/facebook/o
-00007720: 7074 2d32 2e37 6229 0a2d 205b 6661 6365  pt-2.7b).- [face
-00007730: 626f 6f6b 2f6f 7074 2d36 2e37 625d 2868  book/opt-6.7b](h
-00007740: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00007750: 6365 2e63 6f2f 6661 6365 626f 6f6b 2f6f  ce.co/facebook/o
-00007760: 7074 2d36 2e37 6229 0a2d 205b 6661 6365  pt-6.7b).- [face
-00007770: 626f 6f6b 2f6f 7074 2d36 3662 5d28 6874  book/opt-66b](ht
-00007780: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00007790: 652e 636f 2f66 6163 6562 6f6f 6b2f 6f70  e.co/facebook/op
-000077a0: 742d 3636 6229 0a0a 3c2f 6465 7461 696c  t-66b)..</detail
-000077b0: 733e 0a0a 3c64 6574 6169 6c73 3e0a 0a3c  s>..<details>..<
-000077c0: 7375 6d6d 6172 793e 5068 693c 2f73 756d  summary>Phi</sum
-000077d0: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
-000077e0: 6b73 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f  kstart....> **No
-000077f0: 7465 3a2a 2a20 5068 6920 7265 7175 6972  te:** Phi requir
-00007800: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
-00007810: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
-00007820: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
-00007830: 6e6c 6c6d 5b70 6869 5d22 0a3e 2060 6060  nllm[phi]".> ```
-00007840: 0a0a 0a52 756e 2074 6865 2066 6f6c 6c6f  ...Run the follo
-00007850: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
-00007860: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
-00007870: 6120 5068 6920 7365 7276 6572 3a0a 0a60  a Phi server:..`
-00007880: 6060 6261 7368 0a54 5255 5354 5f52 454d  ``bash.TRUST_REM
-00007890: 4f54 455f 434f 4445 3d54 7275 6520 6f70  OTE_CODE=True op
-000078a0: 656e 6c6c 6d20 7374 6172 7420 6d69 6372  enllm start micr
-000078b0: 6f73 6f66 742f 7068 692d 320a 6060 600a  osoft/phi-2.```.
-000078c0: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-000078d0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-000078e0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-000078f0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-00007900: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-00007910: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00007920: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00007930: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00007940: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00007950: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00007960: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00007970: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00007980: 2a4e 6f74 653a 2a2a 2041 6e79 2050 6869  *Note:** Any Phi
-00007990: 2076 6172 6961 6e74 7320 6361 6e20 6265   variants can be
-000079a0: 2064 6570 6c6f 7965 6420 7769 7468 204f   deployed with O
-000079b0: 7065 6e4c 4c4d 2e20 5669 7369 7420 7468  penLLM. Visit th
-000079c0: 6520 5b48 7567 6769 6e67 4661 6365 204d  e [HuggingFace M
-000079d0: 6f64 656c 2048 7562 5d28 6874 7470 733a  odel Hub](https:
-000079e0: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
-000079f0: 2f6d 6f64 656c 733f 736f 7274 3d74 7265  /models?sort=tre
-00007a00: 6e64 696e 6726 7365 6172 6368 3d70 6869  nding&search=phi
-00007a10: 2920 746f 2073 6565 206d 6f72 6520 5068  ) to see more Ph
-00007a20: 692d 636f 6d70 6174 6962 6c65 206d 6f64  i-compatible mod
-00007a30: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
-00007a40: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
-00007a50: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
-00007a60: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
-00007a70: 6e67 2050 6869 206d 6f64 656c 7320 7669  ng Phi models vi
-00007a80: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
-00007a90: 603a 0a0a 0a2d 205b 6d69 6372 6f73 6f66  `:...- [microsof
-00007aa0: 742f 7068 692d 325d 2868 7474 7073 3a2f  t/phi-2](https:/
-00007ab0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00007ac0: 6d69 6372 6f73 6f66 742f 7068 692d 3229  microsoft/phi-2)
-00007ad0: 0a2d 205b 6d69 6372 6f73 6f66 742f 7068  .- [microsoft/ph
-00007ae0: 692d 315f 355d 2868 7474 7073 3a2f 2f68  i-1_5](https://h
-00007af0: 7567 6769 6e67 6661 6365 2e63 6f2f 6d69  uggingface.co/mi
-00007b00: 6372 6f73 6f66 742f 7068 692d 315f 3529  crosoft/phi-1_5)
-00007b10: 0a0a 3c2f 6465 7461 696c 733e 0a0a 3c64  ..</details>..<d
-00007b20: 6574 6169 6c73 3e0a 0a3c 7375 6d6d 6172  etails>..<summar
-00007b30: 793e 5177 656e 3c2f 7375 6d6d 6172 793e  y>Qwen</summary>
-00007b40: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
-00007b50: 740a 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  t....> **Note:**
-00007b60: 2051 7765 6e20 7265 7175 6972 6573 2074   Qwen requires t
-00007b70: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
-00007b80: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
-00007b90: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
-00007ba0: 5b71 7765 6e5d 220a 3e20 6060 600a 0a0a  [qwen]".> ```...
-00007bb0: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
-00007bc0: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
-00007bd0: 636b 6c79 2073 7069 6e20 7570 2061 2051  ckly spin up a Q
-00007be0: 7765 6e20 7365 7276 6572 3a0a 0a60 6060  wen server:..```
-00007bf0: 6261 7368 0a54 5255 5354 5f52 454d 4f54  bash.TRUST_REMOT
-00007c00: 455f 434f 4445 3d54 7275 6520 6f70 656e  E_CODE=True open
-00007c10: 6c6c 6d20 7374 6172 7420 7177 656e 2f51  llm start qwen/Q
-00007c20: 7765 6e2d 3742 2d43 6861 740a 6060 600a  wen-7B-Chat.```.
-00007c30: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-00007c40: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-00007c50: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-00007c60: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-00007c70: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-00007c80: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00007c90: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00007ca0: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00007cb0: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00007cc0: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00007cd0: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00007ce0: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00007cf0: 2a4e 6f74 653a 2a2a 2041 6e79 2051 7765  *Note:** Any Qwe
-00007d00: 6e20 7661 7269 616e 7473 2063 616e 2062  n variants can b
-00007d10: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
-00007d20: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
-00007d30: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
-00007d40: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
-00007d50: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00007d60: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
-00007d70: 656e 6469 6e67 2673 6561 7263 683d 7177  ending&search=qw
-00007d80: 656e 2920 746f 2073 6565 206d 6f72 6520  en) to see more 
-00007d90: 5177 656e 2d63 6f6d 7061 7469 626c 6520  Qwen-compatible 
-00007da0: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
-00007db0: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
-00007dc0: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
-00007dd0: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
-00007de0: 6f77 696e 6720 5177 656e 206d 6f64 656c  owing Qwen model
-00007df0: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
-00007e00: 7461 7274 603a 0a0a 0a2d 205b 7177 656e  tart`:...- [qwen
-00007e10: 2f51 7765 6e2d 3742 2d43 6861 745d 2868  /Qwen-7B-Chat](h
-00007e20: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00007e30: 6365 2e63 6f2f 7177 656e 2f51 7765 6e2d  ce.co/qwen/Qwen-
-00007e40: 3742 2d43 6861 7429 0a2d 205b 7177 656e  7B-Chat).- [qwen
-00007e50: 2f51 7765 6e2d 3742 2d43 6861 742d 496e  /Qwen-7B-Chat-In
-00007e60: 7438 5d28 6874 7470 733a 2f2f 6875 6767  t8](https://hugg
-00007e70: 696e 6766 6163 652e 636f 2f71 7765 6e2f  ingface.co/qwen/
-00007e80: 5177 656e 2d37 422d 4368 6174 2d49 6e74  Qwen-7B-Chat-Int
-00007e90: 3829 0a2d 205b 7177 656e 2f51 7765 6e2d  8).- [qwen/Qwen-
-00007ea0: 3742 2d43 6861 742d 496e 7434 5d28 6874  7B-Chat-Int4](ht
-00007eb0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
-00007ec0: 652e 636f 2f71 7765 6e2f 5177 656e 2d37  e.co/qwen/Qwen-7
-00007ed0: 422d 4368 6174 2d49 6e74 3429 0a2d 205b  B-Chat-Int4).- [
-00007ee0: 7177 656e 2f51 7765 6e2d 3134 422d 4368  qwen/Qwen-14B-Ch
-00007ef0: 6174 5d28 6874 7470 733a 2f2f 6875 6767  at](https://hugg
-00007f00: 696e 6766 6163 652e 636f 2f71 7765 6e2f  ingface.co/qwen/
-00007f10: 5177 656e 2d31 3442 2d43 6861 7429 0a2d  Qwen-14B-Chat).-
-00007f20: 205b 7177 656e 2f51 7765 6e2d 3134 422d   [qwen/Qwen-14B-
-00007f30: 4368 6174 2d49 6e74 385d 2868 7474 7073  Chat-Int8](https
-00007f40: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
-00007f50: 6f2f 7177 656e 2f51 7765 6e2d 3134 422d  o/qwen/Qwen-14B-
-00007f60: 4368 6174 2d49 6e74 3829 0a2d 205b 7177  Chat-Int8).- [qw
-00007f70: 656e 2f51 7765 6e2d 3134 422d 4368 6174  en/Qwen-14B-Chat
-00007f80: 2d49 6e74 345d 2868 7474 7073 3a2f 2f68  -Int4](https://h
-00007f90: 7567 6769 6e67 6661 6365 2e63 6f2f 7177  uggingface.co/qw
-00007fa0: 656e 2f51 7765 6e2d 3134 422d 4368 6174  en/Qwen-14B-Chat
-00007fb0: 2d49 6e74 3429 0a0a 3c2f 6465 7461 696c  -Int4)..</detail
-00007fc0: 733e 0a0a 3c64 6574 6169 6c73 3e0a 0a3c  s>..<details>..<
-00007fd0: 7375 6d6d 6172 793e 5374 6162 6c65 4c4d  summary>StableLM
-00007fe0: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
-00007ff0: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
-00008000: 202a 2a4e 6f74 653a 2a2a 2053 7461 626c   **Note:** Stabl
-00008010: 654c 4d20 7265 7175 6972 6573 2074 6f20  eLM requires to 
-00008020: 696e 7374 616c 6c20 7769 7468 3a0a 3e20  install with:.> 
-00008030: 6060 6062 6173 680a 3e20 7069 7020 696e  ```bash.> pip in
-00008040: 7374 616c 6c20 226f 7065 6e6c 6c6d 5b73  stall "openllm[s
-00008050: 7461 626c 656c 6d5d 220a 3e20 6060 600a  tablelm]".> ```.
-00008060: 0a0a 5275 6e20 7468 6520 666f 6c6c 6f77  ..Run the follow
-00008070: 696e 6720 636f 6d6d 616e 6420 746f 2071  ing command to q
-00008080: 7569 636b 6c79 2073 7069 6e20 7570 2061  uickly spin up a
-00008090: 2053 7461 626c 654c 4d20 7365 7276 6572   StableLM server
-000080a0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
-000080b0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
-000080c0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
-000080d0: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
-000080e0: 6c65 6c6d 2d74 756e 6564 2d61 6c70 6861  lelm-tuned-alpha
-000080f0: 2d33 620a 6060 600a 496e 2061 2064 6966  -3b.```.In a dif
-00008100: 6665 7265 6e74 2074 6572 6d69 6e61 6c2c  ferent terminal,
-00008110: 2072 756e 2074 6865 2066 6f6c 6c6f 7769   run the followi
-00008120: 6e67 2063 6f6d 6d61 6e64 2074 6f20 696e  ng command to in
-00008130: 7465 7261 6374 2077 6974 6820 7468 6520  teract with the 
-00008140: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
-00008150: 0a65 7870 6f72 7420 4f50 454e 4c4c 4d5f  .export OPENLLM_
-00008160: 454e 4450 4f49 4e54 3d68 7474 703a 2f2f  ENDPOINT=http://
-00008170: 6c6f 6361 6c68 6f73 743a 3330 3030 0a6f  localhost:3000.o
-00008180: 7065 6e6c 6c6d 2071 7565 7279 2027 5768  penllm query 'Wh
-00008190: 6174 2061 7265 206c 6172 6765 206c 616e  at are large lan
-000081a0: 6775 6167 6520 6d6f 6465 6c73 3f27 0a60  guage models?'.`
-000081b0: 6060 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  ``...> **Note:**
-000081c0: 2041 6e79 2053 7461 626c 654c 4d20 7661   Any StableLM va
-000081d0: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
-000081e0: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
-000081f0: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
-00008200: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
-00008210: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
-00008220: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
-00008230: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
-00008240: 6e67 2673 6561 7263 683d 7374 6162 6c65  ng&search=stable
-00008250: 6c6d 2920 746f 2073 6565 206d 6f72 6520  lm) to see more 
-00008260: 5374 6162 6c65 4c4d 2d63 6f6d 7061 7469  StableLM-compati
-00008270: 626c 6520 6d6f 6465 6c73 2e0a 0a0a 0a23  ble models.....#
-00008280: 2323 2053 7570 706f 7274 6564 206d 6f64  ## Supported mod
-00008290: 656c 730a 0a59 6f75 2063 616e 2073 7065  els..You can spe
-000082a0: 6369 6679 2061 6e79 206f 6620 7468 6520  cify any of the 
-000082b0: 666f 6c6c 6f77 696e 6720 5374 6162 6c65  following Stable
-000082c0: 4c4d 206d 6f64 656c 7320 7669 6120 606f  LM models via `o
-000082d0: 7065 6e6c 6c6d 2073 7461 7274 603a 0a0a  penllm start`:..
-000082e0: 0a2d 205b 7374 6162 696c 6974 7961 692f  .- [stabilityai/
-000082f0: 7374 6162 6c65 6c6d 2d74 756e 6564 2d61  stablelm-tuned-a
-00008300: 6c70 6861 2d33 625d 2868 7474 7073 3a2f  lpha-3b](https:/
-00008310: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00008320: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
-00008330: 6c65 6c6d 2d74 756e 6564 2d61 6c70 6861  lelm-tuned-alpha
-00008340: 2d33 6229 0a2d 205b 7374 6162 696c 6974  -3b).- [stabilit
-00008350: 7961 692f 7374 6162 6c65 6c6d 2d74 756e  yai/stablelm-tun
-00008360: 6564 2d61 6c70 6861 2d37 625d 2868 7474  ed-alpha-7b](htt
-00008370: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
-00008380: 2e63 6f2f 7374 6162 696c 6974 7961 692f  .co/stabilityai/
-00008390: 7374 6162 6c65 6c6d 2d74 756e 6564 2d61  stablelm-tuned-a
-000083a0: 6c70 6861 2d37 6229 0a2d 205b 7374 6162  lpha-7b).- [stab
-000083b0: 696c 6974 7961 692f 7374 6162 6c65 6c6d  ilityai/stablelm
-000083c0: 2d62 6173 652d 616c 7068 612d 3362 5d28  -base-alpha-3b](
-000083d0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-000083e0: 6163 652e 636f 2f73 7461 6269 6c69 7479  ace.co/stability
-000083f0: 6169 2f73 7461 626c 656c 6d2d 6261 7365  ai/stablelm-base
-00008400: 2d61 6c70 6861 2d33 6229 0a2d 205b 7374  -alpha-3b).- [st
-00008410: 6162 696c 6974 7961 692f 7374 6162 6c65  abilityai/stable
-00008420: 6c6d 2d62 6173 652d 616c 7068 612d 3762  lm-base-alpha-7b
-00008430: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
-00008440: 6766 6163 652e 636f 2f73 7461 6269 6c69  gface.co/stabili
-00008450: 7479 6169 2f73 7461 626c 656c 6d2d 6261  tyai/stablelm-ba
-00008460: 7365 2d61 6c70 6861 2d37 6229 0a0a 3c2f  se-alpha-7b)..</
-00008470: 6465 7461 696c 733e 0a0a 3c64 6574 6169  details>..<detai
-00008480: 6c73 3e0a 0a3c 7375 6d6d 6172 793e 5374  ls>..<summary>St
-00008490: 6172 436f 6465 723c 2f73 756d 6d61 7279  arCoder</summary
-000084a0: 3e0a 0a0a 2323 2320 5175 6963 6b73 7461  >...### Quicksta
-000084b0: 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465 3a2a  rt....> **Note:*
-000084c0: 2a20 5374 6172 436f 6465 7220 7265 7175  * StarCoder requ
-000084d0: 6972 6573 2074 6f20 696e 7374 616c 6c20  ires to install 
-000084e0: 7769 7468 3a0a 3e20 6060 6062 6173 680a  with:.> ```bash.
-000084f0: 3e20 7069 7020 696e 7374 616c 6c20 226f  > pip install "o
-00008500: 7065 6e6c 6c6d 5b73 7461 7263 6f64 6572  penllm[starcoder
-00008510: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
-00008520: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
-00008530: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
-00008540: 7370 696e 2075 7020 6120 5374 6172 436f  spin up a StarCo
-00008550: 6465 7220 7365 7276 6572 3a0a 0a60 6060  der server:..```
-00008560: 6261 7368 0a54 5255 5354 5f52 454d 4f54  bash.TRUST_REMOT
-00008570: 455f 434f 4445 3d54 7275 6520 6f70 656e  E_CODE=True open
-00008580: 6c6c 6d20 7374 6172 7420 6269 6763 6f64  llm start bigcod
-00008590: 652f 7374 6172 636f 6465 720a 6060 600a  e/starcoder.```.
-000085a0: 496e 2061 2064 6966 6665 7265 6e74 2074  In a different t
-000085b0: 6572 6d69 6e61 6c2c 2072 756e 2074 6865  erminal, run the
-000085c0: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
-000085d0: 6e64 2074 6f20 696e 7465 7261 6374 2077  nd to interact w
-000085e0: 6974 6820 7468 6520 7365 7276 6572 3a0a  ith the server:.
-000085f0: 0a60 6060 6261 7368 0a65 7870 6f72 7420  .```bash.export 
-00008600: 4f50 454e 4c4c 4d5f 454e 4450 4f49 4e54  OPENLLM_ENDPOINT
-00008610: 3d68 7474 703a 2f2f 6c6f 6361 6c68 6f73  =http://localhos
-00008620: 743a 3330 3030 0a6f 7065 6e6c 6c6d 2071  t:3000.openllm q
-00008630: 7565 7279 2027 5768 6174 2061 7265 206c  uery 'What are l
-00008640: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00008650: 6465 6c73 3f27 0a60 6060 0a0a 0a3e 202a  dels?'.```...> *
-00008660: 2a4e 6f74 653a 2a2a 2041 6e79 2053 7461  *Note:** Any Sta
-00008670: 7243 6f64 6572 2076 6172 6961 6e74 7320  rCoder variants 
-00008680: 6361 6e20 6265 2064 6570 6c6f 7965 6420  can be deployed 
-00008690: 7769 7468 204f 7065 6e4c 4c4d 2e20 5669  with OpenLLM. Vi
-000086a0: 7369 7420 7468 6520 5b48 7567 6769 6e67  sit the [Hugging
-000086b0: 4661 6365 204d 6f64 656c 2048 7562 5d28  Face Model Hub](
-000086c0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
-000086d0: 6163 652e 636f 2f6d 6f64 656c 733f 736f  ace.co/models?so
-000086e0: 7274 3d74 7265 6e64 696e 6726 7365 6172  rt=trending&sear
-000086f0: 6368 3d73 7461 7263 6f64 6572 2920 746f  ch=starcoder) to
-00008700: 2073 6565 206d 6f72 6520 5374 6172 436f   see more StarCo
-00008710: 6465 722d 636f 6d70 6174 6962 6c65 206d  der-compatible m
-00008720: 6f64 656c 732e 0a0a 0a0a 2323 2320 5375  odels.....### Su
-00008730: 7070 6f72 7465 6420 6d6f 6465 6c73 0a0a  pported models..
-00008740: 596f 7520 6361 6e20 7370 6563 6966 7920  You can specify 
-00008750: 616e 7920 6f66 2074 6865 2066 6f6c 6c6f  any of the follo
-00008760: 7769 6e67 2053 7461 7243 6f64 6572 206d  wing StarCoder m
-00008770: 6f64 656c 7320 7669 6120 606f 7065 6e6c  odels via `openl
-00008780: 6c6d 2073 7461 7274 603a 0a0a 0a2d 205b  lm start`:...- [
-00008790: 6269 6763 6f64 652f 7374 6172 636f 6465  bigcode/starcode
-000087a0: 725d 2868 7474 7073 3a2f 2f68 7567 6769  r](https://huggi
-000087b0: 6e67 6661 6365 2e63 6f2f 6269 6763 6f64  ngface.co/bigcod
-000087c0: 652f 7374 6172 636f 6465 7229 0a2d 205b  e/starcoder).- [
-000087d0: 6269 6763 6f64 652f 7374 6172 636f 6465  bigcode/starcode
-000087e0: 7262 6173 655d 2868 7474 7073 3a2f 2f68  rbase](https://h
-000087f0: 7567 6769 6e67 6661 6365 2e63 6f2f 6269  uggingface.co/bi
-00008800: 6763 6f64 652f 7374 6172 636f 6465 7262  gcode/starcoderb
-00008810: 6173 6529 0a0a 3c2f 6465 7461 696c 733e  ase)..</details>
-00008820: 0a0a 3c64 6574 6169 6c73 3e0a 0a3c 7375  ..<details>..<su
-00008830: 6d6d 6172 793e 5969 3c2f 7375 6d6d 6172  mmary>Yi</summar
-00008840: 793e 0a0a 0a23 2323 2051 7569 636b 7374  y>...### Quickst
-00008850: 6172 740a 0a0a 0a3e 202a 2a4e 6f74 653a  art....> **Note:
-00008860: 2a2a 2059 6920 7265 7175 6972 6573 2074  ** Yi requires t
-00008870: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
-00008880: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
-00008890: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
-000088a0: 5b79 695d 220a 3e20 6060 600a 0a0a 5275  [yi]".> ```...Ru
-000088b0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
-000088c0: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
-000088d0: 6c79 2073 7069 6e20 7570 2061 2059 6920  ly spin up a Yi 
-000088e0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
-000088f0: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
-00008900: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
-00008910: 7374 6172 7420 3031 2d61 692f 5969 2d36  start 01-ai/Yi-6
-00008920: 420a 6060 600a 496e 2061 2064 6966 6665  B.```.In a diffe
-00008930: 7265 6e74 2074 6572 6d69 6e61 6c2c 2072  rent terminal, r
-00008940: 756e 2074 6865 2066 6f6c 6c6f 7769 6e67  un the following
-00008950: 2063 6f6d 6d61 6e64 2074 6f20 696e 7465   command to inte
-00008960: 7261 6374 2077 6974 6820 7468 6520 7365  ract with the se
-00008970: 7276 6572 3a0a 0a60 6060 6261 7368 0a65  rver:..```bash.e
-00008980: 7870 6f72 7420 4f50 454e 4c4c 4d5f 454e  xport OPENLLM_EN
-00008990: 4450 4f49 4e54 3d68 7474 703a 2f2f 6c6f  DPOINT=http://lo
-000089a0: 6361 6c68 6f73 743a 3330 3030 0a6f 7065  calhost:3000.ope
-000089b0: 6e6c 6c6d 2071 7565 7279 2027 5768 6174  nllm query 'What
-000089c0: 2061 7265 206c 6172 6765 206c 616e 6775   are large langu
-000089d0: 6167 6520 6d6f 6465 6c73 3f27 0a60 6060  age models?'.```
-000089e0: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2041  ...> **Note:** A
-000089f0: 6e79 2059 6920 7661 7269 616e 7473 2063  ny Yi variants c
-00008a00: 616e 2062 6520 6465 706c 6f79 6564 2077  an be deployed w
-00008a10: 6974 6820 4f70 656e 4c4c 4d2e 2056 6973  ith OpenLLM. Vis
-00008a20: 6974 2074 6865 205b 4875 6767 696e 6746  it the [HuggingF
-00008a30: 6163 6520 4d6f 6465 6c20 4875 625d 2868  ace Model Hub](h
-00008a40: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
-00008a50: 6365 2e63 6f2f 6d6f 6465 6c73 3f73 6f72  ce.co/models?sor
-00008a60: 743d 7472 656e 6469 6e67 2673 6561 7263  t=trending&searc
-00008a70: 683d 7969 2920 746f 2073 6565 206d 6f72  h=yi) to see mor
-00008a80: 6520 5969 2d63 6f6d 7061 7469 626c 6520  e Yi-compatible 
-00008a90: 6d6f 6465 6c73 2e0a 0a0a 0a23 2323 2053  models.....### S
-00008aa0: 7570 706f 7274 6564 206d 6f64 656c 730a  upported models.
-00008ab0: 0a59 6f75 2063 616e 2073 7065 6369 6679  .You can specify
-00008ac0: 2061 6e79 206f 6620 7468 6520 666f 6c6c   any of the foll
-00008ad0: 6f77 696e 6720 5969 206d 6f64 656c 7320  owing Yi models 
-00008ae0: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
-00008af0: 7274 603a 0a0a 0a2d 205b 3031 2d61 692f  rt`:...- [01-ai/
-00008b00: 5969 2d36 425d 2868 7474 7073 3a2f 2f68  Yi-6B](https://h
-00008b10: 7567 6769 6e67 6661 6365 2e63 6f2f 3031  uggingface.co/01
-00008b20: 2d61 692f 5969 2d36 4229 0a2d 205b 3031  -ai/Yi-6B).- [01
-00008b30: 2d61 692f 5969 2d33 3442 5d28 6874 7470  -ai/Yi-34B](http
-00008b40: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00008b50: 636f 2f30 312d 6169 2f59 692d 3334 4229  co/01-ai/Yi-34B)
-00008b60: 0a2d 205b 3031 2d61 692f 5969 2d36 422d  .- [01-ai/Yi-6B-
-00008b70: 3230 304b 5d28 6874 7470 733a 2f2f 6875  200K](https://hu
-00008b80: 6767 696e 6766 6163 652e 636f 2f30 312d  ggingface.co/01-
-00008b90: 6169 2f59 692d 3642 2d32 3030 4b29 0a2d  ai/Yi-6B-200K).-
-00008ba0: 205b 3031 2d61 692f 5969 2d33 3442 2d32   [01-ai/Yi-34B-2
-00008bb0: 3030 4b5d 2868 7474 7073 3a2f 2f68 7567  00K](https://hug
-00008bc0: 6769 6e67 6661 6365 2e63 6f2f 3031 2d61  gingface.co/01-a
-00008bd0: 692f 5969 2d33 3442 2d32 3030 4b29 0a0a  i/Yi-34B-200K)..
-00008be0: 3c2f 6465 7461 696c 733e 0a0a 3c21 2d2d  </details>..<!--
-00008bf0: 2075 7064 6174 652d 7265 6164 6d65 2e70   update-readme.p
-00008c00: 793a 2073 746f 7020 2d2d 3e0a 0a4d 6f72  y: stop -->..Mor
-00008c10: 6520 6d6f 6465 6c73 2077 696c 6c20 6265  e models will be
-00008c20: 2069 6e74 6567 7261 7465 6420 7769 7468   integrated with
-00008c30: 204f 7065 6e4c 4c4d 2061 6e64 2077 6520   OpenLLM and we 
-00008c40: 7765 6c63 6f6d 6520 796f 7572 2063 6f6e  welcome your con
-00008c50: 7472 6962 7574 696f 6e73 2069 6620 796f  tributions if yo
-00008c60: 7520 7761 6e74 2074 6f20 696e 636f 7270  u want to incorp
-00008c70: 6f72 6174 6520 796f 7572 2063 7573 746f  orate your custo
-00008c80: 6d20 4c4c 4d73 2069 6e74 6f20 7468 6520  m LLMs into the 
-00008c90: 6563 6f73 7973 7465 6d2e 2043 6865 636b  ecosystem. Check
-00008ca0: 206f 7574 205b 4164 6469 6e67 2061 204e   out [Adding a N
-00008cb0: 6577 204d 6f64 656c 2047 7569 6465 5d28  ew Model Guide](
-00008cc0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00008cd0: 6f6d 2f62 656e 746f 6d6c 2f4f 7065 6e4c  om/bentoml/OpenL
-00008ce0: 4c4d 2f62 6c6f 622f 6d61 696e 2f41 4444  LM/blob/main/ADD
-00008cf0: 494e 475f 4e45 575f 4d4f 4445 4c2e 6d64  ING_NEW_MODEL.md
-00008d00: 2920 746f 206c 6561 726e 206d 6f72 652e  ) to learn more.
-00008d10: 0a0a 2323 20f0 9f92 bb20 5275 6e20 796f  ..## .... Run yo
-00008d20: 7572 206d 6f64 656c 206f 6e20 6d75 6c74  ur model on mult
-00008d30: 6970 6c65 2047 5055 730a 0a4f 7065 6e4c  iple GPUs..OpenL
-00008d40: 4c4d 2061 6c6c 6f77 7320 796f 7520 746f  LM allows you to
-00008d50: 2073 7461 7274 2079 6f75 7220 6d6f 6465   start your mode
-00008d60: 6c20 7365 7276 6572 206f 6e20 6d75 6c74  l server on mult
-00008d70: 6970 6c65 2047 5055 7320 616e 6420 7370  iple GPUs and sp
-00008d80: 6563 6966 7920 7468 6520 6e75 6d62 6572  ecify the number
-00008d90: 206f 6620 776f 726b 6572 7320 7065 7220   of workers per 
-00008da0: 7265 736f 7572 6365 2061 7373 6967 6e65  resource assigne
-00008db0: 6420 7573 696e 6720 7468 6520 602d 2d77  d using the `--w
-00008dc0: 6f72 6b65 7273 2d70 6572 2d72 6573 6f75  orkers-per-resou
-00008dd0: 7263 6560 206f 7074 696f 6e2e 2046 6f72  rce` option. For
-00008de0: 2065 7861 6d70 6c65 2c20 6966 2079 6f75   example, if you
-00008df0: 2068 6176 6520 3420 6176 6169 6c61 626c   have 4 availabl
-00008e00: 6520 4750 5573 2c20 796f 7520 7365 7420  e GPUs, you set 
-00008e10: 7468 6520 7661 6c75 6520 6173 206f 6e65  the value as one
-00008e20: 2064 6976 6964 6564 2062 7920 7468 6520   divided by the 
-00008e30: 6e75 6d62 6572 2061 7320 6f6e 6c79 206f  number as only o
-00008e40: 6e65 2069 6e73 7461 6e63 6520 6f66 2074  ne instance of t
-00008e50: 6865 2052 756e 6e65 7220 7365 7276 6572  he Runner server
-00008e60: 2077 696c 6c20 6265 2073 7061 776e 6564   will be spawned
-00008e70: 2e0a 0a60 6060 6261 7368 0a54 5255 5354  ...```bash.TRUST
-00008e80: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
-00008e90: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
-00008ea0: 6d69 6372 6f73 6f66 742f 7068 692d 3220  microsoft/phi-2 
-00008eb0: 2d2d 776f 726b 6572 732d 7065 722d 7265  --workers-per-re
-00008ec0: 736f 7572 6365 2030 2e32 350a 6060 600a  source 0.25.```.
-00008ed0: 0a3e 205b 214e 4f54 455d 0a3e 2054 6865  .> [!NOTE].> The
-00008ee0: 2061 6d6f 756e 7420 6f66 2047 5055 7320   amount of GPUs 
-00008ef0: 7265 7175 6972 6564 2064 6570 656e 6473  required depends
-00008f00: 206f 6e20 7468 6520 6d6f 6465 6c20 7369   on the model si
-00008f10: 7a65 2069 7473 656c 662e 0a3e 2059 6f75  ze itself..> You
-00008f20: 2063 616e 2075 7365 205b 7468 6520 4d6f   can use [the Mo
-00008f30: 6465 6c20 4d65 6d6f 7279 2043 616c 6375  del Memory Calcu
-00008f40: 6c61 746f 7220 6672 6f6d 2048 7567 6769  lator from Huggi
-00008f50: 6e67 2046 6163 655d 2868 7474 7073 3a2f  ng Face](https:/
-00008f60: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
-00008f70: 7370 6163 6573 2f68 662d 6163 6365 6c65  spaces/hf-accele
-00008f80: 7261 7465 2f6d 6f64 656c 2d6d 656d 6f72  rate/model-memor
-00008f90: 792d 7573 6167 6529 2074 6f0a 3e20 6361  y-usage) to.> ca
-00008fa0: 6c63 756c 6174 6520 686f 7720 6d75 6368  lculate how much
-00008fb0: 2076 5241 4d20 6973 206e 6565 6465 6420   vRAM is needed 
-00008fc0: 746f 2074 7261 696e 2061 6e64 2070 6572  to train and per
-00008fd0: 666f 726d 2062 6967 206d 6f64 656c 0a3e  form big model.>
-00008fe0: 2069 6e66 6572 656e 6365 206f 6e20 6120   inference on a 
-00008ff0: 6d6f 6465 6c20 616e 6420 7468 656e 2070  model and then p
-00009000: 6c61 6e20 796f 7572 2047 5055 2073 7472  lan your GPU str
-00009010: 6174 6567 7920 6261 7365 6420 6f6e 2069  ategy based on i
-00009020: 742e 0a0a 5768 656e 2075 7369 6e67 2074  t...When using t
-00009030: 6865 2060 2d2d 776f 726b 6572 732d 7065  he `--workers-pe
-00009040: 722d 7265 736f 7572 6365 6020 6f70 7469  r-resource` opti
-00009050: 6f6e 2077 6974 6820 7468 6520 606f 7065  on with the `ope
-00009060: 6e6c 6c6d 2062 7569 6c64 6020 636f 6d6d  nllm build` comm
-00009070: 616e 642c 2074 6865 2065 6e76 6972 6f6e  and, the environ
-00009080: 6d65 6e74 2076 6172 6961 626c 6520 6973  ment variable is
-00009090: 2073 6176 6564 2069 6e74 6f20 7468 6520   saved into the 
-000090a0: 7265 7375 6c74 696e 6720 4265 6e74 6f2e  resulting Bento.
-000090b0: 0a0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
-000090c0: 6d61 7469 6f6e 2c20 7365 6520 5b52 6573  mation, see [Res
-000090d0: 6f75 7263 6520 7363 6865 6475 6c69 6e67  ource scheduling
-000090e0: 2073 7472 6174 6567 795d 2868 7474 7073   strategy](https
-000090f0: 3a2f 2f64 6f63 732e 6265 6e74 6f6d 6c2e  ://docs.bentoml.
-00009100: 6f72 672f 656e 2f6c 6174 6573 742f 6775  org/en/latest/gu
-00009110: 6964 6573 2f73 6368 6564 756c 696e 672e  ides/scheduling.
-00009120: 6874 6d6c 2329 2e0a 0a23 2320 f09f 9b9e  html#)...## ....
-00009130: 2052 756e 7469 6d65 2069 6d70 6c65 6d65   Runtime impleme
-00009140: 6e74 6174 696f 6e73 0a0a 4469 6666 6572  ntations..Differ
-00009150: 656e 7420 4c4c 4d73 206d 6179 2073 7570  ent LLMs may sup
-00009160: 706f 7274 206d 756c 7469 706c 6520 7275  port multiple ru
-00009170: 6e74 696d 6520 696d 706c 656d 656e 7461  ntime implementa
-00009180: 7469 6f6e 732e 204d 6f64 656c 7320 7468  tions. Models th
-00009190: 6174 2068 6176 6520 6076 4c4c 4d60 2028  at have `vLLM` (
-000091a0: 6076 6c6c 6d60 2920 7375 7070 6f72 7473  `vllm`) supports
-000091b0: 2077 696c 6c20 7573 6520 764c 4c4d 2062   will use vLLM b
-000091c0: 7920 6465 6661 756c 742c 206f 7468 6572  y default, other
-000091d0: 7769 7365 2069 7420 6661 6c6c 6261 636b  wise it fallback
-000091e0: 2074 6f20 7573 6520 6050 7954 6f72 6368   to use `PyTorch
-000091f0: 6020 2860 7074 6029 2e0a 0a54 6f20 7370  ` (`pt`)...To sp
-00009200: 6563 6966 7920 6120 7370 6563 6966 6963  ecify a specific
-00009210: 2072 756e 7469 6d65 2066 6f72 2079 6f75   runtime for you
-00009220: 7220 6368 6f73 656e 206d 6f64 656c 2c20  r chosen model, 
-00009230: 7573 6520 7468 6520 602d 2d62 6163 6b65  use the `--backe
-00009240: 6e64 6020 6f70 7469 6f6e 2e20 466f 7220  nd` option. For 
-00009250: 6578 616d 706c 653a 0a0a 6060 6062 6173  example:..```bas
-00009260: 680a 6f70 656e 6c6c 6d20 7374 6172 7420  h.openllm start 
-00009270: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
-00009280: 2d32 2d37 622d 6368 6174 2d68 6620 2d2d  -2-7b-chat-hf --
-00009290: 6261 636b 656e 6420 766c 6c6d 0a60 6060  backend vllm.```
-000092a0: 0a0a 4e6f 7465 3a0a 0a31 2e20 546f 2075  ..Note:..1. To u
-000092b0: 7365 2074 6865 2076 4c4c 4d20 6261 636b  se the vLLM back
-000092c0: 656e 642c 2079 6f75 206e 6565 6420 6120  end, you need a 
-000092d0: 4750 5520 7769 7468 2061 7420 6c65 6173  GPU with at leas
-000092e0: 7420 7468 6520 416d 7065 7265 2061 7263  t the Ampere arc
-000092f0: 6869 7465 6374 7572 6520 6f72 206e 6577  hitecture or new
-00009300: 6572 2061 6e64 2043 5544 4120 7665 7273  er and CUDA vers
-00009310: 696f 6e20 3131 2e38 2e0a 322e 2054 6f20  ion 11.8..2. To 
-00009320: 7365 6520 7468 6520 6261 636b 656e 6420  see the backend 
-00009330: 6f70 7469 6f6e 7320 6f66 2065 6163 6820  options of each 
-00009340: 6d6f 6465 6c20 7375 7070 6f72 7465 6420  model supported 
-00009350: 6279 204f 7065 6e4c 4c4d 2c20 7365 6520  by OpenLLM, see 
-00009360: 7468 6520 5375 7070 6f72 7465 6420 6d6f  the Supported mo
-00009370: 6465 6c73 2073 6563 7469 6f6e 206f 7220  dels section or 
-00009380: 7275 6e20 606f 7065 6e6c 6c6d 206d 6f64  run `openllm mod
-00009390: 656c 7360 2e0a 0a23 2320 f09f 9390 2051  els`...## .... Q
-000093a0: 7561 6e74 697a 6174 696f 6e0a 0a51 7561  uantization..Qua
-000093b0: 6e74 697a 6174 696f 6e20 6973 2061 2074  ntization is a t
-000093c0: 6563 686e 6971 7565 2074 6f20 7265 6475  echnique to redu
-000093d0: 6365 2074 6865 2073 746f 7261 6765 2061  ce the storage a
-000093e0: 6e64 2063 6f6d 7075 7461 7469 6f6e 2072  nd computation r
-000093f0: 6571 7569 7265 6d65 6e74 7320 666f 7220  equirements for 
-00009400: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
-00009410: 206d 6f64 656c 732c 2070 6172 7469 6375   models, particu
-00009420: 6c61 726c 7920 6475 7269 6e67 2069 6e66  larly during inf
-00009430: 6572 656e 6365 2e20 4279 2061 7070 726f  erence. By appro
-00009440: 7869 6d61 7469 6e67 2066 6c6f 6174 696e  ximating floatin
-00009450: 672d 706f 696e 7420 6e75 6d62 6572 7320  g-point numbers 
-00009460: 6173 2069 6e74 6567 6572 7320 2871 7561  as integers (qua
-00009470: 6e74 697a 6564 2076 616c 7565 7329 2c20  ntized values), 
-00009480: 7175 616e 7469 7a61 7469 6f6e 2061 6c6c  quantization all
-00009490: 6f77 7320 666f 7220 6661 7374 6572 2063  ows for faster c
-000094a0: 6f6d 7075 7461 7469 6f6e 732c 2072 6564  omputations, red
-000094b0: 7563 6564 206d 656d 6f72 7920 666f 6f74  uced memory foot
-000094c0: 7072 696e 742c 2061 6e64 2063 616e 206d  print, and can m
-000094d0: 616b 6520 6974 2066 6561 7369 626c 6520  ake it feasible 
-000094e0: 746f 2064 6570 6c6f 7920 6c61 7267 6520  to deploy large 
-000094f0: 6d6f 6465 6c73 206f 6e20 7265 736f 7572  models on resour
-00009500: 6365 2d63 6f6e 7374 7261 696e 6564 2064  ce-constrained d
-00009510: 6576 6963 6573 2e0a 0a4f 7065 6e4c 4c4d  evices...OpenLLM
-00009520: 2073 7570 706f 7274 7320 7468 6520 666f   supports the fo
-00009530: 6c6c 6f77 696e 6720 7175 616e 7469 7a61  llowing quantiza
-00009540: 7469 6f6e 2074 6563 686e 6971 7565 730a  tion techniques.
-00009550: 0a2d 205b 4c4c 4d2e 696e 7438 2829 3a20  .- [LLM.int8(): 
-00009560: 382d 6269 7420 4d61 7472 6978 204d 756c  8-bit Matrix Mul
-00009570: 7469 706c 6963 6174 696f 6e5d 2868 7474  tiplication](htt
-00009580: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00009590: 6273 2f32 3230 382e 3037 3333 3929 2074  bs/2208.07339) t
-000095a0: 6872 6f75 6768 205b 6269 7473 616e 6462  hrough [bitsandb
-000095b0: 7974 6573 5d28 6874 7470 733a 2f2f 6769  ytes](https://gi
-000095c0: 7468 7562 2e63 6f6d 2f54 696d 4465 7474  thub.com/TimDett
-000095d0: 6d65 7273 2f62 6974 7361 6e64 6279 7465  mers/bitsandbyte
-000095e0: 7329 0a2d 205b 5370 5152 3a20 4120 5370  s).- [SpQR: A Sp
-000095f0: 6172 7365 2d51 7561 6e74 697a 6564 2052  arse-Quantized R
-00009600: 6570 7265 7365 6e74 6174 696f 6e20 666f  epresentation fo
-00009610: 7220 4e65 6172 2d4c 6f73 736c 6573 7320  r Near-Lossless 
-00009620: 4c4c 4d20 5765 6967 6874 2043 6f6d 7072  LLM Weight Compr
-00009630: 6573 7369 6f6e 0a20 205d 2868 7474 7073  ession.  ](https
-00009640: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-00009650: 2f32 3330 362e 3033 3037 3829 2074 6872  /2306.03078) thr
-00009660: 6f75 6768 205b 6269 7473 616e 6462 7974  ough [bitsandbyt
-00009670: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-00009680: 7562 2e63 6f6d 2f54 696d 4465 7474 6d65  ub.com/TimDettme
-00009690: 7273 2f62 6974 7361 6e64 6279 7465 7329  rs/bitsandbytes)
-000096a0: 0a2d 205b 4157 513a 2041 6374 6976 6174  .- [AWQ: Activat
-000096b0: 696f 6e2d 6177 6172 6520 5765 6967 6874  ion-aware Weight
-000096c0: 2051 7561 6e74 697a 6174 696f 6e5d 2868   Quantization](h
-000096d0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-000096e0: 2f61 6273 2f32 3330 362e 3030 3937 3829  /abs/2306.00978)
-000096f0: 2c0a 2d20 5b47 5054 513a 2041 6363 7572  ,.- [GPTQ: Accur
-00009700: 6174 6520 506f 7374 2d54 7261 696e 696e  ate Post-Trainin
-00009710: 6720 5175 616e 7469 7a61 7469 6f6e 5d28  g Quantization](
-00009720: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00009730: 672f 6162 732f 3232 3130 2e31 3733 3233  g/abs/2210.17323
-00009740: 290a 2d20 5b53 7175 6565 7a65 4c4c 4d3a  ).- [SqueezeLLM:
-00009750: 2044 656e 7365 2d61 6e64 2d53 7061 7273   Dense-and-Spars
-00009760: 6520 5175 616e 7469 7a61 7469 6f6e 5d28  e Quantization](
-00009770: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00009780: 672f 6162 732f 3233 3036 2e30 3736 3239  g/abs/2306.07629
-00009790: 292e 0a0a 2323 2320 5079 546f 7263 6820  )...### PyTorch 
-000097a0: 6261 636b 656e 640a 0a57 6974 6820 5079  backend..With Py
-000097b0: 546f 7263 6820 6261 636b 656e 642c 204f  Torch backend, O
-000097c0: 7065 6e4c 4c4d 2073 7570 706f 7274 7320  penLLM supports 
-000097d0: 6069 6e74 3860 2c20 6069 6e74 3460 2c20  `int8`, `int4`, 
-000097e0: 616e 6420 6067 7074 7160 2e0a 0a46 6f72  and `gptq`...For
-000097f0: 2075 7369 6e67 2069 6e74 3820 616e 6420   using int8 and 
-00009800: 696e 7434 2071 7561 6e74 697a 6174 696f  int4 quantizatio
-00009810: 6e20 7468 726f 7567 6820 6062 6974 7361  n through `bitsa
-00009820: 6e64 6279 7465 7360 2c20 796f 7520 6361  ndbytes`, you ca
-00009830: 6e20 7573 6520 7468 6520 666f 6c6c 6f77  n use the follow
-00009840: 696e 6720 636f 6d6d 616e 643a 0a0a 6060  ing command:..``
-00009850: 6062 6173 680a 5452 5553 545f 5245 4d4f  `bash.TRUST_REMO
-00009860: 5445 5f43 4f44 453d 5472 7565 206f 7065  TE_CODE=True ope
-00009870: 6e6c 6c6d 2073 7461 7274 206d 6963 726f  nllm start micro
-00009880: 736f 6674 2f70 6869 2d32 202d 2d71 7561  soft/phi-2 --qua
-00009890: 6e74 697a 6520 696e 7438 0a60 6060 0a0a  ntize int8.```..
-000098a0: 546f 2072 756e 2069 6e66 6572 656e 6365  To run inference
-000098b0: 2077 6974 68c2 a060 6770 7471 602c 2073   with..`gptq`, s
-000098c0: 696d 706c 7920 7061 7373 c2a0 602d 2d71  imply pass..`--q
-000098d0: 7561 6e74 697a 6520 6770 7471 603a 0a0a  uantize gptq`:..
-000098e0: 6060 6062 6173 680a 6f70 656e 6c6c 6d20  ```bash.openllm 
-000098f0: 7374 6172 7420 5468 6542 6c6f 6b65 2f4c  start TheBloke/L
-00009900: 6c61 6d61 2d32 2d37 422d 4368 6174 2d47  lama-2-7B-Chat-G
-00009910: 5054 5120 2d2d 7175 616e 7469 7a65 2067  PTQ --quantize g
-00009920: 7074 710a 6060 600a 0a3e 205b 214e 4f54  ptq.```..> [!NOT
-00009930: 455d 0a3e 2049 6e20 6f72 6465 7220 746f  E].> In order to
-00009940: 2072 756e 2047 5054 512c 206d 616b 6520   run GPTQ, make 
-00009950: 7375 7265 2079 6f75 2072 756e c2a0 6070  sure you run..`p
-00009960: 6970 2069 6e73 7461 6c6c 2022 6f70 656e  ip install "open
-00009970: 6c6c 6d5b 6770 7471 5d22 600a 3e20 6669  llm[gptq]"`.> fi
-00009980: 7273 7420 746f 2069 6e73 7461 6c6c 2074  rst to install t
-00009990: 6865 2064 6570 656e 6465 6e63 792e 2046  he dependency. F
-000099a0: 726f 6d20 7468 6520 4750 5451 2070 6170  rom the GPTQ pap
-000099b0: 6572 2c20 6974 2069 7320 7265 636f 6d6d  er, it is recomm
-000099c0: 656e 6465 6420 746f 2071 7561 6e74 697a  ended to quantiz
-000099d0: 6564 2074 6865 2077 6569 6768 7473 2062  ed the weights b
-000099e0: 6566 6f72 6520 7365 7276 696e 672e 0a3e  efore serving..>
-000099f0: 2053 6565 c2a0 5b41 7574 6f47 5054 515d   See..[AutoGPTQ]
-00009a00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00009a10: 636f 6d2f 5061 6e51 6957 6569 2f41 7574  com/PanQiWei/Aut
-00009a20: 6f47 5054 5129 c2a0 666f 7220 6d6f 7265  oGPTQ)..for more
-00009a30: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00009a40: 4750 5451 2071 7561 6e74 697a 6174 696f  GPTQ quantizatio
-00009a50: 6e2e 0a0a 2323 2320 764c 4c4d 2062 6163  n...### vLLM bac
-00009a60: 6b65 6e64 0a0a 5769 7468 2076 4c4c 4d20  kend..With vLLM 
-00009a70: 6261 636b 656e 642c 204f 7065 6e4c 4c4d  backend, OpenLLM
-00009a80: 2073 7570 706f 7274 7320 6061 7771 602c   supports `awq`,
-00009a90: 2060 7371 7565 657a 656c 6c6d 600a 0a54   `squeezellm`..T
-00009aa0: 6f20 7275 6e20 696e 6665 7265 6e63 6520  o run inference 
-00009ab0: 7769 7468 c2a0 6061 7771 602c 2073 696d  with..`awq`, sim
-00009ac0: 706c 7920 7061 7373 c2a0 602d 2d71 7561  ply pass..`--qua
-00009ad0: 6e74 697a 6520 6177 7160 3a0a 0a60 6060  ntize awq`:..```
-00009ae0: 6261 7368 0a6f 7065 6e6c 6c6d 2073 7461  bash.openllm sta
-00009af0: 7274 2054 6865 426c 6f6b 652f 7a65 7068  rt TheBloke/zeph
-00009b00: 7972 2d37 422d 616c 7068 612d 4157 5120  yr-7B-alpha-AWQ 
-00009b10: 2d2d 7175 616e 7469 7a65 2061 7771 0a60  --quantize awq.`
-00009b20: 6060 0a0a 546f 2072 756e 2069 6e66 6572  ``..To run infer
-00009b30: 656e 6365 2077 6974 6820 6073 7175 6565  ence with `squee
-00009b40: 7a65 6c6c 6d60 2c20 7369 6d70 6c79 2070  zellm`, simply p
-00009b50: 6173 7320 602d 2d71 7561 6e74 697a 6520  ass `--quantize 
-00009b60: 7371 7565 657a 656c 6c6d 603a 0a0a 6060  squeezellm`:..``
-00009b70: 6062 6173 680a 6f70 656e 6c6c 6d20 7374  `bash.openllm st
-00009b80: 6172 7420 7371 7565 657a 652d 6169 2d6c  art squeeze-ai-l
-00009b90: 6162 2f73 712d 6c6c 616d 612d 322d 3762  ab/sq-llama-2-7b
-00009ba0: 2d77 342d 7330 202d 2d71 7561 6e74 697a  -w4-s0 --quantiz
-00009bb0: 6520 7371 7565 657a 656c 6c6d 202d 2d73  e squeezellm --s
-00009bc0: 6572 6961 6c69 7a61 7469 6f6e 206c 6567  erialization leg
-00009bd0: 6163 790a 6060 600a 0a3e 205b 2149 4d50  acy.```..> [!IMP
-00009be0: 4f52 5441 4e54 5d0a 3e20 5369 6e63 6520  ORTANT].> Since 
-00009bf0: 626f 7468 2060 7371 7565 657a 656c 6c6d  both `squeezellm
-00009c00: 6020 616e 6420 6061 7771 6020 6172 6520  ` and `awq` are 
-00009c10: 7765 6967 6874 2d61 7761 7265 2071 7561  weight-aware qua
-00009c20: 6e74 697a 6174 696f 6e20 6d65 7468 6f64  ntization method
-00009c30: 732c 206d 6561 6e69 6e67 2074 6865 2071  s, meaning the q
-00009c40: 7561 6e74 697a 6174 696f 6e20 6973 2064  uantization is d
-00009c50: 6f6e 6520 6475 7269 6e67 2074 7261 696e  one during train
-00009c60: 696e 672c 2061 6c6c 2070 7265 2d74 7261  ing, all pre-tra
-00009c70: 696e 6564 2077 6569 6768 7473 206e 6565  ined weights nee
-00009c80: 6473 2074 6f20 6765 7420 7175 616e 7469  ds to get quanti
-00009c90: 7a65 6420 6265 666f 7265 2069 6e66 6572  zed before infer
-00009ca0: 656e 6365 2074 696d 652e 204d 616b 6520  ence time. Make 
-00009cb0: 7375 7265 2074 6f20 6669 6e64 2063 6f6d  sure to find com
-00009cc0: 7061 7469 626c 6520 7765 6967 6874 7320  patible weights 
-00009cd0: 6f6e 2048 7567 6769 6e67 4661 6365 2048  on HuggingFace H
-00009ce0: 7562 2066 6f72 2079 6f75 7220 6d6f 6465  ub for your mode
-00009cf0: 6c20 6f66 2063 686f 6963 652e 0a0a 2323  l of choice...##
-00009d00: 20f0 9f9b a0ef b88f 2053 6572 7669 6e67   ....... Serving
-00009d10: 2066 696e 652d 7475 6e69 6e67 206c 6179   fine-tuning lay
-00009d20: 6572 730a 0a5b 5045 4654 5d28 6874 7470  ers..[PEFT](http
-00009d30: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-00009d40: 636f 2f64 6f63 732f 7065 6674 2f69 6e64  co/docs/peft/ind
-00009d50: 6578 292c 206f 7220 5061 7261 6d65 7465  ex), or Paramete
-00009d60: 722d 4566 6669 6369 656e 7420 4669 6e65  r-Efficient Fine
-00009d70: 2d54 756e 696e 672c 2069 7320 6120 6d65  -Tuning, is a me
-00009d80: 7468 6f64 6f6c 6f67 7920 6465 7369 676e  thodology design
-00009d90: 6564 2074 6f20 6669 6e65 2d74 756e 6520  ed to fine-tune 
-00009da0: 7072 652d 7472 6169 6e65 6420 6d6f 6465  pre-trained mode
-00009db0: 6c73 206d 6f72 6520 6566 6669 6369 656e  ls more efficien
-00009dc0: 746c 792e 2049 6e73 7465 6164 206f 6620  tly. Instead of 
-00009dd0: 6164 6a75 7374 696e 6720 616c 6c20 6d6f  adjusting all mo
-00009de0: 6465 6c20 7061 7261 6d65 7465 7273 2c20  del parameters, 
-00009df0: 5045 4654 2066 6f63 7573 6573 206f 6e20  PEFT focuses on 
-00009e00: 7475 6e69 6e67 206f 6e6c 7920 6120 7375  tuning only a su
-00009e10: 6273 6574 2c20 7265 6475 6369 6e67 2063  bset, reducing c
-00009e20: 6f6d 7075 7461 7469 6f6e 616c 2061 6e64  omputational and
-00009e30: 2073 746f 7261 6765 2063 6f73 7473 2e20   storage costs. 
-00009e40: 5b4c 6f52 415d 2868 7474 7073 3a2f 2f68  [LoRA](https://h
-00009e50: 7567 6769 6e67 6661 6365 2e63 6f2f 646f  uggingface.co/do
-00009e60: 6373 2f70 6566 742f 636f 6e63 6570 7475  cs/peft/conceptu
-00009e70: 616c 5f67 7569 6465 732f 6c6f 7261 2920  al_guides/lora) 
-00009e80: 284c 6f77 2d52 616e 6b20 4164 6170 7461  (Low-Rank Adapta
-00009e90: 7469 6f6e 2920 6973 206f 6e65 206f 6620  tion) is one of 
-00009ea0: 7468 6520 7465 6368 6e69 7175 6573 2073  the techniques s
-00009eb0: 7570 706f 7274 6564 2062 7920 5045 4654  upported by PEFT
-00009ec0: 2e20 4974 2073 7472 6561 6d6c 696e 6573  . It streamlines
-00009ed0: 2066 696e 652d 7475 6e69 6e67 2062 7920   fine-tuning by 
-00009ee0: 7573 696e 6720 6c6f 772d 7261 6e6b 2064  using low-rank d
-00009ef0: 6563 6f6d 706f 7369 7469 6f6e 2074 6f20  ecomposition to 
-00009f00: 7265 7072 6573 656e 7420 7765 6967 6874  represent weight
-00009f10: 2075 7064 6174 6573 2c20 7468 6572 6562   updates, thereb
-00009f20: 7920 6472 6173 7469 6361 6c6c 7920 7265  y drastically re
-00009f30: 6475 6369 6e67 2074 6865 206e 756d 6265  ducing the numbe
-00009f40: 7220 6f66 2074 7261 696e 6162 6c65 2070  r of trainable p
-00009f50: 6172 616d 6574 6572 732e 0a0a 5769 7468  arameters...With
-00009f60: 204f 7065 6e4c 4c4d 2c20 796f 7520 6361   OpenLLM, you ca
-00009f70: 6e20 7461 6b65 2061 6476 616e 7461 6765  n take advantage
-00009f80: 206f 6620 7468 6520 6669 6e65 2d74 756e   of the fine-tun
-00009f90: 696e 6720 6665 6174 7572 6520 6279 2073  ing feature by s
-00009fa0: 6572 7669 6e67 206d 6f64 656c 7320 7769  erving models wi
-00009fb0: 7468 2061 6e79 2050 4546 542d 636f 6d70  th any PEFT-comp
-00009fc0: 6174 6962 6c65 206c 6179 6572 7320 7573  atible layers us
-00009fd0: 696e 6720 7468 6520 602d 2d61 6461 7074  ing the `--adapt
-00009fe0: 6572 2d69 6460 206f 7074 696f 6e2e 2046  er-id` option. F
-00009ff0: 6f72 2065 7861 6d70 6c65 3a0a 0a60 6060  or example:..```
-0000a000: 6261 7368 0a6f 7065 6e6c 6c6d 2073 7461  bash.openllm sta
-0000a010: 7274 2066 6163 6562 6f6f 6b2f 6f70 742d  rt facebook/opt-
-0000a020: 362e 3762 202d 2d61 6461 7074 6572 2d69  6.7b --adapter-i
-0000a030: 6420 6161 726e 7068 6d2f 6f70 742d 362d  d aarnphm/opt-6-
-0000a040: 3762 2d71 756f 7465 733a 6465 6661 756c  7b-quotes:defaul
-0000a050: 740a 6060 600a 0a4f 7065 6e4c 4c4d 2061  t.```..OpenLLM a
-0000a060: 6c73 6f20 7072 6f76 6964 6573 2066 6c65  lso provides fle
-0000a070: 7869 6269 6c69 7479 2062 7920 7375 7070  xibility by supp
-0000a080: 6f72 7469 6e67 2061 6461 7074 6572 7320  orting adapters 
-0000a090: 6672 6f6d 2063 7573 746f 6d20 6669 6c65  from custom file
-0000a0a0: 2070 6174 6873 3a0a 0a60 6060 6261 7368   paths:..```bash
-0000a0b0: 0a6f 7065 6e6c 6c6d 2073 7461 7274 2066  .openllm start f
-0000a0c0: 6163 6562 6f6f 6b2f 6f70 742d 362e 3762  acebook/opt-6.7b
-0000a0d0: 202d 2d61 6461 7074 6572 2d69 6420 2f70   --adapter-id /p
-0000a0e0: 6174 682f 746f 2f61 6461 7074 6572 733a  ath/to/adapters:
-0000a0f0: 6c6f 6361 6c5f 6164 6170 7465 720a 6060  local_adapter.``
-0000a100: 600a 0a54 6f20 7573 6520 6d75 6c74 6970  `..To use multip
-0000a110: 6c65 2061 6461 7074 6572 732c 2075 7365  le adapters, use
-0000a120: 2074 6865 2066 6f6c 6c6f 7769 6e67 2066   the following f
-0000a130: 6f72 6d61 743a 0a0a 6060 6062 6173 680a  ormat:..```bash.
-0000a140: 6f70 656e 6c6c 6d20 7374 6172 7420 6661  openllm start fa
-0000a150: 6365 626f 6f6b 2f6f 7074 2d36 2e37 6220  cebook/opt-6.7b 
-0000a160: 2d2d 6164 6170 7465 722d 6964 2061 6172  --adapter-id aar
-0000a170: 6e70 686d 2f6f 7074 2d36 2e37 622d 6c6f  nphm/opt-6.7b-lo
-0000a180: 7261 3a64 6566 6175 6c74 202d 2d61 6461  ra:default --ada
-0000a190: 7074 6572 2d69 6420 6161 726e 7068 6d2f  pter-id aarnphm/
-0000a1a0: 6f70 742d 362e 3762 2d66 7265 6e63 683a  opt-6.7b-french:
-0000a1b0: 6672 656e 6368 5f6c 6f72 610a 6060 600a  french_lora.```.
-0000a1c0: 0a42 7920 6465 6661 756c 742c 2061 6c6c  .By default, all
-0000a1d0: 2061 6461 7074 6572 7320 7769 6c6c 2062   adapters will b
-0000a1e0: 6520 696e 6a65 6374 6564 2069 6e74 6f20  e injected into 
-0000a1f0: 7468 6520 6d6f 6465 6c73 2064 7572 696e  the models durin
-0000a200: 6720 7374 6172 7475 702e 2041 6461 7074  g startup. Adapt
-0000a210: 6572 7320 6361 6e20 6265 2073 7065 6369  ers can be speci
-0000a220: 6669 6564 2070 6572 2072 6571 7565 7374  fied per request
-0000a230: 2076 6961 2060 6164 6170 7465 725f 6e61   via `adapter_na
-0000a240: 6d65 603a 0a0a 6060 6062 6173 680a 6375  me`:..```bash.cu
-0000a250: 726c 202d 5820 2750 4f53 5427 205c 0a20  rl -X 'POST' \. 
-0000a260: 2027 6874 7470 3a2f 2f6c 6f63 616c 686f   'http://localho
-0000a270: 7374 3a33 3030 302f 7631 2f67 656e 6572  st:3000/v1/gener
-0000a280: 6174 6527 205c 0a20 202d 4820 2761 6363  ate' \.  -H 'acc
-0000a290: 6570 743a 2061 7070 6c69 6361 7469 6f6e  ept: application
-0000a2a0: 2f6a 736f 6e27 205c 0a20 202d 4820 2743  /json' \.  -H 'C
-0000a2b0: 6f6e 7465 6e74 2d54 7970 653a 2061 7070  ontent-Type: app
-0000a2c0: 6c69 6361 7469 6f6e 2f6a 736f 6e27 205c  lication/json' \
-0000a2d0: 0a20 202d 6420 277b 0a20 2022 7072 6f6d  .  -d '{.  "prom
-0000a2e0: 7074 223a 2022 5768 6174 2069 7320 7468  pt": "What is th
-0000a2f0: 6520 6d65 616e 696e 6720 6f66 206c 6966  e meaning of lif
-0000a300: 653f 222c 0a20 2022 7374 6f70 223a 205b  e?",.  "stop": [
-0000a310: 0a20 2020 2022 7068 696c 6f73 6f70 6865  .    "philosophe
-0000a320: 7222 0a20 205d 2c0a 2020 226c 6c6d 5f63  r".  ],.  "llm_c
-0000a330: 6f6e 6669 6722 3a20 7b0a 2020 2020 226d  onfig": {.    "m
-0000a340: 6178 5f6e 6577 5f74 6f6b 656e 7322 3a20  ax_new_tokens": 
-0000a350: 3235 362c 0a20 2020 2022 7465 6d70 6572  256,.    "temper
-0000a360: 6174 7572 6522 3a20 302e 3735 2c0a 2020  ature": 0.75,.  
-0000a370: 2020 2274 6f70 5f6b 223a 2031 352c 0a20    "top_k": 15,. 
-0000a380: 2020 2022 746f 705f 7022 3a20 310a 2020     "top_p": 1.  
-0000a390: 7d2c 0a20 2022 6164 6170 7465 725f 6e61  },.  "adapter_na
-0000a3a0: 6d65 223a 2022 6465 6661 756c 7422 0a7d  me": "default".}
-0000a3b0: 270a 6060 600a 0a54 6f20 696e 636c 7564  '.```..To includ
-0000a3c0: 6520 7468 6973 2069 6e74 6f20 7468 6520  e this into the 
-0000a3d0: 4265 6e74 6f2c 2079 6f75 2063 616e 2073  Bento, you can s
-0000a3e0: 7065 6369 6679 2074 6865 c2a0 602d 2d61  pecify the..`--a
-0000a3f0: 6461 7074 6572 2d69 6460 c2a0 6f70 7469  dapter-id`..opti
-0000a400: 6f6e 2077 6865 6e20 7573 696e 6720 7468  on when using th
-0000a410: 65c2 a060 6f70 656e 6c6c 6d20 6275 696c  e..`openllm buil
-0000a420: 6460 2063 6f6d 6d61 6e64 3a0a 0a60 6060  d` command:..```
-0000a430: 6261 7368 0a6f 7065 6e6c 6c6d 2062 7569  bash.openllm bui
-0000a440: 6c64 2066 6163 6562 6f6f 6b2f 6f70 742d  ld facebook/opt-
-0000a450: 362e 3762 202d 2d61 6461 7074 6572 2d69  6.7b --adapter-i
-0000a460: 6420 2e2e 2e0a 6060 600a 0a49 6620 796f  d ....```..If yo
-0000a470: 7520 7573 6520 6120 7265 6c61 7469 7665  u use a relative
-0000a480: 2070 6174 6820 666f 7220 602d 2d61 6461   path for `--ada
-0000a490: 7074 6572 2d69 6460 2c20 796f 7520 6e65  pter-id`, you ne
-0000a4a0: 6564 2074 6f20 6164 6420 602d 2d62 7569  ed to add `--bui
-0000a4b0: 6c64 2d63 7478 602e 0a0a 6060 6062 6173  ld-ctx`...```bas
-0000a4c0: 680a 6f70 656e 6c6c 6d20 6275 696c 6420  h.openllm build 
-0000a4d0: 6661 6365 626f 6f6b 2f6f 7074 2d36 2e37  facebook/opt-6.7
-0000a4e0: 6220 2d2d 6164 6170 7465 722d 6964 202e  b --adapter-id .
-0000a4f0: 2f70 6174 682f 746f 2f61 6461 7074 6572  /path/to/adapter
-0000a500: 5f69 6420 2d2d 6275 696c 642d 6374 7820  _id --build-ctx 
-0000a510: 2e0a 6060 600a 0a3e 205b 2149 4d50 4f52  ..```..> [!IMPOR
-0000a520: 5441 4e54 5d0a 3e20 4669 6e65 2d74 756e  TANT].> Fine-tun
-0000a530: 696e 6720 7375 7070 6f72 7420 6973 2073  ing support is s
-0000a540: 7469 6c6c 2065 7870 6572 696d 656e 7461  till experimenta
-0000a550: 6c20 616e 6420 6375 7272 656e 746c 7920  l and currently 
-0000a560: 6f6e 6c79 2077 6f72 6b73 2077 6974 6820  only works with 
-0000a570: 5079 546f 7263 6820 6261 636b 656e 642e  PyTorch backend.
-0000a580: 2076 4c4c 4d20 7375 7070 6f72 7420 6973   vLLM support is
-0000a590: 2063 6f6d 696e 6720 736f 6f6e 2e0a 0a23   coming soon...#
-0000a5a0: 2320 f09f 908d 2050 7974 686f 6e20 5344  # .... Python SD
-0000a5b0: 4b0a 0a45 6163 6820 4c4c 4d20 6361 6e20  K..Each LLM can 
-0000a5c0: 6265 2069 6e73 7461 6e74 6961 7465 6420  be instantiated 
-0000a5d0: 7769 7468 2060 6f70 656e 6c6c 6d2e 4c4c  with `openllm.LL
-0000a5e0: 4d60 3a0a 0a60 6060 7079 7468 6f6e 0a69  M`:..```python.i
-0000a5f0: 6d70 6f72 7420 6f70 656e 6c6c 6d0a 0a6c  mport openllm..l
-0000a600: 6c6d 203d 206f 7065 6e6c 6c6d 2e4c 4c4d  lm = openllm.LLM
-0000a610: 2827 6d69 6372 6f73 6f66 742f 7068 692d  ('microsoft/phi-
-0000a620: 3227 290a 6060 600a 0a54 6865 206d 6169  2').```..The mai
-0000a630: 6e20 696e 6665 7265 6e63 6520 4150 4920  n inference API 
-0000a640: 6973 2074 6865 2073 7472 6561 6d69 6e67  is the streaming
-0000a650: 2060 6765 6e65 7261 7465 5f69 7465 7261   `generate_itera
-0000a660: 746f 7260 206d 6574 686f 643a 0a0a 6060  tor` method:..``
-0000a670: 6070 7974 686f 6e0a 6173 796e 6320 666f  `python.async fo
-0000a680: 7220 6765 6e65 7261 7469 6f6e 2069 6e20  r generation in 
-0000a690: 6c6c 6d2e 6765 6e65 7261 7465 5f69 7465  llm.generate_ite
-0000a6a0: 7261 746f 7228 2757 6861 7420 6973 2074  rator('What is t
-0000a6b0: 6865 206d 6561 6e69 6e67 206f 6620 6c69  he meaning of li
-0000a6c0: 6665 3f27 293a 0a20 2070 7269 6e74 2867  fe?'):.  print(g
-0000a6d0: 656e 6572 6174 696f 6e2e 6f75 7470 7574  eneration.output
-0000a6e0: 735b 305d 2e74 6578 7429 0a60 6060 0a0a  s[0].text).```..
-0000a6f0: 3e20 5b21 4e4f 5445 5d0a 3e20 5468 6520  > [!NOTE].> The 
-0000a700: 6d6f 7469 7661 7469 6f6e 2062 6568 696e  motivation behin
-0000a710: 6420 6d61 6b69 6e67 2060 6c6c 6d2e 6765  d making `llm.ge
-0000a720: 6e65 7261 7465 5f69 7465 7261 746f 7260  nerate_iterator`
-0000a730: 2061 6e20 6173 796e 6320 6765 6e65 7261   an async genera
-0000a740: 746f 7220 6973 2074 6f20 7072 6f76 6964  tor is to provid
-0000a750: 6520 7375 7070 6f72 7420 666f 7220 436f  e support for Co
-0000a760: 6e74 696e 756f 7573 2062 6174 6368 696e  ntinuous batchin
-0000a770: 6720 7769 7468 2076 4c4c 4d20 6261 636b  g with vLLM back
-0000a780: 656e 642e 2042 7920 6861 7669 6e67 2074  end. By having t
-0000a790: 6865 2061 7379 6e63 2065 6e64 706f 696e  he async endpoin
-0000a7a0: 7473 2c20 6561 6368 2070 726f 6d70 740a  ts, each prompt.
-0000a7b0: 3e20 7769 6c6c 2062 6520 6164 6465 6420  > will be added 
-0000a7c0: 636f 7272 6563 746c 7920 746f 2074 6865  correctly to the
-0000a7d0: 2072 6571 7565 7374 2071 7565 7565 2074   request queue t
-0000a7e0: 6f20 7072 6f63 6573 7320 7769 7468 2076  o process with v
-0000a7f0: 4c4c 4d20 6261 636b 656e 642e 0a0a 5468  LLM backend...Th
-0000a800: 6572 6520 6973 2061 6c73 6f20 6120 5f6f  ere is also a _o
-0000a810: 6e65 2d73 686f 745f 2060 6765 6e65 7261  ne-shot_ `genera
-0000a820: 7465 6020 6d65 7468 6f64 3a0a 0a60 6060  te` method:..```
-0000a830: 7079 7468 6f6e 0a61 7761 6974 206c 6c6d  python.await llm
-0000a840: 2e67 656e 6572 6174 6528 2757 6861 7420  .generate('What 
-0000a850: 6973 2074 6865 206d 6561 6e69 6e67 206f  is the meaning o
-0000a860: 6620 6c69 6665 3f27 290a 6060 600a 0a54  f life?').```..T
-0000a870: 6869 7320 6d65 7468 6f64 2069 7320 6561  his method is ea
-0000a880: 7379 2074 6f20 7573 6520 666f 7220 6f6e  sy to use for on
-0000a890: 652d 7368 6f74 2067 656e 6572 6174 696f  e-shot generatio
-0000a8a0: 6e20 7573 6520 6361 7365 2c20 6275 7420  n use case, but 
-0000a8b0: 6d65 7265 6c79 2073 6572 7665 6420 6173  merely served as
-0000a8c0: 2061 6e20 6578 616d 706c 6520 686f 7720   an example how 
-0000a8d0: 746f 2075 7365 2060 6c6c 6d2e 6765 6e65  to use `llm.gene
-0000a8e0: 7261 7465 5f69 7465 7261 746f 7260 2061  rate_iterator` a
-0000a8f0: 7320 6974 2075 7365 7320 6067 656e 6572  s it uses `gener
-0000a900: 6174 655f 6974 6572 6174 6f72 6020 756e  ate_iterator` un
-0000a910: 6465 7220 7468 6520 686f 6f64 2e0a 0a3e  der the hood...>
-0000a920: 205b 2149 4d50 4f52 5441 4e54 5d0a 3e20   [!IMPORTANT].> 
-0000a930: 4966 2079 6f75 206e 6565 6420 746f 2063  If you need to c
-0000a940: 616c 6c20 796f 7572 2063 6f64 6520 696e  all your code in
-0000a950: 2061 2073 796e 6368 726f 6e6f 7573 2063   a synchronous c
-0000a960: 6f6e 7465 7874 2c20 796f 7520 6361 6e20  ontext, you can 
-0000a970: 7573 6520 6061 7379 6e63 696f 2e72 756e  use `asyncio.run
-0000a980: 6020 7468 6174 2077 7261 7073 2061 6e20  ` that wraps an 
-0000a990: 6173 796e 6320 6675 6e63 7469 6f6e 3a0a  async function:.
-0000a9a0: 3e0a 3e20 6060 6070 7974 686f 6e0a 3e20  >.> ```python.> 
-0000a9b0: 696d 706f 7274 2061 7379 6e63 696f 0a3e  import asyncio.>
-0000a9c0: 2061 7379 6e63 2064 6566 2067 656e 6572   async def gener
-0000a9d0: 6174 6528 7072 6f6d 7074 2c20 2a2a 6174  ate(prompt, **at
-0000a9e0: 7472 7329 3a20 7265 7475 726e 2061 7761  trs): return awa
-0000a9f0: 6974 206c 6c6d 2e67 656e 6572 6174 6528  it llm.generate(
-0000aa00: 7072 6f6d 7074 2c20 2a2a 6174 7472 7329  prompt, **attrs)
-0000aa10: 0a3e 2061 7379 6e63 696f 2e72 756e 2867  .> asyncio.run(g
-0000aa20: 656e 6572 6174 6528 2254 6865 206d 6561  enerate("The mea
-0000aa30: 6e69 6e67 206f 6620 6c69 6665 2069 7322  ning of life is"
-0000aa40: 2c20 7465 6d70 6572 6174 7572 653d 302e  , temperature=0.
-0000aa50: 3233 2929 0a3e 2060 6060 0a0a 2323 20e2  23)).> ```..## .
-0000aa60: 9a99 efb8 8f20 496e 7465 6772 6174 696f  ..... Integratio
-0000aa70: 6e73 0a0a 4f70 656e 4c4c 4d20 6973 206e  ns..OpenLLM is n
-0000aa80: 6f74 206a 7573 7420 6120 7374 616e 6461  ot just a standa
-0000aa90: 6c6f 6e65 2070 726f 6475 6374 3b20 6974  lone product; it
-0000aaa0: 2773 2061 2062 7569 6c64 696e 6720 626c  's a building bl
-0000aab0: 6f63 6b20 6465 7369 676e 6564 2074 6f0a  ock designed to.
-0000aac0: 696e 7465 6772 6174 6520 7769 7468 206f  integrate with o
-0000aad0: 7468 6572 2070 6f77 6572 6675 6c20 746f  ther powerful to
-0000aae0: 6f6c 7320 6561 7369 6c79 2e20 5765 2063  ols easily. We c
-0000aaf0: 7572 7265 6e74 6c79 206f 6666 6572 2069  urrently offer i
-0000ab00: 6e74 6567 7261 7469 6f6e 2077 6974 680a  ntegration with.
-0000ab10: 5b42 656e 746f 4d4c 5d28 6874 7470 733a  [BentoML](https:
-0000ab20: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
-0000ab30: 746f 6d6c 2f42 656e 746f 4d4c 292c 0a5b  toml/BentoML),.[
-0000ab40: 4f70 656e 4149 2773 2043 6f6d 7061 7469  OpenAI's Compati
-0000ab50: 626c 6520 456e 6470 6f69 6e74 735d 2868  ble Endpoints](h
-0000ab60: 7474 7073 3a2f 2f70 6c61 7466 6f72 6d2e  ttps://platform.
-0000ab70: 6f70 656e 6169 2e63 6f6d 2f64 6f63 732f  openai.com/docs/
-0000ab80: 6170 692d 7265 6665 7265 6e63 652f 636f  api-reference/co
-0000ab90: 6d70 6c65 7469 6f6e 732f 6f62 6a65 6374  mpletions/object
-0000aba0: 292c 0a5b 4c6c 616d 6149 6e64 6578 5d28  ),.[LlamaIndex](
-0000abb0: 6874 7470 733a 2f2f 7777 772e 6c6c 616d  https://www.llam
-0000abc0: 6169 6e64 6578 2e61 692f 292c 0a5b 4c61  aindex.ai/),.[La
-0000abd0: 6e67 4368 6169 6e5d 2868 7474 7073 3a2f  ngChain](https:/
-0000abe0: 2f67 6974 6875 622e 636f 6d2f 6877 6368  /github.com/hwch
-0000abf0: 6173 6531 372f 6c61 6e67 6368 6169 6e29  ase17/langchain)
-0000ac00: 2c20 616e 640a 5b54 7261 6e73 666f 726d  , and.[Transform
-0000ac10: 6572 7320 4167 656e 7473 5d28 6874 7470  ers Agents](http
-0000ac20: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
-0000ac30: 636f 2f64 6f63 732f 7472 616e 7366 6f72  co/docs/transfor
-0000ac40: 6d65 7273 2f74 7261 6e73 666f 726d 6572  mers/transformer
-0000ac50: 735f 6167 656e 7473 292e 0a0a 2323 2320  s_agents)...### 
-0000ac60: 4f70 656e 4149 2043 6f6d 7061 7469 626c  OpenAI Compatibl
-0000ac70: 6520 456e 6470 6f69 6e74 730a 0a4f 7065  e Endpoints..Ope
-0000ac80: 6e4c 4c4d 2053 6572 7665 7220 6361 6e20  nLLM Server can 
-0000ac90: 6265 2075 7365 6420 6173 2061 2064 726f  be used as a dro
-0000aca0: 702d 696e 2072 6570 6c61 6365 6d65 6e74  p-in replacement
-0000acb0: 2066 6f72 204f 7065 6e41 4927 7320 4150   for OpenAI's AP
-0000acc0: 492e 2053 696d 706c 790a 7370 6563 6966  I. Simply.specif
-0000acd0: 7920 7468 6520 6261 7365 5f75 726c 2074  y the base_url t
-0000ace0: 6f20 606c 6c6d 2d65 6e64 706f 696e 742f  o `llm-endpoint/
-0000acf0: 7631 6020 616e 6420 796f 7520 6172 6520  v1` and you are 
-0000ad00: 676f 6f64 2074 6f20 676f 3a0a 0a60 6060  good to go:..```
-0000ad10: 7079 7468 6f6e 0a69 6d70 6f72 7420 6f70  python.import op
-0000ad20: 656e 6169 0a0a 636c 6965 6e74 203d 206f  enai..client = o
-0000ad30: 7065 6e61 692e 4f70 656e 4149 280a 2020  penai.OpenAI(.  
-0000ad40: 6261 7365 5f75 726c 3d27 6874 7470 3a2f  base_url='http:/
-0000ad50: 2f6c 6f63 616c 686f 7374 3a33 3030 302f  /localhost:3000/
-0000ad60: 7631 272c 2061 7069 5f6b 6579 3d27 6e61  v1', api_key='na
-0000ad70: 270a 2920 2023 2048 6572 6520 7468 6520  '.)  # Here the 
-0000ad80: 7365 7276 6572 2069 7320 7275 6e6e 696e  server is runnin
-0000ad90: 6720 6f6e 206c 6f63 616c 686f 7374 3a33  g on localhost:3
-0000ada0: 3030 300a 0a63 6f6d 706c 6574 696f 6e73  000..completions
-0000adb0: 203d 2063 6c69 656e 742e 636f 6d70 6c65   = client.comple
-0000adc0: 7469 6f6e 732e 6372 6561 7465 280a 2020  tions.create(.  
-0000add0: 7072 6f6d 7074 3d27 5772 6974 6520 6d65  prompt='Write me
-0000ade0: 2061 2074 6167 206c 696e 6520 666f 7220   a tag line for 
-0000adf0: 616e 2069 6365 2063 7265 616d 2073 686f  an ice cream sho
-0000ae00: 702e 272c 206d 6f64 656c 3d6d 6f64 656c  p.', model=model
-0000ae10: 2c20 6d61 785f 746f 6b65 6e73 3d36 342c  , max_tokens=64,
-0000ae20: 2073 7472 6561 6d3d 7374 7265 616d 0a29   stream=stream.)
-0000ae30: 0a60 6060 0a0a 5468 6520 636f 6d70 6174  .```..The compat
-0000ae40: 6962 6c65 2065 6e64 706f 696e 7473 2073  ible endpoints s
-0000ae50: 7570 706f 7274 7320 602f 636f 6d70 6c65  upports `/comple
-0000ae60: 7469 6f6e 7360 2c20 602f 6368 6174 2f63  tions`, `/chat/c
-0000ae70: 6f6d 706c 6574 696f 6e73 602c 2061 6e64  ompletions`, and
-0000ae80: 2060 2f6d 6f64 656c 7360 0a0a 3e20 5b21   `/models`..> [!
-0000ae90: 4e4f 5445 5d0a 3e20 596f 7520 6361 6e20  NOTE].> You can 
-0000aea0: 6669 6e64 206f 7574 204f 7065 6e41 4920  find out OpenAI 
-0000aeb0: 6578 616d 706c 6520 636c 6965 6e74 7320  example clients 
-0000aec0: 756e 6465 7220 7468 650a 3e20 5b65 7861  under the.> [exa
-0000aed0: 6d70 6c65 735d 2868 7474 7073 3a2f 2f67  mples](https://g
-0000aee0: 6974 6875 622e 636f 6d2f 6265 6e74 6f6d  ithub.com/bentom
-0000aef0: 6c2f 4f70 656e 4c4c 4d2f 7472 6565 2f6d  l/OpenLLM/tree/m
-0000af00: 6169 6e2f 6578 616d 706c 6573 2920 666f  ain/examples) fo
-0000af10: 6c64 6572 2e0a 0a23 2323 2042 656e 746f  lder...### Bento
-0000af20: 4d4c 0a0a 4f70 656e 4c4c 4d20 4c4c 4d20  ML..OpenLLM LLM 
-0000af30: 6361 6e20 6265 2069 6e74 6567 7261 7465  can be integrate
-0000af40: 6420 6173 2061 0a5b 5275 6e6e 6572 5d28  d as a.[Runner](
-0000af50: 6874 7470 733a 2f2f 646f 6373 2e62 656e  https://docs.ben
-0000af60: 746f 6d6c 2e63 6f6d 2f65 6e2f 6c61 7465  toml.com/en/late
-0000af70: 7374 2f63 6f6e 6365 7074 732f 7275 6e6e  st/concepts/runn
-0000af80: 6572 2e68 746d 6c29 2069 6e20 796f 7572  er.html) in your
-0000af90: 0a42 656e 746f 4d4c 2073 6572 7669 6365  .BentoML service
-0000afa0: 2e20 5369 6d70 6c79 2063 616c 6c20 6061  . Simply call `a
-0000afb0: 7761 6974 206c 6c6d 2e67 656e 6572 6174  wait llm.generat
-0000afc0: 6560 2074 6f20 6765 6e65 7261 7465 2074  e` to generate t
-0000afd0: 6578 742e 204e 6f74 6520 7468 6174 0a60  ext. Note that.`
-0000afe0: 6c6c 6d2e 6765 6e65 7261 7465 6020 7573  llm.generate` us
-0000aff0: 6573 2060 7275 6e6e 6572 6020 756e 6465  es `runner` unde
-0000b000: 7220 7468 6520 686f 6f64 3a0a 0a60 6060  r the hood:..```
-0000b010: 7079 7468 6f6e 0a69 6d70 6f72 7420 6265  python.import be
-0000b020: 6e74 6f6d 6c0a 696d 706f 7274 206f 7065  ntoml.import ope
-0000b030: 6e6c 6c6d 0a0a 6c6c 6d20 3d20 6f70 656e  nllm..llm = open
-0000b040: 6c6c 6d2e 4c4c 4d28 276d 6963 726f 736f  llm.LLM('microso
-0000b050: 6674 2f70 6869 2d32 2729 0a0a 7376 6320  ft/phi-2')..svc 
-0000b060: 3d20 6265 6e74 6f6d 6c2e 5365 7276 6963  = bentoml.Servic
-0000b070: 6528 6e61 6d65 3d27 6c6c 6d2d 7068 692d  e(name='llm-phi-
-0000b080: 7365 7276 6963 6527 2c20 7275 6e6e 6572  service', runner
-0000b090: 733d 5b6c 6c6d 2e72 756e 6e65 725d 290a  s=[llm.runner]).
-0000b0a0: 0a0a 4073 7663 2e61 7069 2869 6e70 7574  ..@svc.api(input
-0000b0b0: 3d62 656e 746f 6d6c 2e69 6f2e 5465 7874  =bentoml.io.Text
-0000b0c0: 2829 2c20 6f75 7470 7574 3d62 656e 746f  (), output=bento
-0000b0d0: 6d6c 2e69 6f2e 5465 7874 2829 290a 6173  ml.io.Text()).as
-0000b0e0: 796e 6320 6465 6620 7072 6f6d 7074 2869  ync def prompt(i
-0000b0f0: 6e70 7574 5f74 6578 743a 2073 7472 2920  nput_text: str) 
-0000b100: 2d3e 2073 7472 3a0a 2020 6765 6e65 7261  -> str:.  genera
-0000b110: 7469 6f6e 203d 2061 7761 6974 206c 6c6d  tion = await llm
-0000b120: 2e67 656e 6572 6174 6528 696e 7075 745f  .generate(input_
-0000b130: 7465 7874 290a 2020 7265 7475 726e 2067  text).  return g
-0000b140: 656e 6572 6174 696f 6e2e 6f75 7470 7574  eneration.output
-0000b150: 735b 305d 2e74 6578 740a 6060 600a 0a23  s[0].text.```..#
-0000b160: 2323 205b 4c6c 616d 6149 6e64 6578 5d28  ## [LlamaIndex](
-0000b170: 6874 7470 733a 2f2f 646f 6373 2e6c 6c61  https://docs.lla
-0000b180: 6d61 696e 6465 782e 6169 2f65 6e2f 7374  maindex.ai/en/st
-0000b190: 6162 6c65 2f6d 6f64 756c 655f 6775 6964  able/module_guid
-0000b1a0: 6573 2f6d 6f64 656c 732f 6c6c 6d73 2f6d  es/models/llms/m
-0000b1b0: 6f64 756c 6573 2e68 746d 6c23 6f70 656e  odules.html#open
-0000b1c0: 6c6c 6d29 0a0a 546f 2073 7461 7274 2061  llm)..To start a
-0000b1d0: 206c 6f63 616c 204c 4c4d 2077 6974 6820   local LLM with 
-0000b1e0: 606c 6c61 6d61 5f69 6e64 6578 602c 2073  `llama_index`, s
-0000b1f0: 696d 706c 7920 7573 6520 606c 6c61 6d61  imply use `llama
-0000b200: 5f69 6e64 6578 2e6c 6c6d 732e 6f70 656e  _index.llms.open
-0000b210: 6c6c 6d2e 4f70 656e 4c4c 4d60 3a0a 0a60  llm.OpenLLM`:..`
-0000b220: 6060 7079 7468 6f6e 0a69 6d70 6f72 7420  ``python.import 
-0000b230: 6173 796e 6369 6f0a 6672 6f6d 206c 6c61  asyncio.from lla
-0000b240: 6d61 5f69 6e64 6578 2e6c 6c6d 732e 6f70  ma_index.llms.op
-0000b250: 656e 6c6c 6d20 696d 706f 7274 204f 7065  enllm import Ope
-0000b260: 6e4c 4c4d 0a0a 6c6c 6d20 3d20 4f70 656e  nLLM..llm = Open
-0000b270: 4c4c 4d28 2748 7567 6769 6e67 4661 6365  LLM('HuggingFace
-0000b280: 4834 2f7a 6570 6879 722d 3762 2d61 6c70  H4/zephyr-7b-alp
-0000b290: 6861 2729 0a0a 6c6c 6d2e 636f 6d70 6c65  ha')..llm.comple
-0000b2a0: 7465 2827 5468 6520 6d65 616e 696e 6720  te('The meaning 
-0000b2b0: 6f66 206c 6966 6520 6973 2729 0a0a 0a61  of life is')...a
-0000b2c0: 7379 6e63 2064 6566 206d 6169 6e28 7072  sync def main(pr
-0000b2d0: 6f6d 7074 2c20 2a2a 6b77 6172 6773 293a  ompt, **kwargs):
-0000b2e0: 0a20 2061 7379 6e63 2066 6f72 2069 7420  .  async for it 
-0000b2f0: 696e 206c 6c6d 2e61 7374 7265 616d 5f63  in llm.astream_c
-0000b300: 6861 7428 7072 6f6d 7074 2c20 2a2a 6b77  hat(prompt, **kw
-0000b310: 6172 6773 293a 0a20 2020 2070 7269 6e74  args):.    print
-0000b320: 2869 7429 0a0a 0a61 7379 6e63 696f 2e72  (it)...asyncio.r
-0000b330: 756e 286d 6169 6e28 2754 6865 2074 696d  un(main('The tim
-0000b340: 6520 6174 2053 616e 2046 7261 6e63 6973  e at San Francis
-0000b350: 636f 2069 7327 2929 0a60 6060 0a0a 4966  co is')).```..If
-0000b360: 2074 6865 7265 2069 7320 6120 7265 6d6f   there is a remo
-0000b370: 7465 204c 4c4d 2053 6572 7665 7220 7275  te LLM Server ru
-0000b380: 6e6e 696e 6720 656c 7365 7768 6572 652c  nning elsewhere,
-0000b390: 2074 6865 6e20 796f 7520 6361 6e20 7573   then you can us
-0000b3a0: 6520 606c 6c61 6d61 5f69 6e64 6578 2e6c  e `llama_index.l
-0000b3b0: 6c6d 732e 6f70 656e 6c6c 6d2e 4f70 656e  lms.openllm.Open
-0000b3c0: 4c4c 4d41 5049 603a 0a0a 6060 6070 7974  LLMAPI`:..```pyt
-0000b3d0: 686f 6e0a 6672 6f6d 206c 6c61 6d61 5f69  hon.from llama_i
-0000b3e0: 6e64 6578 2e6c 6c6d 732e 6f70 656e 6c6c  ndex.llms.openll
-0000b3f0: 6d20 696d 706f 7274 204f 7065 6e4c 4c4d  m import OpenLLM
-0000b400: 4150 490a 6060 600a 0a3e 205b 214e 4f54  API.```..> [!NOT
-0000b410: 455d 0a3e 2041 6c6c 2073 796e 6368 726f  E].> All synchro
-0000b420: 6e6f 7573 2061 6e64 2061 7379 6e63 6872  nous and asynchr
-0000b430: 6f6e 6f75 7320 4150 4920 6672 6f6d 2060  onous API from `
-0000b440: 6c6c 616d 615f 696e 6465 782e 6c6c 6d73  llama_index.llms
-0000b450: 2e4c 4c4d 6020 6172 6520 7375 7070 6f72  .LLM` are suppor
-0000b460: 7465 642e 0a0a 2323 2320 5b4c 616e 6743  ted...### [LangC
-0000b470: 6861 696e 5d28 6874 7470 733a 2f2f 7079  hain](https://py
-0000b480: 7468 6f6e 2e6c 616e 6763 6861 696e 2e63  thon.langchain.c
-0000b490: 6f6d 2f64 6f63 732f 6563 6f73 7973 7465  om/docs/ecosyste
-0000b4a0: 6d2f 696e 7465 6772 6174 696f 6e73 2f6f  m/integrations/o
-0000b4b0: 7065 6e6c 6c6d 290a 0a54 6f20 7175 6963  penllm)..To quic
-0000b4c0: 6b6c 7920 7374 6172 7420 6120 6c6f 6361  kly start a loca
-0000b4d0: 6c20 4c4c 4d20 7769 7468 2060 6c61 6e67  l LLM with `lang
-0000b4e0: 6368 6169 6e60 2c20 7369 6d70 6c79 2064  chain`, simply d
-0000b4f0: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
-0000b500: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-0000b510: 206c 616e 6763 6861 696e 2e6c 6c6d 7320   langchain.llms 
-0000b520: 696d 706f 7274 204f 7065 6e4c 4c4d 0a0a  import OpenLLM..
-0000b530: 6c6c 6d20 3d20 4f70 656e 4c4c 4d28 6d6f  llm = OpenLLM(mo
-0000b540: 6465 6c5f 6e61 6d65 3d27 6c6c 616d 6127  del_name='llama'
-0000b550: 2c20 6d6f 6465 6c5f 6964 3d27 6d65 7461  , model_id='meta
-0000b560: 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32 2d37  -llama/Llama-2-7
-0000b570: 622d 6866 2729 0a0a 6c6c 6d28 2757 6861  b-hf')..llm('Wha
-0000b580: 7420 6973 2074 6865 2064 6966 6665 7265  t is the differe
-0000b590: 6e63 6520 6265 7477 6565 6e20 6120 6475  nce between a du
-0000b5a0: 636b 2061 6e64 2061 2067 6f6f 7365 3f20  ck and a goose? 
-0000b5b0: 416e 6420 7768 7920 7468 6572 6520 6172  And why there ar
-0000b5c0: 6520 736f 206d 616e 7920 476f 6f73 6520  e so many Goose 
-0000b5d0: 696e 2043 616e 6164 613f 2729 0a60 6060  in Canada?').```
-0000b5e0: 0a0a 3e20 5b21 494d 504f 5254 414e 545d  ..> [!IMPORTANT]
-0000b5f0: 0a3e 2042 7920 6465 6661 756c 742c 204f  .> By default, O
-0000b600: 7065 6e4c 4c4d 2075 7365 2060 7361 6665  penLLM use `safe
-0000b610: 7465 6e73 6f72 7360 2066 6f72 6d61 7420  tensors` format 
-0000b620: 666f 7220 7361 7669 6e67 206d 6f64 656c  for saving model
-0000b630: 732e 0a3e 2049 6620 7468 6520 6d6f 6465  s..> If the mode
-0000b640: 6c20 646f 6573 6e27 7420 7375 7070 6f72  l doesn't suppor
-0000b650: 7420 7361 6665 7465 6e73 6f72 732c 206d  t safetensors, m
-0000b660: 616b 6520 7375 7265 2074 6f20 7061 7373  ake sure to pass
-0000b670: 0a3e 2060 7365 7269 616c 6973 6174 696f  .> `serialisatio
-0000b680: 6e3d 226c 6567 6163 7922 6020 746f 2075  n="legacy"` to u
-0000b690: 7365 2074 6865 206c 6567 6163 7920 5079  se the legacy Py
-0000b6a0: 546f 7263 6820 6269 6e20 666f 726d 6174  Torch bin format
-0000b6b0: 2e0a 0a60 6c61 6e67 6368 6169 6e2e 6c6c  ...`langchain.ll
-0000b6c0: 6d73 2e4f 7065 6e4c 4c4d 6020 6861 7320  ms.OpenLLM` has 
-0000b6d0: 7468 6520 6361 7061 6269 6c69 7479 2074  the capability t
-0000b6e0: 6f20 696e 7465 7261 6374 2077 6974 6820  o interact with 
-0000b6f0: 7265 6d6f 7465 204f 7065 6e4c 4c4d 0a53  remote OpenLLM.S
-0000b700: 6572 7665 722e 2047 6976 656e 2074 6865  erver. Given the
-0000b710: 7265 2069 7320 616e 204f 7065 6e4c 4c4d  re is an OpenLLM
-0000b720: 2073 6572 7665 7220 6465 706c 6f79 6564   server deployed
-0000b730: 2065 6c73 6577 6865 7265 2c20 796f 7520   elsewhere, you 
-0000b740: 6361 6e20 636f 6e6e 6563 7420 746f 0a69  can connect to.i
-0000b750: 7420 6279 2073 7065 6369 6679 696e 6720  t by specifying 
-0000b760: 6974 7320 5552 4c3a 0a0a 6060 6070 7974  its URL:..```pyt
-0000b770: 686f 6e0a 6672 6f6d 206c 616e 6763 6861  hon.from langcha
-0000b780: 696e 2e6c 6c6d 7320 696d 706f 7274 204f  in.llms import O
-0000b790: 7065 6e4c 4c4d 0a0a 6c6c 6d20 3d20 4f70  penLLM..llm = Op
-0000b7a0: 656e 4c4c 4d28 7365 7276 6572 5f75 726c  enLLM(server_url
-0000b7b0: 3d27 6874 7470 3a2f 2f34 342e 3233 2e31  ='http://44.23.1
-0000b7c0: 3233 2e31 3a33 3030 3027 2c20 7365 7276  23.1:3000', serv
-0000b7d0: 6572 5f74 7970 653d 2768 7474 7027 290a  er_type='http').
-0000b7e0: 6c6c 6d28 2757 6861 7420 6973 2074 6865  llm('What is the
-0000b7f0: 2064 6966 6665 7265 6e63 6520 6265 7477   difference betw
-0000b800: 6565 6e20 6120 6475 636b 2061 6e64 2061  een a duck and a
-0000b810: 2067 6f6f 7365 3f20 416e 6420 7768 7920   goose? And why 
-0000b820: 7468 6572 6520 6172 6520 736f 206d 616e  there are so man
-0000b830: 7920 476f 6f73 6520 696e 2043 616e 6164  y Goose in Canad
-0000b840: 613f 2729 0a60 6060 0a0a 546f 2069 6e74  a?').```..To int
-0000b850: 6567 7261 7465 2061 204c 616e 6743 6861  egrate a LangCha
-0000b860: 696e 2061 6765 6e74 2077 6974 6820 4265  in agent with Be
-0000b870: 6e74 6f4d 4c2c 2079 6f75 2063 616e 2064  ntoML, you can d
-0000b880: 6f20 7468 6520 666f 6c6c 6f77 696e 673a  o the following:
-0000b890: 0a0a 6060 6070 7974 686f 6e0a 6c6c 6d20  ..```python.llm 
-0000b8a0: 3d20 4f70 656e 4c4c 4d28 6d6f 6465 6c5f  = OpenLLM(model_
-0000b8b0: 6964 3d27 676f 6f67 6c65 2f66 6c61 6e2d  id='google/flan-
-0000b8c0: 7435 2d6c 6172 6765 272c 2065 6d62 6564  t5-large', embed
-0000b8d0: 6465 643d 4661 6c73 652c 2073 6572 6961  ded=False, seria
-0000b8e0: 6c69 7361 7469 6f6e 3d27 6c65 6761 6379  lisation='legacy
-0000b8f0: 2729 0a74 6f6f 6c73 203d 206c 6f61 645f  ').tools = load_
-0000b900: 746f 6f6c 7328 5b27 7365 7270 6170 6927  tools(['serpapi'
-0000b910: 2c20 276c 6c6d 2d6d 6174 6827 5d2c 206c  , 'llm-math'], l
-0000b920: 6c6d 3d6c 6c6d 290a 6167 656e 7420 3d20  lm=llm).agent = 
-0000b930: 696e 6974 6961 6c69 7a65 5f61 6765 6e74  initialize_agent
-0000b940: 2874 6f6f 6c73 2c20 6c6c 6d2c 2061 6765  (tools, llm, age
-0000b950: 6e74 3d41 6765 6e74 5479 7065 2e5a 4552  nt=AgentType.ZER
-0000b960: 4f5f 5348 4f54 5f52 4541 4354 5f44 4553  O_SHOT_REACT_DES
-0000b970: 4352 4950 5449 4f4e 290a 7376 6320 3d20  CRIPTION).svc = 
-0000b980: 6265 6e74 6f6d 6c2e 5365 7276 6963 6528  bentoml.Service(
-0000b990: 276c 616e 6763 6861 696e 2d6f 7065 6e6c  'langchain-openl
-0000b9a0: 6c6d 272c 2072 756e 6e65 7273 3d5b 6c6c  lm', runners=[ll
-0000b9b0: 6d2e 7275 6e6e 6572 5d29 0a0a 0a40 7376  m.runner])...@sv
-0000b9c0: 632e 6170 6928 696e 7075 743d 5465 7874  c.api(input=Text
-0000b9d0: 2829 2c20 6f75 7470 7574 3d54 6578 7428  (), output=Text(
-0000b9e0: 2929 0a64 6566 2063 6861 7428 696e 7075  )).def chat(inpu
-0000b9f0: 745f 7465 7874 3a20 7374 7229 3a0a 2020  t_text: str):.  
-0000ba00: 7265 7475 726e 2061 6765 6e74 2e72 756e  return agent.run
-0000ba10: 2869 6e70 7574 5f74 6578 7429 0a60 6060  (input_text).```
-0000ba20: 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20 596f  ..> [!NOTE].> Yo
-0000ba30: 7520 6361 6e20 6669 6e64 206f 7574 206d  u can find out m
-0000ba40: 6f72 6520 6578 616d 706c 6573 2075 6e64  ore examples und
-0000ba50: 6572 2074 6865 0a3e 205b 6578 616d 706c  er the.> [exampl
-0000ba60: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
-0000ba70: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
-0000ba80: 7065 6e4c 4c4d 2f74 7265 652f 6d61 696e  penLLM/tree/main
-0000ba90: 2f65 7861 6d70 6c65 7329 2066 6f6c 6465  /examples) folde
-0000baa0: 722e 0a0a 2323 2320 5472 616e 7366 6f72  r...### Transfor
-0000bab0: 6d65 7273 2041 6765 6e74 730a 0a4f 7065  mers Agents..Ope
-0000bac0: 6e4c 4c4d 2073 6561 6d6c 6573 736c 7920  nLLM seamlessly 
-0000bad0: 696e 7465 6772 6174 6573 2077 6974 680a  integrates with.
-0000bae0: 5b54 7261 6e73 666f 726d 6572 7320 4167  [Transformers Ag
-0000baf0: 656e 7473 5d28 6874 7470 733a 2f2f 6875  ents](https://hu
-0000bb00: 6767 696e 6766 6163 652e 636f 2f64 6f63  ggingface.co/doc
-0000bb10: 732f 7472 616e 7366 6f72 6d65 7273 2f74  s/transformers/t
-0000bb20: 7261 6e73 666f 726d 6572 735f 6167 656e  ransformers_agen
-0000bb30: 7473 292e 0a0a 3e20 5b21 5741 524e 494e  ts)...> [!WARNIN
-0000bb40: 475d 0a3e 2054 6865 2054 7261 6e73 666f  G].> The Transfo
-0000bb50: 726d 6572 7320 4167 656e 7420 6973 2073  rmers Agent is s
-0000bb60: 7469 6c6c 2061 7420 616e 2065 7870 6572  till at an exper
-0000bb70: 696d 656e 7461 6c20 7374 6167 652e 2049  imental stage. I
-0000bb80: 7420 6973 0a3e 2072 6563 6f6d 6d65 6e64  t is.> recommend
-0000bb90: 6564 2074 6f20 696e 7374 616c 6c20 4f70  ed to install Op
-0000bba0: 656e 4c4c 4d20 7769 7468 2060 7069 7020  enLLM with `pip 
-0000bbb0: 696e 7374 616c 6c20 2d72 206e 6967 6874  install -r night
-0000bbc0: 6c79 2d72 6571 7569 7265 6d65 6e74 732e  ly-requirements.
-0000bbd0: 7478 7460 0a3e 2074 6f20 6765 7420 7468  txt`.> to get th
-0000bbe0: 6520 6c61 7465 7374 2041 5049 2075 7064  e latest API upd
-0000bbf0: 6174 6520 666f 7220 4875 6767 696e 6746  ate for HuggingF
-0000bc00: 6163 6520 6167 656e 742e 0a0a 6060 6070  ace agent...```p
-0000bc10: 7974 686f 6e0a 696d 706f 7274 2074 7261  ython.import tra
-0000bc20: 6e73 666f 726d 6572 730a 0a61 6765 6e74  nsformers..agent
-0000bc30: 203d 2074 7261 6e73 666f 726d 6572 732e   = transformers.
-0000bc40: 4866 4167 656e 7428 2768 7474 703a 2f2f  HfAgent('http://
-0000bc50: 6c6f 6361 6c68 6f73 743a 3330 3030 2f68  localhost:3000/h
-0000bc60: 662f 6167 656e 7427 2920 2023 2055 524c  f/agent')  # URL
-0000bc70: 2074 6861 7420 7275 6e73 2074 6865 204f   that runs the O
-0000bc80: 7065 6e4c 4c4d 2073 6572 7665 720a 0a61  penLLM server..a
-0000bc90: 6765 6e74 2e72 756e 2827 4973 2074 6865  gent.run('Is the
-0000bca0: 2066 6f6c 6c6f 7769 6e67 2060 7465 7874   following `text
-0000bcb0: 6020 706f 7369 7469 7665 206f 7220 6e65  ` positive or ne
-0000bcc0: 6761 7469 7665 3f27 2c20 7465 7874 3d22  gative?', text="
-0000bcd0: 4920 646f 6e27 7420 6c69 6b65 2068 6f77  I don't like how
-0000bce0: 2074 6869 7320 6d6f 6465 6c73 2069 7320   this models is 
-0000bcf0: 6765 6e65 7261 7465 2069 6e70 7574 7322  generate inputs"
-0000bd00: 290a 6060 600a 0a3c 7020 616c 6967 6e3d  ).```..<p align=
-0000bd10: 2263 656e 7465 7222 3e0a 2020 3c69 6d67  "center">.  <img
-0000bd20: 2073 7263 3d22 6874 7470 733a 2f2f 7261   src="https://ra
-0000bd30: 772e 6769 7468 7562 7573 6572 636f 6e74  w.githubusercont
-0000bd40: 656e 742e 636f 6d2f 6265 6e74 6f6d 6c2f  ent.com/bentoml/
-0000bd50: 6f70 656e 6c6c 6d2f 6d61 696e 2f2e 6769  openllm/main/.gi
-0000bd60: 7468 7562 2f61 7373 6574 732f 6167 656e  thub/assets/agen
-0000bd70: 742e 6769 6622 2061 6c74 3d22 4769 6620  t.gif" alt="Gif 
-0000bd80: 7368 6f77 696e 6720 4167 656e 7420 696e  showing Agent in
-0000bd90: 7465 6772 6174 696f 6e22 202f 3e0a 3c2f  tegration" />.</
-0000bda0: 703e 0a0a 2323 20f0 9f9a 8020 4465 706c  p>..## .... Depl
-0000bdb0: 6f79 696e 6720 6d6f 6465 6c73 2074 6f20  oying models to 
-0000bdc0: 7072 6f64 7563 7469 6f6e 0a0a 5468 6572  production..Ther
-0000bdd0: 6520 6172 6520 7365 7665 7261 6c20 7761  e are several wa
-0000bde0: 7973 2074 6f20 6465 706c 6f79 2079 6f75  ys to deploy you
-0000bdf0: 7220 4c4c 4d73 3a0a 0a23 2323 20f0 9f90  r LLMs:..### ...
-0000be00: b320 446f 636b 6572 2063 6f6e 7461 696e  . Docker contain
-0000be10: 6572 0a0a 312e 202a 2a42 7569 6c64 696e  er..1. **Buildin
-0000be20: 6720 6120 4265 6e74 6f2a 2a3a 2057 6974  g a Bento**: Wit
-0000be30: 6820 4f70 656e 4c4c 4d2c 2079 6f75 2063  h OpenLLM, you c
-0000be40: 616e 2065 6173 696c 7920 6275 696c 6420  an easily build 
-0000be50: 6120 4265 6e74 6f20 666f 7220 610a 2020  a Bento for a.  
-0000be60: 2073 7065 6369 6669 6320 6d6f 6465 6c2c   specific model,
-0000be70: 206c 696b 6520 606d 6973 7472 616c 6169   like `mistralai
-0000be80: 2f4d 6973 7472 616c 2d37 422d 496e 7374  /Mistral-7B-Inst
-0000be90: 7275 6374 2d76 302e 3160 2c20 7573 696e  ruct-v0.1`, usin
-0000bea0: 6720 7468 6520 6062 7569 6c64 6020 636f  g the `build` co
-0000beb0: 6d6d 616e 642e 3a0a 0a20 2020 6060 6062  mmand.:..   ```b
-0000bec0: 6173 680a 2020 206f 7065 6e6c 6c6d 2062  ash.   openllm b
-0000bed0: 7569 6c64 206d 6973 7472 616c 6169 2f4d  uild mistralai/M
-0000bee0: 6973 7472 616c 2d37 422d 496e 7374 7275  istral-7B-Instru
-0000bef0: 6374 2d76 302e 310a 2020 2060 6060 0a0a  ct-v0.1.   ```..
-0000bf00: 2020 2041 0a20 2020 5b42 656e 746f 5d28     A.   [Bento](
-0000bf10: 6874 7470 733a 2f2f 646f 6373 2e62 656e  https://docs.ben
-0000bf20: 746f 6d6c 2e63 6f6d 2f65 6e2f 6c61 7465  toml.com/en/late
-0000bf30: 7374 2f63 6f6e 6365 7074 732f 6265 6e74  st/concepts/bent
-0000bf40: 6f2e 6874 6d6c 2377 6861 742d 6973 2d61  o.html#what-is-a
-0000bf50: 2d62 656e 746f 292c 0a20 2020 696e 2042  -bento),.   in B
-0000bf60: 656e 746f 4d4c 2c20 6973 2074 6865 2075  entoML, is the u
-0000bf70: 6e69 7420 6f66 2064 6973 7472 6962 7574  nit of distribut
-0000bf80: 696f 6e2e 2049 7420 7061 636b 6167 6573  ion. It packages
-0000bf90: 2079 6f75 7220 7072 6f67 7261 6d27 7320   your program's 
-0000bfa0: 736f 7572 6365 0a20 2020 636f 6465 2c20  source.   code, 
-0000bfb0: 6d6f 6465 6c73 2c20 6669 6c65 732c 2061  models, files, a
-0000bfc0: 7274 6566 6163 7473 2c20 616e 6420 6465  rtefacts, and de
-0000bfd0: 7065 6e64 656e 6369 6573 2e0a 0a32 2e20  pendencies...2. 
-0000bfe0: 2a2a 436f 6e74 6169 6e65 7269 7a65 2079  **Containerize y
-0000bff0: 6f75 7220 4265 6e74 6f2a 2a0a 0a20 2020  our Bento**..   
-0000c000: 6060 6062 6173 680a 2020 2062 656e 746f  ```bash.   bento
-0000c010: 6d6c 2063 6f6e 7461 696e 6572 697a 6520  ml containerize 
-0000c020: 3c6e 616d 653a 7665 7273 696f 6e3e 0a20  <name:version>. 
-0000c030: 2020 6060 600a 0a20 2020 5468 6973 2067    ```..   This g
-0000c040: 656e 6572 6174 6573 2061 204f 4349 2d63  enerates a OCI-c
-0000c050: 6f6d 7061 7469 626c 6520 646f 636b 6572  ompatible docker
-0000c060: 2069 6d61 6765 2074 6861 7420 6361 6e20   image that can 
-0000c070: 6265 2064 6570 6c6f 7965 6420 616e 7977  be deployed anyw
-0000c080: 6865 7265 0a20 2020 646f 636b 6572 2072  here.   docker r
-0000c090: 756e 732e 2046 6f72 2062 6573 7420 7363  uns. For best sc
-0000c0a0: 616c 6162 696c 6974 7920 616e 6420 7265  alability and re
-0000c0b0: 6c69 6162 696c 6974 7920 6f66 2079 6f75  liability of you
-0000c0c0: 7220 4c4c 4d20 7365 7276 6963 6520 696e  r LLM service in
-0000c0d0: 0a20 2020 7072 6f64 7563 7469 6f6e 2c20  .   production, 
-0000c0e0: 7765 2072 6563 6f6d 6d65 6e64 2064 6570  we recommend dep
-0000c0f0: 6c6f 7920 7769 7468 2042 656e 746f 436c  loy with BentoCl
-0000c100: 6f75 64e3 8082 0a0a 2323 2320 e298 81ef  oud.....### ....
-0000c110: b88f 2042 656e 746f 436c 6f75 640a 0a44  .. BentoCloud..D
-0000c120: 6570 6c6f 7920 4f70 656e 4c4c 4d20 7769  eploy OpenLLM wi
-0000c130: 7468 205b 4265 6e74 6f43 6c6f 7564 5d28  th [BentoCloud](
-0000c140: 6874 7470 733a 2f2f 7777 772e 6265 6e74  https://www.bent
-0000c150: 6f6d 6c2e 636f 6d2f 6265 6e74 6f2d 636c  oml.com/bento-cl
-0000c160: 6f75 642f 292c 2074 6865 0a73 6572 7665  oud/), the.serve
-0000c170: 726c 6573 7320 636c 6f75 6420 666f 7220  rless cloud for 
-0000c180: 7368 6970 7069 6e67 2061 6e64 2073 6361  shipping and sca
-0000c190: 6c69 6e67 2041 4920 6170 706c 6963 6174  ling AI applicat
-0000c1a0: 696f 6e73 2e0a 0a31 2e20 2a2a 4372 6561  ions...1. **Crea
-0000c1b0: 7465 2061 2042 656e 746f 436c 6f75 6420  te a BentoCloud 
-0000c1c0: 6163 636f 756e 743a 2a2a 205b 7369 676e  account:** [sign
-0000c1d0: 2075 7020 6865 7265 5d28 6874 7470 733a   up here](https:
-0000c1e0: 2f2f 6265 6e74 6f6d 6c2e 636f 6d2f 636c  //bentoml.com/cl
-0000c1f0: 6f75 6429 0a20 2020 666f 7220 6561 726c  oud).   for earl
-0000c200: 7920 6163 6365 7373 0a0a 322e 202a 2a4c  y access..2. **L
-0000c210: 6f67 2069 6e74 6f20 796f 7572 2042 656e  og into your Ben
-0000c220: 746f 436c 6f75 6420 6163 636f 756e 743a  toCloud account:
-0000c230: 2a2a 0a0a 2020 2060 6060 6261 7368 0a20  **..   ```bash. 
-0000c240: 2020 6265 6e74 6f6d 6c20 636c 6f75 6420    bentoml cloud 
-0000c250: 6c6f 6769 6e20 2d2d 6170 692d 746f 6b65  login --api-toke
-0000c260: 6e20 3c79 6f75 722d 6170 692d 746f 6b65  n <your-api-toke
-0000c270: 6e3e 202d 2d65 6e64 706f 696e 7420 3c62  n> --endpoint <b
-0000c280: 656e 746f 2d63 6c6f 7564 2d65 6e64 706f  ento-cloud-endpo
-0000c290: 696e 743e 0a20 2020 6060 600a 0a3e 205b  int>.   ```..> [
-0000c2a0: 214e 4f54 455d 0a3e 2052 6570 6c61 6365  !NOTE].> Replace
-0000c2b0: 2060 3c79 6f75 722d 6170 692d 746f 6b65   `<your-api-toke
-0000c2c0: 6e3e 6020 616e 6420 603c 6265 6e74 6f2d  n>` and `<bento-
-0000c2d0: 636c 6f75 642d 656e 6470 6f69 6e74 3e60  cloud-endpoint>`
-0000c2e0: 2077 6974 6820 796f 7572 0a3e 2073 7065   with your.> spe
-0000c2f0: 6369 6669 6320 4150 4920 746f 6b65 6e20  cific API token 
-0000c300: 616e 6420 7468 6520 4265 6e74 6f43 6c6f  and the BentoClo
-0000c310: 7564 2065 6e64 706f 696e 7420 7265 7370  ud endpoint resp
-0000c320: 6563 7469 7665 6c79 2e0a 0a33 2e20 2a2a  ectively...3. **
-0000c330: 4275 6c64 696e 6720 6120 4265 6e74 6f2a  Bulding a Bento*
-0000c340: 2a3a 2057 6974 6820 4f70 656e 4c4c 4d2c  *: With OpenLLM,
-0000c350: 2079 6f75 2063 616e 2065 6173 696c 7920   you can easily 
-0000c360: 6275 696c 6420 6120 4265 6e74 6f20 666f  build a Bento fo
-0000c370: 7220 610a 2020 2073 7065 6369 6669 6320  r a.   specific 
-0000c380: 6d6f 6465 6c2c 2073 7563 6820 6173 2060  model, such as `
-0000c390: 6d69 7374 7261 6c61 692f 4d69 7374 7261  mistralai/Mistra
-0000c3a0: 6c2d 3742 2d49 6e73 7472 7563 742d 7630  l-7B-Instruct-v0
-0000c3b0: 2e31 603a 0a0a 2020 2060 6060 6261 7368  .1`:..   ```bash
-0000c3c0: 0a20 2020 6f70 656e 6c6c 6d20 6275 696c  .   openllm buil
-0000c3d0: 6420 6d69 7374 7261 6c61 692f 4d69 7374  d mistralai/Mist
-0000c3e0: 7261 6c2d 3742 2d49 6e73 7472 7563 742d  ral-7B-Instruct-
-0000c3f0: 7630 2e31 0a20 2020 6060 600a 0a34 2e20  v0.1.   ```..4. 
-0000c400: 2a2a 5075 7368 696e 6720 6120 4265 6e74  **Pushing a Bent
-0000c410: 6f2a 2a3a 2050 7573 6820 796f 7572 2066  o**: Push your f
-0000c420: 7265 7368 6c79 2d62 7569 6c74 2042 656e  reshly-built Ben
-0000c430: 746f 2073 6572 7669 6365 2074 6f20 4265  to service to Be
-0000c440: 6e74 6f43 6c6f 7564 2076 6961 0a20 2020  ntoCloud via.   
-0000c450: 7468 6520 6070 7573 6860 2063 6f6d 6d61  the `push` comma
-0000c460: 6e64 3a0a 0a20 2020 6060 6062 6173 680a  nd:..   ```bash.
-0000c470: 2020 2062 656e 746f 6d6c 2070 7573 6820     bentoml push 
-0000c480: 3c6e 616d 653a 7665 7273 696f 6e3e 0a20  <name:version>. 
-0000c490: 2020 6060 600a 0a35 2e20 2a2a 4465 706c    ```..5. **Depl
-0000c4a0: 6f79 696e 6720 6120 4265 6e74 6f2a 2a3a  oying a Bento**:
-0000c4b0: 2044 6570 6c6f 7920 796f 7572 204c 4c4d   Deploy your LLM
-0000c4c0: 7320 746f 2042 656e 746f 436c 6f75 6420  s to BentoCloud 
-0000c4d0: 7769 7468 2061 2073 696e 676c 650a 2020  with a single.  
-0000c4e0: 2060 6265 6e74 6f6d 6c20 6465 706c 6f79   `bentoml deploy
-0000c4f0: 6d65 6e74 2063 7265 6174 6560 2063 6f6d  ment create` com
-0000c500: 6d61 6e64 2066 6f6c 6c6f 7769 6e67 2074  mand following t
-0000c510: 6865 0a20 2020 5b64 6570 6c6f 796d 656e  he.   [deploymen
-0000c520: 7420 696e 7374 7275 6374 696f 6e73 5d28  t instructions](
-0000c530: 6874 7470 733a 2f2f 646f 6373 2e62 656e  https://docs.ben
-0000c540: 746f 6d6c 2e63 6f6d 2f65 6e2f 6c61 7465  toml.com/en/late
-0000c550: 7374 2f72 6566 6572 656e 6365 2f63 6c69  st/reference/cli
-0000c560: 2e68 746d 6c23 6265 6e74 6f6d 6c2d 6465  .html#bentoml-de
-0000c570: 706c 6f79 6d65 6e74 2d63 7265 6174 6529  ployment-create)
-0000c580: 2e0a 0a23 2320 f09f 91a5 2043 6f6d 6d75  ...## .... Commu
-0000c590: 6e69 7479 0a0a 456e 6761 6765 2077 6974  nity..Engage wit
-0000c5a0: 6820 6c69 6b65 2d6d 696e 6465 6420 696e  h like-minded in
-0000c5b0: 6469 7669 6475 616c 7320 7061 7373 696f  dividuals passio
-0000c5c0: 6e61 7465 2061 626f 7574 204c 4c4d 732c  nate about LLMs,
-0000c5d0: 2041 492c 2061 6e64 206d 6f72 6520 6f6e   AI, and more on
-0000c5e0: 206f 7572 0a5b 4469 7363 6f72 645d 2868   our.[Discord](h
-0000c5f0: 7474 7073 3a2f 2f6c 2e62 656e 746f 6d6c  ttps://l.bentoml
-0000c600: 2e63 6f6d 2f6a 6f69 6e2d 6f70 656e 6c6c  .com/join-openll
-0000c610: 6d2d 6469 7363 6f72 6429 210a 0a4f 7065  m-discord)!..Ope
-0000c620: 6e4c 4c4d 2069 7320 6163 7469 7665 6c79  nLLM is actively
-0000c630: 206d 6169 6e74 6169 6e65 6420 6279 2074   maintained by t
-0000c640: 6865 2042 656e 746f 4d4c 2074 6561 6d2e  he BentoML team.
-0000c650: 2046 6565 6c20 6672 6565 2074 6f20 7265   Feel free to re
-0000c660: 6163 6820 6f75 7420 616e 640a 6a6f 696e  ach out and.join
-0000c670: 2075 7320 696e 206f 7572 2070 7572 7375   us in our pursu
-0000c680: 6974 2074 6f20 6d61 6b65 204c 4c4d 7320  it to make LLMs 
-0000c690: 6d6f 7265 2061 6363 6573 7369 626c 6520  more accessible 
-0000c6a0: 616e 6420 6561 7379 2074 6f20 7573 6520  and easy to use 
-0000c6b0: f09f 9189 0a5b 4a6f 696e 206f 7572 2053  .....[Join our S
-0000c6c0: 6c61 636b 2063 6f6d 6d75 6e69 7479 215d  lack community!]
-0000c6d0: 2868 7474 7073 3a2f 2f6c 2e62 656e 746f  (https://l.bento
-0000c6e0: 6d6c 2e63 6f6d 2f6a 6f69 6e2d 736c 6163  ml.com/join-slac
-0000c6f0: 6b29 0a0a 2323 20f0 9f8e 8120 436f 6e74  k)..## .... Cont
-0000c700: 7269 6275 7469 6e67 0a0a 5765 2077 656c  ributing..We wel
-0000c710: 636f 6d65 2063 6f6e 7472 6962 7574 696f  come contributio
-0000c720: 6e73 2120 4966 2079 6f75 2772 6520 696e  ns! If you're in
-0000c730: 7465 7265 7374 6564 2069 6e20 656e 6861  terested in enha
-0000c740: 6e63 696e 6720 4f70 656e 4c4c 4d27 730a  ncing OpenLLM's.
-0000c750: 6361 7061 6269 6c69 7469 6573 206f 7220  capabilities or 
-0000c760: 6861 7665 2061 6e79 2071 7565 7374 696f  have any questio
-0000c770: 6e73 2c20 646f 6e27 7420 6865 7369 7461  ns, don't hesita
-0000c780: 7465 2074 6f20 7265 6163 6820 6f75 7420  te to reach out 
-0000c790: 696e 206f 7572 0a5b 6469 7363 6f72 6420  in our.[discord 
-0000c7a0: 6368 616e 6e65 6c5d 2868 7474 7073 3a2f  channel](https:/
-0000c7b0: 2f6c 2e62 656e 746f 6d6c 2e63 6f6d 2f6a  /l.bentoml.com/j
-0000c7c0: 6f69 6e2d 6f70 656e 6c6c 6d2d 6469 7363  oin-openllm-disc
-0000c7d0: 6f72 6429 2e0a 0a43 6865 636b 6f75 7420  ord)...Checkout 
-0000c7e0: 6f75 720a 5b44 6576 656c 6f70 6572 2047  our.[Developer G
-0000c7f0: 7569 6465 5d28 6874 7470 733a 2f2f 6769  uide](https://gi
-0000c800: 7468 7562 2e63 6f6d 2f62 656e 746f 6d6c  thub.com/bentoml
-0000c810: 2f4f 7065 6e4c 4c4d 2f62 6c6f 622f 6d61  /OpenLLM/blob/ma
-0000c820: 696e 2f44 4556 454c 4f50 4d45 4e54 2e6d  in/DEVELOPMENT.m
-0000c830: 6429 0a69 6620 796f 7520 7769 7368 2074  d).if you wish t
-0000c840: 6f20 636f 6e74 7269 6275 7465 2074 6f20  o contribute to 
-0000c850: 4f70 656e 4c4c 4d27 7320 636f 6465 6261  OpenLLM's codeba
-0000c860: 7365 2e0a 0a23 2320 f09f 8d87 2054 656c  se...## .... Tel
-0000c870: 656d 6574 7279 0a0a 4f70 656e 4c4c 4d20  emetry..OpenLLM 
-0000c880: 636f 6c6c 6563 7473 2075 7361 6765 2064  collects usage d
-0000c890: 6174 6120 746f 2065 6e68 616e 6365 2075  ata to enhance u
-0000c8a0: 7365 7220 6578 7065 7269 656e 6365 2061  ser experience a
-0000c8b0: 6e64 2069 6d70 726f 7665 2074 6865 2070  nd improve the p
-0000c8c0: 726f 6475 6374 2e0a 5765 206f 6e6c 7920  roduct..We only 
-0000c8d0: 7265 706f 7274 204f 7065 6e4c 4c4d 2773  report OpenLLM's
-0000c8e0: 2069 6e74 6572 6e61 6c20 4150 4920 6361   internal API ca
-0000c8f0: 6c6c 7320 616e 6420 656e 7375 7265 206d  lls and ensure m
-0000c900: 6178 696d 756d 2070 7269 7661 6379 2062  aximum privacy b
-0000c910: 790a 6578 636c 7564 696e 6720 7365 6e73  y.excluding sens
-0000c920: 6974 6976 6520 696e 666f 726d 6174 696f  itive informatio
-0000c930: 6e2e 2057 6520 7769 6c6c 206e 6576 6572  n. We will never
-0000c940: 2063 6f6c 6c65 6374 2075 7365 7220 636f   collect user co
-0000c950: 6465 2c20 6d6f 6465 6c20 6461 7461 2c20  de, model data, 
-0000c960: 6f72 0a73 7461 636b 2074 7261 6365 732e  or.stack traces.
-0000c970: 2046 6f72 2075 7361 6765 2074 7261 636b   For usage track
-0000c980: 696e 672c 2063 6865 636b 206f 7574 2074  ing, check out t
-0000c990: 6865 0a5b 636f 6465 5d28 6874 7470 733a  he.[code](https:
-0000c9a0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
-0000c9b0: 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62 6c6f  toml/OpenLLM/blo
-0000c9c0: 622f 6d61 696e 2f6f 7065 6e6c 6c6d 2d63  b/main/openllm-c
-0000c9d0: 6f72 652f 7372 632f 6f70 656e 6c6c 6d5f  ore/src/openllm_
-0000c9e0: 636f 7265 2f75 7469 6c73 2f61 6e61 6c79  core/utils/analy
-0000c9f0: 7469 6373 2e70 7929 2e0a 0a59 6f75 2063  tics.py)...You c
-0000ca00: 616e 206f 7074 206f 7574 206f 6620 7573  an opt out of us
-0000ca10: 6167 6520 7472 6163 6b69 6e67 2062 7920  age tracking by 
-0000ca20: 7573 696e 6720 7468 6520 602d 2d64 6f2d  using the `--do-
-0000ca30: 6e6f 742d 7472 6163 6b60 2043 4c49 206f  not-track` CLI o
-0000ca40: 7074 696f 6e3a 0a0a 6060 6062 6173 680a  ption:..```bash.
-0000ca50: 6f70 656e 6c6c 6d20 5b63 6f6d 6d61 6e64  openllm [command
-0000ca60: 5d20 2d2d 646f 2d6e 6f74 2d74 7261 636b  ] --do-not-track
-0000ca70: 0a60 6060 0a0a 4f72 2062 7920 7365 7474  .```..Or by sett
-0000ca80: 696e 6720 7468 6520 656e 7669 726f 6e6d  ing the environm
-0000ca90: 656e 7420 7661 7269 6162 6c65 2060 4f50  ent variable `OP
-0000caa0: 454e 4c4c 4d5f 444f 5f4e 4f54 5f54 5241  ENLLM_DO_NOT_TRA
-0000cab0: 434b 3d54 7275 6560 3a0a 0a60 6060 6261  CK=True`:..```ba
-0000cac0: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
-0000cad0: 4d5f 444f 5f4e 4f54 5f54 5241 434b 3d54  M_DO_NOT_TRACK=T
-0000cae0: 7275 650a 6060 600a 0a23 2320 f09f 9394  rue.```..## ....
-0000caf0: 2043 6974 6174 696f 6e0a 0a49 6620 796f   Citation..If yo
-0000cb00: 7520 7573 6520 4f70 656e 4c4c 4d20 696e  u use OpenLLM in
-0000cb10: 2079 6f75 7220 7265 7365 6172 6368 2c20   your research, 
-0000cb20: 7765 2070 726f 7669 6465 2061 205b 6369  we provide a [ci
-0000cb30: 7461 7469 6f6e 5d28 2e2f 4349 5441 5449  tation](./CITATI
-0000cb40: 4f4e 2e63 6666 2920 746f 0a75 7365 3a0a  ON.cff) to.use:.
-0000cb50: 0a60 6060 6269 6274 6578 0a40 736f 6674  .```bibtex.@soft
-0000cb60: 7761 7265 7b50 6861 6d5f 4f70 656e 4c4c  ware{Pham_OpenLL
-0000cb70: 4d5f 4f70 6572 6174 696e 675f 4c4c 4d73  M_Operating_LLMs
-0000cb80: 5f32 3032 332c 0a61 7574 686f 7220 3d20  _2023,.author = 
-0000cb90: 7b50 6861 6d2c 2041 6172 6f6e 2061 6e64  {Pham, Aaron and
-0000cba0: 2059 616e 672c 2043 6861 6f79 7520 616e   Yang, Chaoyu an
-0000cbb0: 6420 5368 656e 672c 2053 6561 6e20 616e  d Sheng, Sean an
-0000cbc0: 6420 205a 6861 6f2c 2053 6865 6e79 616e  d  Zhao, Shenyan
-0000cbd0: 6720 616e 6420 4c65 652c 2053 6175 796f  g and Lee, Sauyo
-0000cbe0: 6e20 616e 6420 4a69 616e 672c 2042 6f20  n and Jiang, Bo 
-0000cbf0: 616e 6420 446f 6e67 2c20 466f 6720 616e  and Dong, Fog an
-0000cc00: 6420 4775 616e 2c20 5869 7065 6e67 2061  d Guan, Xipeng a
-0000cc10: 6e64 204d 696e 672c 2046 726f 7374 7d2c  nd Ming, Frost},
-0000cc20: 0a6c 6963 656e 7365 203d 207b 4170 6163  .license = {Apac
-0000cc30: 6865 2d32 2e30 7d2c 0a6d 6f6e 7468 203d  he-2.0},.month =
-0000cc40: 206a 756e 2c0a 7469 746c 6520 3d20 7b7b   jun,.title = {{
-0000cc50: 4f70 656e 4c4c 4d3a 204f 7065 7261 7469  OpenLLM: Operati
-0000cc60: 6e67 204c 4c4d 7320 696e 2070 726f 6475  ng LLMs in produ
-0000cc70: 6374 696f 6e7d 7d2c 0a75 726c 203d 207b  ction}},.url = {
-0000cc80: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-0000cc90: 6f6d 2f62 656e 746f 6d6c 2f4f 7065 6e4c  om/bentoml/OpenL
-0000cca0: 4c4d 7d2c 0a79 6561 7220 3d20 7b32 3032  LM},.year = {202
-0000ccb0: 337d 0a7d 0a60 6060 0a0a 2323 2052 656c  3}.}.```..## Rel
-0000ccc0: 6561 7365 2049 6e66 6f72 6d61 7469 6f6e  ease Information
-0000ccd0: 0a0a 2323 2320 4261 636b 7761 7264 732d  ..### Backwards-
-0000cce0: 696e 636f 6d70 6174 6962 6c65 2043 6861  incompatible Cha
-0000ccf0: 6e67 6573 0a0a 2d20 2323 2320 6f70 656e  nges..- ### open
-0000cd00: 6c6c 6d2d 636f 7265 0a0a 2020 4275 6d70  llm-core..  Bump
-0000cd10: 2060 6174 7472 7360 2074 6f20 6032 332e   `attrs` to `23.
-0000cd20: 322e 3060 0a0a 2020 4164 6465 6420 6578  2.0`..  Added ex
-0000cd30: 7065 7269 6d65 6e74 616c 2068 656c 7065  perimental helpe
-0000cd40: 7273 2060 2e70 7964 616e 7469 635f 6d6f  rs `.pydantic_mo
-0000cd50: 6465 6c28 2960 2066 756e 6374 696f 6e73  del()` functions
-0000cd60: 2074 6f20 636f 6e76 6572 7420 6375 7272   to convert curr
-0000cd70: 656e 7420 6174 7472 732d 6261 7365 6420  ent attrs-based 
-0000cd80: 636c 6173 7320 746f 2069 7473 2063 6f6d  class to its com
-0000cd90: 7061 7469 626c 6520 7079 6461 6e74 6963  patible pydantic
-0000cda0: 2063 6c61 7373 2e0a 0a20 2023 2323 206f   class...  ### o
-0000cdb0: 7065 6e6c 6c6d 0a0a 2020 5570 6461 7465  penllm..  Update
-0000cdc0: 6420 4f70 656e 4c4c 4d20 6172 6368 6974  d OpenLLM archit
-0000cdd0: 6563 7475 7265 2074 6f20 6e65 7720 312e  ecture to new 1.
-0000cde0: 3220 4265 6e74 6f4d 4c2e 0a0a 2020 606f  2 BentoML...  `o
-0000cdf0: 7065 6e6c 6c6d 2e52 756e 6e65 7260 2072  penllm.Runner` r
-0000ce00: 656d 6169 6e73 2074 6865 206f 6c64 2052  emains the old R
-0000ce10: 756e 6e61 626c 6520 696d 706c 656d 656e  unnable implemen
-0000ce20: 7461 7469 6f6e 2e20 5468 6572 6566 6f72  tation. Therefor
-0000ce30: 652c 2069 6620 796f 7520 7374 696c 6c20  e, if you still 
-0000ce40: 6465 7065 6e64 7320 6f6e 2074 6865 206f  depends on the o
-0000ce50: 6c64 2061 7263 6869 7465 6374 7572 652c  ld architecture,
-0000ce60: 206d 616b 6520 7375 7265 2074 6f20 7573   make sure to us
-0000ce70: 6520 606f 7065 6e6c 6c6d 2e52 756e 6e65  e `openllm.Runne
-0000ce80: 7260 2069 6e73 7465 6164 206f 6620 606c  r` instead of `l
-0000ce90: 6c6d 2e72 756e 6e65 7260 2e0a 0a20 2060  lm.runner`...  `
-0000cea0: 6c6c 6d2e 7275 6e6e 6572 6020 7769 6c6c  llm.runner` will
-0000ceb0: 206e 6f77 2062 6563 6f6d 6520 616e 2060   now become an `
-0000cec0: 6265 6e74 6f6d 6c2e 6465 7065 6e64 7328  bentoml.depends(
-0000ced0: 2960 2073 696e 676c 6574 6f6e 2c20 7468  )` singleton, th
-0000cee0: 6572 6566 6f72 652c 2074 6f20 6176 6f69  erefore, to avoi
-0000cef0: 6420 6272 6561 6b69 6e67 2063 6861 6e67  d breaking chang
-0000cf00: 652c 206d 616b 6520 7375 7265 2074 6f20  e, make sure to 
-0000cf10: 7365 7420 604f 5045 4e4c 4c4d 5f52 554e  set `OPENLLM_RUN
-0000cf20: 4e45 525f 4245 4841 5649 4f55 523d 6465  NER_BEHAVIOUR=de
-0000cf30: 7072 6563 6174 6564 6020 696e 2079 6f75  precated` in you
-0000cf40: 7220 656e 7669 726f 6e6d 656e 7420 7661  r environment va
-0000cf50: 7269 6162 6c65 2e20 5468 6973 2069 7320  riable. This is 
-0000cf60: 7468 6520 6465 6661 756c 7420 6265 6861  the default beha
-0000cf70: 7669 6f75 722e 2054 6f20 6f70 742d 696e  viour. To opt-in
-0000cf80: 2074 6865 206e 6577 2061 7263 6869 7465   the new archite
-0000cf90: 6374 7572 652c 2073 6574 2060 4f50 454e  cture, set `OPEN
-0000cfa0: 4c4c 4d5f 5255 4e4e 4552 5f42 4548 4156  LLM_RUNNER_BEHAV
-0000cfb0: 494f 5552 3d6e 6577 5f69 6d70 6c60 0a20  IOUR=new_impl`. 
-0000cfc0: 205b 2338 3231 5d28 6874 7470 733a 2f2f   [#821](https://
-0000cfd0: 6769 7468 7562 2e63 6f6d 2f62 656e 746f  github.com/bento
-0000cfe0: 6d6c 2f6f 7065 6e6c 6c6d 2f69 7373 7565  ml/openllm/issue
-0000cff0: 732f 3832 3129 0a0a 0a2d 2d2d 0a0a 5b43  s/821)...---..[C
-0000d000: 6c69 636b 206d 6520 666f 7220 6675 6c6c  lick me for full
-0000d010: 2063 6861 6e67 656c 6f67 5d28 6874 7470   changelog](http
-0000d020: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
-0000d030: 656e 746f 6d6c 2f6f 7065 6e6c 6c6d 2f62  entoml/openllm/b
-0000d040: 6c6f 622f 6d61 696e 2f43 4841 4e47 454c  lob/main/CHANGEL
-0000d050: 4f47 2e6d 6429 0a                        OG.md).
+00000000: 215b 4261 6e6e 6572 2066 6f72 204f 7065  ![Banner for Ope
+00000010: 6e4c 4c4d 5d28 2f2e 6769 7468 7562 2f61  nLLM](/.github/a
+00000020: 7373 6574 732f 6d61 696e 2d62 616e 6e65  ssets/main-banne
+00000030: 722e 706e 6729 0a0a 3c21 2d2d 2068 6174  r.png)..<!-- hat
+00000040: 6368 2d66 616e 6379 2d70 7970 692d 7265  ch-fancy-pypi-re
+00000050: 6164 6d65 2069 6e74 726f 2073 7461 7274  adme intro start
+00000060: 202d 2d3e 0a0a 3c64 6976 2061 6c69 676e   -->..<div align
+00000070: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00000080: 6831 2061 6c69 676e 3d22 6365 6e74 6572  h1 align="center
+00000090: 223e f09f a6be 204f 7065 6e4c 4c4d 3a20  ">.... OpenLLM: 
+000000a0: 5365 6c66 2d48 6f73 7469 6e67 204c 4c4d  Self-Hosting LLM
+000000b0: 7320 4d61 6465 2045 6173 793c 2f68 313e  s Made Easy</h1>
+000000c0: 0a20 2020 203c 6120 6872 6566 3d22 6874  .    <a href="ht
+000000d0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000000e0: 726f 6a65 6374 2f6f 7065 6e6c 6c6d 223e  roject/openllm">
+000000f0: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
+00000100: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000110: 6869 656c 6473 2e69 6f2f 7079 7069 2f76  hields.io/pypi/v
+00000120: 2f6f 7065 6e6c 6c6d 2e73 7667 3f6c 6f67  /openllm.svg?log
+00000130: 6f3d 7079 7069 266c 6162 656c 3d50 7950  o=pypi&label=PyP
+00000140: 4926 6c6f 676f 436f 6c6f 723d 676f 6c64  I&logoColor=gold
+00000150: 2220 616c 743d 2270 7970 695f 7374 6174  " alt="pypi_stat
+00000160: 7573 2220 2f3e 0a20 2020 203c 2f61 3e3c  us" />.    </a><
+00000170: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000180: 7465 7374 2e70 7970 692e 6f72 672f 7072  test.pypi.org/pr
+00000190: 6f6a 6563 742f 6f70 656e 6c6c 6d2f 223e  oject/openllm/">
+000001a0: 0a20 2020 2020 2020 203c 696d 6720 7372  .        <img sr
+000001b0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+000001c0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000001d0: 4e69 6768 746c 792d 5079 5049 3f6c 6f67  Nightly-PyPI?log
+000001e0: 6f3d 7079 7069 266c 6162 656c 3d50 7950  o=pypi&label=PyP
+000001f0: 4926 636f 6c6f 723d 6772 6179 266c 696e  I&color=gray&lin
+00000200: 6b3d 6874 7470 7325 3341 2532 4625 3246  k=https%3A%2F%2F
+00000210: 7465 7374 2e70 7970 692e 6f72 6725 3246  test.pypi.org%2F
+00000220: 7072 6f6a 6563 7425 3246 6f70 656e 6c6c  project%2Fopenll
+00000230: 6d25 3246 2220 616c 743d 2274 6573 745f  m%2F" alt="test_
+00000240: 7079 7069 5f73 7461 7475 7322 202f 3e0a  pypi_status" />.
+00000250: 2020 2020 3c2f 613e 3c61 2068 7265 663d      </a><a href=
+00000260: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000270: 636f 6d2f 6265 6e74 6f6d 6c2f 4f70 656e  com/bentoml/Open
+00000280: 4c4c 4d2f 6163 7469 6f6e 732f 776f 726b  LLM/actions/work
+00000290: 666c 6f77 732f 6369 2e79 6d6c 223e 0a20  flows/ci.yml">. 
+000002a0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000002b0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002c0: 636f 6d2f 6265 6e74 6f6d 6c2f 4f70 656e  com/bentoml/Open
+000002d0: 4c4c 4d2f 6163 7469 6f6e 732f 776f 726b  LLM/actions/work
+000002e0: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
+000002f0: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000300: 696e 2220 616c 743d 2263 6922 202f 3e0a  in" alt="ci" />.
+00000310: 2020 2020 3c2f 613e 3c61 2068 7265 663d      </a><a href=
+00000320: 2268 7474 7073 3a2f 2f72 6573 756c 7473  "https://results
+00000330: 2e70 7265 2d63 6f6d 6d69 742e 6369 2f6c  .pre-commit.ci/l
+00000340: 6174 6573 742f 6769 7468 7562 2f62 656e  atest/github/ben
+00000350: 746f 6d6c 2f4f 7065 6e4c 4c4d 2f6d 6169  toml/OpenLLM/mai
+00000360: 6e22 3e0a 2020 2020 2020 2020 3c69 6d67  n">.        <img
+00000370: 2073 7263 3d22 6874 7470 733a 2f2f 7265   src="https://re
+00000380: 7375 6c74 732e 7072 652d 636f 6d6d 6974  sults.pre-commit
+00000390: 2e63 692f 6261 6467 652f 6769 7468 7562  .ci/badge/github
+000003a0: 2f62 656e 746f 6d6c 2f4f 7065 6e4c 4c4d  /bentoml/OpenLLM
+000003b0: 2f6d 6169 6e2e 7376 6722 2061 6c74 3d22  /main.svg" alt="
+000003c0: 7072 652d 636f 6d6d 6974 2e63 6920 7374  pre-commit.ci st
+000003d0: 6174 7573 2220 2f3e 0a20 2020 203c 2f61  atus" />.    </a
+000003e0: 3e3c 6272 3e3c 6120 6872 6566 3d22 6874  ><br><a href="ht
+000003f0: 7470 733a 2f2f 7477 6974 7465 722e 636f  tps://twitter.co
+00000400: 6d2f 6265 6e74 6f6d 6c61 6922 3e0a 2020  m/bentomlai">.  
+00000410: 2020 2020 2020 3c69 6d67 2073 7263 3d22        <img src="
+00000420: 6874 7470 733a 2f2f 6261 6467 656e 2e6e  https://badgen.n
+00000430: 6574 2f62 6164 6765 2f69 636f 6e2f 4062  et/badge/icon/@b
+00000440: 656e 746f 6d6c 6169 2f31 4441 3146 323f  entomlai/1DA1F2?
+00000450: 6963 6f6e 3d74 7769 7474 6572 266c 6162  icon=twitter&lab
+00000460: 656c 3d46 6f6c 6c6f 7725 3230 5573 2220  el=Follow%20Us" 
+00000470: 616c 743d 2254 7769 7474 6572 2220 2f3e  alt="Twitter" />
+00000480: 0a20 2020 203c 2f61 3e3c 6120 6872 6566  .    </a><a href
+00000490: 3d22 6874 7470 733a 2f2f 6c2e 6265 6e74  ="https://l.bent
+000004a0: 6f6d 6c2e 636f 6d2f 6a6f 696e 2d6f 7065  oml.com/join-ope
+000004b0: 6e6c 6c6d 2d64 6973 636f 7264 223e 0a20  nllm-discord">. 
+000004c0: 2020 2020 2020 203c 696d 6720 7372 633d         <img src=
+000004d0: 2268 7474 7073 3a2f 2f62 6164 6765 6e2e  "https://badgen.
+000004e0: 6e65 742f 6261 6467 652f 6963 6f6e 2f4f  net/badge/icon/O
+000004f0: 7065 6e4c 4c4d 2f37 3238 3964 613f 6963  penLLM/7289da?ic
+00000500: 6f6e 3d64 6973 636f 7264 266c 6162 656c  on=discord&label
+00000510: 3d4a 6f69 6e25 3230 5573 2220 616c 743d  =Join%20Us" alt=
+00000520: 2244 6973 636f 7264 2220 2f3e 0a20 2020  "Discord" />.   
+00000530: 203c 2f61 3e0a 3c2f 6469 763e 0a0a 2323   </a>.</div>..##
+00000540: 20f0 9f93 9620 496e 7472 6f64 7563 7469   .... Introducti
+00000550: 6f6e 0a0a 4f70 656e 4c4c 4d20 6865 6c70  on..OpenLLM help
+00000560: 7320 6465 7665 6c6f 7065 7273 202a 2a72  s developers **r
+00000570: 756e 2061 6e79 206f 7065 6e2d 736f 7572  un any open-sour
+00000580: 6365 204c 4c4d 732a 2a2c 2073 7563 6820  ce LLMs**, such 
+00000590: 6173 204c 6c61 6d61 2032 2061 6e64 204d  as Llama 2 and M
+000005a0: 6973 7472 616c 2c20 6173 202a 2a4f 7065  istral, as **Ope
+000005b0: 6e41 492d 636f 6d70 6174 6962 6c65 2041  nAI-compatible A
+000005c0: 5049 2065 6e64 706f 696e 7473 2a2a 2c20  PI endpoints**, 
+000005d0: 6c6f 6361 6c6c 7920 616e 6420 696e 2074  locally and in t
+000005e0: 6865 2063 6c6f 7564 2c20 6f70 7469 6d69  he cloud, optimi
+000005f0: 7a65 6420 666f 7220 7365 7276 696e 6720  zed for serving 
+00000600: 7468 726f 7567 6870 7574 2061 6e64 2070  throughput and p
+00000610: 726f 6475 6374 696f 6e20 6465 706c 6f79  roduction deploy
+00000620: 6d65 6e74 2e0a 0a0a 2d20 f09f 9a82 2053  ment....- .... S
+00000630: 7570 706f 7274 2061 2077 6964 6520 7261  upport a wide ra
+00000640: 6e67 6520 6f66 206f 7065 6e2d 736f 7572  nge of open-sour
+00000650: 6365 204c 4c4d 7320 696e 636c 7564 696e  ce LLMs includin
+00000660: 6720 4c4c 4d73 2066 696e 652d 7475 6e65  g LLMs fine-tune
+00000670: 6420 7769 7468 2079 6f75 7220 6f77 6e20  d with your own 
+00000680: 6461 7461 0a2d 20e2 9b93 efb8 8f20 4f70  data.- ...... Op
+00000690: 656e 4149 2063 6f6d 7061 7469 626c 6520  enAI compatible 
+000006a0: 4150 4920 656e 6470 6f69 6e74 7320 666f  API endpoints fo
+000006b0: 7220 7365 616d 6c65 7373 2074 7261 6e73  r seamless trans
+000006c0: 6974 696f 6e20 6672 6f6d 2079 6f75 7220  ition from your 
+000006d0: 4c4c 4d20 6170 7020 746f 206f 7065 6e2d  LLM app to open-
+000006e0: 736f 7572 6365 204c 4c4d 730a 2d20 f09f  source LLMs.- ..
+000006f0: 94a5 2053 7461 7465 2d6f 662d 7468 652d  .. State-of-the-
+00000700: 6172 7420 7365 7276 696e 6720 616e 6420  art serving and 
+00000710: 696e 6665 7265 6e63 6520 7065 7266 6f72  inference perfor
+00000720: 6d61 6e63 650a 2d20 f09f 8eaf 2053 696d  mance.- .... Sim
+00000730: 706c 6966 6965 6420 636c 6f75 6420 6465  plified cloud de
+00000740: 706c 6f79 6d65 6e74 2076 6961 205b 4265  ployment via [Be
+00000750: 6e74 6f4d 4c5d 2877 7777 2e62 656e 746f  ntoML](www.bento
+00000760: 6d6c 2e63 6f6d 290a 0a0a 3c21 2d2d 2068  ml.com)...<!-- h
+00000770: 6174 6368 2d66 616e 6379 2d70 7970 692d  atch-fancy-pypi-
+00000780: 7265 6164 6d65 2069 6e74 726f 2073 746f  readme intro sto
+00000790: 7020 2d2d 3e0a 0a21 5b47 6966 2073 686f  p -->..![Gif sho
+000007a0: 7769 6e67 204f 7065 6e4c 4c4d 2049 6e74  wing OpenLLM Int
+000007b0: 726f 5d28 2f2e 6769 7468 7562 2f61 7373  ro](/.github/ass
+000007c0: 6574 732f 6f75 7470 7574 2e67 6966 290a  ets/output.gif).
+000007d0: 0a3c 6272 2f3e 0a0a 3c21 2d2d 2068 6174  .<br/>..<!-- hat
+000007e0: 6368 2d66 616e 6379 2d70 7970 692d 7265  ch-fancy-pypi-re
+000007f0: 6164 6d65 2069 6e74 6572 696d 2073 7461  adme interim sta
+00000800: 7274 202d 2d3e 0a0a 2323 20f0 9f92 be20  rt -->..## .... 
+00000810: 544c 2f44 520a 0a46 6f72 2073 7461 7274  TL/DR..For start
+00000820: 6572 2c20 7765 2070 726f 7669 6465 2074  er, we provide t
+00000830: 776f 2077 6179 7320 746f 2071 7569 636b  wo ways to quick
+00000840: 6c79 2074 7279 206f 7574 204f 7065 6e4c  ly try out OpenL
+00000850: 4c4d 3a0a 0a23 2323 204a 7570 7974 6572  LM:..### Jupyter
+00000860: 204e 6f74 6562 6f6f 6b73 0a0a 5472 7920   Notebooks..Try 
+00000870: 7468 6973 205b 4f70 656e 4c4c 4d20 7475  this [OpenLLM tu
+00000880: 746f 7269 616c 2069 6e20 476f 6f67 6c65  torial in Google
+00000890: 2043 6f6c 6162 3a20 5365 7276 696e 6720   Colab: Serving 
+000008a0: 4c6c 616d 6120 3220 7769 7468 204f 7065  Llama 2 with Ope
+000008b0: 6e4c 4c4d 5d28 6874 7470 733a 2f2f 636f  nLLM](https://co
+000008c0: 6c61 622e 7265 7365 6172 6368 2e67 6f6f  lab.research.goo
+000008d0: 676c 652e 636f 6d2f 6769 7468 7562 2f62  gle.com/github/b
+000008e0: 656e 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62  entoml/OpenLLM/b
+000008f0: 6c6f 622f 6d61 696e 2f65 7861 6d70 6c65  lob/main/example
+00000900: 732f 6c6c 616d 6132 2e69 7079 6e62 292e  s/llama2.ipynb).
+00000910: 0a0a 2323 2320 446f 636b 6572 0a0a 5765  ..### Docker..We
+00000920: 2070 726f 7669 6465 2061 2064 6f63 6b65   provide a docke
+00000930: 7220 636f 6e74 6169 6e65 7220 7468 6174  r container that
+00000940: 2068 656c 7073 2079 6f75 2073 7461 7274   helps you start
+00000950: 2072 756e 6e69 6e67 204f 7065 6e4c 4c4d   running OpenLLM
+00000960: 3a0a 0a60 6060 6261 7368 0a64 6f63 6b65  :..```bash.docke
+00000970: 7220 7275 6e20 2d2d 726d 202d 6974 202d  r run --rm -it -
+00000980: 7020 3330 3030 3a33 3030 3020 6768 6372  p 3000:3000 ghcr
+00000990: 2e69 6f2f 6265 6e74 6f6d 6c2f 6f70 656e  .io/bentoml/open
+000009a0: 6c6c 6d20 7374 6172 7420 6661 6365 626f  llm start facebo
+000009b0: 6f6b 2f6f 7074 2d31 2e33 6220 2d2d 6261  ok/opt-1.3b --ba
+000009c0: 636b 656e 6420 7074 0a60 6060 0a0a 3e20  ckend pt.```..> 
+000009d0: 5b21 4e4f 5445 5d0a 3e20 4769 7665 6e20  [!NOTE].> Given 
+000009e0: 796f 7520 6861 7665 2061 6363 6573 7320  you have access 
+000009f0: 746f 2047 5055 7320 616e 6420 6861 7665  to GPUs and have
+00000a00: 2073 6574 7570 205b 6e76 6964 6961 2d64   setup [nvidia-d
+00000a10: 6f63 6b65 725d 2868 7474 7073 3a2f 2f67  ocker](https://g
+00000a20: 6974 6875 622e 636f 6d2f 4e56 4944 4941  ithub.com/NVIDIA
+00000a30: 2f6e 7669 6469 612d 636f 6e74 6169 6e65  /nvidia-containe
+00000a40: 722d 746f 6f6c 6b69 7429 2c20 2079 6f75  r-toolkit),  you
+00000a50: 2063 616e 2061 6464 6974 696f 6e61 6c6c   can additionall
+00000a60: 7920 7061 7373 2069 6e20 602d 2d67 7075  y pass in `--gpu
+00000a70: 7360 0a3e 2074 6f20 7573 6520 4750 5520  s`.> to use GPU 
+00000a80: 666f 7220 6661 7374 6572 2069 6e66 6572  for faster infer
+00000a90: 656e 6365 2061 6e64 206f 7074 696d 697a  ence and optimiz
+00000aa0: 6174 696f 6e0a 3e60 6060 6261 7368 0a3e  ation.>```bash.>
+00000ab0: 2064 6f63 6b65 7220 7275 6e20 2d2d 726d   docker run --rm
+00000ac0: 202d 2d67 7075 7320 616c 6c20 2d70 2033   --gpus all -p 3
+00000ad0: 3030 303a 3330 3030 202d 6974 2067 6863  000:3000 -it ghc
+00000ae0: 722e 696f 2f62 656e 746f 6d6c 2f6f 7065  r.io/bentoml/ope
+00000af0: 6e6c 6c6d 2073 7461 7274 2048 7567 6769  nllm start Huggi
+00000b00: 6e67 4661 6365 4834 2f7a 6570 6879 722d  ngFaceH4/zephyr-
+00000b10: 3762 2d62 6574 6120 2d2d 6261 636b 656e  7b-beta --backen
+00000b20: 6420 766c 6c6d 0a3e 2060 6060 0a0a 0a23  d vllm.> ```...#
+00000b30: 2320 f09f 8f83 2047 6574 2073 7461 7274  # .... Get start
+00000b40: 6564 0a0a 5468 6520 666f 6c6c 6f77 696e  ed..The followin
+00000b50: 6720 7072 6f76 6964 6573 2069 6e73 7472  g provides instr
+00000b60: 7563 7469 6f6e 7320 666f 7220 686f 7720  uctions for how 
+00000b70: 746f 2067 6574 2073 7461 7274 6564 2077  to get started w
+00000b80: 6974 6820 4f70 656e 4c4c 4d20 6c6f 6361  ith OpenLLM loca
+00000b90: 6c6c 792e 0a0a 2323 2320 5072 6572 6571  lly...### Prereq
+00000ba0: 7569 7369 7465 730a 0a59 6f75 2068 6176  uisites..You hav
+00000bb0: 6520 696e 7374 616c 6c65 6420 5079 7468  e installed Pyth
+00000bc0: 6f6e 2033 2e38 2028 6f72 206c 6174 6572  on 3.8 (or later
+00000bd0: 2920 616e 64c2 a060 7069 7060 2e20 5765  ) and..`pip`. We
+00000be0: 2068 6967 686c 7920 7265 636f 6d6d 656e   highly recommen
+00000bf0: 6420 7573 696e 6720 6120 5b56 6972 7475  d using a [Virtu
+00000c00: 616c 2045 6e76 6972 6f6e 6d65 6e74 5d28  al Environment](
+00000c10: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
+00000c20: 686f 6e2e 6f72 672f 332f 6c69 6272 6172  hon.org/3/librar
+00000c30: 792f 7665 6e76 2e68 746d 6c29 2074 6f20  y/venv.html) to 
+00000c40: 7072 6576 656e 7420 7061 636b 6167 6520  prevent package 
+00000c50: 636f 6e66 6c69 6374 732e 0a0a 2323 2320  conflicts...### 
+00000c60: 496e 7374 616c 6c20 4f70 656e 4c4c 4d0a  Install OpenLLM.
+00000c70: 0a49 6e73 7461 6c6c 204f 7065 6e4c 4c4d  .Install OpenLLM
+00000c80: 2062 7920 7573 696e 6720 6070 6970 6020   by using `pip` 
+00000c90: 6173 2066 6f6c 6c6f 7773 3a0a 0a60 6060  as follows:..```
+00000ca0: 6261 7368 0a70 6970 2069 6e73 7461 6c6c  bash.pip install
+00000cb0: 206f 7065 6e6c 6c6d 0a60 6060 0a0a 546f   openllm.```..To
+00000cc0: 2076 6572 6966 7920 7468 6520 696e 7374   verify the inst
+00000cd0: 616c 6c61 7469 6f6e 2c20 7275 6e3a 0a0a  allation, run:..
+00000ce0: 6060 6062 6173 680a 2420 6f70 656e 6c6c  ```bash.$ openll
+00000cf0: 6d20 2d68 0a0a 5573 6167 653a 206f 7065  m -h..Usage: ope
+00000d00: 6e6c 6c6d 205b 4f50 5449 4f4e 535d 2043  nllm [OPTIONS] C
+00000d10: 4f4d 4d41 4e44 205b 4152 4753 5d2e 2e2e  OMMAND [ARGS]...
+00000d20: 0a0a 2020 20e2 9688 e296 88e2 9688 e296  ..   ...........
+00000d30: 88e2 9688 e296 88e2 9597 20e2 9688 e296  .......... .....
+00000d40: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
+00000d50: 20e2 9688 e296 88e2 9688 e296 88e2 9688   ...............
+00000d60: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000d70: 9688 e295 9720 2020 e296 88e2 9688 e295  .....   ........
+00000d80: 97e2 9688 e296 88e2 9597 2020 2020 20e2  ..........     .
+00000d90: 9688 e296 88e2 9597 2020 2020 20e2 9688  ........     ...
+00000da0: e296 88e2 9688 e295 9720 2020 e296 88e2  .........   ....
+00000db0: 9688 e296 88e2 9597 0a20 20e2 9688 e296  .........  .....
+00000dc0: 88e2 9594 e295 90e2 9590 e295 90e2 9688  ................
+00000dd0: e296 88e2 9597 e296 88e2 9688 e295 94e2  ................
+00000de0: 9590 e295 90e2 9688 e296 88e2 9597 e296  ................
+00000df0: 88e2 9688 e295 94e2 9590 e295 90e2 9590  ................
+00000e00: e295 90e2 959d e296 88e2 9688 e296 88e2  ................
+00000e10: 9688 e295 9720 20e2 9688 e296 88e2 9591  .....  .........
+00000e20: e296 88e2 9688 e295 9120 2020 2020 e296  .........     ..
+00000e30: 88e2 9688 e295 9120 2020 2020 e296 88e2  .......     ....
+00000e40: 9688 e296 88e2 9688 e295 9720 e296 88e2  ........... ....
+00000e50: 9688 e296 88e2 9688 e295 910a 2020 e296  ............  ..
+00000e60: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
+00000e70: e295 91e2 9688 e296 88e2 9688 e296 88e2  ................
+00000e80: 9688 e296 88e2 9594 e295 9de2 9688 e296  ................
+00000e90: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
+00000ea0: 9688 e296 88e2 9594 e296 88e2 9688 e295  ................
+00000eb0: 9720 e296 88e2 9688 e295 91e2 9688 e296  . ..............
+00000ec0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
+00000ed0: 9591 2020 2020 20e2 9688 e296 88e2 9594  ..     .........
+00000ee0: e296 88e2 9688 e296 88e2 9688 e295 94e2  ................
+00000ef0: 9688 e296 88e2 9591 0a20 20e2 9688 e296  .........  .....
+00000f00: 88e2 9591 2020 20e2 9688 e296 88e2 9591  ....   .........
+00000f10: e296 88e2 9688 e295 94e2 9590 e295 90e2  ................
+00000f20: 9590 e295 9d20 e296 88e2 9688 e295 94e2  ..... ..........
+00000f30: 9590 e295 90e2 959d 2020 e296 88e2 9688  ........  ......
+00000f40: e295 91e2 959a e296 88e2 9688 e295 97e2  ................
+00000f50: 9688 e296 88e2 9591 e296 88e2 9688 e295  ................
+00000f60: 9120 2020 2020 e296 88e2 9688 e295 9120  .     ......... 
+00000f70: 2020 2020 e296 88e2 9688 e295 91e2 959a      ............
+00000f80: e296 88e2 9688 e295 94e2 959d e296 88e2  ................
+00000f90: 9688 e295 910a 2020 e295 9ae2 9688 e296  ......  ........
+00000fa0: 88e2 9688 e296 88e2 9688 e296 88e2 9594  ................
+00000fb0: e295 9de2 9688 e296 88e2 9591 2020 2020  ............    
+00000fc0: 20e2 9688 e296 88e2 9688 e296 88e2 9688   ...............
+00000fd0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000fe0: 9591 20e2 959a e296 88e2 9688 e296 88e2  .. .............
+00000ff0: 9688 e295 91e2 9688 e296 88e2 9688 e296  ................
+00001000: 88e2 9688 e296 88e2 9688 e295 97e2 9688  ................
+00001010: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00001020: 9688 e295 97e2 9688 e296 88e2 9591 20e2  .............. .
+00001030: 959a e295 90e2 959d 20e2 9688 e296 88e2  ........ .......
+00001040: 9591 0a20 2020 e295 9ae2 9590 e295 90e2  ...   ..........
+00001050: 9590 e295 90e2 9590 e295 9d20 e295 9ae2  ........... ....
+00001060: 9590 e295 9d20 2020 2020 e295 9ae2 9590  .....     ......
+00001070: e295 90e2 9590 e295 90e2 9590 e295 90e2  ................
+00001080: 959d e295 9ae2 9590 e295 9d20 20e2 959a  ...........  ...
+00001090: e295 90e2 9590 e295 90e2 959d e295 9ae2  ................
+000010a0: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+000010b0: 90e2 959d e295 9ae2 9590 e295 90e2 9590  ................
+000010c0: e295 90e2 9590 e295 90e2 959d e295 9ae2  ................
+000010d0: 9590 e295 9d20 2020 2020 e295 9ae2 9590  .....     ......
+000010e0: e295 9d2e 0a0a 2020 416e 206f 7065 6e20  ......  An open 
+000010f0: 706c 6174 666f 726d 2066 6f72 206f 7065  platform for ope
+00001100: 7261 7469 6e67 206c 6172 6765 206c 616e  rating large lan
+00001110: 6775 6167 6520 6d6f 6465 6c73 2069 6e20  guage models in 
+00001120: 7072 6f64 7563 7469 6f6e 2e0a 2020 4669  production..  Fi
+00001130: 6e65 2d74 756e 652c 2073 6572 7665 2c20  ne-tune, serve, 
+00001140: 6465 706c 6f79 2c20 616e 6420 6d6f 6e69  deploy, and moni
+00001150: 746f 7220 616e 7920 4c4c 4d73 2077 6974  tor any LLMs wit
+00001160: 6820 6561 7365 2e0a 0a4f 7074 696f 6e73  h ease...Options
+00001170: 3a0a 2020 2d76 2c20 2d2d 7665 7273 696f  :.  -v, --versio
+00001180: 6e20 2053 686f 7720 7468 6520 7665 7273  n  Show the vers
+00001190: 696f 6e20 616e 6420 6578 6974 2e0a 2020  ion and exit..  
+000011a0: 2d68 2c20 2d2d 6865 6c70 2020 2020 2053  -h, --help     S
+000011b0: 686f 7720 7468 6973 206d 6573 7361 6765  how this message
+000011c0: 2061 6e64 2065 7869 742e 0a0a 436f 6d6d   and exit...Comm
+000011d0: 616e 6473 3a0a 2020 6275 696c 6420 2020  ands:.  build   
+000011e0: 2020 2020 5061 636b 6167 6520 6120 6769      Package a gi
+000011f0: 7665 6e20 6d6f 6465 6c73 2069 6e74 6f20  ven models into 
+00001200: 6120 4265 6e74 6f4c 4c4d 2e0a 2020 696d  a BentoLLM..  im
+00001210: 706f 7274 2020 2020 2020 5365 7475 7020  port      Setup 
+00001220: 4c4c 4d20 696e 7465 7261 6374 6976 656c  LLM interactivel
+00001230: 792e 0a20 206d 6f64 656c 7320 2020 2020  y..  models     
+00001240: 204c 6973 7420 616c 6c20 7375 7070 6f72   List all suppor
+00001250: 7465 6420 6d6f 6465 6c73 2e0a 2020 7072  ted models..  pr
+00001260: 756e 6520 2020 2020 2020 5265 6d6f 7665  une       Remove
+00001270: 2061 6c6c 2073 6176 6564 206d 6f64 656c   all saved model
+00001280: 732c 2028 616e 6420 6f70 7469 6f6e 616c  s, (and optional
+00001290: 6c79 2062 656e 746f 7329 2062 7569 6c74  ly bentos) built
+000012a0: 2077 6974 6820 4f70 656e 4c4c 4d20 6c6f   with OpenLLM lo
+000012b0: 6361 6c6c 792e 0a20 2071 7565 7279 2020  cally..  query  
+000012c0: 2020 2020 2051 7565 7279 2061 204c 4c4d       Query a LLM
+000012d0: 2069 6e74 6572 6163 7469 7665 6c79 2c20   interactively, 
+000012e0: 6672 6f6d 2061 2074 6572 6d69 6e61 6c2e  from a terminal.
+000012f0: 0a20 2073 7461 7274 2020 2020 2020 2053  .  start       S
+00001300: 7461 7274 2061 204c 4c4d 5365 7276 6572  tart a LLMServer
+00001310: 2066 6f72 2061 6e79 2073 7570 706f 7274   for any support
+00001320: 6564 204c 4c4d 2e0a 0a45 7874 656e 7369  ed LLM...Extensi
+00001330: 6f6e 733a 0a20 2062 7569 6c64 2d62 6173  ons:.  build-bas
+00001340: 652d 636f 6e74 6169 6e65 7220 2042 6173  e-container  Bas
+00001350: 6520 696d 6167 6520 6275 696c 6465 7220  e image builder 
+00001360: 666f 7220 4265 6e74 6f4c 4c4d 2e0a 2020  for BentoLLM..  
+00001370: 6469 7665 2d62 656e 746f 7320 2020 2020  dive-bentos     
+00001380: 2020 2020 2020 4469 7665 2069 6e74 6f20        Dive into 
+00001390: 6120 4265 6e74 6f4c 4c4d 2e0a 2020 6765  a BentoLLM..  ge
+000013a0: 742d 636f 6e74 6169 6e65 7266 696c 6520  t-containerfile 
+000013b0: 2020 2020 5265 7475 726e 2043 6f6e 7461      Return Conta
+000013c0: 696e 6572 6669 6c65 206f 6620 616e 7920  inerfile of any 
+000013d0: 6769 7665 6e20 4265 6e74 6f2e 0a20 2067  given Bento..  g
+000013e0: 6574 2d70 726f 6d70 7420 2020 2020 2020  et-prompt       
+000013f0: 2020 2020 2047 6574 2074 6865 2064 6566       Get the def
+00001400: 6175 6c74 2070 726f 6d70 7420 7573 6564  ault prompt used
+00001410: 2062 7920 4f70 656e 4c4c 4d2e 0a20 206c   by OpenLLM..  l
+00001420: 6973 742d 6265 6e74 6f73 2020 2020 2020  ist-bentos      
+00001430: 2020 2020 204c 6973 7420 6176 6169 6c61       List availa
+00001440: 626c 6520 6265 6e74 6f73 2062 7569 6c74  ble bentos built
+00001450: 2062 7920 4f70 656e 4c4c 4d2e 0a20 206c   by OpenLLM..  l
+00001460: 6973 742d 6d6f 6465 6c73 2020 2020 2020  ist-models      
+00001470: 2020 2020 2054 6869 7320 6973 2065 7175       This is equ
+00001480: 6976 616c 656e 7420 746f 206f 7065 6e6c  ivalent to openl
+00001490: 6c6d 206d 6f64 656c 732e 2e2e 0a20 2070  lm models....  p
+000014a0: 6c61 7967 726f 756e 6420 2020 2020 2020  layground       
+000014b0: 2020 2020 204f 7065 6e4c 4c4d 2050 6c61       OpenLLM Pla
+000014c0: 7967 726f 756e 642e 0a60 6060 0a0a 2323  yground..```..##
+000014d0: 2320 5374 6172 7420 6120 4c4c 4d20 7365  # Start a LLM se
+000014e0: 7276 6572 0a0a 4f70 656e 4c4c 4d20 616c  rver..OpenLLM al
+000014f0: 6c6f 7773 2079 6f75 2074 6f20 7175 6963  lows you to quic
+00001500: 6b6c 7920 7370 696e 2075 7020 616e 204c  kly spin up an L
+00001510: 4c4d 2073 6572 7665 7220 7573 696e 6720  LM server using 
+00001520: 606f 7065 6e6c 6c6d 2073 7461 7274 602e  `openllm start`.
+00001530: 2046 6f72 2065 7861 6d70 6c65 2c20 746f   For example, to
+00001540: 2073 7461 7274 2061 c2a0 5b70 6869 2d32   start a..[phi-2
+00001550: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00001560: 6766 6163 652e 636f 2f6d 6963 726f 736f  gface.co/microso
+00001570: 6674 2f70 6869 2d32 29c2 a073 6572 7665  ft/phi-2)..serve
+00001580: 722c 2072 756e 2074 6865 2066 6f6c 6c6f  r, run the follo
+00001590: 7769 6e67 3a0a 0a60 6060 6261 7368 0a54  wing:..```bash.T
+000015a0: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
+000015b0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
+000015c0: 6172 7420 6d69 6372 6f73 6f66 742f 7068  art microsoft/ph
+000015d0: 692d 320a 6060 600a 0a54 6869 7320 7374  i-2.```..This st
+000015e0: 6172 7473 2074 6865 2073 6572 7665 7220  arts the server 
+000015f0: 6174 c2a0 5b68 7474 703a 2f2f 302e 302e  at..[http://0.0.
+00001600: 302e 303a 3330 3030 2f5d 2868 7474 703a  0.0:3000/](http:
+00001610: 2f2f 302e 302e 302e 303a 3330 3030 2f29  //0.0.0.0:3000/)
+00001620: 2e20 4f70 656e 4c4c 4d20 646f 776e 6c6f  . OpenLLM downlo
+00001630: 6164 7320 7468 6520 6d6f 6465 6c20 746f  ads the model to
+00001640: 2074 6865 2042 656e 746f 4d4c 206c 6f63   the BentoML loc
+00001650: 616c 204d 6f64 656c 2053 746f 7265 2069  al Model Store i
+00001660: 6620 6974 2068 6173 206e 6f74 2062 6565  f it has not bee
+00001670: 6e20 7265 6769 7374 6572 6564 2062 6566  n registered bef
+00001680: 6f72 652e 2054 6f20 7669 6577 2079 6f75  ore. To view you
+00001690: 7220 6c6f 6361 6c20 6d6f 6465 6c73 2c20  r local models, 
+000016a0: 7275 6e20 6062 656e 746f 6d6c 206d 6f64  run `bentoml mod
+000016b0: 656c 7320 6c69 7374 602e 0a0a 546f 2069  els list`...To i
+000016c0: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+000016d0: 2073 6572 7665 722c 2079 6f75 2063 616e   server, you can
+000016e0: 2076 6973 6974 2074 6865 2077 6562 2055   visit the web U
+000016f0: 4920 6174 c2a0 5b68 7474 703a 2f2f 302e  I at..[http://0.
+00001700: 302e 302e 303a 3330 3030 2f5d 2868 7474  0.0.0:3000/](htt
+00001710: 703a 2f2f 302e 302e 302e 303a 3330 3030  p://0.0.0.0:3000
+00001720: 2f29 206f 7220 7365 6e64 2061 2072 6571  /) or send a req
+00001730: 7565 7374 2075 7369 6e67 c2a0 6063 7572  uest using..`cur
+00001740: 6c60 2e20 596f 7520 6361 6e20 616c 736f  l`. You can also
+00001750: 2075 7365 204f 7065 6e4c 4c4d e280 9973   use OpenLLM...s
+00001760: 2062 7569 6c74 2d69 6e20 5079 7468 6f6e   built-in Python
+00001770: 2063 6c69 656e 7420 746f 2069 6e74 6572   client to inter
+00001780: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
+00001790: 7665 723a 0a0a 6060 6070 7974 686f 6e0a  ver:..```python.
+000017a0: 696d 706f 7274 206f 7065 6e6c 6c6d 0a0a  import openllm..
+000017b0: 636c 6965 6e74 203d 206f 7065 6e6c 6c6d  client = openllm
+000017c0: 2e63 6c69 656e 742e 4854 5450 436c 6965  .client.HTTPClie
+000017d0: 6e74 2827 6874 7470 3a2f 2f6c 6f63 616c  nt('http://local
+000017e0: 686f 7374 3a33 3030 3027 290a 636c 6965  host:3000').clie
+000017f0: 6e74 2e71 7565 7279 2827 4578 706c 6169  nt.query('Explai
+00001800: 6e20 746f 206d 6520 7468 6520 6469 6666  n to me the diff
+00001810: 6572 656e 6365 2062 6574 7765 656e 2022  erence between "
+00001820: 6675 7274 6865 7222 2061 6e64 2022 6661  further" and "fa
+00001830: 7274 6865 7222 2729 0a60 6060 0a0a 416c  rther"').```..Al
+00001840: 7465 726e 6174 6976 656c 792c 2075 7365  ternatively, use
+00001850: 2074 6865 c2a0 606f 7065 6e6c 6c6d 2071   the..`openllm q
+00001860: 7565 7279 60c2 a063 6f6d 6d61 6e64 2074  uery`..command t
+00001870: 6f20 7175 6572 7920 7468 6520 6d6f 6465  o query the mode
+00001880: 6c3a 0a0a 6060 6062 6173 680a 6578 706f  l:..```bash.expo
+00001890: 7274 204f 5045 4e4c 4c4d 5f45 4e44 504f  rt OPENLLM_ENDPO
+000018a0: 494e 543d 6874 7470 3a2f 2f6c 6f63 616c  INT=http://local
+000018b0: 686f 7374 3a33 3030 300a 6f70 656e 6c6c  host:3000.openll
+000018c0: 6d20 7175 6572 7920 2745 7870 6c61 696e  m query 'Explain
+000018d0: 2074 6f20 6d65 2074 6865 2064 6966 6665   to me the diffe
+000018e0: 7265 6e63 6520 6265 7477 6565 6e20 2266  rence between "f
+000018f0: 7572 7468 6572 2220 616e 6420 2266 6172  urther" and "far
+00001900: 7468 6572 2227 0a60 6060 0a0a 4f70 656e  ther"'.```..Open
+00001910: 4c4c 4d20 7365 616d 6c65 7373 6c79 2073  LLM seamlessly s
+00001920: 7570 706f 7274 7320 6d61 6e79 206d 6f64  upports many mod
+00001930: 656c 7320 616e 6420 7468 6569 7220 7661  els and their va
+00001940: 7269 616e 7473 2e20 596f 7520 6361 6e20  riants. You can 
+00001950: 7370 6563 6966 7920 6469 6666 6572 656e  specify differen
+00001960: 7420 7661 7269 616e 7473 206f 6620 7468  t variants of th
+00001970: 6520 6d6f 6465 6c20 746f 2062 6520 7365  e model to be se
+00001980: 7276 6564 2e20 466f 7220 6578 616d 706c  rved. For exampl
+00001990: 653a 0a0a 6060 6062 6173 680a 6f70 656e  e:..```bash.open
+000019a0: 6c6c 6d20 7374 6172 7420 3c6d 6f64 656c  llm start <model
+000019b0: 5f69 643e 202d 2d3c 6f70 7469 6f6e 733e  _id> --<options>
+000019c0: 0a60 6060 0a0a 3e20 5b21 4e4f 5445 5d0a  .```..> [!NOTE].
+000019d0: 3e20 4f70 656e 4c4c 4d20 7375 7070 6f72  > OpenLLM suppor
+000019e0: 7473 2073 7065 6369 6679 696e 6720 6669  ts specifying fi
+000019f0: 6e65 2d74 756e 696e 6720 7765 6967 6874  ne-tuning weight
+00001a00: 7320 616e 6420 7175 616e 7469 7a65 6420  s and quantized 
+00001a10: 7765 6967 6874 730a 3e20 666f 7220 616e  weights.> for an
+00001a20: 7920 6f66 2074 6865 2073 7570 706f 7274  y of the support
+00001a30: 6564 206d 6f64 656c 7320 6173 206c 6f6e  ed models as lon
+00001a40: 6720 6173 2074 6865 7920 6361 6e20 6265  g as they can be
+00001a50: 206c 6f61 6465 6420 7769 7468 2074 6865   loaded with the
+00001a60: 206d 6f64 656c 0a3e 2061 7263 6869 7465   model.> archite
+00001a70: 6374 7572 652e 2055 7365 2074 6865 c2a0  cture. Use the..
+00001a80: 606f 7065 6e6c 6c6d 206d 6f64 656c 7360  `openllm models`
+00001a90: c2a0 636f 6d6d 616e 6420 746f 2073 6565  ..command to see
+00001aa0: 2074 6865 2063 6f6d 706c 6574 6520 6c69   the complete li
+00001ab0: 7374 206f 6620 7375 7070 6f72 7465 640a  st of supported.
+00001ac0: 3e20 6d6f 6465 6c73 2c20 7468 6569 7220  > models, their 
+00001ad0: 6172 6368 6974 6563 7475 7265 732c 2061  architectures, a
+00001ae0: 6e64 2074 6865 6972 2076 6172 6961 6e74  nd their variant
+00001af0: 732e 0a0a 3e20 5b21 494d 504f 5254 414e  s...> [!IMPORTAN
+00001b00: 545d 0a3e 2049 6620 796f 7520 6172 6520  T].> If you are 
+00001b10: 7465 7374 696e 6720 4f70 656e 4c4c 4d20  testing OpenLLM 
+00001b20: 6f6e 2043 5055 2c20 796f 7520 6d69 6768  on CPU, you migh
+00001b30: 7420 7761 6e74 2074 6f20 7061 7373 2069  t want to pass i
+00001b40: 6e20 6044 5459 5045 3d66 6c6f 6174 3332  n `DTYPE=float32
+00001b50: 602e 2042 7920 6465 6661 756c 742c 0a3e  `. By default,.>
+00001b60: 204f 7065 6e4c 4c4d 2077 696c 6c20 7365   OpenLLM will se
+00001b70: 7420 6d6f 6465 6c20 6064 7479 7065 6020  t model `dtype` 
+00001b80: 746f 2060 6266 6c6f 6174 3136 6020 666f  to `bfloat16` fo
+00001b90: 7220 7468 6520 6265 7374 2070 6572 666f  r the best perfo
+00001ba0: 726d 616e 6365 2e0a 3e20 6060 6062 6173  rmance..> ```bas
+00001bb0: 680a 3e20 4454 5950 453d 666c 6f61 7433  h.> DTYPE=float3
+00001bc0: 3220 6f70 656e 6c6c 6d20 7374 6172 7420  2 openllm start 
+00001bd0: 6d69 6372 6f73 6f66 742f 7068 692d 320a  microsoft/phi-2.
+00001be0: 3e20 6060 600a 3e20 5468 6973 2077 696c  > ```.> This wil
+00001bf0: 6c20 616c 736f 2061 7070 6c69 6573 2074  l also applies t
+00001c00: 6f20 6f6c 6465 7220 4750 5573 2e20 4966  o older GPUs. If
+00001c10: 2079 6f75 7220 4750 5573 2064 6f65 736e   your GPUs doesn
+00001c20: 2774 2073 7570 706f 7274 2060 6266 6c6f  't support `bflo
+00001c30: 6174 3136 602c 2074 6865 6e20 796f 7520  at16`, then you 
+00001c40: 616c 736f 0a3e 2077 616e 7420 746f 2073  also.> want to s
+00001c50: 6574 2060 4454 5950 453d 666c 6f61 7431  et `DTYPE=float1
+00001c60: 3660 2e0a 0a23 2320 f09f a7a9 2053 7570  6`...## .... Sup
+00001c70: 706f 7274 6564 206d 6f64 656c 730a 0a4f  ported models..O
+00001c80: 7065 6e4c 4c4d 2063 7572 7265 6e74 6c79  penLLM currently
+00001c90: 2073 7570 706f 7274 7320 7468 6520 666f   supports the fo
+00001ca0: 6c6c 6f77 696e 6720 6d6f 6465 6c73 2e20  llowing models. 
+00001cb0: 4279 2064 6566 6175 6c74 2c20 4f70 656e  By default, Open
+00001cc0: 4c4c 4d20 646f 6573 6e27 7420 696e 636c  LLM doesn't incl
+00001cd0: 7564 6520 6465 7065 6e64 656e 6369 6573  ude dependencies
+00001ce0: 2074 6f20 7275 6e20 616c 6c20 6d6f 6465   to run all mode
+00001cf0: 6c73 2e20 5468 6520 6578 7472 6120 6d6f  ls. The extra mo
+00001d00: 6465 6c2d 7370 6563 6966 6963 2064 6570  del-specific dep
+00001d10: 656e 6465 6e63 6965 7320 6361 6e20 6265  endencies can be
+00001d20: 2069 6e73 7461 6c6c 6564 2077 6974 6820   installed with 
+00001d30: 7468 6520 696e 7374 7275 6374 696f 6e73  the instructions
+00001d40: 2062 656c 6f77 2e0a 0a3c 212d 2d20 7570   below...<!-- up
+00001d50: 6461 7465 2d72 6561 646d 652e 7079 3a20  date-readme.py: 
+00001d60: 7374 6172 7420 2d2d 3e0a 3c64 6574 6169  start -->.<detai
+00001d70: 6c73 3e0a 0a3c 7375 6d6d 6172 793e 4261  ls>..<summary>Ba
+00001d80: 6963 6875 616e 3c2f 7375 6d6d 6172 793e  ichuan</summary>
+00001d90: 0a0a 0a23 2323 2051 7569 636b 7374 6172  ...### Quickstar
+00001da0: 740a 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a  t....> **Note:**
+00001db0: 2042 6169 6368 7561 6e20 7265 7175 6972   Baichuan requir
+00001dc0: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
+00001dd0: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
+00001de0: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
+00001df0: 6e6c 6c6d 5b62 6169 6368 7561 6e5d 220a  nllm[baichuan]".
+00001e00: 3e20 6060 600a 0a0a 5275 6e20 7468 6520  > ```...Run the 
+00001e10: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00001e20: 6420 746f 2071 7569 636b 6c79 2073 7069  d to quickly spi
+00001e30: 6e20 7570 2061 2042 6169 6368 7561 6e20  n up a Baichuan 
+00001e40: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+00001e50: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
+00001e60: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
+00001e70: 7374 6172 7420 6261 6963 6875 616e 2d69  start baichuan-i
+00001e80: 6e63 2f62 6169 6368 7561 6e2d 3762 0a60  nc/baichuan-7b.`
+00001e90: 6060 0a49 6e20 6120 6469 6666 6572 656e  ``.In a differen
+00001ea0: 7420 7465 726d 696e 616c 2c20 7275 6e20  t terminal, run 
+00001eb0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00001ec0: 6d6d 616e 6420 746f 2069 6e74 6572 6163  mmand to interac
+00001ed0: 7420 7769 7468 2074 6865 2073 6572 7665  t with the serve
+00001ee0: 723a 0a0a 6060 6062 6173 680a 6578 706f  r:..```bash.expo
+00001ef0: 7274 204f 5045 4e4c 4c4d 5f45 4e44 504f  rt OPENLLM_ENDPO
+00001f00: 494e 543d 6874 7470 3a2f 2f6c 6f63 616c  INT=http://local
+00001f10: 686f 7374 3a33 3030 300a 6f70 656e 6c6c  host:3000.openll
+00001f20: 6d20 7175 6572 7920 2757 6861 7420 6172  m query 'What ar
+00001f30: 6520 6c61 7267 6520 6c61 6e67 7561 6765  e large language
+00001f40: 206d 6f64 656c 733f 270a 6060 600a 0a0a   models?'.```...
+00001f50: 3e20 2a2a 4e6f 7465 3a2a 2a20 416e 7920  > **Note:** Any 
+00001f60: 4261 6963 6875 616e 2076 6172 6961 6e74  Baichuan variant
+00001f70: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
+00001f80: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
+00001f90: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
+00001fa0: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
+00001fb0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00001fc0: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
+00001fd0: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
+00001fe0: 6172 6368 3d62 6169 6368 7561 6e29 2074  arch=baichuan) t
+00001ff0: 6f20 7365 6520 6d6f 7265 2042 6169 6368  o see more Baich
+00002000: 7561 6e2d 636f 6d70 6174 6962 6c65 206d  uan-compatible m
+00002010: 6f64 656c 732e 0a0a 0a0a 2323 2320 5375  odels.....### Su
+00002020: 7070 6f72 7465 6420 6d6f 6465 6c73 0a0a  pported models..
+00002030: 596f 7520 6361 6e20 7370 6563 6966 7920  You can specify 
+00002040: 616e 7920 6f66 2074 6865 2066 6f6c 6c6f  any of the follo
+00002050: 7769 6e67 2042 6169 6368 7561 6e20 6d6f  wing Baichuan mo
+00002060: 6465 6c73 2076 6961 2060 6f70 656e 6c6c  dels via `openll
+00002070: 6d20 7374 6172 7460 3a0a 0a0a 2d20 5b62  m start`:...- [b
+00002080: 6169 6368 7561 6e2d 696e 632f 6261 6963  aichuan-inc/baic
+00002090: 6875 616e 322d 3762 2d62 6173 655d 2868  huan2-7b-base](h
+000020a0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+000020b0: 6365 2e63 6f2f 6261 6963 6875 616e 2d69  ce.co/baichuan-i
+000020c0: 6e63 2f62 6169 6368 7561 6e32 2d37 622d  nc/baichuan2-7b-
+000020d0: 6261 7365 290a 2d20 5b62 6169 6368 7561  base).- [baichua
+000020e0: 6e2d 696e 632f 6261 6963 6875 616e 322d  n-inc/baichuan2-
+000020f0: 3762 2d63 6861 745d 2868 7474 7073 3a2f  7b-chat](https:/
+00002100: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00002110: 6261 6963 6875 616e 2d69 6e63 2f62 6169  baichuan-inc/bai
+00002120: 6368 7561 6e32 2d37 622d 6368 6174 290a  chuan2-7b-chat).
+00002130: 2d20 5b62 6169 6368 7561 6e2d 696e 632f  - [baichuan-inc/
+00002140: 6261 6963 6875 616e 322d 3133 622d 6261  baichuan2-13b-ba
+00002150: 7365 5d28 6874 7470 733a 2f2f 6875 6767  se](https://hugg
+00002160: 696e 6766 6163 652e 636f 2f62 6169 6368  ingface.co/baich
+00002170: 7561 6e2d 696e 632f 6261 6963 6875 616e  uan-inc/baichuan
+00002180: 322d 3133 622d 6261 7365 290a 2d20 5b62  2-13b-base).- [b
+00002190: 6169 6368 7561 6e2d 696e 632f 6261 6963  aichuan-inc/baic
+000021a0: 6875 616e 322d 3133 622d 6368 6174 5d28  huan2-13b-chat](
+000021b0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+000021c0: 6163 652e 636f 2f62 6169 6368 7561 6e2d  ace.co/baichuan-
+000021d0: 696e 632f 6261 6963 6875 616e 322d 3133  inc/baichuan2-13
+000021e0: 622d 6368 6174 290a 0a3c 2f64 6574 6169  b-chat)..</detai
+000021f0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a0a  ls>..<details>..
+00002200: 3c73 756d 6d61 7279 3e43 6861 7447 4c4d  <summary>ChatGLM
+00002210: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
+00002220: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
+00002230: 202a 2a4e 6f74 653a 2a2a 2043 6861 7447   **Note:** ChatG
+00002240: 4c4d 2072 6571 7569 7265 7320 746f 2069  LM requires to i
+00002250: 6e73 7461 6c6c 2077 6974 683a 0a3e 2060  nstall with:.> `
+00002260: 6060 6261 7368 0a3e 2070 6970 2069 6e73  ``bash.> pip ins
+00002270: 7461 6c6c 2022 6f70 656e 6c6c 6d5b 6368  tall "openllm[ch
+00002280: 6174 676c 6d5d 220a 3e20 6060 600a 0a0a  atglm]".> ```...
+00002290: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
+000022a0: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
+000022b0: 636b 6c79 2073 7069 6e20 7570 2061 2043  ckly spin up a C
+000022c0: 6861 7447 4c4d 2073 6572 7665 723a 0a0a  hatGLM server:..
+000022d0: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
+000022e0: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
+000022f0: 7065 6e6c 6c6d 2073 7461 7274 2074 6875  penllm start thu
+00002300: 646d 2f63 6861 7467 6c6d 2d36 620a 6060  dm/chatglm-6b.``
+00002310: 600a 496e 2061 2064 6966 6665 7265 6e74  `.In a different
+00002320: 2074 6572 6d69 6e61 6c2c 2072 756e 2074   terminal, run t
+00002330: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00002340: 6d61 6e64 2074 6f20 696e 7465 7261 6374  mand to interact
+00002350: 2077 6974 6820 7468 6520 7365 7276 6572   with the server
+00002360: 3a0a 0a60 6060 6261 7368 0a65 7870 6f72  :..```bash.expor
+00002370: 7420 4f50 454e 4c4c 4d5f 454e 4450 4f49  t OPENLLM_ENDPOI
+00002380: 4e54 3d68 7474 703a 2f2f 6c6f 6361 6c68  NT=http://localh
+00002390: 6f73 743a 3330 3030 0a6f 7065 6e6c 6c6d  ost:3000.openllm
+000023a0: 2071 7565 7279 2027 5768 6174 2061 7265   query 'What are
+000023b0: 206c 6172 6765 206c 616e 6775 6167 6520   large language 
+000023c0: 6d6f 6465 6c73 3f27 0a60 6060 0a0a 0a3e  models?'.```...>
+000023d0: 202a 2a4e 6f74 653a 2a2a 2041 6e79 2043   **Note:** Any C
+000023e0: 6861 7447 4c4d 2076 6172 6961 6e74 7320  hatGLM variants 
+000023f0: 6361 6e20 6265 2064 6570 6c6f 7965 6420  can be deployed 
+00002400: 7769 7468 204f 7065 6e4c 4c4d 2e20 5669  with OpenLLM. Vi
+00002410: 7369 7420 7468 6520 5b48 7567 6769 6e67  sit the [Hugging
+00002420: 4661 6365 204d 6f64 656c 2048 7562 5d28  Face Model Hub](
+00002430: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00002440: 6163 652e 636f 2f6d 6f64 656c 733f 736f  ace.co/models?so
+00002450: 7274 3d74 7265 6e64 696e 6726 7365 6172  rt=trending&sear
+00002460: 6368 3d63 6861 7467 6c6d 2920 746f 2073  ch=chatglm) to s
+00002470: 6565 206d 6f72 6520 4368 6174 474c 4d2d  ee more ChatGLM-
+00002480: 636f 6d70 6174 6962 6c65 206d 6f64 656c  compatible model
+00002490: 732e 0a0a 0a0a 2323 2320 5375 7070 6f72  s.....### Suppor
+000024a0: 7465 6420 6d6f 6465 6c73 0a0a 596f 7520  ted models..You 
+000024b0: 6361 6e20 7370 6563 6966 7920 616e 7920  can specify any 
+000024c0: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
+000024d0: 2043 6861 7447 4c4d 206d 6f64 656c 7320   ChatGLM models 
+000024e0: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
+000024f0: 7274 603a 0a0a 0a2d 205b 7468 7564 6d2f  rt`:...- [thudm/
+00002500: 6368 6174 676c 6d2d 3662 5d28 6874 7470  chatglm-6b](http
+00002510: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00002520: 636f 2f74 6875 646d 2f63 6861 7467 6c6d  co/thudm/chatglm
+00002530: 2d36 6229 0a2d 205b 7468 7564 6d2f 6368  -6b).- [thudm/ch
+00002540: 6174 676c 6d2d 3662 2d69 6e74 385d 2868  atglm-6b-int8](h
+00002550: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00002560: 6365 2e63 6f2f 7468 7564 6d2f 6368 6174  ce.co/thudm/chat
+00002570: 676c 6d2d 3662 2d69 6e74 3829 0a2d 205b  glm-6b-int8).- [
+00002580: 7468 7564 6d2f 6368 6174 676c 6d2d 3662  thudm/chatglm-6b
+00002590: 2d69 6e74 345d 2868 7474 7073 3a2f 2f68  -int4](https://h
+000025a0: 7567 6769 6e67 6661 6365 2e63 6f2f 7468  uggingface.co/th
+000025b0: 7564 6d2f 6368 6174 676c 6d2d 3662 2d69  udm/chatglm-6b-i
+000025c0: 6e74 3429 0a2d 205b 7468 7564 6d2f 6368  nt4).- [thudm/ch
+000025d0: 6174 676c 6d32 2d36 625d 2868 7474 7073  atglm2-6b](https
+000025e0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+000025f0: 6f2f 7468 7564 6d2f 6368 6174 676c 6d32  o/thudm/chatglm2
+00002600: 2d36 6229 0a2d 205b 7468 7564 6d2f 6368  -6b).- [thudm/ch
+00002610: 6174 676c 6d32 2d36 622d 696e 7434 5d28  atglm2-6b-int4](
+00002620: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00002630: 6163 652e 636f 2f74 6875 646d 2f63 6861  ace.co/thudm/cha
+00002640: 7467 6c6d 322d 3662 2d69 6e74 3429 0a2d  tglm2-6b-int4).-
+00002650: 205b 7468 7564 6d2f 6368 6174 676c 6d33   [thudm/chatglm3
+00002660: 2d36 625d 2868 7474 7073 3a2f 2f68 7567  -6b](https://hug
+00002670: 6769 6e67 6661 6365 2e63 6f2f 7468 7564  gingface.co/thud
+00002680: 6d2f 6368 6174 676c 6d33 2d36 6229 0a0a  m/chatglm3-6b)..
+00002690: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+000026a0: 6169 6c73 3e0a 0a3c 7375 6d6d 6172 793e  ails>..<summary>
+000026b0: 4462 7278 3c2f 7375 6d6d 6172 793e 0a0a  Dbrx</summary>..
+000026c0: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
+000026d0: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2044  ...> **Note:** D
+000026e0: 6272 7820 7265 7175 6972 6573 2074 6f20  brx requires to 
+000026f0: 696e 7374 616c 6c20 7769 7468 3a0a 3e20  install with:.> 
+00002700: 6060 6062 6173 680a 3e20 7069 7020 696e  ```bash.> pip in
+00002710: 7374 616c 6c20 226f 7065 6e6c 6c6d 5b64  stall "openllm[d
+00002720: 6272 785d 220a 3e20 6060 600a 0a0a 5275  brx]".> ```...Ru
+00002730: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+00002740: 636f 6d6d 616e 6420 746f 2071 7569 636b  command to quick
+00002750: 6c79 2073 7069 6e20 7570 2061 2044 6272  ly spin up a Dbr
+00002760: 7820 7365 7276 6572 3a0a 0a60 6060 6261  x server:..```ba
+00002770: 7368 0a54 5255 5354 5f52 454d 4f54 455f  sh.TRUST_REMOTE_
+00002780: 434f 4445 3d54 7275 6520 6f70 656e 6c6c  CODE=True openll
+00002790: 6d20 7374 6172 7420 6461 7461 6272 6963  m start databric
+000027a0: 6b73 2f64 6272 782d 696e 7374 7275 6374  ks/dbrx-instruct
+000027b0: 0a60 6060 0a49 6e20 6120 6469 6666 6572  .```.In a differ
+000027c0: 656e 7420 7465 726d 696e 616c 2c20 7275  ent terminal, ru
+000027d0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000027e0: 636f 6d6d 616e 6420 746f 2069 6e74 6572  command to inter
+000027f0: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
+00002800: 7665 723a 0a0a 6060 6062 6173 680a 6578  ver:..```bash.ex
+00002810: 706f 7274 204f 5045 4e4c 4c4d 5f45 4e44  port OPENLLM_END
+00002820: 504f 494e 543d 6874 7470 3a2f 2f6c 6f63  POINT=http://loc
+00002830: 616c 686f 7374 3a33 3030 300a 6f70 656e  alhost:3000.open
+00002840: 6c6c 6d20 7175 6572 7920 2757 6861 7420  llm query 'What 
+00002850: 6172 6520 6c61 7267 6520 6c61 6e67 7561  are large langua
+00002860: 6765 206d 6f64 656c 733f 270a 6060 600a  ge models?'.```.
+00002870: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 416e  ..> **Note:** An
+00002880: 7920 4462 7278 2076 6172 6961 6e74 7320  y Dbrx variants 
+00002890: 6361 6e20 6265 2064 6570 6c6f 7965 6420  can be deployed 
+000028a0: 7769 7468 204f 7065 6e4c 4c4d 2e20 5669  with OpenLLM. Vi
+000028b0: 7369 7420 7468 6520 5b48 7567 6769 6e67  sit the [Hugging
+000028c0: 4661 6365 204d 6f64 656c 2048 7562 5d28  Face Model Hub](
+000028d0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+000028e0: 6163 652e 636f 2f6d 6f64 656c 733f 736f  ace.co/models?so
+000028f0: 7274 3d74 7265 6e64 696e 6726 7365 6172  rt=trending&sear
+00002900: 6368 3d64 6272 7829 2074 6f20 7365 6520  ch=dbrx) to see 
+00002910: 6d6f 7265 2044 6272 782d 636f 6d70 6174  more Dbrx-compat
+00002920: 6962 6c65 206d 6f64 656c 732e 0a0a 0a0a  ible models.....
+00002930: 2323 2320 5375 7070 6f72 7465 6420 6d6f  ### Supported mo
+00002940: 6465 6c73 0a0a 596f 7520 6361 6e20 7370  dels..You can sp
+00002950: 6563 6966 7920 616e 7920 6f66 2074 6865  ecify any of the
+00002960: 2066 6f6c 6c6f 7769 6e67 2044 6272 7820   following Dbrx 
+00002970: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
+00002980: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
+00002990: 5b64 6174 6162 7269 636b 732f 6462 7278  [databricks/dbrx
+000029a0: 2d69 6e73 7472 7563 745d 2868 7474 7073  -instruct](https
+000029b0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+000029c0: 6f2f 6461 7461 6272 6963 6b73 2f64 6272  o/databricks/dbr
+000029d0: 782d 696e 7374 7275 6374 290a 2d20 5b64  x-instruct).- [d
+000029e0: 6174 6162 7269 636b 732f 6462 7278 2d62  atabricks/dbrx-b
+000029f0: 6173 655d 2868 7474 7073 3a2f 2f68 7567  ase](https://hug
+00002a00: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
+00002a10: 6272 6963 6b73 2f64 6272 782d 6261 7365  bricks/dbrx-base
+00002a20: 290a 0a3c 2f64 6574 6169 6c73 3e0a 0a3c  )..</details>..<
+00002a30: 6465 7461 696c 733e 0a0a 3c73 756d 6d61  details>..<summa
+00002a40: 7279 3e44 6f6c 6c79 5632 3c2f 7375 6d6d  ry>DollyV2</summ
+00002a50: 6172 793e 0a0a 0a23 2323 2051 7569 636b  ary>...### Quick
+00002a60: 7374 6172 740a 0a52 756e 2074 6865 2066  start..Run the f
+00002a70: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00002a80: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
+00002a90: 2075 7020 6120 446f 6c6c 7956 3220 7365   up a DollyV2 se
+00002aa0: 7276 6572 3a0a 0a60 6060 6261 7368 0a54  rver:..```bash.T
+00002ab0: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
+00002ac0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
+00002ad0: 6172 7420 6461 7461 6272 6963 6b73 2f64  art databricks/d
+00002ae0: 6f6c 6c79 2d76 322d 3362 0a60 6060 0a49  olly-v2-3b.```.I
+00002af0: 6e20 6120 6469 6666 6572 656e 7420 7465  n a different te
+00002b00: 726d 696e 616c 2c20 7275 6e20 7468 6520  rminal, run the 
+00002b10: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00002b20: 6420 746f 2069 6e74 6572 6163 7420 7769  d to interact wi
+00002b30: 7468 2074 6865 2073 6572 7665 723a 0a0a  th the server:..
+00002b40: 6060 6062 6173 680a 6578 706f 7274 204f  ```bash.export O
+00002b50: 5045 4e4c 4c4d 5f45 4e44 504f 494e 543d  PENLLM_ENDPOINT=
+00002b60: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00002b70: 3a33 3030 300a 6f70 656e 6c6c 6d20 7175  :3000.openllm qu
+00002b80: 6572 7920 2757 6861 7420 6172 6520 6c61  ery 'What are la
+00002b90: 7267 6520 6c61 6e67 7561 6765 206d 6f64  rge language mod
+00002ba0: 656c 733f 270a 6060 600a 0a0a 3e20 2a2a  els?'.```...> **
+00002bb0: 4e6f 7465 3a2a 2a20 416e 7920 446f 6c6c  Note:** Any Doll
+00002bc0: 7956 3220 7661 7269 616e 7473 2063 616e  yV2 variants can
+00002bd0: 2062 6520 6465 706c 6f79 6564 2077 6974   be deployed wit
+00002be0: 6820 4f70 656e 4c4c 4d2e 2056 6973 6974  h OpenLLM. Visit
+00002bf0: 2074 6865 205b 4875 6767 696e 6746 6163   the [HuggingFac
+00002c00: 6520 4d6f 6465 6c20 4875 625d 2868 7474  e Model Hub](htt
+00002c10: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00002c20: 2e63 6f2f 6d6f 6465 6c73 3f73 6f72 743d  .co/models?sort=
+00002c30: 7472 656e 6469 6e67 2673 6561 7263 683d  trending&search=
+00002c40: 646f 6c6c 795f 7632 2920 746f 2073 6565  dolly_v2) to see
+00002c50: 206d 6f72 6520 446f 6c6c 7956 322d 636f   more DollyV2-co
+00002c60: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
+00002c70: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
+00002c80: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
+00002c90: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
+00002ca0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2044   the following D
+00002cb0: 6f6c 6c79 5632 206d 6f64 656c 7320 7669  ollyV2 models vi
+00002cc0: 6120 606f 7065 6e6c 6c6d 2073 7461 7274  a `openllm start
+00002cd0: 603a 0a0a 0a2d 205b 6461 7461 6272 6963  `:...- [databric
+00002ce0: 6b73 2f64 6f6c 6c79 2d76 322d 3362 5d28  ks/dolly-v2-3b](
+00002cf0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00002d00: 6163 652e 636f 2f64 6174 6162 7269 636b  ace.co/databrick
+00002d10: 732f 646f 6c6c 792d 7632 2d33 6229 0a2d  s/dolly-v2-3b).-
+00002d20: 205b 6461 7461 6272 6963 6b73 2f64 6f6c   [databricks/dol
+00002d30: 6c79 2d76 322d 3762 5d28 6874 7470 733a  ly-v2-7b](https:
+00002d40: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00002d50: 2f64 6174 6162 7269 636b 732f 646f 6c6c  /databricks/doll
+00002d60: 792d 7632 2d37 6229 0a2d 205b 6461 7461  y-v2-7b).- [data
+00002d70: 6272 6963 6b73 2f64 6f6c 6c79 2d76 322d  bricks/dolly-v2-
+00002d80: 3132 625d 2868 7474 7073 3a2f 2f68 7567  12b](https://hug
+00002d90: 6769 6e67 6661 6365 2e63 6f2f 6461 7461  gingface.co/data
+00002da0: 6272 6963 6b73 2f64 6f6c 6c79 2d76 322d  bricks/dolly-v2-
+00002db0: 3132 6229 0a0a 3c2f 6465 7461 696c 733e  12b)..</details>
+00002dc0: 0a0a 3c64 6574 6169 6c73 3e0a 0a3c 7375  ..<details>..<su
+00002dd0: 6d6d 6172 793e 4661 6c63 6f6e 3c2f 7375  mmary>Falcon</su
+00002de0: 6d6d 6172 793e 0a0a 0a23 2323 2051 7569  mmary>...### Qui
+00002df0: 636b 7374 6172 740a 0a0a 0a3e 202a 2a4e  ckstart....> **N
+00002e00: 6f74 653a 2a2a 2046 616c 636f 6e20 7265  ote:** Falcon re
+00002e10: 7175 6972 6573 2074 6f20 696e 7374 616c  quires to instal
+00002e20: 6c20 7769 7468 3a0a 3e20 6060 6062 6173  l with:.> ```bas
+00002e30: 680a 3e20 7069 7020 696e 7374 616c 6c20  h.> pip install 
+00002e40: 226f 7065 6e6c 6c6d 5b66 616c 636f 6e5d  "openllm[falcon]
+00002e50: 220a 3e20 6060 600a 0a0a 5275 6e20 7468  ".> ```...Run th
+00002e60: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00002e70: 616e 6420 746f 2071 7569 636b 6c79 2073  and to quickly s
+00002e80: 7069 6e20 7570 2061 2046 616c 636f 6e20  pin up a Falcon 
+00002e90: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+00002ea0: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
+00002eb0: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
+00002ec0: 7374 6172 7420 7469 6975 6165 2f66 616c  start tiiuae/fal
+00002ed0: 636f 6e2d 3762 0a60 6060 0a49 6e20 6120  con-7b.```.In a 
+00002ee0: 6469 6666 6572 656e 7420 7465 726d 696e  different termin
+00002ef0: 616c 2c20 7275 6e20 7468 6520 666f 6c6c  al, run the foll
+00002f00: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
+00002f10: 2069 6e74 6572 6163 7420 7769 7468 2074   interact with t
+00002f20: 6865 2073 6572 7665 723a 0a0a 6060 6062  he server:..```b
+00002f30: 6173 680a 6578 706f 7274 204f 5045 4e4c  ash.export OPENL
+00002f40: 4c4d 5f45 4e44 504f 494e 543d 6874 7470  LM_ENDPOINT=http
+00002f50: 3a2f 2f6c 6f63 616c 686f 7374 3a33 3030  ://localhost:300
+00002f60: 300a 6f70 656e 6c6c 6d20 7175 6572 7920  0.openllm query 
+00002f70: 2757 6861 7420 6172 6520 6c61 7267 6520  'What are large 
+00002f80: 6c61 6e67 7561 6765 206d 6f64 656c 733f  language models?
+00002f90: 270a 6060 600a 0a0a 3e20 2a2a 4e6f 7465  '.```...> **Note
+00002fa0: 3a2a 2a20 416e 7920 4661 6c63 6f6e 2076  :** Any Falcon v
+00002fb0: 6172 6961 6e74 7320 6361 6e20 6265 2064  ariants can be d
+00002fc0: 6570 6c6f 7965 6420 7769 7468 204f 7065  eployed with Ope
+00002fd0: 6e4c 4c4d 2e20 5669 7369 7420 7468 6520  nLLM. Visit the 
+00002fe0: 5b48 7567 6769 6e67 4661 6365 204d 6f64  [HuggingFace Mod
+00002ff0: 656c 2048 7562 5d28 6874 7470 733a 2f2f  el Hub](https://
+00003000: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
+00003010: 6f64 656c 733f 736f 7274 3d74 7265 6e64  odels?sort=trend
+00003020: 696e 6726 7365 6172 6368 3d66 616c 636f  ing&search=falco
+00003030: 6e29 2074 6f20 7365 6520 6d6f 7265 2046  n) to see more F
+00003040: 616c 636f 6e2d 636f 6d70 6174 6962 6c65  alcon-compatible
+00003050: 206d 6f64 656c 732e 0a0a 0a0a 2323 2320   models.....### 
+00003060: 5375 7070 6f72 7465 6420 6d6f 6465 6c73  Supported models
+00003070: 0a0a 596f 7520 6361 6e20 7370 6563 6966  ..You can specif
+00003080: 7920 616e 7920 6f66 2074 6865 2066 6f6c  y any of the fol
+00003090: 6c6f 7769 6e67 2046 616c 636f 6e20 6d6f  lowing Falcon mo
+000030a0: 6465 6c73 2076 6961 2060 6f70 656e 6c6c  dels via `openll
+000030b0: 6d20 7374 6172 7460 3a0a 0a0a 2d20 5b74  m start`:...- [t
+000030c0: 6969 7561 652f 6661 6c63 6f6e 2d37 625d  iiuae/falcon-7b]
+000030d0: 2868 7474 7073 3a2f 2f68 7567 6769 6e67  (https://hugging
+000030e0: 6661 6365 2e63 6f2f 7469 6975 6165 2f66  face.co/tiiuae/f
+000030f0: 616c 636f 6e2d 3762 290a 2d20 5b74 6969  alcon-7b).- [tii
+00003100: 7561 652f 6661 6c63 6f6e 2d34 3062 5d28  uae/falcon-40b](
+00003110: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00003120: 6163 652e 636f 2f74 6969 7561 652f 6661  ace.co/tiiuae/fa
+00003130: 6c63 6f6e 2d34 3062 290a 2d20 5b74 6969  lcon-40b).- [tii
+00003140: 7561 652f 6661 6c63 6f6e 2d37 622d 696e  uae/falcon-7b-in
+00003150: 7374 7275 6374 5d28 6874 7470 733a 2f2f  struct](https://
+00003160: 6875 6767 696e 6766 6163 652e 636f 2f74  huggingface.co/t
+00003170: 6969 7561 652f 6661 6c63 6f6e 2d37 622d  iiuae/falcon-7b-
+00003180: 696e 7374 7275 6374 290a 2d20 5b74 6969  instruct).- [tii
+00003190: 7561 652f 6661 6c63 6f6e 2d34 3062 2d69  uae/falcon-40b-i
+000031a0: 6e73 7472 7563 745d 2868 7474 7073 3a2f  nstruct](https:/
+000031b0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+000031c0: 7469 6975 6165 2f66 616c 636f 6e2d 3430  tiiuae/falcon-40
+000031d0: 622d 696e 7374 7275 6374 290a 0a3c 2f64  b-instruct)..</d
+000031e0: 6574 6169 6c73 3e0a 0a3c 6465 7461 696c  etails>..<detail
+000031f0: 733e 0a0a 3c73 756d 6d61 7279 3e46 6c61  s>..<summary>Fla
+00003200: 6e54 353c 2f73 756d 6d61 7279 3e0a 0a0a  nT5</summary>...
+00003210: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
+00003220: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
+00003230: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
+00003240: 636b 6c79 2073 7069 6e20 7570 2061 2046  ckly spin up a F
+00003250: 6c61 6e54 3520 7365 7276 6572 3a0a 0a60  lanT5 server:..`
+00003260: 6060 6261 7368 0a54 5255 5354 5f52 454d  ``bash.TRUST_REM
+00003270: 4f54 455f 434f 4445 3d54 7275 6520 6f70  OTE_CODE=True op
+00003280: 656e 6c6c 6d20 7374 6172 7420 676f 6f67  enllm start goog
+00003290: 6c65 2f66 6c61 6e2d 7435 2d6c 6172 6765  le/flan-t5-large
+000032a0: 0a60 6060 0a49 6e20 6120 6469 6666 6572  .```.In a differ
+000032b0: 656e 7420 7465 726d 696e 616c 2c20 7275  ent terminal, ru
+000032c0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000032d0: 636f 6d6d 616e 6420 746f 2069 6e74 6572  command to inter
+000032e0: 6163 7420 7769 7468 2074 6865 2073 6572  act with the ser
+000032f0: 7665 723a 0a0a 6060 6062 6173 680a 6578  ver:..```bash.ex
+00003300: 706f 7274 204f 5045 4e4c 4c4d 5f45 4e44  port OPENLLM_END
+00003310: 504f 494e 543d 6874 7470 3a2f 2f6c 6f63  POINT=http://loc
+00003320: 616c 686f 7374 3a33 3030 300a 6f70 656e  alhost:3000.open
+00003330: 6c6c 6d20 7175 6572 7920 2757 6861 7420  llm query 'What 
+00003340: 6172 6520 6c61 7267 6520 6c61 6e67 7561  are large langua
+00003350: 6765 206d 6f64 656c 733f 270a 6060 600a  ge models?'.```.
+00003360: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 416e  ..> **Note:** An
+00003370: 7920 466c 616e 5435 2076 6172 6961 6e74  y FlanT5 variant
+00003380: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
+00003390: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
+000033a0: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
+000033b0: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
+000033c0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+000033d0: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
+000033e0: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
+000033f0: 6172 6368 3d66 6c61 6e5f 7435 2920 746f  arch=flan_t5) to
+00003400: 2073 6565 206d 6f72 6520 466c 616e 5435   see more FlanT5
+00003410: 2d63 6f6d 7061 7469 626c 6520 6d6f 6465  -compatible mode
+00003420: 6c73 2e0a 0a0a 0a23 2323 2053 7570 706f  ls.....### Suppo
+00003430: 7274 6564 206d 6f64 656c 730a 0a59 6f75  rted models..You
+00003440: 2063 616e 2073 7065 6369 6679 2061 6e79   can specify any
+00003450: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00003460: 6720 466c 616e 5435 206d 6f64 656c 7320  g FlanT5 models 
+00003470: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
+00003480: 7274 603a 0a0a 0a2d 205b 676f 6f67 6c65  rt`:...- [google
+00003490: 2f66 6c61 6e2d 7435 2d73 6d61 6c6c 5d28  /flan-t5-small](
+000034a0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+000034b0: 6163 652e 636f 2f67 6f6f 676c 652f 666c  ace.co/google/fl
+000034c0: 616e 2d74 352d 736d 616c 6c29 0a2d 205b  an-t5-small).- [
+000034d0: 676f 6f67 6c65 2f66 6c61 6e2d 7435 2d62  google/flan-t5-b
+000034e0: 6173 655d 2868 7474 7073 3a2f 2f68 7567  ase](https://hug
+000034f0: 6769 6e67 6661 6365 2e63 6f2f 676f 6f67  gingface.co/goog
+00003500: 6c65 2f66 6c61 6e2d 7435 2d62 6173 6529  le/flan-t5-base)
+00003510: 0a2d 205b 676f 6f67 6c65 2f66 6c61 6e2d  .- [google/flan-
+00003520: 7435 2d6c 6172 6765 5d28 6874 7470 733a  t5-large](https:
+00003530: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00003540: 2f67 6f6f 676c 652f 666c 616e 2d74 352d  /google/flan-t5-
+00003550: 6c61 7267 6529 0a2d 205b 676f 6f67 6c65  large).- [google
+00003560: 2f66 6c61 6e2d 7435 2d78 6c5d 2868 7474  /flan-t5-xl](htt
+00003570: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00003580: 2e63 6f2f 676f 6f67 6c65 2f66 6c61 6e2d  .co/google/flan-
+00003590: 7435 2d78 6c29 0a2d 205b 676f 6f67 6c65  t5-xl).- [google
+000035a0: 2f66 6c61 6e2d 7435 2d78 786c 5d28 6874  /flan-t5-xxl](ht
+000035b0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+000035c0: 652e 636f 2f67 6f6f 676c 652f 666c 616e  e.co/google/flan
+000035d0: 2d74 352d 7878 6c29 0a0a 3c2f 6465 7461  -t5-xxl)..</deta
+000035e0: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
+000035f0: 0a3c 7375 6d6d 6172 793e 4765 6d6d 613c  .<summary>Gemma<
+00003600: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
+00003610: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
+00003620: 2a2a 4e6f 7465 3a2a 2a20 4765 6d6d 6120  **Note:** Gemma 
+00003630: 7265 7175 6972 6573 2074 6f20 696e 7374  requires to inst
+00003640: 616c 6c20 7769 7468 3a0a 3e20 6060 6062  all with:.> ```b
+00003650: 6173 680a 3e20 7069 7020 696e 7374 616c  ash.> pip instal
+00003660: 6c20 226f 7065 6e6c 6c6d 5b67 656d 6d61  l "openllm[gemma
+00003670: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
+00003680: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00003690: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
+000036a0: 7370 696e 2075 7020 6120 4765 6d6d 6120  spin up a Gemma 
+000036b0: 7365 7276 6572 3a0a 0a60 6060 6261 7368  server:..```bash
+000036c0: 0a54 5255 5354 5f52 454d 4f54 455f 434f  .TRUST_REMOTE_CO
+000036d0: 4445 3d54 7275 6520 6f70 656e 6c6c 6d20  DE=True openllm 
+000036e0: 7374 6172 7420 676f 6f67 6c65 2f67 656d  start google/gem
+000036f0: 6d61 2d37 620a 6060 600a 496e 2061 2064  ma-7b.```.In a d
+00003700: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
+00003710: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
+00003720: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+00003730: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
+00003740: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
+00003750: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
+00003760: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
+00003770: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
+00003780: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
+00003790: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
+000037a0: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
+000037b0: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
+000037c0: 2a2a 2041 6e79 2047 656d 6d61 2076 6172  ** Any Gemma var
+000037d0: 6961 6e74 7320 6361 6e20 6265 2064 6570  iants can be dep
+000037e0: 6c6f 7965 6420 7769 7468 204f 7065 6e4c  loyed with OpenL
+000037f0: 4c4d 2e20 5669 7369 7420 7468 6520 5b48  LM. Visit the [H
+00003800: 7567 6769 6e67 4661 6365 204d 6f64 656c  uggingFace Model
+00003810: 2048 7562 5d28 6874 7470 733a 2f2f 6875   Hub](https://hu
+00003820: 6767 696e 6766 6163 652e 636f 2f6d 6f64  ggingface.co/mod
+00003830: 656c 733f 736f 7274 3d74 7265 6e64 696e  els?sort=trendin
+00003840: 6726 7365 6172 6368 3d67 656d 6d61 2920  g&search=gemma) 
+00003850: 746f 2073 6565 206d 6f72 6520 4765 6d6d  to see more Gemm
+00003860: 612d 636f 6d70 6174 6962 6c65 206d 6f64  a-compatible mod
+00003870: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
+00003880: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
+00003890: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
+000038a0: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
+000038b0: 6e67 2047 656d 6d61 206d 6f64 656c 7320  ng Gemma models 
+000038c0: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
+000038d0: 7274 603a 0a0a 0a2d 205b 676f 6f67 6c65  rt`:...- [google
+000038e0: 2f67 656d 6d61 2d37 625d 2868 7474 7073  /gemma-7b](https
+000038f0: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00003900: 6f2f 676f 6f67 6c65 2f67 656d 6d61 2d37  o/google/gemma-7
+00003910: 6229 0a2d 205b 676f 6f67 6c65 2f67 656d  b).- [google/gem
+00003920: 6d61 2d37 622d 6974 5d28 6874 7470 733a  ma-7b-it](https:
+00003930: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00003940: 2f67 6f6f 676c 652f 6765 6d6d 612d 3762  /google/gemma-7b
+00003950: 2d69 7429 0a2d 205b 676f 6f67 6c65 2f67  -it).- [google/g
+00003960: 656d 6d61 2d32 625d 2868 7474 7073 3a2f  emma-2b](https:/
+00003970: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00003980: 676f 6f67 6c65 2f67 656d 6d61 2d32 6229  google/gemma-2b)
+00003990: 0a2d 205b 676f 6f67 6c65 2f67 656d 6d61  .- [google/gemma
+000039a0: 2d32 622d 6974 5d28 6874 7470 733a 2f2f  -2b-it](https://
+000039b0: 6875 6767 696e 6766 6163 652e 636f 2f67  huggingface.co/g
+000039c0: 6f6f 676c 652f 6765 6d6d 612d 3262 2d69  oogle/gemma-2b-i
+000039d0: 7429 0a0a 3c2f 6465 7461 696c 733e 0a0a  t)..</details>..
+000039e0: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+000039f0: 6172 793e 4750 544e 656f 583c 2f73 756d  ary>GPTNeoX</sum
+00003a00: 6d61 7279 3e0a 0a0a 2323 2320 5175 6963  mary>...### Quic
+00003a10: 6b73 7461 7274 0a0a 5275 6e20 7468 6520  kstart..Run the 
+00003a20: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00003a30: 6420 746f 2071 7569 636b 6c79 2073 7069  d to quickly spi
+00003a40: 6e20 7570 2061 2047 5054 4e65 6f58 2073  n up a GPTNeoX s
+00003a50: 6572 7665 723a 0a0a 6060 6062 6173 680a  erver:..```bash.
+00003a60: 5452 5553 545f 5245 4d4f 5445 5f43 4f44  TRUST_REMOTE_COD
+00003a70: 453d 5472 7565 206f 7065 6e6c 6c6d 2073  E=True openllm s
+00003a80: 7461 7274 2065 6c65 7574 6865 7261 692f  tart eleutherai/
+00003a90: 6770 742d 6e65 6f78 2d32 3062 0a60 6060  gpt-neox-20b.```
+00003aa0: 0a49 6e20 6120 6469 6666 6572 656e 7420  .In a different 
+00003ab0: 7465 726d 696e 616c 2c20 7275 6e20 7468  terminal, run th
+00003ac0: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00003ad0: 616e 6420 746f 2069 6e74 6572 6163 7420  and to interact 
+00003ae0: 7769 7468 2074 6865 2073 6572 7665 723a  with the server:
+00003af0: 0a0a 6060 6062 6173 680a 6578 706f 7274  ..```bash.export
+00003b00: 204f 5045 4e4c 4c4d 5f45 4e44 504f 494e   OPENLLM_ENDPOIN
+00003b10: 543d 6874 7470 3a2f 2f6c 6f63 616c 686f  T=http://localho
+00003b20: 7374 3a33 3030 300a 6f70 656e 6c6c 6d20  st:3000.openllm 
+00003b30: 7175 6572 7920 2757 6861 7420 6172 6520  query 'What are 
+00003b40: 6c61 7267 6520 6c61 6e67 7561 6765 206d  large language m
+00003b50: 6f64 656c 733f 270a 6060 600a 0a0a 3e20  odels?'.```...> 
+00003b60: 2a2a 4e6f 7465 3a2a 2a20 416e 7920 4750  **Note:** Any GP
+00003b70: 544e 656f 5820 7661 7269 616e 7473 2063  TNeoX variants c
+00003b80: 616e 2062 6520 6465 706c 6f79 6564 2077  an be deployed w
+00003b90: 6974 6820 4f70 656e 4c4c 4d2e 2056 6973  ith OpenLLM. Vis
+00003ba0: 6974 2074 6865 205b 4875 6767 696e 6746  it the [HuggingF
+00003bb0: 6163 6520 4d6f 6465 6c20 4875 625d 2868  ace Model Hub](h
+00003bc0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00003bd0: 6365 2e63 6f2f 6d6f 6465 6c73 3f73 6f72  ce.co/models?sor
+00003be0: 743d 7472 656e 6469 6e67 2673 6561 7263  t=trending&searc
+00003bf0: 683d 6770 745f 6e65 6f78 2920 746f 2073  h=gpt_neox) to s
+00003c00: 6565 206d 6f72 6520 4750 544e 656f 582d  ee more GPTNeoX-
+00003c10: 636f 6d70 6174 6962 6c65 206d 6f64 656c  compatible model
+00003c20: 732e 0a0a 0a0a 2323 2320 5375 7070 6f72  s.....### Suppor
+00003c30: 7465 6420 6d6f 6465 6c73 0a0a 596f 7520  ted models..You 
+00003c40: 6361 6e20 7370 6563 6966 7920 616e 7920  can specify any 
+00003c50: 6f66 2074 6865 2066 6f6c 6c6f 7769 6e67  of the following
+00003c60: 2047 5054 4e65 6f58 206d 6f64 656c 7320   GPTNeoX models 
+00003c70: 7669 6120 606f 7065 6e6c 6c6d 2073 7461  via `openllm sta
+00003c80: 7274 603a 0a0a 0a2d 205b 656c 6575 7468  rt`:...- [eleuth
+00003c90: 6572 6169 2f67 7074 2d6e 656f 782d 3230  erai/gpt-neox-20
+00003ca0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00003cb0: 6e67 6661 6365 2e63 6f2f 656c 6575 7468  ngface.co/eleuth
+00003cc0: 6572 6169 2f67 7074 2d6e 656f 782d 3230  erai/gpt-neox-20
+00003cd0: 6229 0a0a 3c2f 6465 7461 696c 733e 0a0a  b)..</details>..
+00003ce0: 3c64 6574 6169 6c73 3e0a 0a3c 7375 6d6d  <details>..<summ
+00003cf0: 6172 793e 4c6c 616d 613c 2f73 756d 6d61  ary>Llama</summa
+00003d00: 7279 3e0a 0a0a 2323 2320 5175 6963 6b73  ry>...### Quicks
+00003d10: 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465  tart....> **Note
+00003d20: 3a2a 2a20 4c6c 616d 6120 7265 7175 6972  :** Llama requir
+00003d30: 6573 2074 6f20 696e 7374 616c 6c20 7769  es to install wi
+00003d40: 7468 3a0a 3e20 6060 6062 6173 680a 3e20  th:.> ```bash.> 
+00003d50: 7069 7020 696e 7374 616c 6c20 226f 7065  pip install "ope
+00003d60: 6e6c 6c6d 5b6c 6c61 6d61 5d22 0a3e 2060  nllm[llama]".> `
+00003d70: 6060 0a0a 0a52 756e 2074 6865 2066 6f6c  ``...Run the fol
+00003d80: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+00003d90: 6f20 7175 6963 6b6c 7920 7370 696e 2075  o quickly spin u
+00003da0: 7020 6120 4c6c 616d 6120 7365 7276 6572  p a Llama server
+00003db0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
+00003dc0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
+00003dd0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
+00003de0: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
+00003df0: 6d61 2d32 2d37 622d 6866 0a60 6060 0a49  ma-2-7b-hf.```.I
+00003e00: 6e20 6120 6469 6666 6572 656e 7420 7465  n a different te
+00003e10: 726d 696e 616c 2c20 7275 6e20 7468 6520  rminal, run the 
+00003e20: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00003e30: 6420 746f 2069 6e74 6572 6163 7420 7769  d to interact wi
+00003e40: 7468 2074 6865 2073 6572 7665 723a 0a0a  th the server:..
+00003e50: 6060 6062 6173 680a 6578 706f 7274 204f  ```bash.export O
+00003e60: 5045 4e4c 4c4d 5f45 4e44 504f 494e 543d  PENLLM_ENDPOINT=
+00003e70: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+00003e80: 3a33 3030 300a 6f70 656e 6c6c 6d20 7175  :3000.openllm qu
+00003e90: 6572 7920 2757 6861 7420 6172 6520 6c61  ery 'What are la
+00003ea0: 7267 6520 6c61 6e67 7561 6765 206d 6f64  rge language mod
+00003eb0: 656c 733f 270a 6060 600a 0a0a 3e20 2a2a  els?'.```...> **
+00003ec0: 4e6f 7465 3a2a 2a20 416e 7920 4c6c 616d  Note:** Any Llam
+00003ed0: 6120 7661 7269 616e 7473 2063 616e 2062  a variants can b
+00003ee0: 6520 6465 706c 6f79 6564 2077 6974 6820  e deployed with 
+00003ef0: 4f70 656e 4c4c 4d2e 2056 6973 6974 2074  OpenLLM. Visit t
+00003f00: 6865 205b 4875 6767 696e 6746 6163 6520  he [HuggingFace 
+00003f10: 4d6f 6465 6c20 4875 625d 2868 7474 7073  Model Hub](https
+00003f20: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00003f30: 6f2f 6d6f 6465 6c73 3f73 6f72 743d 7472  o/models?sort=tr
+00003f40: 656e 6469 6e67 2673 6561 7263 683d 6c6c  ending&search=ll
+00003f50: 616d 6129 2074 6f20 7365 6520 6d6f 7265  ama) to see more
+00003f60: 204c 6c61 6d61 2d63 6f6d 7061 7469 626c   Llama-compatibl
+00003f70: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
+00003f80: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
+00003f90: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
+00003fa0: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
+00003fb0: 6c6c 6f77 696e 6720 4c6c 616d 6120 6d6f  llowing Llama mo
+00003fc0: 6465 6c73 2076 6961 2060 6f70 656e 6c6c  dels via `openll
+00003fd0: 6d20 7374 6172 7460 3a0a 0a0a 2d20 5b6d  m start`:...- [m
+00003fe0: 6574 612d 6c6c 616d 612f 4c6c 616d 612d  eta-llama/Llama-
+00003ff0: 322d 3730 622d 6368 6174 2d68 665d 2868  2-70b-chat-hf](h
+00004000: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00004010: 6365 2e63 6f2f 6d65 7461 2d6c 6c61 6d61  ce.co/meta-llama
+00004020: 2f4c 6c61 6d61 2d32 2d37 3062 2d63 6861  /Llama-2-70b-cha
+00004030: 742d 6866 290a 2d20 5b6d 6574 612d 6c6c  t-hf).- [meta-ll
+00004040: 616d 612f 4c6c 616d 612d 322d 3133 622d  ama/Llama-2-13b-
+00004050: 6368 6174 2d68 665d 2868 7474 7073 3a2f  chat-hf](https:/
+00004060: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00004070: 6d65 7461 2d6c 6c61 6d61 2f4c 6c61 6d61  meta-llama/Llama
+00004080: 2d32 2d31 3362 2d63 6861 742d 6866 290a  -2-13b-chat-hf).
+00004090: 2d20 5b6d 6574 612d 6c6c 616d 612f 4c6c  - [meta-llama/Ll
+000040a0: 616d 612d 322d 3762 2d63 6861 742d 6866  ama-2-7b-chat-hf
+000040b0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+000040c0: 6766 6163 652e 636f 2f6d 6574 612d 6c6c  gface.co/meta-ll
+000040d0: 616d 612f 4c6c 616d 612d 322d 3762 2d63  ama/Llama-2-7b-c
+000040e0: 6861 742d 6866 290a 2d20 5b6d 6574 612d  hat-hf).- [meta-
+000040f0: 6c6c 616d 612f 4c6c 616d 612d 322d 3730  llama/Llama-2-70
+00004100: 622d 6866 5d28 6874 7470 733a 2f2f 6875  b-hf](https://hu
+00004110: 6767 696e 6766 6163 652e 636f 2f6d 6574  ggingface.co/met
+00004120: 612d 6c6c 616d 612f 4c6c 616d 612d 322d  a-llama/Llama-2-
+00004130: 3730 622d 6866 290a 2d20 5b6d 6574 612d  70b-hf).- [meta-
+00004140: 6c6c 616d 612f 4c6c 616d 612d 322d 3133  llama/Llama-2-13
+00004150: 622d 6866 5d28 6874 7470 733a 2f2f 6875  b-hf](https://hu
+00004160: 6767 696e 6766 6163 652e 636f 2f6d 6574  ggingface.co/met
+00004170: 612d 6c6c 616d 612f 4c6c 616d 612d 322d  a-llama/Llama-2-
+00004180: 3133 622d 6866 290a 2d20 5b6d 6574 612d  13b-hf).- [meta-
+00004190: 6c6c 616d 612f 4c6c 616d 612d 322d 3762  llama/Llama-2-7b
+000041a0: 2d68 665d 2868 7474 7073 3a2f 2f68 7567  -hf](https://hug
+000041b0: 6769 6e67 6661 6365 2e63 6f2f 6d65 7461  gingface.co/meta
+000041c0: 2d6c 6c61 6d61 2f4c 6c61 6d61 2d32 2d37  -llama/Llama-2-7
+000041d0: 622d 6866 290a 2d20 5b4e 6f75 7352 6573  b-hf).- [NousRes
+000041e0: 6561 7263 682f 6c6c 616d 612d 322d 3730  earch/llama-2-70
+000041f0: 622d 6368 6174 2d68 665d 2868 7474 7073  b-chat-hf](https
+00004200: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00004210: 6f2f 4e6f 7573 5265 7365 6172 6368 2f6c  o/NousResearch/l
+00004220: 6c61 6d61 2d32 2d37 3062 2d63 6861 742d  lama-2-70b-chat-
+00004230: 6866 290a 2d20 5b4e 6f75 7352 6573 6561  hf).- [NousResea
+00004240: 7263 682f 6c6c 616d 612d 322d 3133 622d  rch/llama-2-13b-
+00004250: 6368 6174 2d68 665d 2868 7474 7073 3a2f  chat-hf](https:/
+00004260: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00004270: 4e6f 7573 5265 7365 6172 6368 2f6c 6c61  NousResearch/lla
+00004280: 6d61 2d32 2d31 3362 2d63 6861 742d 6866  ma-2-13b-chat-hf
+00004290: 290a 2d20 5b4e 6f75 7352 6573 6561 7263  ).- [NousResearc
+000042a0: 682f 6c6c 616d 612d 322d 3762 2d63 6861  h/llama-2-7b-cha
+000042b0: 742d 6866 5d28 6874 7470 733a 2f2f 6875  t-hf](https://hu
+000042c0: 6767 696e 6766 6163 652e 636f 2f4e 6f75  ggingface.co/Nou
+000042d0: 7352 6573 6561 7263 682f 6c6c 616d 612d  sResearch/llama-
+000042e0: 322d 3762 2d63 6861 742d 6866 290a 2d20  2-7b-chat-hf).- 
+000042f0: 5b4e 6f75 7352 6573 6561 7263 682f 6c6c  [NousResearch/ll
+00004300: 616d 612d 322d 3730 622d 6866 5d28 6874  ama-2-70b-hf](ht
+00004310: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00004320: 652e 636f 2f4e 6f75 7352 6573 6561 7263  e.co/NousResearc
+00004330: 682f 6c6c 616d 612d 322d 3730 622d 6866  h/llama-2-70b-hf
+00004340: 290a 2d20 5b4e 6f75 7352 6573 6561 7263  ).- [NousResearc
+00004350: 682f 6c6c 616d 612d 322d 3133 622d 6866  h/llama-2-13b-hf
+00004360: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00004370: 6766 6163 652e 636f 2f4e 6f75 7352 6573  gface.co/NousRes
+00004380: 6561 7263 682f 6c6c 616d 612d 322d 3133  earch/llama-2-13
+00004390: 622d 6866 290a 2d20 5b4e 6f75 7352 6573  b-hf).- [NousRes
+000043a0: 6561 7263 682f 6c6c 616d 612d 322d 3762  earch/llama-2-7b
+000043b0: 2d68 665d 2868 7474 7073 3a2f 2f68 7567  -hf](https://hug
+000043c0: 6769 6e67 6661 6365 2e63 6f2f 4e6f 7573  gingface.co/Nous
+000043d0: 5265 7365 6172 6368 2f6c 6c61 6d61 2d32  Research/llama-2
+000043e0: 2d37 622d 6866 290a 0a3c 2f64 6574 6169  -7b-hf)..</detai
+000043f0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a0a  ls>..<details>..
+00004400: 3c73 756d 6d61 7279 3e4d 6973 7472 616c  <summary>Mistral
+00004410: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
+00004420: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
+00004430: 202a 2a4e 6f74 653a 2a2a 204d 6973 7472   **Note:** Mistr
+00004440: 616c 2072 6571 7569 7265 7320 746f 2069  al requires to i
+00004450: 6e73 7461 6c6c 2077 6974 683a 0a3e 2060  nstall with:.> `
+00004460: 6060 6261 7368 0a3e 2070 6970 2069 6e73  ``bash.> pip ins
+00004470: 7461 6c6c 2022 6f70 656e 6c6c 6d5b 6d69  tall "openllm[mi
+00004480: 7374 7261 6c5d 220a 3e20 6060 600a 0a0a  stral]".> ```...
+00004490: 5275 6e20 7468 6520 666f 6c6c 6f77 696e  Run the followin
+000044a0: 6720 636f 6d6d 616e 6420 746f 2071 7569  g command to qui
+000044b0: 636b 6c79 2073 7069 6e20 7570 2061 204d  ckly spin up a M
+000044c0: 6973 7472 616c 2073 6572 7665 723a 0a0a  istral server:..
+000044d0: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
+000044e0: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
+000044f0: 7065 6e6c 6c6d 2073 7461 7274 206d 6973  penllm start mis
+00004500: 7472 616c 6169 2f4d 6973 7472 616c 2d37  tralai/Mistral-7
+00004510: 422d 496e 7374 7275 6374 2d76 302e 310a  B-Instruct-v0.1.
+00004520: 6060 600a 496e 2061 2064 6966 6665 7265  ```.In a differe
+00004530: 6e74 2074 6572 6d69 6e61 6c2c 2072 756e  nt terminal, run
+00004540: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00004550: 6f6d 6d61 6e64 2074 6f20 696e 7465 7261  ommand to intera
+00004560: 6374 2077 6974 6820 7468 6520 7365 7276  ct with the serv
+00004570: 6572 3a0a 0a60 6060 6261 7368 0a65 7870  er:..```bash.exp
+00004580: 6f72 7420 4f50 454e 4c4c 4d5f 454e 4450  ort OPENLLM_ENDP
+00004590: 4f49 4e54 3d68 7474 703a 2f2f 6c6f 6361  OINT=http://loca
+000045a0: 6c68 6f73 743a 3330 3030 0a6f 7065 6e6c  lhost:3000.openl
+000045b0: 6c6d 2071 7565 7279 2027 5768 6174 2061  lm query 'What a
+000045c0: 7265 206c 6172 6765 206c 616e 6775 6167  re large languag
+000045d0: 6520 6d6f 6465 6c73 3f27 0a60 6060 0a0a  e models?'.```..
+000045e0: 0a3e 202a 2a4e 6f74 653a 2a2a 2041 6e79  .> **Note:** Any
+000045f0: 204d 6973 7472 616c 2076 6172 6961 6e74   Mistral variant
+00004600: 7320 6361 6e20 6265 2064 6570 6c6f 7965  s can be deploye
+00004610: 6420 7769 7468 204f 7065 6e4c 4c4d 2e20  d with OpenLLM. 
+00004620: 5669 7369 7420 7468 6520 5b48 7567 6769  Visit the [Huggi
+00004630: 6e67 4661 6365 204d 6f64 656c 2048 7562  ngFace Model Hub
+00004640: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00004650: 6766 6163 652e 636f 2f6d 6f64 656c 733f  gface.co/models?
+00004660: 736f 7274 3d74 7265 6e64 696e 6726 7365  sort=trending&se
+00004670: 6172 6368 3d6d 6973 7472 616c 2920 746f  arch=mistral) to
+00004680: 2073 6565 206d 6f72 6520 4d69 7374 7261   see more Mistra
+00004690: 6c2d 636f 6d70 6174 6962 6c65 206d 6f64  l-compatible mod
+000046a0: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
+000046b0: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
+000046c0: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
+000046d0: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
+000046e0: 6e67 204d 6973 7472 616c 206d 6f64 656c  ng Mistral model
+000046f0: 7320 7669 6120 606f 7065 6e6c 6c6d 2073  s via `openllm s
+00004700: 7461 7274 603a 0a0a 0a2d 205b 4875 6767  tart`:...- [Hugg
+00004710: 696e 6746 6163 6548 342f 7a65 7068 7972  ingFaceH4/zephyr
+00004720: 2d37 622d 616c 7068 615d 2868 7474 7073  -7b-alpha](https
+00004730: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00004740: 6f2f 4875 6767 696e 6746 6163 6548 342f  o/HuggingFaceH4/
+00004750: 7a65 7068 7972 2d37 622d 616c 7068 6129  zephyr-7b-alpha)
+00004760: 0a2d 205b 4875 6767 696e 6746 6163 6548  .- [HuggingFaceH
+00004770: 342f 7a65 7068 7972 2d37 622d 6265 7461  4/zephyr-7b-beta
+00004780: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00004790: 6766 6163 652e 636f 2f48 7567 6769 6e67  gface.co/Hugging
+000047a0: 4661 6365 4834 2f7a 6570 6879 722d 3762  FaceH4/zephyr-7b
+000047b0: 2d62 6574 6129 0a2d 205b 6d69 7374 7261  -beta).- [mistra
+000047c0: 6c61 692f 4d69 7374 7261 6c2d 3742 2d49  lai/Mistral-7B-I
+000047d0: 6e73 7472 7563 742d 7630 2e32 5d28 6874  nstruct-v0.2](ht
+000047e0: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+000047f0: 652e 636f 2f6d 6973 7472 616c 6169 2f4d  e.co/mistralai/M
+00004800: 6973 7472 616c 2d37 422d 496e 7374 7275  istral-7B-Instru
+00004810: 6374 2d76 302e 3229 0a2d 205b 6d69 7374  ct-v0.2).- [mist
+00004820: 7261 6c61 692f 4d69 7374 7261 6c2d 3742  ralai/Mistral-7B
+00004830: 2d49 6e73 7472 7563 742d 7630 2e31 5d28  -Instruct-v0.1](
+00004840: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00004850: 6163 652e 636f 2f6d 6973 7472 616c 6169  ace.co/mistralai
+00004860: 2f4d 6973 7472 616c 2d37 422d 496e 7374  /Mistral-7B-Inst
+00004870: 7275 6374 2d76 302e 3129 0a2d 205b 6d69  ruct-v0.1).- [mi
+00004880: 7374 7261 6c61 692f 4d69 7374 7261 6c2d  stralai/Mistral-
+00004890: 3742 2d76 302e 315d 2868 7474 7073 3a2f  7B-v0.1](https:/
+000048a0: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+000048b0: 6d69 7374 7261 6c61 692f 4d69 7374 7261  mistralai/Mistra
+000048c0: 6c2d 3742 2d76 302e 3129 0a0a 3c2f 6465  l-7B-v0.1)..</de
+000048d0: 7461 696c 733e 0a0a 3c64 6574 6169 6c73  tails>..<details
+000048e0: 3e0a 0a3c 7375 6d6d 6172 793e 4d69 7874  >..<summary>Mixt
+000048f0: 7261 6c3c 2f73 756d 6d61 7279 3e0a 0a0a  ral</summary>...
+00004900: 2323 2320 5175 6963 6b73 7461 7274 0a0a  ### Quickstart..
+00004910: 0a0a 3e20 2a2a 4e6f 7465 3a2a 2a20 4d69  ..> **Note:** Mi
+00004920: 7874 7261 6c20 7265 7175 6972 6573 2074  xtral requires t
+00004930: 6f20 696e 7374 616c 6c20 7769 7468 3a0a  o install with:.
+00004940: 3e20 6060 6062 6173 680a 3e20 7069 7020  > ```bash.> pip 
+00004950: 696e 7374 616c 6c20 226f 7065 6e6c 6c6d  install "openllm
+00004960: 5b6d 6978 7472 616c 5d22 0a3e 2060 6060  [mixtral]".> ```
+00004970: 0a0a 0a52 756e 2074 6865 2066 6f6c 6c6f  ...Run the follo
+00004980: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+00004990: 7175 6963 6b6c 7920 7370 696e 2075 7020  quickly spin up 
+000049a0: 6120 4d69 7874 7261 6c20 7365 7276 6572  a Mixtral server
+000049b0: 3a0a 0a60 6060 6261 7368 0a54 5255 5354  :..```bash.TRUST
+000049c0: 5f52 454d 4f54 455f 434f 4445 3d54 7275  _REMOTE_CODE=Tru
+000049d0: 6520 6f70 656e 6c6c 6d20 7374 6172 7420  e openllm start 
+000049e0: 6d69 7374 7261 6c61 692f 4d69 7874 7261  mistralai/Mixtra
+000049f0: 6c2d 3878 3742 2d49 6e73 7472 7563 742d  l-8x7B-Instruct-
+00004a00: 7630 2e31 0a60 6060 0a49 6e20 6120 6469  v0.1.```.In a di
+00004a10: 6666 6572 656e 7420 7465 726d 696e 616c  fferent terminal
+00004a20: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+00004a30: 696e 6720 636f 6d6d 616e 6420 746f 2069  ing command to i
+00004a40: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00004a50: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
+00004a60: 680a 6578 706f 7274 204f 5045 4e4c 4c4d  h.export OPENLLM
+00004a70: 5f45 4e44 504f 494e 543d 6874 7470 3a2f  _ENDPOINT=http:/
+00004a80: 2f6c 6f63 616c 686f 7374 3a33 3030 300a  /localhost:3000.
+00004a90: 6f70 656e 6c6c 6d20 7175 6572 7920 2757  openllm query 'W
+00004aa0: 6861 7420 6172 6520 6c61 7267 6520 6c61  hat are large la
+00004ab0: 6e67 7561 6765 206d 6f64 656c 733f 270a  nguage models?'.
+00004ac0: 6060 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a  ```...> **Note:*
+00004ad0: 2a20 416e 7920 4d69 7874 7261 6c20 7661  * Any Mixtral va
+00004ae0: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
+00004af0: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
+00004b00: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
+00004b10: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
+00004b20: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
+00004b30: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
+00004b40: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
+00004b50: 6e67 2673 6561 7263 683d 6d69 7874 7261  ng&search=mixtra
+00004b60: 6c29 2074 6f20 7365 6520 6d6f 7265 204d  l) to see more M
+00004b70: 6978 7472 616c 2d63 6f6d 7061 7469 626c  ixtral-compatibl
+00004b80: 6520 6d6f 6465 6c73 2e0a 0a0a 0a23 2323  e models.....###
+00004b90: 2053 7570 706f 7274 6564 206d 6f64 656c   Supported model
+00004ba0: 730a 0a59 6f75 2063 616e 2073 7065 6369  s..You can speci
+00004bb0: 6679 2061 6e79 206f 6620 7468 6520 666f  fy any of the fo
+00004bc0: 6c6c 6f77 696e 6720 4d69 7874 7261 6c20  llowing Mixtral 
+00004bd0: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
+00004be0: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
+00004bf0: 5b6d 6973 7472 616c 6169 2f4d 6978 7472  [mistralai/Mixtr
+00004c00: 616c 2d38 7837 422d 496e 7374 7275 6374  al-8x7B-Instruct
+00004c10: 2d76 302e 315d 2868 7474 7073 3a2f 2f68  -v0.1](https://h
+00004c20: 7567 6769 6e67 6661 6365 2e63 6f2f 6d69  uggingface.co/mi
+00004c30: 7374 7261 6c61 692f 4d69 7874 7261 6c2d  stralai/Mixtral-
+00004c40: 3878 3742 2d49 6e73 7472 7563 742d 7630  8x7B-Instruct-v0
+00004c50: 2e31 290a 2d20 5b6d 6973 7472 616c 6169  .1).- [mistralai
+00004c60: 2f4d 6978 7472 616c 2d38 7837 422d 7630  /Mixtral-8x7B-v0
+00004c70: 2e31 5d28 6874 7470 733a 2f2f 6875 6767  .1](https://hugg
+00004c80: 696e 6766 6163 652e 636f 2f6d 6973 7472  ingface.co/mistr
+00004c90: 616c 6169 2f4d 6978 7472 616c 2d38 7837  alai/Mixtral-8x7
+00004ca0: 422d 7630 2e31 290a 0a3c 2f64 6574 6169  B-v0.1)..</detai
+00004cb0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a0a  ls>..<details>..
+00004cc0: 3c73 756d 6d61 7279 3e4d 5054 3c2f 7375  <summary>MPT</su
+00004cd0: 6d6d 6172 793e 0a0a 0a23 2323 2051 7569  mmary>...### Qui
+00004ce0: 636b 7374 6172 740a 0a0a 0a3e 202a 2a4e  ckstart....> **N
+00004cf0: 6f74 653a 2a2a 204d 5054 2072 6571 7569  ote:** MPT requi
+00004d00: 7265 7320 746f 2069 6e73 7461 6c6c 2077  res to install w
+00004d10: 6974 683a 0a3e 2060 6060 6261 7368 0a3e  ith:.> ```bash.>
+00004d20: 2070 6970 2069 6e73 7461 6c6c 2022 6f70   pip install "op
+00004d30: 656e 6c6c 6d5b 6d70 745d 220a 3e20 6060  enllm[mpt]".> ``
+00004d40: 600a 0a0a 5275 6e20 7468 6520 666f 6c6c  `...Run the foll
+00004d50: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
+00004d60: 2071 7569 636b 6c79 2073 7069 6e20 7570   quickly spin up
+00004d70: 2061 204d 5054 2073 6572 7665 723a 0a0a   a MPT server:..
+00004d80: 6060 6062 6173 680a 5452 5553 545f 5245  ```bash.TRUST_RE
+00004d90: 4d4f 5445 5f43 4f44 453d 5472 7565 206f  MOTE_CODE=True o
+00004da0: 7065 6e6c 6c6d 2073 7461 7274 206d 6f73  penllm start mos
+00004db0: 6169 636d 6c2f 6d70 742d 3762 2d69 6e73  aicml/mpt-7b-ins
+00004dc0: 7472 7563 740a 6060 600a 496e 2061 2064  truct.```.In a d
+00004dd0: 6966 6665 7265 6e74 2074 6572 6d69 6e61  ifferent termina
+00004de0: 6c2c 2072 756e 2074 6865 2066 6f6c 6c6f  l, run the follo
+00004df0: 7769 6e67 2063 6f6d 6d61 6e64 2074 6f20  wing command to 
+00004e00: 696e 7465 7261 6374 2077 6974 6820 7468  interact with th
+00004e10: 6520 7365 7276 6572 3a0a 0a60 6060 6261  e server:..```ba
+00004e20: 7368 0a65 7870 6f72 7420 4f50 454e 4c4c  sh.export OPENLL
+00004e30: 4d5f 454e 4450 4f49 4e54 3d68 7474 703a  M_ENDPOINT=http:
+00004e40: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
+00004e50: 0a6f 7065 6e6c 6c6d 2071 7565 7279 2027  .openllm query '
+00004e60: 5768 6174 2061 7265 206c 6172 6765 206c  What are large l
+00004e70: 616e 6775 6167 6520 6d6f 6465 6c73 3f27  anguage models?'
+00004e80: 0a60 6060 0a0a 0a3e 202a 2a4e 6f74 653a  .```...> **Note:
+00004e90: 2a2a 2041 6e79 204d 5054 2076 6172 6961  ** Any MPT varia
+00004ea0: 6e74 7320 6361 6e20 6265 2064 6570 6c6f  nts can be deplo
+00004eb0: 7965 6420 7769 7468 204f 7065 6e4c 4c4d  yed with OpenLLM
+00004ec0: 2e20 5669 7369 7420 7468 6520 5b48 7567  . Visit the [Hug
+00004ed0: 6769 6e67 4661 6365 204d 6f64 656c 2048  gingFace Model H
+00004ee0: 7562 5d28 6874 7470 733a 2f2f 6875 6767  ub](https://hugg
+00004ef0: 696e 6766 6163 652e 636f 2f6d 6f64 656c  ingface.co/model
+00004f00: 733f 736f 7274 3d74 7265 6e64 696e 6726  s?sort=trending&
+00004f10: 7365 6172 6368 3d6d 7074 2920 746f 2073  search=mpt) to s
+00004f20: 6565 206d 6f72 6520 4d50 542d 636f 6d70  ee more MPT-comp
+00004f30: 6174 6962 6c65 206d 6f64 656c 732e 0a0a  atible models...
+00004f40: 0a0a 2323 2320 5375 7070 6f72 7465 6420  ..### Supported 
+00004f50: 6d6f 6465 6c73 0a0a 596f 7520 6361 6e20  models..You can 
+00004f60: 7370 6563 6966 7920 616e 7920 6f66 2074  specify any of t
+00004f70: 6865 2066 6f6c 6c6f 7769 6e67 204d 5054  he following MPT
+00004f80: 206d 6f64 656c 7320 7669 6120 606f 7065   models via `ope
+00004f90: 6e6c 6c6d 2073 7461 7274 603a 0a0a 0a2d  nllm start`:...-
+00004fa0: 205b 6d6f 7361 6963 6d6c 2f6d 7074 2d37   [mosaicml/mpt-7
+00004fb0: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00004fc0: 6e67 6661 6365 2e63 6f2f 6d6f 7361 6963  ngface.co/mosaic
+00004fd0: 6d6c 2f6d 7074 2d37 6229 0a2d 205b 6d6f  ml/mpt-7b).- [mo
+00004fe0: 7361 6963 6d6c 2f6d 7074 2d37 622d 696e  saicml/mpt-7b-in
+00004ff0: 7374 7275 6374 5d28 6874 7470 733a 2f2f  struct](https://
+00005000: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
+00005010: 6f73 6169 636d 6c2f 6d70 742d 3762 2d69  osaicml/mpt-7b-i
+00005020: 6e73 7472 7563 7429 0a2d 205b 6d6f 7361  nstruct).- [mosa
+00005030: 6963 6d6c 2f6d 7074 2d37 622d 6368 6174  icml/mpt-7b-chat
+00005040: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00005050: 6766 6163 652e 636f 2f6d 6f73 6169 636d  gface.co/mosaicm
+00005060: 6c2f 6d70 742d 3762 2d63 6861 7429 0a2d  l/mpt-7b-chat).-
+00005070: 205b 6d6f 7361 6963 6d6c 2f6d 7074 2d37   [mosaicml/mpt-7
+00005080: 622d 7374 6f72 7977 7269 7465 725d 2868  b-storywriter](h
+00005090: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+000050a0: 6365 2e63 6f2f 6d6f 7361 6963 6d6c 2f6d  ce.co/mosaicml/m
+000050b0: 7074 2d37 622d 7374 6f72 7977 7269 7465  pt-7b-storywrite
+000050c0: 7229 0a2d 205b 6d6f 7361 6963 6d6c 2f6d  r).- [mosaicml/m
+000050d0: 7074 2d33 3062 5d28 6874 7470 733a 2f2f  pt-30b](https://
+000050e0: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
+000050f0: 6f73 6169 636d 6c2f 6d70 742d 3330 6229  osaicml/mpt-30b)
+00005100: 0a2d 205b 6d6f 7361 6963 6d6c 2f6d 7074  .- [mosaicml/mpt
+00005110: 2d33 3062 2d69 6e73 7472 7563 745d 2868  -30b-instruct](h
+00005120: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+00005130: 6365 2e63 6f2f 6d6f 7361 6963 6d6c 2f6d  ce.co/mosaicml/m
+00005140: 7074 2d33 3062 2d69 6e73 7472 7563 7429  pt-30b-instruct)
+00005150: 0a2d 205b 6d6f 7361 6963 6d6c 2f6d 7074  .- [mosaicml/mpt
+00005160: 2d33 3062 2d63 6861 745d 2868 7474 7073  -30b-chat](https
+00005170: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00005180: 6f2f 6d6f 7361 6963 6d6c 2f6d 7074 2d33  o/mosaicml/mpt-3
+00005190: 3062 2d63 6861 7429 0a0a 3c2f 6465 7461  0b-chat)..</deta
+000051a0: 696c 733e 0a0a 3c64 6574 6169 6c73 3e0a  ils>..<details>.
+000051b0: 0a3c 7375 6d6d 6172 793e 4f50 543c 2f73  .<summary>OPT</s
+000051c0: 756d 6d61 7279 3e0a 0a0a 2323 2320 5175  ummary>...### Qu
+000051d0: 6963 6b73 7461 7274 0a0a 0a0a 3e20 2a2a  ickstart....> **
+000051e0: 4e6f 7465 3a2a 2a20 4f50 5420 7265 7175  Note:** OPT requ
+000051f0: 6972 6573 2074 6f20 696e 7374 616c 6c20  ires to install 
+00005200: 7769 7468 3a0a 3e20 6060 6062 6173 680a  with:.> ```bash.
+00005210: 3e20 7069 7020 696e 7374 616c 6c20 226f  > pip install "o
+00005220: 7065 6e6c 6c6d 5b6f 7074 5d22 0a3e 2060  penllm[opt]".> `
+00005230: 6060 0a0a 0a52 756e 2074 6865 2066 6f6c  ``...Run the fol
+00005240: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 2074  lowing command t
+00005250: 6f20 7175 6963 6b6c 7920 7370 696e 2075  o quickly spin u
+00005260: 7020 6120 4f50 5420 7365 7276 6572 3a0a  p a OPT server:.
+00005270: 0a60 6060 6261 7368 0a6f 7065 6e6c 6c6d  .```bash.openllm
+00005280: 2073 7461 7274 2066 6163 6562 6f6f 6b2f   start facebook/
+00005290: 6f70 742d 312e 3362 0a60 6060 0a49 6e20  opt-1.3b.```.In 
+000052a0: 6120 6469 6666 6572 656e 7420 7465 726d  a different term
+000052b0: 696e 616c 2c20 7275 6e20 7468 6520 666f  inal, run the fo
+000052c0: 6c6c 6f77 696e 6720 636f 6d6d 616e 6420  llowing command 
+000052d0: 746f 2069 6e74 6572 6163 7420 7769 7468  to interact with
+000052e0: 2074 6865 2073 6572 7665 723a 0a0a 6060   the server:..``
+000052f0: 6062 6173 680a 6578 706f 7274 204f 5045  `bash.export OPE
+00005300: 4e4c 4c4d 5f45 4e44 504f 494e 543d 6874  NLLM_ENDPOINT=ht
+00005310: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a33  tp://localhost:3
+00005320: 3030 300a 6f70 656e 6c6c 6d20 7175 6572  000.openllm quer
+00005330: 7920 2757 6861 7420 6172 6520 6c61 7267  y 'What are larg
+00005340: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
+00005350: 733f 270a 6060 600a 0a0a 3e20 2a2a 4e6f  s?'.```...> **No
+00005360: 7465 3a2a 2a20 416e 7920 4f50 5420 7661  te:** Any OPT va
+00005370: 7269 616e 7473 2063 616e 2062 6520 6465  riants can be de
+00005380: 706c 6f79 6564 2077 6974 6820 4f70 656e  ployed with Open
+00005390: 4c4c 4d2e 2056 6973 6974 2074 6865 205b  LLM. Visit the [
+000053a0: 4875 6767 696e 6746 6163 6520 4d6f 6465  HuggingFace Mode
+000053b0: 6c20 4875 625d 2868 7474 7073 3a2f 2f68  l Hub](https://h
+000053c0: 7567 6769 6e67 6661 6365 2e63 6f2f 6d6f  uggingface.co/mo
+000053d0: 6465 6c73 3f73 6f72 743d 7472 656e 6469  dels?sort=trendi
+000053e0: 6e67 2673 6561 7263 683d 6f70 7429 2074  ng&search=opt) t
+000053f0: 6f20 7365 6520 6d6f 7265 204f 5054 2d63  o see more OPT-c
+00005400: 6f6d 7061 7469 626c 6520 6d6f 6465 6c73  ompatible models
+00005410: 2e0a 0a0a 0a23 2323 2053 7570 706f 7274  .....### Support
+00005420: 6564 206d 6f64 656c 730a 0a59 6f75 2063  ed models..You c
+00005430: 616e 2073 7065 6369 6679 2061 6e79 206f  an specify any o
+00005440: 6620 7468 6520 666f 6c6c 6f77 696e 6720  f the following 
+00005450: 4f50 5420 6d6f 6465 6c73 2076 6961 2060  OPT models via `
+00005460: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
+00005470: 0a0a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ..- [facebook/op
+00005480: 742d 3132 356d 5d28 6874 7470 733a 2f2f  t-125m](https://
+00005490: 6875 6767 696e 6766 6163 652e 636f 2f66  huggingface.co/f
+000054a0: 6163 6562 6f6f 6b2f 6f70 742d 3132 356d  acebook/opt-125m
+000054b0: 290a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ).- [facebook/op
+000054c0: 742d 3335 306d 5d28 6874 7470 733a 2f2f  t-350m](https://
+000054d0: 6875 6767 696e 6766 6163 652e 636f 2f66  huggingface.co/f
+000054e0: 6163 6562 6f6f 6b2f 6f70 742d 3335 306d  acebook/opt-350m
+000054f0: 290a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ).- [facebook/op
+00005500: 742d 312e 3362 5d28 6874 7470 733a 2f2f  t-1.3b](https://
+00005510: 6875 6767 696e 6766 6163 652e 636f 2f66  huggingface.co/f
+00005520: 6163 6562 6f6f 6b2f 6f70 742d 312e 3362  acebook/opt-1.3b
+00005530: 290a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ).- [facebook/op
+00005540: 742d 322e 3762 5d28 6874 7470 733a 2f2f  t-2.7b](https://
+00005550: 6875 6767 696e 6766 6163 652e 636f 2f66  huggingface.co/f
+00005560: 6163 6562 6f6f 6b2f 6f70 742d 322e 3762  acebook/opt-2.7b
+00005570: 290a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ).- [facebook/op
+00005580: 742d 362e 3762 5d28 6874 7470 733a 2f2f  t-6.7b](https://
+00005590: 6875 6767 696e 6766 6163 652e 636f 2f66  huggingface.co/f
+000055a0: 6163 6562 6f6f 6b2f 6f70 742d 362e 3762  acebook/opt-6.7b
+000055b0: 290a 2d20 5b66 6163 6562 6f6f 6b2f 6f70  ).- [facebook/op
+000055c0: 742d 3636 625d 2868 7474 7073 3a2f 2f68  t-66b](https://h
+000055d0: 7567 6769 6e67 6661 6365 2e63 6f2f 6661  uggingface.co/fa
+000055e0: 6365 626f 6f6b 2f6f 7074 2d36 3662 290a  cebook/opt-66b).
+000055f0: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00005600: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
+00005610: 3e50 6869 3c2f 7375 6d6d 6172 793e 0a0a  >Phi</summary>..
+00005620: 0a23 2323 2051 7569 636b 7374 6172 740a  .### Quickstart.
+00005630: 0a0a 0a3e 202a 2a4e 6f74 653a 2a2a 2050  ...> **Note:** P
+00005640: 6869 2072 6571 7569 7265 7320 746f 2069  hi requires to i
+00005650: 6e73 7461 6c6c 2077 6974 683a 0a3e 2060  nstall with:.> `
+00005660: 6060 6261 7368 0a3e 2070 6970 2069 6e73  ``bash.> pip ins
+00005670: 7461 6c6c 2022 6f70 656e 6c6c 6d5b 7068  tall "openllm[ph
+00005680: 695d 220a 3e20 6060 600a 0a0a 5275 6e20  i]".> ```...Run 
+00005690: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+000056a0: 6d6d 616e 6420 746f 2071 7569 636b 6c79  mmand to quickly
+000056b0: 2073 7069 6e20 7570 2061 2050 6869 2073   spin up a Phi s
+000056c0: 6572 7665 723a 0a0a 6060 6062 6173 680a  erver:..```bash.
+000056d0: 5452 5553 545f 5245 4d4f 5445 5f43 4f44  TRUST_REMOTE_COD
+000056e0: 453d 5472 7565 206f 7065 6e6c 6c6d 2073  E=True openllm s
+000056f0: 7461 7274 206d 6963 726f 736f 6674 2f70  tart microsoft/p
+00005700: 6869 2d32 0a60 6060 0a49 6e20 6120 6469  hi-2.```.In a di
+00005710: 6666 6572 656e 7420 7465 726d 696e 616c  fferent terminal
+00005720: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+00005730: 696e 6720 636f 6d6d 616e 6420 746f 2069  ing command to i
+00005740: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00005750: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
+00005760: 680a 6578 706f 7274 204f 5045 4e4c 4c4d  h.export OPENLLM
+00005770: 5f45 4e44 504f 494e 543d 6874 7470 3a2f  _ENDPOINT=http:/
+00005780: 2f6c 6f63 616c 686f 7374 3a33 3030 300a  /localhost:3000.
+00005790: 6f70 656e 6c6c 6d20 7175 6572 7920 2757  openllm query 'W
+000057a0: 6861 7420 6172 6520 6c61 7267 6520 6c61  hat are large la
+000057b0: 6e67 7561 6765 206d 6f64 656c 733f 270a  nguage models?'.
+000057c0: 6060 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a  ```...> **Note:*
+000057d0: 2a20 416e 7920 5068 6920 7661 7269 616e  * Any Phi varian
+000057e0: 7473 2063 616e 2062 6520 6465 706c 6f79  ts can be deploy
+000057f0: 6564 2077 6974 6820 4f70 656e 4c4c 4d2e  ed with OpenLLM.
+00005800: 2056 6973 6974 2074 6865 205b 4875 6767   Visit the [Hugg
+00005810: 696e 6746 6163 6520 4d6f 6465 6c20 4875  ingFace Model Hu
+00005820: 625d 2868 7474 7073 3a2f 2f68 7567 6769  b](https://huggi
+00005830: 6e67 6661 6365 2e63 6f2f 6d6f 6465 6c73  ngface.co/models
+00005840: 3f73 6f72 743d 7472 656e 6469 6e67 2673  ?sort=trending&s
+00005850: 6561 7263 683d 7068 6929 2074 6f20 7365  earch=phi) to se
+00005860: 6520 6d6f 7265 2050 6869 2d63 6f6d 7061  e more Phi-compa
+00005870: 7469 626c 6520 6d6f 6465 6c73 2e0a 0a0a  tible models....
+00005880: 0a23 2323 2053 7570 706f 7274 6564 206d  .### Supported m
+00005890: 6f64 656c 730a 0a59 6f75 2063 616e 2073  odels..You can s
+000058a0: 7065 6369 6679 2061 6e79 206f 6620 7468  pecify any of th
+000058b0: 6520 666f 6c6c 6f77 696e 6720 5068 6920  e following Phi 
+000058c0: 6d6f 6465 6c73 2076 6961 2060 6f70 656e  models via `open
+000058d0: 6c6c 6d20 7374 6172 7460 3a0a 0a0a 2d20  llm start`:...- 
+000058e0: 5b6d 6963 726f 736f 6674 2f70 6869 2d32  [microsoft/phi-2
+000058f0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00005900: 6766 6163 652e 636f 2f6d 6963 726f 736f  gface.co/microso
+00005910: 6674 2f70 6869 2d32 290a 2d20 5b6d 6963  ft/phi-2).- [mic
+00005920: 726f 736f 6674 2f70 6869 2d31 5f35 5d28  rosoft/phi-1_5](
+00005930: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00005940: 6163 652e 636f 2f6d 6963 726f 736f 6674  ace.co/microsoft
+00005950: 2f70 6869 2d31 5f35 290a 0a3c 2f64 6574  /phi-1_5)..</det
+00005960: 6169 6c73 3e0a 0a3c 6465 7461 696c 733e  ails>..<details>
+00005970: 0a0a 3c73 756d 6d61 7279 3e51 7765 6e3c  ..<summary>Qwen<
+00005980: 2f73 756d 6d61 7279 3e0a 0a0a 2323 2320  /summary>...### 
+00005990: 5175 6963 6b73 7461 7274 0a0a 0a0a 3e20  Quickstart....> 
+000059a0: 2a2a 4e6f 7465 3a2a 2a20 5177 656e 2072  **Note:** Qwen r
+000059b0: 6571 7569 7265 7320 746f 2069 6e73 7461  equires to insta
+000059c0: 6c6c 2077 6974 683a 0a3e 2060 6060 6261  ll with:.> ```ba
+000059d0: 7368 0a3e 2070 6970 2069 6e73 7461 6c6c  sh.> pip install
+000059e0: 2022 6f70 656e 6c6c 6d5b 7177 656e 5d22   "openllm[qwen]"
+000059f0: 0a3e 2060 6060 0a0a 0a52 756e 2074 6865  .> ```...Run the
+00005a00: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00005a10: 6e64 2074 6f20 7175 6963 6b6c 7920 7370  nd to quickly sp
+00005a20: 696e 2075 7020 6120 5177 656e 2073 6572  in up a Qwen ser
+00005a30: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
+00005a40: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
+00005a50: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
+00005a60: 7274 2071 7765 6e2f 5177 656e 2d37 422d  rt qwen/Qwen-7B-
+00005a70: 4368 6174 0a60 6060 0a49 6e20 6120 6469  Chat.```.In a di
+00005a80: 6666 6572 656e 7420 7465 726d 696e 616c  fferent terminal
+00005a90: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+00005aa0: 696e 6720 636f 6d6d 616e 6420 746f 2069  ing command to i
+00005ab0: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00005ac0: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
+00005ad0: 680a 6578 706f 7274 204f 5045 4e4c 4c4d  h.export OPENLLM
+00005ae0: 5f45 4e44 504f 494e 543d 6874 7470 3a2f  _ENDPOINT=http:/
+00005af0: 2f6c 6f63 616c 686f 7374 3a33 3030 300a  /localhost:3000.
+00005b00: 6f70 656e 6c6c 6d20 7175 6572 7920 2757  openllm query 'W
+00005b10: 6861 7420 6172 6520 6c61 7267 6520 6c61  hat are large la
+00005b20: 6e67 7561 6765 206d 6f64 656c 733f 270a  nguage models?'.
+00005b30: 6060 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a  ```...> **Note:*
+00005b40: 2a20 416e 7920 5177 656e 2076 6172 6961  * Any Qwen varia
+00005b50: 6e74 7320 6361 6e20 6265 2064 6570 6c6f  nts can be deplo
+00005b60: 7965 6420 7769 7468 204f 7065 6e4c 4c4d  yed with OpenLLM
+00005b70: 2e20 5669 7369 7420 7468 6520 5b48 7567  . Visit the [Hug
+00005b80: 6769 6e67 4661 6365 204d 6f64 656c 2048  gingFace Model H
+00005b90: 7562 5d28 6874 7470 733a 2f2f 6875 6767  ub](https://hugg
+00005ba0: 696e 6766 6163 652e 636f 2f6d 6f64 656c  ingface.co/model
+00005bb0: 733f 736f 7274 3d74 7265 6e64 696e 6726  s?sort=trending&
+00005bc0: 7365 6172 6368 3d71 7765 6e29 2074 6f20  search=qwen) to 
+00005bd0: 7365 6520 6d6f 7265 2051 7765 6e2d 636f  see more Qwen-co
+00005be0: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
+00005bf0: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
+00005c00: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
+00005c10: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
+00005c20: 2074 6865 2066 6f6c 6c6f 7769 6e67 2051   the following Q
+00005c30: 7765 6e20 6d6f 6465 6c73 2076 6961 2060  wen models via `
+00005c40: 6f70 656e 6c6c 6d20 7374 6172 7460 3a0a  openllm start`:.
+00005c50: 0a0a 2d20 5b71 7765 6e2f 5177 656e 2d37  ..- [qwen/Qwen-7
+00005c60: 422d 4368 6174 5d28 6874 7470 733a 2f2f  B-Chat](https://
+00005c70: 6875 6767 696e 6766 6163 652e 636f 2f71  huggingface.co/q
+00005c80: 7765 6e2f 5177 656e 2d37 422d 4368 6174  wen/Qwen-7B-Chat
+00005c90: 290a 2d20 5b71 7765 6e2f 5177 656e 2d37  ).- [qwen/Qwen-7
+00005ca0: 422d 4368 6174 2d49 6e74 385d 2868 7474  B-Chat-Int8](htt
+00005cb0: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00005cc0: 2e63 6f2f 7177 656e 2f51 7765 6e2d 3742  .co/qwen/Qwen-7B
+00005cd0: 2d43 6861 742d 496e 7438 290a 2d20 5b71  -Chat-Int8).- [q
+00005ce0: 7765 6e2f 5177 656e 2d37 422d 4368 6174  wen/Qwen-7B-Chat
+00005cf0: 2d49 6e74 345d 2868 7474 7073 3a2f 2f68  -Int4](https://h
+00005d00: 7567 6769 6e67 6661 6365 2e63 6f2f 7177  uggingface.co/qw
+00005d10: 656e 2f51 7765 6e2d 3742 2d43 6861 742d  en/Qwen-7B-Chat-
+00005d20: 496e 7434 290a 2d20 5b71 7765 6e2f 5177  Int4).- [qwen/Qw
+00005d30: 656e 2d31 3442 2d43 6861 745d 2868 7474  en-14B-Chat](htt
+00005d40: 7073 3a2f 2f68 7567 6769 6e67 6661 6365  ps://huggingface
+00005d50: 2e63 6f2f 7177 656e 2f51 7765 6e2d 3134  .co/qwen/Qwen-14
+00005d60: 422d 4368 6174 290a 2d20 5b71 7765 6e2f  B-Chat).- [qwen/
+00005d70: 5177 656e 2d31 3442 2d43 6861 742d 496e  Qwen-14B-Chat-In
+00005d80: 7438 5d28 6874 7470 733a 2f2f 6875 6767  t8](https://hugg
+00005d90: 696e 6766 6163 652e 636f 2f71 7765 6e2f  ingface.co/qwen/
+00005da0: 5177 656e 2d31 3442 2d43 6861 742d 496e  Qwen-14B-Chat-In
+00005db0: 7438 290a 2d20 5b71 7765 6e2f 5177 656e  t8).- [qwen/Qwen
+00005dc0: 2d31 3442 2d43 6861 742d 496e 7434 5d28  -14B-Chat-Int4](
+00005dd0: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00005de0: 6163 652e 636f 2f71 7765 6e2f 5177 656e  ace.co/qwen/Qwen
+00005df0: 2d31 3442 2d43 6861 742d 496e 7434 290a  -14B-Chat-Int4).
+00005e00: 0a3c 2f64 6574 6169 6c73 3e0a 0a3c 6465  .</details>..<de
+00005e10: 7461 696c 733e 0a0a 3c73 756d 6d61 7279  tails>..<summary
+00005e20: 3e53 7461 626c 654c 4d3c 2f73 756d 6d61  >StableLM</summa
+00005e30: 7279 3e0a 0a0a 2323 2320 5175 6963 6b73  ry>...### Quicks
+00005e40: 7461 7274 0a0a 0a0a 3e20 2a2a 4e6f 7465  tart....> **Note
+00005e50: 3a2a 2a20 5374 6162 6c65 4c4d 2072 6571  :** StableLM req
+00005e60: 7569 7265 7320 746f 2069 6e73 7461 6c6c  uires to install
+00005e70: 2077 6974 683a 0a3e 2060 6060 6261 7368   with:.> ```bash
+00005e80: 0a3e 2070 6970 2069 6e73 7461 6c6c 2022  .> pip install "
+00005e90: 6f70 656e 6c6c 6d5b 7374 6162 6c65 6c6d  openllm[stablelm
+00005ea0: 5d22 0a3e 2060 6060 0a0a 0a52 756e 2074  ]".> ```...Run t
+00005eb0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00005ec0: 6d61 6e64 2074 6f20 7175 6963 6b6c 7920  mand to quickly 
+00005ed0: 7370 696e 2075 7020 6120 5374 6162 6c65  spin up a Stable
+00005ee0: 4c4d 2073 6572 7665 723a 0a0a 6060 6062  LM server:..```b
+00005ef0: 6173 680a 5452 5553 545f 5245 4d4f 5445  ash.TRUST_REMOTE
+00005f00: 5f43 4f44 453d 5472 7565 206f 7065 6e6c  _CODE=True openl
+00005f10: 6c6d 2073 7461 7274 2073 7461 6269 6c69  lm start stabili
+00005f20: 7479 6169 2f73 7461 626c 656c 6d2d 7475  tyai/stablelm-tu
+00005f30: 6e65 642d 616c 7068 612d 3362 0a60 6060  ned-alpha-3b.```
+00005f40: 0a49 6e20 6120 6469 6666 6572 656e 7420  .In a different 
+00005f50: 7465 726d 696e 616c 2c20 7275 6e20 7468  terminal, run th
+00005f60: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00005f70: 616e 6420 746f 2069 6e74 6572 6163 7420  and to interact 
+00005f80: 7769 7468 2074 6865 2073 6572 7665 723a  with the server:
+00005f90: 0a0a 6060 6062 6173 680a 6578 706f 7274  ..```bash.export
+00005fa0: 204f 5045 4e4c 4c4d 5f45 4e44 504f 494e   OPENLLM_ENDPOIN
+00005fb0: 543d 6874 7470 3a2f 2f6c 6f63 616c 686f  T=http://localho
+00005fc0: 7374 3a33 3030 300a 6f70 656e 6c6c 6d20  st:3000.openllm 
+00005fd0: 7175 6572 7920 2757 6861 7420 6172 6520  query 'What are 
+00005fe0: 6c61 7267 6520 6c61 6e67 7561 6765 206d  large language m
+00005ff0: 6f64 656c 733f 270a 6060 600a 0a0a 3e20  odels?'.```...> 
+00006000: 2a2a 4e6f 7465 3a2a 2a20 416e 7920 5374  **Note:** Any St
+00006010: 6162 6c65 4c4d 2076 6172 6961 6e74 7320  ableLM variants 
+00006020: 6361 6e20 6265 2064 6570 6c6f 7965 6420  can be deployed 
+00006030: 7769 7468 204f 7065 6e4c 4c4d 2e20 5669  with OpenLLM. Vi
+00006040: 7369 7420 7468 6520 5b48 7567 6769 6e67  sit the [Hugging
+00006050: 4661 6365 204d 6f64 656c 2048 7562 5d28  Face Model Hub](
+00006060: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00006070: 6163 652e 636f 2f6d 6f64 656c 733f 736f  ace.co/models?so
+00006080: 7274 3d74 7265 6e64 696e 6726 7365 6172  rt=trending&sear
+00006090: 6368 3d73 7461 626c 656c 6d29 2074 6f20  ch=stablelm) to 
+000060a0: 7365 6520 6d6f 7265 2053 7461 626c 654c  see more StableL
+000060b0: 4d2d 636f 6d70 6174 6962 6c65 206d 6f64  M-compatible mod
+000060c0: 656c 732e 0a0a 0a0a 2323 2320 5375 7070  els.....### Supp
+000060d0: 6f72 7465 6420 6d6f 6465 6c73 0a0a 596f  orted models..Yo
+000060e0: 7520 6361 6e20 7370 6563 6966 7920 616e  u can specify an
+000060f0: 7920 6f66 2074 6865 2066 6f6c 6c6f 7769  y of the followi
+00006100: 6e67 2053 7461 626c 654c 4d20 6d6f 6465  ng StableLM mode
+00006110: 6c73 2076 6961 2060 6f70 656e 6c6c 6d20  ls via `openllm 
+00006120: 7374 6172 7460 3a0a 0a0a 2d20 5b73 7461  start`:...- [sta
+00006130: 6269 6c69 7479 6169 2f73 7461 626c 656c  bilityai/stablel
+00006140: 6d2d 7475 6e65 642d 616c 7068 612d 3362  m-tuned-alpha-3b
+00006150: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00006160: 6766 6163 652e 636f 2f73 7461 6269 6c69  gface.co/stabili
+00006170: 7479 6169 2f73 7461 626c 656c 6d2d 7475  tyai/stablelm-tu
+00006180: 6e65 642d 616c 7068 612d 3362 290a 2d20  ned-alpha-3b).- 
+00006190: 5b73 7461 6269 6c69 7479 6169 2f73 7461  [stabilityai/sta
+000061a0: 626c 656c 6d2d 7475 6e65 642d 616c 7068  blelm-tuned-alph
+000061b0: 612d 3762 5d28 6874 7470 733a 2f2f 6875  a-7b](https://hu
+000061c0: 6767 696e 6766 6163 652e 636f 2f73 7461  ggingface.co/sta
+000061d0: 6269 6c69 7479 6169 2f73 7461 626c 656c  bilityai/stablel
+000061e0: 6d2d 7475 6e65 642d 616c 7068 612d 3762  m-tuned-alpha-7b
+000061f0: 290a 2d20 5b73 7461 6269 6c69 7479 6169  ).- [stabilityai
+00006200: 2f73 7461 626c 656c 6d2d 6261 7365 2d61  /stablelm-base-a
+00006210: 6c70 6861 2d33 625d 2868 7474 7073 3a2f  lpha-3b](https:/
+00006220: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00006230: 7374 6162 696c 6974 7961 692f 7374 6162  stabilityai/stab
+00006240: 6c65 6c6d 2d62 6173 652d 616c 7068 612d  lelm-base-alpha-
+00006250: 3362 290a 2d20 5b73 7461 6269 6c69 7479  3b).- [stability
+00006260: 6169 2f73 7461 626c 656c 6d2d 6261 7365  ai/stablelm-base
+00006270: 2d61 6c70 6861 2d37 625d 2868 7474 7073  -alpha-7b](https
+00006280: 3a2f 2f68 7567 6769 6e67 6661 6365 2e63  ://huggingface.c
+00006290: 6f2f 7374 6162 696c 6974 7961 692f 7374  o/stabilityai/st
+000062a0: 6162 6c65 6c6d 2d62 6173 652d 616c 7068  ablelm-base-alph
+000062b0: 612d 3762 290a 0a3c 2f64 6574 6169 6c73  a-7b)..</details
+000062c0: 3e0a 0a3c 6465 7461 696c 733e 0a0a 3c73  >..<details>..<s
+000062d0: 756d 6d61 7279 3e53 7461 7243 6f64 6572  ummary>StarCoder
+000062e0: 3c2f 7375 6d6d 6172 793e 0a0a 0a23 2323  </summary>...###
+000062f0: 2051 7569 636b 7374 6172 740a 0a0a 0a3e   Quickstart....>
+00006300: 202a 2a4e 6f74 653a 2a2a 2053 7461 7243   **Note:** StarC
+00006310: 6f64 6572 2072 6571 7569 7265 7320 746f  oder requires to
+00006320: 2069 6e73 7461 6c6c 2077 6974 683a 0a3e   install with:.>
+00006330: 2060 6060 6261 7368 0a3e 2070 6970 2069   ```bash.> pip i
+00006340: 6e73 7461 6c6c 2022 6f70 656e 6c6c 6d5b  nstall "openllm[
+00006350: 7374 6172 636f 6465 725d 220a 3e20 6060  starcoder]".> ``
+00006360: 600a 0a0a 5275 6e20 7468 6520 666f 6c6c  `...Run the foll
+00006370: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
+00006380: 2071 7569 636b 6c79 2073 7069 6e20 7570   quickly spin up
+00006390: 2061 2053 7461 7243 6f64 6572 2073 6572   a StarCoder ser
+000063a0: 7665 723a 0a0a 6060 6062 6173 680a 5452  ver:..```bash.TR
+000063b0: 5553 545f 5245 4d4f 5445 5f43 4f44 453d  UST_REMOTE_CODE=
+000063c0: 5472 7565 206f 7065 6e6c 6c6d 2073 7461  True openllm sta
+000063d0: 7274 2062 6967 636f 6465 2f73 7461 7263  rt bigcode/starc
+000063e0: 6f64 6572 0a60 6060 0a49 6e20 6120 6469  oder.```.In a di
+000063f0: 6666 6572 656e 7420 7465 726d 696e 616c  fferent terminal
+00006400: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+00006410: 696e 6720 636f 6d6d 616e 6420 746f 2069  ing command to i
+00006420: 6e74 6572 6163 7420 7769 7468 2074 6865  nteract with the
+00006430: 2073 6572 7665 723a 0a0a 6060 6062 6173   server:..```bas
+00006440: 680a 6578 706f 7274 204f 5045 4e4c 4c4d  h.export OPENLLM
+00006450: 5f45 4e44 504f 494e 543d 6874 7470 3a2f  _ENDPOINT=http:/
+00006460: 2f6c 6f63 616c 686f 7374 3a33 3030 300a  /localhost:3000.
+00006470: 6f70 656e 6c6c 6d20 7175 6572 7920 2757  openllm query 'W
+00006480: 6861 7420 6172 6520 6c61 7267 6520 6c61  hat are large la
+00006490: 6e67 7561 6765 206d 6f64 656c 733f 270a  nguage models?'.
+000064a0: 6060 600a 0a0a 3e20 2a2a 4e6f 7465 3a2a  ```...> **Note:*
+000064b0: 2a20 416e 7920 5374 6172 436f 6465 7220  * Any StarCoder 
+000064c0: 7661 7269 616e 7473 2063 616e 2062 6520  variants can be 
+000064d0: 6465 706c 6f79 6564 2077 6974 6820 4f70  deployed with Op
+000064e0: 656e 4c4c 4d2e 2056 6973 6974 2074 6865  enLLM. Visit the
+000064f0: 205b 4875 6767 696e 6746 6163 6520 4d6f   [HuggingFace Mo
+00006500: 6465 6c20 4875 625d 2868 7474 7073 3a2f  del Hub](https:/
+00006510: 2f68 7567 6769 6e67 6661 6365 2e63 6f2f  /huggingface.co/
+00006520: 6d6f 6465 6c73 3f73 6f72 743d 7472 656e  models?sort=tren
+00006530: 6469 6e67 2673 6561 7263 683d 7374 6172  ding&search=star
+00006540: 636f 6465 7229 2074 6f20 7365 6520 6d6f  coder) to see mo
+00006550: 7265 2053 7461 7243 6f64 6572 2d63 6f6d  re StarCoder-com
+00006560: 7061 7469 626c 6520 6d6f 6465 6c73 2e0a  patible models..
+00006570: 0a0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
+00006580: 206d 6f64 656c 730a 0a59 6f75 2063 616e   models..You can
+00006590: 2073 7065 6369 6679 2061 6e79 206f 6620   specify any of 
+000065a0: 7468 6520 666f 6c6c 6f77 696e 6720 5374  the following St
+000065b0: 6172 436f 6465 7220 6d6f 6465 6c73 2076  arCoder models v
+000065c0: 6961 2060 6f70 656e 6c6c 6d20 7374 6172  ia `openllm star
+000065d0: 7460 3a0a 0a0a 2d20 5b62 6967 636f 6465  t`:...- [bigcode
+000065e0: 2f73 7461 7263 6f64 6572 5d28 6874 7470  /starcoder](http
+000065f0: 733a 2f2f 6875 6767 696e 6766 6163 652e  s://huggingface.
+00006600: 636f 2f62 6967 636f 6465 2f73 7461 7263  co/bigcode/starc
+00006610: 6f64 6572 290a 2d20 5b62 6967 636f 6465  oder).- [bigcode
+00006620: 2f73 7461 7263 6f64 6572 6261 7365 5d28  /starcoderbase](
+00006630: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00006640: 6163 652e 636f 2f62 6967 636f 6465 2f73  ace.co/bigcode/s
+00006650: 7461 7263 6f64 6572 6261 7365 290a 0a3c  tarcoderbase)..<
+00006660: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+00006670: 696c 733e 0a0a 3c73 756d 6d61 7279 3e59  ils>..<summary>Y
+00006680: 693c 2f73 756d 6d61 7279 3e0a 0a0a 2323  i</summary>...##
+00006690: 2320 5175 6963 6b73 7461 7274 0a0a 0a0a  # Quickstart....
+000066a0: 3e20 2a2a 4e6f 7465 3a2a 2a20 5969 2072  > **Note:** Yi r
+000066b0: 6571 7569 7265 7320 746f 2069 6e73 7461  equires to insta
+000066c0: 6c6c 2077 6974 683a 0a3e 2060 6060 6261  ll with:.> ```ba
+000066d0: 7368 0a3e 2070 6970 2069 6e73 7461 6c6c  sh.> pip install
+000066e0: 2022 6f70 656e 6c6c 6d5b 7969 5d22 0a3e   "openllm[yi]".>
+000066f0: 2060 6060 0a0a 0a52 756e 2074 6865 2066   ```...Run the f
+00006700: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
+00006710: 2074 6f20 7175 6963 6b6c 7920 7370 696e   to quickly spin
+00006720: 2075 7020 6120 5969 2073 6572 7665 723a   up a Yi server:
+00006730: 0a0a 6060 6062 6173 680a 5452 5553 545f  ..```bash.TRUST_
+00006740: 5245 4d4f 5445 5f43 4f44 453d 5472 7565  REMOTE_CODE=True
+00006750: 206f 7065 6e6c 6c6d 2073 7461 7274 2030   openllm start 0
+00006760: 312d 6169 2f59 692d 3642 0a60 6060 0a49  1-ai/Yi-6B.```.I
+00006770: 6e20 6120 6469 6666 6572 656e 7420 7465  n a different te
+00006780: 726d 696e 616c 2c20 7275 6e20 7468 6520  rminal, run the 
+00006790: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+000067a0: 6420 746f 2069 6e74 6572 6163 7420 7769  d to interact wi
+000067b0: 7468 2074 6865 2073 6572 7665 723a 0a0a  th the server:..
+000067c0: 6060 6062 6173 680a 6578 706f 7274 204f  ```bash.export O
+000067d0: 5045 4e4c 4c4d 5f45 4e44 504f 494e 543d  PENLLM_ENDPOINT=
+000067e0: 6874 7470 3a2f 2f6c 6f63 616c 686f 7374  http://localhost
+000067f0: 3a33 3030 300a 6f70 656e 6c6c 6d20 7175  :3000.openllm qu
+00006800: 6572 7920 2757 6861 7420 6172 6520 6c61  ery 'What are la
+00006810: 7267 6520 6c61 6e67 7561 6765 206d 6f64  rge language mod
+00006820: 656c 733f 270a 6060 600a 0a0a 3e20 2a2a  els?'.```...> **
+00006830: 4e6f 7465 3a2a 2a20 416e 7920 5969 2076  Note:** Any Yi v
+00006840: 6172 6961 6e74 7320 6361 6e20 6265 2064  ariants can be d
+00006850: 6570 6c6f 7965 6420 7769 7468 204f 7065  eployed with Ope
+00006860: 6e4c 4c4d 2e20 5669 7369 7420 7468 6520  nLLM. Visit the 
+00006870: 5b48 7567 6769 6e67 4661 6365 204d 6f64  [HuggingFace Mod
+00006880: 656c 2048 7562 5d28 6874 7470 733a 2f2f  el Hub](https://
+00006890: 6875 6767 696e 6766 6163 652e 636f 2f6d  huggingface.co/m
+000068a0: 6f64 656c 733f 736f 7274 3d74 7265 6e64  odels?sort=trend
+000068b0: 696e 6726 7365 6172 6368 3d79 6929 2074  ing&search=yi) t
+000068c0: 6f20 7365 6520 6d6f 7265 2059 692d 636f  o see more Yi-co
+000068d0: 6d70 6174 6962 6c65 206d 6f64 656c 732e  mpatible models.
+000068e0: 0a0a 0a0a 2323 2320 5375 7070 6f72 7465  ....### Supporte
+000068f0: 6420 6d6f 6465 6c73 0a0a 596f 7520 6361  d models..You ca
+00006900: 6e20 7370 6563 6966 7920 616e 7920 6f66  n specify any of
+00006910: 2074 6865 2066 6f6c 6c6f 7769 6e67 2059   the following Y
+00006920: 6920 6d6f 6465 6c73 2076 6961 2060 6f70  i models via `op
+00006930: 656e 6c6c 6d20 7374 6172 7460 3a0a 0a0a  enllm start`:...
+00006940: 2d20 5b30 312d 6169 2f59 692d 3642 5d28  - [01-ai/Yi-6B](
+00006950: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00006960: 6163 652e 636f 2f30 312d 6169 2f59 692d  ace.co/01-ai/Yi-
+00006970: 3642 290a 2d20 5b30 312d 6169 2f59 692d  6B).- [01-ai/Yi-
+00006980: 3334 425d 2868 7474 7073 3a2f 2f68 7567  34B](https://hug
+00006990: 6769 6e67 6661 6365 2e63 6f2f 3031 2d61  gingface.co/01-a
+000069a0: 692f 5969 2d33 3442 290a 2d20 5b30 312d  i/Yi-34B).- [01-
+000069b0: 6169 2f59 692d 3642 2d32 3030 4b5d 2868  ai/Yi-6B-200K](h
+000069c0: 7474 7073 3a2f 2f68 7567 6769 6e67 6661  ttps://huggingfa
+000069d0: 6365 2e63 6f2f 3031 2d61 692f 5969 2d36  ce.co/01-ai/Yi-6
+000069e0: 422d 3230 304b 290a 2d20 5b30 312d 6169  B-200K).- [01-ai
+000069f0: 2f59 692d 3334 422d 3230 304b 5d28 6874  /Yi-34B-200K](ht
+00006a00: 7470 733a 2f2f 6875 6767 696e 6766 6163  tps://huggingfac
+00006a10: 652e 636f 2f30 312d 6169 2f59 692d 3334  e.co/01-ai/Yi-34
+00006a20: 422d 3230 304b 290a 0a3c 2f64 6574 6169  B-200K)..</detai
+00006a30: 6c73 3e0a 0a3c 212d 2d20 7570 6461 7465  ls>..<!-- update
+00006a40: 2d72 6561 646d 652e 7079 3a20 7374 6f70  -readme.py: stop
+00006a50: 202d 2d3e 0a0a 4d6f 7265 206d 6f64 656c   -->..More model
+00006a60: 7320 7769 6c6c 2062 6520 696e 7465 6772  s will be integr
+00006a70: 6174 6564 2077 6974 6820 4f70 656e 4c4c  ated with OpenLL
+00006a80: 4d20 616e 6420 7765 2077 656c 636f 6d65  M and we welcome
+00006a90: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
+00006aa0: 6f6e 7320 6966 2079 6f75 2077 616e 7420  ons if you want 
+00006ab0: 746f 2069 6e63 6f72 706f 7261 7465 2079  to incorporate y
+00006ac0: 6f75 7220 6375 7374 6f6d 204c 4c4d 7320  our custom LLMs 
+00006ad0: 696e 746f 2074 6865 2065 636f 7379 7374  into the ecosyst
+00006ae0: 656d 2e20 4368 6563 6b20 6f75 7420 5b41  em. Check out [A
+00006af0: 6464 696e 6720 6120 4e65 7720 4d6f 6465  dding a New Mode
+00006b00: 6c20 4775 6964 655d 2868 7474 7073 3a2f  l Guide](https:/
+00006b10: 2f67 6974 6875 622e 636f 6d2f 6265 6e74  /github.com/bent
+00006b20: 6f6d 6c2f 4f70 656e 4c4c 4d2f 626c 6f62  oml/OpenLLM/blob
+00006b30: 2f6d 6169 6e2f 4144 4449 4e47 5f4e 4557  /main/ADDING_NEW
+00006b40: 5f4d 4f44 454c 2e6d 6429 2074 6f20 6c65  _MODEL.md) to le
+00006b50: 6172 6e20 6d6f 7265 2e0a 0a23 2320 f09f  arn more...## ..
+00006b60: 92bb 2052 756e 2079 6f75 7220 6d6f 6465  .. Run your mode
+00006b70: 6c20 6f6e 206d 756c 7469 706c 6520 4750  l on multiple GP
+00006b80: 5573 0a0a 4f70 656e 4c4c 4d20 616c 6c6f  Us..OpenLLM allo
+00006b90: 7773 2079 6f75 2074 6f20 7374 6172 7420  ws you to start 
+00006ba0: 796f 7572 206d 6f64 656c 2073 6572 7665  your model serve
+00006bb0: 7220 6f6e 206d 756c 7469 706c 6520 4750  r on multiple GP
+00006bc0: 5573 2061 6e64 2073 7065 6369 6679 2074  Us and specify t
+00006bd0: 6865 206e 756d 6265 7220 6f66 2077 6f72  he number of wor
+00006be0: 6b65 7273 2070 6572 2072 6573 6f75 7263  kers per resourc
+00006bf0: 6520 6173 7369 676e 6564 2075 7369 6e67  e assigned using
+00006c00: 2074 6865 2060 2d2d 776f 726b 6572 732d   the `--workers-
+00006c10: 7065 722d 7265 736f 7572 6365 6020 6f70  per-resource` op
+00006c20: 7469 6f6e 2e20 466f 7220 6578 616d 706c  tion. For exampl
+00006c30: 652c 2069 6620 796f 7520 6861 7665 2034  e, if you have 4
+00006c40: 2061 7661 696c 6162 6c65 2047 5055 732c   available GPUs,
+00006c50: 2079 6f75 2073 6574 2074 6865 2076 616c   you set the val
+00006c60: 7565 2061 7320 6f6e 6520 6469 7669 6465  ue as one divide
+00006c70: 6420 6279 2074 6865 206e 756d 6265 7220  d by the number 
+00006c80: 6173 206f 6e6c 7920 6f6e 6520 696e 7374  as only one inst
+00006c90: 616e 6365 206f 6620 7468 6520 5275 6e6e  ance of the Runn
+00006ca0: 6572 2073 6572 7665 7220 7769 6c6c 2062  er server will b
+00006cb0: 6520 7370 6177 6e65 642e 0a0a 6060 6062  e spawned...```b
+00006cc0: 6173 680a 5452 5553 545f 5245 4d4f 5445  ash.TRUST_REMOTE
+00006cd0: 5f43 4f44 453d 5472 7565 206f 7065 6e6c  _CODE=True openl
+00006ce0: 6c6d 2073 7461 7274 206d 6963 726f 736f  lm start microso
+00006cf0: 6674 2f70 6869 2d32 202d 2d77 6f72 6b65  ft/phi-2 --worke
+00006d00: 7273 2d70 6572 2d72 6573 6f75 7263 6520  rs-per-resource 
+00006d10: 302e 3235 0a60 6060 0a0a 3e20 5b21 4e4f  0.25.```..> [!NO
+00006d20: 5445 5d0a 3e20 5468 6520 616d 6f75 6e74  TE].> The amount
+00006d30: 206f 6620 4750 5573 2072 6571 7569 7265   of GPUs require
+00006d40: 6420 6465 7065 6e64 7320 6f6e 2074 6865  d depends on the
+00006d50: 206d 6f64 656c 2073 697a 6520 6974 7365   model size itse
+00006d60: 6c66 2e0a 3e20 596f 7520 6361 6e20 7573  lf..> You can us
+00006d70: 6520 5b74 6865 204d 6f64 656c 204d 656d  e [the Model Mem
+00006d80: 6f72 7920 4361 6c63 756c 6174 6f72 2066  ory Calculator f
+00006d90: 726f 6d20 4875 6767 696e 6720 4661 6365  rom Hugging Face
+00006da0: 5d28 6874 7470 733a 2f2f 6875 6767 696e  ](https://huggin
+00006db0: 6766 6163 652e 636f 2f73 7061 6365 732f  gface.co/spaces/
+00006dc0: 6866 2d61 6363 656c 6572 6174 652f 6d6f  hf-accelerate/mo
+00006dd0: 6465 6c2d 6d65 6d6f 7279 2d75 7361 6765  del-memory-usage
+00006de0: 2920 746f 0a3e 2063 616c 6375 6c61 7465  ) to.> calculate
+00006df0: 2068 6f77 206d 7563 6820 7652 414d 2069   how much vRAM i
+00006e00: 7320 6e65 6564 6564 2074 6f20 7472 6169  s needed to trai
+00006e10: 6e20 616e 6420 7065 7266 6f72 6d20 6269  n and perform bi
+00006e20: 6720 6d6f 6465 6c0a 3e20 696e 6665 7265  g model.> infere
+00006e30: 6e63 6520 6f6e 2061 206d 6f64 656c 2061  nce on a model a
+00006e40: 6e64 2074 6865 6e20 706c 616e 2079 6f75  nd then plan you
+00006e50: 7220 4750 5520 7374 7261 7465 6779 2062  r GPU strategy b
+00006e60: 6173 6564 206f 6e20 6974 2e0a 0a57 6865  ased on it...Whe
+00006e70: 6e20 7573 696e 6720 7468 6520 602d 2d77  n using the `--w
+00006e80: 6f72 6b65 7273 2d70 6572 2d72 6573 6f75  orkers-per-resou
+00006e90: 7263 6560 206f 7074 696f 6e20 7769 7468  rce` option with
+00006ea0: 2074 6865 2060 6f70 656e 6c6c 6d20 6275   the `openllm bu
+00006eb0: 696c 6460 2063 6f6d 6d61 6e64 2c20 7468  ild` command, th
+00006ec0: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
+00006ed0: 7269 6162 6c65 2069 7320 7361 7665 6420  riable is saved 
+00006ee0: 696e 746f 2074 6865 2072 6573 756c 7469  into the resulti
+00006ef0: 6e67 2042 656e 746f 2e0a 0a46 6f72 206d  ng Bento...For m
+00006f00: 6f72 6520 696e 666f 726d 6174 696f 6e2c  ore information,
+00006f10: 2073 6565 205b 5265 736f 7572 6365 2073   see [Resource s
+00006f20: 6368 6564 756c 696e 6720 7374 7261 7465  cheduling strate
+00006f30: 6779 5d28 6874 7470 733a 2f2f 646f 6373  gy](https://docs
+00006f40: 2e62 656e 746f 6d6c 2e6f 7267 2f65 6e2f  .bentoml.org/en/
+00006f50: 6c61 7465 7374 2f67 7569 6465 732f 7363  latest/guides/sc
+00006f60: 6865 6475 6c69 6e67 2e68 746d 6c23 292e  heduling.html#).
+00006f70: 0a0a 2323 20f0 9f9b 9e20 5275 6e74 696d  ..## .... Runtim
+00006f80: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+00006f90: 730a 0a44 6966 6665 7265 6e74 204c 4c4d  s..Different LLM
+00006fa0: 7320 6d61 7920 7375 7070 6f72 7420 6d75  s may support mu
+00006fb0: 6c74 6970 6c65 2072 756e 7469 6d65 2069  ltiple runtime i
+00006fc0: 6d70 6c65 6d65 6e74 6174 696f 6e73 2e20  mplementations. 
+00006fd0: 4d6f 6465 6c73 2074 6861 7420 6861 7665  Models that have
+00006fe0: 2060 764c 4c4d 6020 2860 766c 6c6d 6029   `vLLM` (`vllm`)
+00006ff0: 2073 7570 706f 7274 7320 7769 6c6c 2075   supports will u
+00007000: 7365 2076 4c4c 4d20 6279 2064 6566 6175  se vLLM by defau
+00007010: 6c74 2c20 6f74 6865 7277 6973 6520 6974  lt, otherwise it
+00007020: 2066 616c 6c62 6163 6b20 746f 2075 7365   fallback to use
+00007030: 2060 5079 546f 7263 6860 2028 6070 7460   `PyTorch` (`pt`
+00007040: 292e 0a0a 546f 2073 7065 6369 6679 2061  )...To specify a
+00007050: 2073 7065 6369 6669 6320 7275 6e74 696d   specific runtim
+00007060: 6520 666f 7220 796f 7572 2063 686f 7365  e for your chose
+00007070: 6e20 6d6f 6465 6c2c 2075 7365 2074 6865  n model, use the
+00007080: 2060 2d2d 6261 636b 656e 6460 206f 7074   `--backend` opt
+00007090: 696f 6e2e 2046 6f72 2065 7861 6d70 6c65  ion. For example
+000070a0: 3a0a 0a60 6060 6261 7368 0a6f 7065 6e6c  :..```bash.openl
+000070b0: 6c6d 2073 7461 7274 206d 6574 612d 6c6c  lm start meta-ll
+000070c0: 616d 612f 4c6c 616d 612d 322d 3762 2d63  ama/Llama-2-7b-c
+000070d0: 6861 742d 6866 202d 2d62 6163 6b65 6e64  hat-hf --backend
+000070e0: 2076 6c6c 6d0a 6060 600a 0a4e 6f74 653a   vllm.```..Note:
+000070f0: 0a0a 312e 2054 6f20 7573 6520 7468 6520  ..1. To use the 
+00007100: 764c 4c4d 2062 6163 6b65 6e64 2c20 796f  vLLM backend, yo
+00007110: 7520 6e65 6564 2061 2047 5055 2077 6974  u need a GPU wit
+00007120: 6820 6174 206c 6561 7374 2074 6865 2041  h at least the A
+00007130: 6d70 6572 6520 6172 6368 6974 6563 7475  mpere architectu
+00007140: 7265 206f 7220 6e65 7765 7220 616e 6420  re or newer and 
+00007150: 4355 4441 2076 6572 7369 6f6e 2031 312e  CUDA version 11.
+00007160: 382e 0a32 2e20 546f 2073 6565 2074 6865  8..2. To see the
+00007170: 2062 6163 6b65 6e64 206f 7074 696f 6e73   backend options
+00007180: 206f 6620 6561 6368 206d 6f64 656c 2073   of each model s
+00007190: 7570 706f 7274 6564 2062 7920 4f70 656e  upported by Open
+000071a0: 4c4c 4d2c 2073 6565 2074 6865 2053 7570  LLM, see the Sup
+000071b0: 706f 7274 6564 206d 6f64 656c 7320 7365  ported models se
+000071c0: 6374 696f 6e20 6f72 2072 756e 2060 6f70  ction or run `op
+000071d0: 656e 6c6c 6d20 6d6f 6465 6c73 602e 0a0a  enllm models`...
+000071e0: 2323 20f0 9f93 9020 5175 616e 7469 7a61  ## .... Quantiza
+000071f0: 7469 6f6e 0a0a 5175 616e 7469 7a61 7469  tion..Quantizati
+00007200: 6f6e 2069 7320 6120 7465 6368 6e69 7175  on is a techniqu
+00007210: 6520 746f 2072 6564 7563 6520 7468 6520  e to reduce the 
+00007220: 7374 6f72 6167 6520 616e 6420 636f 6d70  storage and comp
+00007230: 7574 6174 696f 6e20 7265 7175 6972 656d  utation requirem
+00007240: 656e 7473 2066 6f72 206d 6163 6869 6e65  ents for machine
+00007250: 206c 6561 726e 696e 6720 6d6f 6465 6c73   learning models
+00007260: 2c20 7061 7274 6963 756c 6172 6c79 2064  , particularly d
+00007270: 7572 696e 6720 696e 6665 7265 6e63 652e  uring inference.
+00007280: 2042 7920 6170 7072 6f78 696d 6174 696e   By approximatin
+00007290: 6720 666c 6f61 7469 6e67 2d70 6f69 6e74  g floating-point
+000072a0: 206e 756d 6265 7273 2061 7320 696e 7465   numbers as inte
+000072b0: 6765 7273 2028 7175 616e 7469 7a65 6420  gers (quantized 
+000072c0: 7661 6c75 6573 292c 2071 7561 6e74 697a  values), quantiz
+000072d0: 6174 696f 6e20 616c 6c6f 7773 2066 6f72  ation allows for
+000072e0: 2066 6173 7465 7220 636f 6d70 7574 6174   faster computat
+000072f0: 696f 6e73 2c20 7265 6475 6365 6420 6d65  ions, reduced me
+00007300: 6d6f 7279 2066 6f6f 7470 7269 6e74 2c20  mory footprint, 
+00007310: 616e 6420 6361 6e20 6d61 6b65 2069 7420  and can make it 
+00007320: 6665 6173 6962 6c65 2074 6f20 6465 706c  feasible to depl
+00007330: 6f79 206c 6172 6765 206d 6f64 656c 7320  oy large models 
+00007340: 6f6e 2072 6573 6f75 7263 652d 636f 6e73  on resource-cons
+00007350: 7472 6169 6e65 6420 6465 7669 6365 732e  trained devices.
+00007360: 0a0a 4f70 656e 4c4c 4d20 7375 7070 6f72  ..OpenLLM suppor
+00007370: 7473 2074 6865 2066 6f6c 6c6f 7769 6e67  ts the following
+00007380: 2071 7561 6e74 697a 6174 696f 6e20 7465   quantization te
+00007390: 6368 6e69 7175 6573 0a0a 2d20 5b4c 4c4d  chniques..- [LLM
+000073a0: 2e69 6e74 3828 293a 2038 2d62 6974 204d  .int8(): 8-bit M
+000073b0: 6174 7269 7820 4d75 6c74 6970 6c69 6361  atrix Multiplica
+000073c0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6172  tion](https://ar
+000073d0: 7869 762e 6f72 672f 6162 732f 3232 3038  xiv.org/abs/2208
+000073e0: 2e30 3733 3339 2920 7468 726f 7567 6820  .07339) through 
+000073f0: 5b62 6974 7361 6e64 6279 7465 735d 2868  [bitsandbytes](h
+00007400: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00007410: 6d2f 5469 6d44 6574 746d 6572 732f 6269  m/TimDettmers/bi
+00007420: 7473 616e 6462 7974 6573 290a 2d20 5b53  tsandbytes).- [S
+00007430: 7051 523a 2041 2053 7061 7273 652d 5175  pQR: A Sparse-Qu
+00007440: 616e 7469 7a65 6420 5265 7072 6573 656e  antized Represen
+00007450: 7461 7469 6f6e 2066 6f72 204e 6561 722d  tation for Near-
+00007460: 4c6f 7373 6c65 7373 204c 4c4d 2057 6569  Lossless LLM Wei
+00007470: 6768 7420 436f 6d70 7265 7373 696f 6e0a  ght Compression.
+00007480: 2020 5d28 6874 7470 733a 2f2f 6172 7869    ](https://arxi
+00007490: 762e 6f72 672f 6162 732f 3233 3036 2e30  v.org/abs/2306.0
+000074a0: 3330 3738 2920 7468 726f 7567 6820 5b62  3078) through [b
+000074b0: 6974 7361 6e64 6279 7465 735d 2868 7474  itsandbytes](htt
+000074c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000074d0: 5469 6d44 6574 746d 6572 732f 6269 7473  TimDettmers/bits
+000074e0: 616e 6462 7974 6573 290a 2d20 5b41 5751  andbytes).- [AWQ
+000074f0: 3a20 4163 7469 7661 7469 6f6e 2d61 7761  : Activation-awa
+00007500: 7265 2057 6569 6768 7420 5175 616e 7469  re Weight Quanti
+00007510: 7a61 7469 6f6e 5d28 6874 7470 733a 2f2f  zation](https://
+00007520: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
+00007530: 3036 2e30 3039 3738 292c 0a2d 205b 4750  06.00978),.- [GP
+00007540: 5451 3a20 4163 6375 7261 7465 2050 6f73  TQ: Accurate Pos
+00007550: 742d 5472 6169 6e69 6e67 2051 7561 6e74  t-Training Quant
+00007560: 697a 6174 696f 6e5d 2868 7474 7073 3a2f  ization](https:/
+00007570: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00007580: 3231 302e 3137 3332 3329 0a2d 205b 5371  210.17323).- [Sq
+00007590: 7565 657a 654c 4c4d 3a20 4465 6e73 652d  ueezeLLM: Dense-
+000075a0: 616e 642d 5370 6172 7365 2051 7561 6e74  and-Sparse Quant
+000075b0: 697a 6174 696f 6e5d 2868 7474 7073 3a2f  ization](https:/
+000075c0: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+000075d0: 3330 362e 3037 3632 3929 2e0a 0a23 2323  306.07629)...###
+000075e0: 2050 7954 6f72 6368 2062 6163 6b65 6e64   PyTorch backend
+000075f0: 0a0a 5769 7468 2050 7954 6f72 6368 2062  ..With PyTorch b
+00007600: 6163 6b65 6e64 2c20 4f70 656e 4c4c 4d20  ackend, OpenLLM 
+00007610: 7375 7070 6f72 7473 2060 696e 7438 602c  supports `int8`,
+00007620: 2060 696e 7434 602c 2061 6e64 2060 6770   `int4`, and `gp
+00007630: 7471 602e 0a0a 466f 7220 7573 696e 6720  tq`...For using 
+00007640: 696e 7438 2061 6e64 2069 6e74 3420 7175  int8 and int4 qu
+00007650: 616e 7469 7a61 7469 6f6e 2074 6872 6f75  antization throu
+00007660: 6768 2060 6269 7473 616e 6462 7974 6573  gh `bitsandbytes
+00007670: 602c 2079 6f75 2063 616e 2075 7365 2074  `, you can use t
+00007680: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6d  he following com
+00007690: 6d61 6e64 3a0a 0a60 6060 6261 7368 0a54  mand:..```bash.T
+000076a0: 5255 5354 5f52 454d 4f54 455f 434f 4445  RUST_REMOTE_CODE
+000076b0: 3d54 7275 6520 6f70 656e 6c6c 6d20 7374  =True openllm st
+000076c0: 6172 7420 6d69 6372 6f73 6f66 742f 7068  art microsoft/ph
+000076d0: 692d 3220 2d2d 7175 616e 7469 7a65 2069  i-2 --quantize i
+000076e0: 6e74 380a 6060 600a 0a54 6f20 7275 6e20  nt8.```..To run 
+000076f0: 696e 6665 7265 6e63 6520 7769 7468 c2a0  inference with..
+00007700: 6067 7074 7160 2c20 7369 6d70 6c79 2070  `gptq`, simply p
+00007710: 6173 73c2 a060 2d2d 7175 616e 7469 7a65  ass..`--quantize
+00007720: 2067 7074 7160 3a0a 0a60 6060 6261 7368   gptq`:..```bash
+00007730: 0a6f 7065 6e6c 6c6d 2073 7461 7274 2054  .openllm start T
+00007740: 6865 426c 6f6b 652f 4c6c 616d 612d 322d  heBloke/Llama-2-
+00007750: 3742 2d43 6861 742d 4750 5451 202d 2d71  7B-Chat-GPTQ --q
+00007760: 7561 6e74 697a 6520 6770 7471 0a60 6060  uantize gptq.```
+00007770: 0a0a 3e20 5b21 4e4f 5445 5d0a 3e20 496e  ..> [!NOTE].> In
+00007780: 206f 7264 6572 2074 6f20 7275 6e20 4750   order to run GP
+00007790: 5451 2c20 6d61 6b65 2073 7572 6520 796f  TQ, make sure yo
+000077a0: 7520 7275 6ec2 a060 7069 7020 696e 7374  u run..`pip inst
+000077b0: 616c 6c20 226f 7065 6e6c 6c6d 5b67 7074  all "openllm[gpt
+000077c0: 715d 2260 0a3e 2066 6972 7374 2074 6f20  q]"`.> first to 
+000077d0: 696e 7374 616c 6c20 7468 6520 6465 7065  install the depe
+000077e0: 6e64 656e 6379 2e20 4672 6f6d 2074 6865  ndency. From the
+000077f0: 2047 5054 5120 7061 7065 722c 2069 7420   GPTQ paper, it 
+00007800: 6973 2072 6563 6f6d 6d65 6e64 6564 2074  is recommended t
+00007810: 6f20 7175 616e 7469 7a65 6420 7468 6520  o quantized the 
+00007820: 7765 6967 6874 7320 6265 666f 7265 2073  weights before s
+00007830: 6572 7669 6e67 2e0a 3e20 5365 65c2 a05b  erving..> See..[
+00007840: 4175 746f 4750 5451 5d28 6874 7470 733a  AutoGPTQ](https:
+00007850: 2f2f 6769 7468 7562 2e63 6f6d 2f50 616e  //github.com/Pan
+00007860: 5169 5765 692f 4175 746f 4750 5451 29c2  QiWei/AutoGPTQ).
+00007870: a066 6f72 206d 6f72 6520 696e 666f 726d  .for more inform
+00007880: 6174 696f 6e20 6f6e 2047 5054 5120 7175  ation on GPTQ qu
+00007890: 616e 7469 7a61 7469 6f6e 2e0a 0a23 2323  antization...###
+000078a0: 2076 4c4c 4d20 6261 636b 656e 640a 0a57   vLLM backend..W
+000078b0: 6974 6820 764c 4c4d 2062 6163 6b65 6e64  ith vLLM backend
+000078c0: 2c20 4f70 656e 4c4c 4d20 7375 7070 6f72  , OpenLLM suppor
+000078d0: 7473 2060 6177 7160 2c20 6073 7175 6565  ts `awq`, `squee
+000078e0: 7a65 6c6c 6d60 0a0a 546f 2072 756e 2069  zellm`..To run i
+000078f0: 6e66 6572 656e 6365 2077 6974 68c2 a060  nference with..`
+00007900: 6177 7160 2c20 7369 6d70 6c79 2070 6173  awq`, simply pas
+00007910: 73c2 a060 2d2d 7175 616e 7469 7a65 2061  s..`--quantize a
+00007920: 7771 603a 0a0a 6060 6062 6173 680a 6f70  wq`:..```bash.op
+00007930: 656e 6c6c 6d20 7374 6172 7420 5468 6542  enllm start TheB
+00007940: 6c6f 6b65 2f7a 6570 6879 722d 3742 2d61  loke/zephyr-7B-a
+00007950: 6c70 6861 2d41 5751 202d 2d71 7561 6e74  lpha-AWQ --quant
+00007960: 697a 6520 6177 710a 6060 600a 0a54 6f20  ize awq.```..To 
+00007970: 7275 6e20 696e 6665 7265 6e63 6520 7769  run inference wi
+00007980: 7468 2060 7371 7565 657a 656c 6c6d 602c  th `squeezellm`,
+00007990: 2073 696d 706c 7920 7061 7373 2060 2d2d   simply pass `--
+000079a0: 7175 616e 7469 7a65 2073 7175 6565 7a65  quantize squeeze
+000079b0: 6c6c 6d60 3a0a 0a60 6060 6261 7368 0a6f  llm`:..```bash.o
+000079c0: 7065 6e6c 6c6d 2073 7461 7274 2073 7175  penllm start squ
+000079d0: 6565 7a65 2d61 692d 6c61 622f 7371 2d6c  eeze-ai-lab/sq-l
+000079e0: 6c61 6d61 2d32 2d37 622d 7734 2d73 3020  lama-2-7b-w4-s0 
+000079f0: 2d2d 7175 616e 7469 7a65 2073 7175 6565  --quantize squee
+00007a00: 7a65 6c6c 6d20 2d2d 7365 7269 616c 697a  zellm --serializ
+00007a10: 6174 696f 6e20 6c65 6761 6379 0a60 6060  ation legacy.```
+00007a20: 0a0a 3e20 5b21 494d 504f 5254 414e 545d  ..> [!IMPORTANT]
+00007a30: 0a3e 2053 696e 6365 2062 6f74 6820 6073  .> Since both `s
+00007a40: 7175 6565 7a65 6c6c 6d60 2061 6e64 2060  queezellm` and `
+00007a50: 6177 7160 2061 7265 2077 6569 6768 742d  awq` are weight-
+00007a60: 6177 6172 6520 7175 616e 7469 7a61 7469  aware quantizati
+00007a70: 6f6e 206d 6574 686f 6473 2c20 6d65 616e  on methods, mean
+00007a80: 696e 6720 7468 6520 7175 616e 7469 7a61  ing the quantiza
+00007a90: 7469 6f6e 2069 7320 646f 6e65 2064 7572  tion is done dur
+00007aa0: 696e 6720 7472 6169 6e69 6e67 2c20 616c  ing training, al
+00007ab0: 6c20 7072 652d 7472 6169 6e65 6420 7765  l pre-trained we
+00007ac0: 6967 6874 7320 6e65 6564 7320 746f 2067  ights needs to g
+00007ad0: 6574 2071 7561 6e74 697a 6564 2062 6566  et quantized bef
+00007ae0: 6f72 6520 696e 6665 7265 6e63 6520 7469  ore inference ti
+00007af0: 6d65 2e20 4d61 6b65 2073 7572 6520 746f  me. Make sure to
+00007b00: 2066 696e 6420 636f 6d70 6174 6962 6c65   find compatible
+00007b10: 2077 6569 6768 7473 206f 6e20 4875 6767   weights on Hugg
+00007b20: 696e 6746 6163 6520 4875 6220 666f 7220  ingFace Hub for 
+00007b30: 796f 7572 206d 6f64 656c 206f 6620 6368  your model of ch
+00007b40: 6f69 6365 2e0a 0a23 2320 f09f 9ba0 efb8  oice...## ......
+00007b50: 8f20 5365 7276 696e 6720 6669 6e65 2d74  . Serving fine-t
+00007b60: 756e 696e 6720 6c61 7965 7273 0a0a 5b50  uning layers..[P
+00007b70: 4546 545d 2868 7474 7073 3a2f 2f68 7567  EFT](https://hug
+00007b80: 6769 6e67 6661 6365 2e63 6f2f 646f 6373  gingface.co/docs
+00007b90: 2f70 6566 742f 696e 6465 7829 2c20 6f72  /peft/index), or
+00007ba0: 2050 6172 616d 6574 6572 2d45 6666 6963   Parameter-Effic
+00007bb0: 6965 6e74 2046 696e 652d 5475 6e69 6e67  ient Fine-Tuning
+00007bc0: 2c20 6973 2061 206d 6574 686f 646f 6c6f  , is a methodolo
+00007bd0: 6779 2064 6573 6967 6e65 6420 746f 2066  gy designed to f
+00007be0: 696e 652d 7475 6e65 2070 7265 2d74 7261  ine-tune pre-tra
+00007bf0: 696e 6564 206d 6f64 656c 7320 6d6f 7265  ined models more
+00007c00: 2065 6666 6963 6965 6e74 6c79 2e20 496e   efficiently. In
+00007c10: 7374 6561 6420 6f66 2061 646a 7573 7469  stead of adjusti
+00007c20: 6e67 2061 6c6c 206d 6f64 656c 2070 6172  ng all model par
+00007c30: 616d 6574 6572 732c 2050 4546 5420 666f  ameters, PEFT fo
+00007c40: 6375 7365 7320 6f6e 2074 756e 696e 6720  cuses on tuning 
+00007c50: 6f6e 6c79 2061 2073 7562 7365 742c 2072  only a subset, r
+00007c60: 6564 7563 696e 6720 636f 6d70 7574 6174  educing computat
+00007c70: 696f 6e61 6c20 616e 6420 7374 6f72 6167  ional and storag
+00007c80: 6520 636f 7374 732e 205b 4c6f 5241 5d28  e costs. [LoRA](
+00007c90: 6874 7470 733a 2f2f 6875 6767 696e 6766  https://huggingf
+00007ca0: 6163 652e 636f 2f64 6f63 732f 7065 6674  ace.co/docs/peft
+00007cb0: 2f63 6f6e 6365 7074 7561 6c5f 6775 6964  /conceptual_guid
+00007cc0: 6573 2f6c 6f72 6129 2028 4c6f 772d 5261  es/lora) (Low-Ra
+00007cd0: 6e6b 2041 6461 7074 6174 696f 6e29 2069  nk Adaptation) i
+00007ce0: 7320 6f6e 6520 6f66 2074 6865 2074 6563  s one of the tec
+00007cf0: 686e 6971 7565 7320 7375 7070 6f72 7465  hniques supporte
+00007d00: 6420 6279 2050 4546 542e 2049 7420 7374  d by PEFT. It st
+00007d10: 7265 616d 6c69 6e65 7320 6669 6e65 2d74  reamlines fine-t
+00007d20: 756e 696e 6720 6279 2075 7369 6e67 206c  uning by using l
+00007d30: 6f77 2d72 616e 6b20 6465 636f 6d70 6f73  ow-rank decompos
+00007d40: 6974 696f 6e20 746f 2072 6570 7265 7365  ition to represe
+00007d50: 6e74 2077 6569 6768 7420 7570 6461 7465  nt weight update
+00007d60: 732c 2074 6865 7265 6279 2064 7261 7374  s, thereby drast
+00007d70: 6963 616c 6c79 2072 6564 7563 696e 6720  ically reducing 
+00007d80: 7468 6520 6e75 6d62 6572 206f 6620 7472  the number of tr
+00007d90: 6169 6e61 626c 6520 7061 7261 6d65 7465  ainable paramete
+00007da0: 7273 2e0a 0a57 6974 6820 4f70 656e 4c4c  rs...With OpenLL
+00007db0: 4d2c 2079 6f75 2063 616e 2074 616b 6520  M, you can take 
+00007dc0: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
+00007dd0: 2066 696e 652d 7475 6e69 6e67 2066 6561   fine-tuning fea
+00007de0: 7475 7265 2062 7920 7365 7276 696e 6720  ture by serving 
+00007df0: 6d6f 6465 6c73 2077 6974 6820 616e 7920  models with any 
+00007e00: 5045 4654 2d63 6f6d 7061 7469 626c 6520  PEFT-compatible 
+00007e10: 6c61 7965 7273 2075 7369 6e67 2074 6865  layers using the
+00007e20: 2060 2d2d 6164 6170 7465 722d 6964 6020   `--adapter-id` 
+00007e30: 6f70 7469 6f6e 2e20 466f 7220 6578 616d  option. For exam
+00007e40: 706c 653a 0a0a 6060 6062 6173 680a 6f70  ple:..```bash.op
+00007e50: 656e 6c6c 6d20 7374 6172 7420 6661 6365  enllm start face
+00007e60: 626f 6f6b 2f6f 7074 2d36 2e37 6220 2d2d  book/opt-6.7b --
+00007e70: 6164 6170 7465 722d 6964 2061 6172 6e70  adapter-id aarnp
+00007e80: 686d 2f6f 7074 2d36 2d37 622d 7175 6f74  hm/opt-6-7b-quot
+00007e90: 6573 3a64 6566 6175 6c74 0a60 6060 0a0a  es:default.```..
+00007ea0: 4f70 656e 4c4c 4d20 616c 736f 2070 726f  OpenLLM also pro
+00007eb0: 7669 6465 7320 666c 6578 6962 696c 6974  vides flexibilit
+00007ec0: 7920 6279 2073 7570 706f 7274 696e 6720  y by supporting 
+00007ed0: 6164 6170 7465 7273 2066 726f 6d20 6375  adapters from cu
+00007ee0: 7374 6f6d 2066 696c 6520 7061 7468 733a  stom file paths:
+00007ef0: 0a0a 6060 6062 6173 680a 6f70 656e 6c6c  ..```bash.openll
+00007f00: 6d20 7374 6172 7420 6661 6365 626f 6f6b  m start facebook
+00007f10: 2f6f 7074 2d36 2e37 6220 2d2d 6164 6170  /opt-6.7b --adap
+00007f20: 7465 722d 6964 202f 7061 7468 2f74 6f2f  ter-id /path/to/
+00007f30: 6164 6170 7465 7273 3a6c 6f63 616c 5f61  adapters:local_a
+00007f40: 6461 7074 6572 0a60 6060 0a0a 546f 2075  dapter.```..To u
+00007f50: 7365 206d 756c 7469 706c 6520 6164 6170  se multiple adap
+00007f60: 7465 7273 2c20 7573 6520 7468 6520 666f  ters, use the fo
+00007f70: 6c6c 6f77 696e 6720 666f 726d 6174 3a0a  llowing format:.
+00007f80: 0a60 6060 6261 7368 0a6f 7065 6e6c 6c6d  .```bash.openllm
+00007f90: 2073 7461 7274 2066 6163 6562 6f6f 6b2f   start facebook/
+00007fa0: 6f70 742d 362e 3762 202d 2d61 6461 7074  opt-6.7b --adapt
+00007fb0: 6572 2d69 6420 6161 726e 7068 6d2f 6f70  er-id aarnphm/op
+00007fc0: 742d 362e 3762 2d6c 6f72 613a 6465 6661  t-6.7b-lora:defa
+00007fd0: 756c 7420 2d2d 6164 6170 7465 722d 6964  ult --adapter-id
+00007fe0: 2061 6172 6e70 686d 2f6f 7074 2d36 2e37   aarnphm/opt-6.7
+00007ff0: 622d 6672 656e 6368 3a66 7265 6e63 685f  b-french:french_
+00008000: 6c6f 7261 0a60 6060 0a0a 4279 2064 6566  lora.```..By def
+00008010: 6175 6c74 2c20 616c 6c20 6164 6170 7465  ault, all adapte
+00008020: 7273 2077 696c 6c20 6265 2069 6e6a 6563  rs will be injec
+00008030: 7465 6420 696e 746f 2074 6865 206d 6f64  ted into the mod
+00008040: 656c 7320 6475 7269 6e67 2073 7461 7274  els during start
+00008050: 7570 2e20 4164 6170 7465 7273 2063 616e  up. Adapters can
+00008060: 2062 6520 7370 6563 6966 6965 6420 7065   be specified pe
+00008070: 7220 7265 7175 6573 7420 7669 6120 6061  r request via `a
+00008080: 6461 7074 6572 5f6e 616d 6560 3a0a 0a60  dapter_name`:..`
+00008090: 6060 6261 7368 0a63 7572 6c20 2d58 2027  ``bash.curl -X '
+000080a0: 504f 5354 2720 5c0a 2020 2768 7474 703a  POST' \.  'http:
+000080b0: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
+000080c0: 2f76 312f 6765 6e65 7261 7465 2720 5c0a  /v1/generate' \.
+000080d0: 2020 2d48 2027 6163 6365 7074 3a20 6170    -H 'accept: ap
+000080e0: 706c 6963 6174 696f 6e2f 6a73 6f6e 2720  plication/json' 
+000080f0: 5c0a 2020 2d48 2027 436f 6e74 656e 742d  \.  -H 'Content-
+00008100: 5479 7065 3a20 6170 706c 6963 6174 696f  Type: applicatio
+00008110: 6e2f 6a73 6f6e 2720 5c0a 2020 2d64 2027  n/json' \.  -d '
+00008120: 7b0a 2020 2270 726f 6d70 7422 3a20 2257  {.  "prompt": "W
+00008130: 6861 7420 6973 2074 6865 206d 6561 6e69  hat is the meani
+00008140: 6e67 206f 6620 6c69 6665 3f22 2c0a 2020  ng of life?",.  
+00008150: 2273 746f 7022 3a20 5b0a 2020 2020 2270  "stop": [.    "p
+00008160: 6869 6c6f 736f 7068 6572 220a 2020 5d2c  hilosopher".  ],
+00008170: 0a20 2022 6c6c 6d5f 636f 6e66 6967 223a  .  "llm_config":
+00008180: 207b 0a20 2020 2022 6d61 785f 6e65 775f   {.    "max_new_
+00008190: 746f 6b65 6e73 223a 2032 3536 2c0a 2020  tokens": 256,.  
+000081a0: 2020 2274 656d 7065 7261 7475 7265 223a    "temperature":
+000081b0: 2030 2e37 352c 0a20 2020 2022 746f 705f   0.75,.    "top_
+000081c0: 6b22 3a20 3135 2c0a 2020 2020 2274 6f70  k": 15,.    "top
+000081d0: 5f70 223a 2031 0a20 207d 2c0a 2020 2261  _p": 1.  },.  "a
+000081e0: 6461 7074 6572 5f6e 616d 6522 3a20 2264  dapter_name": "d
+000081f0: 6566 6175 6c74 220a 7d27 0a60 6060 0a0a  efault".}'.```..
+00008200: 546f 2069 6e63 6c75 6465 2074 6869 7320  To include this 
+00008210: 696e 746f 2074 6865 2042 656e 746f 2c20  into the Bento, 
+00008220: 796f 7520 6361 6e20 7370 6563 6966 7920  you can specify 
+00008230: 7468 65c2 a060 2d2d 6164 6170 7465 722d  the..`--adapter-
+00008240: 6964 60c2 a06f 7074 696f 6e20 7768 656e  id`..option when
+00008250: 2075 7369 6e67 2074 6865 c2a0 606f 7065   using the..`ope
+00008260: 6e6c 6c6d 2062 7569 6c64 6020 636f 6d6d  nllm build` comm
+00008270: 616e 643a 0a0a 6060 6062 6173 680a 6f70  and:..```bash.op
+00008280: 656e 6c6c 6d20 6275 696c 6420 6661 6365  enllm build face
+00008290: 626f 6f6b 2f6f 7074 2d36 2e37 6220 2d2d  book/opt-6.7b --
+000082a0: 6164 6170 7465 722d 6964 202e 2e2e 0a60  adapter-id ....`
+000082b0: 6060 0a0a 4966 2079 6f75 2075 7365 2061  ``..If you use a
+000082c0: 2072 656c 6174 6976 6520 7061 7468 2066   relative path f
+000082d0: 6f72 2060 2d2d 6164 6170 7465 722d 6964  or `--adapter-id
+000082e0: 602c 2079 6f75 206e 6565 6420 746f 2061  `, you need to a
+000082f0: 6464 2060 2d2d 6275 696c 642d 6374 7860  dd `--build-ctx`
+00008300: 2e0a 0a60 6060 6261 7368 0a6f 7065 6e6c  ...```bash.openl
+00008310: 6c6d 2062 7569 6c64 2066 6163 6562 6f6f  lm build faceboo
+00008320: 6b2f 6f70 742d 362e 3762 202d 2d61 6461  k/opt-6.7b --ada
+00008330: 7074 6572 2d69 6420 2e2f 7061 7468 2f74  pter-id ./path/t
+00008340: 6f2f 6164 6170 7465 725f 6964 202d 2d62  o/adapter_id --b
+00008350: 7569 6c64 2d63 7478 202e 0a60 6060 0a0a  uild-ctx ..```..
+00008360: 3e20 5b21 494d 504f 5254 414e 545d 0a3e  > [!IMPORTANT].>
+00008370: 2046 696e 652d 7475 6e69 6e67 2073 7570   Fine-tuning sup
+00008380: 706f 7274 2069 7320 7374 696c 6c20 6578  port is still ex
+00008390: 7065 7269 6d65 6e74 616c 2061 6e64 2063  perimental and c
+000083a0: 7572 7265 6e74 6c79 206f 6e6c 7920 776f  urrently only wo
+000083b0: 726b 7320 7769 7468 2050 7954 6f72 6368  rks with PyTorch
+000083c0: 2062 6163 6b65 6e64 2e20 764c 4c4d 2073   backend. vLLM s
+000083d0: 7570 706f 7274 2069 7320 636f 6d69 6e67  upport is coming
+000083e0: 2073 6f6f 6e2e 0a0a 0a23 2320 e29a 99ef   soon....## ....
+000083f0: b88f 2049 6e74 6567 7261 7469 6f6e 730a  .. Integrations.
+00008400: 0a4f 7065 6e4c 4c4d 2069 7320 6e6f 7420  .OpenLLM is not 
+00008410: 6a75 7374 2061 2073 7461 6e64 616c 6f6e  just a standalon
+00008420: 6520 7072 6f64 7563 743b 2069 7427 7320  e product; it's 
+00008430: 6120 6275 696c 6469 6e67 2062 6c6f 636b  a building block
+00008440: 2064 6573 6967 6e65 6420 746f 0a69 6e74   designed to.int
+00008450: 6567 7261 7465 2077 6974 6820 6f74 6865  egrate with othe
+00008460: 7220 706f 7765 7266 756c 2074 6f6f 6c73  r powerful tools
+00008470: 2065 6173 696c 792e 2057 6520 6375 7272   easily. We curr
+00008480: 656e 746c 7920 6f66 6665 7220 696e 7465  ently offer inte
+00008490: 6772 6174 696f 6e20 7769 7468 0a5b 4f70  gration with.[Op
+000084a0: 656e 4149 2773 2043 6f6d 7061 7469 626c  enAI's Compatibl
+000084b0: 6520 456e 6470 6f69 6e74 735d 2868 7474  e Endpoints](htt
+000084c0: 7073 3a2f 2f70 6c61 7466 6f72 6d2e 6f70  ps://platform.op
+000084d0: 656e 6169 2e63 6f6d 2f64 6f63 732f 6170  enai.com/docs/ap
+000084e0: 692d 7265 6665 7265 6e63 652f 636f 6d70  i-reference/comp
+000084f0: 6c65 7469 6f6e 732f 6f62 6a65 6374 292c  letions/object),
+00008500: 0a5b 4c6c 616d 6149 6e64 6578 5d28 6874  .[LlamaIndex](ht
+00008510: 7470 733a 2f2f 7777 772e 6c6c 616d 6169  tps://www.llamai
+00008520: 6e64 6578 2e61 692f 292c 0a5b 4c61 6e67  ndex.ai/),.[Lang
+00008530: 4368 6169 6e5d 2868 7474 7073 3a2f 2f67  Chain](https://g
+00008540: 6974 6875 622e 636f 6d2f 6877 6368 6173  ithub.com/hwchas
+00008550: 6531 372f 6c61 6e67 6368 6169 6e29 2c20  e17/langchain), 
+00008560: 616e 640a 5b54 7261 6e73 666f 726d 6572  and.[Transformer
+00008570: 7320 4167 656e 7473 5d28 6874 7470 733a  s Agents](https:
+00008580: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00008590: 2f64 6f63 732f 7472 616e 7366 6f72 6d65  /docs/transforme
+000085a0: 7273 2f74 7261 6e73 666f 726d 6572 735f  rs/transformers_
+000085b0: 6167 656e 7473 292e 0a0a 2323 2320 4f70  agents)...### Op
+000085c0: 656e 4149 2043 6f6d 7061 7469 626c 6520  enAI Compatible 
+000085d0: 456e 6470 6f69 6e74 730a 0a4f 7065 6e4c  Endpoints..OpenL
+000085e0: 4c4d 2053 6572 7665 7220 6361 6e20 6265  LM Server can be
+000085f0: 2075 7365 6420 6173 2061 2064 726f 702d   used as a drop-
+00008600: 696e 2072 6570 6c61 6365 6d65 6e74 2066  in replacement f
+00008610: 6f72 204f 7065 6e41 4927 7320 4150 492e  or OpenAI's API.
+00008620: 2053 696d 706c 790a 7370 6563 6966 7920   Simply.specify 
+00008630: 7468 6520 6261 7365 5f75 726c 2074 6f20  the base_url to 
+00008640: 606c 6c6d 2d65 6e64 706f 696e 742f 7631  `llm-endpoint/v1
+00008650: 6020 616e 6420 796f 7520 6172 6520 676f  ` and you are go
+00008660: 6f64 2074 6f20 676f 3a0a 0a60 6060 7079  od to go:..```py
+00008670: 7468 6f6e 0a69 6d70 6f72 7420 6f70 656e  thon.import open
+00008680: 6169 0a0a 636c 6965 6e74 203d 206f 7065  ai..client = ope
+00008690: 6e61 692e 4f70 656e 4149 280a 2020 6261  nai.OpenAI(.  ba
+000086a0: 7365 5f75 726c 3d27 6874 7470 3a2f 2f6c  se_url='http://l
+000086b0: 6f63 616c 686f 7374 3a33 3030 302f 7631  ocalhost:3000/v1
+000086c0: 272c 2061 7069 5f6b 6579 3d27 6e61 270a  ', api_key='na'.
+000086d0: 2920 2023 2048 6572 6520 7468 6520 7365  )  # Here the se
+000086e0: 7276 6572 2069 7320 7275 6e6e 696e 6720  rver is running 
+000086f0: 6f6e 206c 6f63 616c 686f 7374 3a33 3030  on localhost:300
+00008700: 300a 0a63 6f6d 706c 6574 696f 6e73 203d  0..completions =
+00008710: 2063 6c69 656e 742e 636f 6d70 6c65 7469   client.completi
+00008720: 6f6e 732e 6372 6561 7465 280a 2020 7072  ons.create(.  pr
+00008730: 6f6d 7074 3d27 5772 6974 6520 6d65 2061  ompt='Write me a
+00008740: 2074 6167 206c 696e 6520 666f 7220 616e   tag line for an
+00008750: 2069 6365 2063 7265 616d 2073 686f 702e   ice cream shop.
+00008760: 272c 206d 6f64 656c 3d6d 6f64 656c 2c20  ', model=model, 
+00008770: 6d61 785f 746f 6b65 6e73 3d36 342c 2073  max_tokens=64, s
+00008780: 7472 6561 6d3d 7374 7265 616d 0a29 0a60  tream=stream.).`
+00008790: 6060 0a0a 5468 6520 636f 6d70 6174 6962  ``..The compatib
+000087a0: 6c65 2065 6e64 706f 696e 7473 2073 7570  le endpoints sup
+000087b0: 706f 7274 7320 602f 636f 6d70 6c65 7469  ports `/completi
+000087c0: 6f6e 7360 2c20 602f 6368 6174 2f63 6f6d  ons`, `/chat/com
+000087d0: 706c 6574 696f 6e73 602c 2061 6e64 2060  pletions`, and `
+000087e0: 2f6d 6f64 656c 7360 0a0a 3e20 5b21 4e4f  /models`..> [!NO
+000087f0: 5445 5d0a 3e20 596f 7520 6361 6e20 6669  TE].> You can fi
+00008800: 6e64 206f 7574 204f 7065 6e41 4920 6578  nd out OpenAI ex
+00008810: 616d 706c 6520 636c 6965 6e74 7320 756e  ample clients un
+00008820: 6465 7220 7468 650a 3e20 5b65 7861 6d70  der the.> [examp
+00008830: 6c65 735d 2868 7474 7073 3a2f 2f67 6974  les](https://git
+00008840: 6875 622e 636f 6d2f 6265 6e74 6f6d 6c2f  hub.com/bentoml/
+00008850: 4f70 656e 4c4c 4d2f 7472 6565 2f6d 6169  OpenLLM/tree/mai
+00008860: 6e2f 6578 616d 706c 6573 2920 666f 6c64  n/examples) fold
+00008870: 6572 2e0a 0a0a 2323 2320 5b4c 6c61 6d61  er....### [Llama
+00008880: 496e 6465 785d 2868 7474 7073 3a2f 2f64  Index](https://d
+00008890: 6f63 732e 6c6c 616d 6169 6e64 6578 2e61  ocs.llamaindex.a
+000088a0: 692f 656e 2f73 7461 626c 652f 6578 616d  i/en/stable/exam
+000088b0: 706c 6573 2f6c 6c6d 2f6f 7065 6e6c 6c6d  ples/llm/openllm
+000088c0: 2f29 0a0a 546f 2073 7461 7274 2061 206c  /)..To start a l
+000088d0: 6f63 616c 204c 4c4d 2077 6974 6820 606c  ocal LLM with `l
+000088e0: 6c61 6d61 5f69 6e64 6578 602c 2073 696d  lama_index`, sim
+000088f0: 706c 7920 7573 6520 606c 6c61 6d61 5f69  ply use `llama_i
+00008900: 6e64 6578 2e6c 6c6d 732e 6f70 656e 6c6c  ndex.llms.openll
+00008910: 6d2e 4f70 656e 4c4c 4d60 3a0a 0a60 6060  m.OpenLLM`:..```
+00008920: 7079 7468 6f6e 0a69 6d70 6f72 7420 6173  python.import as
+00008930: 796e 6369 6f0a 6672 6f6d 206c 6c61 6d61  yncio.from llama
+00008940: 5f69 6e64 6578 2e6c 6c6d 732e 6f70 656e  _index.llms.open
+00008950: 6c6c 6d20 696d 706f 7274 204f 7065 6e4c  llm import OpenL
+00008960: 4c4d 0a0a 6c6c 6d20 3d20 4f70 656e 4c4c  LM..llm = OpenLL
+00008970: 4d28 2748 7567 6769 6e67 4661 6365 4834  M('HuggingFaceH4
+00008980: 2f7a 6570 6879 722d 3762 2d61 6c70 6861  /zephyr-7b-alpha
+00008990: 2729 0a0a 6c6c 6d2e 636f 6d70 6c65 7465  ')..llm.complete
+000089a0: 2827 5468 6520 6d65 616e 696e 6720 6f66  ('The meaning of
+000089b0: 206c 6966 6520 6973 2729 0a0a 0a61 7379   life is')...asy
+000089c0: 6e63 2064 6566 206d 6169 6e28 7072 6f6d  nc def main(prom
+000089d0: 7074 2c20 2a2a 6b77 6172 6773 293a 0a20  pt, **kwargs):. 
+000089e0: 2061 7379 6e63 2066 6f72 2069 7420 696e   async for it in
+000089f0: 206c 6c6d 2e61 7374 7265 616d 5f63 6861   llm.astream_cha
+00008a00: 7428 7072 6f6d 7074 2c20 2a2a 6b77 6172  t(prompt, **kwar
+00008a10: 6773 293a 0a20 2020 2070 7269 6e74 2869  gs):.    print(i
+00008a20: 7429 0a0a 0a61 7379 6e63 696f 2e72 756e  t)...asyncio.run
+00008a30: 286d 6169 6e28 2754 6865 2074 696d 6520  (main('The time 
+00008a40: 6174 2053 616e 2046 7261 6e63 6973 636f  at San Francisco
+00008a50: 2069 7327 2929 0a60 6060 0a0a 4966 2074   is')).```..If t
+00008a60: 6865 7265 2069 7320 6120 7265 6d6f 7465  here is a remote
+00008a70: 204c 4c4d 2053 6572 7665 7220 7275 6e6e   LLM Server runn
+00008a80: 696e 6720 656c 7365 7768 6572 652c 2074  ing elsewhere, t
+00008a90: 6865 6e20 796f 7520 6361 6e20 7573 6520  hen you can use 
+00008aa0: 606c 6c61 6d61 5f69 6e64 6578 2e6c 6c6d  `llama_index.llm
+00008ab0: 732e 6f70 656e 6c6c 6d2e 4f70 656e 4c4c  s.openllm.OpenLL
+00008ac0: 4d41 5049 603a 0a0a 6060 6070 7974 686f  MAPI`:..```pytho
+00008ad0: 6e0a 6672 6f6d 206c 6c61 6d61 5f69 6e64  n.from llama_ind
+00008ae0: 6578 2e6c 6c6d 732e 6f70 656e 6c6c 6d20  ex.llms.openllm 
+00008af0: 696d 706f 7274 204f 7065 6e4c 4c4d 4150  import OpenLLMAP
+00008b00: 490a 6060 600a 0a3e 205b 214e 4f54 455d  I.```..> [!NOTE]
+00008b10: 0a3e 2041 6c6c 2073 796e 6368 726f 6e6f  .> All synchrono
+00008b20: 7573 2061 6e64 2061 7379 6e63 6872 6f6e  us and asynchron
+00008b30: 6f75 7320 4150 4920 6672 6f6d 2060 6c6c  ous API from `ll
+00008b40: 616d 615f 696e 6465 782e 6c6c 6d73 2e4c  ama_index.llms.L
+00008b50: 4c4d 6020 6172 6520 7375 7070 6f72 7465  LM` are supporte
+00008b60: 642e 0a0a 2323 2320 5b4c 616e 6743 6861  d...### [LangCha
+00008b70: 696e 5d28 6874 7470 733a 2f2f 7079 7468  in](https://pyth
+00008b80: 6f6e 2e6c 616e 6763 6861 696e 2e63 6f6d  on.langchain.com
+00008b90: 2f64 6f63 732f 696e 7465 6772 6174 696f  /docs/integratio
+00008ba0: 6e73 2f6c 6c6d 732f 6f70 656e 6c6c 6d2f  ns/llms/openllm/
+00008bb0: 290a 0a53 7069 6e20 7570 2061 6e20 4f70  )..Spin up an Op
+00008bc0: 656e 4c4c 4d20 7365 7276 6572 2c20 616e  enLLM server, an
+00008bd0: 6420 636f 6e6e 6563 7420 746f 2069 7420  d connect to it 
+00008be0: 6279 2073 7065 6369 6679 696e 6720 6974  by specifying it
+00008bf0: 7320 5552 4c3a 0a0a 6060 6070 7974 686f  s URL:..```pytho
+00008c00: 6e0a 6672 6f6d 206c 616e 6763 6861 696e  n.from langchain
+00008c10: 2e6c 6c6d 7320 696d 706f 7274 204f 7065  .llms import Ope
+00008c20: 6e4c 4c4d 0a0a 6c6c 6d20 3d20 4f70 656e  nLLM..llm = Open
+00008c30: 4c4c 4d28 7365 7276 6572 5f75 726c 3d27  LLM(server_url='
+00008c40: 6874 7470 3a2f 2f34 342e 3233 2e31 3233  http://44.23.123
+00008c50: 2e31 3a33 3030 3027 2c20 7365 7276 6572  .1:3000', server
+00008c60: 5f74 7970 653d 2768 7474 7027 290a 6c6c  _type='http').ll
+00008c70: 6d28 2757 6861 7420 6973 2074 6865 2064  m('What is the d
+00008c80: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+00008c90: 6e20 6120 6475 636b 2061 6e64 2061 2067  n a duck and a g
+00008ca0: 6f6f 7365 3f20 416e 6420 7768 7920 7468  oose? And why th
+00008cb0: 6572 6520 6172 6520 736f 206d 616e 7920  ere are so many 
+00008cc0: 476f 6f73 6520 696e 2043 616e 6164 613f  Goose in Canada?
+00008cd0: 2729 0a60 6060 0a0a 2323 2320 5472 616e  ').```..### Tran
+00008ce0: 7366 6f72 6d65 7273 2041 6765 6e74 730a  sformers Agents.
+00008cf0: 0a4f 7065 6e4c 4c4d 2073 6561 6d6c 6573  .OpenLLM seamles
+00008d00: 736c 7920 696e 7465 6772 6174 6573 2077  sly integrates w
+00008d10: 6974 680a 5b54 7261 6e73 666f 726d 6572  ith.[Transformer
+00008d20: 7320 4167 656e 7473 5d28 6874 7470 733a  s Agents](https:
+00008d30: 2f2f 6875 6767 696e 6766 6163 652e 636f  //huggingface.co
+00008d40: 2f64 6f63 732f 7472 616e 7366 6f72 6d65  /docs/transforme
+00008d50: 7273 2f74 7261 6e73 666f 726d 6572 735f  rs/transformers_
+00008d60: 6167 656e 7473 292e 0a0a 3e20 5b21 5741  agents)...> [!WA
+00008d70: 524e 494e 475d 0a3e 2054 6865 2054 7261  RNING].> The Tra
+00008d80: 6e73 666f 726d 6572 7320 4167 656e 7420  nsformers Agent 
+00008d90: 6973 2073 7469 6c6c 2061 7420 616e 2065  is still at an e
+00008da0: 7870 6572 696d 656e 7461 6c20 7374 6167  xperimental stag
+00008db0: 652e 2049 7420 6973 0a3e 2072 6563 6f6d  e. It is.> recom
+00008dc0: 6d65 6e64 6564 2074 6f20 696e 7374 616c  mended to instal
+00008dd0: 6c20 4f70 656e 4c4c 4d20 7769 7468 2060  l OpenLLM with `
+00008de0: 7069 7020 696e 7374 616c 6c20 2d72 206e  pip install -r n
+00008df0: 6967 6874 6c79 2d72 6571 7569 7265 6d65  ightly-requireme
+00008e00: 6e74 732e 7478 7460 0a3e 2074 6f20 6765  nts.txt`.> to ge
+00008e10: 7420 7468 6520 6c61 7465 7374 2041 5049  t the latest API
+00008e20: 2075 7064 6174 6520 666f 7220 4875 6767   update for Hugg
+00008e30: 696e 6746 6163 6520 6167 656e 742e 0a0a  ingFace agent...
+00008e40: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
+00008e50: 2074 7261 6e73 666f 726d 6572 730a 0a61   transformers..a
+00008e60: 6765 6e74 203d 2074 7261 6e73 666f 726d  gent = transform
+00008e70: 6572 732e 4866 4167 656e 7428 2768 7474  ers.HfAgent('htt
+00008e80: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3330  p://localhost:30
+00008e90: 3030 2f68 662f 6167 656e 7427 2920 2023  00/hf/agent')  #
+00008ea0: 2055 524c 2074 6861 7420 7275 6e73 2074   URL that runs t
+00008eb0: 6865 204f 7065 6e4c 4c4d 2073 6572 7665  he OpenLLM serve
+00008ec0: 720a 0a61 6765 6e74 2e72 756e 2827 4973  r..agent.run('Is
+00008ed0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2060   the following `
+00008ee0: 7465 7874 6020 706f 7369 7469 7665 206f  text` positive o
+00008ef0: 7220 6e65 6761 7469 7665 3f27 2c20 7465  r negative?', te
+00008f00: 7874 3d22 4920 646f 6e27 7420 6c69 6b65  xt="I don't like
+00008f10: 2068 6f77 2074 6869 7320 6d6f 6465 6c73   how this models
+00008f20: 2069 7320 6765 6e65 7261 7465 2069 6e70   is generate inp
+00008f30: 7574 7322 290a 6060 600a 0a3c 212d 2d20  uts").```..<!-- 
+00008f40: 6861 7463 682d 6661 6e63 792d 7079 7069  hatch-fancy-pypi
+00008f50: 2d72 6561 646d 6520 696e 7465 7269 6d20  -readme interim 
+00008f60: 7374 6f70 202d 2d3e 0a0a 215b 4769 6620  stop -->..![Gif 
+00008f70: 7368 6f77 696e 6720 4167 656e 7420 696e  showing Agent in
+00008f80: 7465 6772 6174 696f 6e5d 282f 2e67 6974  tegration](/.git
+00008f90: 6875 622f 6173 7365 7473 2f61 6765 6e74  hub/assets/agent
+00008fa0: 2e67 6966 290a 0a3c 6272 2f3e 0a0a 3c21  .gif)..<br/>..<!
+00008fb0: 2d2d 2068 6174 6368 2d66 616e 6379 2d70  -- hatch-fancy-p
+00008fc0: 7970 692d 7265 6164 6d65 206d 6574 6120  ypi-readme meta 
+00008fd0: 7374 6172 7420 2d2d 3e0a 0a23 2320 f09f  start -->..## ..
+00008fe0: 9a80 2044 6570 6c6f 7969 6e67 206d 6f64  .. Deploying mod
+00008ff0: 656c 7320 746f 2070 726f 6475 6374 696f  els to productio
+00009000: 6e0a 0a54 6865 7265 2061 7265 2073 6576  n..There are sev
+00009010: 6572 616c 2077 6179 7320 746f 2064 6570  eral ways to dep
+00009020: 6c6f 7920 796f 7572 204c 4c4d 733a 0a0a  loy your LLMs:..
+00009030: 2323 2320 f09f 90b3 2044 6f63 6b65 7220  ### .... Docker 
+00009040: 636f 6e74 6169 6e65 720a 0a31 2e20 2a2a  container..1. **
+00009050: 4275 696c 6469 6e67 2061 2042 656e 746f  Building a Bento
+00009060: 2a2a 3a20 5769 7468 204f 7065 6e4c 4c4d  **: With OpenLLM
+00009070: 2c20 796f 7520 6361 6e20 6561 7369 6c79  , you can easily
+00009080: 2062 7569 6c64 2061 2042 656e 746f 2066   build a Bento f
+00009090: 6f72 2061 0a20 2020 7370 6563 6966 6963  or a.   specific
+000090a0: 206d 6f64 656c 2c20 6c69 6b65 2060 6d69   model, like `mi
+000090b0: 7374 7261 6c61 692f 4d69 7374 7261 6c2d  stralai/Mistral-
+000090c0: 3742 2d49 6e73 7472 7563 742d 7630 2e31  7B-Instruct-v0.1
+000090d0: 602c 2075 7369 6e67 2074 6865 2060 6275  `, using the `bu
+000090e0: 696c 6460 2063 6f6d 6d61 6e64 2e3a 0a0a  ild` command.:..
+000090f0: 2020 2060 6060 6261 7368 0a20 2020 6f70     ```bash.   op
+00009100: 656e 6c6c 6d20 6275 696c 6420 6d69 7374  enllm build mist
+00009110: 7261 6c61 692f 4d69 7374 7261 6c2d 3742  ralai/Mistral-7B
+00009120: 2d49 6e73 7472 7563 742d 7630 2e31 0a20  -Instruct-v0.1. 
+00009130: 2020 6060 600a 0a20 2020 410a 2020 205b    ```..   A.   [
+00009140: 4265 6e74 6f5d 2868 7474 7073 3a2f 2f64  Bento](https://d
+00009150: 6f63 732e 6265 6e74 6f6d 6c2e 636f 6d2f  ocs.bentoml.com/
+00009160: 656e 2f6c 6174 6573 742f 636f 6e63 6570  en/latest/concep
+00009170: 7473 2f62 656e 746f 2e68 746d 6c23 7768  ts/bento.html#wh
+00009180: 6174 2d69 732d 612d 6265 6e74 6f29 2c0a  at-is-a-bento),.
+00009190: 2020 2069 6e20 4265 6e74 6f4d 4c2c 2069     in BentoML, i
+000091a0: 7320 7468 6520 756e 6974 206f 6620 6469  s the unit of di
+000091b0: 7374 7269 6275 7469 6f6e 2e20 4974 2070  stribution. It p
+000091c0: 6163 6b61 6765 7320 796f 7572 2070 726f  ackages your pro
+000091d0: 6772 616d 2773 2073 6f75 7263 650a 2020  gram's source.  
+000091e0: 2063 6f64 652c 206d 6f64 656c 732c 2066   code, models, f
+000091f0: 696c 6573 2c20 6172 7465 6661 6374 732c  iles, artefacts,
+00009200: 2061 6e64 2064 6570 656e 6465 6e63 6965   and dependencie
+00009210: 732e 0a0a 322e 202a 2a43 6f6e 7461 696e  s...2. **Contain
+00009220: 6572 697a 6520 796f 7572 2042 656e 746f  erize your Bento
+00009230: 2a2a 0a0a 2020 2060 6060 6261 7368 0a20  **..   ```bash. 
+00009240: 2020 6265 6e74 6f6d 6c20 636f 6e74 6169    bentoml contai
+00009250: 6e65 7269 7a65 203c 6e61 6d65 3a76 6572  nerize <name:ver
+00009260: 7369 6f6e 3e0a 2020 2060 6060 0a0a 2020  sion>.   ```..  
+00009270: 2054 6869 7320 6765 6e65 7261 7465 7320   This generates 
+00009280: 6120 4f43 492d 636f 6d70 6174 6962 6c65  a OCI-compatible
+00009290: 2064 6f63 6b65 7220 696d 6167 6520 7468   docker image th
+000092a0: 6174 2063 616e 2062 6520 6465 706c 6f79  at can be deploy
+000092b0: 6564 2061 6e79 7768 6572 650a 2020 2064  ed anywhere.   d
+000092c0: 6f63 6b65 7220 7275 6e73 2e20 466f 7220  ocker runs. For 
+000092d0: 6265 7374 2073 6361 6c61 6269 6c69 7479  best scalability
+000092e0: 2061 6e64 2072 656c 6961 6269 6c69 7479   and reliability
+000092f0: 206f 6620 796f 7572 204c 4c4d 2073 6572   of your LLM ser
+00009300: 7669 6365 2069 6e0a 2020 2070 726f 6475  vice in.   produ
+00009310: 6374 696f 6e2c 2077 6520 7265 636f 6d6d  ction, we recomm
+00009320: 656e 6420 6465 706c 6f79 2077 6974 6820  end deploy with 
+00009330: 4265 6e74 6f43 6c6f 7564 e380 820a 0a23  BentoCloud.....#
+00009340: 2323 20e2 9881 efb8 8f20 4265 6e74 6f43  ## ...... BentoC
+00009350: 6c6f 7564 0a0a 4465 706c 6f79 204f 7065  loud..Deploy Ope
+00009360: 6e4c 4c4d 2077 6974 6820 5b42 656e 746f  nLLM with [Bento
+00009370: 436c 6f75 645d 2868 7474 7073 3a2f 2f77  Cloud](https://w
+00009380: 7777 2e62 656e 746f 6d6c 2e63 6f6d 2f29  ww.bentoml.com/)
+00009390: 2c20 7468 6520 696e 6665 7265 6e63 6520  , the inference 
+000093a0: 706c 6174 666f 726d 0a66 6f72 2066 6173  platform.for fas
+000093b0: 7420 6d6f 7669 6e67 2041 4920 7465 616d  t moving AI team
+000093c0: 732e 0a0a 312e 202a 2a43 7265 6174 6520  s...1. **Create 
+000093d0: 6120 4265 6e74 6f43 6c6f 7564 2061 6363  a BentoCloud acc
+000093e0: 6f75 6e74 3a2a 2a20 5b73 6967 6e20 7570  ount:** [sign up
+000093f0: 2068 6572 655d 2868 7474 7073 3a2f 2f62   here](https://b
+00009400: 656e 746f 6d6c 2e63 6f6d 2f29 0a0a 322e  entoml.com/)..2.
+00009410: 202a 2a4c 6f67 2069 6e74 6f20 796f 7572   **Log into your
+00009420: 2042 656e 746f 436c 6f75 6420 6163 636f   BentoCloud acco
+00009430: 756e 743a 2a2a 0a0a 2020 2060 6060 6261  unt:**..   ```ba
+00009440: 7368 0a20 2020 6265 6e74 6f6d 6c20 636c  sh.   bentoml cl
+00009450: 6f75 6420 6c6f 6769 6e20 2d2d 6170 692d  oud login --api-
+00009460: 746f 6b65 6e20 3c79 6f75 722d 6170 692d  token <your-api-
+00009470: 746f 6b65 6e3e 202d 2d65 6e64 706f 696e  token> --endpoin
+00009480: 7420 3c62 656e 746f 2d63 6c6f 7564 2d65  t <bento-cloud-e
+00009490: 6e64 706f 696e 743e 0a20 2020 6060 600a  ndpoint>.   ```.
+000094a0: 0a3e 205b 214e 4f54 455d 0a3e 2052 6570  .> [!NOTE].> Rep
+000094b0: 6c61 6365 2060 3c79 6f75 722d 6170 692d  lace `<your-api-
+000094c0: 746f 6b65 6e3e 6020 616e 6420 603c 6265  token>` and `<be
+000094d0: 6e74 6f2d 636c 6f75 642d 656e 6470 6f69  nto-cloud-endpoi
+000094e0: 6e74 3e60 2077 6974 6820 796f 7572 0a3e  nt>` with your.>
+000094f0: 2073 7065 6369 6669 6320 4150 4920 746f   specific API to
+00009500: 6b65 6e20 616e 6420 7468 6520 4265 6e74  ken and the Bent
+00009510: 6f43 6c6f 7564 2065 6e64 706f 696e 7420  oCloud endpoint 
+00009520: 7265 7370 6563 7469 7665 6c79 2e0a 0a33  respectively...3
+00009530: 2e20 2a2a 4275 6c64 696e 6720 6120 4265  . **Bulding a Be
+00009540: 6e74 6f2a 2a3a 2057 6974 6820 4f70 656e  nto**: With Open
+00009550: 4c4c 4d2c 2079 6f75 2063 616e 2065 6173  LLM, you can eas
+00009560: 696c 7920 6275 696c 6420 6120 4265 6e74  ily build a Bent
+00009570: 6f20 666f 7220 610a 2020 2073 7065 6369  o for a.   speci
+00009580: 6669 6320 6d6f 6465 6c2c 2073 7563 6820  fic model, such 
+00009590: 6173 2060 6d69 7374 7261 6c61 692f 4d69  as `mistralai/Mi
+000095a0: 7374 7261 6c2d 3742 2d49 6e73 7472 7563  stral-7B-Instruc
+000095b0: 742d 7630 2e31 603a 0a0a 2020 2060 6060  t-v0.1`:..   ```
+000095c0: 6261 7368 0a20 2020 6f70 656e 6c6c 6d20  bash.   openllm 
+000095d0: 6275 696c 6420 6d69 7374 7261 6c61 692f  build mistralai/
+000095e0: 4d69 7374 7261 6c2d 3742 2d49 6e73 7472  Mistral-7B-Instr
+000095f0: 7563 742d 7630 2e31 0a20 2020 6060 600a  uct-v0.1.   ```.
+00009600: 0a34 2e20 2a2a 5075 7368 696e 6720 6120  .4. **Pushing a 
+00009610: 4265 6e74 6f2a 2a3a 2050 7573 6820 796f  Bento**: Push yo
+00009620: 7572 2066 7265 7368 6c79 2d62 7569 6c74  ur freshly-built
+00009630: 2042 656e 746f 2073 6572 7669 6365 2074   Bento service t
+00009640: 6f20 4265 6e74 6f43 6c6f 7564 2076 6961  o BentoCloud via
+00009650: 0a20 2020 7468 6520 6070 7573 6860 2063  .   the `push` c
+00009660: 6f6d 6d61 6e64 3a0a 0a20 2020 6060 6062  ommand:..   ```b
+00009670: 6173 680a 2020 2062 656e 746f 6d6c 2070  ash.   bentoml p
+00009680: 7573 6820 3c6e 616d 653a 7665 7273 696f  ush <name:versio
+00009690: 6e3e 0a20 2020 6060 600a 0a35 2e20 2a2a  n>.   ```..5. **
+000096a0: 4465 706c 6f79 696e 6720 6120 4265 6e74  Deploying a Bent
+000096b0: 6f2a 2a3a 2044 6570 6c6f 7920 796f 7572  o**: Deploy your
+000096c0: 204c 4c4d 7320 746f 2042 656e 746f 436c   LLMs to BentoCl
+000096d0: 6f75 6420 7769 7468 2061 2073 696e 676c  oud with a singl
+000096e0: 650a 2020 2060 6265 6e74 6f6d 6c20 6465  e.   `bentoml de
+000096f0: 706c 6f79 6d65 6e74 2063 7265 6174 6560  ployment create`
+00009700: 2063 6f6d 6d61 6e64 2066 6f6c 6c6f 7769   command followi
+00009710: 6e67 2074 6865 0a20 2020 5b64 6570 6c6f  ng the.   [deplo
+00009720: 796d 656e 7420 696e 7374 7275 6374 696f  yment instructio
+00009730: 6e73 5d28 6874 7470 733a 2f2f 646f 6373  ns](https://docs
+00009740: 2e62 656e 746f 6d6c 2e63 6f6d 2f65 6e2f  .bentoml.com/en/
+00009750: 6c61 7465 7374 2f72 6566 6572 656e 6365  latest/reference
+00009760: 2f63 6c69 2e68 746d 6c23 6265 6e74 6f6d  /cli.html#bentom
+00009770: 6c2d 6465 706c 6f79 6d65 6e74 2d63 7265  l-deployment-cre
+00009780: 6174 6529 2e0a 0a23 2320 f09f 91a5 2043  ate)...## .... C
+00009790: 6f6d 6d75 6e69 7479 0a0a 456e 6761 6765  ommunity..Engage
+000097a0: 2077 6974 6820 6c69 6b65 2d6d 696e 6465   with like-minde
+000097b0: 6420 696e 6469 7669 6475 616c 7320 7061  d individuals pa
+000097c0: 7373 696f 6e61 7465 2061 626f 7574 204c  ssionate about L
+000097d0: 4c4d 732c 2041 492c 2061 6e64 206d 6f72  LMs, AI, and mor
+000097e0: 6520 6f6e 206f 7572 0a5b 4469 7363 6f72  e on our.[Discor
+000097f0: 645d 2868 7474 7073 3a2f 2f6c 2e62 656e  d](https://l.ben
+00009800: 746f 6d6c 2e63 6f6d 2f6a 6f69 6e2d 6f70  toml.com/join-op
+00009810: 656e 6c6c 6d2d 6469 7363 6f72 6429 210a  enllm-discord)!.
+00009820: 0a4f 7065 6e4c 4c4d 2069 7320 6163 7469  .OpenLLM is acti
+00009830: 7665 6c79 206d 6169 6e74 6169 6e65 6420  vely maintained 
+00009840: 6279 2074 6865 2042 656e 746f 4d4c 2074  by the BentoML t
+00009850: 6561 6d2e 2046 6565 6c20 6672 6565 2074  eam. Feel free t
+00009860: 6f20 7265 6163 6820 6f75 7420 616e 640a  o reach out and.
+00009870: 6a6f 696e 2075 7320 696e 206f 7572 2070  join us in our p
+00009880: 7572 7375 6974 2074 6f20 6d61 6b65 204c  ursuit to make L
+00009890: 4c4d 7320 6d6f 7265 2061 6363 6573 7369  LMs more accessi
+000098a0: 626c 6520 616e 6420 6561 7379 2074 6f20  ble and easy to 
+000098b0: 7573 6520 f09f 9189 0a5b 4a6f 696e 206f  use .....[Join o
+000098c0: 7572 2053 6c61 636b 2063 6f6d 6d75 6e69  ur Slack communi
+000098d0: 7479 215d 2868 7474 7073 3a2f 2f6c 2e62  ty!](https://l.b
+000098e0: 656e 746f 6d6c 2e63 6f6d 2f6a 6f69 6e2d  entoml.com/join-
+000098f0: 736c 6163 6b29 0a0a 2323 20f0 9f8e 8120  slack)..## .... 
+00009900: 436f 6e74 7269 6275 7469 6e67 0a0a 5765  Contributing..We
+00009910: 2077 656c 636f 6d65 2063 6f6e 7472 6962   welcome contrib
+00009920: 7574 696f 6e73 2120 4966 2079 6f75 2772  utions! If you'r
+00009930: 6520 696e 7465 7265 7374 6564 2069 6e20  e interested in 
+00009940: 656e 6861 6e63 696e 6720 4f70 656e 4c4c  enhancing OpenLL
+00009950: 4d27 730a 6361 7061 6269 6c69 7469 6573  M's.capabilities
+00009960: 206f 7220 6861 7665 2061 6e79 2071 7565   or have any que
+00009970: 7374 696f 6e73 2c20 646f 6e27 7420 6865  stions, don't he
+00009980: 7369 7461 7465 2074 6f20 7265 6163 6820  sitate to reach 
+00009990: 6f75 7420 696e 206f 7572 0a5b 6469 7363  out in our.[disc
+000099a0: 6f72 6420 6368 616e 6e65 6c5d 2868 7474  ord channel](htt
+000099b0: 7073 3a2f 2f6c 2e62 656e 746f 6d6c 2e63  ps://l.bentoml.c
+000099c0: 6f6d 2f6a 6f69 6e2d 6f70 656e 6c6c 6d2d  om/join-openllm-
+000099d0: 6469 7363 6f72 6429 2e0a 0a43 6865 636b  discord)...Check
+000099e0: 6f75 7420 6f75 720a 5b44 6576 656c 6f70  out our.[Develop
+000099f0: 6572 2047 7569 6465 5d28 6874 7470 733a  er Guide](https:
+00009a00: 2f2f 6769 7468 7562 2e63 6f6d 2f62 656e  //github.com/ben
+00009a10: 746f 6d6c 2f4f 7065 6e4c 4c4d 2f62 6c6f  toml/OpenLLM/blo
+00009a20: 622f 6d61 696e 2f44 4556 454c 4f50 4d45  b/main/DEVELOPME
+00009a30: 4e54 2e6d 6429 0a69 6620 796f 7520 7769  NT.md).if you wi
+00009a40: 7368 2074 6f20 636f 6e74 7269 6275 7465  sh to contribute
+00009a50: 2074 6f20 4f70 656e 4c4c 4d27 7320 636f   to OpenLLM's co
+00009a60: 6465 6261 7365 2e0a 0a23 2320 f09f 8d87  debase...## ....
+00009a70: 2054 656c 656d 6574 7279 0a0a 4f70 656e   Telemetry..Open
+00009a80: 4c4c 4d20 636f 6c6c 6563 7473 2075 7361  LLM collects usa
+00009a90: 6765 2064 6174 6120 746f 2065 6e68 616e  ge data to enhan
+00009aa0: 6365 2075 7365 7220 6578 7065 7269 656e  ce user experien
+00009ab0: 6365 2061 6e64 2069 6d70 726f 7665 2074  ce and improve t
+00009ac0: 6865 2070 726f 6475 6374 2e0a 5765 206f  he product..We o
+00009ad0: 6e6c 7920 7265 706f 7274 204f 7065 6e4c  nly report OpenL
+00009ae0: 4c4d 2773 2069 6e74 6572 6e61 6c20 4150  LM's internal AP
+00009af0: 4920 6361 6c6c 7320 616e 6420 656e 7375  I calls and ensu
+00009b00: 7265 206d 6178 696d 756d 2070 7269 7661  re maximum priva
+00009b10: 6379 2062 790a 6578 636c 7564 696e 6720  cy by.excluding 
+00009b20: 7365 6e73 6974 6976 6520 696e 666f 726d  sensitive inform
+00009b30: 6174 696f 6e2e 2057 6520 7769 6c6c 206e  ation. We will n
+00009b40: 6576 6572 2063 6f6c 6c65 6374 2075 7365  ever collect use
+00009b50: 7220 636f 6465 2c20 6d6f 6465 6c20 6461  r code, model da
+00009b60: 7461 2c20 6f72 0a73 7461 636b 2074 7261  ta, or.stack tra
+00009b70: 6365 732e 2046 6f72 2075 7361 6765 2074  ces. For usage t
+00009b80: 7261 636b 696e 672c 2063 6865 636b 206f  racking, check o
+00009b90: 7574 2074 6865 0a5b 636f 6465 5d28 6874  ut the.[code](ht
+00009ba0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00009bb0: 2f62 656e 746f 6d6c 2f4f 7065 6e4c 4c4d  /bentoml/OpenLLM
+00009bc0: 2f62 6c6f 622f 6d61 696e 2f6f 7065 6e6c  /blob/main/openl
+00009bd0: 6c6d 2d63 6f72 652f 7372 632f 6f70 656e  lm-core/src/open
+00009be0: 6c6c 6d5f 636f 7265 2f75 7469 6c73 2f61  llm_core/utils/a
+00009bf0: 6e61 6c79 7469 6373 2e70 7929 2e0a 0a59  nalytics.py)...Y
+00009c00: 6f75 2063 616e 206f 7074 206f 7574 206f  ou can opt out o
+00009c10: 6620 7573 6167 6520 7472 6163 6b69 6e67  f usage tracking
+00009c20: 2062 7920 7573 696e 6720 7468 6520 602d   by using the `-
+00009c30: 2d64 6f2d 6e6f 742d 7472 6163 6b60 2043  -do-not-track` C
+00009c40: 4c49 206f 7074 696f 6e3a 0a0a 6060 6062  LI option:..```b
+00009c50: 6173 680a 6f70 656e 6c6c 6d20 5b63 6f6d  ash.openllm [com
+00009c60: 6d61 6e64 5d20 2d2d 646f 2d6e 6f74 2d74  mand] --do-not-t
+00009c70: 7261 636b 0a60 6060 0a0a 4f72 2062 7920  rack.```..Or by 
+00009c80: 7365 7474 696e 6720 7468 6520 656e 7669  setting the envi
+00009c90: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00009ca0: 2060 4f50 454e 4c4c 4d5f 444f 5f4e 4f54   `OPENLLM_DO_NOT
+00009cb0: 5f54 5241 434b 3d54 7275 6560 3a0a 0a60  _TRACK=True`:..`
+00009cc0: 6060 6261 7368 0a65 7870 6f72 7420 4f50  ``bash.export OP
+00009cd0: 454e 4c4c 4d5f 444f 5f4e 4f54 5f54 5241  ENLLM_DO_NOT_TRA
+00009ce0: 434b 3d54 7275 650a 6060 600a 0a23 2320  CK=True.```..## 
+00009cf0: f09f 9394 2043 6974 6174 696f 6e0a 0a49  .... Citation..I
+00009d00: 6620 796f 7520 7573 6520 4f70 656e 4c4c  f you use OpenLL
+00009d10: 4d20 696e 2079 6f75 7220 7265 7365 6172  M in your resear
+00009d20: 6368 2c20 7765 2070 726f 7669 6465 2061  ch, we provide a
+00009d30: 205b 6369 7461 7469 6f6e 5d28 2e2f 4349   [citation](./CI
+00009d40: 5441 5449 4f4e 2e63 6666 2920 746f 0a75  TATION.cff) to.u
+00009d50: 7365 3a0a 0a60 6060 6269 6274 6578 0a40  se:..```bibtex.@
+00009d60: 736f 6674 7761 7265 7b50 6861 6d5f 4f70  software{Pham_Op
+00009d70: 656e 4c4c 4d5f 4f70 6572 6174 696e 675f  enLLM_Operating_
+00009d80: 4c4c 4d73 5f32 3032 332c 0a61 7574 686f  LLMs_2023,.autho
+00009d90: 7220 3d20 7b50 6861 6d2c 2041 6172 6f6e  r = {Pham, Aaron
+00009da0: 2061 6e64 2059 616e 672c 2043 6861 6f79   and Yang, Chaoy
+00009db0: 7520 616e 6420 5368 656e 672c 2053 6561  u and Sheng, Sea
+00009dc0: 6e20 616e 6420 205a 6861 6f2c 2053 6865  n and  Zhao, She
+00009dd0: 6e79 616e 6720 616e 6420 4c65 652c 2053  nyang and Lee, S
+00009de0: 6175 796f 6e20 616e 6420 4a69 616e 672c  auyon and Jiang,
+00009df0: 2042 6f20 616e 6420 446f 6e67 2c20 466f   Bo and Dong, Fo
+00009e00: 6720 616e 6420 4775 616e 2c20 5869 7065  g and Guan, Xipe
+00009e10: 6e67 2061 6e64 204d 696e 672c 2046 726f  ng and Ming, Fro
+00009e20: 7374 7d2c 0a6c 6963 656e 7365 203d 207b  st},.license = {
+00009e30: 4170 6163 6865 2d32 2e30 7d2c 0a6d 6f6e  Apache-2.0},.mon
+00009e40: 7468 203d 206a 756e 2c0a 7469 746c 6520  th = jun,.title 
+00009e50: 3d20 7b7b 4f70 656e 4c4c 4d3a 204f 7065  = {{OpenLLM: Ope
+00009e60: 7261 7469 6e67 204c 4c4d 7320 696e 2070  rating LLMs in p
+00009e70: 726f 6475 6374 696f 6e7d 7d2c 0a75 726c  roduction}},.url
+00009e80: 203d 207b 6874 7470 733a 2f2f 6769 7468   = {https://gith
+00009e90: 7562 2e63 6f6d 2f62 656e 746f 6d6c 2f4f  ub.com/bentoml/O
+00009ea0: 7065 6e4c 4c4d 7d2c 0a79 6561 7220 3d20  penLLM},.year = 
+00009eb0: 7b32 3032 337d 0a7d 0a60 6060 0a0a 3c21  {2023}.}.```..<!
+00009ec0: 2d2d 2068 6174 6368 2d66 616e 6379 2d70  -- hatch-fancy-p
+00009ed0: 7970 692d 7265 6164 6d65 206d 6574 6120  ypi-readme meta 
+00009ee0: 7374 6f70 202d 2d3e 0a                   stop -->.
```

