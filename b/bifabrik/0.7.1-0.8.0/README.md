# Comparing `tmp/bifabrik-0.7.1.tar.gz` & `tmp/bifabrik-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bifabrik-0.7.1.tar", max compression
+gzip compressed data, was "bifabrik-0.8.0.tar", max compression
```

## Comparing `bifabrik-0.7.1.tar` & `bifabrik-0.8.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
--rw-r--r--   0        0        0     1073 2024-04-28 22:11:01.170596 bifabrik-0.7.1/LICENSE
--rw-r--r--   0        0        0     4792 2024-04-28 22:11:01.170596 bifabrik-0.7.1/README.md
--rw-r--r--   0        0        0      575 2024-04-28 22:11:01.170596 bifabrik-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     6451 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/__init__.py
--rw-r--r--   0        0        0     2896 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/base/Pipeline.py
--rw-r--r--   0        0        0     1631 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/base/Task.py
--rw-r--r--   0        0        0     4899 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/CompleteConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/Configuration.py
--rw-r--r--   0        0        0      755 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/CsvSourceConfiguration.py
--rw-r--r--   0        0        0      570 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py
--rw-r--r--   0        0        0      525 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/DataSourceConfigurationBase.py
--rw-r--r--   0        0        0      729 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/ExcelSourceConfiguration.py
--rw-r--r--   0        0        0      715 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/JsonSourceConfiguration.py
--rw-r--r--   0        0        0      512 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py
--rw-r--r--   0        0        0      605 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/TableDestinationConfiguration.py
--rw-r--r--   0        0        0        0 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/__init__.py
--rw-r--r--   0        0        0     5045 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/engine/ConfigContainer.py
--rw-r--r--   0        0        0      411 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/engine/Configuration.py
--rw-r--r--   0        0        0     3895 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/CsvConfiguration.py
--rw-r--r--   0        0        0     2617 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
--rw-r--r--   0        0        0     4700 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/ExcelConfiguration.py
--rw-r--r--   0        0        0     2699 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py
--rw-r--r--   0        0        0     7254 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/JsonConfiguration.py
--rw-r--r--   0        0        0     3782 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/LogConfiguration.py
--rw-r--r--   0        0        0     2159 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
--rw-r--r--   0        0        0     2462 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/SecurityConfiguration.py
--rw-r--r--   0        0        0     2421 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
--rw-r--r--   0        0        0     4673 2024-04-28 22:11:01.170596 bifabrik-0.7.1/src/bifabrik/cfg/specific/TableConfiguration.py
--rw-r--r--   0        0        0      931 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/DataDestination.py
--rw-r--r--   0        0        0    13828 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/LakehouseTableDestination.py
--rw-r--r--   0        0        0      909 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/PandasDfDestination.py
--rw-r--r--   0        0        0      834 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/SparkDfDestination.py
--rw-r--r--   0        0        0    26211 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/WarehouseTableDestination.py
--rw-r--r--   0        0        0        0 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/dst/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/CsvSource.py
--rw-r--r--   0        0        0     3803 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/DataSource.py
--rw-r--r--   0        0        0     3925 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/ExcelSource.py
--rw-r--r--   0        0        0     3447 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/JsonSource.py
--rw-r--r--   0        0        0      919 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/PandasDfSource.py
--rw-r--r--   0        0        0     3588 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SharePointListSource.py
--rw-r--r--   0        0        0      914 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SparkDfSource.py
--rw-r--r--   0        0        0      941 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/SparkSqlSource.py
--rw-r--r--   0        0        0     3945 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/WarehouseSqlSource.py
--rw-r--r--   0        0        0        0 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/src/__init__.py
--rw-r--r--   0        0        0     3548 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/DataTransformation.py
--rw-r--r--   0        0        0     1086 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/PandasDfTransformation.py
--rw-r--r--   0        0        0      916 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/tsf/SparkDfTransformation.py
--rw-r--r--   0        0        0    15243 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/fsUtils.py
--rw-r--r--   0        0        0     7064 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/log.py
--rw-r--r--   0        0        0     2500 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/tableUtils.py
--rw-r--r--   0        0        0     6158 2024-04-28 22:11:01.174596 bifabrik-0.7.1/src/bifabrik/utils/tmslUtils.py
--rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 bifabrik-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-09 13:17:58.797451 bifabrik-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4678 2024-05-09 13:17:58.797451 bifabrik-0.8.0/README.md
+-rw-r--r--   0        0        0      575 2024-05-09 13:17:58.797451 bifabrik-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6451 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/__init__.py
+-rw-r--r--   0        0        0     2896 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/base/Pipeline.py
+-rw-r--r--   0        0        0     1798 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/base/Task.py
+-rw-r--r--   0        0        0     5285 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/CompleteConfiguration.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/Configuration.py
+-rw-r--r--   0        0        0      755 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/CsvSourceConfiguration.py
+-rw-r--r--   0        0        0      570 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py
+-rw-r--r--   0        0        0      525 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/DataSourceConfigurationBase.py
+-rw-r--r--   0        0        0      729 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/ExcelSourceConfiguration.py
+-rw-r--r--   0        0        0      715 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/JsonSourceConfiguration.py
+-rw-r--r--   0        0        0      512 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py
+-rw-r--r--   0        0        0      605 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/TableDestinationConfiguration.py
+-rw-r--r--   0        0        0      481 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/ValidationTransformationConfiguration.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/__init__.py
+-rw-r--r--   0        0        0     5626 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/engine/ConfigContainer.py
+-rw-r--r--   0        0        0      411 2024-05-09 13:17:58.797451 bifabrik-0.8.0/src/bifabrik/cfg/engine/Configuration.py
+-rw-r--r--   0        0        0     3895 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/CsvConfiguration.py
+-rw-r--r--   0        0        0     2617 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py
+-rw-r--r--   0        0        0     4700 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/ExcelConfiguration.py
+-rw-r--r--   0        0        0     2699 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py
+-rw-r--r--   0        0        0     7254 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/JsonConfiguration.py
+-rw-r--r--   0        0        0     3420 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/LogConfiguration.py
+-rw-r--r--   0        0        0     2154 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py
+-rw-r--r--   0        0        0     2457 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/SecurityConfiguration.py
+-rw-r--r--   0        0        0     2421 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py
+-rw-r--r--   0        0        0     5109 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/TableConfiguration.py
+-rw-r--r--   0        0        0     4280 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/cfg/specific/ValidationConfiguration.py
+-rw-r--r--   0        0        0      970 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/CommonDestinationUtils.py
+-rw-r--r--   0        0        0      379 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/DataDestination.py
+-rw-r--r--   0        0        0    14889 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/LakehouseTableDestination.py
+-rw-r--r--   0        0        0      909 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/PandasDfDestination.py
+-rw-r--r--   0        0        0      834 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/SparkDfDestination.py
+-rw-r--r--   0        0        0    29470 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/WarehouseTableDestination.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/dst/__init__.py
+-rw-r--r--   0        0        0     3916 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/CsvSource.py
+-rw-r--r--   0        0        0     4229 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/DataSource.py
+-rw-r--r--   0        0        0     3925 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/ExcelSource.py
+-rw-r--r--   0        0        0     3447 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/JsonSource.py
+-rw-r--r--   0        0        0      919 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/PandasDfSource.py
+-rw-r--r--   0        0        0     3588 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SharePointListSource.py
+-rw-r--r--   0        0        0      914 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SparkDfSource.py
+-rw-r--r--   0        0        0      941 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/SparkSqlSource.py
+-rw-r--r--   0        0        0     3945 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/WarehouseSqlSource.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/src/__init__.py
+-rw-r--r--   0        0        0     3918 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/DataTransformation.py
+-rw-r--r--   0        0        0     1086 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/PandasDfTransformation.py
+-rw-r--r--   0        0        0      916 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/SparkDfTransformation.py
+-rw-r--r--   0        0        0     5538 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/tsf/ValidationTransformation.py
+-rw-r--r--   0        0        0    16111 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/fsUtils.py
+-rw-r--r--   0        0        0     7064 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/log.py
+-rw-r--r--   0        0        0     5371 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/tableUtils.py
+-rw-r--r--   0        0        0     6158 2024-05-09 13:17:58.801451 bifabrik-0.8.0/src/bifabrik/utils/tmslUtils.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 bifabrik-0.8.0/PKG-INFO
```

### Comparing `bifabrik-0.7.1/LICENSE` & `bifabrik-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/README.md` & `bifabrik-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 
 > Consistent configuration is one of the core values of the project.
 > 
 > We like our lakehouses to be uniform in terms of loading patterns, table structures, tracking, etc. At the same time, we want to keep it [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
 > 
 > bifabrik configuration aims to cover many aspects of the lakehouse so that you can define your conventions once, use it repeatedly, and override when neccessary.
 
-See the [github page](https://rjankovic.github.io/bifabrik/tutorial/configuration.html) for more details on this.
 
 ### Spark SQL transformations
 Enough with the files! Let's make a simple Spark SQL transformation, writing data to another SQL table - a straightforward full load:
 
 ```python
 bif.fromSql('''
```

### Comparing `bifabrik-0.7.1/pyproject.toml` & `bifabrik-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bifabrik"
-version = "0.7.1"
+version = "0.8.0"
 description = "Microsoft Fabric ETL toolbox"
 authors = ["Radovan Jankovič"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rjankovic.github.io/bifabrik/"
 documentation = "https://rjankovic.github.io/bifabrik/"
 repository = "https://github.com/rjankovic/bifabrik/"
```

### Comparing `bifabrik-0.7.1/src/bifabrik/__init__.py` & `bifabrik-0.8.0/src/bifabrik/__init__.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/base/Pipeline.py` & `bifabrik-0.8.0/src/bifabrik/base/Pipeline.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/base/Task.py` & `bifabrik-0.8.0/src/bifabrik/base/Task.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,7 +48,13 @@
         """
         return self._pipeline.getTaskResult(self)
 
     def clearResults(self):
         self._result = None
         self._error = None
         self._completed = False
+
+    def run(self) -> any:
+        """Run the pipeline.
+        Returns the result of the last task, if any.
+        """
+        return self._pipeline.execute()
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/CompleteConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/CompleteConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 from bifabrik.cfg.specific.ExcelConfiguration import ExcelConfiguration
 from bifabrik.cfg.specific.FileSourceConfiguration import FileSourceConfiguration
 from bifabrik.cfg.specific.SourceStorageConfiguration import SourceStorageConfiguration
 from bifabrik.cfg.specific.DestinationStorageConfiguration import DestinationStorageConfiguration
 from bifabrik.cfg.specific.MetadataStorageConfiguration import MetadataStorageConfiguration
 from bifabrik.cfg.specific.TableConfiguration import TableConfiguration
 from bifabrik.cfg.specific.SecurityConfiguration import SecurityConfiguration
+from bifabrik.cfg.specific.ValidationConfiguration import ValidationConfiguration
 
 import notebookutils.mssparkutils.fs
 
 class CompleteConfiguration(ConfigContainer):
     """
     Fluent API for configuration
     
     You can set configuration directly through setter methods like .delimiter(';')[.further options...]
     or
     .option(name, value = None) gets / sets a named config property as in
     .option('delimiter', ';') #setter
     .option('delimiter') #getter
+
+    See https://rjankovic.github.io/bifabrik/tutorial/configuration.html for more examples
     """
     def __init__(self):
         self.__log = LogConfiguration()
         self.__csv = CsvConfiguration()
         self.__json = JsonConfiguration()
         self.__excel = ExcelConfiguration()
         self.__fileSource = FileSourceConfiguration()
         self.__sourceStorage = SourceStorageConfiguration()
         self.__destinationStorage = DestinationStorageConfiguration()
         self.__metadataStorage = MetadataStorageConfiguration()
         self.__destinationTable = TableConfiguration()
         self.__security = SecurityConfiguration()
+        self.__validation = ValidationConfiguration()
         super().__init__()
         
 
     @property
     def csv(self) -> CsvConfiguration:
         """CSV files settings"""
         return self.__csv
@@ -83,14 +87,19 @@
         "Destination table settings (increment method, identity column, etc.)"
         return self.__destinationTable
     
     @property
     def security(self) -> SecurityConfiguration:
         return self.__security
     
+    @property
+    def validation(self) -> ValidationConfiguration:
+        """Data validation configuration"""
+        return self.__validation
+    
     def serialize(self) -> str:
         """Serializes the configuration to a string"""
         res = {}
         rootAttribs = dir(self)
         noUnderscoreRootAttrNames = list(filter(lambda x: not x.startswith("_"), rootAttribs))
         for rootAttrName in noUnderscoreRootAttrNames:
             rootAttr = getattr(self, rootAttrName)
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/CsvSourceConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/CsvSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/DataDestinationConfigurationBase.py` & `bifabrik-0.8.0/src/bifabrik/cfg/DataDestinationConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/DataSourceConfigurationBase.py` & `bifabrik-0.8.0/src/bifabrik/cfg/DataSourceConfigurationBase.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/ExcelSourceConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/ExcelSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/JsonSourceConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/JsonSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/SharePointListSourceConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/SharePointListSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/TableDestinationConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/TableDestinationConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/engine/ConfigContainer.py` & `bifabrik-0.8.0/src/bifabrik/cfg/engine/ConfigContainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,32 +7,43 @@
         # to the Configuration objects
         self.__propDict = dict()
         self.setCfgOptions()
     
     def setterFactory(self, attrName):
         def directSetter(val):
             #print(f'DirectSetter: {str(self)} - set {attrName} to {val}')
-            self.option(attrName, val)
+            self.option(attrName, val, True)
             return self
         return directSetter
     
     def setCfgOptions(self):
         rootAttribs = dir(self)
         noUnderscoreRootAttrNames = list(filter(lambda x: not x.startswith("_"), rootAttribs))
         
+        
+        firstConfigAttr = True
+        for rootAttrName in noUnderscoreRootAttrNames:
+            rootAttr = getattr(self, rootAttrName)
+            attrType = type(rootAttr)
+            if attrType.__bases__[0].__name__ == 'Configuration':
+                if firstConfigAttr:
+                    self.__doc__ = (self.__doc__ or "") + \
+f'\nConfiguration parts (properties of this container):\n' + \
+'===================================================\n\t'
+                firstConfigAttr = False
+                self.__doc__ = self.__doc__ + f'{rootAttrName}:\t{rootAttr.__doc__}'
+
         # for adding config options from the partial configs
-        if self.__doc__ is None:
-            self.__doc__ = 'Configuration options:'
-        else:
-            self.__doc__ = self.__doc__ + '\n\nConfiguration options:'
+        self.__doc__ = self.__doc__ + '\n\nConfiguration options:\n' + '=======================\n'
 
         for rootAttrName in noUnderscoreRootAttrNames:
             rootAttr = getattr(self, rootAttrName)
             attrType = type(rootAttr)
             if attrType.__bases__[0].__name__ == 'Configuration':
+
                 cfgPropNames = dir(attrType)
                 for cfgpName in cfgPropNames:
                     cfgAttribute = getattr(attrType, cfgpName)
                     if isinstance(cfgAttribute, CfgProperty):
                         if cfgpName in self.__propDict:
                             matchingAttrTypes = list(filter(lambda x: str(type(x)) == str(type(rootAttr)), self.__propDict[cfgpName]))
                             if len(matchingAttrTypes) == 0:
@@ -55,25 +66,25 @@
                             setattr(self, cfgpName, directSetter)
 
                         # (don't use this - the __doc__ is in the type)
                         # instanceAttr = getattr(attr, cfgp)
                         self.__doc__ = (self.__doc__ or "") + f'\n{cfgpName}: {cfgAttribute.__doc__}\n'
 
        
-    def option(self, name, value = None):
+    def option(self, name, value = None, force_set = False):
         if not (name in self.__propDict):
             raise Exception(f'Configuration key not found: {name}.')
-        if value is None:
+        if value is None and not force_set:
             val = getattr(self.__propDict[name][0], name)
             return val
         #setattr(self.__propDict[name], name, value)
         for prop in self.__propDict[name]:
             setattr(prop, name, value)
         return self
-
+    
     def mergeToCopy(self, other):
         """Meges another configuration into this one; the 'other' config container takes priority.
         Returns a new configuration without affecting the original"""
         cp = self.copy()
         return cp.merge(other)
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/CsvConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/CsvConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/DestinationStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/ExcelConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/ExcelConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/FileSourceConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/FileSourceConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/JsonConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/JsonConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/LogConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/LogConfiguration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,12 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class LogConfiguration(Configuration):
     """Logging configuration
-
-    Examples
-    --------
-    > import bifabrik as bif
-    > from bifabrik.cfg.specific.LogConfiguration import LogConfiguration
-    > from bifabrik.utils import log
-    > 
-    > cfg = LogConfiguration()
-    > cfg.logPath = '/log.csv'
-    > cfg.errorLogPath = '/error_log.csv'
-    > cfg.loggingLevel = 'DEBUG'
-    > 
-    > log.configureLogger(cfg)
     """
     def __init__(self):
         self._explicitProps = {}
         self.__loggingEnabled = True
         self.__logLakehouse = None
         self.__logWorkspace = None
         self.__loggingLevel = 'INFO'
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/MetadataStorageConfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class MetadataStorageConfiguration(Configuration):
-    """Defines the data metadata lakehouse. By default refers to the default lakehouse of the notebook.
-    This is used for logs and metadata tables
+    """Defines the data metadata lakehouse. By default refers to the default lakehouse of the notebook. This is used for logs and metadata tables
     """
     def __init__(self):
         self._explicitProps = {}
         self.__metadataWorkspaceName = None
         self.__metadataLakehouseName = None
         self.__tmslBackupPathPattern = 'Files/tmsl_backup/{workspacename}/{datasetname}/{datasetname}_{timestamp}.json'
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/SecurityConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/SecurityConfiguration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bifabrik.cfg.engine.Configuration import Configuration
 from bifabrik.cfg.engine.Configuration import CfgProperty
 
 class SecurityConfiguration(Configuration):
-    """Credentials configuration, currently used for connecting to Fabric warehouses and the SharePointListSource.
-    (Passwords aren't actually stored here, this configuration only refers to KeyVault secrets.)
+    """Credentials configuration, currently used for connecting to Fabric warehouses and the SharePointListSource. (Passwords aren't actually stored here, this configuration only refers to KeyVault secrets.)
     """
     def __init__(self):
         self._explicitProps = {}
         self.__keyVaultUrl = None
         self.__loginKVSecretName = None
         self.__passwordKVSecretName = None
         self.__servicePrincipalClientId = None
```

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/SourceStorageConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/SourceStorageConfiguration.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/cfg/specific/TableConfiguration.py` & `bifabrik-0.8.0/src/bifabrik/cfg/specific/TableConfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         self.__increment = None
         self.__identityColumnPattern = None
         self.__insertDateColumn = None
         self.__mergeKeyColumns = []
         self.__snapshotKeyColumns = []
         self.__invalidCharactersInColumnNamesReplacement = '_'
         self.__canAddNewColumns = True
+        self.__addNARecord = False
 
     @CfgProperty
     def watermarkColumn(self) -> str:
         """Which column to use as the watermark when filtering records for incremental load.
         If the target table already exists and the watermark column is set, only records where the watermark is greater than the MAX from the table will be inserted.
         default None
         """
@@ -103,7 +104,17 @@
         """If the table already exists and the input dataset has extra columns, add the columns to the table with empty values before loading the new input.
         default True
         """
         return self.__canAddNewColumns
     @canAddNewColumns.setter(key='canAddNewColumns')
     def canAddNewColumns(self, val):
         self.__canAddNewColumns = val
+    
+    @CfgProperty
+    def addNARecord(self) -> bool:
+        """Add a dimension "N/A" record with identity -1, N/A for strings, 0 for numbers. identityColumnPattern needs to be configured when this is enabled.
+        default False
+        """
+        return self.__addNARecord
+    @addNARecord.setter(key='addNARecord')
+    def addNARecord(self, val):
+        self.__addNARecord = val
```

### Comparing `bifabrik-0.7.1/src/bifabrik/dst/LakehouseTableDestination.py` & `bifabrik-0.8.0/src/bifabrik/dst/LakehouseTableDestination.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #from pyspark.sql.functions import col
 from pyspark.sql.functions import *
 from pyspark.sql.window import Window
 import time
 import datetime
 import notebookutils.mssparkutils.fs
 from bifabrik.utils import tableUtils as tu
+import bifabrik.dst.CommonDestinationUtils as commons
 
 class LakehouseTableDestination(DataDestination, TableDestinationConfiguration):
     """Saves data to a lakehouse table.
 
     Examples
     --------
     > import bifabrik as bif
@@ -30,14 +31,15 @@
         self.__config = None
         self.__lhBasePath = None
         self.__identityColumn = None
         self.__insertDateColumn = None
         self.__tableExists = False
         self.__logger = None
         self.__tableLocation = None
+        self.__addNARecord = False
 
     def __str__(self):
         return f'Table destination: {self.__targetTableName}'
     
     def execute(self, input: DataFrame) -> None:
         lgr = lg.getLogger()
         self.__logger = lgr
@@ -63,27 +65,28 @@
         # print(f'insertDateColumn {self.__tableConfig.insertDateColumn}')
         # print(f'invalidCharactersInColumnNamesReplacement {self.__tableConfig.invalidCharactersInColumnNamesReplacement}')
 
         dstLh = mergedConfig.destinationStorage.destinationLakehouse
         dstWs = mergedConfig.destinationStorage.destinationWorkspace
         self.__lhBasePath = fsUtils.getLakehousePath(dstLh, dstWs)
         self.__lhMeta = fsUtils.getLakehouseMeta(dstLh, dstWs)
+        self.__addNARecord = self.__tableConfig.addNARecord
         self.__tableLocation = self.__lhBasePath + "/Tables/" + self.__targetTableName
         self.__tableExists = self.__tableExistsF()
 
-        self.__replaceInvalidCharactersInColumnNames()
-        self.__insertIdentityColumn()
-        self.__insertInsertDateColumn()
-
-
         incrementMethod = mergedConfig.destinationTable.increment
         if incrementMethod is None:
             incrementMethod = 'overwrite'
         self.__incrementMethod = incrementMethod
 
+        self.__replaceInvalidCharactersInColumnNames()
+        self.__insertIdentityColumn()
+        self.__insertInsertDateColumn()
+        self.__insertNARecord()
+
         self.__resolveSchemaDifferences()
         
         self.__filterByWatermark()
 
         # if the target target table does not exist yet, just handle it as an overwrite
         if not(self.__tableExists):
             self.__overwriteTarget()
@@ -160,14 +163,27 @@
             return
         
         self.__insertDateColumn = insertDateColumn
         ts = time.time()
         r = self.__data.withColumn(insertDateColumn, lit(ts).cast("timestamp"))
         self.__data = r
 
+    def __insertNARecord(self):
+        if not self.__addNARecord:
+            return
+        if self.__identityColumn is None:
+            raise Exception('Configuration error - when addNARecord is enabled, identityColumnPattern needs to be configured as well.')
+        if (not self.__tableExists) or (self.__incrementMethod in ['overwrite', 'overwrite', 'snapshot']):
+            self.__data = commons.addNARecord(self.__data, self._spark, self.__targetTableName, self.__identityColumn)
+            return
+        na_exists_sql = f'SELECT COUNT(*) FROM {self.__lhMeta.lakehouseName}.`{self.__targetTableName}` WHERE `{self.__identityColumn}` = -1'
+        na_exists = self._spark.sql(na_exists_sql).collect()[0][0]
+        if na_exists == 0:
+            self.__data = commons.addNARecord(self.__data, self._spark, self.__targetTableName, self.__identityColumn)
+
     def __overwriteTarget(self):
         self.__data.write.mode("overwrite").format("delta").option("overwriteSchema", "true").save(self.__tableLocation)
 
     def __appendTarget(self):
         self.__data.write.mode("append").format("delta").save(self.__tableLocation)
 
     def __resolveSchemaDifferences(self):
```

### Comparing `bifabrik-0.7.1/src/bifabrik/dst/PandasDfDestination.py` & `bifabrik-0.8.0/src/bifabrik/dst/PandasDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/dst/SparkDfDestination.py` & `bifabrik-0.8.0/src/bifabrik/dst/SparkDfDestination.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/dst/WarehouseTableDestination.py` & `bifabrik-0.8.0/src/bifabrik/dst/WarehouseTableDestination.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import time
 import datetime
 import notebookutils.mssparkutils.fs
 from bifabrik.utils import tableUtils as tu
 import uuid
 import pyodbc
 import pandas as pd
+import bifabrik.dst.CommonDestinationUtils as commons
 
 # reuse the table destination configuration
 class WarehouseTableDestination(DataDestination, TableDestinationConfiguration):
     """Saves data to a warehouse table. Uses pyodbc with service principal authentication, which needs to be configured.
     See https://rjankovic.github.io/bifabrik/tutorial/dst_warehouse_table.html
 
     Examples
@@ -52,14 +53,15 @@
         self.__insertDateColumn = None
         self.__tableExists = False
         self.__logger = None
         self.__tempTableName = None
         self.__tempTableLocation = None
         self.__odbcConnection = None
         self.__watermarkColumn = None
+        self.__addNARecord = False
 
     def __str__(self):
         return f'Warehouse table destination: [{self.__targetSchemaName}].[{self.__targetTableName}]'
     
     def execute(self, input: DataFrame) -> None:
         lgr = lg.getLogger()
         self.__logger = lgr
@@ -121,19 +123,21 @@
 
         tableCount = findTableDf[0][0]
         if tableCount == 0:
             self.__tableExists = False
         else:
             self.__tableExists = True
 
+
         # watermark filter filters self.__data DF - this has to be done before thedata is written to the lakehouse temp table
         self.__filterByWatermark()
         # the same replacement as in a lakehouse needs to be applied to the column in order to save the temp table to the lakehouse
         self.__replaceInvalidCharactersInColumnNames()
         
+
         # save to temp table in the lakehouse
         dstLh = mergedConfig.destinationStorage.destinationLakehouse
         dstWs = mergedConfig.destinationStorage.destinationWorkspace
         self.__lhBasePath = fsUtils.getLakehousePath(dstLh, dstWs)
         if self.__lhBasePath is None:
             raise Exception(f'''The warehouse destination needs to use a warehouse for temporary data storage. 
                             Either connect the notebook to a lakehouse or configure the destinationLakehouse and destinationWorkspace properties in bifabrik.config.destinationStorage.''')
@@ -190,40 +194,34 @@
         insertDateColumn = self.__tableConfig.insertDateColumn
         if insertDateColumn is not None:
             self.__insertDateColumn = insertDateColumn
             inputTableColumns.append([self.__insertDateColumn, 'DATETIME2(6)'])
         
         self.__tableColumns = inputTableColumns
         
-
         # create warehouse table if not exists        
         columnDefs = map(lambda x: f'{x[0]} {x[1]} NULL', inputTableColumns)
         column_defs_join = ',\n'.join(columnDefs)
         createTableSql = f'''
 CREATE TABLE [{self.__targetSchemaName}].[{self.__targetTableName}](
 {column_defs_join}
 )
 '''
-
         if not self.__tableExists:
             self.__execute_dml(createTableSql)
+            self.__insertNARecord()
             self.__append_target()
+            drop_temp_sql = f'DROP TABLE IF EXISTS `{self.__destinationLakehouse}`.`{self.__tempTableName}`'
+            self._spark.sql(drop_temp_sql)
             self.__odbcConnection.close()
             self._completed = True
             return
 
         # sync schema if table exists
-        origColumnsTypesDf = self.__execute_select(f'''
-SELECT s.name schema_name, t.name table_name, c.name column_name, tt.name type_name, tt.max_length, tt.precision, tt.scale 
-FROM sys.schemas s
-INNER JOIN sys.tables t ON s.schema_id = t.schema_id
-INNER JOIN sys.columns c ON c.object_id = t.object_id
-INNER JOIN sys.types tt ON tt.system_type_id = c.system_type_id
-WHERE s.name = '{self.__targetSchemaName}' AND t.name = '{self.__targetTableName}'
-        ''')
+        origColumnsTypesDf = self.__get_current_table_structure()
 
         consistent_changes = True
         schema_change = False
 
         if len(origColumnsTypesDf) < len(inputTableColumns):
             schema_change = True
 
@@ -325,15 +323,19 @@
             FROM [{self.__targetSchemaName}].[{whTempTableName}]
             '''
             self.__execute_dml(insertBackQuery)
 
             # DROP temp_old table
             dropQuery = f'DROP TABLE [{self.__targetSchemaName}].[{whTempTableName}]'
             self.__execute_dml(dropQuery)
-            
+        
+        if incrementMethod != 'overwrite':
+            # overwrite will handle it's N/A record by itself
+            self.__insertNARecord()
+
         # handle increments as in a lakehouse
         if incrementMethod == 'overwrite':
             self.__overwrite_target()
         elif incrementMethod == 'append':
             self.__append_target()
         elif incrementMethod == 'merge':
             self.__merge_taget()
@@ -371,19 +373,42 @@
                 self.__odbcConnection.commit()
             elif str(e.args[0]) == '42S02' and e.args[1].find('Invalid object name') > -1 and e.args[1].find('temp') > -1:
                 warn = 'Waiting 5 s for the lakehouse temp table to come online'
                 print(warn)
                 self.__logger.warning(e.args[1])
                 self.__logger.warning(warn)
                 time.sleep(5)
-                self.__odbcConnection.execute(query)
-                self.__odbcConnection.commit()
+                try:
+                    self.__odbcConnection.execute(query)
+                    self.__odbcConnection.commit()
+                except Exception as ee:
+                    if str(ee.args[0]) == '42000' and ee.args[1].find('the object accessed by the statement has been modified by a DDL statement in another concurrent transaction') > -1:
+                        warn = 'Waiting 5 s for blocking DDL to finish'
+                        print(warn)
+                        self.__logger.warning(ee.args[1])
+                        self.__logger.warning(warn)
+                        time.sleep(5)
+                        self.__odbcConnection.execute(query)
+                        self.__odbcConnection.commit()
+                    else:
+                        raise ee
             else:
                 raise e
 
+    def __get_current_table_structure(self):
+        df = self.__execute_select(f'''
+SELECT s.name schema_name, t.name table_name, c.name column_name, tt.name type_name, tt.max_length, tt.precision, tt.scale 
+FROM sys.schemas s
+INNER JOIN sys.tables t ON s.schema_id = t.schema_id
+INNER JOIN sys.columns c ON c.object_id = t.object_id
+INNER JOIN sys.types tt ON tt.system_type_id = c.system_type_id
+WHERE s.name = '{self.__targetSchemaName}' AND t.name = '{self.__targetTableName}'
+        ''')
+        return df
+    
     def __list_diff(self, first_list, second_list):
         diff = [item for item in first_list if item not in second_list]
         return diff
     
     # INSERT INTO destination_table(destination_columns) SELECT {destination_columns, including TS and ID} FROM src
     # [src] to be defined later
     def __create_insert_query(self):
@@ -422,21 +447,68 @@
         append_sql = f'''WITH
 src AS ({src_query}
 )
 {insert_query}
 '''
         self.__execute_dml(append_sql)
 
+    def __insertNARecord(self):        
+        self.__addNARecord = self.__tableConfig.addNARecord
+        if not self.__addNARecord:
+            return
+        if self.__identityColumn is None:
+            raise Exception('Configuration error - when addNARecord is enabled, identityColumnPattern needs to be configured as well.')
+                
+        # IF NOT EXISTS(SELECT TOP 1 1 FROM [dbo].[SurveyData] WHERE [SurveyDataID] = -1)
+        # BEGIN
+        #     INSERT INTO [dbo].[SurveyData] ([SurveyDataID], [Year], [Industry_aggregation_NZSIOC])
+        #     VALUES(-1, 0, 'N/A')
+        # END
+
+        columnsTypesDf = self.__get_current_table_structure()
+
+        insert_list = []
+        value_list = []
+
+        for c in columnsTypesDf:
+            col_name = c.column_name
+            col_type = c.type_name.upper()
+            insert_list.append(col_name)
+            if col_name == self.__identityColumn:
+                value_list.append('-1')
+            elif col_type in ['INT', 'BIGINT', 'SMALLINT', 'BIT']:
+                value_list.append('0')
+            elif col_type in ['REAL', 'FLOAT']:
+                value_list.append('0.0')
+            elif col_type in ['DATETIME', 'DATETIME2']:
+                value_list.append("'2000-01-01'")
+            elif col_type in ['VARCHAR', 'CHAR']:
+                value_list.append("'N/A'")
+        
+        insert_columns = list(map(lambda x: f'[{x}]', insert_list))
+        insert_columns_join = ", \n".join(insert_columns)
+        values_join = ", \n".join(value_list)
+
+        insert_query = f'''
+IF NOT EXISTS(SELECT TOP 1 1 FROM [{self.__targetSchemaName}].[{self.__targetTableName}] WHERE [{self.__identityColumn}] = -1)
+BEGIN
+    INSERT INTO [{self.__targetSchemaName}].[{self.__targetTableName}] ({insert_columns_join})
+    VALUES({values_join})
+END
+'''
+        self.__execute_dml(insert_query)
+    
     def __append_target(self):
         src_query = f'SELECT * FROM [{self.__destinationLakehouse}].[dbo].[{self.__tempTableName}]'
         self.__append_target_query(src_query)
     
     def __overwrite_target(self):
         delte_sql = f'DELETE FROM [{self.__targetSchemaName}].[{self.__targetTableName}]'
         self.__execute_dml(delte_sql)
+        self.__insertNARecord()
         self.__append_target()
     
     def __merge_taget(self):
         all_columns = list(map(lambda x: x[0], self.__tableColumns))
         key_columns = self.__tableConfig.mergeKeyColumns
         non_key_columns = self.__list_diff(self.__list_diff(all_columns, key_columns), [self.__identityColumn, self.__insertDateColumn])
         
@@ -445,22 +517,24 @@
         # print('non-key columns')
         # print(non_key_columns)
         
         if len(key_columns) == 0:
             raise Exception('No key columns set for merge increment. Please set the mergeKeyColumns property in destinationTable configuration to the list of column names.')
         
         join_condition = " AND ".join([f"src.[{item}] = tgt.[{item}]" for item in key_columns])
-        update_list = ",\n".join([f"tgt.[{item}] = src.[{item}]" for item in non_key_columns])
-        update_query = f'''
+        
+        if len(non_key_columns) > 0:
+            update_list = ",\n".join([f"tgt.[{item}] = src.[{item}]" for item in non_key_columns])
+            update_query = f'''
 UPDATE tgt SET
 {update_list}
 FROM [{self.__destinationLakehouse}].[dbo].[{self.__tempTableName}] src
 INNER JOIN [{self.__targetSchemaName}].[{self.__targetTableName}] tgt ON {join_condition}
 '''
-        self.__execute_dml(update_query)
+            self.__execute_dml(update_query)
 
         insert_src_query = f'''
 SELECT src.*
 FROM [{self.__destinationLakehouse}].[dbo].[{self.__tempTableName}] src
 LEFT JOIN [{self.__targetSchemaName}].[{self.__targetTableName}] tgt ON {join_condition}
 WHERE tgt.{key_columns[0]} IS NULL
 '''
```

### Comparing `bifabrik-0.7.1/src/bifabrik/src/CsvSource.py` & `bifabrik-0.8.0/src/bifabrik/src/CsvSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/DataSource.py` & `bifabrik-0.8.0/src/bifabrik/tsf/DataTransformation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 #from pyspark.sql.session import SparkSession
-from pyspark.sql.dataframe import DataFrame
 from bifabrik.dst.LakehouseTableDestination import LakehouseTableDestination
 from bifabrik.dst.WarehouseTableDestination import WarehouseTableDestination
 from bifabrik.dst.SparkDfDestination import SparkDfDestination
 from bifabrik.dst.PandasDfDestination import PandasDfDestination
-from bifabrik.tsf.DataTransformation import DataTransformation
-from bifabrik.tsf import SparkDfTransformation
-from bifabrik.tsf import PandasDfTransformation
 from bifabrik.base.Task import Task
+#from typing import Any, Self
 
-class DataSource(Task):
+class DataTransformation(Task):
     """Generic data source. 
-    Contains methods to initiate a DataDestination after you are done setting the source.
-    bif.sourceInit.sourceOption1(A).srcOpt2(B).toTable("Tab").destinationOption(X)....save()
+    Contains methods to initiate a DataDestination after you are done setting the transformation.
+    bif.sourceInit.sourceOption1(A).srcOpt2(B).transformation1(X).transformation2(Y).toTable("Tab").destinationOption(X)....run()
     """
     def __init__(self, parentPipeline):
         super().__init__(parentPipeline)
         
-
-    # def toDf(self) -> DataFrame:
-    #     """Converts the data to a spark dataframe
-    #     """
-    #     pass
-
     def toTable(self, targetTableName: str) -> LakehouseTableDestination:
         """Sets the lakehouse destination table name
         """
         return self.toLakehouseTable(targetTableName)
     
     def toLakehouseTable(self, targetTableName: str) -> LakehouseTableDestination:
         """Sets the lakehouse destination table name
@@ -60,25 +51,34 @@
         return dst
     
     def toSparkDf(self) -> SparkDfDestination:
         """Sets the destination as a Spark DF (for further processing)
         """
         dst = SparkDfDestination(self._pipeline)
         return dst
-    
+
     def toPandasDf(self) -> PandasDfDestination:
         """Sets the destination as a Pandas DF (for further processing)
         """
         dst = PandasDfDestination(self._pipeline)
         return dst
     
-    def transformSparkDf(self, func) -> SparkDfTransformation.SparkDfTransformation:
+    def transformSparkDf(self, func):
         """Applies the givet function to transform the data as a Spark DF
         """
-        tsf = SparkDfTransformation.SparkDfTransformation(self._pipeline, func)
+        from .SparkDfTransformation import SparkDfTransformation
+        tsf = SparkDfTransformation(self._pipeline, func)
         return tsf
     
-    def transformPandasDf(self, func) -> PandasDfTransformation.PandasDfTransformation:
+    def transformPandasDf(self, func):
         """Applies the givet function to transform the data as a Pandas DF
         """
-        tsf = PandasDfTransformation.PandasDfTransformation(self._pipeline, func)
+        from .PandasDfTransformation import PandasDfTransformation
+        tsf = PandasDfTransformation(self._pipeline, func)
+        return tsf
+        
+    def validate(self, testName = ''):
+        """Test the input data by checking the ValidationResult and ValidationMessage columns to determine if each row failed / passed the validation
+        """
+        from .ValidationTransformation import ValidationTransformation
+        tsf = ValidationTransformation(self._pipeline, testName)
         return tsf
```

### Comparing `bifabrik-0.7.1/src/bifabrik/src/ExcelSource.py` & `bifabrik-0.8.0/src/bifabrik/src/ExcelSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/JsonSource.py` & `bifabrik-0.8.0/src/bifabrik/src/JsonSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/PandasDfSource.py` & `bifabrik-0.8.0/src/bifabrik/src/PandasDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/SharePointListSource.py` & `bifabrik-0.8.0/src/bifabrik/src/SharePointListSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/SparkDfSource.py` & `bifabrik-0.8.0/src/bifabrik/src/SparkDfSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/SparkSqlSource.py` & `bifabrik-0.8.0/src/bifabrik/src/SparkSqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/src/WarehouseSqlSource.py` & `bifabrik-0.8.0/src/bifabrik/src/WarehouseSqlSource.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/tsf/PandasDfTransformation.py` & `bifabrik-0.8.0/src/bifabrik/tsf/PandasDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/tsf/SparkDfTransformation.py` & `bifabrik-0.8.0/src/bifabrik/tsf/SparkDfTransformation.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/utils/fsUtils.py` & `bifabrik-0.8.0/src/bifabrik/utils/fsUtils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import datetime
 import time
 
 __mounts = None
 __defaultWorkspaceId = spf.get_notebook_workspace_id()
 __defaultWorkspaceRefName = 'default'
 __defaultLakehouseId = None
+__defaultLakehouseWorkspaceId = None
 __defaultLakehouseRefName = 'default'
 #lgr = lg.getLogger()
 
 
 def normalizeFileApiPath(path: str):
     """Normalizes a file path to the form of "/lakehouse/default/Files/folder/..."
     """
@@ -280,14 +281,15 @@
 
 __workspaceMap = WorkspaceMap()
 
 defaultMount = getDefaultLakehouseAbfsPath()
 if defaultMount is not None:
     wsLh = getWorkspaceAndLakehouseIdFromMountSource(defaultMount)    
     __defaultLakehouseId = wsLh['lakehouseId']
+    __defaultLakehouseWorkspaceId = wsLh['workspaceId']
 
 def mapLakehouses(workspaceId: str, workspaceName: str):
     lm = LakehouseMap(workspaceId = workspaceId, workspaceName = workspaceName)
     #__workspaceMap.addWorkspace(lm)
     #print(workspaceId)
     #print(workspaceName)
     #print('----')
@@ -353,14 +355,16 @@
         lakehouse = __defaultLakehouseId
     if lakehouse == __defaultLakehouseRefName:
         lakehouse = __defaultLakehouseId
 
     errMsg = f'Could not find lakehouse {lakehouse} in workspace {workspace}'
 
     if lakehouse is None:
+        if suppressNotFound:
+            return None
         raise Exception(errMsg)
     
     lhMap = __workspaceMap[workspace]
     if lhMap is None:
         if suppressNotFound:
             return None
         raise Exception(errMsg)
@@ -368,14 +372,36 @@
     lh = lhMap[lakehouse]
     if lh is None:
         if suppressNotFound:
             return None
         raise Exception(errMsg)
     return lh
 
+def currentLakehouse() -> LakehouseMeta:
+    '''Info on the notebook's default (attached) lakehouse
+    '''
+    l =  getLakehouseMeta(lakehouse = __defaultLakehouseId, workspace = __defaultLakehouseWorkspaceId, suppressNotFound = True)
+    if l is None: 
+        return None
+    return {
+        'lakehouseName' : l.lakehouseName,
+        'lakehouseId' : l.lakehouseId,
+        'workspaceName' : l.workspaceName,
+        'workspaceId' : l.workspaceId,
+        'basePath' : l.basePath
+    } 
+
+def currentLakehouseName() -> str:
+    '''Name of the notebook's default (attached) lakehouse
+    '''
+    clh = currentLakehouse()
+    if clh is None:
+        return None
+    return clh['lakehouseName']
+
 def getLakehousePath(lakehouse: str, workspace: str = None, suppressNotFound = False, useImplicitDefaultLakehousePath = False):
     """
     Returns the lakehouse path as abfss://{workspace id}@onelake.dfs.fabric.microsoft.com/{lakehouse id}
     it can then be appended as e.g
         abfss://{workspace id}@onelake.dfs.fabric.microsoft.com/{lakehouse id}/Tables
         abfss://{workspace id}@onelake.dfs.fabric.microsoft.com/{lakehouse id}/Files
```

### Comparing `bifabrik-0.7.1/src/bifabrik/utils/log.py` & `bifabrik-0.8.0/src/bifabrik/utils/log.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/src/bifabrik/utils/tmslUtils.py` & `bifabrik-0.8.0/src/bifabrik/utils/tmslUtils.py`

 * *Files identical despite different names*

### Comparing `bifabrik-0.7.1/PKG-INFO` & `bifabrik-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bifabrik
-Version: 0.7.1
+Version: 0.8.0
 Summary: Microsoft Fabric ETL toolbox
 Home-page: https://rjankovic.github.io/bifabrik/
 License: MIT
 Author: Radovan Jankovič
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -99,15 +99,14 @@
 
 > Consistent configuration is one of the core values of the project.
 > 
 > We like our lakehouses to be uniform in terms of loading patterns, table structures, tracking, etc. At the same time, we want to keep it [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself).
 > 
 > bifabrik configuration aims to cover many aspects of the lakehouse so that you can define your conventions once, use it repeatedly, and override when neccessary.
 
-See the [github page](https://rjankovic.github.io/bifabrik/tutorial/configuration.html) for more details on this.
 
 ### Spark SQL transformations
 Enough with the files! Let's make a simple Spark SQL transformation, writing data to another SQL table - a straightforward full load:
 
 ```python
 bif.fromSql('''
```

