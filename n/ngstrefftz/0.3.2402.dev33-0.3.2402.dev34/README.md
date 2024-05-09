# Comparing `tmp/ngstrefftz-0.3.2402.dev33.tar.gz` & `tmp/ngstrefftz-0.3.2402.dev34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngstrefftz-0.3.2402.dev33.tar", last modified: Wed May  8 20:05:06 2024, max compression
+gzip compressed data, was "ngstrefftz-0.3.2402.dev34.tar", last modified: Thu May  9 00:42:34 2024, max compression
```

## Comparing `ngstrefftz-0.3.2402.dev33.tar` & `ngstrefftz-0.3.2402.dev34.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.780124 ngstrefftz-0.3.2402.dev33/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_linux_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/ngsolve_version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/build_in_docker.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/_static/breadcrumbs.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.788124 ngstrefftz-0.3.2402.dev33/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/_static/css/mytheme.css
--rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/contrib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/docu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/intro.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-adv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-helm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-poi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-stokes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-wave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/helmholtz.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/laplace.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/qtwave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/tunfitted.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/twave.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/notebooks/twavetents.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/docs/paper/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/codemeta.json
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.ps1
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.sh
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.784124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.792124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/euler2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dtent.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dvertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.796124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/horn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/BurgersMTP.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/INDEX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/StartPitching.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/
--rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/CausalityCond.png
--rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/dag.png
--rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/map.png
--rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/subtents.png
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.800124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.804124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/advection.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/burgers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/concurrentqueue.h
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/conservationlaw.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/euler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/maxwell.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/paralleldepend.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_conslaw.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/symbolic.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/wave.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.804124 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_burgers_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_causal_tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_conslaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tent_height_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tentlayers.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.808124 ngstrefftz-0.3.2402.dev33/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/airy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/condensedg.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/condensedg.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/diffopmapped.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/embtrefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/embtrefftz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/mesh1dtents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/mesh1dtents.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/monomialfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/monomialfespace.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 20:05:06.000000 ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/ngsttd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/planewavefe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/planewavefe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/python_trefftz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialintegrator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/specialintegrator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/trefftzfespace.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/trefftzfespace.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/twavetents.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/src/twavetents.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:05:06.812124 ngstrefftz-0.3.2402.dev33/test/
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/dg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/embt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/tents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-08 20:04:34.000000 ngstrefftz-0.3.2402.dev33/test/trefftz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.334652 ngstrefftz-0.3.2402.dev34/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_linux_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/ngsolve_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.334652 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/build_in_docker.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/_static/breadcrumbs.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/_static/css/mytheme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/docu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/intro.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-adv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-helm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-poi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-stokes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-wave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/helmholtz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/laplace.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/qtwave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/tunfitted.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/twave.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/notebooks/twavetents.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.338652 ngstrefftz-0.3.2402.dev34/docs/paper/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/codemeta.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.330652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d_periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/euler2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/maxwell3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.342652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dtent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dvertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/horn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26966 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/BurgersMTP.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/INDEX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    24974 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/StartPitching.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)    28475 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/CausalityCond.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57380 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/dag.png
+-rw-r--r--   0 runner    (1001) docker     (127)    91865 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/map.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70062 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/subtents.png
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.346652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.350652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/advection.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/burgers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   133375 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/concurrentqueue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/conservationlaw.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    15095 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/euler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/maxwell.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/paralleldepend.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11218 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_conslaw.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8659 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/symbolic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31227 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47172 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13765 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/wave.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.354652 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_burgers_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_causal_tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_conslaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tent_height_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-09 00:41:57.000000 ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tentlayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/airy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/condensedg.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/condensedg.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13580 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/diffopmapped.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26481 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/embtrefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/embtrefftz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/mesh1dtents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/mesh1dtents.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/monomialfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/monomialfespace.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 00:42:34.000000 ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/ngsttd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/planewavefe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12393 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/planewavefe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/python_trefftz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14965 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    60694 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialintegrator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/specialintegrator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    56525 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/trefftzfespace.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/trefftzfespace.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45126 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/twavetents.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8472 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/src/twavetents.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 00:42:34.358652 ngstrefftz-0.3.2402.dev34/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/dg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8739 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/embt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/tents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-05-09 00:41:56.000000 ngstrefftz-0.3.2402.dev34/test/trefftz.py
```

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev34/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/build_linux_test.sh` & `ngstrefftz-0.3.2402.dev34/.github/workflows/build_linux_test.sh`

 * *Files 14% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 $PYDIR/pip install numpy mkl==2023.* mkl-devel==2023.* 
 $PYDIR/pip install -r ./NGSTrefftz/.github/workflows/ngsolve_version.txt
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/opt/_internal/cpython-3.10.9/lib/
 
 echo "SHOW MKL"
 $PYDIR/pip show mkl
 
