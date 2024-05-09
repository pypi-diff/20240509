# Comparing `tmp/fcio-0.3.0.tar.gz` & `tmp/fcio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcio-0.3.0.tar", last modified: Tue Apr 30 11:54:00 2024, max compression
+gzip compressed data, was "fcio-0.4.0.tar", last modified: Thu May  9 11:33:57 2024, max compression
```

## Comparing `fcio-0.3.0.tar` & `fcio-0.4.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0     1507 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/gh-pages-static.yml
--rw-r--r--   0        0        0     1720 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     3178 2024-04-30 11:50:07.000000 fcio-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0       51 2024-04-30 11:50:07.000000 fcio-0.3.0/.gitignore
--rw-r--r--   0        0        0      761 2024-04-30 11:50:07.000000 fcio-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    16726 2024-04-30 11:50:07.000000 fcio-0.3.0/LICENSE
--rw-r--r--   0        0        0      628 2024-04-30 11:50:07.000000 fcio-0.3.0/Makefile
--rw-r--r--   0        0        0     1961 2024-04-30 11:50:07.000000 fcio-0.3.0/README.md
--rw-r--r--   0        0        0      638 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/Makefile
--rw-r--r--   0        0        0      804 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/make.bat
--rw-r--r--   0        0        0       29 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0     1729 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/conf.py
--rw-r--r--   0        0        0      238 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/fcio.rst
--rw-r--r--   0        0        0      223 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/index.rst
--rw-r--r--   0        0        0       45 2024-04-30 11:50:07.000000 fcio-0.3.0/docs/source/readme.rst
--rw-r--r--   0        0        0     1200 2024-04-30 11:50:07.000000 fcio-0.3.0/meson.build
--rw-r--r--   0        0        0     2178 2024-04-30 11:50:07.000000 fcio-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      714 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/__init__.py
--rw-r--r--   0        0        0       92 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cmds/__init__.py
--rw-r--r--   0        0        0     3071 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cmds/cmds.py
--rw-r--r--   0        0        0     1943 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/config.py
--rw-r--r--   0        0        0     8387 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/event.py
--rw-r--r--   0        0        0     4344 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/fcio_cppyy.py
--rw-r--r--   0        0        0     2957 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cppyy_fcio/status.py
--rw-r--r--   0        0        0     4591 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cfcio.pxd
--rw-r--r--   0        0        0    10767 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio.pyx
--rw-r--r--   0        0        0     3742 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_config.pyx
--rw-r--r--   0        0        0     5827 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event.pyx
--rw-r--r--   0        0        0     9108 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
--rw-r--r--   0        0        0     4896 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_recevent.pyx
--rw-r--r--   0        0        0     6334 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx
--rw-r--r--   0        0        0     6425 2024-04-30 11:50:07.000000 fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_status.pyx
--rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/.drone.star
--rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/.gitignore
--rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/LICENSE
--rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/Makefile
--rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/README.md
--rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/examples/bufio_benchmark.c
--rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/examples/meson.build
--rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/meson.build
--rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/bufio.c
--rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/bufio.h
--rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/src/meson.build
--rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
--rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow.c
--rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow_chunk.c
--rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_lockedfile.c
--rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_tcp_connect.c
--rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
--rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
--rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/meson.build
--rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.3.0/subprojects/bufio/tests/test.h
--rw-r--r--   0        0        0      110 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/bufio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/.drone.star
--rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/LICENSE
--rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/Makefile
--rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/README.md
--rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/meson.build
--rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/fcio.c
--rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/fcio.h
--rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/meson.build
--rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/time_utils.c
--rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/src/time_utils.h
--rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.3.0/subprojects/fcio/subprojects/tmio.wrap
--rw-r--r--   0        0        0      109 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/fcio.wrap
--rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/.drone.star
--rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/.gitignore
--rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/LICENSE
--rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/Makefile
--rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/README.md
--rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/meson.build
--rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/timer.c
--rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/timer.h
--rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark.c
--rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
--rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
--rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh
--rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_simple.c
--rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh
--rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_example_reader.c
--rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_example_writer.c
--rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/examples/tmio_sink.c
--rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/meson.build
--rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/meson.build
--rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/tmio.c
--rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/src/tmio.h
--rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.3.0/subprojects/tmio/subprojects/bufio.wrap
--rw-r--r--   0        0        0      108 2024-04-30 11:50:07.000000 fcio-0.3.0/subprojects/tmio.wrap
--rwxr-xr-x   0        0        0      526 2024-04-30 11:50:07.000000 fcio-0.3.0/tests/test_platform.py
--rwxr-xr-x   0        0        0      249 2024-04-30 11:50:07.000000 fcio-0.3.0/tools/create-pxd.sh
--rwxr-xr-x   0        0        0     1374 2024-04-30 11:50:07.000000 fcio-0.3.0/tools/version_util.py
--rw-r--r--   0        0        0     3381 2024-04-30 11:54:00.447475 fcio-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-05-09 11:30:10.000000 fcio-0.4.0/.github/workflows/gh-pages-static.yml
+-rw-r--r--   0        0        0     1720 2024-05-09 11:30:10.000000 fcio-0.4.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3178 2024-05-09 11:30:10.000000 fcio-0.4.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0       51 2024-05-09 11:30:10.000000 fcio-0.4.0/.gitignore
+-rw-r--r--   0        0        0      761 2024-05-09 11:30:10.000000 fcio-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    16726 2024-05-09 11:30:10.000000 fcio-0.4.0/LICENSE
+-rw-r--r--   0        0        0      628 2024-05-09 11:30:10.000000 fcio-0.4.0/Makefile
+-rw-r--r--   0        0        0     1961 2024-05-09 11:30:10.000000 fcio-0.4.0/README.md
+-rw-r--r--   0        0        0      638 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/make.bat
+-rw-r--r--   0        0        0       29 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1729 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/source/conf.py
+-rw-r--r--   0        0        0      238 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/source/fcio.rst
+-rw-r--r--   0        0        0      223 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/source/index.rst
+-rw-r--r--   0        0        0       45 2024-05-09 11:30:10.000000 fcio-0.4.0/docs/source/readme.rst
+-rw-r--r--   0        0        0     1200 2024-05-09 11:30:10.000000 fcio-0.4.0/meson.build
+-rw-r--r--   0        0        0     2178 2024-05-09 11:30:10.000000 fcio-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cmds/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cmds/cmds.py
+-rw-r--r--   0        0        0     1943 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cppyy_fcio/config.py
+-rw-r--r--   0        0        0     8387 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cppyy_fcio/event.py
+-rw-r--r--   0        0        0     4344 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cppyy_fcio/fcio_cppyy.py
+-rw-r--r--   0        0        0     2957 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cppyy_fcio/status.py
+-rw-r--r--   0        0        0     4591 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cfcio.pxd
+-rw-r--r--   0        0        0     3646 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_dead_interval_tracker.pyx
+-rw-r--r--   0        0        0    10806 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio.pyx
+-rw-r--r--   0        0        0     3742 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_config.pyx
+-rw-r--r--   0        0        0     5827 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_event.pyx
+-rw-r--r--   0        0        0     8541 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx
+-rw-r--r--   0        0        0     4896 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_recevent.pyx
+-rw-r--r--   0        0        0     7503 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_recevent_ext.pyx
+-rw-r--r--   0        0        0     6425 2024-05-09 11:30:10.000000 fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_status.pyx
+-rw-r--r--   0        0        0     1272 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/.drone.star
+-rw-r--r--   0        0        0       50 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/LICENSE
+-rw-r--r--   0        0        0      408 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/Makefile
+-rw-r--r--   0        0        0      427 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/README.md
+-rw-r--r--   0        0        0     2365 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/examples/bufio_benchmark.c
+-rw-r--r--   0        0        0      124 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/examples/meson.build
+-rw-r--r--   0        0        0      523 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/meson.build
+-rw-r--r--   0        0        0    45364 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/src/bufio.c
+-rw-r--r--   0        0        0     3273 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/src/bufio.h
+-rw-r--r--   0        0        0      161 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/src/meson.build
+-rw-r--r--   0        0        0      927 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c
+-rw-r--r--   0        0        0     1189 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_follow.c
+-rw-r--r--   0        0        0     1875 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_follow_chunk.c
+-rw-r--r--   0        0        0     1902 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_lockedfile.c
+-rw-r--r--   0        0        0      887 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_tcp_connect.c
+-rw-r--r--   0        0        0     1331 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c
+-rw-r--r--   0        0        0     1232 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c
+-rw-r--r--   0        0        0     1739 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/meson.build
+-rw-r--r--   0        0        0      479 2024-02-09 15:22:16.000000 fcio-0.4.0/subprojects/bufio/tests/test.h
+-rw-r--r--   0        0        0      110 2024-05-09 11:30:10.000000 fcio-0.4.0/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/.drone.star
+-rw-r--r--   0        0        0       18 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/LICENSE
+-rw-r--r--   0        0        0      375 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/Makefile
+-rw-r--r--   0        0        0      715 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/README.md
+-rw-r--r--   0        0        0      549 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/meson.build
+-rw-r--r--   0        0        0    57331 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/src/fcio.c
+-rw-r--r--   0        0        0    13863 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/src/fcio.h
+-rw-r--r--   0        0        0      199 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/src/meson.build
+-rw-r--r--   0        0        0     6190 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/src/time_utils.c
+-rw-r--r--   0        0        0      778 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/src/time_utils.h
+-rw-r--r--   0        0        0      104 2024-03-10 11:25:29.000000 fcio-0.4.0/subprojects/fcio/subprojects/tmio.wrap
+-rw-r--r--   0        0        0      109 2024-05-09 11:30:10.000000 fcio-0.4.0/subprojects/fcio.wrap
+-rw-r--r--   0        0        0      965 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/.drone.star
+-rw-r--r--   0        0        0       44 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/.gitignore
+-rw-r--r--   0        0        0    16726 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/LICENSE
+-rw-r--r--   0        0        0      408 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/Makefile
+-rw-r--r--   0        0        0     2650 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/README.md
+-rw-r--r--   0        0        0      669 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/meson.build
+-rw-r--r--   0        0        0     5929 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/timer.c
+-rw-r--r--   0        0        0      637 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/timer.h
+-rw-r--r--   0        0        0    10493 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark.c
+-rwxr-xr-x   0        0        0      572 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh
+-rwxr-xr-x   0        0        0      575 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh
+-rwxr-xr-x   0        0        0      539 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh
+-rw-r--r--   0        0        0     2389 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_simple.c
+-rwxr-xr-x   0        0        0      926 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh
+-rw-r--r--   0        0        0     1620 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_example_reader.c
+-rw-r--r--   0        0        0     1822 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_example_writer.c
+-rw-r--r--   0        0        0     4720 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/examples/tmio_sink.c
+-rw-r--r--   0        0        0      549 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/meson.build
+-rw-r--r--   0        0        0      182 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/src/meson.build
+-rw-r--r--   0        0        0    33908 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/src/tmio.c
+-rw-r--r--   0        0        0     3723 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/src/tmio.h
+-rw-r--r--   0        0        0      106 2024-03-10 11:24:50.000000 fcio-0.4.0/subprojects/tmio/subprojects/bufio.wrap
+-rw-r--r--   0        0        0      108 2024-05-09 11:30:10.000000 fcio-0.4.0/subprojects/tmio.wrap
+-rwxr-xr-x   0        0        0      526 2024-05-09 11:30:10.000000 fcio-0.4.0/tests/test_platform.py
+-rwxr-xr-x   0        0        0      249 2024-05-09 11:30:10.000000 fcio-0.4.0/tools/create-pxd.sh
+-rwxr-xr-x   0        0        0     1374 2024-05-09 11:30:10.000000 fcio-0.4.0/tools/version_util.py
+-rw-r--r--   0        0        0     3381 2024-05-09 11:33:57.684981 fcio-0.4.0/PKG-INFO
```

### Comparing `fcio-0.3.0/.github/workflows/gh-pages-static.yml` & `fcio-0.4.0/.github/workflows/gh-pages-static.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/.github/workflows/main.yml` & `fcio-0.4.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/.github/workflows/publish.yml` & `fcio-0.4.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/CHANGELOG.md` & `fcio-0.4.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/LICENSE` & `fcio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/Makefile` & `fcio-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/README.md` & `fcio-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/docs/Makefile` & `fcio-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/docs/make.bat` & `fcio-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/docs/source/conf.py` & `fcio-0.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/meson.build` & `fcio-0.4.0/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/pyproject.toml` & `fcio-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/__init__.py` & `fcio-0.4.0/src/fcio/__init__.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cmds/cmds.py` & `fcio-0.4.0/src/fcio/cmds/cmds.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cppyy_fcio/config.py` & `fcio-0.4.0/src/fcio/cppyy_fcio/config.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cppyy_fcio/event.py` & `fcio-0.4.0/src/fcio/cppyy_fcio/event.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cppyy_fcio/fcio_cppyy.py` & `fcio-0.4.0/src/fcio/cppyy_fcio/fcio_cppyy.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cppyy_fcio/status.py` & `fcio-0.4.0/src/fcio/cppyy_fcio/status.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cfcio.pxd` & `fcio-0.4.0/src/fcio/cy_fcio/cfcio.pxd`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 cimport numpy
 import tempfile, os, subprocess
 
 include "cy_fcio_config.pyx"
 include "cy_fcio_event.pyx"
 include "cy_fcio_recevent.pyx"
 include "cy_fcio_status.pyx"
+include "cy_dead_interval_tracker.pyx"
 include "cy_fcio_event_ext.pyx"
 include "cy_fcio_recevent_ext.pyx"
 
 class CyFCIOTag:
   """
   A wrapper class for the fcio tag enum.
   Provides supported tags as attributes.
```

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_config.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_config.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_event.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_event_ext.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,177 @@
 cimport numpy
 import numpy
 
 import sys
 
