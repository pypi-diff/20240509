# Comparing `tmp/adtoolbox-0.5.3.tar.gz` & `tmp/adtoolbox-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.5.3.tar", max compression
+gzip compressed data, was "adtoolbox-0.5.4.tar", max compression
```

## Comparing `adtoolbox-0.5.3.tar` & `adtoolbox-0.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      815 2024-05-08 17:32:14.704061 adtoolbox-0.5.3/README.md
--rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.3/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.3/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.3/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.3/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.3/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29972 2024-05-08 17:23:18.629590 adtoolbox-0.5.3/adtoolbox/cli.py
--rw-r--r--   0        0        0    16775 2024-05-08 19:38:40.864603 adtoolbox-0.5.3/adtoolbox/configs.py
--rw-r--r--   0        0        0   108578 2024-05-08 19:40:08.104097 adtoolbox-0.5.3/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.3/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.3/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.3/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.3/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.3/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.3/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.3/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.5.3/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.5.3/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.3/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.3/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.3/adtoolbox/tables.py
--rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.3/adtoolbox/utils.py
--rw-r--r--   0        0        0      748 2024-05-08 19:40:28.184427 adtoolbox-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4243 2024-05-08 19:40:31.678853 adtoolbox-0.5.3/setup.py
--rw-r--r--   0        0        0     1788 2024-05-08 19:40:31.679055 adtoolbox-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      909 2024-05-08 21:28:31.763577 adtoolbox-0.5.4/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.4/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.4/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.4/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.4/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.4/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.4/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16780 2024-05-09 02:48:46.366677 adtoolbox-0.5.4/adtoolbox/configs.py
+-rw-r--r--   0        0        0   108578 2024-05-08 19:40:08.104097 adtoolbox-0.5.4/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.4/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.4/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.4/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.4/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.4/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.4/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.4/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0     1123 2024-05-01 22:24:41.310110 adtoolbox-0.5.4/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0     1090 2023-01-24 23:43:30.618643 adtoolbox-0.5.4/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.4/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.4/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.4/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15931 2024-02-01 18:57:40.645825 adtoolbox-0.5.4/adtoolbox/utils.py
+-rw-r--r--   0        0        0      748 2024-05-09 02:49:45.988049 adtoolbox-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4338 2024-05-09 02:49:52.340999 adtoolbox-0.5.4/setup.py
+-rw-r--r--   0        0        0     1882 2024-05-09 02:49:52.341253 adtoolbox-0.5.4/PKG-INFO
```

### Comparing `adtoolbox-0.5.3/README.md` & `adtoolbox-0.5.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 
 Interested in trying ADToolbox? Run the notebooks on Binder or Colab:
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)
 <a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
+[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)
 
 ADToolbox comes with a detailed documentation website. You can access this website using the link below:
 
 ** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **
```

### Comparing `adtoolbox-0.5.3/adtoolbox/.DS_Store` & `adtoolbox-0.5.4/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/__init__.py` & `adtoolbox-0.5.4/adtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/adm.py` & `adtoolbox-0.5.4/adtoolbox/adm.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/bio_struct.py` & `adtoolbox-0.5.4/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/cli.py` & `adtoolbox-0.5.4/adtoolbox/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,17 +208,17 @@
         
         elif args.database_module=="show-feed-db":
             if args.filter:
                 t=db_class.get_feed_from_feed_db(field_name="name",field_value=args.filter)
             else:
                 t=db_class.get_feed_from_feed_db(field_name="name",query="")
             if t:
-                feed_table = Table(title="Feed Database",expand=True,safe_box=True)
+                feed_table = Table(title="Feed Database",safe_box=True,expand=True)
                 for i in t[0].to_dict().keys():
-                    feed_table.add_column(i, justify="center", style="cyan", no_wrap=True)
+                    feed_table.add_column(i, justify="center", style="cyan",max_width=20)
                 for i in t:
                     feed_table.add_row(*map(str,list(i.to_dict().values())))
                 console.print(feed_table)
     if args.ADToolbox_Module == 'Database' and "database_module" in args:
         if args.database_module=="initialize-metagenomics-studies-db":
             db_class.initialize_metagenomics_studies_db()
         elif args.database_module=="add-metagenomics-study":
```

### Comparing `adtoolbox-0.5.3/adtoolbox/configs.py` & `adtoolbox-0.5.4/adtoolbox/configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,18 @@
  	"seed_compound_url":"https://github.com/ModelSEED/ModelSEEDDatabase/raw/master/Biochemistry/compounds.json",
 	
 }
 
 INTERNAL_LINKS={
 	"protein_db_url":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Protein_DB.fasta",
 	"adtoolbox_rxn_db_url":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Reaction_Metadata.csv",
-	"feed_db_url":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Feed_DB.json",
+	"feed_db_url":"https://raw.githubusercontent.com/ParsaGhadermazi/Database/main/ADToolbox/feed_db.tsv",
 	"qiime_classifier_db_url":"https://data.qiime2.org/2022.11/common/silva-138-99-515-806-nb-classifier.qza",
 	"metagenomics_studies":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Kbase/metagenomics_studies.tsv",
-    "exmpermental_data_db":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Kbase/experimental_data_references.json"
+    "exmpermental_data_db":"https://github.com/ParsaGhadermazi/Database/blob/main/ADToolbox/experimental_data_references.json"
 }
 
 STUDIES_REMOTE={
 		"metagenomics_studies":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Kbase/metagenomics_studies.tsv",
     "exmpermental_data_db":"https://github.com/ParsaGhadermazi/Database/raw/main/ADToolbox/Kbase/experimental_data_references.json"
 }
```

### Comparing `adtoolbox-0.5.3/adtoolbox/core.py` & `adtoolbox-0.5.4/adtoolbox/core.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/metagenomics_report.py` & `adtoolbox-0.5.4/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/optimize.py` & `adtoolbox-0.5.4/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pipeline.py` & `adtoolbox-0.5.4/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.5.4/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.5.4/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.5.4/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/README.md` & `adtoolbox-0.5.4/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.5.4/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.5.4/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/stats.py` & `adtoolbox-0.5.4/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/tables.py` & `adtoolbox-0.5.4/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/adtoolbox/utils.py` & `adtoolbox-0.5.4/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.3/pyproject.toml` & `adtoolbox-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.5.3"
+version = "0.5.4"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.5.3/setup.py` & `adtoolbox-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
-    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
+    'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `adtoolbox-0.5.3/PKG-INFO` & `adtoolbox-0.5.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.5.3
+Version: 0.5.4
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -31,14 +31,15 @@
 
 Interested in trying ADToolbox? Run the notebooks on Binder or Colab:
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)
 <a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
+[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)
 
 ADToolbox comes with a detailed documentation website. You can access this website using the link below:
 
 ** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **
```

