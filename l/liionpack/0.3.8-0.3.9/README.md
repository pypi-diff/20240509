# Comparing `tmp/liionpack-0.3.8.tar.gz` & `tmp/liionpack-0.3.9.tar.gz`

## Comparing `liionpack-0.3.8.tar` & `liionpack-0.3.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.8/.git-blame-ignore-revs
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 liionpack-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.8/.readthedocs.yaml
--rw-r--r--   0        0        0     5960 2020-02-02 00:00:00.000000 liionpack-0.3.8/CHANGELOG.md
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.8/asv.conf.json
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 liionpack-0.3.8/environment.yml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.8/mkdocs.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/codecov.yml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/workflows/periodic_benchmarks.yml
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/workflows/run_benchmarks_over_history.yml
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 liionpack-0.3.8/.github/workflows/test_on_push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.8/benchmarks/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.8/benchmarks/benchmarks.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/about.md
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/conduct.md
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/contributing.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/index.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/install.md
--rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/liionpack.png
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/mathjax-config.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/reference.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/requirements.txt
--rw-r--r--   0        0        0   428208 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/01 Getting Started.ipynb
--rw-r--r--   0        0        0   258064 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/02 Using inputs.ipynb
--rw-r--r--   0        0        0   129217 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/03 Experiments.ipynb
--rw-r--r--   0        0        0   320758 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/04 Initial SoC.ipynb
--rw-r--r--   0        0        0  1446747 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/05 Drive cycles.ipynb
--rw-r--r--   0        0        0   894028 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/06 Changing a model.ipynb
--rw-r--r--   0        0        0   131502 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/07 Visualizing larger packs.ipynb
--rw-r--r--   0        0        0   986044 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/08 SEI degradation model.ipynb
--rw-r--r--   0        0        0   322325 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/examples/09 Terminal locations.ipynb
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.8/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/basic_16p2s.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/big_circuit.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/different_initial_soc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/draw_circuit.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/draw_terminals.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/drive_cycle.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/drive_cycle_comparison.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/load_4p1s.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/mixed_capacity.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/mixed_terminals.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/paper_example.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/save_output.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/step_external_variable.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.8/examples/thermal_external.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/_version.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/definitions.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/logger.py
--rw-r--r--   0        0        0    25028 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/netlist_utils.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/plots.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/protocols.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/sim_utils.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/simulations.py
--rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/solver_utils.py
--rw-r--r--   0        0        0    18989 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/solvers.py
--rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/version.pyi
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/circuits/4p1s.asc
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/circuits/4p1s.cir
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.8/liionpack/circuits/4p1s.txt
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper.bib
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper.md
--rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper_figures/Figure_0.png
--rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper_figures/Figure_1.png
--rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper_figures/Figure_2.png
--rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.8/paper/paper_figures/Figure_3.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/integration/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/integration/test_1p1s.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/integration/test_all_solvers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_logger.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_netlist_utils.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_notebooks.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_plots.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_protocols.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_sim_utils.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_simulations.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_solver_utils.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_solvers.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.8/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 liionpack-0.3.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.8/LICENSE
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.8/README.md
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 liionpack-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 liionpack-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.9/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liionpack-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 liionpack-0.3.9/CHANGELOG.md
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.9/asv.conf.json
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 liionpack-0.3.9/environment.yml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.9/mkdocs.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/codecov.yml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/workflows/periodic_benchmarks.yml
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/workflows/run_benchmarks_over_history.yml
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 liionpack-0.3.9/.github/workflows/test_on_push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.9/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.9/benchmarks/benchmarks.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/about.md
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/conduct.md
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/contributing.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/index.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/install.md
+-rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/liionpack.png
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/mathjax-config.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/reference.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/requirements.txt
+-rw-r--r--   0        0        0   428202 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/01 Getting Started.ipynb
+-rw-r--r--   0        0        0   258085 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/02 Using inputs.ipynb
+-rw-r--r--   0        0        0   129169 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/03 Experiments.ipynb
+-rw-r--r--   0        0        0   320747 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/04 Initial SoC.ipynb
+-rw-r--r--   0        0        0  1446768 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/05 Drive cycles.ipynb
+-rw-r--r--   0        0        0   894049 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/06 Changing a model.ipynb
+-rw-r--r--   0        0        0   131500 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/07 Visualizing larger packs.ipynb
+-rw-r--r--   0        0        0   986227 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/08 SEI degradation model.ipynb
+-rw-r--r--   0        0        0   322315 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/examples/09 Terminal locations.ipynb
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.9/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/basic_16p2s.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/big_circuit.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/different_initial_soc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/draw_circuit.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/draw_terminals.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/drive_cycle.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/drive_cycle_comparison.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/load_4p1s.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/mixed_capacity.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/mixed_terminals.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/paper_example.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/save_output.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/step_external_variable.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.9/examples/thermal_external.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/_version.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/definitions.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/logger.py
+-rw-r--r--   0        0        0    25028 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/netlist_utils.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/plots.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/protocols.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/sim_utils.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/simulations.py
+-rw-r--r--   0        0        0    16008 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/solver_utils.py
+-rw-r--r--   0        0        0    18997 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/solvers.py
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/version.pyi
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/circuits/4p1s.asc
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/circuits/4p1s.cir
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.9/liionpack/circuits/4p1s.txt
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper.bib
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper.md
+-rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper_figures/Figure_0.png
+-rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper_figures/Figure_1.png
+-rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper_figures/Figure_2.png
+-rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.9/paper/paper_figures/Figure_3.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/integration/test_1p1s.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/integration/test_all_solvers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_logger.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_netlist_utils.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_notebooks.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_plots.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_protocols.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_sim_utils.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_simulations.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_solver_utils.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_solvers.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.9/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 liionpack-0.3.9/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.9/README.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 liionpack-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 liionpack-0.3.9/PKG-INFO
```

### Comparing `liionpack-0.3.8/CHANGELOG.md` & `liionpack-0.3.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,28 @@
 
 - ([#PR](link))
 
 ## Breaking changes
 
 - ([#PR](link))
 
+# [v0.3.9](https://github.com/pybamm-team/liionpack/tree/v0.3.9) - 2024-04-26
+
+## Features
+
+- Update PyBaMM to 24.1 ([#293](https://github.com/pybamm-team/liionpack/pull/293))
+
+## Bug fixes
+
+- Fix event reporting ([#288](https://github.com/pybamm-team/liionpack/pull/288))
+- Fix experiments with small time steps ([#289](https://github.com/pybamm-team/liionpack/pull/289))
+- Remove the Jax install from CI ([#287](https://github.com/pybamm-team/liionpack/pull/287))
+- ([#PR](link))
+
+
 # [v0.3.8](https://github.com/pybamm-team/liionpack/tree/v0.3.8) - 2024-01-20
 
 ## Bug fixes
 
 - Update to PyBaMM 23.9
 
 # [v0.3.7](https://github.com/pybamm-team/liionpack/tree/v0.3.7) - 2023-07-05
```

### Comparing `liionpack-0.3.8/asv.conf.json` & `liionpack-0.3.9/asv.conf.json`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/environment.yml` & `liionpack-0.3.9/environment.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/mkdocs.yml` & `liionpack-0.3.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/ISSUE_TEMPLATE/bug_report.yml` & `liionpack-0.3.9/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/ISSUE_TEMPLATE/feature_request.yml` & `liionpack-0.3.9/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/workflows/periodic_benchmarks.yml` & `liionpack-0.3.9/.github/workflows/periodic_benchmarks.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/workflows/publish_pypi.yml` & `liionpack-0.3.9/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/workflows/run_benchmarks_over_history.yml` & `liionpack-0.3.9/.github/workflows/run_benchmarks_over_history.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.github/workflows/test_on_push.yml` & `liionpack-0.3.9/.github/workflows/test_on_push.yml`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,14 @@
           texlive-pictures
         sudo apt-get install ghostscript
 
     - name: Install liionpack and dependencies
       run: |
         python -m pip install --upgrade pip wheel coverage
         python -m pip install .
-        pybamm_install_jax
 
     - name: Run tests and generate coverage report
       run: |
         coverage run -m unittest -v
 
     - name: Build docs
       run: |
```

### Comparing `liionpack-0.3.8/benchmarks/benchmarks.py` & `liionpack-0.3.9/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/conduct.md` & `liionpack-0.3.9/docs/conduct.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/contributing.md` & `liionpack-0.3.9/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/index.md` & `liionpack-0.3.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/install.md` & `liionpack-0.3.9/docs/install.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/liionpack.png` & `liionpack-0.3.9/docs/liionpack.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/mathjax-config.js` & `liionpack-0.3.9/docs/mathjax-config.js`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/docs/examples/01 Getting Started.ipynb` & `liionpack-0.3.9/docs/examples/01 Getting Started.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981646825396826%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n'), (5, 'import "*

 * *            "pybamm')], delete: [6, 5, 2]}}, 26: {'source': {insert: [(5, '    "*

 * *            "initial_soc=0.5,\\n')], delete: [5]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -25,19 +25,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
-                "import pybamm\n",
-                "import numpy as np"
+                "import pybamm"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can create a pack definition in one of two ways: using an existing netlist or by specifying the number of batteries to connect in series and parallel."
@@ -470,15 +469,15 @@
             ],
             "source": [
                 "output = lp.solve(\n",
                 "    netlist=netlist,\n",
                 "    parameter_values=parameter_values,\n",
                 "    experiment=experiment,\n",
                 "    output_variables=output_variables,\n",
-                "    initial_soc=0.5\n",
+                "    initial_soc=0.5,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -578,15 +577,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `liionpack-0.3.8/docs/examples/02 Using inputs.ipynb` & `liionpack-0.3.9/docs/examples/02 Using inputs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976033834586466%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [2]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,15 +18,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import pybamm\n",
                 "import numpy as np"
             ]
         },
         {
@@ -336,13 +336,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/docs/examples/03 Experiments.ipynb` & `liionpack-0.3.9/docs/examples/03 Experiments.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971968694885361%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n'), (5, 'import "*

 * *            "pybamm')], delete: [7, 6, 5, 2]}}, 16: {'source': {insert: [(6, '    "*

 * *            "initial_soc=0.5,\\n')], delete: [6]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,20 +18,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
-                "import pybamm\n",
-                "import numpy as np\n",
-                "import matplotlib.pyplot as plt"
+                "import pybamm"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Set up the circuit"
@@ -221,15 +219,15 @@
             "source": [
                 "# Solve pack\n",
                 "output = lp.solve(\n",
                 "    netlist=netlist,\n",
                 "    parameter_values=parameter_values,\n",
                 "    experiment=experiment,\n",
                 "    output_variables=output_variables,\n",
-                "    initial_soc=0.5\n",
+                "    initial_soc=0.5,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
@@ -262,13 +260,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/docs/examples/04 Initial SoC.ipynb` & `liionpack-0.3.9/docs/examples/04 Initial SoC.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968982919254659%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n'), (5, 'import "*

 * *            "pybamm')], delete: [7, 6, 5, 2]}}, 22: {'source': ['lp.draw_circuit(\\n', '    "*

 * *            "netlist,\\n', '    dpi=100,\\n', ')']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,20 +18,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
-                "import pybamm\n",
-                "import numpy as np\n",
-                "import matplotlib.pyplot as plt"
+                "import pybamm"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Lets set up the most simple pack possible with one battery and very low busbar resistance to compare to a pure PyBaMM simulation"
@@ -292,15 +290,18 @@
                             "width": 143
                         }
                     },
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "lp.draw_circuit(netlist, dpi=100,)"
+                "lp.draw_circuit(\n",
+                "    netlist,\n",
+                "    dpi=100,\n",
+                ")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -312,13 +313,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/docs/examples/05 Drive cycles.ipynb` & `liionpack-0.3.9/docs/examples/05 Drive cycles.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996055226824457%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [2]}}, 15: "*

 * *            "{'source': {insert: [(0, 'I_mean = np.around(np.mean(drive_cycle[:, 1]), 3)\\n')], "*

 * *            'delete: [0]}}}'}*

```diff
@@ -30,15 +30,15 @@
                         "2024-01-20 12:56:13,672\tINFO util.py:159 -- Missing packages: ['ipywidgets']. Run `pip install -U ipywidgets`, then restart the notebook server for rich notebook output.\n"
                     ]
                 }
             ],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import pybamm\n",
                 "import numpy as np\n",
                 "import os\n",
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
@@ -249,15 +249,15 @@
                     },
                     "execution_count": 11,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "I_mean = np.around(np.mean(drive_cycle[:, 1]),3)\n",
+                "I_mean = np.around(np.mean(drive_cycle[:, 1]), 3)\n",
                 "I_mean"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `liionpack-0.3.8/docs/examples/06 Changing a model.ipynb` & `liionpack-0.3.9/docs/examples/06 Changing a model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976258116883117%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [2]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,15 +18,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import pybamm\n",
                 "import numpy as np"
             ]
         },
         {
@@ -505,13 +505,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/docs/examples/07 Visualizing larger packs.ipynb` & `liionpack-0.3.9/docs/examples/07 Visualizing larger packs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972303878553879%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [2]}}, 4: "*

 * *            '{\'source\': {insert: [(19, \'parameter_values.update({"Total heat transfer '*

 * *            'coefficient [W.m-2.K-1]": "[input]"})\\n\'), (31, \'    nproc=nproc,\\n\')], delete: '*

 * *            '[33, 21, 20, 19]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,15 +18,15 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import numpy as np\n",
                 "import os\n",
                 "import pybamm\n",
                 "\n",
                 "nproc = os.cpu_count()"
@@ -68,29 +68,27 @@
                 "        \"Discharge at 100 A for 10 minutes\",\n",
                 "    ],\n",
                 "    period=\"1 minute\",\n",
                 ")\n",
                 "\n",
                 "# Define the PyBaMM parameters\n",
                 "parameter_values = pybamm.ParameterValues(\"Chen2020\")\n",
-                "parameter_values.update(\n",
-                "    {\"Total heat transfer coefficient [W.m-2.K-1]\": \"[input]\"}\n",
-                ")\n",
+                "parameter_values.update({\"Total heat transfer coefficient [W.m-2.K-1]\": \"[input]\"})\n",
                 "htc = np.random.random(Nspm) * 50.0\n",
                 "inputs = {\"Total heat transfer coefficient [W.m-2.K-1]\": htc}\n",
                 "# Solve the pack\n",
                 "output = lp.solve(\n",
                 "    netlist=netlist,\n",
                 "    sim_func=lp.thermal_simulation,\n",
                 "    parameter_values=parameter_values,\n",
                 "    experiment=experiment,\n",
                 "    output_variables=output_variables,\n",
                 "    inputs=inputs,\n",
                 "    initial_soc=0.5,\n",
-                "    nproc=nproc\n",
+                "    nproc=nproc,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -152,13 +150,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/docs/examples/08 SEI degradation model.ipynb` & `liionpack-0.3.9/docs/examples/08 SEI degradation model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980000901875902%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [2]}}, 6: "*

 * *            "{'source': ['netlist = lp.setup_circuit(\\n', '    Np=Np, Ns=Ns, Rb=R_busbar, "*

 * *            "Rc=R_connection, Ri=Ri_init, V=OCV_init, I=I_mag\\n', ')']}, 8: {'source': {insert: "*

 * *            '[(1, \'    [\\n\'), (2, \'        "Charge at 15 A for 10 minutes",\\n\'), (3, '*

 * *            '\'        "Rest for 10 minutes",\\n\'), (4, \'        "Discharge at 15 A for 10 '*

 * *            'minutes",\\n\'), (5,  […]*

```diff
@@ -31,15 +31,15 @@
                         "2024-01-20 13:06:47,229\tINFO util.py:159 -- Missing packages: ['ipywidgets']. Run `pip install -U ipywidgets`, then restart the notebook server for rich notebook output.\n"
                     ]
                 }
             ],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import pybamm\n",
                 "import numpy as np"
             ]
         },
         {
@@ -78,15 +78,17 @@
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "acc2c154",
             "metadata": {},
             "outputs": [],
             "source": [
-                "netlist = lp.setup_circuit(Np=Np, Ns=Ns, Rb=R_busbar, Rc=R_connection, Ri=Ri_init, V=OCV_init, I=I_mag)"
+                "netlist = lp.setup_circuit(\n",
+                "    Np=Np, Ns=Ns, Rb=R_busbar, Rc=R_connection, Ri=Ri_init, V=OCV_init, I=I_mag\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fe389856",
             "metadata": {},
             "source": [
@@ -97,16 +99,23 @@
             "cell_type": "code",
             "execution_count": 4,
             "id": "119cdc36",
             "metadata": {},
             "outputs": [],
             "source": [
                 "experiment = pybamm.Experiment(\n",
-                "    [\"Charge at 15 A for 10 minutes\", \"Rest for 10 minutes\", \"Discharge at 15 A for 10 minutes\", \"Rest for 10 minutes\"]*100,\n",
-                "    period=\"30 seconds\",)"
+                "    [\n",
+                "        \"Charge at 15 A for 10 minutes\",\n",
+                "        \"Rest for 10 minutes\",\n",
+                "        \"Discharge at 15 A for 10 minutes\",\n",
+                "        \"Rest for 10 minutes\",\n",
+                "    ]\n",
+                "    * 100,\n",
+                "    period=\"30 seconds\",\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "263010f9-c7c3-4938-a5e4-29cd85e3f2a9",
             "metadata": {},
             "source": [
@@ -134,20 +143,20 @@
         {
             "cell_type": "code",
             "execution_count": 12,
             "id": "75a045d3",
             "metadata": {},
             "outputs": [],
             "source": [
-                "output_variables = [  \n",
-                "    'X-averaged positive total SEI thickness [m]',\n",
-                "    'X-averaged negative total SEI thickness [m]',\n",
-                "    'Loss of capacity to positive SEI [A.h]',\n",
-                "    'Loss of capacity to negative SEI [A.h]'\n",
-                "    ]"
+                "output_variables = [\n",
+                "    \"X-averaged positive total SEI thickness [m]\",\n",
+                "    \"X-averaged negative total SEI thickness [m]\",\n",
+                "    \"Loss of capacity to positive SEI [A.h]\",\n",
+                "    \"Loss of capacity to negative SEI [A.h]\",\n",
+                "]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "70b11507-4255-4463-bb70-ec613ac32578",
             "metadata": {},
             "source": [
@@ -339,16 +348,18 @@
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "7d8aa3b4",
             "metadata": {},
             "outputs": [],
             "source": [
-                "parameter_values.update({\"EC initial concentration in electrolyte [mol.m-3]\": \"[input]\"})\n",
-                "EC_conc=np.array([4000.0, 3500.0, 3000.0, 2500.0])\n",
+                "parameter_values.update(\n",
+                "    {\"EC initial concentration in electrolyte [mol.m-3]\": \"[input]\"}\n",
+                ")\n",
+                "EC_conc = np.array([4000.0, 3500.0, 3000.0, 2500.0])\n",
                 "inputs = {\"EC initial concentration in electrolyte [mol.m-3]\": EC_conc}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "24b3c1e5",
@@ -366,15 +377,15 @@
                 "output = lp.solve(\n",
                 "    netlist=netlist,\n",
                 "    parameter_values=parameter_values,\n",
                 "    experiment=experiment,\n",
                 "    sim_func=SEI_degradation,\n",
                 "    inputs=inputs,\n",
                 "    output_variables=output_variables,\n",
-                "    initial_soc=0.5\n",
+                "    initial_soc=0.5,\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 23,
             "id": "df81c6c2",
```

### Comparing `liionpack-0.3.8/docs/examples/09 Terminal locations.ipynb` & `liionpack-0.3.9/docs/examples/09 Terminal locations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972663139329806%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'except ModuleNotFoundError:\\n')], delete: [6, 2]}}, "*

 * *            '11: {\'source\': {insert: [(9, \'                "Discharge at 1 A for 1 '*

 * *            'minutes",\\n\'), (24, \'    plt.legend()\')], delete: [24, 9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.11.5'}}"}*

```diff
@@ -18,19 +18,18 @@
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "try:\n",
                 "    import liionpack as lp\n",
-                "except:\n",
+                "except ModuleNotFoundError:\n",
                 "    !pip install -q git+https://github.com/pybamm-team/liionpack.git@main\n",
                 "    import liionpack as lp\n",
                 "import pybamm\n",
-                "import numpy as np\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -199,30 +198,30 @@
                 "lines = [\"-\", \"--\", \"-.\", \":\", \".-\"]\n",
                 "with plt.rc_context(lp.lp_context()):\n",
                 "    fig, ax = plt.subplots(1, 1, figsize=(10, 10))\n",
                 "    for i, netlist in enumerate(netlists):\n",
                 "        param = pybamm.ParameterValues(\"Chen2020\")\n",
                 "        experiment = pybamm.Experiment(\n",
                 "            [\n",
-                "                f\"Discharge at 1 A for 1 minutes\",\n",
+                "                \"Discharge at 1 A for 1 minutes\",\n",
                 "            ],\n",
                 "            period=\"10 seconds\",\n",
                 "        )\n",
                 "        # Solve pack\n",
                 "        output = lp.solve(\n",
                 "            netlist=netlist,\n",
                 "            parameter_values=param,\n",
                 "            experiment=experiment,\n",
                 "            output_variables=None,\n",
                 "            initial_soc=0.5,\n",
                 "        )\n",
                 "        plt.plot(range(7), output[\"Cell current [A]\"][-1, :], lines[i], label=labels[i])\n",
                 "    ax.set_xlabel(\"Node\")\n",
                 "    ax.set_ylabel(\"Cell current [A]\")\n",
-                "    plt.legend()\n"
+                "    plt.legend()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
@@ -234,13 +233,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.3"
+            "version": "3.11.5"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `liionpack-0.3.8/examples/basic_16p2s.py` & `liionpack-0.3.9/examples/basic_16p2s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/big_circuit.py` & `liionpack-0.3.9/examples/big_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/different_initial_soc.py` & `liionpack-0.3.9/examples/different_initial_soc.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/draw_circuit.py` & `liionpack-0.3.9/examples/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/draw_terminals.py` & `liionpack-0.3.9/examples/draw_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/drive_cycle.py` & `liionpack-0.3.9/examples/drive_cycle.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/drive_cycle_comparison.py` & `liionpack-0.3.9/examples/drive_cycle_comparison.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/load_4p1s.py` & `liionpack-0.3.9/examples/load_4p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/mixed_capacity.py` & `liionpack-0.3.9/examples/mixed_capacity.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/mixed_terminals.py` & `liionpack-0.3.9/examples/mixed_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/paper_example.py` & `liionpack-0.3.9/examples/paper_example.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/save_output.py` & `liionpack-0.3.9/examples/save_output.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/step_external_variable.py` & `liionpack-0.3.9/examples/step_external_variable.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/examples/thermal_external.py` & `liionpack-0.3.9/examples/thermal_external.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/__init__.py` & `liionpack-0.3.9/liionpack/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 # liionpack
 
 liionpack is a tool for simulating battery packs with pybamm. It can design the
 pack with a combination of batteries connected in series and parallel or can
 read a netlist.
 """
+
 from .simulations import basic_simulation
 from .simulations import thermal_simulation
 from .simulations import thermal_external
 from .utils import interp_current
 from .utils import build_inputs_dict
 from .utils import add_events_to_model
 from .utils import save_to_csv
```

### Comparing `liionpack-0.3.8/liionpack/logger.py` & `liionpack-0.3.9/liionpack/logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/netlist_utils.py` & `liionpack-0.3.9/liionpack/netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/plots.py` & `liionpack-0.3.9/liionpack/plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/sim_utils.py` & `liionpack-0.3.9/liionpack/sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/simulations.py` & `liionpack-0.3.9/liionpack/simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/solver_utils.py` & `liionpack-0.3.9/liionpack/solver_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
 
     # Look for events in model variables and create a function to evaluate them
     all_vars = sorted(sim.model.variables.keys())
     event_vars = [v for v in all_vars if "Event" in v]
     if len(event_vars) > 0:
         # Variables function for parallel evaluation
         casadi_objs = sim.built_model.export_casadi_objects(
-            variable_names=variable_names, input_parameter_order=ip_order
+            variable_names=event_vars, input_parameter_order=ip_order
         )
         events = casadi_objs["variables"]
         t, x, z, p = (
             casadi_objs["t"],
             casadi_objs["x"],
             casadi_objs["z"],
             casadi_objs["inputs"],
```

### Comparing `liionpack-0.3.8/liionpack/solvers.py` & `liionpack-0.3.9/liionpack/solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
             mapped = False
         self.Nspm = Nspm
         # Set up simulation
         self.parameter_values = parameter_values
         if initial_soc is not None:
             if (
                 (type(initial_soc) in [float, int])
-                or (type(initial_soc) is list and len(initial_soc) == 1)
-                or (type(initial_soc) is np.ndarray and len(initial_soc) == 1)
+                or (isinstance(initial_soc, list) and len(initial_soc) == 1)
+                or (isinstance(initial_soc, np.ndarray) and len(initial_soc) == 1)
             ):
                 _, _ = lp.update_init_conc(parameter_values, initial_soc, update=True)
             else:
                 lp.logger.warning(
                     "Using a list or an array of initial_soc "
                     + "is not supported, please set the initial "
                     + "concentrations via inputs"
```

### Comparing `liionpack-0.3.8/liionpack/utils.py` & `liionpack-0.3.9/liionpack/utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/circuits/4p1s.asc` & `liionpack-0.3.9/liionpack/circuits/4p1s.asc`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/liionpack/circuits/4p1s.cir` & `liionpack-0.3.9/liionpack/circuits/4p1s.cir`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper.bib` & `liionpack-0.3.9/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper.md` & `liionpack-0.3.9/paper/paper.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper_figures/Figure_0.png` & `liionpack-0.3.9/paper/paper_figures/Figure_0.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper_figures/Figure_1.png` & `liionpack-0.3.9/paper/paper_figures/Figure_1.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper_figures/Figure_2.png` & `liionpack-0.3.9/paper/paper_figures/Figure_2.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/paper/paper_figures/Figure_3.png` & `liionpack-0.3.9/paper/paper_figures/Figure_3.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/integration/test_1p1s.py` & `liionpack-0.3.9/tests/integration/test_1p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/integration/test_all_solvers.py` & `liionpack-0.3.9/tests/integration/test_all_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_logger.py` & `liionpack-0.3.9/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_netlist_utils.py` & `liionpack-0.3.9/tests/unit/test_netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_notebooks.py` & `liionpack-0.3.9/tests/unit/test_notebooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 #
 import os
 import subprocess
 import unittest
 import nbconvert
 import liionpack as lp
 import matplotlib
-matplotlib.use('Agg')  # Switch to a non-GUI backend
+
+matplotlib.use("Agg")  # Switch to a non-GUI backend
+
 
 class TestNotebooks(unittest.TestCase):
     def test_notebooks(self):
         examples_folder = os.path.join(lp.ROOT_DIR, "docs", "examples")
         for filename in os.listdir(examples_folder):
             if os.path.splitext(filename)[1] == ".ipynb":
                 print("-" * 80)
```

### Comparing `liionpack-0.3.8/tests/unit/test_plots.py` & `liionpack-0.3.9/tests/unit/test_plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_protocols.py` & `liionpack-0.3.9/tests/unit/test_protocols.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,27 +43,14 @@
         experiment = pybamm.Experiment(
             [pybamm.step.current(drive_cycle)], period="1 second"
         )
         p = lp.generate_protocol_from_experiment(experiment)
         assert len(p) == 601
         assert np.allclose(np.mean(p), 0.8404807891846922)
 
-    def test_time_exception(self):
-        def bad_timing():
-            experiment = pybamm.Experiment(
-                [
-                    "Charge at 50 A for 31 seconds",
-                ],
-                period="10 seconds",
-            )
-            _ = lp.generate_protocol_from_experiment(experiment)
-
-        with self.assertRaises(ValueError):
-            bad_timing()
-
     def test_current_exception(self):
         def bad_current():
             experiment = pybamm.Experiment(
                 [
                     "Charge at 1 C for 30 seconds",
                 ],
                 period="10 seconds",
```

### Comparing `liionpack-0.3.8/tests/unit/test_sim_utils.py` & `liionpack-0.3.9/tests/unit/test_sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_simulations.py` & `liionpack-0.3.9/tests/unit/test_simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_solver_utils.py` & `liionpack-0.3.9/tests/unit/test_solver_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_solvers.py` & `liionpack-0.3.9/tests/unit/test_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/tests/unit/test_utils.py` & `liionpack-0.3.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/.gitignore` & `liionpack-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/LICENSE` & `liionpack-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/README.md` & `liionpack-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.8/pyproject.toml` & `liionpack-0.3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,38 @@
 name = "liionpack"
 description = "A battery pack simulator for PyBaMM"
 readme = "README.md"
 license = "MIT"
 authors = [
     { name = "Tom Tranter", email = "t.g.tranter@gmail.com" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10, <3.13"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "Ipython",
     "lcapy",
     "matplotlib",
     "networkx",
     "numpy",
     "openpyxl",
     "pandas",
     "plotly",
-    "pybamm==23.9",
+    "pybamm==24.1",
     "ray",
     "redis",
     "scikit-spatial",
     "scipy",
     "textwrapper",
     "tqdm",
     "nbconvert",
```

### Comparing `liionpack-0.3.8/PKG-INFO` & `liionpack-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: liionpack
-Version: 0.3.8
+Version: 0.3.9
 Summary: A battery pack simulator for PyBaMM
 Project-URL: Bug Tracker, https://github.com/pybamm-team/liionpack/issues
 Project-URL: Changelog, https://github.com/pybamm-team/liionpack/blob/develop/CHANGELOG.md
 Project-URL: Documentation, https://liionpack.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/pybamm-team/liionpack
 Author-email: Tom Tranter <t.g.tranter@gmail.com>
 License-Expression: MIT
@@ -12,27 +12,29 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
+Requires-Python: <3.13,>=3.10
 Requires-Dist: ipython
 Requires-Dist: lcapy
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: plotly
-Requires-Dist: pybamm==23.9
+Requires-Dist: pybamm==24.1
 Requires-Dist: ray
 Requires-Dist: redis
 Requires-Dist: scikit-spatial
 Requires-Dist: scipy
 Requires-Dist: textwrapper
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
```