-import numbers
-
 cdef class CyEventExt(CyEvent):
   """
   Class internal to the fcio library. Do not allocate directly, must be created by using `fcio_open` or 
   FCIO.open().
   Exposes the fcio_event struct fields from the fcio.c library.
   All fields are exposes as numpy scalars or arrays with their corresponsing datatype and size.
 
   Additionally CyEventExt offers some extension to the basic CyEvent attributes. These represent either
   convenient names values in some field, or offer some required pre-calculation.
 
   All CyEvent attributes are still available.
   """
-  cdef numpy.int32_t _wait_for_first_event
-
   cdef numpy.ndarray _tracemap
   cdef numpy.ndarray _card_addresses
   cdef numpy.ndarray _card_channels
+
+  cdef int _num_channels_per_card
   
   cdef numpy.int64_t _utc_unix_ns
   cdef numpy.float64_t _utc_unix
   
-  cdef numpy.int64_t _run_time_ns
-  cdef numpy.float64_t _run_time
+  cdef numpy.int64_t _fpga_time_ns
 
   cdef numpy.int32_t _allowed_gps_error_ns
   
-  cdef numpy.int64_t _start_time_ns
-  cdef numpy.ndarray _dead_time_ns
+  cdef numpy.ndarray _start_time_ns
+  cdef numpy.ndarray _cur_dead_time_ns
   cdef numpy.ndarray _total_dead_time_ns
