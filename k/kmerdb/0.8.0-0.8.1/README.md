# Comparing `tmp/kmerdb-0.8.0.tar.gz` & `tmp/kmerdb-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerdb-0.8.0.tar", last modified: Fri Apr 12 23:25:40 2024, max compression
+gzip compressed data, was "kmerdb-0.8.1.tar", last modified: Thu May  9 20:24:48 2024, max compression
```

## Comparing `kmerdb-0.8.0.tar` & `kmerdb-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.0/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.0/MANIFEST.in
--rw-r--r--   0 matt      (1000) matt      (1000)    26629 2024-04-12 23:25:40.515748 kmerdb-0.8.0/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    10606 2024-04-06 05:32:04.000000 kmerdb-0.8.0/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/kmerdb/
--rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.0/kmerdb/CITATION.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)   106771 2024-04-12 23:19:22.000000 kmerdb-0.8.0/kmerdb/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.0/kmerdb/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    33281 2024-04-12 23:22:03.000000 kmerdb-0.8.0/kmerdb/appmap.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.0/kmerdb/banners.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    13805 2024-04-12 23:22:17.000000 kmerdb-0.8.0/kmerdb/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)  1165266 2024-04-12 23:21:13.000000 kmerdb-0.8.0/kmerdb/distance.c
--rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.0/kmerdb/distance.pyx
--rw-rw-r--   0 matt      (1000) matt      (1000)    39346 2024-04-12 21:59:34.000000 kmerdb-0.8.0/kmerdb/fileutil.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    52230 2024-04-11 13:34:16.000000 kmerdb-0.8.0/kmerdb/graph.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.0/kmerdb/index.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-11 15:45:27.000000 kmerdb-0.8.0/kmerdb/kmer.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.0/kmerdb/legacy.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-12 23:09:24.000000 kmerdb-0.8.0/kmerdb/logger.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    19476 2024-04-12 01:25:50.000000 kmerdb-0.8.0/kmerdb/parse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.0/kmerdb/probability.py
--rw-r-----   0 matt      (1000) matt      (1000)     5632 2024-04-11 00:22:28.000000 kmerdb-0.8.0/kmerdb/python_distances.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.0/kmerdb/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/kmerdb.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    26629 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-04-12 23:25:40.000000 kmerdb-0.8.0/kmerdb.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4615 2024-04-12 23:16:02.000000 kmerdb-0.8.0/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-04-12 23:25:40.515748 kmerdb-0.8.0/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-04-12 23:15:53.000000 kmerdb-0.8.0/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-04-12 23:25:40.515748 kmerdb-0.8.0/test/
--rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.0/test/test_kmer.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.1/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.1/MANIFEST.in
+-rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-09 20:24:48.833375 kmerdb-0.8.1/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13884 2024-04-13 02:30:35.000000 kmerdb-0.8.1/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.829375 kmerdb-0.8.1/kmerdb/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.1/kmerdb/CITATION.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)   107575 2024-05-09 20:17:53.000000 kmerdb-0.8.1/kmerdb/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.1/kmerdb/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    59984 2024-05-09 20:21:21.000000 kmerdb-0.8.1/kmerdb/appmap.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.1/kmerdb/banners.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13805 2024-05-09 20:22:40.000000 kmerdb-0.8.1/kmerdb/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)  1166202 2024-05-09 20:18:07.000000 kmerdb-0.8.1/kmerdb/distance.c
+-rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.1/kmerdb/distance.pyx
+-rw-rw-r--   0 matt      (1000) matt      (1000)    40090 2024-05-08 05:07:56.000000 kmerdb-0.8.1/kmerdb/fileutil.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    53348 2024-05-08 05:01:16.000000 kmerdb-0.8.1/kmerdb/graph.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.1/kmerdb/index.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/kmer.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.1/kmerdb/legacy.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/logger.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    19969 2024-04-13 20:20:14.000000 kmerdb-0.8.1/kmerdb/parse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.1/kmerdb/probability.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5632 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/python_distances.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.1/kmerdb/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/kmerdb.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4635 2024-05-09 20:23:12.000000 kmerdb-0.8.1/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-05-09 20:24:48.833375 kmerdb-0.8.1/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-05-09 20:23:01.000000 kmerdb-0.8.1/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/test/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.1/test/test_kmer.py
```

### Comparing `kmerdb-0.8.0/LICENSE.txt` & `kmerdb-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/PKG-INFO` & `kmerdb-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -265,17 +265,17 @@
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
 Requires-Dist: sphinx>=4.3.2; extra == "dev"
 Requires-Dist: pytest>=5.3.5; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
-> A Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph databases
 
-NOTE: This project is in beta stage. Development is ongoing. But feel free to clone the repository and play with the code for yourself.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -286,121 +286,187 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-KDB is a Python library designed for bioinformatics applications. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts/abundances in a columnar format, with input file checksums, total counts, nullomers, and mononucleotide counts in a YAML formatted header in the first block of the `bgzf` formatted `.kdb` file. One restriction is that k-mers with unspecified sequence residues 'N' create gaps in the k-mer to sequence relationship space, and are excluded. That said, non-standard IUPAC residues are supported.
+k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
 
