# Comparing `tmp/powfacpy-0.1.4.tar.gz` & `tmp/powfacpy-0.1.5.tar.gz`

## Comparing `powfacpy-0.1.4.tar` & `powfacpy-0.1.5.tar`

### file list

```diff
@@ -1,140 +1,183 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/.nojekyll
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/Makefile
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/_config.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/index.html
--rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/make.bat
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/api.doctree
--rw-r--r--   0        0        0    27723 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/environment.pickle
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/how_to_contribute.doctree
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/index.doctree
--rw-r--r--   0        0        0    24558 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/introduction.doctree
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/tutorials.doctree
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree
--rw-r--r--   0        0        0    54402 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree
--rw-r--r--   0        0        0    65508 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree
--rw-r--r--   0        0        0    79988 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree
--rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFStudyCases.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/.buildinfo
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/api.html
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/genindex.html
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/how_to_contribute.html
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/index.html
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/introduction.html
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/objects.inv
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/search.html
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/searchindex.js
--rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/tutorials.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/api.rst.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/how_to_contribute.rst.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/introduction.rst.txt
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/tutorials.rst.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powerfactorypy.PFStringManipuilation.rst.txt
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFStringManipuilation.rst.txt
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/basic.css
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/plus.png
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/pygments.css
--rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/underscore.js
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/_static/js/theme.js
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powerfactorypy.PFBaseInterface.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powerfactorypy.PFStringManipuilation.html
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powfacpy.PFBaseInterface.html
--rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powfacpy.PFDynSimInterface.html
--rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powfacpy.PFPlotInterface.html
--rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powfacpy.PFStringManipuilation.html
--rw-r--r--   0        0        0    19956 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/html/generated/powfacpy.PFStudyCases.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/api.rst
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/conf.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/how_to_contribute.rst
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/index.rst
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/introduction.rst
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/generated/powfacpy.PFBaseInterface.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/generated/powfacpy.PFDynSimInterface.rst
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/generated/powfacpy.PFPlotInterface.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/generated/powfacpy.PFStringManipuilation.rst
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.4/docs/source/generated/powfacpy.PFStudyCases.rst
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/__init__.py
--rw-r--r--   0        0        0    49882 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/base_interface.py
--rw-r--r--   0        0        0    22271 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/case_studies.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/database_interface.py
--rw-r--r--   0        0        0    10167 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/dyn_sim_interface.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/engineering_helpers.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/exceptions.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/network_interface.py
--rw-r--r--   0        0        0    31090 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/plot_interface.py
--rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/results_interface.py
--rw-r--r--   0        0        0    11412 2020-02-02 00:00:00.000000 powfacpy-0.1.4/src/powfacpy/script_interface.py
--rw-r--r--   0        0        0    16665 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_base_interface.py
--rw-r--r--   0        0        0    14942 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_case_studies.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_database_interface.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_dyn_sim_interface.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_network_interface.py
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_plot_interface.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_results_interface.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/test_script_interface.py
--rw-r--r--   0        0        0   295168 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_input/powfacpy_tests.pfd
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_input/simple_script.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_input/test_comtrade.cfg
--rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_input/test_comtrade.dat
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/.gitignore
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/file_from_embedded_script.py
--rw-r--r--   0        0        0   140282 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/powfacpy_single_file.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/test1.json
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/test2.json
--rw-r--r--   0        0        0     4482 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/test_get_object_attributes.json
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tests/tests_output/test_get_object_attributes_modified.json
--rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/getting_started.ipynb
--rw-r--r--   0        0        0    50799 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/simulation_and_plotting.ipynb
--rw-r--r--   0        0        0    18578 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/study_cases.ipynb
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/cases_1.png
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/cases_2.png
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/legend_1.png
--rw-r--r--   0        0        0    17537 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/object_path.png
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/rebuild_button.png
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/scenarios_1.png
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 powfacpy-0.1.4/tutorials/figures/variations_3.png
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 powfacpy-0.1.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 powfacpy-0.1.4/LICENSE
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 powfacpy-0.1.4/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 powfacpy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 powfacpy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 powfacpy-0.1.5/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/.nojekyll
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/Makefile
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/_config.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/index.html
+-rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/make.bat
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/api.doctree
+-rw-r--r--   0        0        0    27723 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/environment.pickle
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/how_to_contribute.doctree
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/index.doctree
+-rw-r--r--   0        0        0    24558 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/introduction.doctree
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/tutorials.doctree
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree
+-rw-r--r--   0        0        0    54402 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree
+-rw-r--r--   0        0        0    65508 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree
+-rw-r--r--   0        0        0    79988 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree
+-rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFStudyCases.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/.buildinfo
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/api.html
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/genindex.html
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/how_to_contribute.html
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/index.html
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/introduction.html
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/objects.inv
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/search.html
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/searchindex.js
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/tutorials.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/api.rst.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/how_to_contribute.rst.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/introduction.rst.txt
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/tutorials.rst.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powerfactorypy.PFStringManipuilation.rst.txt
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFStringManipuilation.rst.txt
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/basic.css
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/plus.png
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/pygments.css
+-rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/underscore.js
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powerfactorypy.PFBaseInterface.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powerfactorypy.PFStringManipuilation.html
+-rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powfacpy.PFBaseInterface.html
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powfacpy.PFDynSimInterface.html
+-rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powfacpy.PFPlotInterface.html
+-rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powfacpy.PFStringManipuilation.html
+-rw-r--r--   0        0        0    19956 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/html/generated/powfacpy.PFStudyCases.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/api.rst
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/conf.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/how_to_contribute.rst
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/index.rst
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/introduction.rst
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/generated/powfacpy.PFBaseInterface.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/generated/powfacpy.PFDynSimInterface.rst
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/generated/powfacpy.PFPlotInterface.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/generated/powfacpy.PFStringManipuilation.rst
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.5/docs/source/generated/powfacpy.PFStudyCases.rst
+-rw-r--r--   0        0        0    19795 2020-02-02 00:00:00.000000 powfacpy-0.1.5/power_factory_objects/CopyOfObjectsInTableOfContentsOfScriptingReference.txt
+-rw-r--r--   0        0        0   260282 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmArea.txt
+-rw-r--r--   0        0        0  1076903 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmAsm.txt
+-rw-r--r--   0        0        0  1083370 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmAsmsc.txt
+-rw-r--r--   0        0        0    72412 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmBoundary.txt
+-rw-r--r--   0        0        0  1219126 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmCoup.txt
+-rw-r--r--   0        0        0  1079205 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmGenstat.txt
+-rw-r--r--   0        0        0   609076 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmIac.txt
+-rw-r--r--   0        0        0  1381816 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmLne.txt
+-rw-r--r--   0        0        0   799092 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmLod.txt
+-rw-r--r--   0        0        0   757418 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmLodlv.txt
+-rw-r--r--   0        0        0   799516 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmLodmv.txt
+-rw-r--r--   0        0        0  1081229 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmPvsys.txt
+-rw-r--r--   0        0        0    62660 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmSecctrl.txt
+-rw-r--r--   0        0        0  1078265 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmShnt.txt
+-rw-r--r--   0        0        0  1157076 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmSind.txt
+-rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmStactrl.txt
+-rw-r--r--   0        0        0  1144745 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmSym.txt
+-rw-r--r--   0        0        0   334278 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmTerm.txt
+-rw-r--r--   0        0        0  2031408 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmTr2.txt
+-rw-r--r--   0        0        0  2991495 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmTr3.txt
+-rw-r--r--   0        0        0   643288 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmVac.txt
+-rw-r--r--   0        0        0  1473726 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmVsc.txt
+-rw-r--r--   0        0        0  1093270 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmVscmono.txt
+-rw-r--r--   0        0        0   762160 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmXnet.txt
+-rw-r--r--   0        0        0   260960 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmZone.txt
+-rw-r--r--   0        0        0  1258884 2020-02-02 00:00:00.000000 powfacpy-0.1.5/result_variables/ElmZpu.txt
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/__init__.py
+-rw-r--r--   0        0        0    20180 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/active_project_interface.py
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/case_studies.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/database_interface.py
+-rw-r--r--   0        0        0    12515 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/dyn_sim_interface.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/engineering_helpers.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/exceptions.py
+-rw-r--r--   0        0        0    54130 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/folders_interface.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/functional_interface.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/grouping.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/model_exchange_interfaces.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/network_interface.py
+-rw-r--r--   0        0        0   794654 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/pf_class_protocols.py
+-rw-r--r--   0        0        0   791323 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/pf_class_protocols_old.py
+-rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/pf_classes_protocol_generator.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/pf_elm_objects.py
+-rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/plot_interface.py
+-rw-r--r--   0        0        0  3460426 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/result_variables.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/result_variables_parser.py
+-rw-r--r--   0        0        0    21278 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/results_interface.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/script_interface.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/string_manipulation.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 powfacpy-0.1.5/src/powfacpy/topology.py
+-rw-r--r--   0        0        0    17926 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_active_project_interface.py
+-rw-r--r--   0        0        0    14913 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_case_studies.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_database_interface.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_dyn_sim_interface.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_functional_interface.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_model_exchange_interfaces.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_network_interface.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_plot_interface.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_results_interface.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/test_script_interface.py
+-rw-r--r--   0        0        0   294848 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_input/powfacpy_tests.pfd
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_input/simple_script.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_input/test_comtrade.cfg
+-rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_input/test_comtrade.dat
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/.gitignore
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/file_from_embedded_script.py
+-rw-r--r--   0        0        0   140282 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/powfacpy_single_file.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/test1.json
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/test2.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/test_get_object_attributes.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tests/tests_output/test_get_object_attributes_modified.json
+-rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/getting_started.ipynb
+-rw-r--r--   0        0        0   237127 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/simulation_and_plotting.ipynb
+-rw-r--r--   0        0        0    19570 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/study_cases.ipynb
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/cases_1.png
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/cases_2.png
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/legend_1.png
+-rw-r--r--   0        0        0    17537 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/object_path.png
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/rebuild_button.png
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/scenarios_1.png
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/type_hints.png
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 powfacpy-0.1.5/tutorials/figures/variations_3.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 powfacpy-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 powfacpy-0.1.5/LICENSE
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 powfacpy-0.1.5/README.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 powfacpy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 powfacpy-0.1.5/PKG-INFO
```

### Comparing `powfacpy-0.1.4/docs/Makefile` & `powfacpy-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/make.bat` & `powfacpy-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/api.doctree` & `powfacpy-0.1.5/docs/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/environment.pickle` & `powfacpy-0.1.5/docs/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/how_to_contribute.doctree` & `powfacpy-0.1.5/docs/doctrees/how_to_contribute.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/index.doctree` & `powfacpy-0.1.5/docs/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/introduction.doctree` & `powfacpy-0.1.5/docs/doctrees/introduction.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/tutorials.doctree` & `powfacpy-0.1.5/docs/doctrees/tutorials.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/doctrees/generated/powfacpy.PFStudyCases.doctree` & `powfacpy-0.1.5/docs/doctrees/generated/powfacpy.PFStudyCases.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/api.html` & `powfacpy-0.1.5/docs/html/api.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/genindex.html` & `powfacpy-0.1.5/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/how_to_contribute.html` & `powfacpy-0.1.5/docs/html/how_to_contribute.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/index.html` & `powfacpy-0.1.5/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/introduction.html` & `powfacpy-0.1.5/docs/html/introduction.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/objects.inv` & `powfacpy-0.1.5/docs/html/objects.inv`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/search.html` & `powfacpy-0.1.5/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/searchindex.js` & `powfacpy-0.1.5/docs/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/tutorials.html` & `powfacpy-0.1.5/docs/html/tutorials.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/introduction.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/tutorials.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/tutorials.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt` & `powfacpy-0.1.5/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/_sphinx_javascript_frameworks_compat.js` & `powfacpy-0.1.5/docs/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/basic.css` & `powfacpy-0.1.5/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/doctools.js` & `powfacpy-0.1.5/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/jquery-3.6.0.js` & `powfacpy-0.1.5/docs/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/jquery.js` & `powfacpy-0.1.5/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/language_data.js` & `powfacpy-0.1.5/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/pygments.css` & `powfacpy-0.1.5/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/searchtools.js` & `powfacpy-0.1.5/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/underscore-1.13.1.js` & `powfacpy-0.1.5/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/underscore.js` & `powfacpy-0.1.5/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/badge_only.css` & `powfacpy-0.1.5/docs/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/theme.css` & `powfacpy-0.1.5/docs/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.eot` & `powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.svg` & `powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.ttf` & `powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/fontawesome-webfont.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold-italic.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold-italic.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-bold.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal-italic.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal-italic.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal.woff` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/css/fonts/lato-normal.woff2` & `powfacpy-0.1.5/docs/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/js/badge_only.js` & `powfacpy-0.1.5/docs/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/js/html5shiv-printshiv.min.js` & `powfacpy-0.1.5/docs/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/js/html5shiv.min.js` & `powfacpy-0.1.5/docs/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/_static/js/theme.js` & `powfacpy-0.1.5/docs/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powerfactorypy.PFBaseInterface.html` & `powfacpy-0.1.5/docs/html/generated/powerfactorypy.PFBaseInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powerfactorypy.PFStringManipuilation.html` & `powfacpy-0.1.5/docs/html/generated/powerfactorypy.PFStringManipuilation.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powfacpy.PFBaseInterface.html` & `powfacpy-0.1.5/docs/html/generated/powfacpy.PFBaseInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powfacpy.PFDynSimInterface.html` & `powfacpy-0.1.5/docs/html/generated/powfacpy.PFDynSimInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powfacpy.PFPlotInterface.html` & `powfacpy-0.1.5/docs/html/generated/powfacpy.PFPlotInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powfacpy.PFStringManipuilation.html` & `powfacpy-0.1.5/docs/html/generated/powfacpy.PFStringManipuilation.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/html/generated/powfacpy.PFStudyCases.html` & `powfacpy-0.1.5/docs/html/generated/powfacpy.PFStudyCases.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/conf.py` & `powfacpy-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/introduction.rst` & `powfacpy-0.1.5/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/tutorials.rst` & `powfacpy-0.1.5/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/generated/powfacpy.PFBaseInterface.rst` & `powfacpy-0.1.5/docs/source/generated/powfacpy.PFBaseInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/generated/powfacpy.PFDynSimInterface.rst` & `powfacpy-0.1.5/docs/source/generated/powfacpy.PFDynSimInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/generated/powfacpy.PFPlotInterface.rst` & `powfacpy-0.1.5/docs/source/generated/powfacpy.PFPlotInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/docs/source/generated/powfacpy.PFStudyCases.rst` & `powfacpy-0.1.5/docs/source/generated/powfacpy.PFStudyCases.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/src/powfacpy/base_interface.py` & `powfacpy-0.1.5/src/powfacpy/folders_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,459 +1,724 @@
-"""Contains the class PFBaseInterface (interaction with the PF database)
-and the class PFStringManipulation for string manipulation.
+"""Classes for interaction with the PF database. Based on folders from where downstream objects can accessed (see class PFFolder). The class PFActiveProject inherits from PFFolder and adds some functionality for the active project.
 
-The abbreviation 'PF' is sometimes used for 'PowerFactory'.
-"""
+Also contains the class PFStringManipulation for string manipulation.
 
-from warnings import warn
-from os import replace
+The acronym 'PF' is used for 'PowerFactory'.
+"""
+from __future__ import annotations
 from collections.abc import Iterable
+from typing import Union, Callable, Generator
 from os import path as os_path
+from functools import partial
+
+from icecream import ic
+
 import powfacpy
-import sys
-sys.path.insert(0, r'.\src')
+from powfacpy.pf_class_protocols import PFApp, PFGeneral, IntFolder, IntPrj, SetPrj, SetFilt
+from powfacpy.string_manipulation import PFStringManipulation
 
 
-class PFBaseInterface:
-    """Base interface for interaction with the PF database.
+
+class PFFolder():
+    """Class for interacting with folders in the PowerFactory database (any folder in the hierarchy).
+    
+    The class is very large and has methods to (you can search for sections):
+        - Get objects (search for '# Get') 
+        - Create objects (search for '# Create')
+        - Copy objects (search for '# Copy')
+        - Delete objects (search for '# Delete')
+        - Get/set attributes (search for '# Attributes')
+        - Utils to handle user input etc. (search for '# Handle')
+        - Utils to handle path strings (search for '# Path')
+        - Other functionality (search for '# Other')
+    
+    The class is large to have a convenient interface with a lot of functionality to interact with the PF database (at the cost of the clarity of the code unfortunately)
     """
-    language = "en"
+    
+    def __init__(self, folder:Union[PFGeneral, str], pf_app:PFApp):
+        if pf_app:
+            self.app:PFApp = pf_app
+        else:
+            raise TypeError("The input app is of type 'NoneType'. Maybe the PowerFactory app was not loaded correctly.")   
+        self._folder = self.app.GetActiveProject()
+        if not self._folder:
+            self._folder = self.app.GetCurrentUser()
+        self._folder:PFGeneral = self._handle_single_pf_object_or_path_input(folder)
+       
+    
+    def __getitem__(self, obj:str) -> PFGeneral:
+        """Allows to call 'get_obj' (without optional arguments, i.e. subfolders are included) using brakets.
+         
+        Example: terminals = folder_instance['*.ElmTerm']
+            where folder_instance is an instance of this class.
 
-    def __init__(self, app, language=None):
-        if app:
-            self.app = app
-        else:
-            raise TypeError("The input app is of type 'NoneType'. Maybe the PowerFactory "
-                            "app was not loaded correctly.")
-        if not language:
-            self.language = app.GetLanguage()
-        else:
-            self.language = language
+        Args:
+            obj (str): Object(s) to search for
 
-    def get_obj(self, path, condition=None, parent_folder=None, error_if_non_existent=True,
-                include_subfolders=True):
-        """Returns the PowerFactory object(s) under 'path'. 
-        'path' can contain wildcards ("*") after the last "\". 
-        A condition may be specified as a function, for example to check 
-        certain attributes with lambda function:
-          (eg. "condition = lambda x : getattr(x,"uknom")==110)".
-        By default, the 'path' is relative to the folder of the active project.
-        Only if 'parent_folder' is specified, it is relative to that folder.
-        The parent_folder can be a PF container object or a string:
-          parent_folder = "user" means 'path' is relative to the active user instead
-          of the active project.
-        An error is raised if no object is found, unless 'error_if_non_existent=False'.
+        Returns:
+            PFGeneral: Pointers to object(s) from the PF database
+        """
+        return self.get_obj(obj, include_subfolders=True)
+    
+    
+    def __iter__(self) -> Generator:
+        for obj in self.get_obj("*", 
+                                include_subfolders=False, error_if_non_existent=False):
+            yield obj  
+            
+    
+    def __str__(self) -> str:
+        return str(self._folder)   
+    
+    
+    def __len__(self) -> int:
+        return len(self._folder.GetContents("*"))   
+         
+
+##################
+# Reimplemenatation of methods of PF folder/container objects (to mimic the behavior of powerfactory.DataObject).
+##################        
+        
+    def GetContents(self, name:str, recursive:int=0) -> list[PFGeneral]:
+        return self._folder.GetContents(name, recursive)
+        
+    
+    def GetChildren(self, hiddenMode:int, filter:str, subfolders:int) -> list[PFGeneral]:
+        return self._folder.GetChildren(hiddenMode, filter, subfolders) 
+    
+    
+    def GetAttribute(self, attr:str) -> Union[int|float|str|PFGeneral|list]:
+        return  self._folder.GetAttribute(attr)
+    
+    
+    def SetAttribute(self, attr:str, value:Union[int|float|str|PFGeneral|list]) -> None:
+        return self._folder.SetAttribute(attr, value)    
+    
+    
+    def GetParent(self) -> PFGeneral:
+        return self._folder.GetParent()  
+    
+    
+    def CreateObject(self, 
+                     className:str, 
+                     objectNameParts:Union[int, str]="") -> PFGeneral:
+        return self._folder.CreateObject(className, objectNameParts)
+    
+    
+    def Delete(self) -> int:
+        return self._folder.Delete()      
+        
+    
+    def AddCopy(self, 
+                objectToCopy:list[PFGeneral] | PFGeneral, 
+                partOfName: Union[str, int] ="") -> PFGeneral:
+        return self._folder.AddCopy(objectToCopy, partOfName)    
+        
+    
+    def GetFullName(self) -> str:
+        return self._folder.GetFullName()     
+    
+       
+##################
+# Get
+##################
+    def get_obj(self, 
+                path: str, 
+                condition: Callable = None, 
+                parent_folder: Union[PFGeneral, PFFolder, str] = None, 
+                error_if_non_existent: bool = True,
+                include_subfolders: bool = False) -> list[PFGeneral]:
+        """Get the PowerFactory object(s) under 'path'. By default, 'path' is relative to 'self._folder' (or the active project folder for instances of PFActiveProject). 
+        
+        See also 'get_unique_obj'.
+
+        Args:
+            path (str): path to object(s), can contain wildcards ("*") after the last "\"
+            
+            condition (Callable, optional): filter for attributes etc.; example: "condition = lambda x : getattr(x,"uknom")==110; defaults to None
+            
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): specify a parent folder/container (or its path) from where the search is started ('path' is then relativ to 'parent_folder'); defaults to _folder/the active project folder for instances of PFActiveProject
+            
+            error_if_non_existent (bool, optional): raise exception if no objects are found; defaults to True
+            
+            include_subfolders (bool, optional): include subfolders in the search; defaults to True
+
+        Raises:
+            TypeError: If 'path' is not a string
+
+        Returns:
+            list[PFGeneral]: List with PF objects
 
         Examples:
           pfbi.get_obj("Network Model\\Network Data\\Grid\\Terminal 1")
+          
         The path can also start with "\\" and contain wildcards after last "\\":
           get_obj("\\Network Model\\Network Data\\Grid\\*.ElmTerm")
+        
         With condition:   
           pfbi.get_obj("Network Model\\Network Data\\Grid\\*.ElmTerm"",
             condition = lambda x : getattr(x,"uknom")==110)
-        Search in folder of the active user (instead of in the active project):
-          pfbi.get_obj("My project name", parent_folder="user")
 
-        Note that you can also use r" at the beginning of the string
+        Note that you can also use "r" at the beginning of the string
         argument to use single "\".  
-
-        See also method 'get_single_obj'
         """
-        if not parent_folder:
-            parent_folder = self.get_active_project()
-        else:
-            parent_folder = self.handle_single_pf_object_or_path_input(
-                parent_folder)
+        parent_folder = self._folder if not parent_folder else self._handle_single_pf_object_or_path_input(parent_folder, include_subfolders=False)
+        
         if not include_subfolders:
             try:
                 obj = parent_folder.GetContents(path)
             except (RuntimeError):
                 raise TypeError("Path must be of type string.")
         else:
-            obj = self.handle_inclusion_of_subfolders(
+            obj = self._handle_inclusion_of_subfolders(
                 path, parent_folder, error_if_non_existent)
         if not obj:
-            return self.handle_non_existing_obj(path, parent_folder, error_if_non_existent)
+            return self._handle_non_existing_obj(path, parent_folder, error_if_non_existent)
         if condition:
             obj_with_condition = self.get_by_condition(obj, condition)
             if obj_with_condition:
                 return obj_with_condition
             else:
-                return self.handle_condition_of_obj_not_met(path, obj, error_if_non_existent)
+                return self._handle_condition_of_obj_not_met(path, parent_folder, error_if_non_existent)
         else:
-            return obj
+            return obj    
 
-    def handle_inclusion_of_subfolders(self, path, parent_folder, error_if_non_existent):
-        """If subfolders are included, 'GetChildren' must
-        be used instead of 'GetContents'. 'GetChildren'
-        requires the input to be splitted between path and object name.
-        """
-        try:
-            path_folder_list = path.split('\\')
-            head, tail = '\\'.join(path_folder_list[:-1]), path_folder_list[-1]
-        except (AttributeError):
-            raise TypeError("Path must be of type string.")
-        if head:
-            new_parent_folder = parent_folder.GetContents(head)
-            if new_parent_folder:
-                parent_folder = new_parent_folder[0]
-            else:
-                return self.handle_non_existing_obj(head, parent_folder, error_if_non_existent)
-        return parent_folder.GetChildren(1, tail, 1)
+    
+    def get_obj_including_subfolders(
+                self, 
+                path: str, 
+                condition: Callable=None, 
+                parent_folder: Union[PFGeneral, PFFolder, str] = None, 
+                error_if_non_existent: bool = True,
+                include_subfolders: bool = False) -> list[PFGeneral]:
+        """Call 'get_obj' including subfolders."""
+        return self.get_obj(path,
+                            condition=condition,
+                            parent_folder=parent_folder,
+                            error_if_non_existent=error_if_non_existent,
+                            include_subfolders=True)
+        
+    
+    def get_obj_partial(self, *args, **kwargs) -> Callable:
+        """Partial evaluation of 'get_obj'.
+        
+        Returns a callable to get_obj.
+        
+        Example: a = get_obj_lazy("path\\to\\obj", error_if_non_existent=False)
+                 a() # This calls 'get_obj' with given arguments
+                 
+        For further information arguments etc. see 'get_obj'.         
+        """
+        return partial(self.get_obj, *args, **kwargs)
+        
+    
+    def get_unique_obj(self, 
+                       path:str, 
+                       parent_folder: Union[PFGeneral, PFFolder, str] = None, error_if_non_existent:bool = True,
+                       include_subfolders:bool = False) -> PFGeneral:
+        """Get unique PowerFactory object under 'path'. 
+        
+        Use this method if you want to access one single unique object.
+        This method is an alterntive to 'get_obj' and returns the unique object instead of a list (that needs to be accessed with '[0]'). It also checks whether the found object is unique (only one object is found).  
+        
+        This method is equal to get_single_obj and was added because the method
+        name fits better to what the method does (i.e. to get a unique object and to throw an error if the object is not unique).
+        
+        Args:
+            path (str): path to object(s); can contain wildcards ("*") after the last "\"
+                
+            condition (Callable, optional): filter for attributes etc.; example: "condition = lambda x : getattr(x,"uknom")==110; defaults to None
+                
+            parent_folder (Union[PFGeneral, PFFolder, str], optional):  
+            specify a parent folder/container (or its path) from where the search is started ('path' is then relativ to 'parent_folder'); defaults to _folder/the active project folder for instances of PFActiveProject
+                
+            error_if_non_existent (bool, optional): raise exception if no objects are found; defaults to True
+                
+            include_subfolders (bool, optional): include subfolders in the search; defaults to True
+
+        Raises:
+            TypeError: If 'path' is not a string or if several objects were found. 
 
-    def get_unique_obj(self, path, parent_folder=None, error_if_non_existent=True,
-                       include_subfolders=False):
-        """This method is equal to get_single_obj and was added because the method
-        name fits better to what the method does (i.e. to get a unique object and to
-        throw an error if the object is not unique).
+        Returns:
+            PFGeneral: PF object
         """
-        return self.get_single_obj(path, parent_folder=parent_folder,
+        return self.get_single_obj(path, 
+                                   parent_folder=parent_folder,
                                    error_if_non_existent=error_if_non_existent,
                                    include_subfolders=include_subfolders)
 
-    def get_single_obj(self, path, parent_folder=None, error_if_non_existent=True,
-                       include_subfolders=False):
-        """Use this method if you want to access one single unique object.
-        This method is an alterntive to 'get_obj' and returns the unique object instead
-        of a list (that needs to be accessed with '[0]'). It also checks whether the found
-        object is unique (only one object is found).
-        """
-        obj = self.get_obj(path, parent_folder=parent_folder,
+
+    def get_single_obj(self, 
+                       path:str, 
+                       parent_folder:Union[PFGeneral, PFFolder, str] = None, error_if_non_existent:bool = True,
+                       include_subfolders:bool = False) -> PFGeneral:
+        """Get unique PowerFactory object under 'path'. 
+        
+        Use this method if you want to access one single unique object.
+        This method is an alterntive to 'get_obj' and returns the unique object instead of a list (that needs to be accessed with '[0]'). It also checks whether the found object is unique (only one object is found).  
+        
+        Args:
+            path (str): path to object(s); 
+            can contain wildcards ("*") after the last "\"
+                
+            condition (Callable, optional): 
+            filter for attributes etc.; example: "condition = lambda x : getattr(x,"uknom")==110; 
+            defaults to None
+                
+            parent_folder (Union[PFGeneral, PFFolder, str], optional):  
+            specify a parent folder/container (or its path) from where the search is started ('path' is then relativ to 'parent_folder');
+            defaults to _folder/the active project folder for instances of PFActiveProject
+                
+            error_if_non_existent (bool, optional): 
+            raise exception if no objects are found;
+            defaults to True
+                
+            include_subfolders (bool, optional): 
+            include subfolders in the search;
+            defaults to True
+
+        Raises:
+            TypeError: 
+            If 'path' is not a string.
+            If several objects were found. 
+
+        Returns:
+            PFGeneral: PF object
+        """    
+        obj = self.get_obj(path, 
+                           parent_folder=parent_folder,
                            error_if_non_existent=error_if_non_existent,
                            include_subfolders=include_subfolders)
         if obj:
             if len(obj) < 2:
                 return obj[0]
             else:
-                raise TypeError(f"The path {path} is not a unique object. Did you use wildcards ('*')?"
-                                "This method only returns single unique objects.")
+                if parent_folder:     
+                    parent_folder_str = f" in '{self.get_path_of_object(parent_folder)}'" 
+                else:
+                    parent_folder_str = ""
+                raise TypeError(f"The path {path+parent_folder_str} is not a unique object. Did you use wildcards ('*')? This method only returns single unique objects.")
         else:
             return None
 
-    def get_multiple_obj_from_similar_sub_directories(self, parent_folders, sub_path):
-        """Returns multiple objects that are in a similar subdirectory relativ to
-        their parent folders.
-        Arguments:
-          parents: Parent folders (string path, list of objects/string paths)
-          sub_path: Path within the parent folders (string). Must be unique (don't
-            use placeholders '*')
+
+    def get_multiple_obj_from_similar_sub_directories(
+        self, 
+        parent_folders:Union[list[PFGeneral], str], 
+        sub_path:str) -> list[PFGeneral]:
+        """Get multiple objects that are in a similar subdirectory relativ to
+        their parent folders
+
+        Args:
+            parent_folders (Union[list[PFGeneral], str]): parent folders
+            
+            sub_path (str): 
+                path within the parent folders (string). Must be  unique (don't use placeholders '*')
+
+        Returns:
+            list[PFGeneral]: list of PF objects
 
         Example:
-          If you want to get the "All calculation" objects of all the study cases 
-          in the study case folder, use
-            self.get_multiple_obj_from_similar_sub_directories(
-              r"Study Cases\*","All calculations")     
+          If you want to get the "All calculation" objects of all the study cases in the study case folder, use
+            'self.get_multiple_obj_from_similar_sub_directories(
+              'Study Cases\\','All calculations')'    
         """
         if isinstance(parent_folders, str):
             parent_folders = self.get_obj(parent_folders)
         objs = []
         for parent in parent_folders:
-            parent = self.handle_single_pf_object_or_path_input(parent)
+            parent = self._handle_single_pf_object_or_path_input(parent)
             objs.append(self.get_single_obj(sub_path, parent_folder=parent))
         return objs
 
-    def handle_non_existing_obj(self, path, parent_folder, error_if_non_existent):
-        """Handles the attempted access to a non existent object.
-        """
-        if not error_if_non_existent:
-            return []
-        else:
-            exists_bool, existing_path, non_existing_child = self.path_exists(
-                path, parent_folder, return_info=True)
-            raise powfacpy.PFPathError(non_existing_child, existing_path)
-
-    def handle_condition_of_obj_not_met(self, path, obj, error_if_non_existent):
-        """Handles the attempted access to an object with a certain condition
-        that does not exist.
-        """
-        if not error_if_non_existent:
-            return []
-        else:
-            head, tail = os_path.split(path)
-            raise powfacpy.PFNonExistingObjectError(
-                obj[0].GetParent(), tail, condition=True)
 
-    def get_first_level_folder(self, folder):
-        """Returns folder on first level of PF database.
-        Currently the folder of the active user ('folder'='user') 
-        or the global library ('folder'='global library') can be accessed.
-        """
-        if folder == "user":
-            return self.get_active_user_folder()
-        elif folder == "global library":
-            return self.app.GetGlobalLibrary()
-        else:
-            raise TypeError(f"The first level folder {folder} is not valid. "
-                            "Use one of these: 'user', 'global library'.")
+    def get_upstream_obj(self,
+                         start_obj_or_path:Union[PFGeneral, str],
+                         condition:Callable,
+                         error_if_non_existent:bool=True) -> PFGeneral:
+        """Get upstream object that meets the condition.
+        
+        Searches upstream in the PF database hierarchy.
+
+        Args:
+            start_obj_or_path (Union[PFGeneral, str], optional): Object/folder (or its path) to start from
+                
+            condition (Callable): Condition for the searched object  
+              
+            error_if_non_existent (bool, optional): If True, an exception is raised if no upstream object is found. Defaults to True.
 
-    def path_exists(self, path, parent=None, return_info=False):
-        """Check if the path exists.
-        By default, it is searched in the folder of the active project
-        If 'parent' is specified it is searched relative to that folder.
-        If 'return_info' is True, information about where the path is
-        corrupted is returned. 
-        """
-        if not parent:
-            parent = self.get_active_project()
+        Returns:
+            PFGeneral: The PF object found
+        """        
+        start_obj_or_path = self._folder if not start_obj_or_path else self._handle_single_pf_object_or_path_input(start_obj_or_path)
+        obj_or_path = start_obj_or_path.GetParent()
+        if obj_or_path:
+            if condition(obj_or_path):
+                return obj_or_path
+            else:
+                return self.get_upstream_obj(obj_or_path, condition)
         else:
-            parent = self.handle_single_pf_object_or_path_input(parent)
-        splitted_path = path.split('\\')
-        if path[0] == "\\" or not splitted_path:
-            raise powfacpy.PFPathInputError(path)
-        existing_path = ""
-        child = parent
-        for child_name in splitted_path:
-            child = child.GetContents(f"{child_name}")
-            if child:
-                child = child[0]
-                existing_path = f"{existing_path}\{child.loc_name}"
+            if error_if_non_existent:
+                raise Exception(
+                    "There is no upstream object that fullfills the condition.")
             else:
-                if not return_info:
-                    return False
-                else:
-                    parent_path = parent.GetFullName()
-                    parent_path = PFStringManipulation._remove_class_names(
-                        parent_path)
-                    existing_path = f"{parent_path}{existing_path}"
-                    non_existent_child_name = child_name
-                    return False, existing_path, non_existent_child_name
-        return True
+                return None
+    
 
-    def get_from_study_case(self, class_name: str, if_not_unique: str = "warning", if_no_study_case="error"):
-        '''Returns objects from active study case like the PF built-in function app.GetFromStudyCase(). 
-        Additionally, this function outputs a warnings or errors if there is more than one object found and if no study case is activated.
-
-        Arguments:
-          class_name: class name of the object ('Class'), optionally preceded by an object name without wildcards and a dot ('Name.Class')
-          if_not_unique: set to "warning" or "error" or None, depending on the wanted behavior if the returned object is not unique.
-          if_no_study_case: set to "warning" or "error" or None, depending on the wanted behavior if no study case is active.
-        Returns:
-          Found or created object.
-        '''
-        study_case = self.app.GetActiveStudyCase()
-        object = self.app.GetFromStudyCase(class_name)
-
-        if not study_case:
-            if if_no_study_case == "warning":
-                warn("No study case activated. PowerFactory creates object of class_name in tmp folder, outside any study case.")
-            elif if_no_study_case == "error":
-                raise powfacpy.PFNoActiveStudyCaseError()
-
-        if if_not_unique:
-            if not '.' in class_name:
-                search_string = "*." + class_name
-            all_objects_of_this_class = self.get_obj(
-                search_string, parent_folder=object.GetParent(), include_subfolders=False)
-            if len(all_objects_of_this_class) > 1:
-                parent_path = self.get_path_of_object(object.GetParent())
-                if if_not_unique == "warning":
-                    warn(
-                        f"The returned {class_name} object is not unique in its folder / in its study case: '{parent_path}'. Make sure that the correct {class_name} object is used.")
-                if if_not_unique == "error":
-                    raise TypeError(
-                        f"The returned {class_name} object is not unique in its folder / in its study case: '{parent_path}'")
-
-        return object
-
-    def get_active_project(self):
-        """Returns the currently active project and throws an
-        error if no prject has been activated.
-        """
-        active_project = self.app.GetActiveProject()
-        if active_project:
-            return active_project
-        else:
-            raise powfacpy.PFNotActiveError("a project")
+    def get_by_condition(self, 
+                         objects:list[PFGeneral], 
+                         condition:Callable) -> list[PFGeneral]:
+        """Get objects (from a list of objects) which satisfy 'condition'.
+
+        Args:
+            objects (list[PFGeneral]): list of objects
+            condition (Callable): e.g. lambda function
+
+        Raises:
+            powfacpy.PFAttributeError: If 'condition' queries attributes which an item in 'objects' does not have.
+            TypeError: ToDo
 
-    def get_active_user_folder(self):
-        """Return the folder of the active user.
-        """
-        parent = self.get_active_project()
-        while not parent.GetClassName() == "IntUser":
-            parent = parent.GetParent()
-        return parent
-
-    def get_active_networks(self, error_if_no_network_is_active=True):
-        """Get active networks/grids.  
-        """
-        grids = self.app.GetCalcRelevantObjects(
-            ".ElmNet")  # This also returns the summary grid in the study case
-        # Delete the summary grid which is in the study case
-        grids[:] = [grid for grid in grids if not grid.GetParent().GetClassName()
-                    == "IntCase"]
-        if error_if_no_network_is_active and not grids:
-            raise powfacpy.PFNotActiveError("a network (ElmNet).")
-        return grids
-
-    def get_by_condition(self, objects, condition):
-        """From a list of objects, get those for whom the 'condition' 
-        (which is a function) returns 'True'.
+        Returns:
+            list[PFGeneral]: PF objects
+        
         Example:
           pfbi.get_by_condition(list_of_objects, lambda x : getattr(x,"uknom")==110)
         """
         objects_true = []
         for obj in objects:
             try:
                 # This anonymous function is problematic because it does
                 # not always throw an error when it the user provided
                 # an anonymous function that does not make sense.
                 if condition(obj):
                     objects_true.append(obj)
             except (AttributeError) as e:
                 raise powfacpy.PFAttributeError(obj, e, self)
             except (TypeError) as e:
-                object_str = powfacpy.PFStringManipulation._format_full_path(
-                    str(obj), self)
+                object_str = self.get_path_of_object(obj)
                 raise TypeError(f"{e}. Maybe an unexpected type is used "
                                 f"for attribute of object '{object_str}'.")
         return objects_true
 
-    def get_path_of_object(self, obj):
-        """
-        Returns path relative to active project without class names.
-        """
-        return PFStringManipulation._format_full_path(str(obj), self)
-
-    def get_path_of_object_with_class_names(self, obj):
-        obj = self.handle_single_pf_object_or_path_input(obj)
-        return str(obj)
-
-    def get_path_of_obj_with_class_names_relative_to_project(self, obj):
-        obj = self.handle_single_pf_object_or_path_input(obj)
-        return PFStringManipulation._get_path_inside_project_from_full_path(str(obj), self)
-
-    def get_attr(self, obj, attr, parent_folder=None):
-        """Get the value of an attribute of an object.
-        'obj' can be a path (string) or a Powerfactory object.
-        'attr' can be a string or a list of strings.
-        If parent_folder is specified, the path is relative to 
-        this folder.
-
-        Example:
-         pfbi.get_attr(terminal_1,"systype")
-        """
-        if isinstance(obj, str):
-            obj = self.get_single_obj(obj, parent_folder=parent_folder)
-        try:
-            if not isinstance(attr, list):
-                return obj.GetAttribute(attr)
-            else:
-                attr_values = dict()
-                for attribute in attr:
-                    attr_values[attribute] = obj.GetAttribute(attribute)
-                return attr_values
-        except (AttributeError) as e:
-            raise powfacpy.PFAttributeError(obj, e, self)
 
-    def get_attr_by_path(self, path_with_attr):
-        head_tail = os_path.split(path_with_attr)
-        return self.get_attr(head_tail[0], head_tail[1])
+##################
+# Create
+##################
+    def create_by_path(self, path:str, overwrite:bool=True) -> PFGeneral:
+        """Create an object by specifying its path (including the class at the end) and return the object.
+
+        Args:
+            path (str): path including class name at th end
+            overwrite (bool, optional): Overwrite extisting object. Defaults to True.
 
-    def set_attr(self, obj, params, parent_folder=None):
-        """
-        Set the attribute(s) of an object. 
-        obj: PowerFactory object or its path (string).
-        If 'parent_folder' is specified, the path is relative to 
-        this folder.
-        params: dictionary {parameter1:value1, parameter2:value2,..}.
-        """
-        if isinstance(obj, str):
-            obj = self.get_single_obj(obj, parent_folder=parent_folder)
-        for attr, value in params.items():
-            try:
-                obj.SetAttribute(attr, value)
-            except (TypeError) as e:
-                raise powfacpy.PFAttributeTypeError(obj, attr, e, self)
-            except (AttributeError) as e:
-                raise powfacpy.PFAttributeError(obj, e, self)
+        Raises:
+            TypeError: If 'path' is not a string
 
-    def set_attr_by_path(self, path_with_attr, value):
-        """
-        path_with_attr: path of object plus the attribute name
-        Example:
-          pfbi.set_attr_by_path(self,
-            "Library\\Dynamic Models\\Linear_interpolation\\desc",["description"])
-          Here 'desc' is the name of the attribute.  
-        """
-        head_tail = os_path.split(path_with_attr)
-        self.set_attr(head_tail[0], {head_tail[1]: value})
+        Returns:
+            PFGeneral: The created object
 
-    def create_by_path(self, path, overwrite=True):
-        """Create an object by specifying its path including its class and return the object.
-        If overwrite is true, objects with the same name will be overwritten.
         Example:
-          pfbi.create_by_path(r"Library\Dynamic Models\dummy.BlkDef") 
+          pfbi.create_by_path('Library\\Dynamic Models\\dummy.BlkDef') 
         """
         try:
             folder_path, obj_name_incl_class = path.rsplit('\\', 1)
         except (AttributeError):
             raise TypeError("The argument 'path' must be of type string.")
         folder = self.get_single_obj(folder_path)
-        return self.create_in_folder(folder, obj_name_incl_class, overwrite=overwrite)
+        return self.create_in_folder(obj_name_incl_class, folder, overwrite=overwrite)
+
+
+    def create_in_folder(self, 
+                         obj:str,
+                         folder:Union[PFGeneral, PFFolder, str] = None, 
+                         overwrite:bool = True, 
+                         use_existing:bool = False) -> PFGeneral:
+        """Create an object inside a folder and return the object.
+
+        Args:
+            obj (str): obj including class, e.g. 'model.BlkDef'
+            
+            folder (Union[PFGeneral, PFFolder, str], optional): Target folder. Defaults to None (i.e. 'self._folder')
+            
+            overwrite (bool, optional): objects with the same name will be overwritten. Defaults to True.
+            
+            use_existing (bool, optional): 
+                Only relevant if 'overwrite' is False.
+                If use_existing is False and an object with the same name exists, a new object with "(1)"/"(2)".. in its loc_name is created.
+                If use_existing is True and an object with the same name exists, the method just returns the existing object.
+                Defaults to False.
+                
+        Raises:
+            TypeError: If 'obj' is not a string
+
+        Returns:
+            PFGeneral: The created object
 
-    def create_in_folder(self, folder, obj, overwrite=True, use_existing=False):
-        """Creates an obj inside a folder and returns the object.
-        If overwrite is true, objects with the same name will be overwritten.
-        If use_existing is True, objects with the same name are not replaced.
-        If overwrite and use_existing are false and an object with the same name
-        exists, a new object with "(1)"/"(2)".. in name is created.
         Example:
-          pfbi.create_in_folder("Library\\Dynamic Models","dummy2.BlkDef")
+          pfbi.create_in_folder("dummy2.BlkDef", "Library\\Dynamic Models",)
         """
-        folder = self.handle_single_pf_object_or_path_input(folder)
+        folder = self._folder if not folder else self._handle_single_pf_object_or_path_input(folder)
         try:
             obj_name, _, class_name = obj.rpartition('.')
         except (AttributeError):
             raise TypeError("The argument 'obj' must be of type string.")
         if overwrite:
-            self.delete_obj(obj, parent_folder=folder,
+            self.delete_obj(obj, 
+                            parent_folder=folder,
+                            include_subfolders=False,
                             error_if_non_existent=False)
         elif use_existing:
             existing_obj = self.get_single_obj(
                 obj, parent_folder=folder, error_if_non_existent=False)
             if existing_obj:
                 return existing_obj
         return folder.CreateObject(class_name, obj_name)
 
-    def create_directory(self, directory, parent_folder=None):
-        """Create a directory of folders ('IntFolder') if the 
-        directory does not yet exist.
-        Arguments:
-          path: path of folders
-          parent_folder: If not specified, the active project folder
-            is used.
 
-        Returns the folder in the lowest subdirectory.  
+    def create_directory(self, 
+                         directory:str, 
+                         parent_folder:Union[PFGeneral, PFFolder, str] = None) -> IntFolder:
+        """Create a directory of folders ('IntFolder') if the directory does not exist yet.
+
+        Args:
+            directory (str): path with folders
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): Folder to start from. Defaults to None.
+
+        Returns:
+            IntFolder: the folder in the lowest subdirectory.  
         """
         if not self.path_exists(directory, parent=parent_folder):
-            if parent_folder:
-                folder = parent_folder
-            else:
-                folder = self.app.GetActiveProject()
+            folder = self._folder if not parent_folder else parent_folder
             folder_names = directory.split("\\")
             for folder_name in folder_names:
                 if not self.path_exists(folder_name, parent=folder):
                     folder = self.create_in_folder(
-                        folder, folder_name+".IntFolder")
+                        folder_name + ".IntFolder", folder)
                 else:
                     folder = self.get_single_obj(
-                        folder_name, parent_folder=folder)
+                        folder_name, 
+                        parent_folder=folder, 
+                        include_subfolders=False)
             return folder
         else:
-            return self.get_single_obj(directory, parent_folder=parent_folder)
+            return self.get_single_obj(directory, 
+                                       parent_folder=parent_folder,
+                                       include_subfolders=False)
+    
+    
+    def create_filter_obj(
+        self,
+        name: str, 
+        folder: str | PFGeneral,
+        object_filter: str,
+        look_in: PFGeneral | str,
+        expression: str, 
+        include_subfolders: bool = True,
+        only_calc_relevant_obj: bool = False,
+        overwrite = True,
+        use_existing = False) -> SetFilt:
+        """Create filter object (SetFilt)
+
+        Args:
+            name (str): Name of filter object.
+            
+            folder (PFGeneral | PFFolder | str): target folder where filer is created.
+        
+            object_filter (str): Object/class filter (parameter 'objset'). Class names sparated by commas, e.g. '*.ElmTerm, *.ElmLne'.
+            
+            look_in (PFGeneral | str): Folder from which search is started (parameter 'pstart').
+            
+            expression (str): filter expression (parameter 'expr'), e.g. 'uknom>100.and.uknom<380.and.iUsage=0'
+            
+            include_subfolders (bool, optional): Include subfolders in search. Defaults to True.
+            
+            only_calc_relevant_obj (bool, optional): Search only for calc. relevant objects. Defaults to True.
+            
+            overwrite (bool, optional): Overwrite possible existing filter object. Defaults to True.
+            
+            use_existing (bool, optional): See description of 'create_in_folder' in 'PFFolder' class of powfacpy. Defaults to False.
+
+        Returns:
+            SetFilt: Filter object
+        """ 
+        
+        filter_obj: SetFilt = self.create_in_folder(
+            name + ".SetFilt", 
+            folder=folder,
+            overwrite=overwrite, 
+            use_existing=use_existing)
+        look_in = self._handle_single_pf_object_or_path_input(look_in)
+        filter_obj.objset =  [object_filter]
+        filter_obj.expr = expression
+        filter_obj.pstart = look_in  
+        filter_obj.isubfold = include_subfolders
+        filter_obj.icalcrel = only_calc_relevant_obj
+        return filter_obj
+        
+        
+               
+
+
+##################
+# Copy
+##################
+    def copy_obj(self, 
+                 obj_or_path:Union[PFGeneral, str], 
+                 target_folder:Union[PFGeneral, PFFolder, str], 
+                 overwrite:bool=True, 
+                 condition:Callable=None,
+                 parent_folder:Union[PFGeneral, PFFolder, str]=None, 
+                 error_if_non_existent:bool=True, 
+                 include_subfolders:bool=False) -> list[PFGeneral]:
+        """Copy object(s) to 'target_folder'. 
+        
+        Uses 'get_obj' to get the objects under 'obj_or_path'. Source and target must be in the active project (otherwise use PasteCopy(), see scripting reference)
+        
+        See also 'copy_single_obj'.
+
+        Args:
+            obj_or_path (Union[PFGeneral, str]): 
+                Objects to be copied (get_object is used)
+                
+            target_folder (Union[PFGeneral, PFFolder, str]): 
+                Folder to which objects are copied
+                
+            overwrite (bool, optional): 
+                Overwrite existing objects. Defaults to True.
+                
+            condition (Callable, optional): 
+                Condition used in 'get_obj' for the source objects . Defaults to None.
+                
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): 
+                refers to the source folder and is used in combination with 'obj_or_path' to get the object(s) to be copied. Defaults to  None (i.e. '_folder'/active project is used).
+                
+            error_if_non_existent (bool, optional): 
+                Raise error if no (source) objects are found. Defaults to True.
+                
+            include_subfolders (bool, optional): 
+                Include subfolder in search for source objects. Defaults to False.
+
+        Returns:
+            list[PFGeneral]: Copied objects
+        """
+        obj = self._handle_pf_object_or_path_input(
+            obj_or_path,
+            condition=condition,
+            parent_folder=parent_folder,
+            error_if_non_existent=error_if_non_existent,
+            include_subfolders=include_subfolders)
+        target_folder = self._handle_single_pf_object_or_path_input(
+            target_folder)
+        if overwrite:
+            for object_to_be_copied in obj:
+                self.delete_obj(object_to_be_copied.GetAttribute("loc_name"),
+                                parent_folder=target_folder, error_if_non_existent=False)
+        # AddCopy() accepts a list of objects, but then it returns the target folder object and not the copied objects. Therefore, it is iterated through the objects.
+        copied_obj = []
+        for o in obj:
+            copied_obj.append(target_folder.AddCopy(o))
+        return copied_obj
+
+
+    def copy_single_obj(self, 
+                        obj_or_path:Union[PFGeneral, str], 
+                        target_folder:Union[PFGeneral, PFFolder, str], 
+                        overwrite:bool = True,
+                        new_name:str = None, 
+                        parent_folder:Union[PFGeneral, PFFolder, str] = None, error_if_non_existent:bool = True) -> PFGeneral:
+        """Copy a single PF object to 'target_folder'
+        
+         Uses 'get_unique_obj' to get the object under 'obj_or_path'. Source and target must be in the active project (otherwise use PasteCopy(), see scripting reference)
+        
+        See also 'copy_obj'.
+
+        Args:
+            obj_or_path (Union[PFGeneral, str]): 
+                Object to be copied (get_unique_object is used)
+                
+            target_folder (Union[PFGeneral, PFFolder, str]): 
+                Folder to which object is copied
+                
+            overwrite (bool, optional): 
+                Overwrite existing objects. Defaults to True.
+                
+            new_name (str, optional): 
+                New name (if different to original). Defaults to None.
+                
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): 
+                refers to the source folder and is used in combination with 'obj_or_path' to get the object(s) to be copied. Defaults to  None (i.e. '_folder'/active project is used).
+                
+            error_if_non_existent (bool, optional): 
+                Raise error if no (source) objects are found. Defaults to True.
+                
+            include_subfolders (bool, optional): 
+                Include subfolder in search for source objects. Defaults to False.
+
+        Returns:
+            PFGeneral: Copied object/existing object if overwrite is False
+        """
+        obj = self._handle_single_pf_object_or_path_input(
+            obj_or_path,
+            parent_folder=parent_folder,
+            error_if_non_existent=error_if_non_existent)
+        target_folder = self._handle_single_pf_object_or_path_input(
+            target_folder)
+        if overwrite:
+            if not new_name:
+                self.delete_obj(obj.GetAttribute("loc_name"),
+                                parent_folder=target_folder,
+                                include_subfolders=False,
+                                error_if_non_existent=False)
+            else:
+                self.delete_obj(f"{new_name}.*",
+                                parent_folder=target_folder,
+                                include_subfolders=False,
+                                error_if_non_existent=False)
+        else:
+            existing_obj = self.get_single_obj(obj.GetAttribute("loc_name"),
+                                parent_folder=target_folder, error_if_non_existent=False)  
+            if existing_obj:
+                return existing_obj      
+        if new_name:
+            return target_folder.AddCopy(obj, new_name)
+        else:
+            return target_folder.AddCopy(obj)
+ 
+ 
+##################
+# Delete
+##################
+    def delete_obj(self, 
+                   obj_or_path:Union[PFGeneral, str], 
+                   condition:Callable = None, 
+                   parent_folder:Union[PFGeneral, str] = None, error_if_non_existent:bool = True,
+                   include_subfolders:bool = False):
+        """Delete PF object(s).
+        
+        In a first step, the objects are retrieved using the 'get_obj'
+        method. In a second step, they are deleted. For further info on the input arguments, see the `get_obj` method. Checks whether objects were really deleted, otherwise tries to deactivate the object and then delete it.
+
+        Args:
+            obj_or_path (Union[PFGeneral, str]): objects to be deleted.
+            
+            condition (Callable, optional): 
+                Condition for retrieved object(s). Defaults to None.
+                
+            parent_folder (Union[PFGeneral, str], optional): 
+                Parent folder used in 'get_obj'. Defaults to None.
+                
+            error_if_non_existent (bool, optional): 
+                Throw exception if not objects found. Defaults to True.
+                
+            include_subfolders (bool, optional): Search also in subfolders. Defaults to False.
 
-    def delete_obj(self, obj_or_path, condition=None, parent_folder=None, error_if_non_existent=True,
-                   include_subfolders=False):
-        """Delete object(s). In a first step, the objects are loaded using the `get_obj`
-        method. In a second step, they are deleted. For further info on the input 
-        arguments, see the `get_obj` method. 
-        It is also checked whether the object was really deleted, otherwise it is tried
-        to deactivate the object and then delete it.
+        Raises:
+            TypeError: If an object cannot be deleted.
         """
-        obj = self.handle_pf_object_or_path_input(obj_or_path,
+        obj = self._handle_pf_object_or_path_input(obj_or_path,
                                                   condition=condition,
                                                   parent_folder=parent_folder,
                                                   error_if_non_existent=error_if_non_existent,
                                                   include_subfolders=include_subfolders)
         for o in obj:
             o.Delete()
             # 'IsDeleted' seems to be the savest way to check whether an object has been deleted.
@@ -470,628 +735,554 @@
                         o.Delete()
                     except (AttributeError):  # raised when o cannot be deactivated
                         raise TypeError(f"Object {o} cannot be deleted.")
 
                     if not o.IsDeleted():
                         raise TypeError(f"Object {o} cannot be deleted.")
 
-    def clear_folder(self, folder):
-        """
-        Clear all objects inside folder (including hidden objects).
+
+    def clear_folder(self, folder:Union[PFGeneral, PFFolder, str] = None):
+        """Clear all objects inside folder (including hidden objects).
+
+        Args:
+            folder (Union[PFGeneral, PFFolder, str], optional): Folder/ container objects or its path. Defaults to None (i.e. '_folder'/active project).
         """
-        folder = self.handle_single_pf_object_or_path_input(folder)
+        folder = self._folder if not folder else self._handle_single_pf_object_or_path_input(folder)
         self.delete_obj("*",
                         parent_folder=folder,
-                        include_subfolders=True,
+                        include_subfolders=False,
                         error_if_non_existent=False)
 
-    def handle_pf_object_or_path_input(self, obj_or_path, condition=None, parent_folder=None,
-                                       error_if_non_existent=True, include_subfolders=False):
-        """Handles the input argument when a method accepts either
+ 
+##################
+# Attributes
+##################
+    def get_attr(self, 
+                 obj:Union[PFGeneral, str], 
+                 attr:str, 
+                 parent_folder:Union[PFGeneral, PFFolder, str] = None) -> Union[int|float|str|PFGeneral|list]:
+        """Get the value of an attribute of an object.
+
+        Args:
+            obj (Union[PFGeneral, str]): object or its path
+            attr (str): attribute name
+            parent_folder (Union[PFGeneral, PFFolder, str], optional):  
+                - parent folder of object. Defaults to None.
+
+        Raises:
+            powfacpy.PFAttributeError: If ojbect does not have the specified attribute
+
+        Returns:
+            Union[int|float|str|PFGeneral|list]: Attribute value  
+        
+        Example:
+            get_attr(terminal_1, "systype")
+        """
+        if isinstance(obj, str):
+            obj = self.get_single_obj(obj, parent_folder=parent_folder)
+        try:
+            if not isinstance(attr, list):
+                return obj.GetAttribute(attr)
+            else:
+                attr_values = dict()
+                for attribute in attr:
+                    attr_values[attribute] = obj.GetAttribute(attribute)
+                return attr_values
+        except (AttributeError) as e:
+            raise powfacpy.PFAttributeError(obj, e, self)
+
+
+    def get_attr_by_path(self, path_with_attr:str) -> Union[int|float|str|PFGeneral|list]:
+        """Get attribute using the path including the atrribute name
+
+        Args:
+            path_with_attr (str): path including the atrribute name
+            Example: 'user\\project\\path\\to\\object\\m:Psum:bus1'
+
+        Returns:
+            Union[int|float|str|PFGeneral|list]: Attribute value  
+        """
+        head_tail = os_path.split(path_with_attr)
+        return self.get_attr(head_tail[0], head_tail[1])
+
+
+    def set_attr(self, 
+                 obj:Union[PFGeneral, str], 
+                 params:dict, 
+                 parent_folder:Union[PFGeneral, PFFolder, str]=None) -> None:
+        """Set the attribute(s) of an object.
+
+        Args:
+            obj (Union[PFGeneral, str]): PF object
+            params (dict): atttributes and their values (e.g. {'parameter1':value1, 'parameter2':value2,..})
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): Parent folder object. Defaults to None.
+
+        Raises:
+            powfacpy.PFAttributeTypeError: If the type of an attribute value is wrong
+            powfacpy.PFAttributeError: If an object does not have th especified attribute
+        """
+        obj = self._handle_single_pf_object_or_path_input(
+            obj, parent_folder=parent_folder)
+        for attr, value in params.items():
+            try:
+                obj.SetAttribute(attr, value)
+            except (TypeError) as e:
+                raise powfacpy.PFAttributeTypeError(obj, attr, e, self)
+            except (AttributeError) as e:
+                raise powfacpy.PFAttributeError(obj, e, self)
+
+
+    def set_attr_by_path(self, 
+                         path_with_attr:str, 
+                         value:Union[int|float|str|PFGeneral|list]):
+        """Set attribute using the path including the attribute name.
+
+        Args:
+            path_with_attr (str): path to ojbect with attribute name at the end
+            value (Union[int | float | str | PFGeneral | list]): attribute value
+
+        Example:
+          set_attr_by_path(
+                "Library\\Dynamic Models\\Linear_interpolation\\desc", 
+                ["description"])
+          Here 'desc' is the name of the attribute.  
+        """
+        head_tail = os_path.split(path_with_attr)
+        self.set_attr(head_tail[0], {head_tail[1]: value})
+
+
+##################
+# Handle
+##################
+    def _handle_inclusion_of_subfolders(
+        self, 
+        path:str, 
+        parent_folder:Union[PFGeneral, PFFolder, str], 
+        error_if_non_existent:bool) -> Union[list, PFGeneral]:
+        """Handle the inclusion of subfolders in search for objects.
+
+        If subfolders are included, 'GetChildren' must be used instead of 'GetContents'. 'GetChildren' requires the input to be splitted between path and object name.
+        
+        Args:
+            path (str): Path to object(s)
+            
+            parent_folder (Union[PFGeneral, PFFolder,str]): Parent folder where search is started
+            
+            error_if_non_existent (bool): Raise exception if no objects are found
+
+        Raises:
+            TypeError: If 'path' is not a string
+
+        Returns:
+            Union[list, PFGeneral]: Retrieved objects
+        """
+        try:
+            path_folder_list = path.split('\\')
+            head, tail = '\\'.join(path_folder_list[:-1]), path_folder_list[-1]
+        except (AttributeError):
+            raise TypeError("Path must be of type string.")
+        if head:
+            new_parent_folder = parent_folder.GetContents(head)
+            if new_parent_folder:
+                parent_folder = new_parent_folder[0]
+            else:
+                return self._handle_non_existing_obj(
+                    head, parent_folder, error_if_non_existent)
+        return parent_folder.GetChildren(1, tail, 1)
+
+    
+    def _handle_non_existing_obj(self, 
+                                path:str, 
+                                parent_folder:Union[PFGeneral, PFFolder, str], error_if_non_existent:bool) -> list:
+        """Handle the attempted access to a non existent object.
+
+        Args:
+            path (str): path to object
+            
+            parent_folder (Union[PFGeneral, PFFolder, str]): search is started from here
+            
+            error_if_non_existent (bool): raise exception if non existent
+
+        Raises:
+            powfacpy.PFPathError: if 'error_if_non_existent' is True
+
+        Returns:
+            list: empty list if 'error_if_non_existent' is False
+        """
+        if not error_if_non_existent:
+            return []
+        else:
+            exists_bool, existing_path, non_existing_child = self.path_exists(
+                path, parent_folder, return_info=True)
+            raise powfacpy.PFPathError(non_existing_child, existing_path)
+
+
+    def _handle_condition_of_obj_not_met(
+        self, 
+        path:str, 
+        parent_folder:Union[PFGeneral, PFFolder], 
+        error_if_non_existent:bool) -> list | None:
+        """Handle the attempted access to an object with a specific condition, when such object(s) were found, but none of them meets the condition.
+
+        Args:
+            path (str): path of the object(s)
+            
+            obj (list[Union[PFGeneral, PFFolder]]): list of objects found using path, but none of them satisfies the condition
+            
+            error_if_non_existent (bool): raise exception
+
+        Raises:
+            powfacpy.PFNonExistingObjectError: If 'error_if_non_existent' is True
+
+        Returns:
+            list | None: empty list
+        """
+        if not error_if_non_existent:
+            return []
+        else:
+            # head, tail = os_path.split(path)
+            raise powfacpy.PFNonExistingObjectError(
+                parent_folder, path, condition=True)
+    
+
+    def _handle_pf_object_or_path_input(
+        self, 
+        obj_or_path:Union[PFGeneral, str], 
+        condition:bool=None, 
+        parent_folder:Union[PFGeneral, PFFolder, str]=None,
+        error_if_non_existent:bool=True, 
+        include_subfolders:bool=False) -> PFGeneral | list[PFGeneral]:
+        """Handles the input argument 'obj_or_path' when a method accepts either
           - a path string
           - a PF object
           - an iterable (of PF objects) 