-  cdef int _current_dead_time_end_pps
-  cdef int _current_dead_time_end_ticks
+
+  cdef DeadIntervalBuffer _dead_interval_buffer
 
   def __cinit__(self, fcio : CyFCIO):
 
+    self._dead_interval_buffer = DeadIntervalBuffer()
+
     cdef unsigned int[::1] tracemap_view = self.config_ptr.tracemap
     self._tracemap = numpy.ndarray(shape=(self.maxtraces,), dtype=numpy.uint32, offset=0, buffer=tracemap_view)
 
     self._card_addresses = self._tracemap >> 16 # upper 16bit
     self._card_channels = self._tracemap % (1 << 16) # lower 16bit
 
-    self._dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
+    self._start_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
+    self._start_time_ns[:] = -1
+
+    self._cur_dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
     self._total_dead_time_ns = numpy.zeros(shape=(self.config_ptr.adcs,),dtype=numpy.int64)
 
+    if self.config_ptr.adcbits == 12:
+      self._num_channels_per_card = 24
+    elif self.config_ptr.adcbits == 16:
+      self._num_channels_per_card = 6
+
     self._allowed_gps_error_ns = self.config_ptr.gps
-    self._wait_for_first_event = True
-    self._start_time_ns = 0
 
   cdef update(self):
