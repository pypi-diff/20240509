# Comparing `tmp/proksee_batch-0.6.2.tar.gz` & `tmp/proksee_batch-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proksee_batch-0.6.2.tar", max compression
+gzip compressed data, was "proksee_batch-0.6.3.tar", max compression
```

## Comparing `proksee_batch-0.6.2.tar` & `proksee_batch-0.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1089 2024-05-08 02:33:48.637018 proksee_batch-0.6.2/LICENSE
--rw-r--r--   0        0        0     3861 2024-05-08 02:33:48.637018 proksee_batch-0.6.2/README.md
--rw-r--r--   0        0        0     1817 2024-05-08 02:33:57.985105 proksee_batch-0.6.2/pyproject.toml
--rw-r--r--   0        0        0       21 2024-05-08 02:33:48.641018 proksee_batch-0.6.2/src/proksee_batch/__init__.py
--rw-r--r--   0        0        0    16864 2024-05-08 02:33:48.641018 proksee_batch-0.6.2/src/proksee_batch/__main__.py
--rw-r--r--   0        0        0     2330 2024-05-08 02:33:48.641018 proksee_batch-0.6.2/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
--rw-r--r--   0        0        0    22591 2024-05-08 02:33:48.641018 proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/batch.js
--rw-r--r--   0        0        0   208377 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/cgview.min.js
--rw-r--r--   0        0        0     1843 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/controls.js
--rw-r--r--   0        0        0   274269 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/d3.min.js
--rw-r--r--   0        0        0    61938 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
--rw-r--r--   0        0        0    14980 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/cgview.css
--rw-r--r--   0        0        0     5696 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/controls.css
--rw-r--r--   0        0        0    12170 2024-05-08 02:33:48.645018 proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/style.css
--rw-r--r--   0        0        0  8699885 2024-05-08 02:33:48.689018 proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_1.js
--rw-r--r--   0        0        0  8356605 2024-05-08 02:33:48.697018 proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_2.js
--rw-r--r--   0        0        0  9930491 2024-05-08 02:33:48.729018 proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_3.js
--rw-r--r--   0        0        0 12137099 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_4.js
--rw-r--r--   0        0        0     3874 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/data.example/table_data.js
--rw-r--r--   0        0        0   221376 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/default_proksee_template.json
--rw-r--r--   0        0        0      158 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
--rw-r--r--   0        0        0      269 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
--rw-r--r--   0        0        0      180 2024-05-08 02:33:48.765019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
--rw-r--r--   0        0        0       79 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
--rw-r--r--   0        0        0      134 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
--rw-r--r--   0        0        0       75 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
--rw-r--r--   0        0        0      130 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
--rw-r--r--   0        0        0       75 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
--rw-r--r--   0        0        0      130 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
--rw-r--r--   0        0        0     5127 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/data/report.html
--rw-r--r--   0        0        0     6474 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/download_example_input.py
--rw-r--r--   0        0        0      895 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/generate_proksee_link.py
--rw-r--r--   0        0        0     5311 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/generate_report_html.py
--rw-r--r--   0        0        0     1037 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/get_stats_from_seq_file.py
--rw-r--r--   0        0        0     1952 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/merge_cgview_json_with_template.py
--rw-r--r--   0        0        0    24085 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/parse_additional_features.py
--rw-r--r--   0        0        0        0 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/py.typed
--rw-r--r--   0        0        0     1165 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/remove_covered_features.py
--rw-r--r--   0        0        0     2658 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/scrape_proksee_image.py
--rw-r--r--   0        0        0    11471 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/seq_file_to_cgview_json.py
--rw-r--r--   0        0        0     6271 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/update_legend.py
--rw-r--r--   0        0        0    26801 2024-05-08 02:33:48.769019 proksee_batch-0.6.2/src/proksee_batch/validate_input_data.py
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 proksee_batch-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-08 21:42:05.888997 proksee_batch-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3861 2024-05-08 21:42:05.888997 proksee_batch-0.6.3/README.md
+-rw-r--r--   0        0        0     1817 2024-05-08 21:42:15.221007 proksee_batch-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/__init__.py
+-rw-r--r--   0        0        0    16864 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/__main__.py
+-rw-r--r--   0        0        0     2330 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png
+-rw-r--r--   0        0        0    22591 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/batch.js
+-rw-r--r--   0        0        0   208377 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/cgview.min.js
+-rw-r--r--   0        0        0     1843 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/controls.js
+-rw-r--r--   0        0        0   274269 2024-05-08 21:42:05.896997 proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/d3.min.js
+-rw-r--r--   0        0        0    61938 2024-05-08 21:42:05.900997 proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js
+-rw-r--r--   0        0        0    14980 2024-05-08 21:42:05.900997 proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/cgview.css
+-rw-r--r--   0        0        0     5696 2024-05-08 21:42:05.900997 proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/controls.css
+-rw-r--r--   0        0        0    12170 2024-05-08 21:42:05.900997 proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/style.css
+-rw-r--r--   0        0        0  8699885 2024-05-08 21:42:05.940997 proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_1.js
+-rw-r--r--   0        0        0  8356605 2024-05-08 21:42:05.952997 proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_2.js
+-rw-r--r--   0        0        0  9930491 2024-05-08 21:42:05.984997 proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_3.js
+-rw-r--r--   0        0        0 12137099 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_4.js
+-rw-r--r--   0        0        0     3874 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/data.example/table_data.js
+-rw-r--r--   0        0        0   221376 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/default_proksee_template.json
+-rw-r--r--   0        0        0      158 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/bed/e_coli_features.bed
+-rw-r--r--   0        0        0      269 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/blast/blast_against_e_coli.txt
+-rw-r--r--   0        0        0      180 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Escherichia_coli_str._K-12_substr._MG1655/vcf/e_coli_variants.vcf
+-rw-r--r--   0        0        0       79 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/bed/k_aerogenes_features.bed
+-rw-r--r--   0        0        0      134 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Klebsiella_aerogenes/blast/blast_against_k_aerogenes.txt
+-rw-r--r--   0        0        0       75 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/bed/s_enterica_features.bed
+-rw-r--r--   0        0        0      130 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Salmonella_enterica_subsp._enterica_serovar_Typhimurium_str._LT2/blast/blast_against_s_enterica.txt
+-rw-r--r--   0        0        0       75 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/bed/s_flexneri_features.bed
+-rw-r--r--   0        0        0      130 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/example_input_dir/Shigella_flexneri_2a_str._301/blast/blast_against_s_flexneri.txt
+-rw-r--r--   0        0        0     5127 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/data/report.html
+-rw-r--r--   0        0        0     6474 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/download_example_input.py
+-rw-r--r--   0        0        0      895 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/generate_proksee_link.py
+-rw-r--r--   0        0        0     5311 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/generate_report_html.py
+-rw-r--r--   0        0        0     1037 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/get_stats_from_seq_file.py
+-rw-r--r--   0        0        0     1952 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/merge_cgview_json_with_template.py
+-rw-r--r--   0        0        0    24085 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/parse_additional_features.py
+-rw-r--r--   0        0        0        0 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/py.typed
+-rw-r--r--   0        0        0     1165 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/remove_covered_features.py
+-rw-r--r--   0        0        0     2658 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/scrape_proksee_image.py
+-rw-r--r--   0        0        0    11471 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/seq_file_to_cgview_json.py
+-rw-r--r--   0        0        0     6566 2024-05-08 21:42:06.020997 proksee_batch-0.6.3/src/proksee_batch/update_legend.py
+-rw-r--r--   0        0        0    26801 2024-05-08 21:42:06.024997 proksee_batch-0.6.3/src/proksee_batch/validate_input_data.py
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 proksee_batch-0.6.3/PKG-INFO
```

### Comparing `proksee_batch-0.6.2/LICENSE` & `proksee_batch-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/README.md` & `proksee_batch-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/pyproject.toml` & `proksee_batch-0.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proksee-batch"
-version = "0.6.2"
+version = "0.6.3"
 description = "Proksee Batch"
 authors = ["Lael D. Barlow"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/stothard-group/proksee-batch"
 repository = "https://github.com/stothard-group/proksee-batch"
 documentation = "https://proksee-batch.readthedocs.io"
```

### Comparing `proksee_batch-0.6.2/src/proksee_batch/__main__.py` & `proksee_batch-0.6.3/src/proksee_batch/__main__.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/images/GitHub-Mark-Light-64px.png`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/batch.js` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/batch.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/cgview.min.js` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/cgview.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/controls.js` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/controls.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/d3.min.js` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/d3.min.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/scripts/svgcanvas.iife.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/cgview.css` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/cgview.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/controls.css` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/controls.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/assets/styles/style.css` & `proksee_batch-0.6.3/src/proksee_batch/data/assets/styles/style.css`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_1.js` & `proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_1.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_2.js` & `proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_2.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_3.js` & `proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_3.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/data.example/genome_maps/genome_4.js` & `proksee_batch-0.6.3/src/proksee_batch/data/data.example/genome_maps/genome_4.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/data.example/table_data.js` & `proksee_batch-0.6.3/src/proksee_batch/data/data.example/table_data.js`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/default_proksee_template.json` & `proksee_batch-0.6.3/src/proksee_batch/data/default_proksee_template.json`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/data/report.html` & `proksee_batch-0.6.3/src/proksee_batch/data/report.html`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/download_example_input.py` & `proksee_batch-0.6.3/src/proksee_batch/download_example_input.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/generate_proksee_link.py` & `proksee_batch-0.6.3/src/proksee_batch/generate_proksee_link.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/generate_report_html.py` & `proksee_batch-0.6.3/src/proksee_batch/generate_report_html.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/get_stats_from_seq_file.py` & `proksee_batch-0.6.3/src/proksee_batch/get_stats_from_seq_file.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/merge_cgview_json_with_template.py` & `proksee_batch-0.6.3/src/proksee_batch/merge_cgview_json_with_template.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/parse_additional_features.py` & `proksee_batch-0.6.3/src/proksee_batch/parse_additional_features.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/remove_covered_features.py` & `proksee_batch-0.6.3/src/proksee_batch/remove_covered_features.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/scrape_proksee_image.py` & `proksee_batch-0.6.3/src/proksee_batch/scrape_proksee_image.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/seq_file_to_cgview_json.py` & `proksee_batch-0.6.3/src/proksee_batch/seq_file_to_cgview_json.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/src/proksee_batch/update_legend.py` & `proksee_batch-0.6.3/src/proksee_batch/update_legend.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,46 +61,54 @@
             if track["dataKeys"].startswith(prefix + "_"):
                 # Use setdefault to initialize as a list if not already and append the track info.
                 additional_feature_tracks_by_type.setdefault(prefix, []).append(
                     track["name"]
                 )
                 break
 
+    # Get a list of all the additional feature track names (joined values from the dict).
+    all_additional_feature_track_names = set().union(
+        *additional_feature_tracks_by_type.values()
+    )
+
     # The track names for these additional features should be among the legend
     # item names.
-    for track_names in additional_feature_tracks_by_type.values():
-        for track_name in track_names:
-            assert (
-                track_name in all_legend_names
-            ), f"Track name '{track_name}' is not among the legend item names."
+    for track_name in all_additional_feature_track_names:
+        assert (
+            track_name in all_legend_names
+        ), f"Track name '{track_name}' is not among the legend item names."
 
     # The names_of_legend_items_to_leave_unmodified should not be among the
     # legend item names.
     for name in names_of_legend_items_to_leave_unmodified:
         assert (
             name not in all_legend_names
         ), f"Name '{name}' is among the legend item names."
 
     # Count the number of legend items that need to be assigned a color.
-    num_legends_to_color = len(all_legend_names) - len(
-        additional_feature_tracks_by_type.values()
-    )
+    num_legends_to_color = len(all_legend_names)
 
     # Set a default number of colors to use in a palette.
     default_num_colors = 12
 
     # Obtain a color palette of an appropriate length from Seaborn
     # (https://seaborn.pydata.org/tutorial/color_palettes.html).
     palette = sns.color_palette("husl", max(num_legends_to_color, default_num_colors))
 
+    ## Check that none of the legend names contain a comma.
+    # for legend_name in all_legend_names:
+    #    assert (
+    #        "," not in legend_name
+    #    ), f"Legend name '{legend_name}' contains a comma, which is not allowed."
+
     # Sort the legend names for additional feature tracks alphabetically, assign
     # them colors from the palette (starting from the beginning), and add
     # corresponding legend items to the legend.
     # Legend items should be of the form: {"name": "legend name here", "swatchColor": "rgba(0,0,0,1)", "decoration": "arc"}
-    for legend_name in sorted(additional_feature_tracks_by_type.values()):
+    for legend_name in sorted(all_additional_feature_track_names):
         color = palette.pop(0)
         cgview_map_json_data["cgview"]["legend"]["items"].append(
             {
                 "name": legend_name,
                 "swatchColor": f"rgba({int(color[0]*255)},{int(color[1]*255)},{int(color[2]*255)},1)",
                 "decoration": "arc",
             }
@@ -133,15 +141,15 @@
         )
 
     # For the remaining legend items, assign a color from the palette and add
     # corresponding legend items to the legend.
     remaining_legends = list(
         set(all_legend_names)
         - set(common_genbank_legend_names)
-        - set().union(*additional_feature_tracks_by_type.values())
+        - set(all_additional_feature_track_names)
     )
     for legend_name in remaining_legends:
         color = palette.pop(0)
         cgview_map_json_data["cgview"]["legend"]["items"].append(
             {
                 "name": legend_name,
                 "swatchColor": f"rgba({int(color[0]*255)},{int(color[1]*255)},{int(color[2]*255)},1)",
```

### Comparing `proksee_batch-0.6.2/src/proksee_batch/validate_input_data.py` & `proksee_batch-0.6.3/src/proksee_batch/validate_input_data.py`

 * *Files identical despite different names*

### Comparing `proksee_batch-0.6.2/PKG-INFO` & `proksee_batch-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proksee-batch
-Version: 0.6.2
+Version: 0.6.3
 Summary: Proksee Batch
 Home-page: https://github.com/stothard-group/proksee-batch
 License: MIT
 Author: Lael D. Barlow
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