+`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
-The k-mer spectrum of the fasta or fastq sequencing data is stored in the `.kdb` format spec, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided to decompress a `.kdb` file into a standard output stream. The output file is compatible with `zlib`.
 
+## Usage
 
+```bash
+# Usage    --help option    --debug mode
+kmerdb --help # [+ --debug mode]
+kmerdb usage -m graph
+
+# Output:
+ o-O      |||
+o---O     |||             [|[          kmerdb           ]|]
+O---o     |||
+ O-o      |||        version :     v0.8.0
+  O       |||
+ o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
+o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
+O---o     |||      Website   : https://matthewralston.github.io/kmerdb
+ O-o      |||
+                                                                       lang :         python
+                                                                          v :      >= v3.7.4
+
+                      package manger : pip
+                        version      : >= 24.0
+        package root : /path2py/lib/python3.12/site-packages/kmerdb
+        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+
+                      required packages : 8
+                   development packages : 14
+
+           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+        
+...
+
+Beginning program...
+
+                          name : graph
+                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
+        
+
+* features
+
+- name: k-mer count arrays, linear, produced as file is read through sliding window.
+    (Un)compressed support for .fa/.fq.
+  shortname: parallel faux-OP sliding window k-mer shredding
+  description: Sequential k-mers from the input .fq|.fa files are added to the De
+    Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
+    (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
+    for the entire file are given for each file read, + a transparent data structure.
+		
+- name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
+  shortname: weighted undirected graph
+  description: an edge list of a De Bruijn graph is generated from all k-mers in the
+    forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
+    in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
+    graph and the edges provided by the data.
+
+
+
+
+* steps
+
+- name: read input file(s) from filesystem into k-mer arrays
+  shortname: shred inputs into k-mer count arrays
+  description: shred input sequences into k-mer count vector
+  
+- name: merge k-mer arrays and aggregate metadata
+  shortname: merge k-mer count arrays for aggregate metadata (header)
+  description: merge counts of nullomers, unique kmers, and total kmers.
+  
+- name: collate the weighted edge lists after reading multiple files. Output data
+    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
+  shortname: extract undirected weighted graph
+  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
+    edges, and the number of times the pair was observed from forward sequences in
+    the provided dataset
+	
+- name: print 'table' Final stats and close output file
+  shortname: metrics and shutdown
+  description: print final statistics, typically metadata values, and ensure file
+    is closed.
+
+
+
+
+#   +
+
+# [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
-## Installation
-
+# Create a [composite] profile of k-mer counts from sequence files. (.fasta|.fastq|.fa.gz|.fq.gz)
+kmerdb profile -k 8 example_1.fq.gz [example_2.fq.gz] profile_1.8.kdb
 
-### Dependencies
+# Build a weighted edge list (+ node ids/counts = De Bruijn graph)
+kmerdb graph -k 12 example_1.fq.gz example_2.fq.gz edges_1.kdbg
 
-DESeq2 is required as a R dependency for rpy2-mediated normalization.
+# View k-mer count vector
+kmerdb view profile_1.8.kdb # -H for full header
 
-```r
-if (!requireNamespace("BiocManager", quietly = TRUE))
-    install.packages("BiocManager")
+# Note: zlib compatibility
+#zcat profile_1.8.kdb
 
-BiocManager::install("DESeq2")
-```
+# View header (config.py[kdb_metadata_schema#L84])
+kmerdb header profile_1.8.kdb
 
-All other dependencies are managed directly by pip. 
+## Optional normalization, dim reduction, and distance matrix features:
 
+# K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+# 
+# kmerdb matrix DESeq2 *.8.kdb
+# kmerdb matrix PCA *.8.kdb
+# kmerdb matrix tSNE *.8.kdb
+#   # <pass> just makes a k-mer count matrix from k-mer count vectors.
+# 
+
+# Distances on count matrices [ SciPy ]  pdists + [ Cython ] Pearson correlation, scipy Spearman and scipy correlation pdist calculations are available ]
+kmerdb distance -h
+# 
+#
+# usage: kmerdb distance [-h] [-v] [--debug] [-l LOG_FILE] [--output-delimiter OUTPUT_DELIMITER] [-p PARALLEL] [--column-names COLUMN_NAMES] [--delimiter DELIMITER] [-k K]
+#                       {braycurtis,canberra,chebyshev,cityblock,correlation,cosine,dice,euclidean,hamming,jaccard,jensenshannon,kulsinski,mahalanobis,matching,minkowski,pearson,rogerstanimotorusselrao,seuclidean,sokalmichener,sokalsneath,spearman,sqeuclidean,yule} [<kdbfile1 kdbfile2 ...|input.tsv|STDIN> ...]
+
+# +
+
+#    Kmeans (sklearn, BioPython)
+kmerdb kmeans -k 4 -i dist.tsv
+#    BioPython Phylip tree + upgma
+kmerdb hierarchical -i dist.tsv
 
-### OSX and Linux release:
 
-```sh
-pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
+## Installation
 
-### Development installation:
+### OSX and Linux release:
 
 ```sh
-git clone https://github.com/MatthewRalston/kmerdb.git
-pip install .
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
-## Usage Example
+#### Optional DESeq2 normalization
 
-NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
+DESeq2 is an optional R dependency for rpy2-mediated normalization.
 
-<!-- ## NOTE: Temporary usage pattern:
-Migrating the repo from setup.py to the PEP606 standard PyProject.toml is borking my current invocation pattern. Sorry for the inconveniece... it's happening right now. -->
+```r
+if (!requireNamespace("BiocManager", quietly = TRUE))
+    install.packages("BiocManager")
 
-<!-- ```bash
-python -m kmerdb [cmd] [options]
+BiocManager::install("DESeq2")
 ```
 
-See `python -m kmerdb -h` for details.
--->
-
-## CLI Usage
-
-```bash
-kmerdb --help
-# Build a [composite] profile to a new .kdb file
-kmerdb profile -k 8 example1.fq.gz example2.fq.gz profile.8.kdb
-
-# Note: zlib compatibility
-zcat profile.8.kdb
-
-# Build a weighted edge list
-kmerdb graph -k 12 example1.fq.gz example2.fq.gz edges.kdbg
-
-# View the raw data
-kmerdb view profile.8.kdb # -H for full header
-
-# View the header
-kmerdb header profile.8.kdb
-
-# Collate the files. See 'kmerdb matrix -h' for more information.
-# Note: the 'pass' subcommand passes the int counts through collation, without normalization.
-# In this case the shell interprets '*.8.kdb' as all 8-mer profiles in the current working directory.
-# The k-mer profiles are read in parallel (-p $cores), and collated into one Pandas dataframe, which is printed to STDOUT.
-# Other options include DESeq2 normalization, frequency matrix, or PCA|tSNE based dimensionality reduction techniques.
-kmerdb matrix -p $cores pass *.8.kdb > kmer_count_dataframe.tsv
-
-# Calculate similarity between two (or more) profiles
-# The correlation distance from Numpy is used on one or more profiles, or piped output from 'kmerdb matrix'.
-kmerdb distance correlation profile1.kdb profile2.kdb (...) > distance.tsv
-
-# A condensed, one-line invocation of the matrix and distance command using the bash shell's pipe mechanism is as follows.
-kmerdb matrix pass *.8.kdb | kmerdb distance correlation STDIN > distance.tsv
-```
 
 ## IUPAC support:
 
 ```bash
 kmerdb profile -k $k input.fa output.kdb # This may discard non-IUPAC characters, this feature lacks documentation!
 ```
-IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting.
-
+IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting. Non-standard IUPAC residues are counted as doublets or triplets.
 
 
 ## Documentation
 
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
-Important features to usage that may be important may not be fully documented.
-
-For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing.
+Important features to usage that may be important may not be fully documented as the project is in beta.
 
-In addition, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
+For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
 Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
@@ -442,30 +508,42 @@
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
 
 ## Acknowledgements
 
-Thank you to the authors of kPAL and Jellyfish for the early inspiration. And thank you to others for the encouragement along the way, who shall remain nameless. I wanted this library to be a good strategy for assessing these k-mer profiles, in a way that is both cost aware of the analytical tasks at play, capable of storing the exact profiles in sync with the current assemblies, and then updating the kmer databases only when needed to generate enough spectral signature information.
+Thanks mom and dad and my hometown, awesome hs, and the University of Delaware faculty for support and encouragement. Thanks to my former mentors, bosses, and coworkers. It's been really enjoyable anticipating what the metagenomics community might want from a tool that can handle microbial k-mers well.
 
-The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on just this one project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+Thank you to the authors of kPAL and Jellyfish for the inspiration and bit shifting trick. And thank you to others for the encouragement along the way, who shall remain nameless. 
 
-More on the flip-side of this file. Literally. And figuratively. It's so complex with technology these days.
+The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on this project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+
+More on the flip-side. It's so complex with technology these days...
 
 <!--
-Thanks of course to that French girl from the children's series. 
+Thanks of course to my fans (and haters). Yeah i see you.... but i dont.
 Thanks to my former mentors BC, MR, IN, CR, and my newer bosses PJ and KL.
 Thanks to the Pap lab for the first dataset that I continue to use.
 Thank you to Ryan for the food and stuff. I actually made this project specifically so you and I could converse...
 Thanks to Blahah for tolerating someone snooping and imitating his Ruby style.
 Thanks to Erin for getting my feet wet in this new field. You are my mvp.
 Thanks to Rachel for the good memories and friendship. And Sophie too. veggies n' R love.
 Thanks to Yasmeen for the usual banter.
-Thanks to Max, Robin, and Robert for the good memories in St. Louis.
-Thanks to Freddy Miller for the good memories.
-Thanks to Nichole for the cookies and good memories. And your cute furballs too!
-Thanks to Stace for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
+Thanks to A for the newer banter.
+Thanks to Max, Robin, and Robert for the good memories in St. Louis. What's new?
+Thanks to Fred for the good memories.
+Thanks to Nichole for the cookies and good memories. And your cute furballs too! Hope you're well
+Thanks to S for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
 Thanks to a few friends I met in 2023 that reminded me I have a lot to learn about friendship, dating, and street smarts.
+Thanks to them even more now that I got it xd up.
+
+Thanks to the people of NCC for the Doordash money. It might not be much but I don't have it twisted (I do.)
+
+
+
+Thanks to D from BCCS.
+Thanks to C4H&H. I'm 'healthier' now, but I really still think I need more support than just BCCS. it's urgent.
+
 And thanks to my family and friends.
 Go Blue Hens
 -->
```

### Comparing `kmerdb-0.8.0/README.md` & `kmerdb-0.8.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # README - kmerdb
-> A Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph databases
 
-NOTE: This project is in beta stage. Development is ongoing. But feel free to clone the repository and play with the code for yourself.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -16,121 +16,187 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-KDB is a Python library designed for bioinformatics applications. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts/abundances in a columnar format, with input file checksums, total counts, nullomers, and mononucleotide counts in a YAML formatted header in the first block of the `bgzf` formatted `.kdb` file. One restriction is that k-mers with unspecified sequence residues 'N' create gaps in the k-mer to sequence relationship space, and are excluded. That said, non-standard IUPAC residues are supported.
+k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
 
+`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
-The k-mer spectrum of the fasta or fastq sequencing data is stored in the `.kdb` format spec, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided to decompress a `.kdb` file into a standard output stream. The output file is compatible with `zlib`.
 
+## Usage
 
+```bash
+# Usage    --help option    --debug mode
+kmerdb --help # [+ --debug mode]
+kmerdb usage -m graph
+
+# Output:
+ o-O      |||
+o---O     |||             [|[          kmerdb           ]|]
+O---o     |||
+ O-o      |||        version :     v0.8.0
+  O       |||
+ o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
+o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
+O---o     |||      Website   : https://matthewralston.github.io/kmerdb
+ O-o      |||
+                                                                       lang :         python
+                                                                          v :      >= v3.7.4
+
+                      package manger : pip
+                        version      : >= 24.0
+        package root : /path2py/lib/python3.12/site-packages/kmerdb
+        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+
+                      required packages : 8
+                   development packages : 14
+
+           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+        
+...
+
+Beginning program...
+
+                          name : graph
+                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
+        
+
+* features
+
+- name: k-mer count arrays, linear, produced as file is read through sliding window.
+    (Un)compressed support for .fa/.fq.
+  shortname: parallel faux-OP sliding window k-mer shredding
+  description: Sequential k-mers from the input .fq|.fa files are added to the De
+    Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
+    (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
+    for the entire file are given for each file read, + a transparent data structure.
+		
+- name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
+  shortname: weighted undirected graph
+  description: an edge list of a De Bruijn graph is generated from all k-mers in the
+    forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
+    in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
+    graph and the edges provided by the data.
+
+
+
+
+* steps
+
+- name: read input file(s) from filesystem into k-mer arrays
+  shortname: shred inputs into k-mer count arrays
+  description: shred input sequences into k-mer count vector
+  
+- name: merge k-mer arrays and aggregate metadata
+  shortname: merge k-mer count arrays for aggregate metadata (header)
+  description: merge counts of nullomers, unique kmers, and total kmers.
+  
+- name: collate the weighted edge lists after reading multiple files. Output data
+    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
+  shortname: extract undirected weighted graph
+  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
+    edges, and the number of times the pair was observed from forward sequences in
+    the provided dataset
+	
+- name: print 'table' Final stats and close output file
+  shortname: metrics and shutdown
+  description: print final statistics, typically metadata values, and ensure file
+    is closed.
+
+
+
+
+#   +
+
+# [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
-## Installation
-
+# Create a [composite] profile of k-mer counts from sequence files. (.fasta|.fastq|.fa.gz|.fq.gz)
+kmerdb profile -k 8 example_1.fq.gz [example_2.fq.gz] profile_1.8.kdb
 
-### Dependencies
+# Build a weighted edge list (+ node ids/counts = De Bruijn graph)
+kmerdb graph -k 12 example_1.fq.gz example_2.fq.gz edges_1.kdbg
 
-DESeq2 is required as a R dependency for rpy2-mediated normalization.
+# View k-mer count vector
+kmerdb view profile_1.8.kdb # -H for full header
 
-```r
-if (!requireNamespace("BiocManager", quietly = TRUE))
-    install.packages("BiocManager")
+# Note: zlib compatibility
+#zcat profile_1.8.kdb
 
-BiocManager::install("DESeq2")
-```
+# View header (config.py[kdb_metadata_schema#L84])
+kmerdb header profile_1.8.kdb
 
-All other dependencies are managed directly by pip. 
+## Optional normalization, dim reduction, and distance matrix features:
 
+# K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+# 
+# kmerdb matrix DESeq2 *.8.kdb
+# kmerdb matrix PCA *.8.kdb
+# kmerdb matrix tSNE *.8.kdb
+#   # <pass> just makes a k-mer count matrix from k-mer count vectors.
+# 
+
+# Distances on count matrices [ SciPy ]  pdists + [ Cython ] Pearson correlation, scipy Spearman and scipy correlation pdist calculations are available ]
+kmerdb distance -h
+# 
+#
+# usage: kmerdb distance [-h] [-v] [--debug] [-l LOG_FILE] [--output-delimiter OUTPUT_DELIMITER] [-p PARALLEL] [--column-names COLUMN_NAMES] [--delimiter DELIMITER] [-k K]
+#                       {braycurtis,canberra,chebyshev,cityblock,correlation,cosine,dice,euclidean,hamming,jaccard,jensenshannon,kulsinski,mahalanobis,matching,minkowski,pearson,rogerstanimotorusselrao,seuclidean,sokalmichener,sokalsneath,spearman,sqeuclidean,yule} [<kdbfile1 kdbfile2 ...|input.tsv|STDIN> ...]
+
+# +
+
+#    Kmeans (sklearn, BioPython)
+kmerdb kmeans -k 4 -i dist.tsv
+#    BioPython Phylip tree + upgma
+kmerdb hierarchical -i dist.tsv
 
-### OSX and Linux release:
 
-```sh
-pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
+## Installation
 
-### Development installation:
+### OSX and Linux release:
 
 ```sh
-git clone https://github.com/MatthewRalston/kmerdb.git
-pip install .
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
-## Usage Example
+#### Optional DESeq2 normalization
 
-NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
+DESeq2 is an optional R dependency for rpy2-mediated normalization.
 
-<!-- ## NOTE: Temporary usage pattern:
-Migrating the repo from setup.py to the PEP606 standard PyProject.toml is borking my current invocation pattern. Sorry for the inconveniece... it's happening right now. -->
+```r
+if (!requireNamespace("BiocManager", quietly = TRUE))
+    install.packages("BiocManager")
 
-<!-- ```bash
-python -m kmerdb [cmd] [options]
+BiocManager::install("DESeq2")
 ```
 
-See `python -m kmerdb -h` for details.
--->
-
-## CLI Usage
-
-```bash
-kmerdb --help
-# Build a [composite] profile to a new .kdb file
-kmerdb profile -k 8 example1.fq.gz example2.fq.gz profile.8.kdb
-
-# Note: zlib compatibility
-zcat profile.8.kdb
-
-# Build a weighted edge list
-kmerdb graph -k 12 example1.fq.gz example2.fq.gz edges.kdbg
-
-# View the raw data
-kmerdb view profile.8.kdb # -H for full header
-
-# View the header
-kmerdb header profile.8.kdb
-
-# Collate the files. See 'kmerdb matrix -h' for more information.
-# Note: the 'pass' subcommand passes the int counts through collation, without normalization.
-# In this case the shell interprets '*.8.kdb' as all 8-mer profiles in the current working directory.
-# The k-mer profiles are read in parallel (-p $cores), and collated into one Pandas dataframe, which is printed to STDOUT.
-# Other options include DESeq2 normalization, frequency matrix, or PCA|tSNE based dimensionality reduction techniques.
-kmerdb matrix -p $cores pass *.8.kdb > kmer_count_dataframe.tsv
-
-# Calculate similarity between two (or more) profiles
-# The correlation distance from Numpy is used on one or more profiles, or piped output from 'kmerdb matrix'.
-kmerdb distance correlation profile1.kdb profile2.kdb (...) > distance.tsv
-
-# A condensed, one-line invocation of the matrix and distance command using the bash shell's pipe mechanism is as follows.
-kmerdb matrix pass *.8.kdb | kmerdb distance correlation STDIN > distance.tsv
-```
 
 ## IUPAC support:
 
 ```bash
 kmerdb profile -k $k input.fa output.kdb # This may discard non-IUPAC characters, this feature lacks documentation!
 ```
-IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting.
-
+IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting. Non-standard IUPAC residues are counted as doublets or triplets.
 
 
 ## Documentation
 
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
-Important features to usage that may be important may not be fully documented.
-
-For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing.
+Important features to usage that may be important may not be fully documented as the project is in beta.
 
-In addition, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
+For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
 Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
@@ -172,30 +238,42 @@
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
 
 ## Acknowledgements
 
-Thank you to the authors of kPAL and Jellyfish for the early inspiration. And thank you to others for the encouragement along the way, who shall remain nameless. I wanted this library to be a good strategy for assessing these k-mer profiles, in a way that is both cost aware of the analytical tasks at play, capable of storing the exact profiles in sync with the current assemblies, and then updating the kmer databases only when needed to generate enough spectral signature information.
+Thanks mom and dad and my hometown, awesome hs, and the University of Delaware faculty for support and encouragement. Thanks to my former mentors, bosses, and coworkers. It's been really enjoyable anticipating what the metagenomics community might want from a tool that can handle microbial k-mers well.
 
-The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on just this one project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+Thank you to the authors of kPAL and Jellyfish for the inspiration and bit shifting trick. And thank you to others for the encouragement along the way, who shall remain nameless. 
 
-More on the flip-side of this file. Literally. And figuratively. It's so complex with technology these days.
+The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on this project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+
+More on the flip-side. It's so complex with technology these days...
 
 <!--
-Thanks of course to that French girl from the children's series. 
+Thanks of course to my fans (and haters). Yeah i see you.... but i dont.
 Thanks to my former mentors BC, MR, IN, CR, and my newer bosses PJ and KL.
 Thanks to the Pap lab for the first dataset that I continue to use.
 Thank you to Ryan for the food and stuff. I actually made this project specifically so you and I could converse...
 Thanks to Blahah for tolerating someone snooping and imitating his Ruby style.
 Thanks to Erin for getting my feet wet in this new field. You are my mvp.
 Thanks to Rachel for the good memories and friendship. And Sophie too. veggies n' R love.
 Thanks to Yasmeen for the usual banter.
-Thanks to Max, Robin, and Robert for the good memories in St. Louis.
-Thanks to Freddy Miller for the good memories.
-Thanks to Nichole for the cookies and good memories. And your cute furballs too!
-Thanks to Stace for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
+Thanks to A for the newer banter.
+Thanks to Max, Robin, and Robert for the good memories in St. Louis. What's new?
+Thanks to Fred for the good memories.
+Thanks to Nichole for the cookies and good memories. And your cute furballs too! Hope you're well
+Thanks to S for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
 Thanks to a few friends I met in 2023 that reminded me I have a lot to learn about friendship, dating, and street smarts.
+Thanks to them even more now that I got it xd up.
+
+Thanks to the people of NCC for the Doordash money. It might not be much but I don't have it twisted (I do.)
+
+
+
+Thanks to D from BCCS.
+Thanks to C4H&H. I'm 'healthier' now, but I really still think I need more support than just BCCS. it's urgent.
+
 And thanks to my family and friends.
 Go Blue Hens
 -->
```

### Comparing `kmerdb-0.8.0/kmerdb/__init__.py` & `kmerdb-0.8.1/kmerdb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,24 +59,25 @@
 
 
 
 def print_argv():
     argv = sys.argv
     sys.stderr.write(" ".join(argv[0:4]) + " ...\n")
 
-def citation():
+def citation(arguments):
 
     MODULE_ROOT = os.path.dirname(__file__)
     citation_file = os.path.join(MODULE_ROOT,  'CITATION.txt')
     if os.access(citation_file, os.R_OK):
-        with open(citation_file, 'w') as cit_file:
-            cit_file.write("")
 
-    sys.stderr.write("On the real, we gotta eat.")
-    sys.stderr.write("Consider a +1 on Github to keep it real...")
+        sys.stderr.write("Removing '{0}'\n".format(citation_file))
+        os.remove(citation_file)
+
+    sys.stderr.write("On the real, gotta eat.\n")
+    sys.stderr.write("Consider a +1 on Github to keep it real...\n\n")
 
 def index_file(arguments):
     from kmerdb import fileutil, index
     from kmerdb.config import DONE
     
     with fileutil.open(arguments.kdb, mode='r') as kdb:
         k = kdb.metadata['k']
@@ -1106,36 +1107,41 @@
 
     sfx = os.path.splitext(arguments.kdb)[-1]
     metadata = None
     
     if sfx != ".kdb" and sfx != ".kdbg": # A filepath with invalid suffix
         raise IOError("Viewable .kdb(g) filepath does not end in '.kdb' or '.kdbg'")
     elif not os.path.exists(arguments.kdb):
-        raise IOError("Viewable .kdb(g) filepath '{0}' does not exist on the filesystem".format(arguments.kdb_in))
+        raise IOError("Input .kdb(g) filepath '{0}' does not exist on the filesystem".format(arguments.kdb_in))
 
     if sfx == ".kdb":
         kdb = fileutil.open(arguments.kdb, mode='r', sort=arguments.re_sort, slurp=True)
         metadata = kdb.metadata
+            
         kmer_ids_dtype = metadata["kmer_ids_dtype"]
         N = 4**metadata["k"]
         if metadata["version"] != config.VERSION:
             logger.log_it(".kdb version is out of date, may be incompatible with current KDBReader class", "WARNING")
 
         assert kdb.kmer_ids.size == N, "view | read kmer_ids size did not match N from the header metadata"
         assert kdb.counts.size == N, "view | read counts size did not match N from the header metadata"
         assert kdb.frequencies.size == N, "view | read frequencies size did not match N from the header metadata"
         metadata = kdb.metadata
     elif sfx == ".kdbg":
         kdb = graph.open(arguments.kdb, mode='r')
         if kdb.metadata["version"] != config.VERSION:
             logger.log_it(".kdb file version is out of date, may be incompatible with current fileutil.KDBReader class", "WARNING")
 
+
+            
         N = 4**kdb.metadata["k"]
         metadata = kdb.metadata
 
+    else:
+        raise ValueError("Input to 'kmerdb header' is a .kdb or .kdbg (gzipped .tsv) file of a count vector or a graph. Requires YAML metadata header.Try creating a k-mer count profile with 'kmerdb profile' or edge list with 'kmerdb graph'")
     if arguments.json:
         print(dict(kdb.metadata))
     else:
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
         print(yaml.dump(metadata))
         print(config.header_delimiter)
             
@@ -1190,14 +1196,16 @@
     if sfx != ".kdb" and sfx != ".kdbg": # A filepath with invalid suffix
         raise IOError("Viewable .kdb(g) filepath does not end in '.kdb' or '.kdbg'")
     elif not os.path.exists(arguments.kdb_in):
         raise IOError("Viewable .kdb(g) filepath '{0}' does not exist on the filesystem".format(arguments.kdb_in))
     if sfx == ".kdb":
         with fileutil.open(arguments.kdb_in, mode='r', sort=arguments.re_sort, slurp=True) as kdb_in:
             metadata = kdb_in.metadata
+
+            
             kmer_ids_dtype = metadata["kmer_ids_dtype"]
             N = 4**metadata["k"]
             if metadata["version"] != config.VERSION:
                 logger.log_it("KDB version is out of date, may be incompatible with current KDBReader class", "WARNING")
             if arguments.kdb_out is None or (arguments.kdb_out == "/dev/stdout" or arguments.kdb_out == "STDOUT"): # Write to stdout, uncompressed
                 if arguments.header:
                     yaml.add_representer(OrderedDict, util.represent_ordereddict)
@@ -1293,14 +1301,16 @@
                             #kdb_out._handle.flush()
                             #kdb_out._handle.close()
                             sys.stderr.write(config.DONE)
     elif sfx == ".kdbg":
         kdbg_in = graph.open(arguments.kdb_in, mode='r', slurp=True)
         metadata = kdbg_in.metadata
 
+        
+
         n1_dtype      = metadata["n1_dtype"]
         n2_dtype      = metadata["n2_dtype"]
         weights_dtype = metadata["weights_dtype"]
 
             
         if metadata["version"] != config.VERSION:
             logger.log_it("KDB version is out of date, may be incompatible with current KDBReader class", "WARNING")
@@ -1362,16 +1372,18 @@
                         logger.log_it(e.__str__(), "ERROR")
                         raise e
                     finally:
                         #kdb_out._write_block(kdb_out._buffer)
                         #kdb_out._handle.flush()
                         #kdb_out._handle.close()
                         sys.stderr.write(config.DONE)
+    else:
+        raise ValueError("Input files in kmerdb are tab delimited .csv files, either a count vector or a edge list (block gzip compression). Requires a YAML metadata header. Try making a k-mer count profile/vector with 'kmerdb profile -k 12 <input_1.fa>' ")
 
-
+            
 def assembly(arguments):
     from kmerdb import graph
 
 
 
 
 
@@ -2045,19 +2057,21 @@
         if citation == "":
             return
         else:
             sys.stderr.write("Printing citation notice to stderr. This will not interfere with the execution of the program in any way. Please see CITATION_FAQ.md for any questions.\n")
             sys.stderr.write(citation + "\n\n\n")
             sys.stderr.write("Run 'kmerdb citation' to silence.\n")
     else:
-        raise IOError("Cannot locate the extra package data file 'kmerdb/CITATION', which should have been distributed with the program")
+        sys.stderr.write("Thanks for using/citing kmerdb")
+    # else:
+    #     raise IOError("Cannot locate the extra package data file 'kmerdb/CITATION', which should have been distributed with the program")
 
 
 def get_program_header(arguments):
-    import appmap.py
+    import appmap
     import sys
 
 
     argv = sys.argv
 
     kmerdb_appmap = appmap.kmerdb_appmap( argv )
 
@@ -2067,15 +2081,15 @@
 
     return kmerdb_appmap
 
 def cli():
 
     import sys
 
-    from kmerdb import config
+    from kmerdb import config, appmap
 
     
     argv = sys.argv
 
     
     sys.stderr.write("Running kdb script from '{0}'\n".format(__file__))
     sys.stderr.write("Checking installed environment...\n")
@@ -2093,15 +2107,15 @@
 
     
     parser = argparse.ArgumentParser()
 
     subparsers = parser.add_subparsers(help="Use --help with sub-commands")
 
 
-    profile_parser = subparsers.add_parser("profile", help="Parse data into the database from one or more sequence files")
+    profile_parser = subparsers.add_parser("profile", help=appmap.command_1_description)
     profile_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
 
     profile_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)")
 
     profile_parser.add_argument("-p", "--parallel", type=int, default=1, help="Shred k-mers from reads in parallel")
 
     # profile_parser.add_argument("--batch-size", type=int, default=100000, help="Number of updates to issue per batch to PostgreSQL while counting")
@@ -2118,15 +2132,15 @@
     profile_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     #profile_parser.add_argument("--sparse", action="store_true", default=False, help="Whether or not to store the profile as sparse")
 
     profile_parser.add_argument("seqfile", nargs="+", type=str, metavar="<.fasta|.fastq>", help="Fasta or fastq files")
     profile_parser.add_argument("kdb", type=str, help="Kdb file")
     profile_parser.set_defaults(func=profile)
 
-    graph_parser = subparsers.add_parser("graph", help="Generate an adjacency list from .fa/.fq files")
+    graph_parser = subparsers.add_parser("graph", help=appmap.command_2_description)
     graph_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
 
     graph_parser.add_argument("-k", default=12, type=int, help="Choose k-mer size (Default: 12)", required=True)
 
     graph_parser.add_argument("-p", "--parallel", type=int, default=1, help="Parallel file reading only.")
     graph_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
     graph_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
@@ -2145,15 +2159,15 @@
     # assembly_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     # assembly_parser.add_argument("-g", "--gpu", action="store_true", default=False, help="Utilize GPU resources (requires CUDA library cugraph)")
     # assembly_parser.add_argument("kdbg", type=str, help=".kdbg file")
     # assembly_parser.set_defaults(func=assembly)
 
 
     usage_parser = subparsers.add_parser("usage", help="provide expanded usage information on parameters and functions provided")
-    usage_parser.add_argument("-m", "--method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), required=True, help="Print expanded usage statement")
+    usage_parser.add_argument("method", type=str, choices=("usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"), help="Print expanded usage statement")
     usage_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     usage_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     usage_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     usage_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help=argparse.SUPPRESS)
     usage_parser.set_defaults(func=expanded_help)
 
     help_parser = subparsers.add_parser("help", help="provide expanded help section on parameters and functions provided")
@@ -2161,38 +2175,40 @@
     help_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     help_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     help_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     help_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help=argparse.SUPPRESS)
     help_parser.set_defaults(func=expanded_help)
     
     