-    cdef numpy.int64_t _event_deadtime
-
-    if self._wait_for_first_event:
-      self._start_time_ns = self.event_ptr.deadregion[2] * 1000000000L + self.event_ptr.deadregion[3] * 4
-      self._wait_for_first_event = False
-    else:
-      # determine if we have a new dead region end and update the counters
-      if self._current_dead_time_end_pps == self.event_ptr.deadregion[2] and self._current_dead_time_end_ticks == self.event_ptr.deadregion[3]:
-        self._dead_time_ns[:] = 0
-      else:
-        _event_deadtime = (self.event_ptr.deadregion[2]-self.event_ptr.deadregion[0]) * 1000000000L + (self.event_ptr.deadregion[3]-self.event_ptr.deadregion[1]) * 4
-        self._dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] = _event_deadtime
-        self._total_dead_time_ns[self.event_ptr.deadregion[5] : self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]] += _event_deadtime
-    
-    cdef expected_max_ticks = 249999999
-    
-    cdef numpy.int64_t _current_clock_offset
-
-    _current_clock_offset = abs(self.timestamp[3] - expected_max_ticks) * 4  
     
-    if _current_clock_offset > self._allowed_gps_error_ns:
-      print(f"WARNING fcio: max_ticks of last pps cycle {self.timestamp[3]} with { _current_clock_offset } > {self._allowed_gps_error_ns}",file=sys.stderr)
+    ## calculate timestamps in nanoseconds and update float properties
 