+          
+        Note: Unfortunately, it cannot be checked whether 'obj' is a PF DataObject, because the module powerfactory is not available.
 
-        Returns the PF object(s) in a list.
-        If 'obj' is a path string, it returns the PF object(s) of that path.
-        If 'obj' is a PF object (or multiple), it does nothing and just returns 
-        the object(s).
+        See also '_handle_single_pf_object_or_path_input'  
 
-        Note: Unfortunately, it cannot be checked whether 'obj' is a PF DataObject, 
-        because the module powerfactory is not available.
+        Args:
+            obj_or_path (Union[PFGeneral, str]): see get_obj
+            
+            condition (bool, optional): see get_obj. Defaults to None.
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): see get_obj. Defaults to None.
+            
+            error_if_non_existent (bool, optional): see get_obj. Defaults to True.
+            
+            include_subfolders (bool, optional): see get_obj. Defaults to False.
 
-        See also method 'handle_single_pf_object_or_path_input'
+        Returns:
+            PFGeneral: 
+                - PF object(s) in a list. 
+                - If 'obj_or_path' is a path string, it returns the PF object(s) of that path.
+                - If 'obj_or_path' is a PF object (or multiple), it does nothing and just returns the object(s).
         """
         if isinstance(obj_or_path, str):
             return self.get_obj(obj_or_path, condition=condition,
                                 parent_folder=parent_folder,
                                 error_if_non_existent=error_if_non_existent,
                                 include_subfolders=include_subfolders)
         elif not isinstance(obj_or_path, Iterable):
             return [obj_or_path]
-        else:  # If all former conditions are False, it is assumed that the
-            # input already was a list of PF object(s).
-            return obj_or_path
-
-    def handle_single_pf_object_or_path_input(self, obj, parent_folder=None,
-                                              error_if_non_existent=True):
+        elif not isinstance(obj_or_path[0], str):
+            return obj_or_path    
+        else: 
+            objs = []
+            for obj in obj_or_path:
+                objs += self.get_obj(obj)
+            return objs
+            
+
+
+    def _handle_single_pf_object_or_path_input(
+        self, 
+        obj_or_path:Union[PFGeneral, str], 
+        parent_folder:Union[PFGeneral, PFFolder, str] = None,
+        error_if_non_existent:bool = True,
+        include_subfolders:bool = False) -> PFGeneral:
         """Handles the input argument when a method accepts either
           - a path string
           - or a PF object
-          - but NOT an iterable of PF objects
+          - but NOT an iterable of PF objects (difference to    _handle_pf_object_or_path_input)
+          
+        Note: Unfortunately, it cannot be checked whether 'obj' is a PF DataObject, because the module powerfactory is not available.
+
+        See also method 'handle_pf_object_path_input'  
+
+        Args:
+            obj (Union[PFGeneral, str]): see get_single_obj
+            
+            parent_folder (Union[PFGeneral, PFFolder, str], optional): get_single_obj. Defaults to None.
+            
+            error_if_non_existent (bool, optional): get_single_obj. Defaults to True.
 
-        If 'obj' is a path string, it returns the PF object of that path.
-        If 'obj' is a PF object, it does nothing and just returns the object.
-        If 'obj' is an iterable (unexpected), a meaningfull error message is provided.
+        Raises:
+            TypeError: If 'obj_or_path' is an iterable (unexpected), a meaningfull error is raised.
 
-        Note: Unfortunately, it cannot be checked whether 'obj' is a PF DataObject, 
-        because the module powerfactory is not available.
-
-        See also method 'handle_pf_object_path_input'
+        Returns:
+            PFGeneral: If 'obj_or_path' is a path string, it returns the PF object of that path.
+            If 'obj_or_path' is a PF object, it does nothing and just returns the object.
         """
-        if isinstance(obj, str):
-            return self.get_single_obj(obj, parent_folder=parent_folder,
-                                       error_if_non_existent=error_if_non_existent)
-        elif isinstance(obj, Iterable):
-            elements_count = len(obj)
-            if obj:
-                first_obj_type = type(obj[0])
+        if isinstance(obj_or_path, str):
+            return self.get_single_obj(
+                obj_or_path, 
+                parent_folder=parent_folder,
+                error_if_non_existent=error_if_non_existent,
+                include_subfolders=include_subfolders)
+        elif isinstance(obj_or_path, Iterable) and not isinstance(obj_or_path, powfacpy.PFFolder):
+            elements_count = len(obj_or_path)
+            if obj_or_path:
+                first_obj_type = type(obj_or_path[0])
                 try:
-                    first_obj_path = self.get_path_of_object(obj[0])
-                    msg_obj = (f"The first element is of type {first_obj_type} and its "
-                               f"path is {first_obj_path}.")
+                    first_obj_path = self.get_path_of_object(obj_or_path[0])
+                    msg_obj = (f"The first element is of type {first_obj_type} and its path is {first_obj_path}.")
                 except (AttributeError):
                     msg_obj = f"The first element is of type {first_obj_type}."
-                msg = (f"Expected a PowerFactory object or a path string. Instead an "
-                       f"iterable of length {elements_count} is given. {msg_obj}")
+                msg = (f"Expected a PowerFactory object or a path string. Instead an iterable of length {elements_count} is given. {msg_obj}")
                 raise TypeError(msg)
             else:
-                msg = (f"Expected a PowerFactory object or a path string. Instead an "
-                       f"empty object of type '{type(obj).__name__}' is given.")
+                msg = (f"Expected a PowerFactory object or a path string. Instead an empty object of type '{type(obj_or_path).__name__}' is given.")
                 raise TypeError(msg)
         else:  # If all former conditions are False, it is assumed that the
             # input already was a PF object.
-            return obj
+            return obj_or_path
 
-    def copy_obj(self, obj_or_path, target_folder, overwrite=True, condition=None,
-                 parent_folder=None, error_if_non_existent=True, include_subfolders=False):
-        """Copies object(s) by using 'get_obj' in first step and then copying 
-        the returned objects to 'target_folder'. Source and target must be in 
-        the active project (otherwise use PasteCopy(), see scripting reference).
-        The argument 'parent_folder' refers to the source folder and is used in
-        combination with 'obj_or_path' to get the object(s) to be copied.
-        If 'overwrite' is True, existing objects with the same name are overwritten
-        in the target folder.
-        For further information on the input arguments, see method 'get_obj'.
 
-        Returns a list of the created copy/copies.
+######################
+# Paths
+######################
+    def path_exists(self, 
+                    path:str, 
+                    parent:Union[PFGeneral, PFFolder, str] = None, 
+                    return_info:bool=False) -> bool:
+        """Check if the path exists.
+        
+        If 'parent' is specified it is searched relative to that folder.
+        If 'return_info' is True, . 
 
-        See also 'copy_single_obj'
-        """
-        obj = self.handle_pf_object_or_path_input(obj_or_path,
-                                                  condition=condition,
-                                                  parent_folder=parent_folder,
-                                                  error_if_non_existent=error_if_non_existent,
-                                                  include_subfolders=include_subfolders)
-        target_folder = self.handle_single_pf_object_or_path_input(
-            target_folder)
-        if overwrite:
-            for object_to_be_copied in obj:
-                self.delete_obj(object_to_be_copied.GetAttribute("loc_name"),
-                                parent_folder=target_folder, error_if_non_existent=False)
-        # AddCopy() accepts a list of objects, but then it returns the target
-        # folder object and not the copied objects. Therefore, it is iterated through the
-        # objects.
-        copied_obj = []
-        for o in obj:
-            copied_obj.append(target_folder.AddCopy(o))
-        return copied_obj
+        Args:
+            path (str): path
+            
+            parent (Union[PFGeneral, PFFolder, str], optional): Parent folder where search is started. Defaults to None (i.e. 'self._folder').
+            
+            return_info (bool, optional): information about where the path is
+            corrupted is returned. Defaults to False.
 
-    def copy_single_obj(self, obj_or_path, target_folder, overwrite=True,
-                        new_name=None, parent_folder=None, error_if_non_existent=True):
-        """Copies single object by using 'get_single_obj' in first step and then copying 
-        the returned object to 'target_folder'.
-        The argument 'parent_folder' refers to the source folder and is used in
-        combination with 'obj_or_path' to get the object to be copied.
-        If 'overwrite' is True, existing objects with the same name are overwritten
-        in the target folder.
-        A 'new_name' can be provided (in contrast to method 'copy_obj').
-        For further information on the input arguments, see methods 'get_obj' or
-        'get_single_obj'.
-
-        Returns the created copy.
-
-        See also 'copy_obj'
-        """
-        obj = self.handle_single_pf_object_or_path_input(obj_or_path,
-                                                         parent_folder=parent_folder,
-                                                         error_if_non_existent=error_if_non_existent)
-        target_folder = self.handle_single_pf_object_or_path_input(
-            target_folder)
-        if overwrite:
-            if not new_name:
-                self.delete_obj(obj.GetAttribute("loc_name"),
-                                parent_folder=target_folder, error_if_non_existent=False)
+        Raises:
+            powfacpy.PFPathInputError: If path is invalid.
+
+        Returns:
+            bool: True if path exists
+        """
+        
+        parent = self._folder if not parent else self._handle_single_pf_object_or_path_input(parent)
+        
+        splitted_path = path.split('\\')
+        if path[0] == "\\" or not splitted_path:
+            raise powfacpy.PFPathInputError(path)
+        existing_path = ""
+        child = parent
+        for child_name in splitted_path:
+            child = child.GetContents(f"{child_name}")
+            if child:
+                child = child[0]
+                existing_path = f"{existing_path}\\{child.loc_name}"
             else:
-                self.delete_obj(f"{new_name}.*",
-                                parent_folder=target_folder, error_if_non_existent=False)
-        if new_name:
-            return target_folder.AddCopy(obj, new_name)
-        else:
-            return target_folder.AddCopy(obj)
+                if not return_info:
+                    return False
+                else:
+                    parent_path = parent.GetFullName()
+                    parent_path = PFStringManipulation.remove_class_names(
+                        parent_path)
+                    existing_path = f"{parent_path}{existing_path}"
+                    non_existent_child_name = child_name
+                    return False, existing_path, non_existent_child_name
+        return True
+    
+    
+    def get_path_of_object(self, obj:Union[PFGeneral, PFFolder]) -> str:
+        """Get path relative to 'self._folder' without class names.
+        
+        Args:
+            obj (PFGeneral): PF object
 
-    def is_container(self, obj):
-        """Checks whether a PF object is a container. It is assumed
-        that an object is a container if it has the attribute 'contents'.
+        Returns:
+            str: path
         """
-        obj = self.handle_single_pf_object_or_path_input(obj)
-        return obj.HasAttribute("contents")
+        obj = self._handle_single_pf_object_or_path_input(obj)
+        return PFStringManipulation.remove_class_names(self.get_path_of_obj_with_class_names(obj))
+
+
+    def get_path_of_obj_with_class_names(
+        self, 
+        obj:Union[PFGeneral, PFFolder, str]) -> str:
+        """Get path relative to 'self._folder' including class names.
+
+        Args:
+            obj (Union[PFGeneral, PFFolder, str]): PF object
+
+        Returns:
+            str: path
+        """
+        _folder_path_without_closing_tag = PFStringManipulation.remove_closing_html_tag_from_path(str(self._folder))
+        obj = self._handle_single_pf_object_or_path_input(obj)
+        obj_str = PFStringManipulation.remove_closing_html_tag_from_path(str(obj))
+        return PFStringManipulation.truncate_beginning(
+            obj_str, _folder_path_without_closing_tag)
+    
+
+    def get_full_path_of_object(self, obj:Union[PFGeneral, PFFolder]) -> str:
+        """Get full path in PF database without class names.
+
+        Args:
+            obj (PFGeneral): PF object
 
-    def activate_study_case(self, path):
-        """Activate study case under path.
+        Returns:
+            str: path
         """
-        study_case = self.get_single_obj(path)
-        study_case.Activate()
-        return study_case
-
-    def add_results_variable(self, obj, variables, results_obj=None):
-        """Adds variables of the object to the PowerFactory results object (ElmRes)
-        obj: PowerFactory object or its path
+        obj = self.get_full_path_of_object_with_class_names(obj)
+        return PFStringManipulation.remove_class_names(obj)
+    
+    
+    def get_full_path_of_object_with_class_names(
+        self, 
+        obj:Union[PFGeneral, PFFolder, str]) -> str:
+        """Get path in PF database including class names.
+
+        Args:
+            obj (PFGeneral): PF object
+
+        Returns:
+            str: path
         """
-        if not results_obj:
-            results_obj = self.get_from_study_case("ElmRes")
-        else:
-            results_obj = self.handle_single_pf_object_or_path_input(
-                results_obj)
-        obj = self.handle_single_pf_object_or_path_input(obj)
-        if isinstance(variables, str):
-            variables = [variables]
-        for var in variables:
-            results_obj.AddVariable(obj, var)
-        results_obj.Load()
-        return results_obj
-
-    def clear_elmres_from_objects_with_status_deleted(self, results_obj=None):
-        """Deletes all objects from a results object (ElmRes) that have the
-        status deleted (i.e. attribute 'obj_id' is deleted).
-        """
-        if not results_obj:
-            results_obj = self.app.GetFromStudyCase("ElmRes")
-        obj_in_elmres = results_obj.GetContents("*")
-        for o in obj_in_elmres:
-            obj_id = o.obj_id
-            if obj_id.IsDeleted():
-                o.Delete()
-
-    def get_parameter_value_string(self, parameters, delimiter=" "):
-        param_value_string = ""
-        for parname, path_with_par in parameters.items():
-            value = self.get_attr_by_path(path_with_par)
-            param_value_string += parname + "=" + str(value) + delimiter
-        return param_value_string[:-len(delimiter)]  # omit last delimiter
-
-    def _replace_special_PF_characters_in_path_string(self, path):
-        """Replaces special characters '$(ExtDataDir)','$(WorkspaceDir)','$(InstallationDir)'
-        in a path string with their actual directories.
+        obj = self._handle_single_pf_object_or_path_input(obj)
+        return PFStringManipulation.remove_html_tags_from_path(str(obj))
+    
+    
+    def get_path_of_object_in_active_project(
+        self, 
+        obj:Union[PFGeneral, PFFolder, str]) -> str:
+        """Get path relative to active project without class names.
+        
+        Args:
+            obj (PFGeneral): PF object
+
+        Returns:
+            str: path
+        """
+        obj = self.get_path_of_object_in_active_project_with_class_names(obj)
+        return PFStringManipulation.remove_class_names(obj)
+    
+    
+    def get_path_of_object_in_active_project_with_class_names(
+        self, 
+        obj:Union[PFGeneral, PFFolder, str]) -> str:
+        """Get path relative to active project including class names.
+
+        Args:
+            obj (Union[PFGeneral, PFFolder, str]): PF object or its path
+
+        Returns:
+            str: path
+        """
+        active_project_path = PFStringManipulation.remove_closing_html_tag_from_path(str(self.app.GetActiveProject()))
+        obj = self._handle_single_pf_object_or_path_input(obj)
+        obj_str = PFStringManipulation.remove_closing_html_tag_from_path(str(obj))
+        return PFStringManipulation.truncate_beginning(
+            obj_str, active_project_path)
+    
+
+    def _replace_special_PF_characters_in_path_string(self, path:str) -> str:
+        """Replaces special characters '$(ExtDataDir)','$(WorkspaceDir)','$(InstallationDir)' in path with their actual directories.
         """
         if "$(ExtDataDir)" in path:
             project_settings = self.get_project_settings()
             ext_data_dir = self.get_attr(project_settings, "extDataDir")
             path = path.replace("$(ExtDataDir)", ext_data_dir)
         path = path.replace("$(WorkspaceDir)",
                             self.app.GetWorkspaceDirectory())
         return path.replace("$(InstallationDir)", self.app.GetInstallationDirectory())
 
-    def get_project_settings(self):
-        """Returns project settings object.
-        """
-        project_settings_folder = self.get_single_obj("*.SetFold")
-        return self.get_single_obj("*.SetPrj", parent_folder=project_settings_folder)
-
-    @staticmethod
-    def replace_headers_of_csv_file_with_number_of_colums(file_path):
-        """Replaces the first row (headers) of a csv file with its number of
-        columns. This is needed for import of csv files to PF using ElmFile.
-        """
-        with open(file_path+".csv") as read_file, open(file_path + ".temp", "w") as write_file:
-            columns_of_first_row = read_file.readline().split(",")
-            if columns_of_first_row[-1] == "\n":
-                columns_of_first_row = columns_of_first_row[:-1]
-            # Minus one because first column is time and should not be counted.
-            number_of_columns = len(columns_of_first_row)-1
-            write_file.write(str(number_of_columns)+"\n")
-            row = read_file.readline()
-            while row:
-                write_file.write(row)
-                row = read_file.readline()
-        replace(file_path + ".temp", file_path+".csv")
-        return number_of_columns
 
-    @staticmethod
-    def insert_row_with_number_of_columns_in_csv_file(file_path):
-        """Gets the number of columns of the first row in a csv file and
-        inserts a row (first row) with this number in the first column.
-        This is needed for ElmFile to read csv files.
-        """
-        with open(file_path+".csv") as read_file, open(file_path + ".temp", "w") as write_file:
-            first_row = read_file.readline()
-            columns_of_first_row = first_row.split(",")
-            if columns_of_first_row[-1] == "\n":
-                columns_of_first_row = columns_of_first_row[:-1]
-            # Minus one because first column is time and should not be counted.
-            number_of_columns = len(columns_of_first_row)-1
-            write_file.write(str(number_of_columns)+"\n")
-            write_file.write(first_row)
-            row = read_file.readline()
-            while row:
-                write_file.write(row)
-                row = read_file.readline()
-        replace(file_path + ".temp", file_path+".csv")
-        return number_of_columns
+    def get_path_between_objects(
+        self, 
+        obj_high:Union[PFGeneral, PFFolder, str], 
+        obj_low:Union[PFGeneral, PFFolder, str]) -> str:
+        """Get path between two objects in the PF database.
+
+        Args:
+            obj_high (Union[PFGeneral, PFFolder, str]): object higher in the hierarchy
+            obj_low (Union[PFGeneral, PFFolder, str]): object lower in the hierarchy
 
-    def get_upstream_obj(self,
-                         obj_or_path,
-                         condition,
-                         error_if_non_existent=True):
-        """Returns the upstream object that meets the condition.
-        Goes up step by step to the parent folders until the condition is met.
-        Arguments:
-          obj_or_path: Object (or its path) to start from.
-          condition: lamba function with condition for parent object.
-          error_if_non_existent: If True, an exception is raised if no upstream 
-            object is found. If False, None is then returned.
+        Returns:
+            str: path between
         """
-        obj_or_path = self.handle_single_pf_object_or_path_input(obj_or_path)
-        obj_or_path = obj_or_path.GetParent()
-        if obj_or_path:
-            if condition(obj_or_path):
-                return obj_or_path
-            else:
-                return self.get_upstream_obj(obj_or_path, condition)
-        else:
-            if error_if_non_existent:
-                raise Exception(
-                    "There is no upstream object that fullfills the condition.")
-            else:
-                return None
-
-    def get_path_between_objects(self, obj_high, obj_low):
-        """Returns the path between two objects in the database.
-        Arguments:
-          object_high: Object higher in the hierarchy.
-          object_low: Object lower in the hierarchy. 
-        """
-        obj_high = self.handle_single_pf_object_or_path_input(obj_high)
-        obj_high = PFStringManipulation._format_full_path(str(obj_high), self)
-        obj_low = self.handle_single_pf_object_or_path_input(obj_low)
-        obj_low = PFStringManipulation._format_full_path(str(obj_low), self)
+        obj_high = self._handle_single_pf_object_or_path_input(obj_high)
+        obj_high = self.get_path_of_object(obj_high)
+        obj_low = self._handle_single_pf_object_or_path_input(obj_low)
+        obj_low = self.get_path_of_object(obj_low)
         path = str(obj_low).split(str(obj_high))[1][1:]
         return path
 
+
     @staticmethod
-    def get_loc_name_with_class(powerfactory_objects):
+    def get_loc_name_with_class(
+        objects:Union[PFGeneral, list[PFGeneral]]) -> Union[str, list[str]]:
+        """Get local name (loc_name) including class.
 
+        Args:
+            objects (Union[PFGeneral, list[PFGeneral]]): PF objects(s)
+
+        Returns:
+            Union[str, list[str]]: local name(s)
+        """
         is_list = True
-        if not type(powerfactory_objects) == list:
-            powerfactory_objects = [powerfactory_objects,]
+        if not type(objects) == list:
+            objects = [objects,]
             is_list = False
 
         loc_name_with_class = []
-        for powerfactory_object in powerfactory_objects:
+        for powerfactory_object in objects:
             loc_name_with_class.append(
                 powerfactory_object.loc_name
                 + '.'
                 + powerfactory_object.GetClassName())
 
         if not is_list:
             loc_name_with_class = loc_name_with_class[0]
         return loc_name_with_class
 
-    def create_comtrade_obj(self, file_path: str, parent_folder=None):
-        """Add an IntComtrade that refers to file_path (*.cfg).
-        The objects are stored in a folder "Comtrade" in the currently active
-        study case, unless a parent_folder is provided. A new object is only
-        created if there exists no object yet that points to the same file
-        (f_name attribute is the file path). The file name is used for the
-        new object name (without the .cfg ending).
-        """
-        if parent_folder:
-            parent_folder = self.handle_single_pf_object_or_path_input(
-                parent_folder)
-        else:
-            parent_folder = self.app.GetFromStudyCase("Comtrade.IntFolder")
-
-        intcomtrade = self.get_obj("*.IntComtrade",
-                                   parent_folder=parent_folder,
-                                   condition=lambda x: getattr(
-                                       x, "f_name") == file_path,
-                                   error_if_non_existent=False)
-        if not intcomtrade:
-            _, file_name = os_path.split(file_path)
-            intcomtrade = self.create_in_folder(parent_folder,
-                                                file_name.replace(".cfg", "") + ".IntComtrade", overwrite=False,
-                                                use_existing=False)
-            intcomtrade.f_name = file_path
-        else:
-            intcomtrade = intcomtrade[0]
-        # intcomtrade.Load() probably not required
-        return intcomtrade
-
-    def _handle_possible_attribute_not_set_error(self,
-                                                 possibly_not_secified_attr,
-                                                 attribute_description: str,
-                                                 e):
-        """Handles exception if an AttributeError was raised in a
-        method call on an attribute of a powfacpy class.
-        """
-        if not possibly_not_secified_attr:
-            raise powfacpy.PFAttributeNotSetError(attribute_description)
-        else:
-            raise AttributeError(e)
-
-
-class PFStringManipulation:
-
-    @staticmethod
-    def replace_between_characters(char1, char2, replacement: str, original: str):
-        """
-        Example:
-          Calling      
-            powfacpy.PFStringManipulation.replace_between_characters(
-              '.', 
-              '\\', 
-              '\\', 
-              'username.IntUser\\pow.facpy.\\powfacpy.tests.IntPrj\\Network Model.IntPrjfolder\\Network Data.IntPrjfolder\\test_base_interface\\Grid.ElmNet\\Terminal HV 1.ElmTerm'
-          would give the output:
-            'username\\pow.facpy\\powfacpy.tests\\Network Model\\Network Data\\test_base_interface\\Grid\\Terminal HV 1' 
-          Note the behavior when there are several '.' in between '\\' 
-          -> then the replacement starts after the last '.'
-        """
-        new_string = ""
-        is_after_char_1 = False
-        string_between_char_1_occurrences = ""
-        for c in original:
-            if c == char1:
-                is_after_char_1 = True
-                new_string += string_between_char_1_occurrences
-                string_between_char_1_occurrences = ""
-            elif c == char2:
-                if is_after_char_1:
-                    new_string += replacement
-                else:
-                    new_string += c
-                string_between_char_1_occurrences = ""
-                is_after_char_1 = False
-            if is_after_char_1:
-                string_between_char_1_occurrences += c
-            elif not c == char2:
-                new_string += c
-        return new_string
-
-    @staticmethod
-    def _remove_class_names(path):
-        return PFStringManipulation.replace_between_characters('.', '\\', '\\', path)
-
-    @staticmethod
-    def _get_path_inside_project_from_full_path(path: str, pf_interface):
-        """
-        Takes the full path (including user and project) and returns the path 
-        relative to the currently active project.
-        Example:
-          input path:  \\username.IntUser\\powfacpy_base.IntPrj\\Network Model.IntPrjfolder\\Network Data.IntPrjfolder\\Grid.ElmNet\\Terminal 1.ElmTerm</l3>
-          output: Network Model.IntPrjfolder\\Network Data.IntPrjfolder\\Grid.ElmNet\\Terminal 1.ElmTerm
-        """
-        project_name = pf_interface.app.GetActiveProject().loc_name + '.IntPrj\\'
-        path = PFStringManipulation.truncate_until(path, project_name)
-        # In case a closing tag occurs at the end of the path </l3> (e.g. when
-        # str() is called on a PF object) make sure this is removed.
-        if path[-1] == ">":
-            path = path[0:path.rfind("<")]
-        return path
-
-    @staticmethod
-    def truncate_until(original: str, string_pattern: str):
-        """
-        Truncate all characters until (and including) the occurence of string_pattern
-        in original.
-        """
-        return original[original.find(string_pattern)+len(string_pattern):]
 
-    @staticmethod
-    def truncate_beginning(original: str, string_pattern: str):
-        """
-        Truncate string_pattern if it occurs at the beginning of the
-        original string. Otherwise return original string.
-        """
-        index_where_pattern_begins = original.find(string_pattern)
-        if index_where_pattern_begins == 0:
-            return original[index_where_pattern_begins+len(string_pattern):]
-        else:
-            return original
-
-    @staticmethod
-    def _format_full_path(path, pf_interface):
-        """
-        Takes the full path (including user and project) and returns the path 
-        relative to the currently active project. Deletes class information.
-        Example:
-          input path:  \\username.IntUser\\powfacpy_base.IntPrj\\Network Model.IntPrjfolder\\Network Data.IntPrjfolder\\Grid.ElmNet\\Terminal 1.ElmTerm
-          output: Network Model\\Network Data\\Grid\\Terminal 1 
-        """
-        path = PFStringManipulation._get_path_inside_project_from_full_path(
-            path, pf_interface)
-        return PFStringManipulation._remove_class_names(path)
-
-    @staticmethod
-    def _format_variable_name(name: str) -> str:
-        """
-        Takes PF-generated csv export variable name and returns shortened version.
-        Example:
-          name: 's:u0 in kV'
-          output: 's:u0' 
+#####################
+# Other
+#####################   
+    def is_pf_class(self, class_name: str) -> bool:
+        """Checks if class_name is a valid PF class (using the class ID).
+        """
+        return self.app.GetClassId(class_name) != 0
+    
+    
+    def is_container(self, obj:Union[PFGeneral, PFFolder, str]) -> bool:
+        """Checks whether a PF object is a container. It is assumed
+        that an object is a container if it has the attribute 'contents'.
         """
-        return name.split(" ", 1)[0].replace("\"", "").replace("\n", "")  # get rid of description and quotation marks
+        obj = self._handle_single_pf_object_or_path_input(obj)
+        return obj.HasAttribute("contents")
+    
 
-    @staticmethod
-    def handle_path(path):
-        """Checks if path starts with \ (not accepted by most PF methods)
-        and also if 'path' is of type string.
+    def get_project_settings(self) -> SetPrj:
+        """Get project settings object.
         """