-    view_parser = subparsers.add_parser("view", help="View the contents of the .kdb file")
+    view_parser = subparsers.add_parser("view", help="View the contents of the .kdb or .kdbg file")
     view_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     view_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     view_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
+    view_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     view_parser.add_argument("-H", "--header", action="store_true", help="Include header in the output")
     view_parser.add_argument("--re-sort", action="store_true", help="Sort the k-mer profile before displaying") # FIXME
     view_parser.add_argument("--un-sort", action="store_true", help="Unsort the k-mer profile before displaying") # FIXME 
     view_parser.add_argument("--dtype", type=str, default="uint64", help="Read in the profiles as unsigned integer 64bit NumPy arrays")
     view_parser.add_argument("-d", "--decompress", action="store_true", help="Decompress input? DEFAULT: ")
     view_parser.add_argument("-c", "--compress", action="store_true", help="Print compressed output")
     view_parser.add_argument("kdb_in", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be read (Optional)")
     view_parser.add_argument("kdb_out", type=str, nargs="?", default=None, help="A k-mer database file (.kdb) to be written to (Optional)")
     view_parser.set_defaults(func=view)
 
-    header_parser = subparsers.add_parser("header", help="Print the YAML header of the .kdb file and exit")
+    header_parser = subparsers.add_parser("header", help="Print the YAML header of the .kdb or .kdbg file and exit")
     header_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     header_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     header_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
+    header_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     header_parser.add_argument("-j", "--json", help="Print as JSON. DEFAULT: YAML")
     header_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
     header_parser.set_defaults(func=header)
 
 
-    matrix_parser = subparsers.add_parser("matrix", help="Generate a reduced-dimensionality matrix of the 4^k * n (k-mers x samples) data matrix.")
+    matrix_parser = subparsers.add_parser("matrix", help=appmap.command_3_description)
     matrix_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     matrix_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     matrix_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     matrix_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
 
     matrix_parser.add_argument("-p", "--parallel", type=int, default=1, help="Read files in parallel")
     matrix_parser.add_argument("--with-index", default=False, action="store_true", help="Print the row indices as well")
@@ -2215,41 +2231,42 @@
     # rarefy_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     # rarefy_parser.add_argument("-d", "--delimiter", default="\t", type=str, help="The choice of delimiter to parse the DataFrame with")
     # rarefy_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     # rarefy_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input reduced dimension or simply normalized matrix to use with K-means clustering")
     # rarefy_parser.add_argument("-o", "--output", type=argparse.FileType("w"), default=None, help="THe output csv/tsv of rarefied data")
     # rarefy_parser.set_defaults(func=rarefy)
 
-    kmeans_parser = subparsers.add_parser("kmeans", help="Cluster the files according to their k-mer profile")
+    kmeans_parser = subparsers.add_parser("kmeans", help=appmap.command_7_description)
     kmeans_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     kmeans_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
-    kmeans_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     kmeans_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
+    kmeans_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     kmeans_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter of the input csv/tsv to parse, presumably produced by 'kdb matrix'.")
     kmeans_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     kmeans_parser.add_argument("--distance", type=str, default='e', choices=['e', 'b', 'c', 'a', 'u', 'x', 's', 'k'], help="Different distance metrics offered by kcluster. It is highly advised that you check both this source and their documentation to see how this is implemented.")
 
     
     kmeans_parser.add_argument("-k", default=None, type=int, help="The choice of k for clustering", required=True)
     kmeans_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input reduced dimension or mereley normalized matrix to use with K-means clustering")
     kmeans_parser.add_argument("-o", "--output", type=argparse.FileType("w"), default=None, help="The output csv/tsv with added 'label' to use for graphing in R, if the matplotlib graphs are not sufficient.")
     kmeans_parser.add_argument("method", choices=["sklearn", "Biopython"], default="Biopython", help="The Python implementation of k-means to use. The Biopython method is selected for access to alternative distance metrics")
     kmeans_parser.set_defaults(func=kmeans)
 
-    hierarchical_parser = subparsers.add_parser("hierarchical", help="Use scipy.cluster.hierarchy to generate a dendrogram from a distance matrix")
+    hierarchical_parser = subparsers.add_parser("hierarchical", help=appmap.command_8_description)
     hierarchical_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     hierarchical_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
-    hierarchical_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     hierarchical_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help="Number of logged lines to print to stderr. Default: 50")
+    hierarchical_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
+
     hierarchical_parser.add_argument("-d", "--delimiter", type=str, default="\t", help="The delimiter to use when reading the csv.")
     hierarchical_parser.add_argument("-i", "--input", type=argparse.FileType("r"), default=None, help="The input distance matrix for hierarchical clustering")