-    cdef numpy.int64_t nanoseconds_since_daq_reset
-    # store the current clock cycle information temporarily
-    nanoseconds_since_daq_reset = (1000000000L * self.timestamp[1] + 4 * self.timestamp[2])
-
-    # update relative time information, correct for time until the trigger was enabled in the system
-    self._run_time_ns = nanoseconds_since_daq_reset - self._start_time_ns
-    self._run_time = self._run_time_ns / 1000000000L
+    # update current pps/clk counters
+    cdef long _daq_synchronized_timestamp_ns = (1000000000L * self.timestamp[1] + 4 * self.timestamp[2])
+    self._fpga_time_ns = _daq_synchronized_timestamp_ns
 
     # update absolute time information
     if self.config_ptr.gps != 0:
-      self._utc_unix_ns = nanoseconds_since_daq_reset + self.timeoffset[2] * 1000000000L
+      # we have external clock (likely from a timeserver or gps clock)
+      self._utc_unix_ns = _daq_synchronized_timestamp_ns + self.timeoffset[2] * 1000000000L
     else:
-      self._utc_unix_ns = nanoseconds_since_daq_reset + 1000000000L * self.timeoffset[0] + 1000 * self.timeoffset[1]
+      # synchronization via server clock (likely from NTP server)
+      self._utc_unix_ns = _daq_synchronized_timestamp_ns + 1000000000L * self.timeoffset[0] + 1000 * self.timeoffset[1]
     
-    self._utc_unix = self._utc_unix_ns / 1.0e-9
-
-  cpdef trace_indices(self, trace_idx = None, trace_map = None, warn_unmapped = False):
-
-    cdef set trace_indices = set()
-    cdef unsigned int tracemap_to_check
+    self._utc_unix = self._utc_unix_ns / 1.0e9
 