-        try:
-            if not path[0] == "\\":
-                return path
-            else:
-                return path[1:]
-        except (TypeError):
-            raise TypeError("Path must be of type string.")
-
-    @staticmethod
-    def replace_outside_or_inside_of_strings_in_a_string(
-            string: str,
-            replacements: dict,
-            outside=True):
-        """This method replaces parts of a string but only in the sections
-        of the original string that are either outside of strings. This is best
-        explained by example:
-        "p HV load >= 2 and 'This is a string inside the string'"
-        In this string the part 'This is a string inside the string'
-        is a string inside the original string and no replacements are
-        made in this part.
-
-        Arguments:
-          - string: The string that will be adjusted
-          - replacements: key-value pairs of matching strings and their replacement
+        project_settings_folder = self.get_single_obj("*.SetFold")
+        return self.get_single_obj(
+            "*.SetPrj", parent_folder=project_settings_folder)  
+        
+    
+    def get_active_project(self) -> IntPrj:
+        """Get currently active project. Throw an error if no project is active.
         """
-        if outside:
-            modulo_result = 0
-        else:
-            modulo_result = 1
-        string = PFStringManipulation.split_but_keep_delimiter(string, "'")
-        for n, part_of_string in enumerate(string):
-            if n % 2 == modulo_result:  # Even elemnts store the parts that are outside strings
-                for par_name, var_name in replacements.items():
-                    part_of_string = part_of_string.replace(par_name, var_name)
-                    string[n] = part_of_string
-        return "".join(string).strip()
-
-    @staticmethod
-    def split_but_keep_delimiter(string: str, delimiter: str):
-        """Uses the split() method to separate a string acoording
-        to a delimiter, but keeps the delimiter in the
-        separated strings (it is suprising that this is not optional
-        in the split() method).
-        Example:
-          split_but_keep_delimiter(
-            "p HV load >= 2 and (control 1 == 'A' and control 2 != 'S')",
-            delimiter: "'")
-          returns 
-            ["p HV load >= 2 and (control 1 == '", "A'", " and control 2 != '", "S'", ')']
-        """
-        split_strings_list = [part + delimiter
-                              for part in string.split(delimiter)]
-        split_strings_list[-1] = split_strings_list[-1].rstrip(delimiter)
-        return split_strings_list
-
-
-class PFTranslator:
-
-    @staticmethod
-    def get_default_result_object_name(language):
-        if language == "en":
-            return "All calculations.ElmRes"
-        elif language == "de":
-            return "Alle Berechnungsarten.ElmRes"
-
-    @staticmethod
-    def get_default_graphics_board_name(language):
-        if language == "en":
-            return "Graphics Board.SetDesktop"
-        elif language == "de":
-            return "Grafiksammlung.SetDesktop"
-
-    @staticmethod
-    def get_default_study_case_folder_name(language):
-        if language == "en":
-            return "Study Cases.IntPrjfolder"
-        elif language == "de":
-            return "Berechnungsfälle.IntPrjfolder"
-
-    @staticmethod
-    def get_default_operation_scenario_folder_path(language):
-        if language == "en":
-            return r"Network Model\Operation Scenarios"
-        elif language == "de":
-            return r"Netzmodell\Betriebsfälle"
-
-    @staticmethod
-    def get_default_variations_folder_path(language):
-        if language == "en":
-            return r"Network Model\Variations"
-        elif language == "de":
-            return r"Netzmodell\Varianten"
-
-    @staticmethod
-    def _get_language_dependent_name_from_studycase(
-            studycase, english_name, german_name):
-        studycase_contents = powfacpy.PFTranslator.\
-            get_name_with_ending(
-                studycase.GetContents())
-        has_english_name = english_name in studycase_contents
-        has_german_name = german_name in studycase_contents
-        assert not (has_english_name and has_german_name), \
-            'Two redundant file versions: English and German named files exist.'
-        if has_english_name:
-            return english_name
+        active_project = self.app.GetActiveProject()
+        if active_project:
+            return active_project
         else:
-            return german_name
-
-    @staticmethod
-    def get_graphics_board_name_from_studycase(studycase):
-        name = powfacpy.PFTranslator.\
-            _get_language_dependent_name_from_studycase(
-                studycase=studycase,
-                english_name="Graphics Board.SetDesktop",
-                german_name="Grafiksammlung.SetDesktop",
-            )
-        return name
+            raise powfacpy.PFNotActiveError("a project")      
 
-    @staticmethod
-    def get_result_object_name_from_studycase(studycase):
-        name = powfacpy.PFTranslator.\
-            _get_language_dependent_name_from_studycase(
-                studycase=studycase,
-                english_name="All calculations.ElmRes",
-                german_name="Alle Berechnungsarten.ElmRes",
-            )
-        return name
-
-    @staticmethod
-    def get_name_with_ending(objects):
-        if not type(objects) == list:
-            objects = [objects]
-        return [x.GetFullName().split('\\')[-1] for x in objects]
-
-
-def set_attr_of_obj(obj, attributes: dict):
-    """Set attributes of object.
-    The difference to set_attr of PFBaseInterface is that
-    this method only accepts PF objects (and not path strings)
-    and is slightly more performant.
-    """
-    for attr, value in attributes.items():
-        obj.SetAttribute(attr, value)
-
-
-def set_attr_of_objects(objects: Iterable, attributes: Iterable):
-    """Set attributes of multiple objects.
-    """
-    for obj in objects:
-        set_attr_of_obj(obj, attributes)
-
-
-def set_attr_of_child(parent, child: str, attributes: dict):
-    """Set attributes of a child object in parent.
-    Just syntactic sugar.
-    """
-    child = parent.GetContents(child)[0]
-    for attr, value in attributes.items():
-        child.SetAttribute(attr, value)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `powfacpy-0.1.4/src/powfacpy/database_interface.py` & `powfacpy-0.1.5/src/powfacpy/database_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 The database interface is helpful to interact with larger numbers
 of PF objects in the database (getting, setting, storing or comparing
 attributes).
 One use case is for example to define a set of standard parameters for a
-larger model. Using the interface, one can easily get, store (e.g. in a json file)
-and later reset a set of parameters.
+larger model. Using the interface, one can easily get, store (e.g. in a json file) and later reset a set of parameters.
 
 ToDo: Add tutorial for this interface (when there is more functionality).
 """
-
-
 import sys
+from fnmatch import fnmatchcase
+
 sys.path.insert(0, r'.\src')
 import powfacpy
-from fnmatch import fnmatchcase
 
-class PFDatabaseInterface(powfacpy.PFBaseInterface):
-  language = powfacpy.PFBaseInterface.language
+
+class PFDatabaseInterface(powfacpy.PFActiveProject):
   
   def __init__(self, app):
     super().__init__(app)
 
   def get_object_attributes(
       self,
       objs,
@@ -63,19 +61,19 @@
             "loc_name": "Cub_1"
       },
     }
     """
     if not class_attributes:
       class_attributes = {"*": []} # no relevant attributes -> get only keys (object paths)
     if truncated_path: # include class names in truncated_path
-      truncated_path = self.get_path_of_obj_with_class_names_relative_to_project(truncated_path)  
+      truncated_path = self.get_path_of_obj_with_class_names(truncated_path)  
 
     obj_attr_dict = {}
     for obj in objs:
-      obj_path = self.get_path_of_obj_with_class_names_relative_to_project(obj)
+      obj_path = self.get_path_of_obj_with_class_names(obj)
       if truncated_path: 
         obj_path = powfacpy.PFStringManipulation.truncate_until(
           obj_path,truncated_path + "\\") 
       obj_attr_dict[obj_path] = {}
       for class_name in class_attributes.keys():
         if fnmatchcase(obj.GetClassName(), class_name): # fnmatch allows to use wildcards ("*")
           for attr in class_attributes[class_name]:
@@ -96,19 +94,19 @@
       - obj_attr_dict: data
       - added_path: Assumes that the object paths are relative to a parent 
         folder inside the project. Adds added_path to the paths. 
     """
     for obj, attr_key_val in obj_attr_dict.items():
       if added_path:
         obj = added_path + "\\" + obj
-      obj = self.get_unique_obj(obj)
+      obj = self.get_unique_obj(obj, include_subfolders=False)
       for attr, value in attr_key_val.items():
         if isinstance(value, str):
-          if not isinstance(obj.GetAttributeType(attr), str): # Then a PF objeczt is expected
-            value_pf_obj = self.get_unique_obj(value, error_if_non_existent=False)
+          if not isinstance(obj.GetAttributeType(attr), str): # Then a PF object is expected
+            value_pf_obj = self.get_unique_obj(value, error_if_non_existent=False, include_subfolders=False)
             if value_pf_obj:
               value = value_pf_obj    
         self.set_attr(obj, {attr: value})  
 
   def _handle_attribute_type_for_reading(
       self,
       obj,
@@ -130,16 +128,16 @@
     """
     attr_value = self.get_attr(obj,attr)
     if isinstance(attr_value, (str, int, float)) or not attr_value:
       return attr_value
     else: # Then it must be a PF object
       if pf_obj_handling == "path":
         if truncated_path:
-          truncated_path = self.get_path_of_obj_with_class_names_relative_to_project(truncated_path)    
-        return self.get_path_of_obj_with_class_names_relative_to_project(attr_value)
+          truncated_path = self.get_path_of_obj_with_class_names(truncated_path)    
+        return self.get_path_of_obj_with_class_names(attr_value)
       elif pf_obj_handling == "original_pf_obj":
         return attr_value 
 
 
   # Todo: define standard class attributes
   def get_standard_class_attributes():
     return {
```

### Comparing `powfacpy-0.1.4/src/powfacpy/dyn_sim_interface.py` & `powfacpy-0.1.5/src/powfacpy/dyn_sim_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,151 @@
-import sys
-sys.path.insert(0, r'.\src')
-import powfacpy
+from warnings import warn
+from os import getcwd, remove
+
+import pandas as pd
 
+import powfacpy
+from powfacpy.pf_class_protocols import PFGeneral, ComMod, ElmRes, ComRes
 
-class PFDynSimInterface(powfacpy.PFBaseInterface):
+class PFDynSimInterface(powfacpy.PFActiveProject):
+  """Dynamic simulation interface"""
   
   def __init__(self, app): 
     super().__init__(app) 
-    
+ 
 
   def initialize_sim(self, param=None):
     """
     Initialize time domain simulation.
     Parameters for 'ComInc' command object can be specified in 'param' dictionary.
     """
     cominc = self.app.GetFromStudyCase("ComInc")
     if param is not None:
       self.set_attr(cominc, param)
     cominc.Execute()
 
+
   def run_sim(self, param=None):
     """
     Perform dynamic simulation.
     Parameters for 'ComSim' command object can be specified in 'param' dictionary.
     """
     comsim = self.app.GetFromStudyCase("ComSim")
     if param is not None:
       self.set_attr(comsim, param)
     comsim.Execute()
 
+
   def initialize_and_run_sim(self):
     """Initialize and perform time domain simulation."""
     self.initialize_sim()
     self.run_sim()
+    
+    
+  def get_eigenvalues_of_current_state(
+    self, 
+    commod_parameters: dict[str, object] = {}) -> pd.DataFrame:
+    """Get the eigenvalues of the current state of the system.
+    
+    Uses the modal analysis command (ComMod) to calculate the eigenvalues. Eigenvectors and participation factors are omitted). The operating point of the current simulaiton time is used.
+    Then uses result export (ComRes) to export the eigenvalues to csv, which is then read to a pandas DataFrame.
 
-  
-  """
-  def create_reference_signal(self, path, points):
-    composite_model = self.create_by_path(path + ".ElmComp")
-    composite_frame = self.get_obj(self.dynamic_model_teamplates_path +
-      r"\reference_signal_frame")
-    composite_model.SetAttribute("typ_id", composite_frame)
-    dsl_obj = self.create_in_folder(composite_model,"lin_interpol_model.ElmDsl")
-    lin_interpol_model = self.get_obj(self.dynamic_model_teamplates_path +
-      r"\Linear_interpolation")
-    dsl_obj.SetAttribute("typ_id", lin_interpol_model)
-    set_dsl_obj_matrix(dsl_obj, points)
-    composite_model.SetAttribute("pelm",[dsl_obj])
-  """
+    Args:
+        commod_parameters (dict[str, str], optional): Additional parameter settings of modal analysis command (ComMod). Defaults to {}.
 
-  def create_event(self, name_incl_class, params={}, parent_folder=None, overwrite=True):
+    Returns:
+        pd.DataFrame: pandas DataFrame with columns "real in 1/s", "imag in rad/s"
+    """
+    commod: ComMod = self.get_from_study_case("ComMod")
+    commod.iLeft = False
+    commod.iRight = False
+    commod.iPart = False
+    commod.initMode = 0
+    if commod_parameters:
+      self.set_attr(commod, commod_parameters)
+    commod.Execute()
+    
+    elmres: ElmRes = commod.ResultFile
+    comres: ComRes = self.app.GetFromStudyCase("ComRes")      
+    comres.pResult = elmres
+    comres.iopt_csel = 0 # export all variables
+    comres.f_name = getcwd() + "\\temp.csv"
+    try:
+      comres.Execute()
+      df = pd.read_csv(comres.f_name, encoding='ISO-8859-1', header=[0,1], index_col=0)
+    finally:
+      remove(comres.f_name)  
+    df.columns = ["real in 1/s", "imag in rad/s"]  
+    return df   
+
+
+  def create_dyn_sim_event(self, 
+                   name_incl_class: str, 
+                   params: dict[str, object] = {}, 
+                   parent_folder: PFGeneral | str = None, 
+                   overwrite: bool = True):
+    """Creates an event for dynamic simulations (RMS/EMT) and sets the parameters in 'params'.
+
+    Args:
+        name_incl_class (str): Event name including the class.
+        
+        params (dict, optional): Paramter-values dictionary for created event object. Defaults to {}.
+        
+        parent_folder (PFGeneral | str, optional): Folder where event is created. If None, the events folder from the initial conditions calculation (ComInc) is used. Defaults to None.
+        
+        overwrite (bool, optional): Overwrite existing event with same name. Defaults to True.
+    """
+    if not parent_folder:
+      parent_folder = self.get_events_folder_from_initial_conditions_calc()
+    event_obj = self.create_in_folder(name_incl_class, parent_folder, overwrite=overwrite)
+    self.set_attr(event_obj, params)  
+    
+      
+  def create_event(self, 
+                   name_incl_class, 
+                   params={}, 
+                   parent_folder=None, 
+                   overwrite=True):
     """Creates an event and sets the parameters in 'params'.
+    
     Arguments:
       name_incl_class: Event name including the class.
       params: Paramter-values dictionary.
-      parent_folder: If None, the events folder from the active study case is used.
+      parent_folder: If None, the events folder from the initial conditions calculation (ComInc) is used.
       overwrite: Oerwrite existing event with same name.
     """
-    if not parent_folder:
-      parent_folder = self.app.GetFromStudyCase("IntEvt")
-    event_obj = self.create_in_folder(parent_folder, name_incl_class, overwrite=overwrite)
-    self.set_attr(event_obj, params)  
+    warn(f'{self.create_event.__name__} will be deprecated. Please use the method create_dyn_sim_event instead.',
+             DeprecationWarning, stacklevel=2)
+    self.create_dyn_sim_event(name_incl_class, 
+                              params, 
+                              parent_folder,
+                              overwrite) 
+   
 
   def get_dsl_model_parameter_names(self, dsl_model):
     """
     Get the parameter names of the block definition (BlkDef)
     of a dsl model.
     """
-    dsl_model = self.handle_single_pf_object_or_path_input(dsl_model)
+    dsl_model = self._handle_single_pf_object_or_path_input(dsl_model)
     try: 
       parameter_names = dsl_model.typ_id.sParams
       if parameter_names:
         return parameter_names[0].split(",")
     except AttributeError:
       msg = "Attribute 'typ_id' is of type 'None'"
       raise powfacpy.PFObjectAttributeTypeError(dsl_model, msg, self)
   
+  
   def get_dsl_models_inside_composite_model(self, composite_model):
     return self.get_obj("*.ElmDsl", 
                         parent_folder=composite_model,
                         include_subfolders=True)
   
+  
   def get_parameters_of_dsl_models_in_composite_model(
       self, 
       composite_model,
       single_dict_for_all_dsl_models = False,
       ):
     """
     Returns a dictionary with the parameter names (of the block definition) 
@@ -102,15 +163,15 @@
         - If false, the returned dictionary contains dictionaries for each dsl model.
         Example:
           {
           "controller_a": {"a": 1, "b":0}
           "controller_b": {"a": 5, "c":2}
           } 
     """
-    composite_model = self.handle_single_pf_object_or_path_input(composite_model)
+    composite_model = self._handle_single_pf_object_or_path_input(composite_model)
     dsl_models = self.get_dsl_models_inside_composite_model(composite_model)
     all_models_params_dict = {}
     for dsl_model in dsl_models:
       parameter_names_incl_dsl_lookup = self.get_dsl_model_parameter_names(dsl_model)
       # Ignore dsl lookup arrays/matrices
       parameter_names = []
       if parameter_names_incl_dsl_lookup:
@@ -133,14 +194,15 @@
                                     **parameter_names_and_values}
         else:
           all_models_params_dict[dsl_model.loc_name] = parameter_names_and_values
       elif not single_dict_for_all_dsl_models:
         all_models_params_dict[dsl_model.loc_name] = {}  
     return all_models_params_dict
 
+
   def set_parameters_of_dsl_models_in_composite_model(
       self, 
       composite_model,
       models_params_dict,
       single_dict_for_all_dsl_models = False,
       ):
     """
@@ -157,44 +219,47 @@
         - If false, models_params_dict contains dictionaries for each dsl model.
         Example:
           {
           "controller_a": {"a": 1, "b":0}
           "controller_b": {"a": 5, "c":2}
           } 
     """
-    composite_model = self.handle_single_pf_object_or_path_input(composite_model)
+    composite_model = self._handle_single_pf_object_or_path_input(composite_model)
     if not single_dict_for_all_dsl_models:
       for dsl_model, parameter_value_dict in models_params_dict.items():
         dsl_model = self.get_unique_obj(dsl_model+".ElmDsl", 
                                         parent_folder=composite_model,
                                         include_subfolders=True)
         self.set_attr(dsl_model, parameter_value_dict)
     else:
       dsl_models = self.get_dsl_models_inside_composite_model(composite_model)
       for dsl_model in dsl_models:
         for param_name, value in models_params_dict.items(): 
           if dsl_model.HasAttribute(param_name):
             dsl_model.SetAttribute(param_name, value)   
 
+
   @staticmethod
   def is_dsl_lookup_arrays_and_matrices_name(string: str):
     """
     dsl has a special variable type for lookup tables. Such variables
     are defined using certain variable names starting with e.g. 'array_'.
     """
     is_dsl_lookup = False
     for dsl_lookup_name in PFDynSimInterface.get_dsl_lookup_arrays_and_matrices_names():
       if dsl_lookup_name in string:
         is_dsl_lookup = True
     return is_dsl_lookup    
 
+
   @staticmethod
   def get_dsl_lookup_arrays_and_matrices_names():
     return ["oarray_", "array_", "matrix", "omatrix"]
 
+
   @staticmethod 
   def set_dsl_obj_array(dsl_obj,
                         rows,
                         array_num=None,
                         size_included_in_array=True): 
     """Set the array of a DSL object ('Advanced 1' tab).
     The array_num specifies which array is set (if None,
@@ -218,14 +283,15 @@
         dsl_obj.SetAttribute(attrib, row)
       else:
         complete_row = dsl_obj.GetAttribute(attrib)
         complete_row[(array_num-1)*2] = row[0]
         complete_row[(array_num-1)*2+1] = row[1]
         dsl_obj.SetAttribute(attrib, complete_row)
 
+
   @staticmethod 
   def get_dsl_obj_array(dsl_obj,
                         array_num=None,
                         size_included_in_array=True):
     """Get the array of DSL object ('Advanced 1' tab).
     The array_num specifies which array is returend (if None,
     all arays/colmns are returned).
```

### Comparing `powfacpy-0.1.4/src/powfacpy/engineering_helpers.py` & `powfacpy-0.1.5/src/powfacpy/engineering_helpers.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/src/powfacpy/exceptions.py` & `powfacpy-0.1.5/src/powfacpy/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,34 +9,33 @@
   from 'Exception') for all custom errors/exceptions.
   """
   pass
 
 class PFAttributeError(PFInterfaceError):
   """Attempt to access an invalid attribute of a PF object.
   """
-  def __init__(self, obj, msg_raised, pf_base_interface):
-    object_str = powfacpy.PFStringManipulation._format_full_path(str(obj), pf_base_interface)
+  def __init__(self, obj, msg_raised, pf_active_project: powfacpy.PFActiveProject):
+    object_str = pf_active_project.get_path_of_object(obj)
     self.message = (f"Unexpected attribute of object '{object_str}': {msg_raised}.")
     super().__init__(self.message)
 
 class PFObjectAttributeTypeError(PFInterfaceError):
   """Unexpected type of a PF object attribute (e.g. 'None' type).
   """
-  def __init__(self, obj, msg_raised, pf_base_interface):
-    object_str = powfacpy.PFStringManipulation._format_full_path(str(obj), pf_base_interface)
+  def __init__(self, obj, msg_raised, pf_active_project):
+    object_str = pf_active_project.get_path_of_object(obj)
     self.message = (f"Unexpected attribute of object '{object_str}': {msg_raised}.")
     super().__init__(self.message) 
      
 class PFAttributeTypeError(PFInterfaceError):
   """Attempt to set an invalid type for the attribute of a PF object.
   """
-  def __init__(self, obj, attr, msg_raised, pf_base_interface):
-    object_str = powfacpy.PFStringManipulation._format_full_path(str(obj), pf_base_interface)
-    self.message = (f"The attribute '{attr}' of the object '{object_str}' "
-      f"is of unexpected type: {msg_raised}.")
+  def __init__(self, obj, attr, msg_raised, pf_active_project):
+    object_str = pf_active_project.get_path_of_object(obj)
+    self.message = (f"The attribute '{attr}' of the object '{object_str}' is of unexpected type: {msg_raised}.")
     super().__init__(self.message)
 
 class PFPathError(PFInterfaceError):
   """Attempt to access invalid path in PF database.
   """
   def __init__(self, non_existing_child, existing_path):
     self.message = f"'{non_existing_child}' does not exist in '{existing_path}'"
@@ -47,24 +46,24 @@
   """
   def __init__(self, path):
     self.message = (f"The path '{path}' is invalid or empty. Please don't start " +
     f"the path with '\\'.")
     super().__init__(self.message)
 
 class PFNonExistingObjectError(PFInterfaceError):
-  """Attempt to access PF object that does not exist.
+  """Attempt to access PF object (optional: with a specific condition) that does not exist.
   """
   def __init__(self, folder, obj, condition=False, include_subfolders=False):
-    folder_str = powfacpy.PFStringManipulation._remove_class_names(str(folder))
+    folder_str = powfacpy.PFStringManipulation.remove_html_tags_from_path(str(folder))
+    folder_str = powfacpy.PFStringManipulation.remove_class_names(folder_str)
     if include_subfolders:
       msg_subfolder = " (and its subfolders)"
     else:
       msg_subfolder = ""
-    msg = (f"The folder '{folder_str}'{msg_subfolder} does not contain "
-      f"any object named '{obj}'")
+    msg = (f"The folder '{folder_str}'{msg_subfolder} does not contain any object or path named '{obj}'")
     if condition:
       msg = msg + " with specified condition"  
     self.message = msg
     super().__init__(self.message)
 
 class PFNotActiveError(PFInterfaceError):
   """Unexpected inactive PF object.
```

### Comparing `powfacpy-0.1.4/src/powfacpy/network_interface.py` & `powfacpy-0.1.5/src/powfacpy/network_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import sys
 sys.path.insert(0, r'.\src')
 import powfacpy
 
-class PFNetworkInterface(powfacpy.PFBaseInterface):
+class PFNetworkInterface(powfacpy.PFActiveProject):
     
   def __init__(self, app):
     super().__init__(app) 
 
   def get_vacant_cubicle_of_terminal(self, terminal, new_cubicle_name=None):
     """Gets the first vacant cubicle found in a terminal (i.e. nothing is connected
     to this cubicle).
     If there is no vacant cuibicle, a new cubicle is created.
 
     Arguments:
       terminal: ElmTerm
       new_cubicle_name: Name  that is set for the found or created cubicle 
     """
-    terminal = self.handle_single_pf_object_or_path_input(terminal)
+    terminal = self._handle_single_pf_object_or_path_input(terminal)
     cubicles = self.get_cubicles_of_terminal(terminal)
     for cubicle in cubicles:
       if cubicle.obj_id == None:
         if new_cubicle_name:
           cubicle.loc_name = new_cubicle_name
         return cubicle
     if not new_cubicle_name:
       new_cubicle_name = "Cub_"+str(len(cubicles)+1)     
-    return self.create_in_folder(terminal, new_cubicle_name+".StaCubic")
+    return self.create_in_folder(new_cubicle_name+".StaCubic", terminal)
 
   def get_cubicles_of_terminal(self, terminal, only_calc_relevant=False):
     if not only_calc_relevant:
       return self.get_obj("*", parent_folder=terminal,
         condition=lambda x: x.GetClassName() == "StaCubic")
     else:
       return terminal.GetCalcRelevantCubicles()
@@ -47,15 +47,15 @@
 
   def copy_grid(self, grid_or_path, target_folder, new_name,
     parent_folder=None,
     error_if_non_existent=True):
     """Copying a grid is not trivial in PF because the graphical network objects
     need to be copied and assigned manually as this is not done automatically.
     """
-    grid_to_be_copied = self.handle_single_pf_object_or_path_input(grid_or_path)
+    grid_to_be_copied = self._handle_single_pf_object_or_path_input(grid_or_path)
     new_grid = self.copy_single_obj(grid_to_be_copied, target_folder,
       overwrite=True,
       new_name=new_name,
       parent_folder=parent_folder,
       error_if_non_existent=error_if_non_existent)
     new_network_diagram = self.copy_single_obj(grid_to_be_copied.pDiagram,
       self.app.GetProjectFolder("dia"),new_name=new_name,overwrite=True)
@@ -66,10 +66,10 @@
       path_in_grid = self.get_path_between_objects(grid_to_be_copied, element)
       graphical_net_obj.pDataObj = self.get_single_obj(path_in_grid, parent_folder=new_grid)
     new_network_diagram.pDataFolder = new_grid
     new_grid.pDiagram = new_network_diagram
     return new_grid
 
   def get_parent_grid(self, obj_or_path):
-    obj_or_path = self.handle_single_pf_object_or_path_input(obj_or_path)
+    obj_or_path = self._handle_single_pf_object_or_path_input(obj_or_path)
     return self.get_upstream_obj(obj_or_path, lambda x: x.GetClassName == "IntNet")
```

### Comparing `powfacpy-0.1.4/src/powfacpy/plot_interface.py` & `powfacpy-0.1.5/src/powfacpy/plot_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,545 +1,663 @@
 """Plotting interface.
 """
 
 import sys
 sys.path.insert(0, r'.\src')
-import powfacpy
+from collections.abc import Iterable
+from os import getcwd
+from warnings import warn
+
 import pandas
 from matplotlib import pyplot
-from collections.abc import Iterable
-from os import getcwd, path
-from os import path as os_path
 
-class PFPlotInterface(powfacpy.PFBaseInterface):
+import powfacpy
+from powfacpy.pf_class_protocols import GrpPage, SetVipage, VisPlot, PltLinebarplot, PltVectorplot, SetDesktop, PFGeneral, PltDataseries, PltAxis,PltLegend, PltTitle, IntCase, ElmNet
+
+
+
+class PFPlotInterface(powfacpy.PFActiveProject):
 
   def __init__(self, app):
     super().__init__(app) 
-    self.active_graphics_page = None
-    self.active_plot = None
+    self.active_graphics_page: GrpPage | SetVipage = None
+    "Currently active graphics page."
+    self.active_plot: VisPlot | PltLinebarplot | PltVectorplot  = None
+    "Currently active plot."
 
 
-  def set_active_graphics_page(self, page):
+  def plot(self, 
+           obj: PFGeneral | str, 
+           variables: str | list[str], 
+           graphics_page: str | GrpPage | SetVipage = None, 
+           plot: str | VisPlot | PltLinebarplot | PltVectorplot = None,
+           **kwargs) -> None:
+    """Plots the variables of 'obj' to the currently active plot.
+    
+    Also adds the variables to the results (ElmRes) object.
+    The active plot can be set with the optional arguments.
+
+    Args:
+    
+      obj (PFGeneral): Object (e.g. of class 'Elm...') of which variables are plotted.
+      
+      variables (str | list[str]): string or list of variable names 
+      
+      graphics_page (str | GrpPage | SetVipage, optional): Defaults to None.
+      
+      plot (str | VisPlot | PltLinebarplot | PltVectorplot, optional): Plot object. Defaults to None.
+      
+      kwargs:
+      
+      results_obj: result object used (object or path)
+      linestyle: int
+      linewidth: double
+      color: int
+      label: str
+    """
+    obj = self._handle_single_pf_object_or_path_input(obj)
+    if "results_obj" in kwargs:
+      results_obj = kwargs["results_obj"]
+    else:
+      results_obj = None
+    self.add_results_variable(obj, variables, results_obj=results_obj)
+    self.plot_monitored_variables(obj, variables,
+      graphics_page=graphics_page, plot=plot,**kwargs) 
+    
+
+  def plot_monitored_variables(
+    self, 
+    obj: PFGeneral, 
+    variables: str | list[str],
+    graphics_page: str | GrpPage | SetVipage = None, 
+    plot: VisPlot | PltLinebarplot | PltVectorplot = None,
+    **kwargs) -> None:
+    """Plot varibales. Variables must have been added to the monitored
+    variables before (e.g. using 'add_results_variable').
+
+    Args:
+        obj (PFGeneral): Object (e.g. of class 'Elm...') of which variables are plotted.
+        
+        variables (str | list[str]): Variable(s) to be plotted.
+        
+        graphics_page (str | GrpPage | SetVipage, optional): Graphics page. Defaults to None.
+        
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): Plot object. Defaults to None.
+        
+        kwargs:
+          result_obj: result object used (object or path)
+          linestyle: int
+          linewidth: double
+          color: int
+          label: str
+    """
+    if graphics_page:
+      self.set_active_graphics_page(graphics_page)
+    if plot:
+      self.set_active_plot(plot)
+    data_series = self.get_data_series_of_active_plot()
+    if "results_obj" in kwargs:
+      data_series.SetAttribute("useIndividualResults", 1)
+    obj = self._handle_single_pf_object_or_path_input(obj)
+    if isinstance(variables, str):
+     variables = [variables]
+    for var in variables:
+      data_series.AddCurve(obj, var)
+      self.set_curve_attributes(data_series,**kwargs)
+    self.active_graphics_page.Show()
+
+
+  def set_active_graphics_page(self, page: str | GrpPage | SetVipage) -> None:
     """Sets the active graphics page.
