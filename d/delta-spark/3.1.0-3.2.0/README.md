# Comparing `tmp/delta-spark-3.1.0.tar.gz` & `tmp/delta-spark-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-spark-3.1.0.tar", last modified: Fri Jan 26 22:56:15 2024, max compression
+gzip compressed data, was "dist/delta-spark-3.2.0.tar", last modified: Mon May  6 23:34:16 2024, max compression
```

## Comparing `delta-spark-3.1.0.tar` & `delta-spark-3.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        0 2024-01-26 22:56:15.848939 delta-spark-3.1.0/
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)    21864 2024-01-26 22:30:50.000000 delta-spark-3.1.0/LICENSE.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)      963 2024-01-26 22:30:50.000000 delta-spark-3.1.0/NOTICE.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     1930 2024-01-26 22:56:15.844939 delta-spark-3.1.0/PKG-INFO
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     9969 2024-01-26 22:30:50.000000 delta-spark-3.1.0/README.md
-drwxr-xr-x   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        0 2024-01-26 22:56:15.844939 delta-spark-3.1.0/python/
-drwxr-xr-x   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        0 2024-01-26 22:56:15.844939 delta-spark-3.1.0/python/delta/
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)      753 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/__init__.py
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)      870 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/_typing.py
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     5214 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/exceptions.py
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     3255 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/pip_utils.py
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        0 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/py.typed
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)    54376 2024-01-26 22:30:50.000000 delta-spark-3.1.0/python/delta/tables.py
-drwxr-xr-x   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        0 2024-01-26 22:56:15.844939 delta-spark-3.1.0/python/delta_spark.egg-info/
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     1930 2024-01-26 22:56:15.000000 delta-spark-3.1.0/python/delta_spark.egg-info/PKG-INFO
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)      397 2024-01-26 22:56:15.000000 delta-spark-3.1.0/python/delta_spark.egg-info/SOURCES.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        1 2024-01-26 22:56:15.000000 delta-spark-3.1.0/python/delta_spark.egg-info/dependency_links.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)       48 2024-01-26 22:56:15.000000 delta-spark-3.1.0/python/delta_spark.egg-info/requires.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)        6 2024-01-26 22:56:15.000000 delta-spark-3.1.0/python/delta_spark.egg-info/top_level.txt
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)       38 2024-01-26 22:56:15.848939 delta-spark-3.1.0/setup.cfg
--rw-r--r--   0 venkateshwar.korukanti  (1000) ubuntu    (1000)     2142 2024-01-26 22:30:50.000000 delta-spark-3.1.0/setup.py
+drwxr-xr-x   0 scott.sandre  (1000) ubuntu    (1000)        0 2024-05-06 23:34:16.000000 delta-spark-3.2.0/
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     2142 2024-05-06 22:20:06.000000 delta-spark-3.2.0/setup.py
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)    21864 2024-05-06 22:20:06.000000 delta-spark-3.2.0/LICENSE.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     9987 2024-05-06 22:20:06.000000 delta-spark-3.2.0/README.md
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)      963 2024-05-06 22:20:06.000000 delta-spark-3.2.0/NOTICE.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     1872 2024-05-06 23:34:16.000000 delta-spark-3.2.0/PKG-INFO
+drwxr-xr-x   0 scott.sandre  (1000) ubuntu    (1000)        0 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/
+drwxr-xr-x   0 scott.sandre  (1000) ubuntu    (1000)        0 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta/
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)        0 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/py.typed
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)      753 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/__init__.py
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)      870 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/_typing.py
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     5214 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/exceptions.py
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)    56056 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/tables.py
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     3255 2024-05-06 22:20:06.000000 delta-spark-3.2.0/python/delta/pip_utils.py
+drwxr-xr-x   0 scott.sandre  (1000) ubuntu    (1000)        0 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)        6 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/top_level.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)      397 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)     1872 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/PKG-INFO
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)        1 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)       48 2024-05-06 23:34:16.000000 delta-spark-3.2.0/python/delta_spark.egg-info/requires.txt
+-rw-r--r--   0 scott.sandre  (1000) ubuntu    (1000)       38 2024-05-06 23:34:16.000000 delta-spark-3.2.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `delta-spark-3.1.0/LICENSE.txt` & `delta-spark-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/NOTICE.txt` & `delta-spark-3.2.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/PKG-INFO` & `delta-spark-3.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: delta-spark
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python APIs for using Delta Lake with Apache Spark
 Home-page: https://github.com/delta-io/delta/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta
 Project-URL: Documentation, https://docs.delta.io/latest/index.html
 Project-URL: Issues, https://github.com/delta-io/delta/issues
 Keywords: delta.io
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: pyspark<3.6.0,>=3.5.0
-Requires-Dist: importlib_metadata>=1.0.0
 
 # Delta Lake
 
 [Delta Lake](https://delta.io) is an open source storage layer that brings reliability to data lakes. Delta Lake provides ACID transactions, scalable metadata handling, and unifies streaming and batch data processing. Delta Lake runs on top of your existing data lake and is fully compatible with Apache Spark APIs.
 
 This PyPi package contains the Python APIs for using Delta Lake with Apache Spark.
 
@@ -34,7 +33,9 @@
 
 1. Install using `pip install delta-spark`
 2. To use the Delta Lake with Apache Spark, you have to set additional configurations when creating the SparkSession. See the online [project web page](https://docs.delta.io/latest/delta-intro.html) for details.
 
 ## Documentation
 
 This README file only contains basic information related to pip installed Delta Lake. You can find the full documentation on the [project web page](https://docs.delta.io/latest/delta-intro.html)
+
+
```