-    # convert
-    if trace_idx != None:
-      if isinstance(trace_idx, numbers.Integral):
-        trace_idx = [trace_idx]
-
-      if numpy.iterable(trace_idx):
-        for idx in trace_idx:
-          if isinstance(idx, numbers.Integral):
-            if idx >= 0 or idx < self.maxtraces:
-              trace_indices.add(idx)
-            else:
-              raise KeyError(f"trace_idx {idx} not found in mapped channels.")
-          else:
-            raise ValueError(f"trace_idx {trace_idx} is not of integer type.")
-      else:
-        raise ValueError(f"{trace_idx} is neither an integer nor an iterable.")
-
-    if trace_map != None:
-      if not numpy.iterable(trace_map):
-        trace_map = [trace_map]
-
-      if numpy.iterable(trace_map):
-        for card_to_map in trace_map:
-          if isinstance(card_to_map, numbers.Integral):
-            tracemap_to_check = card_to_map
-          elif isinstance(card_to_map[0], numbers.Integral) and isinstance(card_to_map[1], numbers.Integral):
-            tracemap_to_check = (card_to_map[0] << 16) + card_to_map[1]
-          else:
-            raise ValueError(f"trace_map {card_to_map} is neither of integer type or a sequence if minimum two integers.")
-
-          # stupid search
-          for i, tracemap_entry in enumerate(self._tracemap):
-            if tracemap_entry == tracemap_to_check:
-              trace_indices.add(i)
-              break
-            elif warn_unmapped and tracemap_entry == 0:
-              raise KeyError(f"trace_map {hex(tracemap_to_check)} not found in mapped channels.")
-    return numpy.array(sorted(trace_indices))
+    cdef int _expected_max_ticks = 249999999
+    cdef int _current_clock_offset = abs(self.timestamp[3] - _expected_max_ticks) * 4  
+    # if _current_clock_offset > self._allowed_gps_error_ns:
+    #   print(f"WARNING fcio: max_ticks of last pps cycle {self.timestamp[3]} with { _current_clock_offset } > {self._allowed_gps_error_ns}",file=sys.stderr)
+
+    # default deadtimes are the same for all channels
+    # we update them with the same values
+    # only dr_start is used to track progress
+    cdef int dr_start = 0
+    cdef int dr_end = self.config_ptr.adcs
+
+    # for daqmode 12, each card has it's own eventnumbers, clock counters and deadregions
+    # need to track them separately, but will do it on a channel list basis
+
+    if self.event_ptr.type == 11:
+      dr_start = self.event_ptr.deadregion[5]
+      dr_end = self.event_ptr.deadregion[5] + self.event_ptr.deadregion[6]
+
+    cdef long _dead_interval_start_ns = self.event_ptr.deadregion[0] * 1000000000L + self.event_ptr.deadregion[1] * 4 
+    cdef long _dead_interval_stop_ns = self.event_ptr.deadregion[2] * 1000000000L + self.event_ptr.deadregion[3] * 4
+    cdef long _dead_interval_ns = _dead_interval_stop_ns - _dead_interval_start_ns
+
+    if numpy.any(self._start_time_ns[dr_start : dr_end] == -1):
+      # start times not set yet
+      if _dead_interval_start_ns == 0 and _dead_interval_stop_ns > 0:
+        # if only start is zero, it's daqmode 12 per card and we can estimate the trigger enable timestamp from that
+        self._start_time_ns[dr_start : dr_end] = _dead_interval_stop_ns
+      elif _dead_interval_start_ns == 0 and _dead_interval_stop_ns == 0:
+        self._start_time_ns[dr_start : dr_end] = _daq_synchronized_timestamp_ns
+
+    if _dead_interval_start_ns > 0:
+      # if first event contains start and stop stamps, it's a true dead interval between events, add it
+      self._dead_interval_buffer.add(_dead_interval_start_ns, _dead_interval_stop_ns, self.event_ptr.deadregion[5], self.event_ptr.deadregion[6])
+
+    self._cur_dead_time_ns[dr_start : dr_end] = 0
+    while self._dead_interval_buffer.is_before(_daq_synchronized_timestamp_ns, self.event_ptr.deadregion[5], self.event_ptr.deadregion[6]):
+      self._cur_dead_time_ns[dr_start : dr_end] = self._dead_interval_buffer.read(self.event_ptr.deadregion[5], self.event_ptr.deadregion[6])
+      self._total_dead_time_ns[dr_start : dr_end] += self._cur_dead_time_ns[dr_start : dr_end]
 
   @property
   def fpga_baseline(self):
     """
     1D array.
     shape is (<total number of mapped trace>,)
     Contains the fpga baseline values.
     """
