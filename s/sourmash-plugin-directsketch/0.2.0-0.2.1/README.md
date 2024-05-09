# Comparing `tmp/sourmash_plugin_directsketch-0.2.0.tar.gz` & `tmp/sourmash_plugin_directsketch-0.2.1.tar.gz`

## Comparing `sourmash_plugin_directsketch-0.2.0.tar` & `sourmash_plugin_directsketch-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.0/Cargo.toml
--rw-r--r--   0      501       20      405 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/.github/dependabot.yml
--rw-r--r--   0      501       20     1474 2024-05-08 16:20:14.000000 sourmash_plugin_directsketch-0.2.0/.github/workflows/build-test.yml
--rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.0/.gitignore
--rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/LICENSE
--rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.0/Makefile
--rw-r--r--   0      501       20     2417 2024-05-01 22:22:17.000000 sourmash_plugin_directsketch-0.2.0/README.md
--rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.0/environment.yml
--rw-r--r--   0      501       20    51553 2024-05-02 00:08:24.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_assembly_report.txt
--rw-r--r--   0      501       20   798402 2024-05-02 00:08:23.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20    36700 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20    25113 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/src/directsketch.rs
--rw-r--r--   0      501       20     2359 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/src/lib.rs
--rw-r--r--   0      501       20     4597 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/src/python/sourmash_plugin_directsketch/__init__.py
--rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.0/src/utils.rs
--rw-r--r--   0      501       20    38326 2024-05-08 14:36:55.000000 sourmash_plugin_directsketch-0.2.0/test.zip
--rw-r--r--   0      501       20      410 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.0/tests/conftest.py
--rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/tests/sourmash_tst_utils.py
--rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/.notempty
--rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000175555.1.sig.gz
--rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.protein.sig.gz
--rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.sig.gz
--rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/acc.csv
--rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
--rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
--rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
--rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
--rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
--rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
--rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
--rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
--rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
--rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.0/tests/test-data/test.zip
--rw-r--r--   0      501       20    11413 2024-05-06 22:31:50.000000 sourmash_plugin_directsketch-0.2.0/tests/test_gbsketch.py
--rw-r--r--   0      501       20    63427 2024-05-08 18:30:02.000000 sourmash_plugin_directsketch-0.2.0/Cargo.lock
--rw-r--r--   0      501       20     1003 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.1/Cargo.toml
+-rw-r--r--   0      501       20      405 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/.github/dependabot.yml
+-rw-r--r--   0      501       20     1474 2024-05-08 16:20:14.000000 sourmash_plugin_directsketch-0.2.1/.github/workflows/build-test.yml
+-rw-r--r--   0      501       20      718 2024-04-26 03:30:23.000000 sourmash_plugin_directsketch-0.2.1/.gitignore
+-rw-r--r--   0      501       20     1540 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/LICENSE
+-rw-r--r--   0      501       20      368 2024-05-01 15:59:57.000000 sourmash_plugin_directsketch-0.2.1/Makefile
+-rw-r--r--   0      501       20     2417 2024-05-01 22:22:17.000000 sourmash_plugin_directsketch-0.2.1/README.md
+-rw-r--r--   0      501       20      176 2024-04-30 23:49:37.000000 sourmash_plugin_directsketch-0.2.1/environment.yml
+-rw-r--r--   0      501       20    51553 2024-05-02 00:08:24.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_assembly_report.txt
+-rw-r--r--   0      501       20   798402 2024-05-02 00:08:23.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20    36700 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_assembly_report.txt
+-rw-r--r--   0      501       20   526013 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20   314606 2024-05-02 00:08:22.000000 sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20    24921 2024-05-08 21:50:14.000000 sourmash_plugin_directsketch-0.2.1/src/directsketch.rs
+-rw-r--r--   0      501       20     2359 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.1/src/lib.rs
+-rw-r--r--   0      501       20     4597 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/src/python/sourmash_plugin_directsketch/__init__.py
+-rw-r--r--   0      501       20     5730 2024-05-07 17:31:28.000000 sourmash_plugin_directsketch-0.2.1/src/utils.rs
+-rw-r--r--   0      501       20    38326 2024-05-08 21:42:37.000000 sourmash_plugin_directsketch-0.2.1/test.zip
+-rw-r--r--   0      501       20      410 2024-05-08 18:17:29.000000 sourmash_plugin_directsketch-0.2.1/tests/conftest.py
+-rw-r--r--   0      501       20     6849 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/tests/sourmash_tst_utils.py
+-rw-r--r--   0      501       20        0 2024-04-26 00:09:24.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/.notempty
+-rw-r--r--   0      501       20    44471 2024-04-26 18:22:33.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000175555.1.sig.gz
+-rw-r--r--   0      501       20    20407 2024-04-27 01:42:18.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.protein.sig.gz
+-rw-r--r--   0      501       20    29259 2024-04-26 18:04:28.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.sig.gz
+-rw-r--r--   0      501       20      497 2024-04-27 02:01:15.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/acc.csv
+-rw-r--r--   0      501       20   798402 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20   526013 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20   314606 2024-04-27 00:46:04.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   798402 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz
+-rw-r--r--   0      501       20     7793 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt
+-rw-r--r--   0      501       20  1118769 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt
+-rw-r--r--   0      501       20   702342 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz
+-rw-r--r--   0      501       20    36700 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt
+-rw-r--r--   0      501       20   526013 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz
+-rw-r--r--   0      501       20     1201 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt
+-rw-r--r--   0      501       20   314606 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz
+-rw-r--r--   0      501       20   735547 2024-04-26 18:00:37.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz
+-rw-r--r--   0      501       20   118778 2024-04-27 00:46:05.000000 sourmash_plugin_directsketch-0.2.1/tests/test-data/test.zip
+-rw-r--r--   0      501       20    11413 2024-05-06 22:31:50.000000 sourmash_plugin_directsketch-0.2.1/tests/test_gbsketch.py
+-rw-r--r--   0      501       20    63427 2024-05-08 21:52:08.000000 sourmash_plugin_directsketch-0.2.1/Cargo.lock
+-rw-r--r--   0      501       20     1003 2024-05-08 16:20:18.000000 sourmash_plugin_directsketch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 sourmash_plugin_directsketch-0.2.1/PKG-INFO
```

### Comparing `sourmash_plugin_directsketch-0.2.0/Cargo.toml` & `sourmash_plugin_directsketch-0.2.1/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [package]
 name = "sourmash_plugin_directsketch"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 
 [lib]
 name = "sourmash_plugin_directsketch"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `sourmash_plugin_directsketch-0.2.0/.github/workflows/build-test.yml` & `sourmash_plugin_directsketch-0.2.1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/.gitignore` & `sourmash_plugin_directsketch-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/LICENSE` & `sourmash_plugin_directsketch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/README.md` & `sourmash_plugin_directsketch-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.1/out_fastas/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/src/directsketch.rs` & `sourmash_plugin_directsketch-0.2.1/src/directsketch.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 use std::fs::{self, create_dir_all};
 use std::io::Cursor;
 use std::path::Path;
 use std::sync::Arc;
 use tokio::fs::File;
 use tokio::io::{AsyncWriteExt, BufWriter};
 use tokio::sync::Semaphore;
-use tokio::time::Duration;
 use tokio_util::compat::Compat;
 
 use pyo3::prelude::*;
 
 use sourmash::manifest::{Manifest, Record};
 use sourmash::signature::Signature;
 
@@ -611,19 +610,16 @@
     let mut handles = Vec::new();
     let sig_handle = sigwriter_handle(recv_sigs, output_sigs, error_sender.clone());
     let failures_handle = failures_handle(failed_csv, recv_failed, error_sender.clone());
     handles.push(sig_handle);
     handles.push(failures_handle);
 
     // // Worker tasks
-    // let client = Client::new();
     let semaphore = Arc::new(Semaphore::new(3)); // Limiting concurrent downloads
     let client = Arc::new(Client::new());
-    // let semaphore = Arc::new(Semaphore::new(3)); // Allows up to 3 concurrent tasks
-    let mut interval = tokio::time::interval(Duration::from_secs(1));
 
     // Open the file containing the accessions synchronously
     let (accession_info, n_accs) = load_accession_info(input_csv)?;
     if n_accs == 0 {
         bail!("No accessions to download and sketch.")
     }
 
@@ -634,41 +630,41 @@
         Err(e) => {
             bail!("Failed to parse params string: {}", e);
         }
     };
     let dna_sig_templates = build_siginfo(&params_vec, "DNA");
     let prot_sig_templates = build_siginfo(&params_vec, "protein");
 
-    // report every 5 percent (or ever 1, whichever is larger)
-    let reporting_threshold = std::cmp::max(n_accs / 20, 1);
+    // report every 1 percent (or every 1, whichever is larger)
+    let reporting_threshold = std::cmp::max(n_accs / 100, 1);
 
     for (i, accinfo) in accession_info.into_iter().enumerate() {
         py.check_signals()?; // If interrupted, return an Err automatically
-        interval.tick().await; // Wait for the next interval tick before continuing
         let semaphore_clone = Arc::clone(&semaphore);
         let client_clone = Arc::clone(&client);
         let send_sigs = send_sigs.clone();
         let send_failed = send_failed.clone();
         let download_path_clone = download_path.clone(); // Clone the path for each task
         let send_errors = error_sender.clone();
 
         let dna_sigs = dna_sig_templates.clone();
         let prot_sigs = prot_sig_templates.clone();
 
-        if (i + 1) % reporting_threshold == 0 {
-            let percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
-            println!(
-                "Starting accession {}/{} ({}%)",
-                (i + 1),
-                n_accs,
-                percent_processed
-            );
-        }
         tokio::spawn(async move {
             let _permit = semaphore_clone.acquire().await;
+            // Report when the permit is available and processing begins
+            if (i + 1) % reporting_threshold == 0 {
+                let percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
+                println!(
+                    "Starting accession {}/{} ({}%)",
+                    (i + 1),
+                    n_accs,
+                    percent_processed
+                );
+            }
             // Perform download and sketch
             let result = dl_sketch_accession(
                 &client_clone,
                 accinfo.accession.clone(),
                 accinfo.name.clone(),
                 &download_path_clone,
                 Some(retry_times),
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 use anyhow::{anyhow, bail, Context, Error, Result}; use async_zip::base::
 write::ZipFileWriter; use async_zip::{Compression, ZipDateTime,
 ZipEntryBuilder}; use camino::Utf8PathBuf as PathBuf; use chrono::Utc; use
 needletail::parse_fastx_reader; use regex::Regex; use reqwest::Client; use
 std::collections::HashMap; use std::fs::{self, create_dir_all}; use std::io::
 Cursor; use std::path::Path; use std::sync::Arc; use tokio::fs::File; use
-tokio::io::{AsyncWriteExt, BufWriter}; use tokio::sync::Semaphore; use tokio::
-time::Duration; use tokio_util::compat::Compat; use pyo3::prelude::*; use
-sourmash::manifest::{Manifest, Record}; use sourmash::signature::Signature; use
-crate::utils::{build_siginfo, load_accession_info, parse_params_str}; #[allow
-(dead_code)] enum GenBankFileType { Genomic, Protein, AssemblyReport, Checksum,
-} impl GenBankFileType { fn suffix(&self) -> &'static str { match self
+tokio::io::{AsyncWriteExt, BufWriter}; use tokio::sync::Semaphore; use
+tokio_util::compat::Compat; use pyo3::prelude::*; use sourmash::manifest::
+{Manifest, Record}; use sourmash::signature::Signature; use crate::utils::
+{build_siginfo, load_accession_info, parse_params_str}; #[allow(dead_code)]
+enum GenBankFileType { Genomic, Protein, AssemblyReport, Checksum, } impl
+GenBankFileType { fn suffix(&self) -> &'static str { match self
 { GenBankFileType::Genomic => "_genomic.fna.gz", GenBankFileType::Protein =>
 "_protein.faa.gz", GenBankFileType::AssemblyReport => "_assembly_report.txt",
 GenBankFileType::Checksum => "md5checksums.txt", } } //use for checksums fn
 server_filename(&self, full_name: &str) -> String { format!("{}{}", full_name,
 self.suffix()) } fn filename_to_write(&self, accession: &str) -> String { match
 self { GenBankFileType::Checksum => format!("{}_{}", accession, self.suffix()),
 _ => format!("{}{}", accession, self.suffix()), } } fn url(&self, base_url:
@@ -195,51 +195,47 @@
 speeds things up let (send_sigs, recv_sigs) = tokio::sync::mpsc::channel::
 Signature>>(4); let (send_failed, recv_failed) = tokio::sync::mpsc::channel::
 (4); // // Error channel for handling task errors let (error_sender, mut
 error_receiver) = tokio::sync::mpsc::channel::(1); // // // Set up collector/
 writing tasks let mut handles = Vec::new(); let sig_handle = sigwriter_handle
 (recv_sigs, output_sigs, error_sender.clone()); let failures_handle =
 failures_handle(failed_csv, recv_failed, error_sender.clone()); handles.push
-(sig_handle); handles.push(failures_handle); // // Worker tasks // let client =
-Client::new(); let semaphore = Arc::new(Semaphore::new(3)); // Limiting
-concurrent downloads let client = Arc::new(Client::new()); // let semaphore =
-Arc::new(Semaphore::new(3)); // Allows up to 3 concurrent tasks let mut
-interval = tokio::time::interval(Duration::from_secs(1)); // Open the file
-containing the accessions synchronously let (accession_info, n_accs) =
-load_accession_info(input_csv)?; if n_accs == 0 { bail!("No accessions to
-download and sketch.") } // // parse param string into params_vec, print error
-if fail let param_result = parse_params_str(param_str); let params_vec = match
-param_result { Ok(params) => params, Err(e) => { bail!("Failed to parse params
-string: {}", e); } }; let dna_sig_templates = build_siginfo(&params_vec,
-"DNA"); let prot_sig_templates = build_siginfo(&params_vec, "protein"); /
-/ report every 5 percent (or ever 1, whichever is larger) let
-reporting_threshold = std::cmp::max(n_accs / 20, 1); for (i, accinfo) in
-accession_info.into_iter().enumerate() { py.check_signals()?; // If
-interrupted, return an Err automatically interval.tick().await; // Wait for the
-next interval tick before continuing let semaphore_clone = Arc::clone
-(&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
+(sig_handle); handles.push(failures_handle); // // Worker tasks let semaphore =
+Arc::new(Semaphore::new(3)); // Limiting concurrent downloads let client =
+Arc::new(Client::new()); // Open the file containing the accessions
+synchronously let (accession_info, n_accs) = load_accession_info(input_csv)?;
+if n_accs == 0 { bail!("No accessions to download and sketch.") } // // parse
+param string into params_vec, print error if fail let param_result =
+parse_params_str(param_str); let params_vec = match param_result { Ok(params)
+=> params, Err(e) => { bail!("Failed to parse params string: {}", e); } }; let
+dna_sig_templates = build_siginfo(&params_vec, "DNA"); let prot_sig_templates =
+build_siginfo(&params_vec, "protein"); // report every 1 percent (or every 1,
+whichever is larger) let reporting_threshold = std::cmp::max(n_accs / 100, 1);
+for (i, accinfo) in accession_info.into_iter().enumerate() { py.check_signals
+()?; // If interrupted, return an Err automatically let semaphore_clone = Arc::
+clone(&semaphore); let client_clone = Arc::clone(&client); let send_sigs =
 send_sigs.clone(); let send_failed = send_failed.clone(); let
 download_path_clone = download_path.clone(); // Clone the path for each task
 let send_errors = error_sender.clone(); let dna_sigs = dna_sig_templates.clone
-(); let prot_sigs = prot_sig_templates.clone(); if (i + 1) %
-reporting_threshold == 0 { let percent_processed = (((i + 1) as f64 / n_accs as
-f64) * 100.0).round(); println!( "Starting accession {}/{} ({}%)", (i + 1),
-n_accs, percent_processed ); } tokio::spawn(async move { let _permit =
-semaphore_clone.acquire().await; // Perform download and sketch let result =
-dl_sketch_accession( &client_clone, accinfo.accession.clone(),
-accinfo.name.clone(), &download_path_clone, Some(retry_times), keep_fastas,
-dna_sigs, prot_sigs, genomes_only, proteomes_only, download_only, ) .await;
-match result { Ok((sigs, failed_downloads)) => { if let Err(e) = send_sigs.send
-(sigs).await { eprintln!("Failed to send signatures: {}", e); let _ =
-send_errors.send(e.into()).await; // Send the error through the channel } for
-fail in failed_downloads { if let Err(e) = send_failed.send(fail).await
-{ eprintln!("Failed to send failed download info: {}", e); let _ =
-send_errors.send(e.into()).await; // Send the error through the channel } } }
-Err(e) => { let _ = send_errors.send(e).await; } } drop(send_errors); }); } /
-/ drop senders as we're done sending data drop(send_sigs); drop(send_failed);
-drop(error_sender); // Wait for all tasks to complete for handle in handles
-{ if let Err(e) = handle.await { eprintln!("A task encountered an error: {}",
-e); } } // // Handle errors received from the error channel while let Some
-(error) = error_receiver.recv().await { eprintln!("Error: {}", error); // Check
-if the error message contains "No signatures written" if error.to_string
-().contains("No signatures written") & !download_only { bail!("{}.", error); }
-} Ok(()) }
+(); let prot_sigs = prot_sig_templates.clone(); tokio::spawn(async move { let
+_permit = semaphore_clone.acquire().await; // Report when the permit is
+available and processing begins if (i + 1) % reporting_threshold == 0 { let
+percent_processed = (((i + 1) as f64 / n_accs as f64) * 100.0).round();
+println!( "Starting accession {}/{} ({}%)", (i + 1), n_accs, percent_processed
+); } // Perform download and sketch let result = dl_sketch_accession
+( &client_clone, accinfo.accession.clone(), accinfo.name.clone(),
+&download_path_clone, Some(retry_times), keep_fastas, dna_sigs, prot_sigs,
+genomes_only, proteomes_only, download_only, ) .await; match result { Ok((sigs,
+failed_downloads)) => { if let Err(e) = send_sigs.send(sigs).await { eprintln!
+("Failed to send signatures: {}", e); let _ = send_errors.send(e.into()).await;
+// Send the error through the channel } for fail in failed_downloads { if let
+Err(e) = send_failed.send(fail).await { eprintln!("Failed to send failed
+download info: {}", e); let _ = send_errors.send(e.into()).await; // Send the
+error through the channel } } } Err(e) => { let _ = send_errors.send(e).await;
+} } drop(send_errors); }); } // drop senders as we're done sending data drop
+(send_sigs); drop(send_failed); drop(error_sender); // Wait for all tasks to
+complete for handle in handles { if let Err(e) = handle.await { eprintln!("A
+task encountered an error: {}", e); } } // // Handle errors received from the
+error channel while let Some(error) = error_receiver.recv().await { eprintln!
+("Error: {}", error); // Check if the error message contains "No signatures
+written" if error.to_string().contains("No signatures written") &
+!download_only { bail!("{}.", error); } } Ok(()) }
```

