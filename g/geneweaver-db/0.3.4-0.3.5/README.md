# Comparing `tmp/geneweaver_db-0.3.4.tar.gz` & `tmp/geneweaver_db-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.3.4.tar", max compression
+gzip compressed data, was "geneweaver_db-0.3.5.tar", max compression
```

## Comparing `geneweaver_db-0.3.4.tar` & `geneweaver_db-0.3.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-02 20:40:14.961223 geneweaver_db-0.3.4/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/README.md
--rw-r--r--   0        0        0      953 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     4802 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8651 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     4859 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     4785 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     3928 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1571 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1776 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3085 2024-05-02 20:40:14.965223 geneweaver_db-0.3.4/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/README.md
+-rw-r--r--   0        0        0      953 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     4802 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8651 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     4786 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     3928 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1571 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1776 2024-05-09 16:59:11.045205 geneweaver_db-0.3.5/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-09 16:59:11.049205 geneweaver_db-0.3.5/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-09 16:59:11.049205 geneweaver_db-0.3.5/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-09 16:59:11.049205 geneweaver_db-0.3.5/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3085 2024-05-09 16:59:11.049205 geneweaver_db-0.3.5/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 geneweaver_db-0.3.5/PKG-INFO
```

### Comparing `geneweaver_db-0.3.4/LICENSE` & `geneweaver_db-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/README.md` & `geneweaver_db-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/pyproject.toml` & `geneweaver_db-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.3.4"
+version = "0.3.5"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.3.5/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.3.5/src/geneweaver/db/aio/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.3.5/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.3.5/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.3.5/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.3.5/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.3.5/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/gene.py` & `geneweaver_db-0.3.5/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/geneset.py` & `geneweaver_db-0.3.5/src/geneweaver/db/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.3.5/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/publication.py` & `geneweaver_db-0.3.5/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/gene.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,30 @@
     "ode_ref_id": "reference_id",
     "gdb_id": "gene_database",
     "sp_id": "species",
     "ode_pref": "preferred",
     "ode_date": "date",
 }
 
+GENE_INFO_FIELDS_MAP = {
+    "gi_accession": "accession",
+    "gi_symbol": "symbol",
+    "gi_name": "name",
+    "gi_description": "description",
+    "gi_type": "type",
+    "gi_chromosome": "chromosome",
+    "gi_start_bp": "start_bp",
+    "gi_end_bp": "end_bp",
+    "gi_strand": "strand",
+    "sp_id": "species",
+    "gene_rank": "rank",
+}
+
 GENE_FIELDS = format_sql_fields(GENE_FIELDS_MAP, query_table="gene")
+GENE_INFO_FIELDS = format_sql_fields(GENE_INFO_FIELDS_MAP, query_table="gene_info")
 
 
 def get(
     gene_id: Optional[int] = None,
     reference_id: Optional[str] = None,
     gene_database: Optional[GeneIdentifier] = None,
     species: Optional[Species] = None,
@@ -37,15 +52,20 @@
     :param preferred: Whether to search for preferred genes.
     :param limit: The limit of results to return.
     :param offset: The offset of results to return.
 
     :return:  A query (and params) that can be executed on a cursor.
     """
     params = {}
-    query = SQL("SELECT") + SQL(",").join(GENE_FIELDS) + SQL("FROM gene")
+    query = (
+        SQL("SELECT")
+        + SQL(",").join(GENE_FIELDS + GENE_INFO_FIELDS)
+        + SQL("FROM gene JOIN gene_info")
+        + SQL("ON gene.ode_gene_id = gene_info.ode_gene_id")
+    )
 
     filtering = []
 
     if gene_id:
         filtering.append(SQL("ode_gene_id = %(gene_id)s"))
         params["gene_id"] = gene_id
```

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         {
             "gs_id": gs_id,
             "usr_id": owner_id,
             "sp_id": int(species) if species is not None else None,
             "gs_name": name,
             "gs_abbreviation": abbreviation,
             "pub_id": publication_id,
-            "publication.pubmed_id": pubmed_id,
+            "publication.pub_pubmed": pubmed_id,
             "gs_gene_id_type": int(gene_id_type) if gene_id_type is not None else None,
             "gs_status": status,
         },
     )
 
     if len(filtering) > 0:
         query += SQL("WHERE") + SQL("AND").join(filtering)
```

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/project.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/species.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.3.5/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/species.py` & `geneweaver_db-0.3.5/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/threshold.py` & `geneweaver_db-0.3.5/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/user.py` & `geneweaver_db-0.3.5/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/src/geneweaver/db/utils.py` & `geneweaver_db-0.3.5/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.3.4/PKG-INFO` & `geneweaver_db-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.3.4
+Version: 0.3.5
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