-cmake -DCMAKE_CXX_COMPILER=ngscxx -DNETGENDIR=$PYDIR/.. -DCMAKE_PREFIX_PATH=$PYDIR/..  -DPYTHON_EXECUTABLE=$PYDIR/python3 -DPYTHON_LIBRARY=$PYDIR/../lib -DPYTHON_INCLUDE_DIR=$PYDIR/../include -B ./NGSTrefftz/make -S ./NGSTrefftz/src/
+cmake -DCMAKE_CXX_COMPILER=ngscxx -DNETGENDIR=$PYDIR/.. -DCMAKE_PREFIX_PATH=$PYDIR/..  -DPYTHON_EXECUTABLE=$PYDIR/python3 -DPYTHON_LIBRARY=$PYDIR/../lib -DPYTHON_INCLUDE_DIR=$PYDIR/../include -DMKL_LIBRARY:PATH=$PYDIR/../lib/libmkl_rt.so.2 -B ./NGSTrefftz/make -S ./NGSTrefftz/src/
 make -C ./NGSTrefftz/make
 env CTEST_OUTPUT_ON_FAILURE=1 make -C ./NGSTrefftz/make test
 make -C ./NGSTrefftz/make install
```

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.ps1`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,36 @@
 #$env:PYDIR = (Join-Path (Get-Item .).FullName "venv_ngs\")
 #Get-ChildItem venv_ngs
 #Get-ChildItem venv_ngs\lib
 #Get-ChildItem venv_ngs\include
 #Get-ChildItem venv_ngs\scripts
 #Write-Host $env:LIB
 
+Set-Location ../..
+Get-ChildItem
+python.exe -m venv .\venv_ngs
+.\venv_ngs\scripts\Activate.ps1
+$env:PATH += Join-Path ";" (Get-Item .).FullName "venv_ngs\bin"
+Write-Host $env:PATH
 
-pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.* setuptools setuptools_scm
-pip3 install -r ngsolve_version.txt
-
+pip3 install scikit-build wheel numpy twine mkl-devel==2022.* mkl==2022.* setuptools==69.5.1 setuptools_scm==8.1.0
+pip3 install -r .github/workflows/ngsolve_version.txt
 
 #$env:PYDIR = "$env:Python3_ROOT_DIR"
 #$env:PATH += ";$env:pythonLibrary;$env:Python3_ROOT_DIR"
-$env:NGSolve_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\ngsolve\cmake"
-$env:Netgen_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\netgen\cmake"
+#$env:NGSolve_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\ngsolve\cmake"
+#$env:Netgen_DIR = "$env:Python3_ROOT_DIR\lib\site-packages\netgen\cmake"
 #$env:LIB = "$env:LIB;$env:Python3_ROOT_DIR\libs"
 #$env:LIBPATH = "$env:LIBPATH;$env:Python3_ROOT_DIR\libs"
 
 #Get-ChildItem $env:pythonLibrary
 #Get-ChildItem $env:Python3_ROOT_DIR
 #Get-ChildItem $env:Python3_ROOT_DIR\lib
 #Get-ChildItem $env:Python3_ROOT_DIR\libs
 #Get-ChildItem $env:Python3_ROOT_DIR\include
 #Get-ChildItem $env:Python3_ROOT_DIR\scripts
 #Get-ChildItem $env:Python3_ROOT_DIR\share
 #Get-ChildItem $env:Python3_ROOT_DIR\lib\site-packages
 #Get-ChildItem $env:Python3_ROOT_DIR\lib\site-packages\ngsolve
 