-    hierarchical_parser.add_argument("-m", "--method", type=str, choices=["single", "complete", "average", "weighted", "centroid", "median", "ward"], default="ward", help="The method for linkage fitting in R to use")
+    hierarchical_parser.add_argument("-m", "--method", type=str, choices=["single", "complete", "average", "weighted", "centroid", "median", "ward"], default="ward", help="The method for linkage fitting to use")
     hierarchical_parser.set_defaults(func=hierarchical)
     
-    dist_parser = subparsers.add_parser("distance", help="Calculate various distance metrics between profiles")
+    dist_parser = subparsers.add_parser("distance", help=appmap.command_4_description)
     dist_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     dist_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     dist_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")        
     dist_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     dist_parser.add_argument("--output-delimiter", type=str, default="\t", help="The output delimiter of the final csv/tsv to write.")
     dist_parser.add_argument("-p", "--parallel", type=int, default=1, help="Read files in parallel")
     dist_parser.add_argument("--column-names", type=str, default=None, help="A filepath to a plaintext flat file of column names.")
@@ -2281,23 +2298,23 @@
         "spearman",
         "sqeuclidean",
         "yule"], default="correlation", help="Choice of distance metric between two profiles")
     dist_parser.add_argument("input", nargs="*", default=[], metavar="<kdbfile1 kdbfile2 ...|input.tsv|STDIN>", help="Two or more .kdb files, or another count matrix in tsv/csv")
     dist_parser.set_defaults(func=distances)
 
 
-    index_parser = subparsers.add_parser("index", help="Create a index file that can be held in memory")
+    index_parser = subparsers.add_parser("index", help=appmap.command_9_description)
     index_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     index_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     index_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     index_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     index_parser.add_argument("kdb", type=str, help="A k-mer database file (.kdb)")
     index_parser.set_defaults(func=index_file)
 
-    shuf_parser = subparsers.add_parser("shuf", help="Create a shuffled .kdb file")
+    shuf_parser = subparsers.add_parser("shuf", help=appmap.command_10_description)
     shuf_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     shuf_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     shuf_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     shuf_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     shuf_parser.add_argument("kdb_in", type=str, help="An indexed k-mer database file (.kdb)")
     shuf_parser.add_argument("kdb_out", type=str, help="The output shuffled k-mer database file (.kdb)")
     shuf_parser.set_defaults(func=shuf)
@@ -2318,16 +2335,17 @@
     # markov_probability_parser.add_argument("kdb", type=str, help="An indexed k-mer database file (.kdb)")
     # markov_probability_parser.set_defaults(func=markov_probability)
 
     citation_parser = subparsers.add_parser("citation", help="Silence the citation notice on further runs")
     citation_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     citation_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     citation_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
+    citation_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     citation_parser.set_defaults(func=citation)
-    
+
     args=parser.parse_args()
     global logger
     global exit_code
 
     
     global step
     global feature