### Comparing `sourmash_plugin_directsketch-0.2.0/src/lib.rs` & `sourmash_plugin_directsketch-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/src/python/sourmash_plugin_directsketch/__init__.py` & `sourmash_plugin_directsketch-0.2.1/src/python/sourmash_plugin_directsketch/__init__.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/src/utils.rs` & `sourmash_plugin_directsketch-0.2.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/test.zip` & `sourmash_plugin_directsketch-0.2.1/test.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,5 +1,5 @@
 Zip file size: 38326 bytes, number of entries: 3
-?---------  6.3 unx    15043 b- stor 24-May-08 14:36 signatures/d900308fb443444ff6127b7bfbd463c1.sig.gz
-?---------  6.3 unx    22245 b- stor 24-May-08 14:36 signatures/8196cc69b814cab9fc3c7e9eed861bf6.sig.gz
-?---------  6.3 unx      546 b- stor 24-May-08 14:36 SOURMASH-MANIFEST.csv
+?---------  6.3 unx    15043 b- stor 24-May-08 21:42 signatures/d900308fb443444ff6127b7bfbd463c1.sig.gz
+?---------  6.3 unx    22245 b- stor 24-May-08 21:42 signatures/8196cc69b814cab9fc3c7e9eed861bf6.sig.gz
+?---------  6.3 unx      546 b- stor 24-May-08 21:42 SOURMASH-MANIFEST.csv
 3 files, 37834 bytes uncompressed, 37834 bytes compressed:  0.0%