-Set-Location ../..
-Get-ChildItem
+
 python setup.py bdist_wheel -G"Visual Studio 16 2019" -d wheelhouse
```

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev34/.github/workflows/build_pip_mac.sh`

 * *Files 20% similar despite different names*

```diff
@@ -2,29 +2,34 @@
 set -e
 cd ../..
 rm -rf _skbuild dist venv_ngs
 
 export PYDIR=$Python3_ROOT_DIR/bin
 #export PYDIR=/Library/Frameworks/Python.framework/Versions/$1/bin
 
-$PYDIR/python3 --version
+#$PYDIR/python3 --version
 #$PYDIR/python3 -m venv venv_ngs
-#source venv_ngs/bin/activate
+#. venv_ngs/bin/activate
 
 export PATH=/Applications/CMake.app/Contents/bin:$PATH
 export NETGEN_Dir=$PYDIR/../lib/python$1/site-packages/netgen/cmake
 export NGSolve_Dir=$PYDIR/../lib/python$1/site-packages/ngsolve/cmake
 export CMAKE_PREFIX_PATH=$CMAKE_PREFIX_PATH:$NGSolve_Dir:$NETGEN_Dir
 #export PYDIR=/Library/Frameworks/Python.framework/Versions/$1/bin
 #$PYDIR/python3 -m venv ../venv_ngs
 #source ../venv_ngs/bin/activate
-$PYDIR/pip3 install scikit-build wheel setuptools setuptools_scm
+$PYDIR/pip3 install scikit-build wheel setuptools==69.5.1 setuptools_scm==8.1.0
 #$PYDIR/pip3 install -U pytest-check numpy wheel scikit-build mkl==2022.* mkl-devel==2022.* setuptools
 
 export CMAKE_OSX_ARCHITECTURES='arm64;x86_64'
 #export CMAKE_OSX_ARCHITECTURES='x86_64'
 $PYDIR/pip3 install -r ./.github/workflows/ngsolve_version.txt
+#export NETGEN_Dir=$PWD/venv_ngs/lib/make/netgen/
+#export NGSolve_Dir=$PWD/venv_ngs/lib/cmake/ngsolve/
+#export NETGEN_Dir=$PWD/venv_ngs/lib/python$1/site-packages/netgen/cmake
+#export NGSolve_Dir=$PWD/venv_ngs/lib/python$1/site-packages/ngsolve/cmake
+#export CMAKE_PREFIX_PATH=$CMAKE_PREFIX_PATH:$NGSolve_Dir:$NETGEN_Dir
 
 #$PYDIR/pip3 wheel .
 $PYDIR/python3 setup.py bdist_wheel --plat-name macosx-10.15-universal2 -d wheelhouse
 
 cat src/ngstrefftz.egg-info/SOURCES.txt
```

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev34/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/Dockerfile` & `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/build_in_docker.sh` & `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/build_in_docker.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/merge.py` & `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/merge.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/.github/workflows/pyodide/requirements.txt` & `ngstrefftz-0.3.2402.dev34/.github/workflows/pyodide/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/CONTRIBUTING.md` & `ngstrefftz-0.3.2402.dev34/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/Dockerfile` & `ngstrefftz-0.3.2402.dev34/Dockerfile`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/LICENSE` & `ngstrefftz-0.3.2402.dev34/LICENSE`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/PKG-INFO` & `ngstrefftz-0.3.2402.dev34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev33
+Version: 0.3.2402.dev34
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
```

### Comparing `ngstrefftz-0.3.2402.dev33/README.md` & `ngstrefftz-0.3.2402.dev34/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/conf.py` & `ngstrefftz-0.3.2402.dev34/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/docu.rst` & `ngstrefftz-0.3.2402.dev34/docs/docu.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/index.rst` & `ngstrefftz-0.3.2402.dev34/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/intro.rst` & `ngstrefftz-0.3.2402.dev34/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-adv.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-adv.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-helm.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-helm.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-poi.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-poi.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-stokes.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-stokes.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz-wave.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz-wave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/embTrefftz.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/embTrefftz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/helmholtz.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/helmholtz.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/index.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/index.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/laplace.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/laplace.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/qtwave.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/qtwave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/tunfitted.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/tunfitted.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/twave.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/twave.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/notebooks/twavetents.ipynb` & `ngstrefftz-0.3.2402.dev34/docs/notebooks/twavetents.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/paper/codemeta.json` & `ngstrefftz-0.3.2402.dev34/docs/paper/codemeta.json`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/paper/paper.bib` & `ngstrefftz-0.3.2402.dev34/docs/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/docs/paper/paper.md` & `ngstrefftz-0.3.2402.dev34/docs/paper/paper.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build.yml` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.ps1` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.ps1`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip.sh` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/build_pip_mac.sh`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/.github/workflows/fix_auditwheel_policy.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/README.md` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/README.md`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/Advection_Periodic_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/advection/advection2d_periodic.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/advection/advection2d_periodic.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/Burgers_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers1d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers1d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/burgers/burgers2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/burgers/burgers2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/Euler_Clipping.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/euler2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/euler2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/euler/mach3_windtunnel.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/maxwell/maxwell3d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/maxwell/maxwell3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_advection2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_burgers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_euler.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/symbolic_wave1d_interface.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/symbolic/wave_penetrable_cylinder.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dtent.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dtent.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/tents/draw3dvertex.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/tents/draw3dvertex.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/horn.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/horn.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave2d_timedepbc.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/demo/wave/wave3d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/demo/wave/wave3d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/BurgersMTP.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/BurgersMTP.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/INDEX.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/INDEX.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/StartPitching.ipynb` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/StartPitching.ipynb`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/conf.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/CausalityCond.png` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/CausalityCond.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/dag.png` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/dag.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/map.png` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/map.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/figs/subtents.png` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/figs/subtents.png`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/index.rst` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/docs/requirements.txt` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/conslaw/__init__.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/conslaw/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/py/utils/_drawtents2d.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/py/utils/_drawtents2d.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/setup.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/setup.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/CMakeLists.txt` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/advection.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/advection.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/burgers.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/burgers.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/concurrentqueue.h` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/concurrentqueue.h`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/conservationlaw.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/conservationlaw.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/euler.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/euler.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/maxwell.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/maxwell.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/paralleldepend.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/paralleldepend.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_conslaw.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_conslaw.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/python_tents.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/python_tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/symbolic.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/symbolic.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tconservationlaw_tp_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tents.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/tentsolver_impl.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/tentsolver_impl.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/vis3d.hpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/vis3d.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/src/wave.cpp` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/src/wave.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_burgers_2D.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_burgers_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_causal_tents.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_causal_tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_conslaw.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_conslaw.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tent_height_2D.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tent_height_2D.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/external_dependencies/ngstents/tests/test_tentlayers.py` & `ngstrefftz-0.3.2402.dev34/external_dependencies/ngstents/tests/test_tentlayers.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/setup.py` & `ngstrefftz-0.3.2402.dev34/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,37 +17,31 @@
     # from distutils.sysconfig import get_python_lib
     # py_install_dir = get_python_lib(1,0,'').replace('\\','/')
     # root_dir = os.path.abspath(os.path.join(netgen.__file__, '../'*(len(py_install_dir.split('/'))+2)))
 # except:
 root_dir = sys.prefix
 print(f'root_dir: {root_dir}')
 if 'darwin' in sys.platform:
-    _cmake_args += [
-        '-DBUILD_STUB_FILES=ON',
-    ]
+    _cmake_args += [ ]
 elif 'linux' in sys.platform:
     _cmake_args += [
         '-DUSE_MKL:BOOL=ON',
         f'-DMKL_ROOT:PATH={root_dir}',
         f'-DMKL_LIBRARY:PATH={root_dir}/lib/libmkl_rt.so.2',
         f'-DMKL_INCLUDE_DIR:PATH={root_dir}/include',
-        '-DUSE_CUDA=ON',
-        '-DCMAKE_CUDA_ARCHITECTURES=all',
-        '-DBUILD_STUB_FILES=ON',
     ]
     install_requires.append('mkl')
     packages = []
 elif 'win' in sys.platform:
     _cmake_args += [
         '-DUSE_MKL:BOOL=ON',
         f'-DMKL_ROOT:PATH={root_dir}',
         f'-DMKL_LIBRARY:PATH={root_dir}/Library/lib/mkl_rt.lib',
         f'-DMKL_INCLUDE_DIR:PATH={root_dir}/Library/include',
         f'-DNGSOLVE_INSTALL_DIR_TCL:PATH=Scripts',
-        '-DBUILD_STUB_FILES=OFF',
     ]
     install_requires.append('mkl')
 
 
 setup(
     name='ngstrefftz',
     version=version,
```