-    Arguments:
-      page:graphics page  name.
+
+    Args:
+        page (str | GrpPage | SetVipage): graphics page object or name
     """
     if isinstance(page, str):
       grb = self.get_or_create_graphics_board()
       self.active_graphics_page = grb.GetPage(page,1,"GrpPage")
     else:
       self.active_graphics_page = page
 
 
-  def set_active_plot(self, name_or_obj, graphics_page=None):
-    """Set the currently active plot. Adjusts the active graphics
-    page accordingly if name_or_object is a PF plot object (the graphics
-    page cannot be infered from a string path) or if the
-    optional argument graphics_page is given.
-    Arguments:
-      name_or_obj: name of plot (string) or plot object.
-      graphics_page: name of grphics page (string). If  
-        specified, this sets the currently active page.
+  def set_active_plot(
+    self, 
+    name_or_obj: str | VisPlot | PltLinebarplot | PltVectorplot, 
+    graphics_page: GrpPage | SetVipage = None) -> None:
+    """Set the currently active plot. 
+    
+    Adjusts the active graphics page accordingly if 'name_or_object' is a PF plot object (the graphics page cannot be infered from a string path) or if the optional argument graphics_page is given.
+
+    Args:
+        name_or_obj (str): name of plot (string) or plot object
+        graphics_page (str | GrpPage | SetVipage, optional): Graphics page object or string. Defaults to None.
     """
     if graphics_page:
       self.set_active_graphics_page(graphics_page)
     if not isinstance(name_or_obj, str): # is plot object
       self.active_plot = name_or_obj
       self.set_active_graphics_page(self.active_plot.GetParent())
     else:
       try:
         self.active_plot = self.active_graphics_page.GetOrInsertCurvePlot(name_or_obj)
       except(AttributeError) as e:
         self._handle_possible_attribute_not_set_error(self.active_graphics_page,
           "active_grapics_page", e) 
 
-  def get_or_create_graphics_board(self):
+
+  def get_or_create_graphics_board(self) -> SetDesktop:
     """Get the graphics board of the currently active study case or create
     a new graphics board if it does not exist within the study case yet.
     """
     grb = self.app.GetGraphicsBoard()  
     if not grb:
-      active_study_case = self.app.GetActiveStudyCase()
-      graphics_board_name = powfacpy.PFTranslator.get_default_graphics_board_name(
-         self.language)
-      grb = self.create_in_folder(active_study_case, graphics_board_name)
+      grb = self.get_from_study_case("SetDesktop")
       grb.Show()
-      grb = self.app.GetGraphicsBoard() # get grb again to get correct object from PF
     return grb  
 
-
-  def plot_monitored_variables(self, obj, variables,
-    graphics_page=None, plot=None,**kwargs):
-    """Plot varibales that were already added to the monitored
-    variables.
-    Arguments:
-      obj: PowerFactory object or its path
-      variables: string or list of variable names 
-      graphics_page: name of graphics page
-      plot: name of plot
-      kwargs:
-        result_obj: result object used (object or path)
-        linestyle: int
-        linewidth: double
-        color: int
-        label: str
-    """
-    if graphics_page:
-      self.set_active_graphics_page(graphics_page)
-    if plot:
-      self.set_active_plot(plot)
-    data_series = self.get_data_series_of_active_plot()
-    if "results_obj" in kwargs:
-      data_series.SetAttribute("useIndividualResults", 1)
-    obj = self.handle_single_pf_object_or_path_input(obj)
-    if isinstance(variables, str):
-     variables = [variables]
-    for var in variables:
-      data_series.AddCurve(obj, var)
-      self.set_curve_attributes(data_series,**kwargs)
-    self.active_graphics_page.Show()
-
-  def get_data_series_of_active_plot(self):
-    """Get the dataseries of the currently active plot.
+  
+  def get_data_series_of_active_plot(self) -> PltDataseries:
+    """Get dataseries object of the currently active plot.
     """
     try:
       return self.active_plot.GetDataSeries()
     except(AttributeError) as e:
-      self._handle_possible_attribute_not_set_error(self.active_plot,
-          "active_plot", e)
+      self._handle_possible_attribute_not_set_error(
+        self.active_plot, "active_plot", e)
+
 
-  def get_x_axis_of_active_plot(self):
+  def get_x_axis_of_active_plot(self) -> PltAxis:
     """Get the x-axis of the currently active plot.
     """
     try:
       return self.active_plot.GetAxisX()
     except(AttributeError) as e:
       self._handle_possible_attribute_not_set_error(self.active_plot,
           "active_plot", e)
   
-  def get_y_axis_of_active_plot(self):
+  
+  def get_y_axis_of_active_plot(self) -> PltAxis:
     """Get the y-axis of the currently active plot.
     """
     try:
       return self.active_plot.GetAxisY()
     except(AttributeError) as e:
       self._handle_possible_attribute_not_set_error(self.active_plot,
           "active_plot", e)
 
-  def get_legend_of_active_plot(self): 
+
+  def get_legend_of_active_plot(self) -> PltLegend: 
     try:
       return self.active_plot.GetLegend()
     except(AttributeError) as e:
       self._handle_possible_attribute_not_set_error(self.active_plot,
           "active_plot", e) 
 
-  def get_title_obj_of_active_plot(self): 
+
+  def get_title_obj_of_active_plot(self) -> PltTitle: 
     try:
       return self.active_plot.GetTitleObject()
     except(AttributeError) as e:
       self._handle_possible_attribute_not_set_error(self.active_plot,
           "active_plot", e) 
       
-  def set_all_fonts_of_active_plot(self, fontsize=10, fontname="Arial", fontstyle=0):
-    """Sets the fonts of all text elements (axis labels,legend,title). Note that the 
-    fonts are not attributes of the PF objects (x-axis, title object,..), but can only be 
-    set using the method 'SetFont'.
-    """
-    self.get_x_axis_of_active_plot().SetFont(fontname,fontsize,fontstyle)
-    self.get_y_axis_of_active_plot().SetFont(fontname,fontsize,fontstyle) 
-    self.get_legend_of_active_plot().SetFont(fontname,fontsize,fontstyle)  
-    self.get_title_obj_of_active_plot().SetFont(fontname,fontsize,fontstyle)
-
-  def plot(self, obj, variables, graphics_page=None, plot=None,**kwargs):
-    """Plots the variables of 'obj' to the currently active plot.
-    Includes adding the variables to the results (ElmRes) object.
-    The active plot can be set with the optional arguments.
-    Arguments:
-      variables: string or list of variable names 
-      graphics_page: name of graphics page
-      plot: name of plot
-      kwargs:
-        results_obj: result object used (object or path)
-        linestyle: int
-        linewidth: double
-        color: int
-        label: str
-    """
-    obj = self.handle_single_pf_object_or_path_input(obj)
-    if "results_obj" in kwargs:
-      results_obj = kwargs["results_obj"]
-    else:
-      results_obj = None
-    self.add_results_variable(obj, variables, results_obj=results_obj)
-    self.plot_monitored_variables(obj, variables,
-      graphics_page=graphics_page, plot=plot,**kwargs) 
-  
+      
+  def set_all_fonts_of_active_plot(self, 
+                                   fontsize: int = 10, 
+                                   fontname: str = "Arial", 
+                                   fontstyle: int = 0) -> None:
+    """Sets the fonts of all text elements (axis labels,legend,title). 
+    
+    Note that the fonts are not attributes of the PF objects (x-axis, title object,..), but can only be set using the method 'SetFont'.
 
-  def set_curve_attributes(self, data_series,**kwargs):
-    """Set curve attributes.
-    Arguments:
-      data_series: data series of plot.
-      kwargs:
-        results_obj: result object used (object or path)
-        linestyle: int
-        linewidth: double
-        color: int
-        label: str
-    """
+    Args:
+        fontsize (int, optional): Defaults to 10.
+        fontname (str, optional): Defaults to "Arial".
+        fontstyle (int, optional): Defaults to 0.
+    """
+    self.get_x_axis_of_active_plot().SetFont(fontname, fontsize, fontstyle)
+    self.get_y_axis_of_active_plot().SetFont(fontname, fontsize, fontstyle) 
+    self.get_legend_of_active_plot().SetFont(fontname, fontsize, fontstyle)  
+    self.get_title_obj_of_active_plot().SetFont(fontname, fontsize, fontstyle)
+
+
+  def set_curve_attributes(self, 
+                           data_series: PltDataseries = None,
+                           curve_num: int = -1,
+                           **kwargs) -> None:
+    """Set curve attributes in dataseries object of a plot.
+
+    Args:
+        data_series (PltDataseries, optional): data series of plot. Defaults to None (dataseries of active plot is used).
+        
+        curve_num (int, optional): Curve number. Defaults to -1 (last curve).
+        
+        kwargs:
+          results_obj: result object used (object or path)
+          linestyle: int
+          linewidth: double
+          color: int
+          label: str
+    """
+    if curve_num > 0:
+      curve_num -= 1 
+    if not data_series:
+      data_series = self.get_data_series_of_active_plot()  
     if  "linestyle" in kwargs:
       list_curveTableAttr = data_series.GetAttribute("curveTableLineStyle")
-      list_curveTableAttr[-1] = kwargs['linestyle']
+      list_curveTableAttr[curve_num] = kwargs['linestyle']
       data_series.SetAttribute("curveTableLineStyle", list_curveTableAttr)
     if "linewidth" in kwargs:
       list_curveTableAttr = data_series.GetAttribute("curveTableLineWidth")
-      list_curveTableAttr[-1] = kwargs['linewidth']
+      list_curveTableAttr[curve_num] = kwargs['linewidth']
       data_series.SetAttribute("curveTableLineWidth", list_curveTableAttr)
     else:
       # The linewidth must be set to the standard value. Otherwise PF uses 
       # the value from the previous data series (this seems to be a PF bug).
       list_curveTableAttr = data_series.GetAttribute("curveTableLineWidth")
-      list_curveTableAttr[-1] = 100
+      list_curveTableAttr[curve_num] = 100
       data_series.SetAttribute("curveTableLineWidth", list_curveTableAttr)
     if "color" in kwargs:
       list_curveTableAttr = data_series.GetAttribute("curveTableColor")
-      list_curveTableAttr[-1] = kwargs['color']
+      list_curveTableAttr[curve_num] = kwargs['color']
       data_series.SetAttribute("curveTableColor", list_curveTableAttr)
     # The label must be handled differently because PF returns an empty list
     # if there haven't been any labels specified yet for any of the curves.
     if "label" in kwargs:
       list_curveTableAttr = data_series.GetAttribute("curveTableLabel")
       if list_curveTableAttr:
-        list_curveTableAttr[-1] = kwargs['label']
+        list_curveTableAttr[curve_num] = kwargs['label']
       else:
         list_curveTableAttr = [kwargs['label']]
       data_series.SetAttribute("curveTableLabel", list_curveTableAttr)
     if "results_obj" in kwargs:
       list_curveTableAttr = data_series.GetAttribute("curveTableResultFile")
-      list_curveTableAttr[-1] = self.handle_single_pf_object_or_path_input(
+      list_curveTableAttr[curve_num] = self._handle_single_pf_object_or_path_input(
         kwargs['results_obj'])
       data_series.SetAttribute("curveTableResultFile", list_curveTableAttr)
 
-  def set_x_axis_attributes(self,**kwargs):
-    """Set x-axis attributes.
-    Arguments:
-      key-value-pairs of axis-related PF attributes and the desired value.
-    """
-    self._set_axis_attributes(
-      self.get_x_axis_of_active_plot(),
-      kwargs)
-    
-  def set_y_axis_attributes(self, **kwargs):
+
+  def set_x_axis_attributes(self, **kwargs) -> None:
     """Set y-axis attributes.
-    Arguments:
-      key-value-pairs of axis-related PF attributes and the desired value.
+    
+    Args:
+      kwargs:
+        key-value-pairs of axis-related PF attributes and their value.
     """
-    self._set_axis_attributes(
-      self.get_y_axis_of_active_plot(),
-      kwargs)      
-    
-  def _set_axis_attributes(self, axis, kwargs):
-    """ set axis attributes for given axis. 
-    set_y_axis_attributes() and set_x_axis_attributes() use this funciton.
+    x_axis = self.get_x_axis_of_active_plot()
+    for attribute, value in kwargs.items():
+      x_axis.SetAttribute(attribute, value)
+    
+    
+  def set_y_axis_attributes(self, **kwargs) -> None:
+    """Set y-axis attributes.
+    
+    Args:
+      kwargs:
+        key-value-pairs of axis-related PF attributes and their value.
     """
+    y_axis = self.get_y_axis_of_active_plot()
     for attribute, value in kwargs.items():
-      axis.SetAttribute(attribute, value)      
+      y_axis.SetAttribute(attribute, value)    
+   
 
-  def set_x_axis_range_of_active_plot(self, range: Iterable):
+  def set_x_axis_range_of_active_plot(self, range: tuple[float]) -> None:
     self.set_x_axis_attributes(rangeMin=range[0], rangeMax=range[1])
 
-  def set_y_axis_range_of_active_plot(self, range: Iterable):
-    self.set_y_axis_attributes(rangeMin=range[0], rangeMax=range[1])  
-
-  def plot_from_comtrade(self,
-                      file_path,
-                      variables,
-                      graphics_page=None,
-                      plot=None,
-                      parent_folder_comtrade=None,
-                      **kwargs):
-    """Plot a varibale from a COMTRADE formated file under file_path (*.cfg).
-    Creates the comtrade object (IntComtrade) and plots.
-    
-    If you want to plot from a comtrade object (IntComtrade) that already 
-    exists in the PF database, use the method plot_monitored_variables as shown
-    in this method.
-    
-    Arguments:
-      file_path: str
-      variables: The entry in the second column of a signal in .cfg
-      parent_folder_comtrade: Container in PF database for comtrade objects
-        (str or PF object)
-         
-    For further info on the arguments see method plot_monitored_variables.  
-    """                  
-    intcomtrade = self.create_comtrade_obj(file_path,
-      parent_folder=parent_folder_comtrade)
-    self.plot_monitored_variables(intcomtrade,
-              variables,
-              graphics_page=graphics_page,
-              plot=plot,
-              results_obj=intcomtrade,
-              **kwargs)
 
-  def plot_from_csv_using_elm_file(self, file_path, variable,**kwargs):
-    """Use an ElmFile object to plot data from csv file.
-    The ElmFiles are stored in a dummy network because the simulation needs to be run
-    to read the data from the csv file and is not just printed to the plot automatically.
-    """
-    # Deactivate currently active networks
-    active_networks = self.get_active_networks(
-      error_if_no_network_is_active=False)
-    for network in active_networks:
-      network.Deactivate()
-    # Activate dummy network
-    elmfiles_network = self.create_dummy_network("network_for_elmfiles")  
-    elmfiles_network.Activate()  
-    # Add new ElmFile
-    elmfile_num = 1
-    while True:
-      existing_elmfile = self.get_single_obj("elmfile_"+str(elmfile_num),
-        parent_folder=elmfiles_network, error_if_non_existent=False)
-      if not existing_elmfile:
-        break
-      elmfile_num += 1 
-    elmfile = self.create_in_folder(elmfiles_network,
-      "elmfile_"+str(elmfile_num)+".ElmFile", overwrite=True)
-    self.clear_elmres_from_objects_with_status_deleted()
-    elmfile.f_name = file_path + ".csv"
-    # Add ElmREs for ElmFiles
-    active_case = self.app.GetActiveStudyCase()
-    elmres_for_elmfiles = self.create_in_folder(active_case,
-      "elmres_for_elmfiles.ElmRes", overwrite=False, use_existing=True)
-    # Plot
-    kwargs.update({"results_obj":elmres_for_elmfiles})  
-    self.plot(elmfile, variable,**kwargs)
-    # Simulate
-    pfds = powfacpy.PFDynSimInterface(self.app)
-    cominc = self.app.GetFromStudyCase("ComInc")
-    initial_elmres = self.get_attr(cominc,"p_resvar")
-    self.set_attr(cominc,{"p_resvar":elmres_for_elmfiles})
-    pfds.initialize_and_run_sim()
-    self.set_attr(cominc,{"p_resvar":initial_elmres})
-    # Reactivate the initial networks
-    elmfiles_network.Deactivate()
-    for network in active_networks:
-      network.Activate()
+  def set_y_axis_range_of_active_plot(self, range: tuple[float]) -> None:
+    self.set_y_axis_attributes(rangeMin=range[0], rangeMax=range[1])  
 
 
-  def create_dummy_network(self, name=None):
-    """Creates a network with only one terminal.
-    Such a network is used for example to read in ElmFile objects.
+  def autoscale(self) -> None:
+    """Autoscale all axis. 
+    
+    ToDo: Check if this really works as excpeted.
     """
-    if not name:
-      name = "dummy_network"
-    network_folder = self.app.GetProjectFolder("netdat",1)
-    dummy_network = self.create_in_folder(network_folder,
-      name+".ElmNet", overwrite=False, use_existing=True)
-    self.create_in_folder(dummy_network,
-      "dummy_terminal.ElmTerm", overwrite=False, use_existing=True)
-    return dummy_network
-
-  def autoscale(self):
     self.active_graphics_page.DoAutoScaleY()
     self.active_graphics_page.DoAutoScaleX()
     self.active_graphics_page.DoAutoScaleY()
     self.active_graphics_page.DoAutoScaleX()
 
-  def clear_curves(self):
+
+  def clear_curves(self) -> None:
     """Clear all curves from active plot.
     """
     data_series = self.get_data_series_of_active_plot()
     data_series.ClearCurves()
 
-  def clear_curves_from_all_plots(self): 
+
+  def clear_curves_from_all_plots(self) -> None: 
     """Clear curves from all plots of the active study case.
     """     
     grb = self.get_or_create_graphics_board()
     graphics = grb.GetContents()
     for graphic in graphics:
       if graphic.GetClassName() == "GrpPage":    
         for child in graphic.GetContents(): 
           if child.GetClassName() == "PltLinebarplot":
             data_series =child.GetDataSeries()
             data_series.ClearCurves()  
 
-  def clear_plot_pages(self):
+
+  def clear_plot_pages(self) -> None:
     """Deletes all graphics (plot) pages from the graphics board of 
     the active study case. 
     """
     self.clear_graphics_board(obj="*.GrpPage")
 
-  def clear_grid_diagrams(self):
+
+  def clear_grid_diagrams(self) -> None:
     self.clear_graphics_board(obj="*.SetDeskpage") 
 
-  def clear_all_graphics_pages(self):
+
+  def clear_all_graphics_pages(self) -> None:
     self.clear_graphics_board(obj="*.GrpPage")
     self.clear_graphics_board(obj="*.SetDeskpage") 
 
-  def clear_graphics_board(self, obj="*"):
+
+  def clear_graphics_board(self, obj: str = "*") -> None:
     """Clear the graphics board from specific objects or from all objects.
     Objects of class SetDeskpage are closed, 
     objects of class GrpPage are removed, 
-    others are deleted.
+    other objects are deleted.
+
+    Args:
+        obj (str, optional): Object name (can include class and placeholders). Defaults to "*".
     """
     grb = self.get_or_create_graphics_board()
     graphics = grb.GetContents(obj)
     for graphic in graphics:
       if graphic.GetClassName() == "SetDeskpage":
         graphic.Close()
       elif graphic.GetClassName() == "GrpPage":
         graphic.RemovePage()
       else:
         graphic.Delete()
+
   
-  def copy_graphics_board_content(self, source_study_case,
-    target_study_cases, obj_to_copy="*",
-    clear_target_graphics_board=False):
+  def copy_graphics_board_content(
+    self, 
+    source_study_case: str | IntCase,
+    target_study_cases: str | IntCase | list[str] | list[IntCase], 
+    obj_to_copy: str = "*",
+    clear_target_graphics_board: bool = False) -> None:
     """Copy the graphics board content of a study case to another study cases.
-    Arguments:
-      source_study_case: Source case (path or object)
-      target_study_cases: Target case(s) (path(s) or object(s))
-      obj_to_copy: name of objects to be copied from graphics board 
-        (e.g. "*.GrpPage" to copy only the plot pages)
-      clear_target_graphics_board: If true, the graphics boards of the target 
-        cases are cleared before pasting the content  
-    """    
-    
-    currently_active_study_case = self.app.GetActiveStudyCase() # Method should not change active case
-    graphics_board_name = powfacpy.PFTranslator.get_graphics_board_name_from_studycase(
-      currently_active_study_case) # assumption: graphics board names identical in all study cases 
-    source_study_case = self.handle_single_pf_object_or_path_input(source_study_case)
+
+    Args:
+        source_study_case (str | IntCase): Source case (path or object)
+        
+        target_study_cases (str | IntCase | list[str] | list[IntCase]): Target case(s) (path(s) or object(s))
+        
+        obj_to_copy (str, optional): name of objects to be copied from graphics board.(e.g. "*.GrpPage" to copy only the plot pages). Defaults to "*".
+        
+        clear_target_graphics_board (bool, optional): If true, the graphics boards of the target cases are cleared before pasting the content. Defaults to False.
+    """   
+    currently_active_study_case = self.app.GetActiveStudyCase() # Method should not change active case 
+    source_study_case = self._handle_single_pf_object_or_path_input(source_study_case, include_subfolders=False)
     source_graphics_board = self.get_single_obj(".SetDesktop",
-      parent_folder=source_study_case)
+      parent_folder=source_study_case, include_subfolders=False)
     if not isinstance(target_study_cases,(list, tuple)):
       target_study_cases = [target_study_cases]  
     for target_study_case in target_study_cases:
-      target_study_case = self.handle_single_pf_object_or_path_input(target_study_case)
+      target_study_case = self._handle_single_pf_object_or_path_input(target_study_case, include_subfolders=False)
       if not target_study_case == source_study_case:
         target_study_case.Deactivate() # Writing to active graphics board not possible 
-        target_graphics_board = self.get_single_obj(".SetDesktop", parent_folder=target_study_case)
+        target_graphics_board = self.get_single_obj(".SetDesktop", parent_folder=target_study_case, include_subfolders=False)
         if clear_target_graphics_board:
           self.delete_obj("*", parent_folder=target_graphics_board, error_if_non_existent=False)
-        self.copy_obj(obj_to_copy, target_folder=target_graphics_board, overwrite=True,
-          parent_folder=source_graphics_board)
+        self.copy_obj(obj_to_copy, 
+                      target_folder=target_graphics_board, 
+                      overwrite=True,
+                      parent_folder=source_graphics_board)
     if currently_active_study_case:         
       currently_active_study_case.Activate() # Activate if it was deactivated
 
-  def copy_graphics_board_content_to_all_study_cases(self, source_study_case,
-    target_parent_folder=None,
-    include_subfolders=True,
-    obj_to_copy="*",
-    clear_target_graphics_board=False):
+
+  def copy_graphics_board_content_to_all_study_cases(
+    self, 
+    source_study_case: str | IntCase,
+    target_parent_folder: str | PFGeneral = None,
+    include_subfolders: bool = True,
+    obj_to_copy: str = "*",
+    clear_target_graphics_board: bool = False) -> None:
     """Copy the content of the graphics board to all study cases.
-    Arguments:
-      source_study_case: Source case (path or object)
-      target_parent_folder: Parent folder of target cases. By default,
-        the study case folder of the project is used. Any folder inside
-        the study case folder of the project can be specified.
-      obj_to_copy: name of objects to be copied from graphics board 
-        (e.g. "*.GrpPage" to copy only the plot pages)
-      clear_target_graphics_board: If true, the graphics boards of the target 
-        cases are cleared before pasting the content
+
+    Args:
+        source_study_case (str | IntCase): Source case (path or object)
+        
+        target_parent_folder (str | PFGeneral, optional): Parent folder of target cases. By default, the study case folder of the project is used. Any folder inside the study case folder of the project can be specified.
+        
+        include_subfolders (bool, optional): Applies to search for target study cases. Defaults to True.
+        
+        obj_to_copy (str, optional): name of objects to be copied from graphics board (e.g. "*.GrpPage" to copy only the plot pages). . Defaults to "*".
+        
+        clear_target_graphics_board (bool, optional): If true, the graphics boards of the target cases are cleared before pasting the content. Defaults to False.
     """
     if not target_parent_folder:
-      #study_case_project_folder_name = powfacpy.PFTranslator.get_default_study_case_folder_name(
-      #  self.language)
-      #target_parent_folder = self.get_single_obj(study_case_project_folder_name)
       target_parent_folder = self.app.GetProjectFolder("study")  
     target_study_cases = self.get_obj("*.IntCase",
       parent_folder=target_parent_folder,
       include_subfolders=include_subfolders)
     self.copy_graphics_board_content(source_study_case, target_study_cases,
       obj_to_copy=obj_to_copy,
       clear_target_graphics_board=clear_target_graphics_board)
 
+
   @staticmethod
-  def plot_from_csv(csv_path, variables, offset=0, plot_interface=None):
+  def plot_from_csv(csv_path: str, 
+                    variables: str | list[str], 
+                    offset: float = 0, 
+                    plot_interface: object = None) -> VisPlot | PltLinebarplot | PltVectorplot:
     """Plot results from csv file using pyplot.
-    Arguments:
-      csv_path: path of csv file
-      variables: path of variables to be plotted
-      offset: time offset
-
-    Returns the plot.
 
+    Args:
+        csv_path (str): path of csv file
+        variables (str | list[str]): variables to be plotted
+        offset (float, optional): time offset. Defaults to 0.
+        plot_interface (object, optional): _description_. Defaults to None.
+
+    Returns:
+        VisPlot | PltLinebarplot | PltVectorplot: Returns the plot.
+        
     Example:
       plot_from_csv("results.csv",
         ["Network Model\\Network Data\\Grid\\AC Voltage Source\\s:u0",
-        "Network Model\\Network Data\\Grid\\AC Voltage Source\\m:Psum:bus1"])  
+        "Network Model\\Network Data\\Grid\\AC Voltage Source\\m:Psum:bus1"])    
     """
     if not plot_interface:
       plot_interface = pyplot
     if isinstance(variables, str):
       variables = [variables]
     with open(csv_path) as file:
       csv_file = pandas.read_csv(file)
       for var in variables:
         plot = plot_interface.plot(csv_file["time"]+offset, csv_file[var], label = var)   
     return plot
 
-  def get_data_series_of_plot(self, plot=None):
-    """Returns the data series object of a plot,
-    If plot is None, the active plot is used.
+
+  def plot_from_comtrade(self,
+                      file_path: str,
+                      variables: str | list[str],
+                      graphics_page: str | GrpPage | SetVipage = None,
+                      plot: VisPlot | PltLinebarplot | PltVectorplot = None,
+                      parent_folder_comtrade: str | PFGeneral = None,
+                      **kwargs) -> None:
+    """Plot a varibale from a COMTRADE formated file.
+    
+    Creates the comtrade object (IntComtrade) and plots. For further info on the arguments see method 'plot_monitored_variables'.  
+    If you want to plot from a comtrade object (IntComtrade) that already 
+    exists in the PF database, use the method 'plot_monitored_variables' as shown in the code below.
+
+    Args:
+        file_path (str): of comtrade file
+        
+        variables (str | list[str]): The entry in the second column of a signal in .cfg
+        
+        graphics_page (str | GrpPage | SetVipage, optional): _description_. Defaults to None.
+        
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): _description_. Defaults to None.
+        
+        parent_folder_comtrade (str | PFGeneral, optional): FolderContainer in PF database for comtrade objects (str or PF object). Defaults to None ("Comtrade.IntFolder" in active study case is used).
+    """                  
+    intcomtrade = self.create_comtrade_obj(file_path,
+      parent_folder=parent_folder_comtrade)
+    self.plot_monitored_variables(intcomtrade,
+              variables,
+              graphics_page=graphics_page,
+              plot=plot,
+              results_obj=intcomtrade,
+              **kwargs)
+
+
+  def plot_from_csv_using_elm_file(
+    self, 
+    file_path: str, 
+    variable: str,
+    **kwargs) -> None:
+    """Use an ElmFile object to plot data from csv file.
+    
+    It is generally preferrable and more stable to use the COMTRADE format to plot external data.
+    
+    The ElmFile objects are stored in a dummy network because the simulation needs to be run to read the data from the csv file and is not just printed to the plot automatically.
+
+    Args:
+        file_path (str): path to csv file
+        variable (str): varaible name in csv file header
+    """
+    # Deactivate currently active networks
+    active_networks = self.get_active_networks(
+      error_if_no_network_is_active=False)
+    for network in active_networks:
+      network.Deactivate()
+    # Activate dummy network
+    elmfiles_network = self.create_dummy_network("network_for_elmfiles")  
+    elmfiles_network.Activate()  
+    # Add new ElmFile
+    elmfile_num = 1
+    while True:
+      existing_elmfile = self.get_single_obj("elmfile_"+str(elmfile_num),
+        parent_folder=elmfiles_network, error_if_non_existent=False)
+      if not existing_elmfile:
+        break
+      elmfile_num += 1 
+    elmfile = self.create_in_folder(
+      "elmfile_" + str(elmfile_num) + ".ElmFile",       
+      elmfiles_network,
+      overwrite=True)
+    self.clear_elmres_from_objects_with_status_deleted()
+    elmfile.f_name = file_path + ".csv"
+    # Add ElmREs for ElmFiles
+    active_case = self.app.GetActiveStudyCase()
+    elmres_for_elmfiles = self.create_in_folder(
+      "elmres_for_elmfiles.ElmRes",
+      active_case,
+      overwrite=False, 
+      use_existing=True)
+    # Plot
+    kwargs["results_obj"] = elmres_for_elmfiles  
+    self.plot(elmfile, variable, **kwargs)
+    # Simulate
+    pfds = powfacpy.PFDynSimInterface(self.app)
+    cominc = self.get_from_study_case("ComInc")
+    initial_elmres = self.get_attr(cominc,"p_resvar")
+    self.set_attr(cominc,{"p_resvar":elmres_for_elmfiles})
+    pfds.initialize_and_run_sim()
+    self.set_attr(cominc,{"p_resvar":initial_elmres})
+    # Reactivate the initial networks
+    elmfiles_network.Deactivate()
+    for network in active_networks:
+      network.Activate()
+
+
+  def create_dummy_network(self, 
+                           name: str = "dummy_network") -> ElmNet:
+    """Creates a network with only one terminal.
+    Such a network is used for example to read in ElmFile objects.
+    """
+    network_folder = self.app.GetProjectFolder("netdat",1)
+    dummy_network = self.create_in_folder(
+      name+".ElmNet", 
+      network_folder,
+      overwrite=False, 
+      use_existing=True)
+    self.create_in_folder("dummy_terminal.ElmTerm", dummy_network, overwrite=False, use_existing=True)
+    return dummy_network
+  
+
+  def get_data_series_of_plot(
+    self, 
+    plot: VisPlot | PltLinebarplot | PltVectorplot = None) -> PltDataseries:
+    """Returns the data series object of a plot. If plot is None, the active plot is used.
     """
     if not plot:
       return self.get_data_series_of_active_plot()
     else:
-      plot = self.handle_single_pf_object_or_path_input(plot)
+      plot = self._handle_single_pf_object_or_path_input(plot)
       return plot.GetDataSeries()
 
+
   def get_curve_table_attributes(
       self, 
-      plot=None, 
-      adjust_result_file=True) -> dict:
-    """Returns a dictionary with all curve table attributes (keys) and
+      plot: VisPlot | PltLinebarplot | PltVectorplot = None, 
+      adjust_result_file = True) -> dict[str, list]:
+    """Get dictionary with all curve table attributes (keys) and
     list with the attributes values for each curve (values) of a plot (i.e. its data series).
 
-    Arguments:
-      - plot: path or PF object. If None, the active plot is used
-      - adjust_result_file: please see get_curve_table_attributes_referring_to_data_source
-        for a detailed description 
+    Args:
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): path or PF object. If None, the active plot is used. 
+        
+        adjust_result_file (bool, optional): please see get_curve_table_attributes_referring_to_data_source
+        for a detailed description . Defaults to True.
+
+    Returns:
+        dict[str, list]: curve table attributes
     """
     attributes_referring_to_data_source = self.get_curve_table_attributes_referring_to_data_source(
       plot=plot, 
       adjust_result_file=adjust_result_file)
     attributes_referring_to_visualisation_visualization = self.get_curve_table_attributes_referring_to_visualization(
       plot=plot)
     return {**attributes_referring_to_data_source,
             **attributes_referring_to_visualisation_visualization}
 