```

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/sourmash_tst_utils.py` & `sourmash_plugin_directsketch-0.2.1/tests/sourmash_tst_utils.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000175555.1.sig.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000175555.1.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.protein.sig.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.protein.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/GCA_000961135.2.sig.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/GCA_000961135.2.sig.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/out_fastas/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000175555.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000337115.1_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_assembly_report.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_md5checksums.txt`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_000961135.2_protein.faa.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/outputs/GCA_001950595.1_genomic.fna.gz`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test-data/test.zip` & `sourmash_plugin_directsketch-0.2.1/tests/test-data/test.zip`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/tests/test_gbsketch.py` & `sourmash_plugin_directsketch-0.2.1/tests/test_gbsketch.py`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/Cargo.lock` & `sourmash_plugin_directsketch-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1811,15 +1811,15 @@
  "vec-collections",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "sourmash_plugin_directsketch"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "async_zip",
  "camino",
  "chrono",
  "csv",
  "futures",
```

### Comparing `sourmash_plugin_directsketch-0.2.0/pyproject.toml` & `sourmash_plugin_directsketch-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_directsketch-0.2.0/PKG-INFO` & `sourmash_plugin_directsketch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sourmash_plugin_directsketch
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: sourmash >=4.8.5, <5
 Requires-Dist: pytest >=6.2.4, <8.3.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.12, <6.0 ; extra == 'test'
 Requires-Dist: pytest-xdist ; extra == 'test'
```