### Comparing `delta-spark-3.1.0/README.md` & `delta-spark-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -123,19 +123,19 @@
 
 To execute tests, run
 
     build/sbt test
 
 To execute a single test suite, run
 
-    build/sbt 'testOnly org.apache.spark.sql.delta.optimize.OptimizeCompactionSuite'
+    build/sbt spark/'testOnly org.apache.spark.sql.delta.optimize.OptimizeCompactionSQLSuite'
 
 To execute a single test within and a single test suite, run
 
-    build/sbt 'testOnly *.OptimizeCompactionSuite -- -z "optimize command: on partitioned table - all partitions"'
+    build/sbt spark/'testOnly *.OptimizeCompactionSQLSuite -- -z "optimize command: on partitioned table - all partitions"'
 
 Refer to [SBT docs](https://www.scala-sbt.org/1.x/docs/Command-Line-Reference.html) for more commands.
 
 ## IntelliJ Setup
 
 IntelliJ is the recommended IDE to use when developing Delta Lake. To import Delta Lake as a new project:
 1. Clone Delta Lake into, for example, `~/delta`.
```

### Comparing `delta-spark-3.1.0/python/delta/__init__.py` & `delta-spark-3.2.0/python/delta/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/python/delta/_typing.py` & `delta-spark-3.2.0/python/delta/_typing.py`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/python/delta/exceptions.py` & `delta-spark-3.2.0/python/delta/exceptions.py`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/python/delta/pip_utils.py` & `delta-spark-3.2.0/python/delta/pip_utils.py`

 * *Files identical despite different names*

### Comparing `delta-spark-3.1.0/python/delta/tables.py` & `delta-spark-3.2.0/python/delta/tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
         :return: builder object to specify whether to update, delete or insert rows based on
                  whether the condition matched or not
         :rtype: :py:class:`delta.tables.DeltaMergeBuilder`
         """
         if source is None:
             raise ValueError("'source' in merge cannot be None")
-        elif type(source) is not DataFrame:
+        elif not isinstance(source, DataFrame):
             raise TypeError("Type of 'source' in merge must be DataFrame.")
         if condition is None:
             raise ValueError("'condition' in merge cannot be None")
 
         jbuilder = self._jdt.merge(source._jdf, DeltaTable._condition_to_jcolumn(condition))
         return DeltaMergeBuilder(self._spark, jbuilder)
 
@@ -389,17 +389,18 @@
 
     @classmethod
     @since(0.7)  # type: ignore[arg-type]
     def forName(
         cls, sparkSession: SparkSession, tableOrViewName: str
     ) -> "DeltaTable":
         """
-        Instantiate a :class:`DeltaTable` object using the given table or view name. If the given
+        Instantiate a :class:`DeltaTable` object using the given table name. If the given
         tableOrViewName is invalid (i.e. either no table exists or an existing table is not a
-        Delta table), it throws a `not a Delta table` error.
+        Delta table), it throws a `not a Delta table` error. Note: Passing a view name will
+        also result in this error as views are not supported.
 
         The given tableOrViewName can also be the absolute path of a delta datasource (i.e.
         delta.`path`), If so, instantiate a :class:`DeltaTable` object representing the data at
         the given path (consistent with the `forPath`).
 
         :param sparkSession: SparkSession to use for loading the table
         :param tableOrViewName: name of the table or view