```

### Comparing `kmerdb-0.8.0/kmerdb/__main__.py` & `kmerdb-0.8.1/kmerdb/__main__.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/banners.py` & `kmerdb-0.8.1/kmerdb/banners.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/config.py` & `kmerdb-0.8.1/kmerdb/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 '''
 
 
 
-VERSION="0.8.0"
+VERSION="0.8.1"
 REQUIRES_PYTHON="3.7.4"
 header_delimiter = "\n" + ("="*24) + "\n"
 
 
 requirements_count = 8
 requirements_dev_count = 14 # 4/9/24 there are some duplicates sure, but the requirements evolve faster than the dev do, are more essential for function, and I dont change the -dev file much.
```

### Comparing `kmerdb-0.8.0/kmerdb/distance.c` & `kmerdb-0.8.1/kmerdb/distance.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/_dev/hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "kmerdb.distance",
         "sources": [
             "kmerdb/distance.pyx"
         ]
     },
     "module_name": "kmerdb.distance"
@@ -1674,177 +1674,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1877,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18030,261 +18030,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18293,29 +18293,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18326,15 +18326,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18343,29 +18343,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18376,15 +18376,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18393,29 +18393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18426,15 +18426,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18443,29 +18443,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18476,15 +18476,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18493,29 +18493,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18526,217 +18526,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18752,15 +18752,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18768,68 +18768,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18837,15 +18837,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18860,15 +18860,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18884,15 +18884,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18900,68 +18900,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18969,15 +18969,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18992,15 +18992,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19016,15 +19016,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19032,68 +19032,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19101,15 +19101,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19124,170 +19124,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22077,26 +22077,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../hot/_10+/tmp/pip-build-env-gi6uz2qj/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `kmerdb-0.8.0/kmerdb/distance.pyx` & `kmerdb-0.8.1/kmerdb/distance.pyx`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/fileutil.py` & `kmerdb-0.8.1/kmerdb/fileutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from builtins import open as _open
 
 import jsonschema
 from Bio import SeqIO, bgzf
 
 #sys.path.append('..')
 
-from kmerdb import kmer, util, config
+from kmerdb import kmer, util, config, appmap
 
 # Logging configuration
 global logger
 logger = None
 
 
 # S3 configuration
@@ -261,16 +261,16 @@
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'column_dtype' to be a str")
         elif count_dtype is None or type(count_dtype) is not str:
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'count_dtype' to be a str")
         elif frequencies_dtype is None or type(frequencies_dtype) is not str:
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'frequencies_dtype' to be a str")
         elif slurp is None or type(slurp) is not bool:
             raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'slurp' to be a bool")
-        elif logger is None:
-            raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'logger' to be valid")
+        # elif logger is None:
+        #     raise TypeError("kmerdb.fileutil.KDBReader expects the keyword argument 'logger' to be valid")
 
         
         
         
         if fileobj:
             assert filename is None
             handle = fileobj
@@ -373,16 +373,43 @@
             if self._loggable:
                 self.logger.log_it("Self assigning dtype to uint64 probably", "DEBUG")
                 self.logger.log_it("Checking for metadata inference...", "DEBUG")
             self.kmer_ids = np.zeros(4**self.metadata["k"], dtype=self.metadata["kmer_ids_dtype"])
             self.counts = np.zeros(4**self.metadata["k"], dtype=self.metadata["count_dtype"])
             self.frequencies = np.zeros(4**self.metadata["k"], dtype=self.metadata["frequencies_dtype"])
         except jsonschema.ValidationError as e:
-            logger.error("kmerdb.fileutil.KDBReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks))
-            raise e
+            if self._loggable:
+                self.logger.log_it("kmerdb.fileutil.KDBReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks), "ERROR")
+                self.logger.log_it("""
+
+
+Failed to validate YAML header.
+
+-------------------------------
+
+
+
+ You can store unique k-mer counts, total nullomer counts, and other metadata alongside a k-mer count vector with the 'kmerdb profile' command
+
+
+
+{0}
+
+ ...then try again to view the header with 'kmerdb header' or the whole file : 'kmerdb view -H kmer_count_vector.12.kdb'
+
+
+
+""".format(appmap.command_1_usage, "ERROR")
+
+                self.logger.log_it(e.__str__, "ERROR")
+            raise ValueError("Requires kmerdb v{0} format YAML header. Body is .tsv format table, .bgzf file.      - k-mer count vector        (idx, k-mer id, count, frequency)".format(config.VERSION))
+
+            
+
+
         self.metadata["header_offset"] = self._handle.tell()
         if self._loggable:
             self.logger.log_it("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]), "DEBUG")
         #self._reader = gzip.open(self._filepath, 'r')
         self._offsets = deque()
         for values in bgzf.BgzfBlocks(self._handle):
             #logger.debug("Raw start %i, raw length %i, data start %i, data length %i" % values)
```

### Comparing `kmerdb-0.8.0/kmerdb/graph.py` & `kmerdb-0.8.1/kmerdb/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -938,16 +938,16 @@
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'weights_dtype' to be a str")
 
         elif sort is not None and type(sort) is not bool:
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'sort' to be a bool")
         elif slurp is not None and type(slurp) is not bool:
             raise TypeError("kmerdb.graph.KDBGReader expects the keyword argument 'slurp' to be a bool")
 
-        if logger is None:
-            raise ValueError("graph.KDBGReader expects the keyword argument 'logger' to be valid")
+        # if logger is None:
+        #     raise ValueError("graph.KDBGReader expects the keyword argument 'logger' to be valid")
         
         """
 
         Handle fileobj or 
         """
         
         if fileobj:
@@ -971,14 +971,15 @@
         self.max_cache     = 100
         
         self._buffers      = {}
         self._block_start_offset = None
         self._block_raw_length = None
 
         self.logger = logger
+        self._loggable = logger is not None
         """
 
         np.array defs
 
         n1
         n2
         weights
@@ -991,20 +992,23 @@
         self.n2_dtype   = None
         self.weights       = None
         self.weights_dtype = None
 
         self.read_and_validate_kdbg_header()
 
         if slurp is True:
-            self.logger.log_it("Reading .kdbg contents into memory", "INFO")
+            if self._loggable:
+                self.logger.log_it("Reading .kdbg contents into memory", "INFO")
             self.slurp(n1_dtype=n1_dtype, n2_dtype=n2_dtype, weights_dtype=weights_dtype)
 
         self.is_int = True
-        handle.close()
-        self._handle.close()
+        if handle is not None:
+            handle.close()
+        if self._handle is not None:
+            self._handle.close()
         self._handle = None
         handle = None
         fileobj=None
         return
 
     def read_and_validate_kdbg_header(self):
 
@@ -1014,84 +1018,113 @@
 
         """
 
         '''
         Here we want to load the metadata blocks. We want to load the first two lines of the file: the first line is the version, followed by the number of metadata blocks
         '''
         # 0th block
-        self.logger.log_it("Loading the 0th block from '{0}'...".format(self._filepath), "INFO")
+        if self._loggable:
+            self.logger.log_it("Loading the 0th block from '{0}'...".format(self._filepath), "INFO")
         self._load_block(self._handle.tell())
 
         self._buffer = self._buffer.rstrip(config.header_delimiter)
         
         initial_header_data = OrderedDict(yaml.safe_load(self._buffer))
 
         # Placeholder
         num_header_blocks = None
 
         if type(initial_header_data) is str:
-            self.logger.log_it("Inappropriate type for the header data.", "ERROR")
+            if self._loggable:
+                self.logger.log_it("Inappropriate type for the header data.", "ERROR")
             #logger.info("Um, what the heckin' is this in my metadata block?")
             raise TypeError("kmerdb.graph.KDBGReader could not parse the YAML formatted metadata in the first blocks of the file")
-        elif type(initial_header_data) is OrderedDict:
+        elif type(initial_header_data) is OrderedDict and self._loggable:
             self.logger.log_it("Successfully parsed the 0th block of the file, which is expected to be the first block of YAML formatted metadata", "INFO")
             self.logger.log_it("Assuming YAML blocks until delimiter reached.", "INFO")
 
         """
 
         KDBGReader
         
         YAML metadata spec validation
         """
             
         if "version" not in initial_header_data.keys():
             raise TypeError("kmerdb.graph.KDBGReader couldn't validate the header YAML")
         elif "metadata_blocks" not in initial_header_data.keys():
             raise TypeError("kmerdb.graph.KDBGReader couldn't validate the header YAML")
-            
-        self.logger.log_it(initial_header_data, "INFO")
+
+        if self._loggable:
+            self.logger.log_it(initial_header_data, "INFO")
         
         if initial_header_data["metadata_blocks"] != 1:
-            self.logger.log_it("More than 1 metadata block: uhhhhh are we loading any additional blocks", "ERROR")
+            if self._loggable:
+                self.logger.log_it("More than 1 metadata block: uhhhhh are we loading any additional blocks", "ERROR")
             raise IOError("Cannot read more than 1 metadata block yet")
 
         for i in range(initial_header_data["metadata_blocks"] - 1):
-            self.logger.log_it("Multiple metadata blocks read, most likely from a composite edge-graph...", "WARNING")
+            if self._loggable:
+                self.logger.log_it("Multiple metadata blocks read, most likely from a composite edge-graph...", "WARNING")
             self._load_block(self._handle.tell())
             addtl_header_data = yaml.safe_load(self._buffer.rstrip(config.header_delimiter))
             if type(addtl_header_data) is str:
-                self.logger.log_it(addtl_header_data, "ERROR")
+                if self._loggable:
+                    self.logger.log_it(str(addtl_header_data), "ERROR")
                 raise TypeError("kmerdb.graph.KDBGReader determined the data in the {0} block of the header data from '{1}' was not YAML formatted".format(i, self._filepath))
             elif type(addtl_header_data) is dict:
                 sys.stderr.write("\r")
                 sys.stderr.write("Successfully parsed {0} blocks of YAML formatted metadata".format(i))
                 initial_header_data.update(addtl_header_data)
                 num_header_blocks = i
             else:
-                self.logger.log_it(addtl_header_data, "ERROR")
+                if self._loggable:
+                    self.logger.log_it(str(addtl_header_data), "ERROR")
                 raise RuntimeError("kmerdb.graph.KDBGReader encountered a addtl_header_data type that wasn't expected when parsing the {0} block from the .kdb file '{1}'.".format(i, self._filepath))
 
         #raise RuntimeError("kmerdb.graph.KDBGReader encountered an unexpected type for the header_dict read from the .kdb header blocks")
 
-    
-        self.logger.log_it("Validating the header YAML...", "INFO")
+        if self._loggable:
+            self.logger.log_it("Validating the header YAML...", "INFO")
 
         try:
             jsonschema.validate(instance=initial_header_data, schema=config.graph_schema)
             self.metadata = dict(initial_header_data)
             
             self.k = self.metadata['k']
             self.n1_dtype = self.metadata["n1_dtype"]
             self.n2_dtype = self.metadata["n2_dtype"]
             self.weights_dtype = self.metadata["weights_dtype"]
             self.sorted = self.metadata["sorted"]
 
         except jsonschema.ValidationError as e:
-            self.logger.log_it("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks), "ERROR")
-            raise e
+            if self._loggable:
+                self.logger.log_it("kmerdb.graph.KDBGReader couldn't validate the header/metadata YAML from {0} header blocks".format(num_header_blocks), "ERROR")
+
+                self.logger.log_it("""
+
+
+Failed to validate YAML header.
+
+-------------------------------
+
+
+
+ You can store unique k-mer counts, total nullomer counts, and other metadata alongside the weighted edge list with the 'kmerdb graph' command
+
+
+ ...then try again to view the header with 'kmerdb header'
+
+
+
+""", "ERROR")
+
+                
+                self.logger.log_it(e.__str__, "ERROR")
+            raise ValueError("Requires kmerdb v{0} format YAML header. Body is .tsv format table, .bgzf file.       - weighted edge list        (idx, node1, node2, weight)")
         self.metadata["header_offset"] = self._handle.tell()
         #logger.debug("Handle set to {0} after reading header, saving as handle offset".format(self.metadata["header_offset"]))
         #self._reader = gzip.open(self._filepath, 'r')
         self._offsets = deque()
         for values in bgzf.BgzfBlocks(self._handle):
             #logger.debug("Raw start %i, raw length %i, data start %i, data length %i" % values)
             self._offsets.appendleft(values) # raw start, raw length, data start, data length
@@ -1164,18 +1197,20 @@
         reading=True
         while reading is True:
 
             try:
                 line = next(self)
 
             except StopIteration as e:
-                self.logger.log_it("Finished loading .kdbg through slurp (on init)", "ERROR")
+                if self._loggable:
+                    self.logger.log_it("Finished loading .kdbg through slurp (on init)", "ERROR")
                 raise e
             if line is None:
-                self.logger.log_it("'next' returned None. Panic", "WARNING")
+                if self._loggable:
+                    self.logger.log_it("'next' returned None. Panic", "WARNING")
 
                 raise RuntimeError("kmerdb.graph.KDBGReader.slurp Panicked on new line")
 
 
                   
             try:
```

### Comparing `kmerdb-0.8.0/kmerdb/index.py` & `kmerdb-0.8.1/kmerdb/index.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/kmer.py` & `kmerdb-0.8.1/kmerdb/kmer.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/legacy.py` & `kmerdb-0.8.1/kmerdb/legacy.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/logger.py` & `kmerdb-0.8.1/kmerdb/logger.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/parse.py` & `kmerdb-0.8.1/kmerdb/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 from kmerdb import kmer
 
 
 
 
 
-def parsefile(filepath:str, k:int, logger): #rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
+def parsefile(filepath:str, k:int, logger=None): #rows_per_batch:int=100000, b:int=50000, n:int=1000, both_strands:bool=False, all_metadata:bool=False):
     """Parse a single sequence file in blocks/chunks with multiprocessing support
 
     :param filepath: Path to a fasta or fastq file
     :type filepath: str
     :param k: Choice of k to shred k-mers with
     :type k: int
     :param b: Number of reads (per block) to process in parallel
@@ -83,70 +83,90 @@
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'b' to be an int")
     # elif n is None or type(n) is not int:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'n' to be an int")
     # elif both_strands is None or type(both_strands) is not bool:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'both_strands' to be a bool")
     # elif all_metadata is None or type(all_metadata) is not bool:
     #     raise TypeError("kmerdb.parse.parsefile expects the keyword argument 'all_metadata' to be a bool")
-    if logger is None:
-        raise ValueError("Invalid logger")
+    # if logger is None:
+    #     raise ValueError("Invalid logger")
+
+    _loggable = logger is not None
+    
     data = {} # This is the dictionary of tuples, keyed on k-mer id, and containing 3-tuples ('kmer_id', 'read/start/reverse')
     keys = set()
     rows = []
     N = 4**k
     nullomers = set()
+
+    
     # Build fasta/fastq parser object to stream reads into memory
-    logger.log_it("Initializing parser...", "INFO")
+    if _loggable:
+        logger.log_it("Initializing parser...", "INFO")
+
+
+    
     seqprsr = SeqParser(filepath, k, logger)
     fasta = not seqprsr.fastq # Look inside the seqprsr object for the type of file
 
     # Initialize the kmer array
     try:
         counts = np.zeros(N, dtype="uint64")
     except TypeError as e:
-        logger.log_it("Invalid dtype for numpy array instantiation", "ERROR")
-        logger.log_it(e.__str__(), "ERROR")
+        if _loggable:
+            logger.log_it("Invalid dtype for numpy array instantiation", "ERROR")
+            logger.log_it(e.__str__(), "ERROR")
         raise e
 
-    logger.log_it("Successfully allocated space for {0} unsigned integers: {1} bytes".format(N, counts.nbytes), "INFO")
+    if _loggable:
+        logger.log_it("Successfully allocated space for {0} unsigned integers: {1} bytes".format(N, counts.nbytes), "INFO")
         # Instantiate the kmer class
     Kmer = kmer.Kmers(k, verbose=fasta) # A wrapper class to shred k-mers with
 
     recs = [r for r in seqprsr] # A block of exactly 'b' reads-per-block to process in parallel
     if not fasta:
-        logger.log_it("Read exactly {0} records from the seqparser object".format(len(recs)), "DEBUG")
+        if _loggable:
+            logger.log_it("Read exactly {0} records from the seqparser object".format(len(recs)), "DEBUG")
         assert len(recs) <= b, "The seqparser should return exactly {0} records at a time".format(b)
-    else:
+    elif _loggable:
         logger.log_it("Skipping the block size assertion for fasta files", "DEBUG")
-    logger.log_it("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
+
+    if _loggable:
+        logger.log_it("Read {0} sequences from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
     all_kmer_metadata = list([] for x in range(N))
     while len(recs): # While the seqprsr continues to produce blocks of reads
 
         num_recs = len(recs)
-        logger.log_it("Processing a block of {0} reads/sequences".format(num_recs), "INFO")
+
+        if _loggable:
+            logger.log_it("Processing a block of {0} reads/sequences".format(num_recs), "INFO")
 
         # Initialize an all_kmer_metadata list
         kmer_metadata = []
         list_of_dicts = list(map(Kmer.shred, recs))
 
         # Flatmap to 'kmers', the dictionary of {'id': read_id, 'kmers': [ ... ]}
-        logger.log_it("\n\nAcquiring linked-list of all k-mer ids from {0} sequence records...\n\n".format(num_recs), "INFO")
+        if _loggable:
+            logger.log_it("\n\nAcquiring linked-list of all k-mer ids from {0} sequence records...\n\n".format(num_recs), "INFO")
         kmer_ids = list(chain.from_iterable(map(lambda x: x['kmers'], list_of_dicts)))
 
         sus = set()
-        logger.log_it("Removing any eroneous k-mers without an id, cause by 'N' content, creating new gaps in the k-mer profile...", "WARNING")
-        logger.log_it("Will substitute IUPAC residues with their respective residues, adding one count for each", "WARNING")
+
+        
+        if _loggable:
+            logger.log_it("Removing any eroneous k-mers without an id, cause by 'N' content, creating new gaps in the k-mer profile...", "WARNING")
+            logger.log_it("Will substitute IUPAC residues with their respective residues, adding one count for each", "WARNING")
         num_sus = 0
         for i, k in enumerate(kmer_ids):
             if k is None:
                 sus.add(i) # This propagates the N removal, by adding those to the set for removal later.
                 num_sus += 1
 
         logger.log_it("Created {0} gaps in the k-mer profile to clean it of N-content".format(num_sus), "INFO")
-        if num_sus > 0:
+        if num_sus > 0 and _loggable:
             logger.log_it("{0} uncountable k-mer identified".format(num_sus), "WARNING")
             logger.log_it("Likely caused by the presence of the unspecified nucleotide 'N' in a .fasta file", "WARNING")
             logger.log_t("Will remove from the final committed profile", "WARNING")
 
         ########################
         # K-mer cleaning
         #
@@ -155,18 +175,20 @@
         # More specifically, it eliminates entries that were formally loaded into the k-mers array,
         # and thus would be a minor percentage of the total number of k-mers,
         # Specifically, k-mers or subsequences with N can be excluded from the profile
         # To essentially eliminate an area of sequence and create an artificial gap in the "retained" graph.
         # The graph can be explicitly collapsed when you want to, by supplying reads or sequence information, that is contiguous "in your judgement".
         # By introducing these artificial gaps, we expose the errors or unspecified bases through data.
         #
-        logger.log_it("Found {0} invalid or enumerable k-mers, sequences which have no defined index, i".format(num_sus), "INFO")
-        logger.log_it("In other words, one or more characters in your .fasta or .fastq file were 'N' or otherwise contained IUPAC characters that need to be substituted.", "DEBUG")
-        logger.log_it("We have chosen to omit k-mer with unspecified nucleotides 'N', and these make gaps in our database explicitly.", "DEBUG")
-        logger.log_it("These can be recovered from the reads if they are needed, and the read ids may be found with the experimental --all-metadata flag", "INFO")
+
+        if _loggable:
+            logger.log_it("Found {0} invalid or enumerable k-mers, sequences which have no defined index, i".format(num_sus), "INFO")
+            logger.log_it("In other words, one or more characters in your .fasta or .fastq file were 'N' or otherwise contained IUPAC characters that need to be substituted.", "DEBUG")
+            logger.log_it("We have chosen to omit k-mer with unspecified nucleotides 'N', and these make gaps in our database explicitly.", "DEBUG")
+            logger.log_it("These can be recovered from the reads if they are needed, and the read ids may be found with the experimental --all-metadata flag", "INFO")
         # if all_metadata:
 
         #     logger.warning("\n\n\nGENERATING ALL METADATA\n\n\nThis is extremely expensive and experimental. You have been warned.\n\n\n")
         #     reads = list(chain.from_iterable(map(lambda x: x['seqids'], list_of_dicts)))
         #     starts = list(chain.from_iterable(map(lambda x: x['starts'], list_of_dicts)))
         #     reverses = list(chain.from_iterable(map(lambda x: x['reverses'], list_of_dicts)))
         #     logger.debug("Checking each k-mer for N-content and IUPAC substitution")
@@ -177,32 +199,40 @@
         #             starts[i] = None
         #             reverses[i] = None
         #     kmer_ids = list(filter(lambda k: k is not None, kmer_ids)) 
         #     reads = list(filter(lambda r: r is not None, reads))
         #     starts = list(filter(lambda s: s is not None, starts))
         #     reverses = list(filter(lambda r: r is not None, reverses))
         # else:
-        logger.log_it("Checking each k-mer for IUPAC substitution or N content.", "DEBUG")
+        if _loggable:
+            logger.log_it("Checking each k-mer for IUPAC substitution or N content.", "DEBUG")
         for i, x in enumerate(kmer_ids): # Here we remove the k-mer ids where N-content is detected, in case they are needed, you can use kmer_ids prior to this point to build functionality.
             if i in sus:
                 kmer_ids[i] = None
-        logger.log_it("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions", "INFO")
+
+        if _loggable:
+            logger.log_it("Eliminating suspicious 'sus' k-mers, i.e. those with N-content or IUPAC substitutions", "INFO")
+
+
+            
         kmer_ids = list(filter(lambda k: k is not None, kmer_ids))
         reads = [] # I'm keeping this in, just in case for some reason the variable names are needed in the 
         starts = []
         reverses = []
         if None in kmer_ids:
             # Actually they were just introduced to be filtered out, instead of deleted
             # Because each deletion whould cange the array index
             # So instead we set ghtme to None, and filter out
             raise ValueError("kmerdb.parse.parsefile encountered an invalid kmer_id. Internal error.")
 
 
-        logger.log_it("{0} 'clean' kmers were identified successfully from {1} input sequences".format(len(kmer_ids), num_recs), "DEBUG")
-        logger.log_it("Flatmapped {0} kmers for their metadata aggregation".format(len(kmer_ids), len(starts)), "DEBUG")
+
+        if _loggable:
+            logger.log_it("{0} 'clean' kmers were identified successfully from {1} input sequences".format(len(kmer_ids), num_recs), "DEBUG")
+            logger.log_it("Flatmapped {0} kmers for their metadata aggregation".format(len(kmer_ids), len(starts)), "DEBUG")
         # Assert that all list lengths are equal before adding metadata to k-mers
         # else:
         #     raise RuntimeError("Still have no clue what's going on...")
         # On disk k-mer counting
         # Thank you, this was brilliant
         # https://stackoverflow.com/a/9294062/12855110
         # 01-01-2022 This has been removed in favor of in-memory counting
@@ -216,15 +246,18 @@
                 counts[kmer] += 1
         # all_kmer_metadata
         # if all_metadata:
         #     for single_kmer_id, read, start, reverse in kmer_metadata:
         #         all_kmer_metadata[single_kmer_id].append((read, start, reverse))
 
         recs = [r for r in seqprsr] # The next block of exactly 'b' reads
-        logger.log_it("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
+
+
+        if _loggable:
+            logger.log_it("Read {0} more records from the {1} seqparser object".format(len(recs), "fasta" if fasta else "fastq"), "INFO")
     # Get nullomers
     # only nullomer counts
     unique_kmers = int(np.count_nonzero(counts))
 
 
     all_theoretical_kmer_ids = list(range(N))
 
@@ -239,15 +272,18 @@
     
     seqprsr.total_kmers = int(np.sum(counts))
     seqprsr.unique_kmers = unique_kmers
     seqprsr.nullomers = num_nullomers
 
     
     seqprsr.nullomer_array = np.array(all_theoretical_kmer_ids, dtype="uint64")[is_nullomer]
-    logger.log_it("\n\n\nFinished counting k-mers from '{0}'...\n\n\n".format(filepath), "INFO")
+
+
+    if _loggable:
+        logger.log_it("\n\n\nFinished counting k-mers from '{0}'...\n\n\n".format(filepath), "INFO")
 
     return counts, seqprsr.header_dict(), seqprsr.nullomer_array, logger.logs
```

### Comparing `kmerdb-0.8.0/kmerdb/probability.py` & `kmerdb-0.8.1/kmerdb/probability.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/python_distances.py` & `kmerdb-0.8.1/kmerdb/python_distances.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb/util.py` & `kmerdb-0.8.1/kmerdb/util.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/kmerdb.egg-info/PKG-INFO` & `kmerdb-0.8.1/kmerdb.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -265,17 +265,17 @@
 Requires-Dist: expects>=0.9.0; extra == "dev"
 Requires-Dist: docutils>=0.17; extra == "dev"
 Requires-Dist: sphinx>=4.3.2; extra == "dev"
 Requires-Dist: pytest>=5.3.5; extra == "dev"
 Requires-Dist: twine==4.0.1; extra == "dev"
 
 # README - kmerdb
-> A Python CLI and module for k-mer profiles, similarities, and graph databases
+> Python CLI and module for k-mer profiles, similarities, and graph databases
 
-NOTE: This project is in beta stage. Development is ongoing. But feel free to clone the repository and play with the code for yourself.
+NOTE: Beta-stage `.bgzf` and `zlib` compatible k-mer count and DeBruijn graph formats.
 
 ## Development Status
 [![Downloads](https://static.pepy.tech/personalized-badge/kmerdb?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pypi.org/project/kmerdb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/kmerdb)
 [![GitHub Downloads](https://img.shields.io/github/downloads/MatthewRalston/kdb/total.svg?style=social&logo=github&label=Download)](https://github.com/MatthewRalston/kmerdb/releases)
 [![PyPI version](https://img.shields.io/pypi/v/kmerdb.svg)][pip]
 [![Python versions](https://img.shields.io/pypi/pyversions/kmerdb.svg)][Pythons]
@@ -286,121 +286,187 @@
 
 [pip]: https://pypi.org/project/kmerdb/
 [Pythons]: https://pypi.org/project/kmerdb/
 [RTD]: https://kdb.readthedocs.io/en/latest/
 
 ## Summary 
 
-KDB is a Python library designed for bioinformatics applications. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts/abundances in a columnar format, with input file checksums, total counts, nullomers, and mononucleotide counts in a YAML formatted header in the first block of the `bgzf` formatted `.kdb` file. One restriction is that k-mers with unspecified sequence residues 'N' create gaps in the k-mer to sequence relationship space, and are excluded. That said, non-standard IUPAC residues are supported.
+k-mer counts or De Bruijn graph of .fa(.gz)/.fq(.gz) sequence data can be converted to `.kdb` (+new! `.kdbg` De Bruijn graph) format, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided. The output file is compatible with `zlib`.
 
+`pip install kmerdb` is a Python CLI designed for k-mer counting and De Bruijn graphs. It addresses the ['k-mer' problem](https://en.wikipedia.org/wiki/K-mer) (substrings of length k) in a simple and performant manner. It stores the k-mer counts in a columnar format (input checksums, total and unique k-mer counts, nullomers, mononucleotide counts) with a YAML formatted metadata header in the first block of the `bgzf` formatted `.kdb` (k-mer database) file. 
 
 Please see the [Quickstart guide](https://matthewralston.github.io/kmerdb/quickstart) for more information about the format, the library, and the project.
 
-The k-mer spectrum of the fasta or fastq sequencing data is stored in the `.kdb` format spec, a bgzf file similar to `.bam`. For those familiar with `.bam`, a `view` and `header` functions are provided to decompress a `.kdb` file into a standard output stream. The output file is compatible with `zlib`.
 
+## Usage
 
+```bash
+# Usage    --help option    --debug mode
+kmerdb --help # [+ --debug mode]
+kmerdb usage -m graph
+
+# Output:
+ o-O      |||
+o---O     |||             [|[          kmerdb           ]|]
+O---o     |||
+ O-o      |||        version :     v0.8.0
+  O       |||
+ o-O      |||        GitHub  : https://github.com/MatthewRalston/kmerdb/issues
+o---O     |||         PyPI   : https://pypi.org/project/kmerdb/
+O---o     |||      Website   : https://matthewralston.github.io/kmerdb
+ O-o      |||
+                                                                       lang :         python
+                                                                          v :      >= v3.7.4
+
+                      package manger : pip
+                        version      : >= 24.0
+        package root : /path2py/lib/python3.12/site-packages/kmerdb
+        exe file     : /path2py/lib/python3.12/site-packages/kmerdb/__init__.py
+
+                      required packages : 8
+                   development packages : 14
+
+           ARGV : ['/path2py/bin/kmerdb', 'usage', '-m', 'graph']
+        
+...
+
+Beginning program...
+
+                          name : graph
+                   description : create edge nodes in (block) .gz compressed format from .fasta or .fq format.
+        
+
+* features
+
+- name: k-mer count arrays, linear, produced as file is read through sliding window.
+    (Un)compressed support for .fa/.fq.
+  shortname: parallel faux-OP sliding window k-mer shredding
+  description: Sequential k-mers from the input .fq|.fa files are added to the De
+    Bruijn graph. In the case of secondary+ sequences in the .fa or considering NGS
+    (.fq) data, non-adjacent k-mers are pruned with a warning. Summary statistics
+    for the entire file are given for each file read, + a transparent data structure.
+		
+- name: k-mer neighbors assessed and tallied, creates a unsorted edge list, with weights
+  shortname: weighted undirected graph
+  description: an edge list of a De Bruijn graph is generated from all k-mers in the
+    forward direction of .fa/.fq sequences/reads. i.e. only truly neighboring k-mers
+    in the sequence data are added to the tally of the k-mer nodes of the de Bruijn
+    graph and the edges provided by the data.
+
+
+
+
+* steps
+
+- name: read input file(s) from filesystem into k-mer arrays
+  shortname: shred inputs into k-mer count arrays
+  description: shred input sequences into k-mer count vector
+  
+- name: merge k-mer arrays and aggregate metadata
+  shortname: merge k-mer count arrays for aggregate metadata (header)
+  description: merge counts of nullomers, unique kmers, and total kmers.
+  
+- name: collate the weighted edge lists after reading multiple files. Output data
+    consists of a edge_list, analogous metadata-header as YAML, kmer_counts, and nullomer_ids.
+  shortname: extract undirected weighted graph
+  description: consists of info from a .kdb file and a .kdbg file. The node IDs, the
+    edges, and the number of times the pair was observed from forward sequences in
+    the provided dataset
+	
+- name: print 'table' Final stats and close output file
+  shortname: metrics and shutdown
+  description: print final statistics, typically metadata values, and ensure file
+    is closed.
+
+
+
+
+#   +
+
+# [ 3 main features: ]     k-mer counts (kmerdb profile -k 12 <input.fa|.fq> [<input.fa|.fq>])    'De Bruijn' graph (kmerdb graph)         [matrices, distances, and clustering!]
 
-## Installation
-
+# Create a [composite] profile of k-mer counts from sequence files. (.fasta|.fastq|.fa.gz|.fq.gz)
+kmerdb profile -k 8 example_1.fq.gz [example_2.fq.gz] profile_1.8.kdb
 
-### Dependencies
+# Build a weighted edge list (+ node ids/counts = De Bruijn graph)
+kmerdb graph -k 12 example_1.fq.gz example_2.fq.gz edges_1.kdbg
 
-DESeq2 is required as a R dependency for rpy2-mediated normalization.
+# View k-mer count vector
+kmerdb view profile_1.8.kdb # -H for full header
 
-```r
-if (!requireNamespace("BiocManager", quietly = TRUE))
-    install.packages("BiocManager")
+# Note: zlib compatibility
+#zcat profile_1.8.kdb
 
-BiocManager::install("DESeq2")
-```
+# View header (config.py[kdb_metadata_schema#L84])
+kmerdb header profile_1.8.kdb
 
-All other dependencies are managed directly by pip. 
+## Optional normalization, dim reduction, and distance matrix features:
 
+# K-mer count matrix - Cython Pearson coefficient of correlation [ ssxy/sqrt(ssxx*ssyy) ]
+kmerdb matrix pass *.8.kdb | kmerdb distance pearson -i STDIN
+# 
+# kmerdb matrix DESeq2 *.8.kdb
+# kmerdb matrix PCA *.8.kdb
+# kmerdb matrix tSNE *.8.kdb
+#   # <pass> just makes a k-mer count matrix from k-mer count vectors.
+# 
+
+# Distances on count matrices [ SciPy ]  pdists + [ Cython ] Pearson correlation, scipy Spearman and scipy correlation pdist calculations are available ]
+kmerdb distance -h
+# 
+#
+# usage: kmerdb distance [-h] [-v] [--debug] [-l LOG_FILE] [--output-delimiter OUTPUT_DELIMITER] [-p PARALLEL] [--column-names COLUMN_NAMES] [--delimiter DELIMITER] [-k K]
+#                       {braycurtis,canberra,chebyshev,cityblock,correlation,cosine,dice,euclidean,hamming,jaccard,jensenshannon,kulsinski,mahalanobis,matching,minkowski,pearson,rogerstanimotorusselrao,seuclidean,sokalmichener,sokalsneath,spearman,sqeuclidean,yule} [<kdbfile1 kdbfile2 ...|input.tsv|STDIN> ...]
+
+# +
+
+#    Kmeans (sklearn, BioPython)
+kmerdb kmeans -k 4 -i dist.tsv
+#    BioPython Phylip tree + upgma
+kmerdb hierarchical -i dist.tsv
 
-### OSX and Linux release:
 
-```sh
-pip install --python-version 3.7.4 --pre kmerdb
 ```
 
 
+## Installation
 
-### Development installation:
+### OSX and Linux release:
 
 ```sh
-git clone https://github.com/MatthewRalston/kmerdb.git
-pip install .
+pip install --python-version 3.7.4 --pre kmerdb
 ```
 
-## Usage Example
+#### Optional DESeq2 normalization
 
-NOTE: Usage in detail can be found on the [quickstart page](https://matthewralston.github.io/kmerdb/quickstart#usage)
+DESeq2 is an optional R dependency for rpy2-mediated normalization.
 
-<!-- ## NOTE: Temporary usage pattern:
-Migrating the repo from setup.py to the PEP606 standard PyProject.toml is borking my current invocation pattern. Sorry for the inconveniece... it's happening right now. -->
+```r
+if (!requireNamespace("BiocManager", quietly = TRUE))
+    install.packages("BiocManager")
 
-<!-- ```bash
-python -m kmerdb [cmd] [options]
+BiocManager::install("DESeq2")
 ```
 
-See `python -m kmerdb -h` for details.
--->
-
-## CLI Usage
-
-```bash
-kmerdb --help
-# Build a [composite] profile to a new .kdb file
-kmerdb profile -k 8 example1.fq.gz example2.fq.gz profile.8.kdb
-
-# Note: zlib compatibility
-zcat profile.8.kdb
-
-# Build a weighted edge list
-kmerdb graph -k 12 example1.fq.gz example2.fq.gz edges.kdbg
-
-# View the raw data
-kmerdb view profile.8.kdb # -H for full header
-
-# View the header
-kmerdb header profile.8.kdb
-
-# Collate the files. See 'kmerdb matrix -h' for more information.
-# Note: the 'pass' subcommand passes the int counts through collation, without normalization.
-# In this case the shell interprets '*.8.kdb' as all 8-mer profiles in the current working directory.
-# The k-mer profiles are read in parallel (-p $cores), and collated into one Pandas dataframe, which is printed to STDOUT.
-# Other options include DESeq2 normalization, frequency matrix, or PCA|tSNE based dimensionality reduction techniques.
-kmerdb matrix -p $cores pass *.8.kdb > kmer_count_dataframe.tsv
-
-# Calculate similarity between two (or more) profiles
-# The correlation distance from Numpy is used on one or more profiles, or piped output from 'kmerdb matrix'.
-kmerdb distance correlation profile1.kdb profile2.kdb (...) > distance.tsv
-
-# A condensed, one-line invocation of the matrix and distance command using the bash shell's pipe mechanism is as follows.
-kmerdb matrix pass *.8.kdb | kmerdb distance correlation STDIN > distance.tsv
-```
 
 ## IUPAC support:
 
 ```bash
 kmerdb profile -k $k input.fa output.kdb # This may discard non-IUPAC characters, this feature lacks documentation!
 ```
-IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting.
-
+IUPAC residues (ATCG+RYSWKM+BDHV) are kept throughout the k-mer counting. But non-IUPAC residues (N) and characters are trimmed from the sequences prior to k-mer counting. Non-standard IUPAC residues are counted as doublets or triplets.
 
 
 ## Documentation
 
 Check out the [main webpage](https://matthewralston.github.io/kmerdb) and the [Readthedocs documentation](https://kdb.readthedocs.io/en/stable/), with examples and descriptions of the module usage.
 
-Important features to usage that may be important may not be fully documented.
-
-For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing.
+Important features to usage that may be important may not be fully documented as the project is in beta.
 
-In addition, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
+For example, the IUPAC treatment is largely custom, and does the sensible thing when ambiguous bases are found in fasta files, but it could use some polishing. For example, the '`N`' residue rejection creates gaps in the k-mer profile from the real dataset by admittedly ommitting certain k-mer counts.
 This is one method for counting k-mers and handling ambiguity. Fork it and play with it a bit.
 
 Also, the parallel handling may not always be smooth, if you're trying to load dozens of 12+ mer profiles into memory. This would especially matter in the matrix command, before the matrix is generated. You can use single-core if your machine can't collate that much into main memory at once, depending on how deep the fastq dataset is, and the `--block-size` parameter in `kmerdb profile` is likely going to facilitate your memory overhead by reading chunks of `--block-size` reads into memory at once while accumulating the k-mer counts in a `uint64` array. Even when handling small-ish k-mer profiles, you may bump into memory overheads rather quickly. 
 
 Besides that, I'd suggest reading the source, the differente elements of the [main page](https://matthewralston.github.io/kmerdb) or the [RTD documentation](https://kdb.readthedocs.io/en/stable/).
 
 
@@ -442,30 +508,42 @@
 2. Create your feature branch (`git checkout -b feature/fooBar`)
 3. Commit your changes (`git commit -am 'Add some fooBar'`)
 4. Push to the branch (`git push origin feature/fooBar`)
 5. Create a new Pull Request
 
 ## Acknowledgements
 
-Thank you to the authors of kPAL and Jellyfish for the early inspiration. And thank you to others for the encouragement along the way, who shall remain nameless. I wanted this library to be a good strategy for assessing these k-mer profiles, in a way that is both cost aware of the analytical tasks at play, capable of storing the exact profiles in sync with the current assemblies, and then updating the kmer databases only when needed to generate enough spectral signature information.
+Thanks mom and dad and my hometown, awesome hs, and the University of Delaware faculty for support and encouragement. Thanks to my former mentors, bosses, and coworkers. It's been really enjoyable anticipating what the metagenomics community might want from a tool that can handle microbial k-mers well.
 
-The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on just this one project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+Thank you to the authors of kPAL and Jellyfish for the inspiration and bit shifting trick. And thank you to others for the encouragement along the way, who shall remain nameless. 
 
-More on the flip-side of this file. Literally. And figuratively. It's so complex with technology these days.
+The intention is that more developers would want to add functionality to the codebase or even just utilize things downstream, but to build out directly with numpy and scipy/scikit as needed to suggest the basic infrastructure for the ML problems and modeling approaches that could be applied to such datasets. This project began under GPL v3.0 and was relicensed with Apache v2. Hopefully this project could gain some interest. I have so much fun working on this project. There's more to it than meets the eye. I'm working on a preprint, and the draft is included in some of the latest versions of the codebase, specifically .Rmd files.
+
+More on the flip-side. It's so complex with technology these days...
 
 <!--
-Thanks of course to that French girl from the children's series. 
+Thanks of course to my fans (and haters). Yeah i see you.... but i dont.
 Thanks to my former mentors BC, MR, IN, CR, and my newer bosses PJ and KL.
 Thanks to the Pap lab for the first dataset that I continue to use.
 Thank you to Ryan for the food and stuff. I actually made this project specifically so you and I could converse...
 Thanks to Blahah for tolerating someone snooping and imitating his Ruby style.
 Thanks to Erin for getting my feet wet in this new field. You are my mvp.
 Thanks to Rachel for the good memories and friendship. And Sophie too. veggies n' R love.
 Thanks to Yasmeen for the usual banter.
-Thanks to Max, Robin, and Robert for the good memories in St. Louis.
-Thanks to Freddy Miller for the good memories.
-Thanks to Nichole for the cookies and good memories. And your cute furballs too!
-Thanks to Stace for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
+Thanks to A for the newer banter.
+Thanks to Max, Robin, and Robert for the good memories in St. Louis. What's new?
+Thanks to Fred for the good memories.
+Thanks to Nichole for the cookies and good memories. And your cute furballs too! Hope you're well
+Thanks to S for the lessons, convos, and even embarassing moments. You're kind of awesome to me.
 Thanks to a few friends I met in 2023 that reminded me I have a lot to learn about friendship, dating, and street smarts.
+Thanks to them even more now that I got it xd up.
+
+Thanks to the people of NCC for the Doordash money. It might not be much but I don't have it twisted (I do.)
+
+
+
+Thanks to D from BCCS.
+Thanks to C4H&H. I'm 'healthier' now, but I really still think I need more support than just BCCS. it's urgent.
+
 And thanks to my family and friends.
 Go Blue Hens
 -->
```

### Comparing `kmerdb-0.8.0/kmerdb.egg-info/SOURCES.txt` & `kmerdb-0.8.1/kmerdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.0/pyproject.toml` & `kmerdb-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # requires numpy and cython for custom cython correlation function
 
 requires = ["setuptools>=69.2.0", "numpy>=1.21.2", "Cython>=3.0.8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kmerdb"
-version = "0.8.0"
+version = "0.8.1"
 description = "Yet another corretion to the 'yet another correction to just a k-mer counter...'"
 readme = "README.md"
 authors = [{name="Matt Ralston <mralston.development@gmail.com>", email="mralston.development@gmail.com"}]
 license = { file = "LICENSE.txt" }
 classifiers = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
@@ -98,14 +98,15 @@
     # 'rypy2>=3.4.2'
     # Vanity
     #'ghstats>=1.2.0',
     #########################################
     # Documentation
     #########################################
     'docutils>=0.17',
+    #'grip>=4.6.2',
     'sphinx>=4.3.2',
     #'sphinx-autodoc',
     # These are kind of developmental things, there really cant be testing around a 5% tested codebase, this is open source at its worse,
     # and considering  otherwise is toxic.
     'pytest>=5.3.5',
     #########################################
     #
```

### Comparing `kmerdb-0.8.0/setup.py` & `kmerdb-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,20 @@
         return None
                 
 # Package meta-data.
 NAME = 'kmerdb'
 DESCRIPTION = 'Yet another kmer library for Python'
 long_description = 'See README.md for details'
 URL = 'https://github.com/MatthewRalston/kmerdb'
-CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.7.8.tar.gz"
+CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz"
 EMAIL = 'mralston.development@gmail.com'
 AUTHOR = 'fross'
 REQUIRES_PYTHON = ">=3.7.4"
 #REQUIRES_PYTHON = '>=3.12.2'
-VERSION = "0.8.0"
+VERSION = "0.8.1"
 KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer"]
 CLASSIFIERS = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
 	    "Development Status :: 7 - Inactive",
 	    "Environment :: Console",
 	    "Intended Audience :: Developers",
```

### Comparing `kmerdb-0.8.0/test/test_kmer.py` & `kmerdb-0.8.1/test/test_kmer.py`

 * *Files identical despite different names*