-    return self.theader[self._np_trace_list,0] / self.config_ptr.blprecision
+    return self.theader[self.trace_list,0] / self.config_ptr.blprecision
 
   @property
   def fpga_energy(self):
     """
     1D array.
     shape is (<total number of mapped trace>,)
     Contains the fpga energy values.
     """
     if self.config_ptr.adcbits == 12: #250MHz
-      return self.config_ptr.sumlength / self.config_ptr.blprecision * (self.theader[self._np_trace_list,1] - self.theader[self._np_trace_list,0])
+      return self.config_ptr.sumlength / self.config_ptr.blprecision * (self.theader[self.trace_list,1] - self.theader[self.trace_list,0])
     elif self.config_ptr.adcbits == 16: #62.5MHz
-      return self.theader[self._np_trace_list,1]
+      return self.theader[self.trace_list,1]
   
   @property
-  def dead_time_ns(self):
+  def cur_dead_time_ns(self):
     """
     The dead time since the last triggered event in nanoseconds
     """
-    return self._dead_time_ns[self._np_trace_list]
+    return self._cur_dead_time_ns[self.trace_list]
+
+  @property
+  def start_time_ns(self):
+    return self._start_time_ns[self.trace_list]
 
   @property
-  def total_dead_time_ns(self):
+  def dead_time_ns(self):
     """
     The total dead time since the last DAQ reset (start of run) in nanoseconds
     """
-    return self._total_dead_time_ns[self._np_trace_list]
+    return self._total_dead_time_ns[self.trace_list]
 
   @property
   def card_address(self):
     """
     List of corresponding MAC addresses of the FADC Card per channel.
     Display in human readable form as hex(car_address[index])
     """
-    return self._card_addresses[self._np_trace_list]
+    return self._card_addresses[self.trace_list]
 
   @property
   def card_channel(self):
     """
     List of input RJ45 Jacks of the FADC Card per channel.
     Must be within [0,5] for 16-bit firmware and [0,23] for 12-bit firmware.
     """
-    return self._card_channels[self._np_trace_list]
+    return self._card_channels[self.trace_list]
 
   @property
   def eventsamples(self):
     """
     The number of samples of each waveform.
     This parameter is taken from the Config Record and exposed here for convenience.
     """
@@ -208,26 +190,19 @@
     """
     The maximum time difference between fpga pps and readout server second.
     If no external clock is used, this parameter is 0.
     """
     return numpy.int32(self.config_ptr.gps)
 
   @property
-  def run_time_ns(self):
-    """
-    The number of nanoseconds since trigger enable.
-    """
-    return self._run_time_ns
-
-  @property
-  def run_time(self):
+  def fpga_time_ns(self):
     """
-    run_time_ns in seconds as float64.
+    The number of nanoseconds since daq reset.
     """
-    return self._run_time
+    return self._fpga_time_ns
 
   @property
   def utc_unix_ns(self):
     """
     The number of nanoseconds since 1970 (UTC unix timestamps).
     """
     return self._utc_unix_ns
@@ -243,16 +218,16 @@
   @property
   def trace(self):
     """
     2D array containing the waveforms.
     shape is (<total number of traces in this event>,<number of samples>).
     See trace_list to get the correct trace_index or card_address / card_channel attributes.
     """
