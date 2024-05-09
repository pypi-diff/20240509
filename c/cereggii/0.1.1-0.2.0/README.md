# Comparing `tmp/cereggii-0.1.1.tar.gz` & `tmp/cereggii-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cereggii-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cereggii-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cereggii-0.1.1.tar` & `cereggii-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,40 @@
--rw-r--r--   0        0        0       79 2023-12-20 10:49:46.054887 cereggii-0.1.1/CMakeLists.txt
--rw-r--r--   0        0        0    11357 2023-12-20 10:49:46.054887 cereggii-0.1.1/LICENSE
--rw-r--r--   0        0        0     7147 2023-12-20 10:49:46.054887 cereggii-0.1.1/README.md
--rw-r--r--   0        0        0     2721 2023-12-20 10:49:46.054887 cereggii-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1513 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/CMakeLists.txt
--rw-r--r--   0        0        0      273 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/__about__.py
--rw-r--r--   0        0        0      621 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/__init__.py
--rw-r--r--   0        0        0     7431 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/_cereggii.pyi
--rw-r--r--   0        0        0      487 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/__init__.py
--rw-r--r--   0        0        0    14838 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/atomic_dict.c
--rw-r--r--   0        0        0     3912 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/blocks.c
--rw-r--r--   0        0        0      338 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/delete.c
--rw-r--r--   0        0        0    16756 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/insert.c
--rw-r--r--   0        0        0     3848 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/lookup.c
--rw-r--r--   0        0        0     4421 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/meta.c
--rw-r--r--   0        0        0      580 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/migrate.c
--rw-r--r--   0        0        0     9834 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/node_ops.c
--rw-r--r--   0        0        0     1194 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/node_sizes_table.c
--rw-r--r--   0        0        0     2433 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_dict/reservation_buffer.c
--rw-r--r--   0        0        0      615 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_int/__init__.py
--rw-r--r--   0        0        0    29066 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_int/atomic_int.c
--rw-r--r--   0        0        0    11866 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_int/handle.c
--rw-r--r--   0        0        0     2848 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_ref.c
--rw-r--r--   0        0        0      484 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/atomic_ref.py
--rw-r--r--   0        0        0    13773 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/cereggii/cereggii.c
--rw-r--r--   0        0        0     1271 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/include/atomic_dict.h
--rw-r--r--   0        0        0     6600 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/include/atomic_dict_internal.h
--rw-r--r--   0        0        0    11957 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/include/atomic_int.h
--rw-r--r--   0        0        0     1776 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/include/atomic_int_internal.h
--rw-r--r--   0        0        0      995 2023-12-20 10:49:46.054887 cereggii-0.1.1/src/include/atomic_ref.h
--rw-r--r--   0        0        0     8184 1970-01-01 00:00:00.000000 cereggii-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       79 2024-05-09 15:25:04.105747 cereggii-0.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0    11357 2024-05-09 15:25:04.105747 cereggii-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7421 2024-05-09 15:25:04.105747 cereggii-0.2.0/README.md
+-rw-r--r--   0        0        0     2771 2024-05-09 15:25:04.105747 cereggii-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1715 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/CMakeLists.txt
+-rw-r--r--   0        0        0      273 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/__about__.py
+-rw-r--r--   0        0        0      675 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/__init__.py
+-rw-r--r--   0        0        0     8732 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/_cereggii.pyi
+-rw-r--r--   0        0        0      487 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/atomic_dict/__init__.py
+-rw-r--r--   0        0        0     4617 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/atomic_dict/accessor_storage.c
+-rw-r--r--   0        0        0    20352 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/atomic_dict/atomic_dict.c
+-rw-r--r--   0        0        0     6019 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/atomic_dict/blocks.c
+-rw-r--r--   0        0        0     6907 2024-05-09 15:25:04.105747 cereggii-0.2.0/src/cereggii/atomic_dict/delete.c
+-rw-r--r--   0        0        0    14366 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/insert.c
+-rw-r--r--   0        0        0     3152 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/iter.c
+-rw-r--r--   0        0        0     9020 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/lookup.c
+-rw-r--r--   0        0        0     8212 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/meta.c
+-rw-r--r--   0        0        0    15290 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/migrate.c
+-rw-r--r--   0        0        0    15057 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/node_ops.c
+-rw-r--r--   0        0        0     1194 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/node_sizes_table.c
+-rw-r--r--   0        0        0     4241 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_dict/robin_hood.c
+-rw-r--r--   0        0        0     1670 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_event.c
+-rw-r--r--   0        0        0      615 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_int/__init__.py
+-rw-r--r--   0        0        0    29150 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_int/atomic_int.c
+-rw-r--r--   0        0        0    11866 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_int/handle.c
+-rw-r--r--   0        0        0    13430 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_ops.c
+-rw-r--r--   0        0        0     3061 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_ref.c
+-rw-r--r--   0        0        0      484 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/atomic_ref.py
+-rw-r--r--   0        0        0    18933 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/cereggii.c
+-rw-r--r--   0        0        0      586 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/constants.c
+-rw-r--r--   0        0        0      358 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/cereggii/constants.py
+-rw-r--r--   0        0        0     2176 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_dict.h
+-rw-r--r--   0        0        0    12814 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_dict_internal.h
+-rw-r--r--   0        0        0     1012 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_event.h
+-rw-r--r--   0        0        0    11957 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_int.h
+-rw-r--r--   0        0        0     1776 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_int_internal.h
+-rw-r--r--   0        0        0    11183 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_ops.h
+-rw-r--r--   0        0        0      995 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/atomic_ref.h
+-rw-r--r--   0        0        0      600 2024-05-09 15:25:04.109747 cereggii-0.2.0/src/include/constants.h
+-rw-r--r--   0        0        0     8529 1970-01-01 00:00:00.000000 cereggii-0.2.0/PKG-INFO
```

### Comparing `cereggii-0.1.1/LICENSE` & `cereggii-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/pyproject.toml` & `cereggii-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ]
 dependencies = []
 
 [project.optional-dependencies]
 dev = [
   "build==1.0.3",
   "pytest==7.4.2",
+  "pytest-reraise==2.1.2",
   "black==23.9.1",
   "ruff==0.0.292",
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/dpdani/cereggii#readme"
@@ -45,16 +46,17 @@
 directory = "src"
 
 [tool.py-build-cmake.sdist]
 include = ["CMakeLists.txt", "src/CMakeLists.txt", "src/include/*"]
 
 [tool.py-build-cmake.cmake]
 minimum_version = "3.18"
-build_type = "Debug"
+build_type = "RelWithDebInfo"
 source_path = "src"
+args = ["-L"]
 build_args = ["-j"]
 install_components = ["python_modules"]
 
 
 [tool.black]
 target-version = ["py39"]
 line-length = 120
```

### Comparing `cereggii-0.1.1/src/CMakeLists.txt` & `cereggii-0.2.0/src/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 cmake_minimum_required(VERSION 3.18)
 project(cereggii)
 
 set(PY_BUILD_CMAKE_MODULE_NAME "cereggii")
 
 
 set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
-add_compile_options("-march=native")
+add_compile_options("-mcx16")
+add_compile_options("-msse4.2")
 
 message("Python3_INCLUDE_DIR=" ${Python3_INCLUDE_DIR})
 execute_process(COMMAND python -c "import sysconfig; print(sysconfig.get_path('include'), end='')" OUTPUT_VARIABLE Python3_INCLUDE_DIR)
 message("Python3_INCLUDE_DIR=" ${Python3_INCLUDE_DIR})
 find_package(Python3 REQUIRED COMPONENTS Development.Module)
 
 
 include_directories("include/")
 
 # Add the module to compile
 Python3_add_library(_cereggii MODULE
+        "cereggii/atomic_dict/accessor_storage.c"
         "cereggii/atomic_dict/atomic_dict.c"
         "cereggii/atomic_dict/blocks.c"
         "cereggii/atomic_dict/delete.c"
         "cereggii/atomic_dict/insert.c"
+        "cereggii/atomic_dict/iter.c"
         "cereggii/atomic_dict/lookup.c"
         "cereggii/atomic_dict/meta.c"
         "cereggii/atomic_dict/migrate.c"
         "cereggii/atomic_dict/node_ops.c"
         "cereggii/atomic_dict/node_sizes_table.c"
-        "cereggii/atomic_dict/reservation_buffer.c"
+        "cereggii/atomic_dict/robin_hood.c"
         "cereggii/atomic_int/atomic_int.c"
         "cereggii/atomic_int/handle.c"
+        "cereggii/atomic_event.c"
+        "cereggii/atomic_ops.c"
         "cereggii/atomic_ref.c"
         "cereggii/cereggii.c"
+        "cereggii/constants.c"
 )
 
 # Install the module
 install(TARGETS _cereggii
         EXCLUDE_FROM_ALL
         COMPONENT python_modules
         DESTINATION ${PY_BUILD_CMAKE_MODULE_NAME})
```

### Comparing `cereggii-0.1.1/src/cereggii/__init__.py` & `cereggii-0.2.0/src/cereggii/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # SPDX-FileCopyrightText: 2023-present dpdani <git@danieleparmeggiani.me>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 """
-
-Concurrent threading utilities for Python
-
+Thread synchronization utilities for free-threaded Python.
 """
 
 import sys
 import warnings
 
 from .__about__ import __license__, __version__, __version_tuple__  # noqa: F401
 from .atomic_dict import AtomicDict  # noqa: F401
 from .atomic_int import AtomicInt, AtomicIntHandle  # noqa: F401
 from .atomic_ref import AtomicRef  # noqa: F401
+from .constants import *  # noqa: F403
 
 
 if not getattr(sys.flags, "nogil", False):
     warnings.warn(
         "this library is meant to be used with nogil python: https://github.com/colesbury/nogil", stacklevel=1
     )
```

### Comparing `cereggii-0.1.1/src/cereggii/_cereggii.pyi` & `cereggii-0.2.0/src/cereggii/_cereggii.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,27 @@
+from collections.abc import Iterator
 from typing import Callable, NewType, SupportsComplex, SupportsFloat, SupportsInt
 
 Key = NewType("Key", object)
-Value = NewType("Value", object)
+Value = NewType("Value", object | None)
 Cancel = NewType("Cancel", object)
 
 Number = SupportsInt | SupportsFloat | SupportsComplex
 
+NOT_FOUND: object
+ANY: object
+EXPECTATION_FAILED: object
+ExpectationFailed: Exception
+
 class AtomicDict:
     """A thread-safe dictionary (hashmap), that's almost-lock-free™."""
 
-    def __init__(self, iterable: dict | None = None, /, *, min_size: int | None = None, **kwargs):
+    def __init__(
+        self, iterable: dict | None = None, /, *, min_size: int | None = None, buffer_size: int | None = None, **kwargs
+    ):
         """Constructor method
 
         :param iterable: an iterable to initialize this dictionary with. For now,
             only `dict` can be supplied to this parameter.
 
         :param min_size: the size initially allocated. Using this
             parameter possibly avoids re-allocations and migrations during inserts.
@@ -25,59 +33,28 @@
             This follows the behavior of built-in dictionary, but slightly differs:
             keys that are already parameters to this ``__init__`` method will not be
             considered, because of Python's ``**kwargs`` behavior.
             E.g. ``AtomicDict(initial_size=123)`` will not create a dictionary
             mapping ``initial_size`` to 123, but an empty one.
         """
     # def __contains__(self, item: Key) -> bool: ...
-    # def __delitem__(self, item: Key) -> None: ...
+    def __delitem__(self, item: Key) -> None: ...
     def __getitem__(self, item: Key) -> object: ...
     # def __ior__(self, other) -> None: ...
     # def __iter__(self) -> Iterable[Key, Value]: ...
-    # def __len__(self) -> int: ...
+    def __len__(self) -> int: ...
     # def __eq__(self, other) -> bool: ...
     # def __or__(self, other) -> AtomicDict: ...
     # def __ror__(self, other) -> AtomicDict: ...
     def __repr__(self) -> str: ...
     # def __reversed__(self) -> AtomicDict: ...
     def __setitem__(self, key: Key, value: Value) -> None: ...
     # def __sizeof__(self) -> int: ...
     # def __str__(self) -> str: ...
     # def __subclasshook__(self): ...
-    # def batch_lookup(self, batch: dict) -> dict:
-    #     """Batch many lookups together for efficient memory access.
-    #
-    #     Whatever the values provided in :param:`batch`, they will be substituted with
-    #     the found values, or ``KeyError``. Notice no exception is thrown: the
-    #     ``KeyError`` object instead is the returned value for a non-found key. If you
-    #     have ``KeyError`` values in your :class:`AtomicDict`, you may have trouble
-    #     distinguishing between a ``KeyError`` that implies a lookup failure,
-    #     and a ``KeyError`` that was indeed found.
-    #
-    #     The values themselves, provided in :param:`batch`, will always be substituted.
-    #
-    #     An example call::
-    #
-    #         foo = AtomicDict({'a': 1, 'b': 2, 'c': 3})
-    #         foo.batch_lookup({
-    #             'a': None,
-    #             'b': None,
-    #             'f': None,
-    #         })
-    #
-    #     which will return::
-    #
-    #         {
-    #            'a': 1,
-    #            'b': 2,
-    #            'f': KeyError,
-    #         }
-    #
-    #     :returns: the input :param:`batch` dictionary, with substituted values.
-    #     """
     # def clear(self) -> None: ...
     # def copy(self) -> AtomicDict: ...
     # @classmethod
     # def fromkeys(cls, iterable: Iterable[Key], value=None) -> AtomicDict: ...
     def get(self, key: Key, default: Value | None = None): ...
     # def items(self) -> Iterable[Key, Value]: ...
     # def keys(self) -> Iterable[Key]: ...
@@ -121,15 +98,75 @@
     #
     #     Note that having :param:`fn` return ``cancel`` instead of the unchanged
     #     ``value`` may be more efficient: it avoids a redundant atomic write to memory.
     #
     #     :returns: None
     #     """
     # def values(self) -> Iterable[Value]: ...
+    def compare_and_set(self, key: Key, expected: Value, desired: Value) -> None: ...
+    def len_bounds(self) -> tuple[int, int]: ...
+    def approx_len(self) -> int: ...
+    def fast_iter(self, partitions=1, this_partition=0) -> Iterator[tuple[Key, Value]]: ...
+    def batch_getitem(self, batch: dict, chunk_size: int = 128) -> dict:
+        """Batch many lookups together for efficient memory access.
+
+        Whatever the values provided in :param:`batch`, they will be substituted with
+        the found values, or ``cereggii.NOT_FOUND``.
+        Notice no exception is thrown: the ``cereggii.NOT_FOUND`` object instead
+        is the returned value for a non-found key.
+        Also notice that the ``cereggii.NOT_FOUND`` object can never be inserted
+        into an ``AtomicDict``.
+
+        The values themselves, provided in :param:`batch`, will always be substituted.
+
+        An example call::
+
+            foo = AtomicDict({'a': 1, 'b': 2, 'c': 3})
+            foo.batch_getitem({
+                'a': None,
+                'b': None,
+                'f': None,
+            })
+
+        which will return::
+
+            {
+               'a': 1,
+               'b': 2,
+               'f': <cereggii.NOT_FOUND>,
+            }
+
+        :returns: the input :param:`batch` dictionary, with substituted values.
+        """
+    # def aggregate(self, iterator: Iterator[tuple[Key, Value]], aggregation: Callable[[Key, Value, Value], Value])
+    # -> None:
+    #     """
+    #     Aggregate the values in this dictionary with those found in ``iterator``, as computed by ``aggregation``.
+    #
+    #     The ``aggregation`` parameter expects a function that takes as input a key, the value currently stored
+    #     in the dictionary, and the new value from ``iterator``, and then returns the aggregated value.
+    #
+    #     For instance, to aggregate counts::
+    #
+    #         d = AtomicDict()
+    #
+    #         it = [
+    #             ("red", 1),
+    #             ("green", 3),
+    #             ("blue", 40),
+    #             ("red", 1),
+    #         ]
+    #
+    #         d.aggregate(it, lambda key, current, new:
+    #             new if current is cereggii.NOT_FOUND else current + new
+    #         )
+    #     """
+    def compact(self) -> None: ...
     def debug(self) -> dict: ...
+    def rehash(self, o: object) -> int: ...
 
 class AtomicRef:
     """An object reference that may be updated atomically."""
 
     def __init__(self, reference: object | None = None): ...
     def compare_and_set(self, expected: object, updated: object) -> bool: ...
     def get(self) -> object: ...
```

### Comparing `cereggii-0.1.1/src/cereggii/atomic_dict/atomic_dict.c` & `cereggii-0.2.0/src/cereggii/atomic_dict/atomic_dict.c`

 * *Files 23% similar despite different names*

```diff
@@ -9,59 +9,56 @@
 #include "atomic_ref.h"
 #include "pythread.h"
 
 
 PyObject *
 AtomicDict_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwds))
 {
-    AtomicDict *self;
+    AtomicDict *self = NULL;
     self = (AtomicDict *) type->tp_alloc(type, 0);
     if (self != NULL) {
+        self->metadata = NULL;
         self->metadata = (AtomicRef *) AtomicRef_new(&AtomicRef_Type, NULL, NULL);
         if (self->metadata == NULL)
             goto fail;
         AtomicRef_init(self->metadata, NULL, NULL);
 
-        self->new_gen_metadata = (AtomicRef *) AtomicRef_new(&AtomicRef_Type, NULL, NULL);
-        if (self->new_gen_metadata == NULL)
-            goto fail;
-        AtomicRef_init(self->new_gen_metadata, NULL, NULL);
-
         self->reservation_buffer_size = 0;
-        Py_tss_t *tss_key = PyThread_tss_alloc();
+        Py_tss_t *tss_key = NULL;
+        tss_key = PyThread_tss_alloc();
         if (tss_key == NULL)
             goto fail;
         if (PyThread_tss_create(tss_key))
             goto fail;
         assert(PyThread_tss_is_created(tss_key) != 0);
-        self->tss_key = tss_key;
+        self->accessor_key = tss_key;
 
-        self->reservation_buffers = Py_BuildValue("[]");
-        if (self->reservation_buffers == NULL)
+        self->accessors = NULL;
+        self->accessors = Py_BuildValue("[]");
+        if (self->accessors == NULL)
             goto fail;
     }
     return (PyObject *) self;
 
     fail:
     Py_XDECREF(self->metadata);
-    Py_XDECREF(self->new_gen_metadata);
+    Py_XDECREF(self->accessors);
     Py_XDECREF(self);
     return NULL;
 }
 
 int
 AtomicDict_init(AtomicDict *self, PyObject *args, PyObject *kwargs)
 {
     assert(AtomicRef_Get(self->metadata) == Py_None);
-    assert(AtomicRef_Get(self->new_gen_metadata) == Py_None);
     int64_t init_dict_size = 0;
     int64_t min_size = 0;
     int64_t buffer_size = 4;
     PyObject *init_dict = NULL;
-    atomic_dict_meta *meta = NULL;
+    AtomicDict_Meta *meta = NULL;
 
     if (args != NULL) {
         if (!PyArg_ParseTuple(args, "|O", &init_dict)) {
             goto fail;
         }
         if (init_dict != NULL) {
             if (!PyDict_Check(init_dict)) {
@@ -86,35 +83,35 @@
         PyObject *buffer_size_arg = PyDict_GetItemString(kwargs, "buffer_size");
         if (buffer_size_arg != NULL) {
             buffer_size = PyLong_AsLong(buffer_size_arg);
             PyDict_DelItemString(kwargs, "buffer_size");
             if (buffer_size != 1 && buffer_size != 2 && buffer_size != 4 &&
                 buffer_size != 8 && buffer_size != 16 && buffer_size != 32 &&
                 buffer_size != 64) {
-                PyErr_SetString(PyExc_ValueError, "buffer_size not in [1, 2, 4, 8, 16, 32, 64]");
+                PyErr_SetString(PyExc_ValueError, "buffer_size not in (1, 2, 4, 8, 16, 32, 64)");
                 return -1;
             }
         }
 
         if (init_dict == NULL) {
             init_dict = kwargs;
         } else {
             // this internally calls Py_BEGIN_CRITICAL_SECTION
             PyDict_Update(init_dict, kwargs);
         }
     }
 
     if (init_dict != NULL) {
-        init_dict_size = PyDict_Size(init_dict);
+        init_dict_size = PyDict_Size(init_dict) * 2;
     }
-    if (init_dict_size % 64 == 0) { // allocate one more entry: cannot write to entry 0
+    if (init_dict_size % ATOMIC_DICT_ENTRIES_IN_BLOCK == 0) { // allocate one more entry: cannot write to entry 0
         init_dict_size++;
     }
-    if (min_size < 64) {
-        min_size = 64;
+    if (min_size < ATOMIC_DICT_ENTRIES_IN_BLOCK) {
+        min_size = ATOMIC_DICT_ENTRIES_IN_BLOCK;
     }
 
     self->reservation_buffer_size = buffer_size;
 
     uint8_t log_size = 0, init_dict_log_size = 0;
     uint64_t min_size_tmp = (uint64_t) min_size;
     uint64_t init_dict_size_tmp = (uint64_t) init_dict_size;
@@ -146,262 +143,472 @@
         init_dict_log_size++;
     }
     if (init_dict_log_size > log_size) {
         log_size = init_dict_log_size;
     }
 
     create:
-    meta = AtomicDict_NewMeta(log_size, NULL);
+    meta = NULL;
+    meta = AtomicDictMeta_New(log_size);
     if (meta == NULL)
         goto fail;
+    AtomicDictMeta_ClearIndex(meta);
+    if (AtomicDictMeta_InitBlocks(meta) < 0)
+        goto fail;
     AtomicRef_Set(self->metadata, (PyObject *) meta);
 
-    atomic_dict_block *block;
+    AtomicDict_Block *block;
     int64_t i;
-    for (i = 0; i < init_dict_size / 64; i++) {
+    for (i = 0; i < init_dict_size / ATOMIC_DICT_ENTRIES_IN_BLOCK; i++) {
         // allocate blocks
-        block = AtomicDict_NewBlock(meta);
+        block = AtomicDictBlock_New(meta);
         if (block == NULL)
             goto fail;
         meta->blocks[i] = block;
-        if (i + 1 < (1 << log_size) >> 6) {
+        if (i + 1 < (1 << log_size) >> ATOMIC_DICT_LOG_ENTRIES_IN_BLOCK) {
             meta->blocks[i + 1] = NULL;
         }
         meta->greatest_allocated_block++;
     }
-    if (init_dict_size % 64 > 0) {
+    if (init_dict_size % ATOMIC_DICT_ENTRIES_IN_BLOCK > 0) {
         // allocate additional block
-        block = AtomicDict_NewBlock(meta);
+        block = AtomicDictBlock_New(meta);
         if (block == NULL)
             goto fail;
         meta->blocks[i] = block;
-        if (i + 1 < (1 << log_size) >> 6) {
+        if (i + 1 < (1 << log_size) >> ATOMIC_DICT_LOG_ENTRIES_IN_BLOCK) {
             meta->blocks[i + 1] = NULL;
         }
         meta->greatest_allocated_block++;
     }
 
     meta->inserting_block = 0;
-    atomic_dict_reservation_buffer *rb;
-    atomic_dict_entry_loc entry_loc;
+    AtomicDict_AccessorStorage *storage;
+    AtomicDict_EntryLoc entry_loc;
+    self->sync_op.v = 0;
+    self->len = 0;
+    self->len_dirty = 0;
 
     if (init_dict != NULL && PyDict_Size(init_dict) > 0) {
         PyObject *key, *value;
         Py_hash_t hash;
         Py_ssize_t pos = 0;
 
         while (PyDict_Next(init_dict, &pos, &key, &value)) {
             hash = PyObject_Hash(key);
             if (hash == -1)
                 goto fail;
 
-            int inserted = AtomicDict_UnsafeInsert(self, key, hash, value, pos); // we want to avoid pos = 0
+            self->len++; // we want to avoid pos = 0
+            AtomicDict_Entry *entry = AtomicDict_GetEntryAt(self->len, meta);
+            Py_INCREF(key);
+            Py_INCREF(value);
+            entry->flags = ENTRY_FLAGS_RESERVED;
+            entry->hash = hash;
+            entry->key = key;
+            entry->value = value;
+            int inserted = AtomicDict_UnsafeInsert(meta, hash, self->len);
             if (inserted == -1) {
                 Py_DECREF(meta);
                 log_size++;
                 goto create;
             }
         }
-        meta->inserting_block = pos >> 6;
+        meta->inserting_block = self->len >> ATOMIC_DICT_LOG_ENTRIES_IN_BLOCK;
 
-        if (pos > 0) {
-            rb = AtomicDict_GetReservationBuffer(self);
-            if (rb == NULL)
+        if (self->len > 0) {
+            storage = AtomicDict_GetOrCreateAccessorStorage(self);
+            if (storage == NULL)
                 goto fail;
 
             // handle possibly misaligned reservations on last block
             // => put them into this thread's reservation buffer
-            entry_loc.entry = &meta->blocks[(pos + 1) >> 6]->entries[(pos + 1) & 63];
-            entry_loc.location = pos + 1;
-            uint8_t n = self->reservation_buffer_size - (uint8_t) (entry_loc.location % self->reservation_buffer_size);
-            if (n > 0) {
-                AtomicDict_ReservationBufferPut(rb, &entry_loc, n);
+            if (AtomicDict_BlockOf(self->len + 1) <= meta->greatest_allocated_block) {
+                entry_loc.entry = AtomicDict_GetEntryAt(self->len + 1, meta);
+                entry_loc.location = self->len + 1;
+
+                uint8_t n =
+                    self->reservation_buffer_size - (uint8_t) (entry_loc.location % self->reservation_buffer_size);
+                assert(n <= ATOMIC_DICT_ENTRIES_IN_BLOCK);
+                while (AtomicDict_BlockOf(self->len + n) > meta->greatest_allocated_block) {
+                    n--;
+
+                    if (n == 0)
+                        break;
+                }
+
+                if (n > 0) {
+                    AtomicDict_ReservationBufferPut(&storage->reservation_buffer, &entry_loc, n);
+                }
             }
         }
     }
 
-    if (!(meta->blocks[0]->entries[0].flags & ENTRY_FLAGS_RESERVED)) {
-        rb = AtomicDict_GetReservationBuffer(self);
-        if (rb == NULL)
+    self->accessors_lock.v = 0;  // https://github.com/colesbury/nogil/blob/043f29ab2afab9cef5edd07875816d3354cb9d2c/Objects/dictobject.c#L334
+
+    if (!(AtomicDict_GetEntryAt(0, meta)->flags & ENTRY_FLAGS_RESERVED)) {
+        storage = AtomicDict_GetOrCreateAccessorStorage(self);
+        if (storage == NULL)
             goto fail;
 
         // mark entry 0 as reserved and put the remaining entries
         // into this thread's reservation buffer
-        meta->blocks[0]->entries[0].flags |= ENTRY_FLAGS_RESERVED;
+        AtomicDict_GetEntryAt(0, meta)->flags |= ENTRY_FLAGS_RESERVED;
         for (i = 1; i < self->reservation_buffer_size; ++i) {
-            entry_loc.entry = &meta->blocks[0]->entries[i & 63];
+            entry_loc.entry = AtomicDict_GetEntryAt(i, meta);
             entry_loc.location = i;
             if (entry_loc.entry->key == NULL) {
                 int found = 0;
                 for (int j = 0; j < RESERVATION_BUFFER_SIZE; ++j) {
-                    if (rb->reservations[j].location == entry_loc.location) {
+                    if (storage->reservation_buffer.reservations[j].location == entry_loc.location) {
                         found = 1;
                         break;
                     }
                 }
                 if (!found) {
-                    AtomicDict_ReservationBufferPut(rb, &entry_loc, 1);
+                    AtomicDict_ReservationBufferPut(&storage->reservation_buffer, &entry_loc, 1);
                 }
             }
         }
     }
 
     Py_XDECREF(init_dict);
+    Py_DECREF(meta); // so that the only meta's refcount depends only on AtomicRef
+    assert(Py_REFCNT(meta) == 1);
     return 0;
     fail:
     Py_XDECREF(meta);
     Py_XDECREF(init_dict);
+    if (!PyErr_Occurred()) {
+        PyErr_SetString(PyExc_RuntimeError, "error during initialization.");
+    }
     return -1;
 }
 
 void
 AtomicDict_dealloc(AtomicDict *self)
 {
     PyObject_GC_UnTrack(self);
-    atomic_dict_meta *meta = (atomic_dict_meta *) AtomicRef_Get(self->metadata);
-    PyMem_RawFree(meta->blocks);
-    Py_DECREF(meta); // decref for the above atomic_ref_get_ref
+
+    AtomicDict_Meta *meta = NULL;
+    meta = (AtomicDict_Meta *) AtomicRef_Get(self->metadata);
+
+    if ((PyObject *) meta != Py_None) {
+        AtomicRef_Set(self->metadata, Py_None);  // this decref's meta
+
+        assert(Py_REFCNT(meta) == 1);
+        Py_DECREF(meta); // should call dealloc
+    }
+
     Py_CLEAR(self->metadata);
-    Py_CLEAR(self->new_gen_metadata);
-    Py_CLEAR(self->reservation_buffers);
+    Py_CLEAR(self->accessors);
     // this should be enough to deallocate the reservation buffers themselves as well:
     // the list should be the only reference to them anyway
-    PyThread_tss_delete(self->tss_key);
-    PyThread_tss_free(self->tss_key);
-    // clear this dict's elements (iter XXX)
+    PyThread_tss_delete(self->accessor_key);
+    PyThread_tss_free(self->accessor_key);
+
     Py_TYPE(self)->tp_free((PyObject *) self);
 }
 
 int
 AtomicDict_traverse(AtomicDict *self, visitproc visit, void *arg)
 {
     Py_VISIT(self->metadata);
-    Py_VISIT(self->new_gen_metadata);
+    Py_VISIT(self->accessors);
     // traverse this dict's elements (iter XXX)
     return 0;
 }
 
 /**
  * This is not thread-safe!
  *
  * Used at initialization time, when there can be no concurrent access.
  * Doesn't allocate blocks, nor check for migrations, nor update dk->metadata refcount.
  * Doesn't do updates: repeated keys will be repeated, so make sure successive
  * calls to this function don't try to insert the same key into the same AtomicDict.
  **/
 int
-AtomicDict_UnsafeInsert(AtomicDict *self, PyObject *key, Py_hash_t hash, PyObject *value, Py_ssize_t pos)
+AtomicDict_UnsafeInsert(AtomicDict_Meta *meta, Py_hash_t hash, uint64_t pos)
 {
-    atomic_dict_meta meta;
-    meta = *(atomic_dict_meta *) AtomicRef_Get(self->metadata);
     // pos === node_index
-    atomic_dict_block *block = meta.blocks[pos >> 6];
-    block->entries[pos & 63].flags = ENTRY_FLAGS_RESERVED;
-    block->entries[pos & 63].hash = hash;
-    block->entries[pos & 63].key = key;
-    block->entries[pos & 63].value = value;
-
-    atomic_dict_node temp;
-    atomic_dict_node node = {
+    AtomicDict_Node temp;
+    AtomicDict_Node node = {
         .index = pos,
         .tag = hash,
     };
-    uint64_t ix = hash & ((1 << meta.log_size) - 1);
+    uint64_t ix = AtomicDict_Distance0Of(hash, meta);
 
-    for (int probe = 0; probe < (1 << meta.distance_size); probe++) {
-        AtomicDict_ReadNodeAt(ix + probe, &temp, &meta);
+    for (int probe = 0; probe < meta->max_distance; probe++) {
+        AtomicDict_ReadNodeAt(ix + probe, &temp, meta);
 
         if (temp.node == 0) {
             node.distance = probe;
-            AtomicDict_WriteNodeAt(ix + probe, &node, &meta);
+            AtomicDict_WriteNodeAt(ix + probe, &node, meta);
             goto done;
         }
 
         if (temp.distance < probe) {
             // non-atomic robin hood
             node.distance = probe;
-            uint64_t i = ix + probe;
-            AtomicDict_WriteNodeAt(i, &node, &meta);
+            AtomicDict_WriteNodeAt(ix + probe, &node, meta);
+//            ix = ix + probe - temp.distance;
+            ix -= temp.distance;
+            probe = temp.distance;
             node = temp;
-            i++;
-            while (temp.node != 0) { // until first empty slot
-                AtomicDict_ReadNodeAt(i, &temp, &meta);
-                if (node.distance > temp.distance) {
-                    AtomicDict_WriteNodeAt(i, &node, &meta);
-                    node = temp;
-                }
-                i++;
-            }
-            AtomicDict_WriteNodeAt(i, &temp, &meta);
-            goto done;
         }
     }
     // probes exhausted
     return -1;
     done:
-    Py_INCREF(key);
-    Py_INCREF(value);
     return 0;
 }
 
+int
+AtomicDict_CountKeysInBlock(int64_t block_ix, AtomicDict_Meta *meta)
+{
+    int found = 0;
+
+    AtomicDict_Entry *entry_p, entry;
+    AtomicDict_SearchResult sr;
+
+    for (int64_t i = 0; i < ATOMIC_DICT_ENTRIES_IN_BLOCK; ++i) {
+        uint64_t entry_ix = block_ix * ATOMIC_DICT_ENTRIES_IN_BLOCK + i;
+        entry_p = AtomicDict_GetEntryAt(entry_ix, meta);
+        AtomicDict_ReadEntry(entry_p, &entry);
+
+        if (entry.value != NULL) {
+            AtomicDict_LookupEntry(meta, entry_ix, entry.hash, &sr);
+            if (sr.found) {
+                found++;
+            }
+        }
+    }
+
+    return found;
+}
+
+PyObject *
+AtomicDict_LenBounds(AtomicDict *self)
+{
+    AtomicDict_Meta *meta = NULL;
+    meta = (AtomicDict_Meta *) AtomicRef_Get(self->metadata);
+    if (meta == NULL)
+        goto fail;
+
+    int64_t gab = meta->greatest_allocated_block + 1;
+    int64_t gdb = meta->greatest_deleted_block + 1;
+    int64_t grb = meta->greatest_refilled_block + 1;
+    // todo: handle greedy alloc
+
+    int64_t supposedly_full_blocks = (gab - gdb + grb - 1);
+
+    // visit the gab
+    int64_t found = AtomicDict_CountKeysInBlock(gab - 1, meta);
+
+    if (gab - 1 != gdb) {
+        supposedly_full_blocks--;
+
+        // visit the gdb
+        found += AtomicDict_CountKeysInBlock(gdb, meta);
+    }
+
+    if (grb != gab - 1 && grb != gdb) {
+        supposedly_full_blocks--;
+
+        // visit the grb
+        found += AtomicDict_CountKeysInBlock(grb, meta);
+    }
+    Py_DECREF(meta);
+
+    if (supposedly_full_blocks < 0) {
+        supposedly_full_blocks = 0;
+    }
+
+    int64_t upper = supposedly_full_blocks * ATOMIC_DICT_ENTRIES_IN_BLOCK;
+
+    Py_ssize_t threads_count = PyList_Size(self->accessors);
+    int64_t lower =
+        supposedly_full_blocks * ATOMIC_DICT_ENTRIES_IN_BLOCK - threads_count * self->reservation_buffer_size;
+
+    AtomicDict_ReservationBuffer *rb;
+    for (int i = 0; i < threads_count; ++i) {
+        rb = (AtomicDict_ReservationBuffer *) PyList_GetItem(self->accessors, i);
+
+        if (rb == NULL)
+            goto fail;
+
+        lower += self->reservation_buffer_size - rb->count;
+    }
+
+    if (upper < 0) upper = 0;
+    if (lower < 0) lower = 0;
+
+    return Py_BuildValue("(ll)", lower + found, upper + found);
+
+    fail:
+    Py_XDECREF(meta);
+    return NULL;
+}
+
+PyObject *
+AtomicDict_ApproxLen(AtomicDict *self)
+{
+    PyObject *bounds = NULL;
+    PyObject *lower = NULL;
+    PyObject *upper = NULL;
+    PyObject *sum = NULL;
+    PyObject *avg = NULL;
+
+    bounds = AtomicDict_LenBounds(self);
+    if (bounds == NULL)
+        goto fail;
+
+    lower = PyTuple_GetItem(bounds, 0);
+    upper = PyTuple_GetItem(bounds, 1);
+    if (lower == NULL || upper == NULL)
+        goto fail;
+
+    sum = PyNumber_Add(lower, upper);
+    if (sum == NULL)
+        goto fail;
+
+    avg = PyNumber_FloorDivide(sum, PyLong_FromLong(2));
+    // PyLong_FromLong(2) will not return NULL
+
+    Py_DECREF(bounds);
+    Py_DECREF(lower);
+    Py_DECREF(upper);
+    Py_DECREF(sum);
+    return avg;
+
+    fail:
+    Py_XDECREF(bounds);
+    Py_XDECREF(lower);
+    Py_XDECREF(upper);
+    Py_XDECREF(sum);
+    Py_XDECREF(avg);
+    return NULL;
+}
+
+Py_ssize_t
+AtomicDict_Len_impl(AtomicDict *self)
+{
+    PyObject *len = NULL, *local_len = NULL;
+    Py_ssize_t int_len;
+
+    if (!self->len_dirty) {
+        int_len = self->len;
+        return int_len;
+    }
+
+    len = PyLong_FromSsize_t(self->len);
+    if (len == NULL)
+        goto fail;
+
+    for (Py_ssize_t i = 0; i < PyList_Size(self->accessors); ++i) {
+        AtomicDict_AccessorStorage *storage = NULL;
+        storage = (AtomicDict_AccessorStorage *) PyList_GetItem(self->accessors, i);
+        assert(storage != NULL);
+
+        local_len = PyLong_FromLong(storage->local_len);
+        if (local_len == NULL)
+            goto fail;
+
+        len = PyNumber_InPlaceAdd(len, local_len);
+        Py_DECREF(local_len);
+        local_len = NULL;
+        storage->local_len = 0;
+    }
+
+    int_len = PyLong_AsSsize_t(len);
+    assert(!PyErr_Occurred());
+
+    self->len = int_len;
+    self->len_dirty = 0;
+
+    Py_DECREF(len);
+    return int_len;
+    fail:
+    Py_XDECREF(len);
+    return -1;
+}
+
+Py_ssize_t
+AtomicDict_Len(AtomicDict *self)
+{
+    Py_ssize_t len;
+    AtomicDict_BeginSynchronousOperation(self);
+    len = AtomicDict_Len_impl(self);
+    AtomicDict_EndSynchronousOperation(self);
+
+    return len;
+}
+
 PyObject *
 AtomicDict_Debug(AtomicDict *self)
 {
-    atomic_dict_meta meta;
-    meta = *(atomic_dict_meta *) AtomicRef_Get(self->metadata);
+    AtomicDict_Meta *meta = NULL;
+    meta = (AtomicDict_Meta *) AtomicRef_Get(self->metadata);
     PyObject *metadata = Py_BuildValue("{sOsOsOsOsOsOsOsOsOsOsOsOsO}",
-                                       "log_size\0", Py_BuildValue("B", meta.log_size),
-                                       "generation\0", Py_BuildValue("O", meta.generation),
-                                       "node_size\0", Py_BuildValue("B", meta.node_size),
-                                       "distance_size\0", Py_BuildValue("B", meta.distance_size),
-                                       "tag_size\0", Py_BuildValue("B", meta.tag_size),
-                                       "node_mask\0", Py_BuildValue("k", meta.node_mask),
-                                       "index_mask\0", Py_BuildValue("k", meta.index_mask),
-                                       "distance_mask\0", Py_BuildValue("k", meta.distance_mask),
-                                       "tag_mask\0", Py_BuildValue("k", meta.tag_mask),
-                                       "inserting_block\0", Py_BuildValue("l", meta.inserting_block),
-                                       "greatest_allocated_block\0", Py_BuildValue("l", meta.greatest_allocated_block),
-                                       "greatest_deleted_block\0", Py_BuildValue("l", meta.greatest_deleted_block),
-                                       "greatest_refilled_block\0", Py_BuildValue("l", meta.greatest_refilled_block));
+                                       "log_size\0", Py_BuildValue("B", meta->log_size),
+                                       "generation\0", Py_BuildValue("O", meta->generation),
+                                       "node_size\0", Py_BuildValue("B", meta->node_size),
+                                       "distance_size\0", Py_BuildValue("B", meta->distance_size),
+                                       "tag_size\0", Py_BuildValue("B", meta->tag_size),
+                                       "node_mask\0", Py_BuildValue("k", meta->node_mask),
+                                       "index_mask\0", Py_BuildValue("k", meta->index_mask),
+                                       "distance_mask\0", Py_BuildValue("k", meta->distance_mask),
+                                       "tag_mask\0", Py_BuildValue("k", meta->tag_mask),
+                                       "tombstone\0", Py_BuildValue("k", meta->tombstone.node),
+                                       "is_compact\0", Py_BuildValue("B", meta->is_compact),
+                                       "inserting_block\0", Py_BuildValue("l", meta->inserting_block),
+                                       "greatest_allocated_block\0", Py_BuildValue("l", meta->greatest_allocated_block),
+                                       "greatest_deleted_block\0", Py_BuildValue("l", meta->greatest_deleted_block),
+                                       "greatest_refilled_block\0", Py_BuildValue("l", meta->greatest_refilled_block));
     if (metadata == NULL)
         goto fail;
 
     PyObject *index_nodes = Py_BuildValue("[]");
     if (index_nodes == NULL)
         goto fail;
 
-    atomic_dict_node node;
-    for (uint64_t i = 0; i < (1 << meta.log_size); i++) {
-        AtomicDict_ReadNodeAt(i, &node, &meta);
+    AtomicDict_Node node;
+    for (uint64_t i = 0; i < meta->size; i++) {
+        AtomicDict_ReadNodeAt(i, &node, meta);
         PyObject *n = Py_BuildValue("k", node.node);
         if (n == NULL)
             goto fail;
         PyList_Append(index_nodes, n);
         Py_DECREF(n);
     }
 
     PyObject *blocks = Py_BuildValue("[]");
     if (blocks == NULL)
         goto fail;
 
-    atomic_dict_block *block;
+    AtomicDict_Block *block;
     PyObject *entries = NULL;
     PyObject *entry_tuple = NULL;
     PyObject *block_info = NULL;
-    for (uint64_t i = 0; i <= meta.greatest_allocated_block; i++) {
-        block = meta.blocks[i];
+    for (uint64_t i = 0; i <= meta->greatest_allocated_block; i++) {
+        block = meta->blocks[i];
         entries = Py_BuildValue("[]");
         if (entries == NULL)
             goto fail;
 
         for (int j = 0; j < 64; j++) {
             PyObject *key = block->entries[j].key;
+            PyObject *value = block->entries[j].value;
             if (key != NULL) {
-                PyObject *value = block->entries[j].value;
-                entry_tuple = Py_BuildValue("(BlOO)",
+                if (value == NULL) {
+                    value = PyExc_KeyError;
+                }
+                uint64_t entry_ix = (i << ATOMIC_DICT_LOG_ENTRIES_IN_BLOCK) + j;
+                entry_tuple = Py_BuildValue("(kBlOO)",
+                                            entry_ix,
                                             block->entries[j].flags,
                                             block->entries[j].hash,
                                             key,
                                             value);
                 if (entry_tuple == NULL)
                     goto fail;
                 Py_INCREF(key);
@@ -420,21 +627,23 @@
         PyList_Append(blocks, block_info);
         Py_DECREF(block_info);
     }
 
     PyObject *out = Py_BuildValue("{sOsOsO}", "meta\0", metadata, "blocks\0", blocks, "index\0", index_nodes);
     if (out == NULL)
         goto fail;
+    Py_DECREF(meta);
     Py_DECREF(metadata);
     Py_DECREF(blocks);
     Py_DECREF(index_nodes);
     return out;
 
     fail:
     PyErr_SetString(PyExc_RuntimeError, "unable to get debug info");
+    Py_XDECREF(meta);
     Py_XDECREF(metadata);
     Py_XDECREF(index_nodes);
     Py_XDECREF(blocks);
     Py_XDECREF(entries);
     Py_XDECREF(entry_tuple);
     Py_XDECREF(block_info);
     return NULL;
```

### Comparing `cereggii-0.1.1/src/cereggii/atomic_dict/node_ops.c` & `cereggii-0.2.0/src/cereggii/atomic_dict/node_ops.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,122 +1,228 @@
 // SPDX-FileCopyrightText: 2023-present dpdani <git@danieleparmeggiani.me>
 //
 // SPDX-License-Identifier: Apache-2.0
 
-#include <stdatomic.h>
-#include "atomic_dict.h"
 #include "atomic_dict_internal.h"
+#include "atomic_ops.h"
 
 // these functions take a pointer to meta, but to avoid multiple reads
 // you should dereference dk->meta (i.e. make a thread-local copy) and
 // then pass a reference to the copy to these functions instead.
 
 
 inline void
-AtomicDict_ComputeRawNode(atomic_dict_node *node, atomic_dict_meta *meta)
+AtomicDict_ComputeRawNode(AtomicDict_Node *node, AtomicDict_Meta *meta)
 {
-    assert(node->index < (1 << meta->log_size));
+    assert(node->index < meta->size);
     assert(node->distance <= meta->max_distance);
     node->node =
         (node->index << (meta->node_size - meta->log_size))
         | (meta->distance_mask - ((uint64_t) node->distance << (uint64_t) meta->tag_size))
         | (node->tag & meta->tag_mask);
 }
 
 inline int
-AtomicDict_NodeIsReservation(atomic_dict_node *node, atomic_dict_meta *meta)
+AtomicDict_NodeIsReservation(AtomicDict_Node *node, AtomicDict_Meta *meta)
 {
     return node->node != 0 && node->distance == (1 << meta->distance_size) - 1;
 }
 
+inline int
+AtomicDict_NodeIsTombstone(AtomicDict_Node *node, AtomicDict_Meta *meta)
+{
+    return node->node == meta->tombstone.node;
+}
+
 inline uint64_t
-AtomicDict_RegionOf(uint64_t ix, atomic_dict_meta *meta)
+AtomicDict_RegionOf(uint64_t ix, AtomicDict_Meta *meta)
 {
-    ix = ix % (1 << meta->log_size);
+    ix = ix & (meta->size - 1);
     return (ix & ~meta->shift_mask) / meta->nodes_in_region;
 }
 
 inline uint64_t
-AtomicDict_ShiftInRegionOf(uint64_t ix, atomic_dict_meta *meta)
+AtomicDict_ZoneOf(uint64_t ix, AtomicDict_Meta *meta)
+{
+    return AtomicDict_RegionOf(ix, meta) & (ULONG_MAX - 1UL);
+}
+
+#define UPPER_SEED 12923598712359872066ull
+#define LOWER_SEED 7467732452331123588ull
+#define REHASH(x) (uint64_t) (__builtin_ia32_crc32di((x), LOWER_SEED) | (__builtin_ia32_crc32di((x), UPPER_SEED) << 32))
+
+PyObject *
+AtomicDict_ReHash(AtomicDict *Py_UNUSED(self), PyObject *ob)
+{
+    Py_hash_t hash = PyObject_Hash(ob);
+    return PyLong_FromUnsignedLongLong(REHASH(hash));
+}
+
+inline uint64_t
+AtomicDict_Distance0Of(Py_hash_t hash, AtomicDict_Meta *meta)
+{
+    return REHASH(hash) >> meta->d0_shift;
+}
+
+inline uint64_t
+AtomicDict_ShiftInRegionOf(uint64_t ix, AtomicDict_Meta *meta)
 {
     return ix & meta->shift_mask;
 }
 
 inline uint8_t *
-AtomicDict_IndexAddressOf(uint64_t ix, atomic_dict_meta *meta)
+AtomicDict_IndexAddressOf(uint64_t ix, AtomicDict_Meta *meta)
 {
     uint64_t shift = AtomicDict_ShiftInRegionOf(ix, meta);
     uint64_t region = AtomicDict_RegionOf(ix, meta);
     return (uint8_t *) &meta->index[region] + shift * (meta->node_size / 8);
 }
 
 inline int
-AtomicDict_IndexAddressIsAligned(uint64_t ix, int alignment, atomic_dict_meta *meta)
+AtomicDict_IndexAddressIsAligned(uint64_t ix, int alignment, AtomicDict_Meta *meta)
 {
     return (int64_t) AtomicDict_IndexAddressOf(ix, meta) % alignment == 0;
 }
 
 inline void
-AtomicDict_ParseNodeFromRaw(uint64_t node_raw, atomic_dict_node *node,
-                            atomic_dict_meta *meta)
+AtomicDict_ParseNodeFromRaw(uint64_t node_raw, AtomicDict_Node *node,
+                            AtomicDict_Meta *meta)
 {
     node->node = node_raw;
     node->index = (node_raw & meta->index_mask) >> (meta->node_size - meta->log_size);
     node->distance = (~(node_raw & meta->distance_mask) & meta->distance_mask) >> meta->tag_size;
     node->tag = node_raw & meta->tag_mask;
 }
 
 
 inline void
-AtomicDict_ParseNodeFromRegion(uint64_t ix, uint64_t region, atomic_dict_node *node,
-                               atomic_dict_meta *meta)
+AtomicDict_ParseNodeFromRegion(uint64_t ix, uint64_t region, AtomicDict_Node *node,
+                               AtomicDict_Meta *meta)
 {
     uint64_t shift = AtomicDict_ShiftInRegionOf(ix, meta);
     uint64_t node_raw =
         (region & (meta->node_mask << (shift * meta->node_size))) >> (shift * meta->node_size);
     AtomicDict_ParseNodeFromRaw(node_raw, node, meta);
 }
 
-void
-AtomicDict_ReadNodeAt(uint64_t ix, atomic_dict_node *node, atomic_dict_meta *meta)
+inline uint64_t
+AtomicDict_ParseRawNodeFromRegion(uint64_t ix, uint64_t region, AtomicDict_Meta *meta)
+{
+    uint64_t shift = AtomicDict_ShiftInRegionOf(ix, meta);
+    uint64_t node_raw =
+        (region & (meta->node_mask << (shift * meta->node_size))) >> (shift * meta->node_size);
+    return node_raw;
+}
+
+inline void
+AtomicDict_CopyNodeBuffers(AtomicDict_Node *from_buffer, AtomicDict_Node *to_buffer)
+{
+    for (int i = 0; i < 16; ++i) {
+        to_buffer[i] = from_buffer[i];
+    }
+}
+
+inline void
+AtomicDict_ComputeBeginEndWrite(AtomicDict_Meta *meta, AtomicDict_Node *read_buffer, AtomicDict_Node *temp,
+                                int *begin_write, int *end_write)
+{
+    int j;
+    *begin_write = -1;
+    for (j = 0; j < meta->nodes_in_zone; ++j) {
+        AtomicDict_ComputeRawNode(&temp[j], meta);
+        if (temp[j].node != read_buffer[j].node) {
+            *begin_write = j;
+            break;
+        }
+    }
+    assert(*begin_write != -1);
+    *end_write = -1;
+    for (j = meta->nodes_in_zone - 1; j > *begin_write; --j) {
+        AtomicDict_ComputeRawNode(&temp[j], meta);
+        if (temp[j].node != read_buffer[j].node) {
+            *end_write = j + 1;
+            break;
+        }
+    }
+    if (*end_write == -1) {
+        *end_write = meta->nodes_in_zone;
+    }
+    assert(*end_write > *begin_write);
+
+    int n = *end_write - *begin_write;
+    int must_write = AtomicDict_MustWriteBytes(n, meta);
+    int must_write_nodes = must_write / (meta->node_size / 8);
+
+    if (n != must_write_nodes || !AtomicDict_IndexAddressIsAligned(*begin_write, n, meta)) {
+        // no need to check for alignment from the beginning of the index, since
+        // we already assume that begin_write = 0 is already 16-bytes aligned.
+
+        if (must_write_nodes == meta->nodes_in_zone) {
+            *begin_write = 0;
+            *end_write = meta->nodes_in_zone;
+        } else {
+            if (*begin_write <= meta->nodes_in_region && *end_write <= meta->nodes_in_region) {
+                *begin_write = 0;
+                *end_write = meta->nodes_in_region;
+            } else if (*begin_write >= meta->nodes_in_region && *end_write >= meta->nodes_in_region) {
+                *begin_write = meta->nodes_in_region;
+                *end_write = meta->nodes_in_zone;
+            } else {
+                // fallback to entire zone
+                *begin_write = 0;
+                *end_write = meta->nodes_in_zone;
+            }
+        }
+    }
+}
+
+inline void
+AtomicDict_ReadNodeAt(uint64_t ix, AtomicDict_Node *node, AtomicDict_Meta *meta)
 {
     uint64_t node_region = meta->index[AtomicDict_RegionOf(ix, meta)];
     AtomicDict_ParseNodeFromRegion(ix, node_region, node, meta);
 }
 
+inline int64_t
+AtomicDict_ReadRawNodeAt(uint64_t ix, AtomicDict_Meta *meta)
+{
+    uint64_t node_region = meta->index[AtomicDict_RegionOf(ix, meta)];
+    return (int64_t) AtomicDict_ParseRawNodeFromRegion(ix, node_region, meta);
+}
+
 /**
  * the following functions read more than one node at a time.
  * NB: they expect all the nodes to be in two successive words of memory!
  * this means that in order to call e.g. AtomicDict_Read8NodesAt,
  * meta->node_size must be at most 16.
  **/
 
 void
-AtomicDict_Read1NodeAt(uint64_t ix, atomic_dict_node *nodes, atomic_dict_meta *meta)
+AtomicDict_Read1NodeAt(uint64_t ix, AtomicDict_Node *nodes, AtomicDict_Meta *meta)
 {
     uint64_t node_region = meta->index[AtomicDict_RegionOf(ix, meta)];
     AtomicDict_ParseNodeFromRegion(ix, node_region, &nodes[0], meta);
 }
 
 void
-AtomicDict_Read2NodesAt(uint64_t ix, atomic_dict_node *nodes, atomic_dict_meta *meta)
+AtomicDict_Read2NodesAt(uint64_t ix, AtomicDict_Node *nodes, AtomicDict_Meta *meta)
 {
     uint64_t little = AtomicDict_RegionOf(ix, meta);
     uint64_t big = AtomicDict_RegionOf(ix + 1, meta);
     uint64_t node_region_little = meta->index[little];
     uint64_t node_region_big = node_region_little;
     if (big != little) {
         node_region_big = meta->index[big];
     }
     AtomicDict_ParseNodeFromRegion(ix, node_region_little, &nodes[0], meta);
     AtomicDict_ParseNodeFromRegion(ix + 1, node_region_big, &nodes[1], meta);
 }
 
 void
-AtomicDict_Read4NodesAt(uint64_t ix, atomic_dict_node *nodes, atomic_dict_meta *meta)
+AtomicDict_Read4NodesAt(uint64_t ix, AtomicDict_Node *nodes, AtomicDict_Meta *meta)
 {
     assert(meta->node_size <= 32);
     uint64_t little = AtomicDict_RegionOf(ix, meta);
     uint64_t middle = AtomicDict_RegionOf(ix + 2, meta);
     uint64_t big = AtomicDict_RegionOf(ix + 3, meta);
     uint64_t node_region_little = meta->index[little];
     uint64_t node_region_middle = node_region_little;
@@ -139,15 +245,15 @@
             region = node_region_big;
         }
         AtomicDict_ParseNodeFromRegion(ix + i, region, &nodes[i], meta);
     }
 }
 
 void
-AtomicDict_Read8NodesAt(uint64_t ix, atomic_dict_node *nodes, atomic_dict_meta *meta)
+AtomicDict_Read8NodesAt(uint64_t ix, AtomicDict_Node *nodes, AtomicDict_Meta *meta)
 {
     assert(meta->node_size <= 16);
     uint64_t little = AtomicDict_RegionOf(ix, meta);
     uint64_t middle = AtomicDict_RegionOf(ix + 4, meta);
     uint64_t big = AtomicDict_RegionOf(ix + 7, meta);
     uint64_t node_region_little = meta->index[little];
     uint64_t node_region_middle = node_region_little;
@@ -170,15 +276,15 @@
             region = node_region_big;
         }
         AtomicDict_ParseNodeFromRegion(ix + i, region, &nodes[i], meta);
     }
 }
 
 void
-AtomicDict_Read16NodesAt(uint64_t ix, atomic_dict_node *nodes, atomic_dict_meta *meta)
+AtomicDict_Read16NodesAt(uint64_t ix, AtomicDict_Node *nodes, AtomicDict_Meta *meta)
 {
     assert(meta->node_size == 8);
     uint64_t little = AtomicDict_RegionOf(ix, meta);
     uint64_t middle = AtomicDict_RegionOf(ix + 8, meta);
     uint64_t big = AtomicDict_RegionOf(ix + 15, meta);
     uint64_t node_region_little = meta->index[little];
     uint64_t node_region_middle = node_region_little;
@@ -200,29 +306,81 @@
         } else {
             region = node_region_big;
         }
         AtomicDict_ParseNodeFromRegion(ix + i, region, &nodes[i], meta);
     }
 }
 
+inline void
+AtomicDict_ReadNodesFromZoneIntoBuffer(uint64_t idx, AtomicDict_BufferedNodeReader *reader, AtomicDict_Meta *meta)
+{
+    idx &= (int64_t) (meta->size - 1);
+    uint64_t zone = AtomicDict_ZoneOf(idx, meta);
+
+    if (reader->zone != zone) {
+        meta->read_nodes_in_zone(idx, reader->buffer, meta);
+        reader->zone = (int64_t) zone;
+        reader->nodes_offset = (int) -(idx % meta->nodes_in_zone);
+    }
+
+    reader->idx_in_buffer = (int) (idx % meta->nodes_in_zone + reader->nodes_offset);
+    assert(reader->idx_in_buffer < meta->nodes_in_zone);
+    reader->node = reader->buffer[reader->idx_in_buffer];
+}
+
+inline void
+AtomicDict_ReadNodesFromZoneStartIntoBuffer(uint64_t idx, AtomicDict_BufferedNodeReader *reader,
+                                            AtomicDict_Meta *meta)
+{
+    AtomicDict_ReadNodesFromZoneIntoBuffer(idx / meta->nodes_in_zone * meta->nodes_in_zone,
+                                           reader, meta);
+    reader->idx_in_buffer = (int) (idx % meta->nodes_in_zone + reader->nodes_offset);
+    reader->node = reader->buffer[reader->idx_in_buffer];
+}
+
 
-int
-AtomicDict_WriteNodeAt(uint64_t ix, atomic_dict_node *node, atomic_dict_meta *meta)
+inline void
+AtomicDict_WriteNodeAt(uint64_t ix, AtomicDict_Node *node, AtomicDict_Meta *meta)
 {
     AtomicDict_ComputeRawNode(node, meta);
-    uint64_t shift = ix & meta->shift_mask;
+    AtomicDict_WriteRawNodeAt(ix, node->node, meta);
+}
+
+inline void
+AtomicDict_WriteRawNodeAt(uint64_t ix, uint64_t raw_node, AtomicDict_Meta *meta)
+{
+    assert(ix >= 0);
+    assert(ix < meta->size);
+
+    uint64_t shift = AtomicDict_ShiftInRegionOf(ix, meta);
+    assert(shift < meta->nodes_in_region);
     uint64_t region = AtomicDict_RegionOf(ix, meta);
-    uint64_t node_raw = meta->index[region];
-    node_raw &= ~(meta->node_mask << (shift * meta->node_size));
-    node_raw |= node->node << (shift * meta->node_size);
-    meta->index[region] = node_raw;
+    assert(region < meta->size / meta->nodes_in_region);
+    uint64_t *region_address = &meta->index[region];
+
+    switch (meta->node_size) {
+        case 8:
+            *((uint8_t *) region_address + shift) = raw_node;
+            break;
+        case 16:
+            *((uint16_t *) region_address + shift) = raw_node;
+            break;
+        case 32:
+            *((uint32_t *) region_address + shift) = raw_node;
+            break;
+        case 64:
+            *((uint64_t *) region_address + shift) = raw_node;
+            break;
+        default:
+            assert(0);
+    }
 }
 
 inline int
-AtomicDict_MustWriteBytes(int n, atomic_dict_meta *meta)
+AtomicDict_MustWriteBytes(int n, AtomicDict_Meta *meta)
 {
     int n_bytes = (meta->node_size >> 3) * n;
     assert(n_bytes <= 16);
     if (n_bytes == 1) {
         return 1;
     }
     if (n_bytes <= 2) {
@@ -230,68 +388,63 @@
     }
     if (n_bytes <= 4) {
         return 4;
     }
     if (n_bytes <= 8) {
         return 8;
     }
-    if (n_bytes <= 16) {
-        return 16;
-    }
-    assert(0);
+    return 16;
 }
 
-int
-AtomicDict_AtomicWriteNodesAt(uint64_t ix, int n, atomic_dict_node *expected, atomic_dict_node *new,
-                              atomic_dict_meta *meta)
+inline int
+AtomicDict_AtomicWriteNodesAt(uint64_t ix, int n, AtomicDict_Node *expected, AtomicDict_Node *desired,
+                              AtomicDict_Meta *meta)
 {
+    assert(ix >= 0);
+    assert(ix < meta->size);
+    assert(ix <= meta->size - n); // XXX implement index circular behavior
     assert(n > 0);
-    assert(n <= meta->nodes_in_two_regions);
-
+    assert(n <= meta->nodes_in_zone);
 
     uint64_t little = AtomicDict_RegionOf(ix, meta);
     uint64_t middle = AtomicDict_RegionOf(ix + n / 2, meta);
     uint64_t big = AtomicDict_RegionOf(ix + n - 1, meta);
     assert(little <= middle <= little + 1); // XXX implement index circular behavior
     assert(middle <= big <= middle + 1); // XXX implement index circular behavior
-    __uint128_t expected_raw = 0, new_raw = 0, node; // il bello sta nelle piccole cose
+    __uint128_t expected_raw = 0, desired_raw = 0, node; // il bello sta nelle piccole cose
     int i;
     for (i = 0; i < n; ++i) {
         AtomicDict_ComputeRawNode(&expected[i], meta);
-        AtomicDict_ComputeRawNode(&new[i], meta);
+        AtomicDict_ComputeRawNode(&desired[i], meta);
     }
     for (i = 0; i < n; ++i) {
         node = expected[i].node;
         node <<= meta->node_size * i;
         expected_raw |= node;
-        node = new[i].node;
+        node = desired[i].node;
         node <<= meta->node_size * i;
-        new_raw |= node;
+        desired_raw |= node;
     }
 
     int must_write = AtomicDict_MustWriteBytes(n, meta);
     int must_write_nodes = must_write / (meta->node_size / 8);
-    for (; i < must_write_nodes; ++i) {
-        node = expected[i].node;
-        node <<= meta->node_size * (meta->node_size - i - 1);
-        new_raw |= node;
-    }
+    assert(i == must_write_nodes);
 
     uint8_t *index_address = AtomicDict_IndexAddressOf(ix, meta);
     switch (must_write) {
         case 1:
-            return __sync_bool_compare_and_swap_1(index_address, expected_raw, new_raw);
+            return CereggiiAtomic_CompareExchangeUInt8(index_address, expected_raw, desired_raw);
         case 2:
-            return __sync_bool_compare_and_swap_2(index_address, expected_raw, new_raw);
+            return CereggiiAtomic_CompareExchangeUInt16((uint16_t *) index_address, expected_raw, desired_raw);
         case 4:
-            return __sync_bool_compare_and_swap_4(index_address, expected_raw, new_raw);
+            return CereggiiAtomic_CompareExchangeUInt32((uint32_t *) index_address, expected_raw, desired_raw);
         case 8:
-            return __sync_bool_compare_and_swap_8(index_address, expected_raw, new_raw);
+            return CereggiiAtomic_CompareExchangeUInt64((uint64_t *) index_address, expected_raw, desired_raw);
         case 16:
             // assert memory access is aligned
             // this is not required for <=8 bytes CAS on x86_64
             assert(AtomicDict_IndexAddressIsAligned(ix, 16, meta));
-            return __sync_bool_compare_and_swap_16(index_address, expected_raw, new_raw);
+            return CereggiiAtomic_CompareExchangeUInt128((__uint128_t *) index_address, expected_raw, desired_raw);
         default:
             assert(0);
     }
 }
```

### Comparing `cereggii-0.1.1/src/cereggii/atomic_dict/node_sizes_table.c` & `cereggii-0.2.0/src/cereggii/atomic_dict/node_sizes_table.c`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/src/cereggii/atomic_int/__init__.py` & `cereggii-0.2.0/src/cereggii/atomic_int/__init__.py`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/src/cereggii/atomic_int/atomic_int.c` & `cereggii-0.2.0/src/cereggii/atomic_int/atomic_int.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 // SPDX-FileCopyrightText: 2023-present dpdani <git@danieleparmeggiani.me>
 //
 // SPDX-License-Identifier: Apache-2.0
 
 #include "atomic_int.h"
 #include "atomic_int_internal.h"
+#include "atomic_ops.h"
 
 #include "pyhash.h"
 
 
 inline int
 AtomicInt_ConvertToCLongOrSetException(PyObject *py_integer /* borrowed */, int64_t *integer)
 {
@@ -111,15 +112,15 @@
     }
 
     return overflowed;
 }
 
 
 PyObject *
-AtomicInt_new(PyTypeObject *type, PyObject *args, PyObject *kwargs)
+AtomicInt_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwargs))
 {
     AtomicInt *self;
     self = (AtomicInt *) type->tp_alloc(type, 0);
 
     return (PyObject *) self;
 }
 
@@ -169,15 +170,15 @@
 }
 
 void
 AtomicInt_Set(AtomicInt *self, int64_t updated)
 {
     int64_t current = self->integer;
 
-    while (!_Py_atomic_compare_exchange_int64(&self->integer, current, updated)) {
+    while (!CereggiiAtomic_CompareExchangeInt64(&self->integer, current, updated)) {
         current = self->integer;
     }
 }
 
 PyObject *
 AtomicInt_Set_callable(AtomicInt *self, PyObject *py_integer)
 {
@@ -194,15 +195,15 @@
     fail:
     return NULL;
 }
 
 inline int
 AtomicInt_CompareAndSet(AtomicInt *self, int64_t expected, int64_t updated)
 {
-    return _Py_atomic_compare_exchange_int64(&self->integer, expected, updated);
+    return CereggiiAtomic_CompareExchangeInt64(&self->integer, expected, updated);
 }
 
 PyObject *
 AtomicInt_CompareAndSet_callable(AtomicInt *self, PyObject *args, PyObject *kwargs)
 {
     PyObject *py_expected;
     PyObject *py_updated;
@@ -225,15 +226,15 @@
         Py_RETURN_FALSE;
     }
 }
 
 inline int64_t
 AtomicInt_GetAndSet(AtomicInt *self, int64_t updated)
 {
-    return _Py_atomic_exchange_int64(&self->integer, updated);
+    return CereggiiAtomic_ExchangeInt64(&self->integer, updated);
 }
 
 PyObject *
 AtomicInt_GetAndSet_callable(AtomicInt *self, PyObject *args, PyObject *kwargs)
 {
     PyObject *py_integer = NULL;
     int64_t updated;
@@ -538,15 +539,15 @@
     fail:
     return NULL;
 }
 
 Py_hash_t
 AtomicInt_Hash(AtomicInt *self)
 {
-    return _Py_HashPointer(self);
+    return _Py_HashPointer(self); // this will be public in 3.13
 }
 
 inline PyObject *
 AtomicInt_Add(AtomicInt *self, PyObject *other)
 {
     PyObject *current = NULL;
```

### Comparing `cereggii-0.1.1/src/cereggii/atomic_int/handle.c` & `cereggii-0.2.0/src/cereggii/atomic_int/handle.c`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/src/cereggii/atomic_ref.c` & `cereggii-0.2.0/src/cereggii/atomic_ref.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 // SPDX-FileCopyrightText: 2023-present dpdani <git@danieleparmeggiani.me>
 //
 // SPDX-License-Identifier: Apache-2.0
 
 #include "atomic_ref.h"
+#include "atomic_ops.h"
 
 
 PyObject *
-AtomicRef_new(PyTypeObject *type, PyObject *args, PyObject *kwds)
+AtomicRef_new(PyTypeObject *type, PyObject *Py_UNUSED(args), PyObject *Py_UNUSED(kwds))
 {
     AtomicRef *self;
     self = (AtomicRef *) type->tp_alloc(type, 0);
     if (self != NULL) {
         self->reference = Py_None;
     }
     if (!PyObject_GC_IsTracked((PyObject *) self)) {
         PyObject_GC_Track(self);
     }
     return (PyObject *) self;
 }
 
 int
-AtomicRef_init(AtomicRef *self, PyObject *args, PyObject *kwargs)
+AtomicRef_init(AtomicRef *self, PyObject *args, PyObject *Py_UNUSED(kwargs))
 {
     PyObject *reference = NULL;
     if (args != NULL) {
         if (!PyArg_ParseTuple(args, "|O", &reference))
             goto fail;
     }
 
     if (reference != NULL) {
         Py_INCREF(reference);
+        // decref'ed in destructor
         self->reference = reference;
     }
-    // decref'ed in destructor
     return 0;
 
     fail:
     Py_XDECREF(reference);
     return -1;
 }
 
@@ -69,30 +70,31 @@
 AtomicRef_Set(AtomicRef *self, PyObject *reference)
 {
     assert(reference != NULL);
 
     PyObject *current_reference;
     current_reference = AtomicRef_Get(self);
     Py_INCREF(reference);
-    while (!_Py_atomic_compare_exchange_ptr(&self->reference, current_reference, reference)) {
+    while (!CereggiiAtomic_CompareExchangePtr((void **) &self->reference, current_reference, reference)) {
         Py_DECREF(current_reference);
         current_reference = AtomicRef_Get(self);
     }
-    Py_DECREF(current_reference);
+    Py_DECREF(current_reference);  // decrement for the AtomicRef_Get
+    Py_DECREF(current_reference);  // decrement because not holding it anymore
     Py_RETURN_NONE;
 }
 
 int
 AtomicRef_CompareAndSet(AtomicRef *self, PyObject *expected, PyObject *new)
 {
     assert(expected != NULL);
     assert(new != NULL);
 
     Py_INCREF(new);
-    int retval = _Py_atomic_compare_exchange_ptr(&self->reference, expected, new);
+    int retval = CereggiiAtomic_CompareExchangePtr((void **) &self->reference, expected, new);
     if (retval) {
         Py_DECREF(expected);
         return 1;
     } else {
         Py_DECREF(new);
         return 0;
     }
@@ -116,11 +118,11 @@
 }
 
 PyObject *AtomicRef_GetAndSet(AtomicRef *self, PyObject *new)
 {
     assert(new != NULL);
 
     Py_INCREF(new);
-    PyObject *current_reference = _Py_atomic_exchange_ptr(&self->reference, new);
+    PyObject *current_reference = CereggiiAtomic_ExchangePtr((void **) &self->reference, new);
     // don't decref current_reference: passing it to python
     return current_reference;
 }
```

### Comparing `cereggii-0.1.1/src/include/atomic_int.h` & `cereggii-0.2.0/src/include/atomic_int.h`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/src/include/atomic_int_internal.h` & `cereggii-0.2.0/src/include/atomic_int_internal.h`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/src/include/atomic_ref.h` & `cereggii-0.2.0/src/include/atomic_ref.h`

 * *Files identical despite different names*

### Comparing `cereggii-0.1.1/PKG-INFO` & `cereggii-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: cereggii
-Version: 0.1.1
-Summary: Concurrent threading utilities for Python
+Version: 0.2.0
+Summary: Thread synchronization utilities for free-threaded Python.
 Keywords: multithreading
 Author-email: dpdani <git@danieleparmeggiani.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Dist: build==1.0.3 ; extra == "dev"
 Requires-Dist: pytest==7.4.2 ; extra == "dev"
+Requires-Dist: pytest-reraise==2.1.2 ; extra == "dev"
 Requires-Dist: black==23.9.1 ; extra == "dev"
 Requires-Dist: ruff==0.0.292 ; extra == "dev"
 Project-URL: Documentation, https://github.com/dpdani/cereggii#readme
 Project-URL: Issues, https://github.com/dpdani/cereggii/issues
 Project-URL: Source, https://github.com/dpdani/cereggii
 Provides-Extra: dev
 
@@ -44,14 +45,17 @@
 _Image credits: Patrick Alexander, Peniocereus greggii var. greggii, south of Cooke's Range, Luna County, New Mexico, 10
 May 2018, CC0. [source](https://www.flickr.com/photos/aspidoscelis/42926986382)_
 
 ## Installing
 
 *This library is experimental*
 
+*Arm disclaimer:* `aarch64` processors are generally not supported, but this library was successfully used with Apple
+Silicon.
+
 Using [@colesbury's original nogil fork](https://github.com/colesbury/nogil?tab=readme-ov-file#installation) is required
 to use this library.
 You can get it with pyenv:
 
 ```shell
 pyenv install nogil-3.9.10-1
 ```
@@ -66,73 +70,59 @@
 see poor performance.
 
 ## AtomicInt
 
 In Python (be it free-threaded or not), the following piece of code is not thread-safe:
 
 ```python
-a = 0
-a += 1
+i = 0
+i += 1
 ```
 
-That is, if `a` is shared with multiple threads, and they attempt to modify `a`, the value of `a` after any
+That is, if `i` is shared with multiple threads, and they attempt to modify `i`, the value of `i` after any
 number (> 1) of writes, is undefined.
 
 The following piece of code is instead thread-safe:
 
 ```python
-a = cereggii.AtomicInt(0)
-a += 1
-```
-
-Also, consider the following piece of code:
-
-```python
-import threading
-
-
-class Spam:
-    def __init__(self):
-        self.counter = 0
-
-
-spam = Spam()
-print(f"{spam.counter=}")
+import cereggii
 
 
-def incr():
-    for i in range(1_000_000):
-        spam.counter += 1
-
-
-t1 = threading.Thread(target=incr)
-t2 = threading.Thread(target=incr)
-t1.start()
-t2.start()
-t1.join()
-t2.join()
-
-print(f"{spam.counter=}")
+i = cereggii.AtomicInt(0)
+i += 1
+print(i.get())
 ```
 
-The output you'll see onscreen is not known.
-If you subsititute `self.counter = 0` with `self.counter = AtomicInt(0)`, you'll be guaranteed to see
-`2_000_000`, and the program should run slightly faster.
-
-If you make an additional modification, your program will run much faster:
+Also, consider the [counter example](./examples/atomic_int/counter.py) where three counter implementations are compared:
 
-```python
-def incr():
-    h = spam.counter.get_handle()
-
-    for i in range(1_000_000):
-        h += 1
-```
+1. using a built-in `int`,
+2. using `AtomicInt`, and
+3. using `AtomicInt` with `AtomicIntHandle`.
 
-When using `AtomicIntHandle`, you should see your CPUs being fully used.
+```text
+A counter using the built-in int.
+spam.counter=0
+spam.counter=5019655
+Took 39.17 seconds.
+
+A counter using cereggii.AtomicInt.
+spam.counter.get()=0
+spam.counter.get()=15000000
+Took 36.78 seconds (1.07x faster).
+
+A counter using cereggii.AtomicInt and cereggii.AtomicIntHandle.
+spam.counter.get()=0
+spam.counter.get()=15000000
+Took 2.64 seconds (14.86x faster).
+```
+
+Notice that when using `AtomicInt` the count is correctly computed, and that using `AtomicInt.get_handle`
+to access the counter greatly improves performance.
+When using `AtomicIntHandle`, you should see your CPUs being fully used, because no implicit lock
+prevents the execution of any thread. [^implicitlock]
 
 `AtomicInt` borrows part of its API from Java's `AtomicInteger`, so that it should feel familiar to use, if you're
 coming to Python from Java.
 It also implements most numeric magic methods, so that it should feel comfortable to use for Pythonistas.
 It tries to mimic Python's `int` as close as possible, with some caveats:
 
 - it is bound to 64-bit integers, so you may encounter `OverflowError`;
@@ -147,104 +137,91 @@
     - `from_bytes`
     - `to_bytes`
     - `denominator`
     - `numerator`
     - `imag`
     - `real`
 
+[^implicitlock]: Put simply, in a free-threaded build,
+the [global interpreter lock](https://docs.python.org/3/glossary.html#term-global-interpreter-lock) is substituted with
+many per-object locks.
+
 [^1]: This behavior ensures the hashing property that identity implies hash equality.
 
 ### An explanation of these claims
 
 First, `a += 1` in CPython actually translates to more than one bytecode instruction, namely:
 
 ```text
-              0 LOAD_CONST               2 (1)
-              2 INPLACE_ADD              0 (a)
-              4 STORE_FAST               0 (a)
+LOAD_CONST               2 (1)
+INPLACE_ADD              0 (a)
+STORE_FAST               0 (a)
 ```
 
 This means that between the `INPLACE_ADD` and the `STORE_FAST` instructions, the value of `a` may have been changed by
 another thread, so that one or multiple increments may be lost.
 
 Second, the performance problem.
 How come the speedup?
 
-If we look again at the code, there are a couple of implicit memory locations which are being contended by threads:
+If we look again at [the example code](./examples/atomic_int/counter.py), there are a couple of implicit memory
+locations which are being contended by threads:
 
 1. the reference count of `spam.count`;
 2. the reference counts of the `int` objects themselves; and
 3. the lock protecting the implicit `spam.__dict__`.
 
 These contentions are eliminated by `AtomicInt`, cf.:
 
 1. `spam.count` is accessed indirectly through an `AtomicIntHandle` which avoids contention on its reference count (it
    is contended only during the `.get_handle()` call);
 2. this is avoided by not creating `int` objects during the increment;
-3. again, using the handle instead of the `AtomicInt` itself avoids spurious contention.
+3. again, using the handle instead of the `AtomicInt` itself avoids spurious contention, because `spam.__dict__` is not
+   modified.
 
 Also see colesbury/nogil#121.
 
 ## AtomicDict
 
-Currently, the implementation of `AtomicDict` is quite limited:
+You can see that there is some more performance to be gained by simply using `AtomicDict`, looking at the execution
+of [the count keys example](./examples/atomic_dict/count_keys.py).
+
+```text
+Counting keys using the built-in dict.
+Took 35.46 seconds.
 
-- (dpdani/cereggii#3) it can hold at most $2^{25}$ keys (~33.5M);
-- (dpdani/cereggii#4) it does not support deletions (`del d[k]`);
-- (dpdani/cereggii#5) it does not support dynamic resizing; and
-- several common functionalities are missing.
+Counting keys using cereggii.AtomicDict.
+Took 7.51 seconds (4.72x faster).
+```
 
-You can see that there is some more performance to be gained by simply using `AtomicDict`, comparing the following two
-programs.
+Notice that the performance gain was achieved by simply wrapping the dictionary initialization with `AtomicDict`
+(compare `Spam.d` and `AtomicSpam.d` in [the example source](./examples/atomic_dict/count_keys.py)).
 
 The usage of `AtomicInt` provides correctness, regardless of the hashmap implementation.
 But using `AtomicDict` instead of `dict` improves performance, even without using handles: writes to distinct keys do
 not generate contention.
 
-With `dict`:
-
-```python
-import threading
-
-from cereggii import AtomicDict, AtomicInt
-
+### Pre-sized dictionary, with partitioned iterations
 
-class Spam:
-    def __init__(self):
-        self.d = {k: AtomicInt(0) for k in range(10)}
+`AtomicDict` provides some more features compared to Python's `dict`, in
+the [partitioned iteration example](./examples/atomic_dict/partitioned_iter.py) two of them are shown:
 
+1. pre-sizing, which allows for the expensive dynamic resizing of a hash table to be avoided, and
+2. partitioned iterations, which allows to split the number of elements among threads.
 
-spam = Spam()
-print(
-    f"{spam.d[0].get()=} {spam.d[1].get()=} {spam.d[2].get()=} {spam.d[3].get()=} {spam.d[4].get()=} "
-    f"{spam.d[5].get()=} {spam.d[6].get()=} {spam.d[7].get()=} {spam.d[8].get()=} {spam.d[9].get()=} "
-)
-
-
-def incr():
-    keys = list(range(10))
-    for _ in range(5_000_000):
-        spam.d[keys[_ % len(keys)]] += 1
-
-
-threads = [threading.Thread(target=incr) for _ in range(3)]
-for t in threads:
-    t.start()
-
-for t in threads:
-    t.join()
-
-print(
-    f"{spam.d[0].get()=} {spam.d[1].get()=} {spam.d[2].get()=} {spam.d[3].get()=} {spam.d[4].get()=} "
-    f"{spam.d[5].get()=} {spam.d[6].get()=} {spam.d[7].get()=} {spam.d[8].get()=} {spam.d[9].get()=} "
-)
+```text
+Insertion into builtin dict took 36.81s
+Builtin dict iter took 17.56s with 1 thread.
+----------
+Insertion took 17.17s
+Partitioned iter took 8.80s with 1 threads.
+Partitioned iter took 5.03s with 2 threads.
+Partitioned iter took 3.92s with 3 threads.
 ```
 
-To use `AtomicDict`, substitute in `self.d = AtomicDict({k: AtomicInt(0) for k in range(10)})`.
-
 ## AtomicRef
 
 You can use an `AtomicRef` when you have a shared variable that points to an object, and you need to change the
 referenced object concurrently.
 
 This is not available in the Python standard library and was initially implemented as part of `AtomicDict`.
```