+
   def get_curve_table_attributes_referring_to_data_source(
       self, 
-      plot=None, 
-      adjust_result_file=True) -> dict:
+      plot: VisPlot | PltLinebarplot | PltVectorplot = None, 
+      adjust_result_file: bool = True) -> dict:
     """Get the curve table attributes referring to the data source 
     of the curves from a plot (i.e. its data series).
+    
     These attributes are: "curveTableResultFile", "curveTableElement",
       "curveTableVariable"
-    The return value is a dictionary with 
-      - keys: attribute names
-      - values: lists with the values for each curve
-
+      
     Use this method if the data sources of the curves are of interest.
     If further attributes on visualisation are of interest, see also the
     methods:
       - get_curve_table_attributes
       - get_curve_table_attributes_referring_to_visualization
 
-    Arguments:
-      - plot: path or PF object. If None, the active plot is used.
-      - adjust_result_file: 
-        - If False, the list in "curveTableResultFile" is used as is
-        - If True, the list is adjusted depending on the plot settings
-          "useIndividualResults". If "useIndividualResults" is True,
-          the result files from the list "curveTableResultFile" are used
-          by default. If an element of this list is empty, the 
-          "userSelectedResultFile" is used. Note that there is a bug in
-          PF so that "autoSelectedResultFile" is always empty as described 
-          below.
+    Args:
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): path or PF object. If None, the active plot is used. Defaults to None.
+        
+        adjust_result_file (bool, optional): Defaults to True.
+          - If False, the list in "curveTableResultFile" is used as is
+          - If True, the list is adjusted depending on the plot settings
+            "useIndividualResults". If "useIndividualResults" is True,
+            the result files from the list "curveTableResultFile" are used
+            by default. If an element of this list is empty, the 
+            "userSelectedResultFile" is used. Note that there is a bug in
+            PF so that "autoSelectedResultFile" is always empty as described 
+            below.
+
+    Returns:
+        dict: 
+          - keys: attribute names
+          - values: lists with the values for each curve
     """
     data_series = self.get_data_series_of_plot(plot)
     attributes = dict.fromkeys(["curveTableResultFile", 
                                 "curveTableElement",
                                 "curveTableVariable"]) 
     attributes["curveTableElement"] = data_series.GetAttribute("curveTableElement")
     attributes["curveTableVariable"] = data_series.GetAttribute("curveTableVariable")
@@ -561,33 +679,36 @@
           if result_file:
             attributes["curveTableResultFile"][idx] = result_file   
     else:
       attributes["curveTableResultFile"] = data_series.GetAttribute(
         "curveTableResultFile")  
     return attributes
   
+  
   def get_curve_table_attributes_referring_to_visualization(
       self, 
-      plot=None) -> dict:
-    """Returns the curve table attributes of a plot  (i.e. its data series) 
+      plot: VisPlot | PltLinebarplot | PltVectorplot = None) -> dict[str, object]:
+    """Get the curve table attributes of a plot  (i.e. its data series) 
     that refer to the visualisation. 
-
+    
     The return value is a dictionary with 
       - keys: attribute names
       - values: lists with the values for each curve
 
     Use this method if the data sources of the curves are of interest.
     If further attributes on the data sources are of interest, see also the
     methods:
       - get_curve_table_attributes
-      - get_curve_table_attributes_referring_to_data_source    
+      - get_curve_table_attributes_referring_to_data_source
 
-    Arguments:
-      - plot: path or PF object. If None, the active plot is used.
+    Args:
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): path or PF object. If None, the active plot is used. Defaults to None.
 
+    Returns:
+        dict[str, object]: dict with attributes and their values.
     """
     data_series = self.get_data_series_of_plot(plot)
     attributes = dict.fromkeys(["curveTableVisible", 
                                 "curveTableNormalise",
                                 "curveTableNormValue",
                                 "curveTableColor", 
                                 "curveTableLineStyle",
@@ -595,134 +716,88 @@
                                 "curveTableShape",
                                 "curveTableFillStyle", 
                                 "curveTableLabel"])
     for attr in attributes.keys():
       attributes[attr] = data_series.GetAttribute(attr)
     return attributes
 
+
   def set_curve_table_attributes(
       self, 
-      attributes:dict, 
-      plot=None) -> None:
+      attributes: dict[str, list], 
+      plot: VisPlot | PltLinebarplot | PltVectorplot = None) -> None:
     """Set the curve table attributes of a plot  (i.e. its data series).
 
-    Arguments:
-      - attributes: a dictionary with 
-        - keys: argument names, e.g. "curveTableLabel"
-        - values: list with the values for each curve
-        - plot: path or PF object. If None, the active plot is used. 
-    """     
+    Args:
+        attributes (dict[str, list]): a dictionary with 
+          - keys: argument names, e.g. "curveTableLabel"
+          - values: list with the values for each curve
+          
+        plot (VisPlot | PltLinebarplot | PltVectorplot, optional): Plot object. Defaults to None (active plot is used).
+    """    
     data_series = self.get_data_series_of_plot(plot)
     for attr,value in attributes.items():
       data_series.SetAttribute(attr,value)
 
+
   @staticmethod
   def clear_curves_from_curve_table_attributes_dict(
     attributes: dict, 
-    index: "int|slice") -> dict:
+    index: int | slice) -> None:
     """Clear curves from a dictionary with the curve table attributes (keys)
     and the entries for each curve (values).
+    
     IMPORTANT: Zero based indexing is used i.e. the first curve has index 0.
     Note that this does not clear the curves from the data series in the 
     PF plot, but only from the dictionary. If you want to clear the curves
     from a plot, use clear_curves_by_index_from_active_plot
 
     Arguments: 
-      - attributes: dictionary with attribute names (keys) and entries for each 
+      - attributes (dict): dictionary with attribute names (keys) and entries for each 
         curve (values)
-      - index: can be an integer or slice
+      - index (int | slice): can be an integer or slice
         - integer: index of one curve to be deleted
         - slice: several curves are deleted. Examples:
           - slices have the general form "slice(start, end, step)" (see for example https://www.programiz.com/python-programming/methods/built-in/slice) 
           - "slice(2,4)": clear curves with index 2,3 (step=1 is default)
           - "slice(-1,1,-1): start at the end and delete all curves larger than index 1  
     """
     for values in attributes.values():
       del values[index]
 
-  def clear_curves_by_index_from_active_plot(self, index: "int|slice") -> None:
+
+  def clear_curves_by_index_from_active_plot(self, index: int | slice) -> None:
     """Clear curves with certain index from plot (i.e. its data series).
     IMPORTANT: Zero based indexing is used i.e. the first curve has index 0.
     The native PF API has no such functionality and can only delete all curves.
     The method works as follows: 
      - gets the curve table attributes in a dictionary
      - clears all curves from plot
      - clear certain curves from the dictionary
      - set the curve table attributes according to the dictionary
 
      Arguments:
-      - index: for a detailled description please have 
+      - index (int | slice): for a detailled description please have 
         a look at clear_curves_from_curve_table_attributes_dict
     """
     curve_table_attr = self.get_curve_table_attributes()
     self.clear_curves()
     powfacpy.PFPlotInterface.clear_curves_from_curve_table_attributes_dict(
       curve_table_attr,index)
     self.set_curve_table_attributes(curve_table_attr)
 
-  def get_lists_from_data_series_of_plot(self, plot=None, indexes=None, include_curve_options=False):
-    """Depracated: Please use get_curve_table_attributes instead. The usage of
-    a the class PFListsOfDataSeriesOfPlot has turned out to be less convenient than
-    just using a dictionary for the curve table attributes.
-
-    Returns PFListsOfDataSeriesOfPlot object with lists of the data from 
-    DataSeries (PltDataseries) of a plot.
-    """
-    data_series = self.get_data_series_of_plot(plot)   
-    lists = PFListsOfDataSeriesOfPlot(
-      data_series.GetAttribute("curveTableElement"),  
-      data_series.GetAttribute("curveTableVariable"), 
-      [], [], [], [], []
-    )
-    if data_series.useIndividualResults:
-      lists.result_objects = data_series.GetAttribute("curveTableResultFile") 
-      for idx, res_obj in enumerate(lists.result_objects):
-        if not res_obj:
-          lists.result_objects[idx] = data_series.GetAttribute("userSelectedResultFile")
-    else:
-      # PF bug:
-      # Even if 'autoSearchResultsFile' is True, 'userSelectedResultFile' and 
-      # not 'autoSelectedResultFile' must be used.
-      # Furthermore, 'autoSearchResultFile' must be deactivated and activated once.
-      auto_search_result_file_original_value = data_series.autoSearchResultFile 
-      data_series.autoSearchResultFile = 0
-      data_series.autoSearchResultFile = 1
-      data_series.autoSearchResultFile = auto_search_result_file_original_value
-      lists.result_objects = [data_series.GetAttribute("userSelectedResultFile")]*len(lists.elements)
-    if include_curve_options:
-      lists.line_styles = data_series.GetAttribute("curveTableResultFile") 
-      lists.line_widths = data_series.GetAttribute("curveTableLineWidth") 
-      lists.colors = data_series.GetAttribute("curveTableColor") 
-      lists.labels = data_series.GetAttribute("curveTableLabel")
-    # Return only curves contained in indexes  
-    if indexes:
-      lists.elements = [lists.elements[i] for i in indexes]
-      lists.variables = [lists.variables[i] for i in indexes]
-      lists.result_objects = [lists.result_objects[i] for i in indexes] 
-      if include_curve_options:
-        lists.line_style = [lists.line_style[i] for i in indexes] 
-        lists.line_widths = [lists.line_widths[i] for i in indexes] 
-        lists.colors = [lists.colors[i] for i in indexes]  
-        lists.labels = [lists.labels[i] for i in indexes]  
-    return lists
 
-  def export_active_page(self, format='pdf', path=getcwd()):
-    """Export active page using ComWr.
+  def export_active_page(self, 
+                         format: str = 'pdf', 
+                         path: str = getcwd()) -> None:
+    """Export active page (e.g. to pdf) using the 'ComWr' object.
+
+    Args:
+        format (str, optional): Export format. Defaults to 'pdf'.
+        path (str, optional): Export path. Defaults to current working directory (getcwd()).
     """
     self.active_graphics_page.Show()
-    comwr = self.app.GetFromStudyCase('ComWr')
-    self.set_attr(comwr,{'iopt_rd': format,'iopt_savas': 0, 'f': path + "." + format})
+    comwr = self.get_from_study_case('ComWr')
+    self.set_attr(comwr,{'iopt_rd': format,
+                         'iopt_savas': 0, 
+                         'f': path + "." + format})
     comwr.Execute()  
-
-
-class PFListsOfDataSeriesOfPlot:
-  """Deprecated: This class turned out to be less convenient than
-  just using a dictionary for the curve table attributes"""
-
-  def __init__(self, elements, variables, result_objects, line_styles, line_widths, colors, labels) -> None:
-    self.elements = elements
-    self.variables = variables 
-    self.result_objects = result_objects
-    self.line_styles = line_styles
-    self.line_widths = line_widths
-    self.colors = colors
-    self.labels = labels
```

### Comparing `powfacpy-0.1.4/src/powfacpy/results_interface.py` & `powfacpy-0.1.5/src/powfacpy/results_interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,46 @@
 import sys
-sys.path.insert(0, r'.\src')
-import powfacpy
-import numpy as np
 from os import remove, getcwd, replace
-import pandas as pd
 from math import inf
 from warnings import warn
+from typing import Iterable
 
+import pandas as pd
+from icecream import ic
 
-class PFResultsInterface(powfacpy.PFBaseInterface):
+sys.path.insert(0, r'.\src')
+import powfacpy
+from powfacpy import PFStringManipulation
+from powfacpy.pf_class_protocols import PFGeneral, ElmRes
+
+class PFResultsInterface(powfacpy.PFActiveProject):
 
   def __init__(self, app):
     super().__init__(app)
+    self.truncate_paths_until: str = PFStringManipulation.format_full_path(str(self.network_data_folder), self.app) + "\\"
+    self.variable_aliases: dict[str, str] = {}
+    self.obj_aliases: dict[str, str] = {}
 
 
   def get_list_with_results_of_variable_from_elmres(self, obj, variable, results_obj=None, load_elmres=True):
     if not results_obj:
       results_obj = self.app.GetFromStudyCase("ElmRes")
     if load_elmres:  
       results_obj.Load()  
-    obj = self.handle_single_pf_object_or_path_input(obj)  
+    obj = self._handle_single_pf_object_or_path_input(obj)  
     column = results_obj.FindColumn(obj, variable)
     return self.get_list_with_results_of_column(column, results_obj=results_obj, load_elmres=False)  
 
 
   def get_list_with_results_of_column_from_elmres(self, column, results_obj=None, load_elmres=True):
     if not results_obj:
       results_obj = self.app.GetFromStudyCase("ElmRes")
     if load_elmres:  
       results_obj.Load()   
-    intvec = self.create_in_folder(results_obj.GetParent(),"test.IntVec", overwrite=True) 
+    intvec = self.create_in_folder("test.IntVec", results_obj.GetParent(),overwrite=True) 
     results_obj.GetColumnValues(intvec, column) 
     list = intvec.V
     intvec.Delete()
     return list
   
 
   def export_to_csv(self,
@@ -72,15 +79,15 @@
         format_csv_file: Format csv file so there is only one row for the header
           (see also _format_csv_for_elmres and format_csv_for_comtrade).
 
       Returns:
         Path of csv file.
               
       Example (export a selection of results variables): 
-        voltage_source = pfbi.get_unique_obj('Network Model\\Network Data\\test_plot_interface\\Grid 1\\AC Voltage Source')
+        voltage_source = pfbi.get_unique_obj(r'Network Model\\Network Data\\test_plot_interface\\Grid 1\\AC Voltage Source')
         control_model = pfbi.get_unique_obj('Network Model\\Network Data\\test_plot_interface\Grid 1\\WECC WT Control System Type 4A\\REEC_A Electrical Control Model')
         objects =   [voltage_source, voltage_source, control_model]
         variables = ['m:Qsum:bus1',  'm:Psum:bus1',  's:Ipcmd'    ]
         elmres_list = [pfbi.app.GetFromStudyCase('ElmRes'),]*len(variables)
         df = pfbi.export_to_csv(list_of_results_objs = elmres_list, 
                                 objects = objects, 
                                 variables = variables)    
@@ -102,15 +109,15 @@
                          "must be specified together.")      
       else:
         if not results_obj:
           if not self.app.GetActiveStudyCase():
             raise powfacpy.PFNotActiveError("study case")
           comres.pResult = self.get_from_study_case("ElmRes")
         else:
-          comres.pResult = self.handle_single_pf_object_or_path_input(results_obj)
+          comres.pResult = self._handle_single_pf_object_or_path_input(results_obj)
         comres.iopt_csel = 0 # export all variables
       
       self._set_comres_settings_for_csv_export(comres, dir, file_name, column_separator, decimal_separator, comres_parameters)
       export_successful = comres.Execute()
       if export_successful != 0:
         comres_path = self.get_path_of_object(comres)
         raise Exception("CSV export was not successful using '" +
@@ -228,17 +235,17 @@
       else:
         read_file.readline().split(",")
         full_paths = read_file.readline().split(",")
         variables = read_file.readline().split(",")
       for col, path in enumerate(full_paths):
           is_last_column = (col == len(full_paths)-1)
           if col > 0:
-              formated_path = powfacpy.PFStringManipulation._format_full_path(path, self)
-              variable_name = powfacpy.PFStringManipulation._format_variable_name(variables[col])
-              row = row + formated_path + "\\" + variable_name + ","*(not is_last_column) # consistently add headers to row
+            path = self._format_path_of_obj(path)
+            variable_name = PFStringManipulation.format_variable_name(variables[col])
+            row = row + path + "\\" + variable_name + ","*(not is_last_column) # consistently add headers to row
           else:
               row = "time," # Header of first column
       write_file.write(row+"\n")
       # Write remaining data rows until end of file is reached
       while row:
           row = read_file.readline()
           write_file.write(row)
@@ -276,23 +283,21 @@
     else:
       comres.resultobj = list_of_results_objs
       comres.element = elements
       comres.variable = variables
 
 
   def export_to_pandas(self, 
-                      results_obj=None, 
-                      list_of_results_objs:list = None,
-                      elements:list = None, 
-                      variables:list = None,
-                      comres_parameters:dict = {},) -> None:
-    """
-    Returns pandas DataFrame of the simulation results in ElmRes. By default, all
-    results variables of the first ElmRes object found in the active study case
-    are exported. A selection of specific variables can be exported using 
+                      results_obj: ElmRes = None, 
+                      list_of_results_objs: list = None,
+                      elements: list = None, 
+                      variables: list = None,
+                      comres_parameters: dict = {},) -> pd.DataFrame:
+    """
+    Returns pandas DataFrame of the simulation results in ElmRes. By default, all  results variables of the first ElmRes object found in the active study case are exported. A selection of specific variables can be exported using 
     the optional arguments. Uses intermediate step by exporting to csv format
     with comres object.
     
     Arguments:
       results_obj: PF ElmRes or IntComtrade object, by default the first ElmRes 
           found in the active study case is used. All variables from this object 
           are exported.
@@ -332,33 +337,126 @@
         elements=elements,
         variables=variables,
         comres_parameters=comres_parameters,
         format_csv_file=False)
       
       df = pd.read_csv(full_path, encoding='ISO-8859-1', header=[0,1])
       self._format_pandas_column_headers(df, list_of_results_objs)  
+      
       if list_of_results_objs:
         if len(list_of_results_objs) != len(df.columns) - 1:
           warn("Not all specified results were exported. Some of the elements may be 'out of service' and were not included.")
     finally:
       remove(full_path)
+    df.set_index("time", inplace=True)  
     return df
   
 
-  def _format_pandas_column_headers(self, df:pd.DataFrame, list_of_results_objs:list) -> None:
+  def _format_pandas_column_headers(
+    self, 
+    df: pd.DataFrame, 
+    list_of_results_objs: list[ElmRes]) -> None:
+    """Format column headers of pandas DataFrame.
+    
+    Use single line column headers with path of object and results varible. 
+
+    Args:
+        df (pd.DataFrame): unformatted DataFrame.
+        list_of_results_objs (list[ElmRes]): Used to get numer of header rows of exported csv file.
+    """
     num_header_rows = self._get_number_of_header_rows_of_exported_csv_file(
         list_of_results_objs)
     headers = ["time"]
     for col in df.columns[1:]:
-      path = powfacpy.PFStringManipulation._format_full_path(col[num_header_rows-2], self)
-      var = powfacpy.PFStringManipulation._format_variable_name(col[num_header_rows-1])
+      path = self._format_path_of_obj(col[num_header_rows-2])
+      var = PFStringManipulation.format_variable_name(col[num_header_rows-1])
       headers.append(path + '\\' + var)
     df.columns = headers
+    
+  
+  def _format_path_of_obj(self, 
+                         path: str) -> str:
+    """Format the path of an obj.
+
+    Args:
+        path (str): unformated full path (usually created using 'str(obj)')
+
+    Returns:
+        str: path inside active project without class name and truncated until 'self.truncate_paths_until'
+    """
+    path = PFStringManipulation.format_full_path(path, self.app)
+    if self.truncate_paths_until:
+      path = PFStringManipulation.truncate_until(
+        path,
+        self.truncate_paths_until)  
+    return path
+  
+  
+  def replace_variable_aliases(self, var_name: str) -> str:
+    """Replace 'var_name' with correponding entry in 'self.variable_aliases'. If no such key exists in 'self.variable_aliases', 'var_name' is returned.
+
+    Args:
+        var_name (str): Original name (key in 'self.variable_aliases')
+
+    Returns:
+        str: Replacement (value in 'self.variable_aliases')
+    """
+    replacement = self.variable_aliases.get(var_name)
+    if replacement:
+      return replacement
+    else:
+      return var_name
+      
+      
+  def replace_object_aliases(self, obj_name: str) -> str:
+    """Replace 'obj_name' with correponding entry in 'self.obj_aliases'. If no such key exists in 'self.obj_aliases', 'obj_name' is returned.
+
+    Args:
+        obj_name (str): Original name (key in 'self.obj_aliases')
+
+    Returns:
+        str: Replacement (value in 'self.obj_aliases')
+    """ 
+    replacement = self.obj_aliases.get(obj_name)
+    if replacement:
+      return replacement
+    else:
+      return obj_name
+  
+  
+  def get_simulation_results_from_dataframe(
+    self, 
+    df: pd.DataFrame, 
+    objs: PFGeneral | str | Iterable[PFGeneral | str], 
+    variables: str | Iterable[str]) -> pd.DataFrame:
+    """Get simulation results from a DataFrame (which was created using 'export_to_pandas')
 
+    Args:
+    
+        df (pd.DataFrame): DataFrame with simulation results (created using 'export_to_pandas')
+        
+        objs (PFGeneral | str | Iterable[PFGeneral  |  str]): objects (for which results must be contained in the 'df')
+        
+        variables (str | Iterable[str]): variables (for which results must be contained in the 'df')
 