@@ -1008,14 +1009,27 @@
         :param condition: Optional condition of the delete
         :type condition: str or pyspark.sql.Column
         :return: this builder
         """
         new_jbuilder = self.__getNotMatchedBySourceBuilder(condition).delete()
         return DeltaMergeBuilder(self._spark, new_jbuilder)
 
+    @since(3.2)  # type: ignore[arg-type]
+    def withSchemaEvolution(self) -> "DeltaMergeBuilder":
+        """
+        Enable schema evolution for the merge operation. This allows the target table schema to
+        be automatically updated based on the schema of the source DataFrame.
+
+        See :py:class:`~delta.tables.DeltaMergeBuilder` for complete usage details.
+
+        :return: this builder
+        """
+        new_jbuilder = self._jbuilder.withSchemaEvolution()
+        return DeltaMergeBuilder(self._spark, new_jbuilder)
+
     @since(0.4)  # type: ignore[arg-type]
     def execute(self) -> None:
         """
         Execute the merge operation based on the built matched and not matched actions.
 
         See :py:class:`~delta.tables.DeltaMergeBuilder` for complete usage details.
         """
@@ -1267,14 +1281,51 @@
                 self._raise_type_error("Partitioning column must be str.", [c])
         self._jbuilder = self._jbuilder.partitionedBy(_to_seq(
             self._spark._sc,  # type: ignore[attr-defined]
             cast(Iterable[Union[Column, str]], cols)
         ))
         return self
 
+    @overload
+    def clusterBy(
+        self, *cols: str
+    ) -> "DeltaTableBuilder":
+        ...
+
+    @overload
+    def clusterBy(
+        self, __cols: Union[List[str], Tuple[str, ...]]
+    ) -> "DeltaTableBuilder":
+        ...
+
+    @since(3.2)  # type: ignore[arg-type]
+    def clusterBy(
+        self, *cols: Union[str, List[str], Tuple[str, ...]]
+    ) -> "DeltaTableBuilder":
+        """
+        Specify columns for clustering
+
+        :param cols: the clustering cols
+        :type cols: str or list name of columns
+
+        :return: this builder
+
+        .. note:: Evolving
+        """
+        if len(cols) == 1 and isinstance(cols[0], (list, tuple)):
+            cols = cols[0]  # type: ignore[assignment]
+        for c in cols:
+            if type(c) is not str:
+                self._raise_type_error("Clustering column must be str.", [c])
+        self._jbuilder = self._jbuilder.clusterBy(_to_seq(
+            self._spark._sc,  # type: ignore[attr-defined]
+            cast(Iterable[Union[Column, str]], cols)
+        ))
+        return self
+
     @since(1.0)  # type: ignore[arg-type]
     def property(self, key: str, value: str) -> "DeltaTableBuilder":
         """
         Specify a table property
 
         :param key: the table property key
         :type value: the table property value
```

### Comparing `delta-spark-3.1.0/python/delta_spark.egg-info/PKG-INFO` & `delta-spark-3.2.0/python/delta_spark.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: delta-spark
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python APIs for using Delta Lake with Apache Spark
 Home-page: https://github.com/delta-io/delta/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta
 Project-URL: Documentation, https://docs.delta.io/latest/index.html
 Project-URL: Issues, https://github.com/delta-io/delta/issues
 Keywords: delta.io
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
-Requires-Dist: pyspark<3.6.0,>=3.5.0
-Requires-Dist: importlib_metadata>=1.0.0
 
 # Delta Lake
 
 [Delta Lake](https://delta.io) is an open source storage layer that brings reliability to data lakes. Delta Lake provides ACID transactions, scalable metadata handling, and unifies streaming and batch data processing. Delta Lake runs on top of your existing data lake and is fully compatible with Apache Spark APIs.
 
 This PyPi package contains the Python APIs for using Delta Lake with Apache Spark.
 
@@ -34,7 +33,9 @@
 
 1. Install using `pip install delta-spark`
 2. To use the Delta Lake with Apache Spark, you have to set additional configurations when creating the SparkSession. See the online [project web page](https://docs.delta.io/latest/delta-intro.html) for details.
 
 ## Documentation
 
 This README file only contains basic information related to pip installed Delta Lake. You can find the full documentation on the [project web page](https://docs.delta.io/latest/delta-intro.html)
+
+
```

### Comparing `delta-spark-3.1.0/setup.py` & `delta-spark-3.2.0/setup.py`

 * *Files identical despite different names*