### Comparing `ngstrefftz-0.3.2402.dev33/src/CMakeLists.txt` & `ngstrefftz-0.3.2402.dev34/src/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,28 @@
 set(Netgen_DIR "" CACHE PATH "Path to directory containing NetgenConfig.cmake")
 set(NGSolve_DIR "" CACHE PATH "Path to directory containing NGSolveConfig.cmake")
 execute_process(COMMAND ${Python3_EXECUTABLE} -m netgen.config OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE Netgen_DIR)
 execute_process(COMMAND ${Python3_EXECUTABLE} -m ngsolve.config OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NGSolve_DIR)
 find_package(NGSolve CONFIG REQUIRED)
 
 ### check if CMAKE_INSTALL_PREFIX is set by user, if not install in NGSolve python dir
+
+#set(INSTDIR_FROM_NGSOLVE ${CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT} CACHE BOOL "Try to get install dir from NGSolve")
 if(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
     execute_process(COMMAND ${Python3_EXECUTABLE} -m site --user-site OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE install_dir RESULT_VARIABLE ret)
     if (NOT ret EQUAL 0)
         # user site directory is disabled (are we in a virtual environment?)
         set(install_dir ${Python3_SITEARCH})
     endif()
-    message("The python module ${module_name} will be installed to: ${install_dir}")
+    message("Install dir from NGSolve: ${install_dir}")
     set(CMAKE_INSTALL_PREFIX ${install_dir} CACHE PATH "Install dir" FORCE)
 else(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
-    set(PY_INSTALL_DIR ${NGSOLVE_INSTALL_DIR_PYTHON} CACHE STRING "subdir of install dir for python modules")
+    #set(PY_INSTALL_DIR ${NGSOLVE_INSTALL_DIR_PYTHON} CACHE STRING "subdir of install dir for python modules")
+    execute_process(COMMAND ${Python3_EXECUTABLE} -c "import os.path, sysconfig;print(os.path.relpath(sysconfig.get_path('platlib'), sysconfig.get_path('data')))" OUTPUT_VARIABLE PY_INSTALL_DIR OUTPUT_STRIP_TRAILING_WHITESPACE)
+    message("python packages install dir: ${PY_INSTALL_DIR}")
 endif(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
 set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR} CACHE PATH "build dir")
 
 ### install message
 set(NGSTREFFTZ_USE_MKL ${NGSOLVE_USE_MKL} CACHE BOOL "Try to use mkl")
 set(NGSTREFFTZ_USE_LAPACK ${NGSOLVE_USE_LAPACK} CACHE BOOL "Try to use lapack from ngsolve")
 set(INSTALL_TENTS ON CACHE BOOL "Install ngstents")
@@ -124,56 +128,72 @@
     set(MKL_MULTI_THREADED ON CACHE BOOL "Use threaded MKL libs")
     if(NOT MKL_MULTI_THREADED)
       set(MKL_THREADING sequential)
     endif()
     set(MKL_STATIC OFF CACHE BOOL "Link static MKL")
     set(MKL_SDL ON CACHE BOOL "Link single dynamic MKL lib")
     set(MKL_ARCH "intel64")
+    message("MKL_ARCH=${MKL_ARCH}")
     if(NOT MKL_LINK)
       if(MKL_STATIC)
         set(MKL_LINK static)
       elseif(MKL_SDL AND NOT USE_MPI)
         set(MKL_LINK sdl)
       else()
         set(MKL_LINK dynamic)
       endif()
     endif()
     find_package(MKL) # HINTS ${MKL_ROOT} ${CMAKE_INSTALL_PREFIX}/../../cmake/mkl ${Python3_ROOT_DIR}/lib/cmake/mkl)
-    if(APPLE OR WIN32)
-      set(MKL_RT_NAME mkl_rt.2)
-    else()
-      set(MKL_RT_NAME libmkl_rt.so.2)
-    endif()
-    find_library(MKLRT ${MKL_RT_NAME} HINTS ${MKL_ROOT}/lib)
-    message("MKL minimal: ${MKL_MINIMAL_LIBRARIES}")
-    message("MKLRT: ${MKLRT}")
-
-    #if(NOT MKL_FOUND OR NOT MKLRT)
-    if(NOT MKL_MINIMAL_LIBRARIES)
-        message("${Red}MKL not found, switching off NGSTREFFTZ_USE_LAPACK!${ColourReset}")
-        set(NGSTREFFTZ_USE_LAPACK OFF)
-    else()
-        if(WIN32)
-            set(LAPACK_LIBRARIES "${MKL_MINIMAL_LIBRARIES}")
-        else()
-            set(LAPACK_LIBRARIES "${MKLRT}")
-        endif()
+    #message("MKL minimal: ${MKL_MINIMAL_LIBRARIES}")
+    #message("MKL libraries: ${MKL_LIBRARIES}")
+    #message("MKL link flags: ${MKL_LINK_FLAGS}")
+
+    #if(MKL_FOUND)
+    if(MKL_MINIMAL_LIBRARIES)
+        set(LAPACK_LIBRARIES "${MKL_LIBRARIES}")
         message("Setting LAPACK_LIBRARIES=${LAPACK_LIBRARIES}")
         target_include_directories(_trefftz PRIVATE "${MKL_INCLUDE_DIRS}")
     endif()
+    if(MKL_LIBRARY)
+        message("MKL_LIBRARY=${MKL_LIBRARY}")
+        #if(WIN32)
+            #set(LAPACK_LIBRARIES "${MKL_MINIMAL_LIBRARIES}")
+        #else()
+            #set(LAPACK_LIBRARIES "${MKL_LIBRARIES}")
+        #endif()
+    #if(NOT MKL_LIBRARIES)
+        #if(APPLE OR WIN32)
+          #set(MKL_RT_NAME mkl_rt.2)
+        #else()
+          #set(MKL_RT_NAME libmkl_rt.so.2)
+        #endif()
+        get_filename_component(MKL_RT_NAME ${MKL_LIBRARY} NAME)
+        message("MKL_RT_NAME=${MKL_RT_NAME}")
+        find_library(MKLRT ${MKL_RT_NAME} HINTS ${MKL_ROOT}/lib ${MKL_LIBRARY})
+        message("MKLRT=${MKLRT}")
+        if(MKLRT)
+            set(LAPACK_LIBRARIES ${MKLRT})
+            message("MKLRT setting LAPACK_LIBRARIES=${LAPACK_LIBRARIES}")
+        endif()
+    #else()
+        #message("${Red}MKL not found, switching off NGSTREFFTZ_USE_LAPACK!${ColourReset}")
+        #set(NGSTREFFTZ_USE_LAPACK OFF)
+    endif()
 endif (NGSTREFFTZ_USE_MKL)
 if(NGSTREFFTZ_USE_LAPACK AND NOT LAPACK_LIBRARIES)
     find_package(LAPACK)
-endif(NGSTREFFTZ_USE_LAPACK)
+endif(NGSTREFFTZ_USE_LAPACK AND NOT LAPACK_LIBRARIES)
 if(LAPACK_LIBRARIES)
     #target_link_libraries(_trefftz PRIVATE $<BUILD_INTERFACE:ngs_lapack>)
     message("Linking with LAPACK_LIBRARIES=${LAPACK_LIBRARIES}")
     target_link_libraries(_trefftz PRIVATE ${LAPACK_LIBRARIES})
     target_compile_definitions(_trefftz PRIVATE NGSTREFFTZ_USE_LAPACK)
-endif()
+else(LAPACK_LIBRARIES)
+    message("${Red}LAPACK not found, restricted usage${ColourReset}")
+endif(LAPACK_LIBRARIES)
 
 ### install
 set_target_properties(_trefftz PROPERTIES LIBRARY_OUTPUT_DIRECTORY "${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/ngstrefftz")
 file(COPY ${CMAKE_SOURCE_DIR}/__init__.py DESTINATION ${CMAKE_LIBRARY_OUTPUT_DIRECTORY}/ngstrefftz)
 install(TARGETS _trefftz DESTINATION ${CMAKE_INSTALL_PREFIX}/${PY_INSTALL_DIR}/ngstrefftz)
 install(FILES __init__.py DESTINATION ${CMAKE_INSTALL_PREFIX}/${PY_INSTALL_DIR}/ngstrefftz) #COMPONENT ngstrefftz
```

### Comparing `ngstrefftz-0.3.2402.dev33/src/__init__.py` & `ngstrefftz-0.3.2402.dev34/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/airy.cpp` & `ngstrefftz-0.3.2402.dev34/src/airy.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/condensedg.cpp` & `ngstrefftz-0.3.2402.dev34/src/condensedg.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/condensedg.hpp` & `ngstrefftz-0.3.2402.dev34/src/condensedg.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/diffopmapped.hpp` & `ngstrefftz-0.3.2402.dev34/src/diffopmapped.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/embtrefftz.cpp` & `ngstrefftz-0.3.2402.dev34/src/embtrefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/embtrefftz.hpp` & `ngstrefftz-0.3.2402.dev34/src/embtrefftz.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/mesh1dtents.cpp` & `ngstrefftz-0.3.2402.dev34/src/mesh1dtents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/monomialfespace.cpp` & `ngstrefftz-0.3.2402.dev34/src/monomialfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/monomialfespace.hpp` & `ngstrefftz-0.3.2402.dev34/src/monomialfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/PKG-INFO` & `ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngstrefftz
-Version: 0.3.2402.dev33
+Version: 0.3.2402.dev34
 Summary: NGSTrefftz is an add-on to NGSolve for Trefftz methods.
 Home-page: https://github.com/PaulSt/ngstrefftz
 Author: Paul Stocker
 Author-email: p.stocker@math.uni-goettingen.de
 License: LGPL2.1
 License-File: LICENSE
 Requires-Dist: ngsolve>=6.2.2401.post24.dev0
```

### Comparing `ngstrefftz-0.3.2402.dev33/src/ngstrefftz.egg-info/SOURCES.txt` & `ngstrefftz-0.3.2402.dev34/src/ngstrefftz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/planewavefe.cpp` & `ngstrefftz-0.3.2402.dev34/src/planewavefe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/planewavefe.hpp` & `ngstrefftz-0.3.2402.dev34/src/planewavefe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/python_trefftz.cpp` & `ngstrefftz-0.3.2402.dev34/src/python_trefftz.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.cpp` & `ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/scalarmappedfe.hpp` & `ngstrefftz-0.3.2402.dev34/src/scalarmappedfe.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.cpp` & `ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/specialcoefficientfunction.hpp` & `ngstrefftz-0.3.2402.dev34/src/specialcoefficientfunction.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/specialintegrator.cpp` & `ngstrefftz-0.3.2402.dev34/src/specialintegrator.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/specialintegrator.hpp` & `ngstrefftz-0.3.2402.dev34/src/specialintegrator.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/trefftzfespace.cpp` & `ngstrefftz-0.3.2402.dev34/src/trefftzfespace.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/trefftzfespace.hpp` & `ngstrefftz-0.3.2402.dev34/src/trefftzfespace.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/twavetents.cpp` & `ngstrefftz-0.3.2402.dev34/src/twavetents.cpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/src/twavetents.hpp` & `ngstrefftz-0.3.2402.dev34/src/twavetents.hpp`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/test/dg.py` & `ngstrefftz-0.3.2402.dev34/test/dg.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/test/embt.py` & `ngstrefftz-0.3.2402.dev34/test/embt.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/test/tents.py` & `ngstrefftz-0.3.2402.dev34/test/tents.py`

 * *Files identical despite different names*

### Comparing `ngstrefftz-0.3.2402.dev33/test/trefftz.py` & `ngstrefftz-0.3.2402.dev34/test/trefftz.py`

 * *Files identical despite different names*