-    return self._np_trace[self._np_trace_list]
+    return self._np_trace[self.trace_list]
 
   @property
   def theader(self):
     """
     2D array of the waveforms headers containing the [0]fpga baseline and [1] fpga energy.
     shape is (<total number of traces in this event>,<2>)
     """
-    return self._np_theader[self._np_trace_list]
+    return self._np_theader[self.trace_list]
```

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_recevent.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_recevent.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/src/fcio/cy_fcio/cy_fcio_status.pyx` & `fcio-0.4.0/src/fcio/cy_fcio/cy_fcio_status.pyx`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/.drone.star` & `fcio-0.4.0/subprojects/bufio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/LICENSE` & `fcio-0.4.0/subprojects/bufio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/examples/bufio_benchmark.c` & `fcio-0.4.0/subprojects/bufio/examples/bufio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/meson.build` & `fcio-0.4.0/subprojects/bufio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/src/bufio.c` & `fcio-0.4.0/subprojects/bufio/src/bufio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/src/bufio.h` & `fcio-0.4.0/subprojects/bufio/src/bufio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_delayed_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_follow.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_follow_chunk.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_follow_chunk.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_lockedfile.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_lockedfile.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_tcp_connect.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_tcp_connect.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c` & `fcio-0.4.0/subprojects/bufio/tests/bufio_test_wait_on_tcpclose_with_pending_data.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/bufio/tests/meson.build` & `fcio-0.4.0/subprojects/bufio/tests/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/.drone.star` & `fcio-0.4.0/subprojects/fcio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/LICENSE` & `fcio-0.4.0/subprojects/fcio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/README.md` & `fcio-0.4.0/subprojects/fcio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/meson.build` & `fcio-0.4.0/subprojects/fcio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/src/fcio.c` & `fcio-0.4.0/subprojects/fcio/src/fcio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/src/fcio.h` & `fcio-0.4.0/subprojects/fcio/src/fcio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/src/time_utils.c` & `fcio-0.4.0/subprojects/fcio/src/time_utils.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/fcio/src/time_utils.h` & `fcio-0.4.0/subprojects/fcio/src/time_utils.h`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/.drone.star` & `fcio-0.4.0/subprojects/tmio/.drone.star`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/LICENSE` & `fcio-0.4.0/subprojects/tmio/LICENSE`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/README.md` & `fcio-0.4.0/subprojects/tmio/README.md`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/meson.build` & `fcio-0.4.0/subprojects/tmio/examples/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/timer.c` & `fcio-0.4.0/subprojects/tmio/examples/timer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/timer.h` & `fcio-0.4.0/subprojects/tmio/examples/timer.h`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark.c` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_disk_read.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_disk_write.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_pipe.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_simple.c` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_simple.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh` & `fcio-0.4.0/subprojects/tmio/examples/tmio_benchmark_tcp.sh`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_example_reader.c` & `fcio-0.4.0/subprojects/tmio/examples/tmio_example_reader.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_example_writer.c` & `fcio-0.4.0/subprojects/tmio/examples/tmio_example_writer.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/examples/tmio_sink.c` & `fcio-0.4.0/subprojects/tmio/examples/tmio_sink.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/meson.build` & `fcio-0.4.0/subprojects/tmio/meson.build`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/src/tmio.c` & `fcio-0.4.0/subprojects/tmio/src/tmio.c`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/subprojects/tmio/src/tmio.h` & `fcio-0.4.0/subprojects/tmio/src/tmio.h`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/tests/test_platform.py` & `fcio-0.4.0/tests/test_platform.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/tools/version_util.py` & `fcio-0.4.0/tools/version_util.py`

 * *Files identical despite different names*

### Comparing `fcio-0.3.0/PKG-INFO` & `fcio-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fcio
-Version: 0.3.0
+Version: 0.4.0
 Summary: FlashCam File Format (FCIO) reader for python.
 Author-Email: Simon Sailer <simon.sailer@mpi-hd.mpg.de>
 License: MPL-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