+    Returns:
+        DataFrame: DataFrame with specified results
+    """
+    objs = self._handle_pf_object_or_path_input(objs)
+    if isinstance(variables, str):
+      variables = [variables]
+    obj_and_var_strings = []
+    for obj in objs:
+      obj_and_var_string = self._format_path_of_obj(PFStringManipulation.remove_html_tags_from_path(str(obj)))
+      for var in variables:
+        obj_and_var_string += "\\" + var
+        obj_and_var_strings.append(obj_and_var_string) 
+    return df[obj_and_var_strings]  
+    
+      
   def _get_time_variable_name_from_elmres(self,elmres) -> str:
     """Returns the variable name of simulation time in an ElmRes object. 
     Different PF simulation types (RMS, quasi-static,..) 
     have different names for the time variable.
     """
     if elmres.calTp == 0: # RMS/EMT
       return 'b:tnow'
@@ -367,8 +465,9 @@
     else:
       elmres_path = self.get_path_of_object(elmres)
       raise Exception(f"""The PF simulation type number '{elmres.calTp}' of the results object 
       '{elmres_path}' 
       (attribute 'calTp' of ElmRes object) is not known or has not been implemented yet. Consider changes in the source code to 
       _get_time_variable_name_from_elmres (or open an issue: https://github.com/FraunhIEE-UniKassel-PowSysStability/powfacpy/).""")
       
-
+      
+
```

### Comparing `powfacpy-0.1.4/src/powfacpy/script_interface.py` & `powfacpy-0.1.5/src/powfacpy/script_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,45 +11,45 @@
 import powfacpy
 import warnings
 from os import path as os_path
 import os
 import shutil
 
 
-class PFComPythonObjectInterface(powfacpy.PFBaseInterface):
+class PFComPythonObjectInterface(powfacpy.PFActiveProject):
   """Interface to python script objects.
   """
 
   def __init__(self, app): 
     super().__init__(app) 
 
   def create_file_from_embedded_script(self, out_file, compython):
     """Create a .py file from an embedded script.
     """
-    compython = self.handle_single_pf_object_or_path_input(compython)
+    compython = self._handle_single_pf_object_or_path_input(compython)
     # The xScript attribute is a list with all lines of the script
     TextFileProcessor.create_file_from_list_of_lines(out_file, compython.xScript)
 
   def set_embedded_script_from_file(self, compython, file):
     """Set the embedded script based on a .py file.
     """
-    compython = self.handle_single_pf_object_or_path_input(compython)
+    compython = self._handle_single_pf_object_or_path_input(compython)
     compython.xScript = TextFileProcessor.get_list_of_lines_of_file(file)
 
   def merge_file_into_embedded_script(self,
     compython,
     inserted_file:str,
     start_after_line,
     end_before_line):
     """Merge a file into an embedded script between the starting 
     and ending lines.
     The start and end lines can either be integers (line numbers) or
     string matches.
     """
-    compython = self.handle_single_pf_object_or_path_input(compython)
+    compython = self._handle_single_pf_object_or_path_input(compython)
     temporary_dir = "powfacpy_temp"
     os.makedirs(temporary_dir, exist_ok=True)
     try:
       embedded_script_original_file = temporary_dir + r"\embedded_script_original.py"
       self.create_file_from_embedded_script(embedded_script_original_file, compython)
       merged_file = temporary_dir + r"\merged.py"
       TextFileProcessor.merge_into_file(embedded_script_original_file,
@@ -68,15 +68,15 @@
     and ending lines.
     The start and end lines can either be integers (line numbers) or
     string matches.
     """
     temporary_dir = "powfacpy_temp"  
     os.makedirs(temporary_dir)
     try:
-      compython = self.handle_single_pf_object_or_path_input(compython)
+      compython = self._handle_single_pf_object_or_path_input(compython)
       merged_package_file = temporary_dir + r"\merged_package.py"
       PythonFileInterface.merge_package_into_single_file(init_file, merged_package_file)
       original_embedded_script_file = temporary_dir + r"\original_embedded_script.py"
       self.create_file_from_embedded_script(original_embedded_script_file, compython)
       merged_package_into_embedded_file = temporary_dir + r"\merged_package_into_embedded.py"
       TextFileProcessor.merge_into_file(original_embedded_script_file,
         merged_package_file,
```

### Comparing `powfacpy-0.1.4/tests/test_base_interface.py` & `powfacpy-0.1.5/tests/test_active_project_interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,300 +1,314 @@
-import pytest
+"""Tests for the class PFActiveProject.
+
+The class PFActiveProject inherits from PFFolder. There are no separate tests for the PFFolder class, all tests for both classes are included here.
+"""
 import sys
 import os
 import json
-settings_file = open('.\\settings.json')
-settings = json.load(settings_file)
+import importlib
+
+import pytest
+
+with open('.\\settings.json') as settings_file:
+    settings = json.load(settings_file)
 sys.path.append(settings["local path to PowerFactory application"])
 import powerfactory
+
 sys.path.insert(0, r'.\src')
 import powfacpy 
-import importlib
 importlib.reload(powfacpy)
 
 
-
 @pytest.fixture(scope='session')
 def pf_app():
     return powerfactory.GetApplication()
 
-@pytest.fixture
-def pfbi(pf_app):
-    # Return PFBaseInterface instance
-    return powfacpy.PFBaseInterface(pf_app)   
 
-@pytest.fixture
-def activate_test_project(pfbi):
+@pytest.fixture(scope='session')
+def pfp(pf_app) -> powfacpy.PFActiveProject:
+    # Return PFActiveProject instance
+    return powfacpy.PFActiveProject(pf_app)   
+
+
+@pytest.fixture()
+def activate_test_project(pfp):
     """The project for testing must be located in the current
     user under "powfacpy\\powfacpy_tests". This method will create
     a copy of that project which is then used for the tests. This 
     ensures that the tests are always run with the same initial
     project state.
     """
-    user = pfbi.app.GetCurrentUser()
-    project_for_testing = pfbi.get_single_obj(r"powfacpy\powfacpy_tests",
-        parent_folder = user)
-    folder_of_project_for_testing = pfbi.get_single_obj(r"powfacpy",
-        parent_folder = user)    
-    project_copy = pfbi.copy_single_obj(project_for_testing,
-        folder_of_project_for_testing, new_name="powfacpy_tests_copy_where_tests_are_run")    
-    project_copy.Activate()    
+    user = pfp.app.GetCurrentUser()
+    project_for_testing = pfp.get_single_obj(r"powfacpy\powfacpy_tests",
+        parent_folder = user, include_subfolders=False)
+    folder_of_project_for_testing = pfp.get_single_obj(r"powfacpy",
+        parent_folder = user, include_subfolders=False)   
+    project_copy = pfp.copy_single_obj(project_for_testing,
+        folder_of_project_for_testing, 
+        new_name="powfacpy_tests_copy_where_tests_are_run")    
+    project_copy.Activate()   
     
 
-def test_get_from_study_case(pfbi, activate_test_project):
-    study_case = pfbi.get_unique_obj(r'Study Cases\test_base_interface\multiple_elmres.IntCase')
-    study_case.Activate()
-
-    with pytest.warns(Warning):
-        pfbi.get_from_study_case('ElmRes')
-
-    study_case.Deactivate()
-    with pytest.raises(powfacpy.PFNoActiveStudyCaseError):
-        pfbi.get_from_study_case('ElmRes')
-    pass
-
-
-def test_get_single_object(pfbi, activate_test_project):
-    terminal_1=pfbi.get_single_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 1") 
-    assert isinstance(terminal_1, powerfactory.DataObject)
-    with pytest.raises(TypeError):
-       terminals=pfbi.get_single_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal*")  
-
-def test_get_obj(pfbi, activate_test_project):
-    terminal_1 = pfbi.get_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 1")[0]
+def test_get_obj(pfp, activate_test_project):
+    terminal_1 = pfp.get_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 1")[0]
     assert isinstance(terminal_1, powerfactory.DataObject)
     with pytest.raises(powfacpy.PFPathError):
-        terminal_1 = pfbi.get_obj(r"Stretchwork Model\Stretchwork Data\Grid\Termalamala")[0]
+        terminal_1 = pfp.get_obj(r"Stretchwork Model\Stretchwork Data\Grid\Termalamala")[0]
     with pytest.raises(powfacpy.PFPathError):
-        terminal_1 = pfbi.get_obj(r"N")[0]    
+        terminal_1 = pfp.get_obj(r"N")[0]    
     with pytest.raises(TypeError):
-        terminal_1 = pfbi.get_obj(terminal_1)[0]
+        terminal_1 = pfp.get_obj(terminal_1)[0]
     with pytest.raises(TypeError):
-        terminal_1 = pfbi.get_obj(terminal_1, include_subfolders=False)[0]
+        terminal_1 = pfp.get_obj(terminal_1, include_subfolders=False)[0]
 
-def test_get_obj_with_condition(pfbi, activate_test_project):
-    hv_terminals = pfbi.get_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal*",
+
+def test_get_single_object(pfp, activate_test_project):
+    terminal_1=pfp.get_single_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 1") 
+    assert isinstance(terminal_1, powerfactory.DataObject)
+    with pytest.raises(TypeError):
+       terminals=pfp.get_single_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal*")  
+
+
+def test_get_obj_with_condition(pfp, activate_test_project):
+    hv_terminals = pfp.get_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal*",
         condition=lambda x: getattr(x,"uknom") > 50)
     assert len(hv_terminals) == 2    
 
-def test_get_obj_with_parent_folder_argument(pfbi, activate_test_project):
-    parent_folder = pfbi.get_first_level_folder("user")
-    terminal_1 = pfbi.get_obj(r"powfacpy\powfacpy_tests\Network Model\Network Data\test_base_interface\Grid\Terminal HV 1",
+
+def test_get_obj_with_parent_folder_argument(pfp, activate_test_project):
+    parent_folder = pfp.get_first_level_folder("user")
+    terminal_1 = pfp.get_obj(r"powfacpy\powfacpy_tests\Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 1",
         parent_folder=parent_folder)[0]
     assert isinstance(terminal_1, powerfactory.DataObject)
 
-    grid = pfbi.get_obj("Grid", parent_folder=r"Network Model\Network Data\test_base_interface")[0]
+    grid = pfp.get_obj("Grid", parent_folder=r"Network Model\Network Data\test_active_project_interface")[0]
     assert isinstance(grid, powerfactory.DataObject)
+    
+    parent_folder = powfacpy.PFFolder(r"Network Model\Network Data\test_active_project_interface", pfp.app)
+    grid = pfp.get_obj("Grid", parent_folder=parent_folder)[0]
+    assert isinstance(grid, powerfactory.DataObject)
+
 
-def test_get_obj_including_subfolders(pfbi, activate_test_project):
-    terminals = pfbi.get_obj(r"Network Data\test_base_interface\*.ElmTerm", parent_folder="Network Model",
+def test_get_obj_including_subfolders(pfp, activate_test_project):
+    terminals = pfp.get_obj(r"Network Data\test_active_project_interface\*.ElmTerm", parent_folder="Network Model",
         include_subfolders=True) 
     assert len(terminals) == 3    
 
-def test_path_exists(pfbi, activate_test_project):
-    assert pfbi.path_exists(r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 1")
 
-def test_set_attr(pfbi, activate_test_project):
+def test_path_exists(pfp, activate_test_project):
+    assert pfp.path_exists(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 1")
+
+
+def test_set_attr(pfp, activate_test_project):
     test_string_1 = "TestString1"
     test_string_2 = "TestString2"
-    pfbi.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTitle":test_string_1})
-    pfbi.set_attr("Linear_interpolation",{"sTitle":test_string_2,
+    pfp.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTitle":test_string_1})
+    pfp.set_attr("Linear_interpolation",{"sTitle":test_string_2,
         "desc":["dummy description"]}, parent_folder=r"Library\Dynamic Models")
-    stitle = pfbi.get_attr(r"Library\Dynamic Models\Linear_interpolation","sTitle")
+    stitle = pfp.get_attr(r"Library\Dynamic Models\Linear_interpolation","sTitle")
     assert stitle == test_string_2
 
-def test_set_attr_of_obj(pfbi, activate_test_project):
-    test_string_1 = "TestString1"
-    model = pfbi.get_single_obj(r"Library\Dynamic Models\Linear_interpolation")
-    powfacpy.set_attr_of_obj(model,{"sTitle":test_string_1})
-    stitle = pfbi.get_attr(model,"sTitle")
-    assert stitle == test_string_1
 
-def test_set_attr_exceptions(pfbi, activate_test_project):
+def test_set_attr_exceptions(pfp, activate_test_project):
     with pytest.raises(powfacpy.exceptions.PFAttributeTypeError):
-        pfbi.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTitle":"dummy",
+        pfp.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTitle":"dummy",
         "desc":2}) # "desc" should be a list with one string item
     with pytest.raises(powfacpy.exceptions.PFAttributeError):
-        pfbi.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTie":"dummy",
+        pfp.set_attr(r"Library\Dynamic Models\Linear_interpolation",{"sTie":"dummy",
         "desc":["dummy description"]}) # 'sTie' is not a valid attribute 
     with pytest.raises(powfacpy.exceptions.PFPathError):
-        terminal_1 = pfbi.get_obj(r"Network Model\Network Data\test_base_interface\Grid\Termalamala")
+        terminal_1 = pfp.get_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Termalamala")
 
-def test_set_attr_by_path(pfbi, activate_test_project):
-    pfbi.set_attr_by_path(r"Library\Dynamic Models\Linear_interpolation\desc",["description"])
+
+def test_set_attr_by_path(pfp, activate_test_project):
+    pfp.set_attr_by_path(r"Library\Dynamic Models\Linear_interpolation\desc",["description"])
     with pytest.raises(powfacpy.exceptions.PFPathError):
-        pfbi.set_attr_by_path(r"Stretchwork Model\Stretchwork Data\Grid\Termalamala",["description"])
+        pfp.set_attr_by_path(r"Stretchwork Model\Stretchwork Data\Grid\Termalamala",["description"])
+
 
-def test_get_attr(pfbi, activate_test_project):
-    terminal_1 = pfbi.get_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 1")[0]
-    systype = pfbi.get_attr(terminal_1,"systype")
+def test_get_attr(pfp, activate_test_project):
+    terminal_1 = pfp.get_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 1")[0]
+    systype = pfp.get_attr(terminal_1,"systype")
     assert systype == 0
     with pytest.raises(powfacpy.exceptions.PFAttributeError):
-        systype = pfbi.get_attr(terminal_1,"trixi")
+        systype = pfp.get_attr(terminal_1,"trixi")
+
 
-def test_create_by_path(pfbi, activate_test_project):
-    pfbi.create_by_path(r"Library\Dynamic Models\dummy.BlkDef")   
+def test_create_by_path(pfp, activate_test_project):
+    pfp.create_by_path(r"Library\Dynamic Models\dummy.BlkDef")   
     with pytest.raises(powfacpy.exceptions.PFPathError):
-        pfbi.create_by_path(r"ry\Dynamic Models\dummy.BlkDef")
+        pfp.create_by_path(r"ry\Dynamic Models\dummy.BlkDef")
     with pytest.raises(TypeError):
-        pfbi.create_by_path(4)
+        pfp.create_by_path(4)
 
-def test_create_in_folder(pfbi, activate_test_project):
-    pfbi.create_in_folder(r"Library\Dynamic Models","dummy2.BlkDef")
+
+def test_create_in_folder(pfp, activate_test_project):
+    pfp.create_in_folder("dummy2.BlkDef", r"Library\Dynamic Models")
     with pytest.raises(TypeError):
-        pfbi.create_in_folder(r"Library\Dynamic Models",2)
+        pfp.create_in_folder(2, r"Library\Dynamic Models")
+
 
-def test_get_by_condition(pfbi, activate_test_project):
-    folder = r"Network Model\Network Data\test_base_interface\Grid"
-    all_terminals = pfbi.get_obj("*.ElmTerm", parent_folder=folder)
+def test_get_by_condition(pfp, activate_test_project):
+    folder = r"Network Model\Network Data\test_active_project_interface\Grid"
+    all_terminals = pfp.get_obj("*.ElmTerm", parent_folder=folder)
     
-    mv_terminals = pfbi.get_by_condition(all_terminals, lambda x:getattr(x,"uknom") > 100)
+    mv_terminals = pfp.get_by_condition(all_terminals, lambda x:getattr(x,"uknom") > 100)
     assert len(mv_terminals) == 2
 
     with pytest.raises(powfacpy.exceptions.PFAttributeError):
-        mv_terminals = pfbi.get_by_condition(all_terminals,
+        mv_terminals = pfp.get_by_condition(all_terminals,
             lambda x:getattr(x,"wrong_attr") > 100)
 
-def test_delete_obj(pfbi, activate_test_project):
+
+def test_delete_obj(pfp, activate_test_project):
     folder = r"Library\Dynamic Models\TestDelete"
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_1.BlkDef")
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_2.BlkDef")    
-    pfbi.delete_obj("dummy_to_be_deleted*", parent_folder=folder)
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder,
+    pfp.create_in_folder("dummy_to_be_deleted_1.BlkDef", folder,)
+    pfp.create_in_folder("dummy_to_be_deleted_2.BlkDef", folder,)    
+    pfp.delete_obj("dummy_to_be_deleted*", parent_folder=folder)
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder,
         error_if_non_existent=False)
     assert len(objects_in_folder) == 0
 
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_1.BlkDef")
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_2.BlkDef")    
-    pfbi.delete_obj("dummy_to_be_deleted_1.BlkDef", parent_folder=folder)
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder)
+    pfp.create_in_folder("dummy_to_be_deleted_1.BlkDef", folder,)
+    pfp.create_in_folder("dummy_to_be_deleted_2.BlkDef", folder,)    
+    pfp.delete_obj("dummy_to_be_deleted_1.BlkDef", parent_folder=folder)
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder)
     assert len(objects_in_folder) == 1
     
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_1.BlkDef")
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_2.BlkDef")
-    pfbi.delete_obj("dummy_to_be_deleted*",
+    pfp.create_in_folder("dummy_to_be_deleted_1.BlkDef", folder,)
+    pfp.create_in_folder("dummy_to_be_deleted_2.BlkDef", folder,)
+    pfp.delete_obj("dummy_to_be_deleted*",
         parent_folder=r"Library\Dynamic Models", include_subfolders=True)
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder,
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder,
         error_if_non_existent=False)
     assert len(objects_in_folder) == 0
 
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_1.BlkDef")
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_2.BlkDef")
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder)
-    pfbi.delete_obj(objects_in_folder)
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder,
+    pfp.create_in_folder("dummy_to_be_deleted_1.BlkDef",folder,)
+    pfp.create_in_folder("dummy_to_be_deleted_2.BlkDef",folder,)
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder)
+    pfp.delete_obj(objects_in_folder)
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder,
         error_if_non_existent=False)
     assert len(objects_in_folder) == 0
 
-    pfbi.create_in_folder(folder,"dummy_to_be_deleted_1.BlkDef")
-    object_in_folder = pfbi.get_single_obj("*", parent_folder=folder)
-    pfbi.delete_obj(object_in_folder)
-    objects_in_folder = pfbi.get_obj("*", parent_folder=folder,
+    pfp.create_in_folder("dummy_to_be_deleted_1.BlkDef",folder)
+    object_in_folder = pfp.get_single_obj("*", parent_folder=folder)
+    pfp.delete_obj(object_in_folder)
+    objects_in_folder = pfp.get_obj("*", parent_folder=folder,
         error_if_non_existent=False)
     assert len(objects_in_folder) == 0
 
-def test_copy_obj(pfbi, activate_test_project):
+
+def test_copy_obj(pfp, activate_test_project):
     folder_copy_from = r"Library\Dynamic Models\TestCopyFrom"
     folder_copy_to = r"Library\Dynamic Models\TestCopyTo"
 
-    pfbi.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
-    copied_objects = pfbi.copy_obj("*", folder_copy_to, parent_folder=folder_copy_from)
+    pfp.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
+    copied_objects = pfp.copy_obj("*", folder_copy_to, parent_folder=folder_copy_from)
     assert len(copied_objects) == 2
     # test that the copied objects are returned and not the initial objects to be copied
-    obj_to_be_copied = pfbi.get_obj("*", parent_folder=folder_copy_from)
+    obj_to_be_copied = pfp.get_obj("*", parent_folder=folder_copy_from)
     for idx, obj in enumerate(obj_to_be_copied):
         assert copied_objects[idx] != obj
     
-    pfbi.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
-    folder_copy_from = pfbi.get_obj(r"Library\Dynamic Models\TestCopyFrom")[0]
-    folder_copy_to = pfbi.get_obj(r"Library\Dynamic Models\TestCopyTo")[0]
-    copied_objects = pfbi.copy_obj("*", folder_copy_to, parent_folder = folder_copy_from)
+    pfp.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
+    folder_copy_from = pfp.get_obj(r"Library\Dynamic Models\TestCopyFrom")[0]
+    folder_copy_to = pfp.get_obj(r"Library\Dynamic Models\TestCopyTo")[0]
+    copied_objects = pfp.copy_obj("*", folder_copy_to, parent_folder = folder_copy_from)
     assert len(copied_objects) == 2
 
-    objects_to_copy = pfbi.get_obj("*", parent_folder=folder_copy_from)
-    copied_objects = pfbi.copy_obj(objects_to_copy, folder_copy_to, overwrite=False)
+    objects_to_copy = pfp.get_obj("*", parent_folder=folder_copy_from)
+    copied_objects = pfp.copy_obj(objects_to_copy, folder_copy_to, overwrite=False)
     assert len(copied_objects) == 2
-    all_objects_in_folder = pfbi.get_obj("*", parent_folder=folder_copy_to)
+    all_objects_in_folder = pfp.get_obj("*", parent_folder=folder_copy_to)
     assert len(all_objects_in_folder) == 4
     
-    pfbi.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
-    objects_to_copy = pfbi.get_obj("*", parent_folder=folder_copy_from)[0]
-    copied_objects = pfbi.copy_obj(objects_to_copy, folder_copy_to, overwrite=False)
+    pfp.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
+    objects_to_copy = pfp.get_obj("*", parent_folder=folder_copy_from)[0]
+    copied_objects = pfp.copy_obj(objects_to_copy, folder_copy_to, overwrite=False)
     assert len(copied_objects) == 1
-    all_objects_in_folder = pfbi.get_obj("*", parent_folder=folder_copy_to)
+    all_objects_in_folder = pfp.get_obj("*", parent_folder=folder_copy_to)
     assert len(all_objects_in_folder) == 1
 
-def test_copy_single_obj(pfbi, activate_test_project):
+
+def test_copy_single_obj(pfp, activate_test_project):
     folder_copy_from = r"Library\Dynamic Models\TestDummyFolder"
     folder_copy_to = r"Library\Dynamic Models\TestCopy"
 
-    pfbi.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
-    copied_object=pfbi.copy_single_obj("dummy.*", folder_copy_to,
+    pfp.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
+    copied_object=pfp.copy_single_obj("dummy.*", folder_copy_to,
         parent_folder=folder_copy_from, new_name="new_dummy_name")
-    copied_obj_from_folder = pfbi.get_single_obj("new_dummy_name",
+    copied_obj_from_folder = pfp.get_single_obj("new_dummy_name",
         parent_folder = folder_copy_to)
     assert copied_object == copied_obj_from_folder
 
-    obj_to_copy = pfbi.get_single_obj("dummy2.*", parent_folder=folder_copy_from)
-    copied_object=pfbi.copy_single_obj(obj_to_copy, folder_copy_to, overwrite=True) 
-    copied_obj_from_folder = pfbi.get_single_obj("dummy2",
+    obj_to_copy = pfp.get_single_obj("dummy2.*", parent_folder=folder_copy_from)
+    copied_object=pfp.copy_single_obj(obj_to_copy, folder_copy_to, overwrite=True) 
+    copied_obj_from_folder = pfp.get_single_obj("dummy2",
         parent_folder = folder_copy_to)
     assert copied_object == copied_obj_from_folder
 
-    pfbi.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
-    obj_to_copy = pfbi.get_single_obj("dummy2.*", parent_folder=folder_copy_from)
-    copied_object=pfbi.copy_single_obj(obj_to_copy, folder_copy_to, overwrite=False,
+    pfp.delete_obj("*", parent_folder=folder_copy_to, error_if_non_existent=False)
+    obj_to_copy = pfp.get_single_obj("dummy2.*", parent_folder=folder_copy_from)
+    copied_object=pfp.copy_single_obj(obj_to_copy, folder_copy_to, overwrite=False,
         parent_folder=folder_copy_from, new_name="new_dummy_name")  
-    copied_obj_from_folder = pfbi.get_single_obj("new_dummy_name",
+    copied_obj_from_folder = pfp.get_single_obj("new_dummy_name",
         parent_folder = folder_copy_to)
     assert copied_object == copied_obj_from_folder
 
-def test_handle_single_pf_object_or_path_input(pfbi, activate_test_project):
-    folder = pfbi.get_obj(r"Network Model\Network Data")[0]
+
+def test_handle_single_pf_object_or_path_input(pfp, activate_test_project):
+    folder = pfp.get_obj(r"Network Model\Network Data")[0]
     with pytest.raises(TypeError):
-        pfbi.handle_single_pf_object_or_path_input([folder])
+        pfp._handle_single_pf_object_or_path_input([folder])
     
-    same_folder_returned = pfbi.handle_single_pf_object_or_path_input(folder)
+    same_folder_returned = pfp._handle_single_pf_object_or_path_input(folder)
     assert same_folder_returned == folder
 
-    same_folder_using_string = pfbi.handle_single_pf_object_or_path_input(
+    same_folder_using_string = pfp._handle_single_pf_object_or_path_input(
         r"Network Model\Network Data")
     assert same_folder_using_string == folder
 
-def test_get_parameter_value_string(pfbi, activate_test_project):
+
+def test_get_parameter_value_string(pfp, activate_test_project):
     params = {
-        "p":r"Network Model\Network Data\test_base_interface\Grid\General Load HV\plini",
-        "q":r"Network Model\Network Data\test_base_interface\Grid\General Load HV\qlini",
-        "u":r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 2\uknom"
+        "p":r"Network Model\Network Data\test_active_project_interface\Grid\General Load HV\plini",
+        "q":r"Network Model\Network Data\test_active_project_interface\Grid\General Load HV\qlini",
+        "u":r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 2\uknom"
     }
-    pfbi.get_parameter_value_string(params, delimiter=" ")      
+    pfp.get_parameter_value_string(params, delimiter=" ")      
+
 
-def test_create_directory(pfbi, activate_test_project):
-    pfbi.create_directory(r"test1\test2",
+def test_create_directory(pfp, activate_test_project):
+    pfp.create_directory(r"test1\test2",
         parent_folder=r"Study Cases\test_case_studies")
 
-    pfbi.create_directory(r"test1\test2\test3\test4",
+    pfp.create_directory(r"test1\test2\test3\test4",
         parent_folder=r"Study Cases\test_case_studies")
-    pfbi.delete_obj("test1", parent_folder=r"Study Cases\test_case_studies")
+    pfp.delete_obj("test1", parent_folder=r"Study Cases\test_case_studies")
+
+    pfp.create_directory(r"test1\test2")
+    pfp.delete_obj("test1")
 
-    pfbi.create_directory(r"test1\test2")
-    pfbi.delete_obj("test1")
 
-def test_get_loc_name_with_class(pfbi, activate_test_project):
-    pf_objects = pfbi.get_obj(r'*.ElmTerm', include_subfolders=True)
-    pfbi.get_loc_name_with_class(pf_objects)
-    pfbi.get_loc_name_with_class(pf_objects[0])
+def test_get_loc_name_with_class(pfp, activate_test_project):
+    pf_objects = pfp.get_obj(r'*.ElmTerm', include_subfolders=True)
+    pfp.get_loc_name_with_class(pf_objects)
+    pfp.get_loc_name_with_class(pf_objects[0])
 
-def test_create_comtrade_obj(pfbi, activate_test_project):
+
+def test_create_comtrade_obj(pfp, activate_test_project):
     path_of_cfg = os.path.dirname(__file__) + r"\tests_input\test_comtrade.cfg"
-    intcomtrade = pfbi.create_comtrade_obj(path_of_cfg)
+    intcomtrade = pfp.create_comtrade_obj(path_of_cfg)
     intcomtrade.Load()
     assert(intcomtrade.FindColumn("AC Voltage Source:m:u:bus1:A") == 1)
 
-def test_replace_outside_or_inside_of_strings_in_a_string(pfbi,               activate_test_project):
+
+def test_replace_outside_or_inside_of_strings_in_a_string(pfp, activate_test_project):
     conditions = "lorem ipsum control 1 == 'ABC control 1' 'control 1' control 1"
     conditions = powfacpy.PFStringManipulation.replace_outside_or_inside_of_strings_in_a_string(
 	    conditions, {"control 1": "x[1]"})    
     assert(conditions == "lorem ipsum x[1] == 'ABC control 1' 'control 1' x[1]")
 
     conditions = "lorem ipsum control 1 == 'ABC control 1' 'control 1'"
     conditions = powfacpy.PFStringManipulation.replace_outside_or_inside_of_strings_in_a_string(
@@ -307,33 +321,62 @@
     assert(conditions == "lorem ipsum x[1] == 'ABC control 1' 'control 1'")
 
     conditions = "lorem ipsum control 1 == 'ABC control 1' 'control 1' "
     conditions = powfacpy.PFStringManipulation.replace_outside_or_inside_of_strings_in_a_string(
 	    conditions, {"control 1": "x[1]"}, outside=False)    
     assert(conditions == "lorem ipsum control 1 == 'ABC x[1]' 'x[1]'")
 
-def test_get_path_of_object(pfbi, activate_test_project):
-    path = "Network Model\\Network Data\\test_base_interface\\Grid\\Line 1.2"
-    line = pfbi.get_unique_obj(path)    
-    path_derived = pfbi.get_path_of_object(line)
+
+def test_get_path_of_object(pfp, activate_test_project):
+    path = "Network Model\\Network Data\\test_active_project_interface\\Grid\\Line 1.2"
+    line = pfp.get_unique_obj(path)    
+    path_derived = pfp.get_path_of_object(line)
     assert (path==path_derived)
 
-def test_get_upstream_object(pfbi, activate_test_project):
-    grid = pfbi.get_upstream_obj(r"Network Model\Network Data\test_database_interface\Grid\Voltage source ctrl\Frequency",
+
+def test_get_upstream_object(pfp, activate_test_project):
+    grid = pfp.get_upstream_obj(r"Network Model\Network Data\test_database_interface\Grid\Voltage source ctrl\Frequency",
                       lambda x: x.loc_name == "Grid")
-    grid_using_get_unique_obj = pfbi.get_unique_obj(r"Network Model\Network Data\test_database_interface\Grid")
+    grid_using_get_unique_obj = pfp.get_unique_obj(r"Network Model\Network Data\test_database_interface\Grid")
     assert(grid == grid_using_get_unique_obj)
     with pytest.raises(Exception):
-        pfbi.get_upstream_obj(r"Network Model\Network Data\test_database_interface\Grid\Voltage source ctrl\Frequency",
+        pfp.get_upstream_obj(r"Network Model\Network Data\test_database_interface\Grid\Voltage source ctrl\Frequency",
                         lambda x: x.loc_name == "wrong name") 
 
-def test_get_from_study_case(pfbi, activate_test_project):
-    pfbi.activate_study_case(r"Study Cases\test_base_interface\multiple_elmres")
+
+def test_get_from_study_case(pfp, activate_test_project):
+    pfp.activate_study_case(r"Study Cases\test_active_project_interface\multiple_elmres")
     with pytest.warns():
-        pfbi.get_from_study_case("ElmRes")
+        pfp.get_from_study_case("ElmRes")
     with pytest.raises(Exception):    
-        pfbi.get_from_study_case("ElmRes", if_not_unique="error")
+        pfp.get_from_study_case("ElmRes", if_not_unique="error")
+        
+        
+def test_get_calc_relevant_obj(pfp, activate_test_project): 
+    pfp.activate_study_case(r"Study Cases\test_active_project_interface\Study Case 1")
+    # Assert similar objects found with with get_obj  
+    terminals_getobj = []
+    for network in pfp.get_active_networks():     
+        terminals_getobj += pfp.get_obj("*.ElmTerm", 
+                                        parent_folder=network,
+                                        include_subfolders=True)
+    terminals_calc_rel = pfp.get_calc_relevant_obj("*.ElmTerm")
+    assert len(terminals_getobj) == len(terminals_calc_rel)
+    
+    terminals_getobj = []
+    for network in pfp.get_active_networks():     
+        terminals_getobj += pfp.get_obj("*.ElmTerm", 
+                                    parent_folder=network,
+                                    include_subfolders=True,
+                                    condition=lambda x: x.uknom > 100)
+    terminals_calc_rel = pfp.get_calc_relevant_obj(
+        "*.ElmTerm",
+        condition=lambda x: x.uknom > 100)
+    assert len(terminals_getobj) == len(terminals_calc_rel)
     
+    with pytest.raises(powfacpy.PFNonExistingObjectError):    
+        pfp.get_calc_relevant_obj("*.ElmTerm", 
+                                  condition=lambda x: x.uknom > 5000)
 
 if __name__ == "__main__":
-    pytest.main([r"tests\test_base_interface.py"])
-    # pytest.main(([r"tests"]))
+    pytest.main([r"tests\test_active_project_interface.py::test_get_calc_relevant_obj"])
+    #pytest.main(([r"tests"]))
```

### Comparing `powfacpy-0.1.4/tests/test_case_studies.py` & `powfacpy-0.1.5/tests/test_case_studies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import pytest
 import sys
 
+import pytest
+
 sys.path.insert(0, r'.\src')
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
+from test_active_project_interface import pfp, pf_app, activate_test_project
 
-from test_base_interface import pfbi, pf_app, activate_test_project
 
 @pytest.fixture
 def pfsc(pf_app):
     return powfacpy.PFStudyCases(pf_app)
 
 def test_create_cases_1(pfsc, activate_test_project):   
     pfsc.parameter_values = {
@@ -295,19 +296,19 @@
     pfsc.clear_parent_folders()
     pfsc.base_study_case = r"Study Cases\test_case_studies\base_study_case"
     pfsc.create_cases()    
     # Actual tests
     # Make sure the various possible input argument variations give
     # the same results.
     study_cases = pfsc.study_cases    
-    study_cases1, case_numbers1 = pfsc.handle_study_case_objects_case_numbers_input(
+    study_cases1, case_numbers1 = pfsc._handle_study_case_objects_case_numbers_input(
       study_cases=pfsc.study_cases)
     assert(study_cases == study_cases1)
-    study_cases2, case_numbers2 = pfsc.handle_study_case_objects_case_numbers_input( 
+    study_cases2, case_numbers2 = pfsc._handle_study_case_objects_case_numbers_input( 
       case_numbers=case_numbers1)
     assert(case_numbers1 == case_numbers2)
-    study_cases3, case_numbers3 = pfsc.handle_study_case_objects_case_numbers_input()
+    study_cases3, case_numbers3 = pfsc._handle_study_case_objects_case_numbers_input()
     assert(study_cases == study_cases3)
     assert(case_numbers2 == list(case_numbers3))
 
 if __name__ == "__main__":
-    pytest.main(([r"tests\test_case_studies.py::test_export_results_of_study_cases_to_csv"]))
+    pytest.main(([r"tests\test_case_studies.py"]))
```

### Comparing `powfacpy-0.1.4/tests/test_database_interface.py` & `powfacpy-0.1.5/tests/test_database_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-import pytest
 import sys
 import json
+import importlib
+
+import pytest
+from jsondiff import diff
+
 settings_file = open('.\\settings.json')
 settings = json.load(settings_file)
 sys.path.append(settings["local path to PowerFactory application"])
 import powerfactory
 sys.path.insert(0, r'.\src')
 import powfacpy 
-import importlib
 importlib.reload(powfacpy)
-from jsondiff import diff
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+
+from test_active_project_interface import pfp, pf_app, activate_test_project
 
 @pytest.fixture
 def pfdbi(pf_app):
   # Return PFDataBaseInterface instance
   return powfacpy.PFDatabaseInterface(pf_app)
 
 def test_get_and_set_object_attributes(pfdbi, activate_test_project):
@@ -26,16 +29,15 @@
     1. getting data of PF objects from the PF database.
     2. modifiy some of the data.
     3. setting the data of the PF objects in the PF database with the output from 2.
     4. again getting data of PF objects from the PF database.
     5. Checking if the output from 2. and 4. are equal. If so, getting and setting
     data works correctly.
   This process is done with various optional arguments (relative_paths, pf_obj_handling_options).
-  The json files under 'tests\tests_output\test_get_object_attributes*.json' can help with the 
-  interpretation of the operations.
+  The json files under 'tests\tests_output\test_get_object_attributes*.json' can help with the interpretation of the operations.
   """
   truncated_paths = ["", r"Network Model\Network Data"]
   pf_obj_handling_options = ["path", "original_pf_obj"]
   for truncated_path in truncated_paths:
     for pf_obj_handling in pf_obj_handling_options:
       objs = pfdbi.get_obj("*",parent_folder=r"Network Model\Network Data\test_database_interface\Grid")
       class_attributes =  {
@@ -64,8 +66,8 @@
         truncated_path=truncated_path,
         pf_obj_handling = pf_obj_handling) 
       assert(not diff(obj_attr_dict, obj_attr_dict_after_reading_and_writing))
 
 
 if __name__ == "__main__":
   pytest.main([r"tests\test_database_interface.py"])
-  # pytest.main(([r"tests"]))
+  # pytest.main(([r"tests"]))
```

### Comparing `powfacpy-0.1.4/tests/test_dyn_sim_interface.py` & `powfacpy-0.1.5/tests/test_dyn_sim_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import pytest
 import sys
 sys.path.insert(0, r'.\src')
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
 from os import remove, getcwd
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+import pytest
+
+from test_active_project_interface import pfp, pf_app, activate_test_project
+
 
 @pytest.fixture
 def pfsim(pf_app):
     # Return PFDynSimInterface instance
     return powfacpy.PFDynSimInterface(pf_app)   
 
 def test_export_to_csv(pfsim, activate_test_project):
@@ -57,18 +59,18 @@
     array_returned = powfacpy.PFDynSimInterface.get_dsl_obj_array(
         dsl_obj, array_num=2, size_included_in_array=False)
     assert(array_returned == array_two_column)
 
 def test_create_event(pfsim, activate_test_project):
     
     target = pfsim.get_single_obj(r"Network Model\Network Data\test_dyn_sim_interface\Grid 1\AC Voltage Source")
-    pfsim.create_event("test.EvtParam",{"time":1,"p_target":target,"variable":"u0","value":"1.05"})
+    pfsim.create_dyn_sim_event("test.EvtParam",{"time":1,"p_target":target,"variable":"u0","value":"1.05"})
 
     target = pfsim.get_single_obj(r"Network Model\Network Data\test_dyn_sim_interface\Grid 1\General Load HV")
-    pfsim.create_event("loadevent.EvtLod",{"time":1,"p_target":target,"dP":100})
+    pfsim.create_dyn_sim_event("loadevent.EvtLod",{"time":1,"p_target":target,"dP":100})
     
 def test_get_parameters_of_dsl_models_in_composite_model(pfsim, activate_test_project):
     pfsim.get_single_obj(r"Study Cases\test_dyn_sim_interface\Study Case").Activate()
     composite_model = pfsim.get_unique_obj(
         r"Network Model\Network Data\test_dyn_sim_interface\Grid 1\test_composite_model")
     
     par_val_dict_1 = pfsim.get_parameters_of_dsl_models_in_composite_model(
```

### Comparing `powfacpy-0.1.4/tests/test_network_interface.py` & `powfacpy-0.1.5/tests/test_network_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 import sys
 sys.path.insert(0, r'.\src')
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+from test_active_project_interface import pfp, pf_app, activate_test_project
 
 @pytest.fixture
 def pfni(pf_app):
   return powfacpy.PFNetworkInterface(pf_app)
 
 def test_get_vacant_cubicle_of_terminal(pfni, activate_test_project):
   study_case = pfni.get_single_obj(r"Study Cases\test_network_interface\Study Case")
   study_case.Activate()
   pfni.get_vacant_cubicle_of_terminal(
     r"Network Model\Network Data\test_plot_interface\Grid 1\Terminal HV 2")
 
 if __name__ == "__main__":
-  pytest.main(([r"tests\test_network_interface.py"]))
+  pytest.main(([r"tests\test_network_interface.py"]))
```

### Comparing `powfacpy-0.1.4/tests/test_plot_interface.py` & `powfacpy-0.1.5/tests/test_plot_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
 from matplotlib import pyplot
 from os import getcwd
 import os
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+from test_active_project_interface import pfp, pf_app, activate_test_project
+
 
 @pytest.fixture
 def pfplot(pf_app):
     # Return PFPlotInterface instance and show app
     pfplot = powfacpy.PFPlotInterface(pf_app)
     
     return pfplot 
@@ -57,16 +58,16 @@
     pfsim.initialize_and_run_sim()
     pfri = powfacpy.PFResultsInterface(pfplot.app)
     pfri.export_to_csv(export_dir,file_name=file_name)
 
     pyplot.figure()
     powfacpy.PFPlotInterface.plot_from_csv(
         export_dir + "\\" + file_name + ".csv",
-        [r"Network Model\Network Data\test_plot_interface\Grid 1\AC Voltage Source\s:u0",
-        r"Network Model\Network Data\test_plot_interface\Grid 1\AC Voltage Source\m:Qsum:bus1"]) 
+        [r"test_plot_interface\Grid 1\AC Voltage Source\s:u0",
+        r"test_plot_interface\Grid 1\AC Voltage Source\m:Qsum:bus1"]) 
     pyplot.xlabel("t [s]")
 
 def test_copy_graphics_board_content(pfplot, activate_test_project):
     source_study_case = r"Study Cases\test_plot_interface\Study Case 1"
     target_study_cases = [r"Study Cases\test_plot_interface\Study Case 2", 
         r"Study Cases\test_plot_interface\Study Case 3"]
     pfplot.copy_graphics_board_content(source_study_case, target_study_cases,
@@ -88,15 +89,15 @@
         linestyle=2, linewidth=100, color=3, label="comtrade test")
 
 def test_activate_plot(pfplot, activate_test_project):
     with pytest.raises(powfacpy.PFAttributeNotSetError):
         pfplot.set_active_plot("test_plot 1")
 
 def test_clear_curves_by_index_from_active_plot(pfplot, activate_test_project):
-    pfplot.get_unique_obj(r"Study Cases\test_plot_interface\Study Case 1").Activate()
+    pfplot.get_unique_obj(r"Study Cases\test_plot_interface\Study Case 1", include_subfolders = False).Activate()
     pfplot.set_active_plot("test clear curves","test clear curves")
 
     # Plot and simulate    
     pfplot.clear_curves()
     pfplot.plot(r"Network Model\Network Data\test_plot_interface\Grid 1\AC Voltage Source","m:Psum:bus1")
     pfplot.plot(r"Network Model\Network Data\test_plot_interface\Grid 1\AC Voltage Source","m:Qsum:bus1")
     pfplot.plot(r"Network Model\Network Data\test_plot_interface\Grid 1\AC Voltage Source","s:u0")
```

### Comparing `powfacpy-0.1.4/tests/test_results_interface.py` & `powfacpy-0.1.5/tests/test_results_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import pytest
 import sys
 sys.path.insert(0, r'.\src')
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
 from os import getcwd
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+import pytest
+
+from test_active_project_interface import pfp, pf_app, activate_test_project
 
 @pytest.fixture
 def pfri(pf_app):
     # Return PFResultsInterface instance and show app
     pfri = powfacpy.PFResultsInterface(pf_app)
     return pfri
 
 def test_export_to_csv(pfri, activate_test_project):
     study_case_1 = pfri.get_unique_obj(r"Study Cases\test_results_interface\Export Simulation 1.IntCase")
     study_case_2 = pfri.get_unique_obj(r"Study Cases\test_results_interface\Export Simulation 2.IntCase")
     pfdi = powfacpy.PFDynSimInterface(pfri.app)
     elmres_list = []
-    terminal_hv_1 = pfri.get_unique_obj(r"Network Model\Network Data\test_base_interface\Grid\Terminal HV 2")
+    terminal_hv_1 = pfri.get_unique_obj(r"Network Model\Network Data\test_active_project_interface\Grid\Terminal HV 2")
     for case in [study_case_1, study_case_2]:
         case.Activate()
         pfdi.add_results_variable(terminal_hv_1,"m:u1")
         pfdi.initialize_and_run_sim()
         elmres_list.append(pfri.get_from_study_case("ElmRes"))
     study_case_1.Activate()
     dir = getcwd()  + "\\tests\\tests_output"
@@ -76,18 +77,18 @@
     pfri.get_unique_obj(r"Study Cases\test_results_interface\Study Case").Activate()
     network_element = pfri.get_obj(r'Network Model\Network Data\test_results_interface\Grid\General Load HV.ElmLod', include_subfolders=True)[0]
     variables = ['m:i1:bus1', 'm:u1:bus1']
     elmres = pfri.add_results_variable(network_element, variables)
     pfdi = powfacpy.PFDynSimInterface(pfri.app)
     pfdi.initialize_sim(param={"p_resvar":elmres})
     pfdi.run_sim()
-    nr_of_columns_including_time = len(variables) + 1
+    nr_of_columns = len(variables)
     df = pfri.export_to_pandas(
         list_of_results_objs=[elmres,]*len(variables),
         elements=[network_element,]*len(variables), 
         variables=variables)
-    assert len(df.columns) == nr_of_columns_including_time
+    assert len(df.columns) == nr_of_columns
 
     df = pfri.export_to_pandas()
 
 if __name__ == "__main__":
     pytest.main(([r"tests\test_results_interface.py"]))
```

### Comparing `powfacpy-0.1.4/tests/test_script_interface.py` & `powfacpy-0.1.5/tests/test_script_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import pytest
 import sys
 
 sys.path.insert(0, r'.\src')
 import powfacpy 
 import importlib
 importlib.reload(powfacpy)
 
-from test_base_interface import pfbi, pf_app, activate_test_project
+import pytest
+
+from test_active_project_interface import pfp, pf_app, activate_test_project
 
 @pytest.fixture
 def pfscripts(pf_app):
     return powfacpy.PFComPythonObjectInterface(pf_app)
 
 def test_create_file_from_embedded_script(pfscripts, activate_test_project):
   compython = r"Library\Scripts\embedded_test_script"
```

### Comparing `powfacpy-0.1.4/tests/tests_input/test_comtrade.cfg` & `powfacpy-0.1.5/tests/tests_input/test_comtrade.cfg`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tests/tests_input/test_comtrade.dat` & `powfacpy-0.1.5/tests/tests_input/test_comtrade.dat`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tests/tests_output/powfacpy_single_file.py` & `powfacpy-0.1.5/tests/tests_output/powfacpy_single_file.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tests/tests_output/test1.json` & `powfacpy-0.1.5/tests/tests_output/test1.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tests/tests_output/test2.json` & `powfacpy-0.1.5/tests/tests_output/test2.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/study_cases.ipynb` & `powfacpy-0.1.5/tutorials/study_cases.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886025746051788%*

 * *Differences: {"'cells'": "{1: {'execution_count': 2, 'outputs': {0: {'execution_count': 2}}, 'source': {insert: "*

 * *            '[(2, "sys.path.append(r\'C:\\\\Program Files\\\\DIgSILENT\\\\PowerFactory 2023 '*

 * *            'SP3\\\\Python\\\\3.11\') # you may use a different directory\\n"), (6, \'\\n\'), (9, '*

 * *            '\'app.ActivateProject(r"powfacpy\\\\powfacpy_tests_copy_where_tests_are_run") # You '*

 * *            "may change the project path.')], delete: [8, 2]}}, 2: {'source': {insert: [(1, 'We "*

 * *            'use the […]*

```diff
@@ -8,146 +8,152 @@
                 "Parameter studies are organized in study cases, operation scenarios and variations in PowerFactory. This tutorials shows how to create parameter studies with ease and fully automated using the study cases interface of *powfacpy*.  \n",
                 "\n",
                 "First, we activate the PowerFactory project as in the *getting started* tutorial."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "0"
                         ]
                     },
-                    "execution_count": 1,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# If you use IPython/Jupyter:\n",
                 "import sys\n",
-                "sys.path.append(r'C:\\Program Files\\DIgSILENT\\PowerFactory 2023 SP5\\Python\\3.10') # you may use a different directory\n",
+                "sys.path.append(r'C:\\Program Files\\DIgSILENT\\PowerFactory 2023 SP3\\Python\\3.11') # you may use a different directory\n",
                 "# Get the PF app\n",
                 "import powerfactory\n",
                 "app = powerfactory.GetApplication()\n",
+                "\n",
                 "import powfacpy\n",
                 "app.Show()\n",
-                "app.ActivateProject(r\"powfacpy\\powfacpy_tests\") # You may change the project path.\n"
+                "app.ActivateProject(r\"powfacpy\\powfacpy_tests_copy_where_tests_are_run\") # You may change the project path."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Simple Parameter Study\n",
-                "We use the class `PFStudyCases`. This class inherits from `PFBaseInterface`, so all methods from that class are available. We want to create study case with various values for the active and reactive power of a load. \n",
+                "We use the class `PFStudyCases`. This class inherits from `PFActiveProject`, so all methods from that class are available. We want to create study case with various values for the active and reactive power of a load. \n",
                 "\n",
                 "First we set the attribute `parameter_values` and define a dictionary with parameter names and a list of values. Each element in the lists is used in one study case. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pfsc = powfacpy.PFStudyCases(app)\n",
                 "pfsc.parameter_values = {\n",
                 "    \"p HV load\":[ 1,  2, 1, 2],\n",
                 "    \"q HV load\":[-1, -1, 1, 1],\n",
-                "}\n"
+                "}"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Here we have defined four study cases and in the first case `p HV load` equals 1 and `q HV load` equals -1. The parameter names must not contain *?=\",\\~|()! as these characters cannot be used for names of objects in PF.\n",
                 "\n",
                 "Next we  connect the variables to the PF database by defining a dictionary with paths in the attribute `parameter_paths` using the same parameter names as keys. The paths include the attribute name (e.g. `plini` which is the active power of the load). "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pfsc.parameter_paths = {\n",
                 "    \"p HV load\":r\"Network Model\\Network Data\"\n",
                 "        r\"\\test_case_studies\\Grid 2\\General Load HV\\plini\", # This is one string split over several lines\n",
                 "    \"q HV load\":r\"Network Model\\Network Data\"\n",
                 "        r\"\\test_case_studies\\Grid 2\\General Load HV\\qlini\",\n",
-                "}\n"
+                "}"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Finally we define the active grids. For now, we assume that for all cases exactly one grid is active (we look at more complicated cases later). "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pfsc.active_grids = r\"Network Model\\Network Data\\test_case_studies\\Grid 2\"\n"
+                "pfsc.active_grids = r\"Network Model\\Network Data\\test_case_studies\\Grid 2\""
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now let's create the study cases."
+                "Now let's create the study cases (and corresponding operation scenarios) in a new folder named 'Autocreated':"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pfsc.create_cases()\n"
+                "pfsc.parent_folder_study_cases = pfsc.create_in_folder(\"Autocreated.IntFolder\", folder=pfsc.study_cases_folder)\n",
+                "pfsc.parent_folder_scenarios = pfsc.create_in_folder(\"Autocreated.IntFolder\", folder=pfsc.operation_scenarios_folder)\n",
+                "# Alternatively, just use\n",
+                "pfsc.set_parent_folders_for_cases_scenarios_variations(\"Autocreated\")\n",
+                "\n",
+                "pfsc.create_cases()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This creates the following study cases:\n",
+                "This creates the following study cases in the 'Autocreated' folder:\n",
                 "\n",
                 "![](figures/cases_1.png)\n",
                 "\n",
                 "The names of the study cases are created according to the parameter names and their values (\"_\" is used instead of \"=\" which is not allowed in PF object names). Furthermore, the corresponding operation scenarios are created: \n",
                 "\n",
                 "![](figures/scenarios_1.png)\n",
                 "\n",
-                "For more complicated case studies with further parameters, it is advisable to structure the cases in folders. We define the attribute `hierarchy` using a list of parameter names (in this case with only one element) that corresponds to folder directories."
+                "For more complicated case studies with further parameters, it is advisable to structure the cases in folders. We define the attribute `hierarchy` using a list (in this case with onl yone item) of parameter names that corresponds to folder directories."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pfsc.hierarchy = [\"q HV load\", \"p HV load\"]\n",
-                "pfsc.create_cases()\n"
+                "pfsc.hierarchy = [\"q HV load\"]\n",
+                "pfsc.create_cases()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -165,15 +171,15 @@
             "source": [
                 "# Advanced Parameter Study\n",
                 "Let's take a look at a more complex parameter study."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pfsc = powfacpy.PFStudyCases(app)\n",
                 "pfsc.parameter_values = {\n",
                 "    \"p HV load\":[1, 2, 1, 2, 1, 2, 1, 2, ],\n",
                 "    \"q HV load\":[-1, -1, 1, 1, -1, -1, 1, 1, ],\n",
@@ -183,53 +189,54 @@
                 "    \"p HV load\":r\"Network Model\\Network Data\"\n",
                 "        r\"\\test_case_studies\\Grid 2\\General Load HV\\plini\", \n",
                 "\n",
                 "    \"q HV load\":r\"Network Model\\Network Data\"\n",
                 "        r\"\\test_case_studies\\Grid 2\\General Load HV\\qlini\", \n",
                 "\n",
                 "}\n",
-                "pfsc.active_grids = r\"Network Model\\Network Data\\test_case_studies\\Grid 2\"\n"
+                "pfsc.active_grids = r\"Network Model\\Network Data\\test_case_studies\\Grid 2\"\n",
+                "pfsc.set_parent_folders_for_cases_scenarios_variations(\"Autocreated\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "An additional parameter `control` is defined. Note that there is no parameter path defined for this parameter. The parameter can be seen as a placeholder for the study cases structure and to do more complicated things than simply setting an attribute of a PF object later (we'll see below).\n",
                 "\n",
                 "By default, study cases and operation scenarios are created. If variations should be created in addition, use:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pfsc.add_variation_to_each_case = True\n"
+                "pfsc.add_variation_to_each_case = True"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This can be necessary because some parameters, like attributes of DSL objects, are stored in variants and not in operation scenarios.\n",
                 "Let's again create the study cases."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pfsc.hierarchy = [\"control\", \"q HV load\"]\n",
-                "pfsc.create_cases()\n"
+                "pfsc.create_cases()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -239,15 +246,15 @@
                 "\n",
                 "Let's set further parameters, add plots (using plot interface) and simulate (using dyn. simulation interface) for each study case. The study case objects are stored in the `study_cases` attribute. We can iterate through the cases and set parameters depending on the previously defined `control` parameter.\n",
                 "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pfpi = powfacpy.PFPlotInterface(app)\n",
                 "pfds = powfacpy.PFDynSimInterface(app)\n",
                 "dsl_controller_obj = pfsc.get_unique_obj(r\"Network Model\\Network Data\"\n",
                 "    r\"\\test_case_studies\\Grid 2\\WECC WT Control System Type 4A\\REEC_A Electrical Control Model\")\n",
@@ -259,15 +266,15 @@
                 "    elif pfsc.get_value_of_parameter_for_case(\"control\", case_num) == \"B\":\n",
                 "        pfsc.set_attr(dsl_controller_obj, {\"PfFlag\":1, \"VFlag\":0}) \n",
                 "    # Prepare plots\n",
                 "    pfpi.clear_plot_pages()\n",
                 "    pfpi.set_active_plot(\"Reactive current\", \"WPP\")\n",
                 "    pfpi.plot(dsl_controller_obj, \"s:Iqcmd\")\n",
                 "    # Simulate   \n",
-                "    pfds.initialize_and_run_sim() \n"
+                "    pfds.initialize_and_run_sim() "
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -284,20 +291,20 @@
             "source": [
                 "# Compare Study Cases\n",
                 "It is often required to compare the results of cases. In the following, we use the previously defined cases to compare the simulation results for cases where the parameter `p HV load` equals 1 (note that you may have to \"Rebuild\" ![](figures/rebuild_button.png) the plot in the upper left for PF to show it correctly):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 28,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Create a study case where results from other cases are compared in a plot\n",
-                "study_case_comparison = pfsc.create_by_path(r\"Study Cases\\Comparison.IntCase\")\n",
+                "study_case_comparison = pfsc.create_by_path(r\"Study Cases\\Autocreated\\Comparison.IntCase\")\n",
                 "study_case_comparison.Activate()\n",
                 "pfpi.clear_plot_pages()\n",
                 "pfpi.set_active_plot(\"Reactive current controller setpoint for p HV load = 1\", \"Comparison \")\n",
                 "dsl_controller_obj = (r\"Network Model\\Network Data\\test_case_studies\" \n",
                 "    r\"\\Grid 2\\WECC WT Control System Type 4A\\REEC_A Electrical Control Model\")\n",
                 "for case_num, study_case_obj in enumerate(pfsc.study_cases):  \n",
                 "    if pfsc.get_value_of_parameter_for_case(\"p HV load\", case_num) == 1:\n",
@@ -309,15 +316,15 @@
                 "            omitted_parameters=\"p HV load\",\n",
                 "            delimiter=\" | \",\n",
                 "            equals_sign=\"=\") \n",
                 "        label = \"Iq setpoint (\" + case_label + \")\"\n",
                 "        # Plot\n",
                 "        pfpi.plot(dsl_controller_obj, \"s:Iqcmd\",\n",
                 "            results_obj=results_obj,\n",
-                "            label=label)\n"
+                "            label=label)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -328,15 +335,15 @@
                 "Let's walk through the code. After creating a study case where the results are compared in a plot, it is again iterated through all cases. For cases where `p HV load` has a certain value, the result object is fetched. Next we want to create a label for the curve in the plot. We use the method `get_case_params_value_string` with certain options for the delimiter and the equals symbol (here we have more options than for PF object names, i.e. `=` and `|` are allowed). Moreover, the parameter `p HV load` is omitted because it is the same for all compared cases (i.e. 1, see condition). Further information on the variable is added to the label and the curve is finally added to the plot.\n",
                 "\n",
                 "An alternative to iterating through all study cases is to get certain cases using the method `get_study_cases`:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "study_cases_p_HV_load_equals_1 = pfsc.get_study_cases({\"p HV load\":lambda x: x==1})\n",
                 "for study_case_obj in study_cases_p_HV_load_equals_1:\n",
                 "    pass\n",
                 "    # do something with the specific cases\n"
@@ -356,20 +363,20 @@
             "metadata": {},
             "source": [
                 "A very convenient yet powerful alternative to 'get_study_cases' especially for complicated conditionals is 'get_study_cases_from_string'. This method simply accepts a string which can contain complicated conditionals:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "study_cases_from_conditionals = pfsc.get_study_cases_from_string(\n",
-                "    \"p HV load >= 2 and (control == 'A' or q HV load != 1\")\n"
+                "    \"p HV load >= 2 and (control == 'A' or q HV load != 1)\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -379,74 +386,89 @@
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Permutation\n",
                 "It is also possible to create study cases for the permutation of the parameters (i.e. all combinations).\n",
-                "This is achieved with the method `apply_permutation`. Define the parameter values first (and also the hierarchy if applicable) and then call the method. Make sure that the PF application is hidden to improve the performance (if not hidden, this can take minutes and otherwise only seconds): "
+                "This is achieved with the method `apply_permutation`. Define the parameter values first (and also the hierarchy if applicable) and then call the method. Make sure that the PF application is hidden to improve the performance (if not hidden, this can take minutes and otherwise only seconds - the 'try-finally' block ensures that the app is always shown in the end even if an exception is thrown): "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 51,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pfsc.app.Hide()\n",
-                "pfsc.parameter_values = {\n",
-                "        \"p HV load\":[1, 2, 3],\n",
-                "        \"q HV load\":[-1, 1],\n",
-                "        \"control 1\": [\"A\", \"B\"],\n",
-                "        \"control 2\": [\"R\", \"S\"],\n",
-                "    }\n",
-                "pfsc.hierarchy = [\"p HV load\", \"control 1\", ]\n",
-                "pfsc.apply_permutation()\n",
-                "pfsc.create_cases()\n",
-                "pfsc.app.Show()\n"
+                "try:\n",
+                "    pfsc = powfacpy.PFStudyCases(app)\n",
+                "    pfsc.app.Hide()\n",
+                "    pfsc.parameter_values = {\n",
+                "            \"p HV load\":[1, 2, 3],\n",
+                "            \"q HV load\":[-1, 1],\n",
+                "            \"control 1\": [\"A\", \"B\"],\n",
+                "            \"control 2\": [\"R\", \"S\"],\n",
+                "        }\n",
+                "    pfsc.hierarchy = [\"p HV load\", \"control 1\", ]\n",
+                "    pfsc.apply_permutation()\n",
+                "    pfsc.set_parent_folders_for_cases_scenarios_variations(\"Autocreated\")\n",
+                "    pfsc.clear_parent_folders()\n",
+                "    pfsc.create_cases()\n",
+                "finally:     \n",
+                "    pfsc.app.Show()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`apply_permutation` irreversibly replaces the values in `parameter_values` with the permutation. \n",
                 "\n",
-                "It may be desirable to use the permutation but omit certain combinations. These omitted combinations can be defined in a list of dictionaries and used as a keyword argument as follows: "
+                "It may be desirable to use the permutation but omit certain combinations. These omitted combinations can be defined in a list of dictionaries and used as a keyword argument as follows (note that we clear the parent folders from the formerly created objects first): "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 47,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [],
             "source": [
-                "omitted_combinations = [\n",
-                "    {\"q HV load\": [1, 0], \"control 2\": [\"R\", \"T\"]},\n",
-                "    {\"p HV load\": [2], \"control 1\": \"all\", \"control 2\": \"all\"},\n",
-                "]\n",
-                "pfsc.apply_permutation(omitted_combinations=omitted_combinations)\n"
+                "try:\n",
+                "    app.Hide()\n",
+                "    omitted_combinations = [\n",
+                "        {\"q HV load\": [1], \"control 2\": [\"R\"]},\n",
+                "        {\"p HV load\": [2, 3], \"control 1\": \"all\"},\n",
+                "    ]\n",
+                "    pfsc.apply_permutation(omitted_combinations=omitted_combinations)\n",
+                "    pfsc.clear_parent_folders()\n",
+                "    pfsc.create_cases()\n",
+                "finally:\n",
+                "    app.Show()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The first dictionary causes any combinations where \"q HV load\" is 1 or 0 and \"control 2\" is either \"R\" or \"T\" to be omitted (these cases will not be created when `create_cases` is called). In the second dictionary, the keyword \"all\" is used. This means that all combinations with this parameter are omitted."
+                "The first dictionary causes any combinations where \"q HV load\" is 1  and \"control 2\" is \"R\" to be omitted (these cases will not be created when `create_cases` is called). In the second dictionary, the keyword \"all\" is used. This means that all combinations with this parameter are omitted."
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Further functionality\n",
-                "The attributes of `PFStudyCases` instances allow to set further options. The folders in which the study cases/operation scenarios/variations are ceated can be set using the attributes `parent_folder_study_cases/parent_folder_scenarios/parent_folder_variations`. The study case names can be numbered consecutively setting `consecutively_number_case_names`. Sometimes it is convenient to use only parameter values without the parameter names for the folder/study case names (imagine the value of a parameter is expressive enough and you don't want to use \"Controller_GridCode2012Controller\" but only \"GridCode2012Controller\" instead). This can be achieved by adding parameters to the list of `anonymous_parameters` (e.g. `pfsc.anonymous_parameters=[\"Controller\",\"FurtherParName\"]`).\n"
+                "The attributes of `PFStudyCases` instances allow to set further options. \n",
+                "\n",
+                "The study case names can be numbered consecutively setting `consecutively_number_case_names`. \n",
+                "\n",
+                "Sometimes it is convenient to use only parameter values without the parameter names for the folder/study case names (imagine the value of a parameter is expressive enough and you don't want to use \"Controller_GridCode2012Controller\" but only \"GridCode2012Controller\" instead). This can be achieved by adding parameters to the list of `anonymous_parameters` (e.g. `pfsc.anonymous_parameters=[\"Controller\",\"FurtherParName\"]`).\n"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.4 64-bit",
             "language": "python",
@@ -458,15 +480,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.6"
+            "version": "3.11.7"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "20b4f2ae9a71ebfc0af8cf0167d05f9c8f5c94fe23811db744e66ae1fdb328c7"
             }
         }
```

### Comparing `powfacpy-0.1.4/tutorials/figures/cases_1.png` & `powfacpy-0.1.5/tutorials/figures/cases_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/cases_2.png` & `powfacpy-0.1.5/tutorials/figures/cases_2.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/legend_1.png` & `powfacpy-0.1.5/tutorials/figures/legend_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/object_path.png` & `powfacpy-0.1.5/tutorials/figures/object_path.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/rebuild_button.png` & `powfacpy-0.1.5/tutorials/figures/rebuild_button.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/scenarios_1.png` & `powfacpy-0.1.5/tutorials/figures/scenarios_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/tutorials/figures/variations_3.png` & `powfacpy-0.1.5/tutorials/figures/variations_3.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/LICENSE` & `powfacpy-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/README.md` & `powfacpy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.4/PKG-INFO` & `powfacpy-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: powfacpy
-Version: 0.1.4
+Version: 0.1.5
 Summary: PowerFactory wrapper
 Project-URL: Homepage, https://github.com/FraunhIEE-UniKassel-PowSysStability/powfacpy
 Project-URL: Bug Tracker, https://github.com/FraunhIEE-UniKassel-PowSysStability/powfacpy/issues
 Author-email: Sciemon <simon.eberlein@gmx.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,17 +24,17 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: jsondiff>=2
-Requires-Dist: matplotlib>1
-Requires-Dist: pandas>1
+Requires-Python: >=3.8
+Requires-Dist: aenum>=3.1.15
+Requires-Dist: matplotlib>3.8.4
+Requires-Dist: pandas>2.2.2
 Description-Content-Type: text/markdown
 
 # powfacpy
 This package is a wrapper around the Python API of PowerFactory&copy; (power system simulation software by DIgSILENT) with improved syntax and functionality compared to the native API. Please have a look at the [docs](https://fraunhiee-unikassel-powsysstability.github.io/powfacpy/html/index.html) for further information. 
 
 This package is under active development and mainly maintained by Fraunhofer IEE. You are welcome to contribute or feel free to get in touch (contact: simon.eberlein@iee.fraunhofer.de).
```

