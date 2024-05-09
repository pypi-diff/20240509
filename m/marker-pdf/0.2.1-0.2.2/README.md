# Comparing `tmp/marker_pdf-0.2.1.tar.gz` & `tmp/marker_pdf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.2.1.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.2.tar", max compression
```

## Comparing `marker_pdf-0.2.1.tar` & `marker_pdf-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.2.1/LICENSE
--rw-r--r--   0        0        0    12668 2024-05-09 17:58:32.978922 marker_pdf-0.2.1/README.md
--rwxr-xr-x   0        0        0      541 2023-12-19 21:40:35.305844 marker_pdf-0.2.1/chunk_convert.py
--rwxr-xr-x   0        0        0     1151 2024-05-09 16:07:14.765161 marker_pdf-0.2.1/chunk_convert.sh
--rwxr-xr-x   0        0        0     4743 2024-05-07 17:49:43.674850 marker_pdf-0.2.1/convert.py
--rwxr-xr-x   0        0        0     1246 2024-05-08 19:28:45.549038 marker_pdf-0.2.1/convert_single.py
--rw-r--r--   0        0        0     1376 2024-05-09 14:37:06.538810 marker_pdf-0.2.1/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.2.1/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4405 2024-05-08 17:44:54.251299 marker_pdf-0.2.1/marker/cleaners/code.py
--rw-r--r--   0        0        0      950 2024-05-07 20:26:01.091879 marker_pdf-0.2.1/marker/cleaners/fontstyle.py
--rw-r--r--   0        0        0     2766 2024-05-07 20:26:12.412431 marker_pdf-0.2.1/marker/cleaners/headers.py
--rw-r--r--   0        0        0     2456 2024-05-07 19:20:29.345524 marker_pdf-0.2.1/marker/cleaners/headings.py
--rw-r--r--   0        0        0      248 2024-05-03 21:25:54.927963 marker_pdf-0.2.1/marker/cleaners/text.py
--rw-r--r--   0        0        0     5166 2024-05-09 17:45:33.634950 marker_pdf-0.2.1/marker/convert.py
--rw-r--r--   0        0        0     2450 2024-04-30 19:24:46.032856 marker_pdf-0.2.1/marker/debug/data.py
--rw-r--r--   0        0        0     7884 2024-05-08 19:28:39.435042 marker_pdf-0.2.1/marker/equations/equations.py
--rw-r--r--   0        0        0     1549 2024-05-08 19:28:39.424935 marker_pdf-0.2.1/marker/equations/inference.py
--rw-r--r--   0        0        0     2594 2024-05-07 20:51:37.990183 marker_pdf-0.2.1/marker/images/extract.py
--rw-r--r--   0        0        0      473 2024-05-07 17:35:52.062308 marker_pdf-0.2.1/marker/images/save.py
--rw-r--r--   0        0        0     1928 2024-05-09 17:56:48.915437 marker_pdf-0.2.1/marker/layout/layout.py
--rw-r--r--   0        0        0     2488 2024-05-09 17:57:11.112357 marker_pdf-0.2.1/marker/layout/order.py
--rw-r--r--   0        0        0      396 2024-05-01 20:56:02.059168 marker_pdf-0.2.1/marker/logger.py
--rw-r--r--   0        0        0     2085 2024-05-03 23:32:22.398344 marker_pdf-0.2.1/marker/models.py
--rw-r--r--   0        0        0      888 2024-05-09 17:56:54.611918 marker_pdf-0.2.1/marker/ocr/detection.py
--rw-r--r--   0        0        0     2468 2024-05-07 05:37:29.807989 marker_pdf-0.2.1/marker/ocr/heuristics.py
--rw-r--r--   0        0        0      959 2024-05-03 23:32:22.393388 marker_pdf-0.2.1/marker/ocr/lang.py
--rw-r--r--   0        0        0     5188 2024-05-08 19:24:58.173812 marker_pdf-0.2.1/marker/ocr/recognition.py
--rw-r--r--   0        0        0     2180 2024-05-01 20:19:00.486329 marker_pdf-0.2.1/marker/ocr/tesseract.py
--rw-r--r--   0        0        0      258 2024-05-02 23:16:18.893143 marker_pdf-0.2.1/marker/ocr/utils.py
--rw-r--r--   0        0        0     1265 2024-05-07 18:48:43.948534 marker_pdf-0.2.1/marker/output.py
--rw-r--r--   0        0        0     3932 2024-05-07 19:36:28.635033 marker_pdf-0.2.1/marker/pdf/extract_text.py
--rw-r--r--   0        0        0      817 2024-05-07 02:48:52.757068 marker_pdf-0.2.1/marker/pdf/images.py
--rw-r--r--   0        0        0     2339 2024-05-07 19:21:25.071249 marker_pdf-0.2.1/marker/pdf/utils.py
--rw-r--r--   0        0        0     3904 2024-05-08 19:28:39.432619 marker_pdf-0.2.1/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     7103 2024-05-09 16:45:38.707953 marker_pdf-0.2.1/marker/postprocessors/markdown.py
--rw-r--r--   0        0        0     4977 2024-05-07 20:27:15.110937 marker_pdf-0.2.1/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     2849 2024-05-03 13:40:49.822158 marker_pdf-0.2.1/marker/schema/bbox.py
--rw-r--r--   0        0        0     3259 2024-05-08 16:58:04.155413 marker_pdf-0.2.1/marker/schema/block.py
--rw-r--r--   0        0        0      502 2024-05-02 20:26:11.294687 marker_pdf-0.2.1/marker/schema/merged.py
--rw-r--r--   0        0        0     1618 2024-05-08 17:45:07.502133 marker_pdf-0.2.1/marker/schema/page.py
--rw-r--r--   0        0        0     4204 2024-05-09 17:53:04.646429 marker_pdf-0.2.1/marker/settings.py
--rw-r--r--   0        0        0     3384 2024-05-07 19:20:29.343760 marker_pdf-0.2.1/marker/tables/cells.py
--rw-r--r--   0        0        0     7178 2024-05-08 02:12:14.849108 marker_pdf-0.2.1/marker/tables/table.py
--rw-r--r--   0        0        0     1128 2024-05-07 05:24:59.879003 marker_pdf-0.2.1/marker/tables/utils.py
--rw-r--r--   0        0        0      156 2024-05-09 17:43:20.364396 marker_pdf-0.2.1/marker/utils.py
--rw-r--r--   0        0        0     1319 2024-05-09 17:59:12.449026 marker_pdf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    14199 1970-01-01 00:00:00.000000 marker_pdf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.2.2/LICENSE
+-rw-r--r--   0        0        0    13302 2024-05-09 18:42:22.504099 marker_pdf-0.2.2/README.md
+-rwxr-xr-x   0        0        0      541 2023-12-19 21:40:35.305844 marker_pdf-0.2.2/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-09 16:07:14.765161 marker_pdf-0.2.2/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4852 2024-05-09 19:04:27.934570 marker_pdf-0.2.2/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-08 19:28:45.549038 marker_pdf-0.2.2/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-09 14:37:06.538810 marker_pdf-0.2.2/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.2.2/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4405 2024-05-08 17:44:54.251299 marker_pdf-0.2.2/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-07 20:26:01.091879 marker_pdf-0.2.2/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-07 20:26:12.412431 marker_pdf-0.2.2/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-07 19:20:29.345524 marker_pdf-0.2.2/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-03 21:25:54.927963 marker_pdf-0.2.2/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5164 2024-05-09 18:04:24.927228 marker_pdf-0.2.2/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-04-30 19:24:46.032856 marker_pdf-0.2.2/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-08 19:28:39.435042 marker_pdf-0.2.2/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-08 19:28:39.424935 marker_pdf-0.2.2/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-07 20:51:37.990183 marker_pdf-0.2.2/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-07 17:35:52.062308 marker_pdf-0.2.2/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-09 17:56:48.915437 marker_pdf-0.2.2/marker/layout/layout.py
+-rw-r--r--   0        0        0     2516 2024-05-09 18:50:44.232751 marker_pdf-0.2.2/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-01 20:56:02.059168 marker_pdf-0.2.2/marker/logger.py
+-rw-r--r--   0        0        0     2178 2024-05-09 18:19:52.086803 marker_pdf-0.2.2/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-09 17:56:54.611918 marker_pdf-0.2.2/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-07 05:37:29.807989 marker_pdf-0.2.2/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0     1223 2024-05-09 18:28:58.770602 marker_pdf-0.2.2/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5742 2024-05-09 18:45:41.515716 marker_pdf-0.2.2/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-01 20:19:00.486329 marker_pdf-0.2.2/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-02 23:16:18.893143 marker_pdf-0.2.2/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1265 2024-05-07 18:48:43.948534 marker_pdf-0.2.2/marker/output.py
+-rw-r--r--   0        0        0     3932 2024-05-07 19:36:28.635033 marker_pdf-0.2.2/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-07 02:48:52.757068 marker_pdf-0.2.2/marker/pdf/images.py
+-rw-r--r--   0        0        0     2339 2024-05-07 19:21:25.071249 marker_pdf-0.2.2/marker/pdf/utils.py
+-rw-r--r--   0        0        0     3904 2024-05-08 19:28:39.432619 marker_pdf-0.2.2/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7103 2024-05-09 16:45:38.707953 marker_pdf-0.2.2/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-07 20:27:15.110937 marker_pdf-0.2.2/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-03 13:40:49.822158 marker_pdf-0.2.2/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-08 16:58:04.155413 marker_pdf-0.2.2/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-02 20:26:11.294687 marker_pdf-0.2.2/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-08 17:45:07.502133 marker_pdf-0.2.2/marker/schema/page.py
+-rw-r--r--   0        0        0     4236 2024-05-09 18:50:32.918877 marker_pdf-0.2.2/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-07 19:20:29.343760 marker_pdf-0.2.2/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-08 02:12:14.849108 marker_pdf-0.2.2/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-07 05:24:59.879003 marker_pdf-0.2.2/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-09 17:43:20.364396 marker_pdf-0.2.2/marker/utils.py
+-rw-r--r--   0        0        0     1319 2024-05-09 18:02:48.805156 marker_pdf-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    14833 1970-01-01 00:00:00.000000 marker_pdf-0.2.2/PKG-INFO
```

### Comparing `marker_pdf-0.2.1/LICENSE` & `marker_pdf-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/README.md` & `marker_pdf-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -137,14 +137,25 @@
 - `METADATA_FILE` is an optional path to a json file with metadata about the pdfs.  See above for the format.
 - `NUM_DEVICES` is the number of GPUs to use.  Should be `2` or greater.
 - `NUM_WORKERS` is the number of parallel processes to run on each GPU.  Per-GPU parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK`.
 - `MIN_LENGTH` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
 
 Note that the env variables above are specific to this script, and cannot be set in `local.env`.
 
+# Important settings/Troubleshooting
+
+There are some settings that you may find especially useful if things aren't working the way you expect:
+
+- `OCR_ALL_PAGES` - set this to true to force OCR all pages.  This can be very useful if the table layouts aren't recognized properly by default, or if there is garbled text.
+- `TORCH_DEVICE` - set this to force marker to use a given torch device for inference.
+- `OCR_ENGINE` - can set this to `surya` or `ocrmypdf`.
+- `DEBUG` - setting this to `True` shows ray logs when converting multiple pdfs
+
+In general, if output is not what you expect, trying to OCR the PDF is a good first step.
+
 # Benchmarks
 
 Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.  It's noisy, but at least directionally correct.
 
 Benchmarks show that marker is 4x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
 
 **Speed**
@@ -159,15 +170,15 @@
 First 3 are non-arXiv books, last 3 are arXiv papers.
 
 | Method | multicolcnn.pdf | switch_trans.pdf | thinkpython.pdf | thinkos.pdf | thinkdsp.pdf | crowd.pdf |
 |--------|-----------------|------------------|-----------------|-------------|--------------|-----------|
 | marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
 | nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
-Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `5.1GB` for marker.  Benchmarks were run on an A6000 Ada.
+Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `4.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
 Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
```

### Comparing `marker_pdf-0.2.1/chunk_convert.py` & `marker_pdf-0.2.2/chunk_convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/chunk_convert.sh` & `marker_pdf-0.2.2/chunk_convert.sh`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/convert.py` & `marker_pdf-0.2.2/convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,37 +16,38 @@
 import traceback
 import json
 
 configure_logging()
 
 
 @ray.remote(num_cpus=settings.RAY_CORES_PER_WORKER, num_gpus=.05 if settings.CUDA else 0)
-def process_single_pdf(fname: str, out_folder: str, model_refs, metadata: Optional[Dict] = None, min_length: Optional[int] = None):
+def process_single_pdf(filepath: str, out_folder: str, model_refs, metadata: Optional[Dict] = None, min_length: Optional[int] = None):
+    fname = os.path.basename(filepath)
     if markdown_exists(out_folder, fname):
         return
     try:
         # Skip trying to convert files that don't have a lot of embedded text
         # This can indicate that they were scanned, and not OCRed properly
         # Usually these files are not recent/high-quality
         if min_length:
-            filetype = find_filetype(fname)
+            filetype = find_filetype(filepath)
             if filetype == "other":
                 return 0
 
-            length = get_length_of_text(fname)
+            length = get_length_of_text(filepath)
             if length < min_length:
                 return
 
-        full_text, images, out_metadata = convert_single_pdf(fname, model_refs, metadata=metadata)
+        full_text, images, out_metadata = convert_single_pdf(filepath, model_refs, metadata=metadata)
         if len(full_text.strip()) > 0:
             save_markdown(out_folder, fname, full_text, images, out_metadata)
         else:
-            print(f"Empty file: {fname}.  Could not convert.")
+            print(f"Empty file: {filepath}.  Could not convert.")
     except Exception as e:
-        print(f"Error converting {fname}: {e}")
+        print(f"Error converting {filepath}: {e}")
         print(traceback.format_exc())
 
 
 def main():
     parser = argparse.ArgumentParser(description="Convert multiple pdfs to markdown.")
     parser.add_argument("in_folder", help="Input folder with pdfs.")
     parser.add_argument("out_folder", help="Output folder")
@@ -58,14 +59,15 @@
     parser.add_argument("--min_length", type=int, default=None, help="Minimum length of pdf to convert")
 
     args = parser.parse_args()
 
     in_folder = os.path.abspath(args.in_folder)
     out_folder = os.path.abspath(args.out_folder)
     files = [os.path.join(in_folder, f) for f in os.listdir(in_folder)]
+    files = [f for f in files if os.path.isfile(f)]
     os.makedirs(out_folder, exist_ok=True)
 
     # Handle chunks if we're processing in parallel
     # Ensure we get all files into a chunk
     chunk_size = math.ceil(len(files) / args.num_chunks)
     start_idx = args.chunk_idx * chunk_size
     end_idx = start_idx + chunk_size
@@ -96,20 +98,20 @@
 
     # Dynamically set GPU allocation per task based on GPU ram
     gpu_frac = settings.VRAM_PER_TASK / settings.INFERENCE_RAM if settings.CUDA else 0
 
     print(f"Converting {len(files_to_convert)} pdfs in chunk {args.chunk_idx + 1}/{args.num_chunks} with {total_processes} processes, and storing in {out_folder}")
     futures = [
         process_single_pdf.options(num_gpus=gpu_frac).remote(
-            filename,
+            filepath,
             out_folder,
             model_refs,
-            metadata=metadata.get(os.path.basename(filename)),
+            metadata=metadata.get(os.path.basename(filepath)),
             min_length=args.min_length
-        ) for filename in files_to_convert
+        ) for filepath in files_to_convert
     ]
 
     # Run all ray conversion tasks
     progress_bar = tqdm(total=len(futures))
     while len(futures) > 0:
         finished, futures = ray.wait(
             futures, timeout=7.0
```

### Comparing `marker_pdf-0.2.1/convert_single.py` & `marker_pdf-0.2.2/convert_single.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/benchmark/scoring.py` & `marker_pdf-0.2.2/marker/benchmark/scoring.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/cleaners/code.py` & `marker_pdf-0.2.2/marker/cleaners/code.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/cleaners/fontstyle.py` & `marker_pdf-0.2.2/marker/cleaners/fontstyle.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/cleaners/headers.py` & `marker_pdf-0.2.2/marker/cleaners/headers.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/cleaners/headings.py` & `marker_pdf-0.2.2/marker/cleaners/headings.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/convert.py` & `marker_pdf-0.2.2/marker/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import warnings
-
-from marker.utils import flush_cuda_memory
-
 warnings.filterwarnings("ignore", category=UserWarning) # Filter torch pytree user warnings
 
 import pypdfium2 as pdfium
 from PIL import Image
 
+from marker.utils import flush_cuda_memory
 from marker.tables.table import format_tables
 from marker.debug.data import dump_bbox_debug_data
 from marker.layout.layout import surya_layout, annotate_block_types
 from marker.layout.order import surya_order, sort_blocks_in_reading_order
 from marker.ocr.lang import replace_langs_with_codes, validate_langs
 from marker.ocr.detection import surya_detection
 from marker.ocr.recognition import run_ocr
```

### Comparing `marker_pdf-0.2.1/marker/debug/data.py` & `marker_pdf-0.2.2/marker/debug/data.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/equations/equations.py` & `marker_pdf-0.2.2/marker/equations/equations.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/equations/inference.py` & `marker_pdf-0.2.2/marker/equations/inference.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/images/extract.py` & `marker_pdf-0.2.2/marker/images/extract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/layout/layout.py` & `marker_pdf-0.2.2/marker/layout/layout.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/layout/order.py` & `marker_pdf-0.2.2/marker/layout/order.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def surya_order(doc, pages: List[Page], order_model, batch_multiplier=1):
     images = [render_image(doc[pnum], dpi=settings.SURYA_ORDER_DPI) for pnum in range(len(pages))]
 
     # Get bboxes for all pages
     bboxes = []
     for page in pages:
-        bbox = [b.bbox for b in page.layout.bboxes]
+        bbox = [b.bbox for b in page.layout.bboxes][:settings.ORDER_MAX_BBOXES]
         bboxes.append(bbox)
 
     processor = order_model.processor
     order_results = batch_ordering(images, bboxes, order_model, processor, batch_size=get_batch_size() * batch_multiplier)
     for page, order_result in zip(pages, order_results):
         page.order = order_result
```

### Comparing `marker_pdf-0.2.1/marker/models.py` & `marker_pdf-0.2.2/marker/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,11 +46,13 @@
 
 def load_all_models(langs=None):
     # langs is optional list of languages to prune from recognition MoE model
     detection = setup_detection_model()
     layout = setup_layout_model()
     order = setup_order_model()
     edit = load_editing_model()
-    ocr = setup_recognition_model(langs) if settings.OCR_ENGINE == "surya" else None
+
+    # Only load recognition model if we'll need it for all pdfs
+    ocr = setup_recognition_model(langs) if (settings.OCR_ENGINE == "surya" and settings.OCR_ALL_PAGES) else None
     texify = setup_texify_model()
     model_lst = [texify, layout, order, edit, detection, ocr]
-    return model_lst
+    return model_lst
```

### Comparing `marker_pdf-0.2.1/marker/ocr/detection.py` & `marker_pdf-0.2.2/marker/ocr/detection.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/ocr/heuristics.py` & `marker_pdf-0.2.2/marker/ocr/heuristics.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/ocr/lang.py` & `marker_pdf-0.2.2/marker/ocr/lang.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+from typing import List
+
 from surya.languages import CODE_TO_LANGUAGE, LANGUAGE_TO_CODE
+from surya.model.recognition.tokenizer import _tokenize as lang_tokenize
 
 from marker.ocr.tesseract import LANGUAGE_TO_TESSERACT_CODE, TESSERACT_CODE_TO_LANGUAGE
 from marker.settings import settings
 
 
+def langs_to_ids(langs: List[str]):
+    unique_langs = list(set(langs))
+    _, lang_tokens = lang_tokenize("", unique_langs)
+    return lang_tokens
+
+
 def replace_langs_with_codes(langs):
     if settings.OCR_ENGINE == "surya":
         for i, lang in enumerate(langs):
-            if lang in LANGUAGE_TO_CODE:
-                langs[i] = LANGUAGE_TO_CODE[lang]
+            if lang.title() in LANGUAGE_TO_CODE:
+                langs[i] = LANGUAGE_TO_CODE[lang.title()]
     else:
         for i, lang in enumerate(langs):
             if lang in LANGUAGE_TO_CODE:
                 langs[i] = LANGUAGE_TO_TESSERACT_CODE[lang]
     return langs
```

### Comparing `marker_pdf-0.2.1/marker/ocr/recognition.py` & `marker_pdf-0.2.2/marker/ocr/recognition.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 import pypdfium2 as pdfium
 import io
 from concurrent.futures import ThreadPoolExecutor
 
 from surya.ocr import run_recognition
 
+from marker.models import setup_recognition_model
 from marker.ocr.heuristics import should_ocr_page, no_text_found, detect_bad_ocr
+from marker.ocr.lang import langs_to_ids
 from marker.pdf.images import render_image
 from marker.schema.page import Page
 from marker.schema.block import Block, Line, Span
 from marker.settings import settings
 from marker.pdf.extract_text import get_text_blocks
 
 
 def get_batch_size():
     if settings.RECOGNITION_BATCH_SIZE is not None:
         return settings.RECOGNITION_BATCH_SIZE
     elif settings.TORCH_DEVICE_MODEL == "cuda":
-        return 64
+        return 32
     elif settings.TORCH_DEVICE_MODEL == "mps":
         return 32
     return 32
 
 
 def run_ocr(doc, pages: List[Page], langs: List[str], rec_model, batch_multiplier=1) -> (List[Page], Dict):
     ocr_pages = 0
@@ -33,19 +35,33 @@
     ocr_idxs = []
     for pnum, page in enumerate(pages):
         ocr_needed = should_ocr_page(page, no_text)
         if ocr_needed:
             ocr_idxs.append(pnum)
             ocr_pages += 1
 
+    # No pages need OCR
+    if ocr_pages == 0:
+        return pages, {"ocr_pages": 0, "ocr_failed": 0, "ocr_success": 0, "ocr_engine": "none"}
+
     ocr_method = settings.OCR_ENGINE
     if ocr_method is None:
         return pages, {"ocr_pages": 0, "ocr_failed": 0, "ocr_success": 0, "ocr_engine": "none"}
     elif ocr_method == "surya":
+        # Load model just in time if we're not OCRing everything
+        del_rec_model = False
+        if rec_model is None:
+            lang_tokens = langs_to_ids(langs)
+            rec_model = setup_recognition_model(lang_tokens)
+            del_rec_model = True
+
         new_pages = surya_recognition(doc, ocr_idxs, langs, rec_model, pages, batch_multiplier=batch_multiplier)
+
+        if del_rec_model:
+            del rec_model
     elif ocr_method == "ocrmypdf":
         new_pages = tesseract_recognition(doc, ocr_idxs, langs)
     else:
         raise ValueError(f"Unknown OCR method {ocr_method}")
 
     for orig_idx, page in zip(ocr_idxs, new_pages):
         if detect_bad_ocr(page.prelim_text) or len(page.prelim_text) == 0:
```

### Comparing `marker_pdf-0.2.1/marker/ocr/tesseract.py` & `marker_pdf-0.2.2/marker/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/output.py` & `marker_pdf-0.2.2/marker/output.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/pdf/extract_text.py` & `marker_pdf-0.2.2/marker/pdf/extract_text.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/pdf/images.py` & `marker_pdf-0.2.2/marker/pdf/images.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/pdf/utils.py` & `marker_pdf-0.2.2/marker/pdf/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/postprocessors/editor.py` & `marker_pdf-0.2.2/marker/postprocessors/editor.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/postprocessors/markdown.py` & `marker_pdf-0.2.2/marker/postprocessors/markdown.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/postprocessors/t5.py` & `marker_pdf-0.2.2/marker/postprocessors/t5.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/schema/bbox.py` & `marker_pdf-0.2.2/marker/schema/bbox.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/schema/block.py` & `marker_pdf-0.2.2/marker/schema/block.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/schema/page.py` & `marker_pdf-0.2.2/marker/schema/page.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/settings.py` & `marker_pdf-0.2.2/marker/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     LAYOUT_MODEL_CHECKPOINT: str = "vikp/surya_layout2"
     BBOX_INTERSECTION_THRESH: float = 0.7 # How much the layout and pdf bboxes need to overlap to be the same
     LAYOUT_BATCH_SIZE: Optional[int] = None # Defaults to 12 for cuda, 6 otherwise
 
     # Ordering model
     SURYA_ORDER_DPI: int = 96
     ORDER_BATCH_SIZE: Optional[int] = None  # Defaults to 12 for cuda, 6 otherwise
+    ORDER_MAX_BBOXES: int = 255
 
     # Final editing model
     EDITOR_BATCH_SIZE: Optional[int] = None # Defaults to 6 for cuda, 12 otherwise
     EDITOR_MAX_LENGTH: int = 1024
     EDITOR_MODEL_NAME: str = "vikp/pdf_postprocessor_t5"
     ENABLE_EDITOR_MODEL: bool = False # The editor model can create false positives
     EDITOR_CUTOFF_THRESH: float = 0.9 # Ignore predictions below this probability
```

### Comparing `marker_pdf-0.2.1/marker/tables/cells.py` & `marker_pdf-0.2.2/marker/tables/cells.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/tables/table.py` & `marker_pdf-0.2.2/marker/tables/table.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/marker/tables/utils.py` & `marker_pdf-0.2.2/marker/tables/utils.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.2.1/pyproject.toml` & `marker_pdf-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.2.1"
+version = "0.2.2"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
```

### Comparing `marker_pdf-0.2.1/PKG-INFO` & `marker_pdf-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.2.1
+Version: 0.2.2
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -173,14 +173,25 @@
 - `METADATA_FILE` is an optional path to a json file with metadata about the pdfs.  See above for the format.
 - `NUM_DEVICES` is the number of GPUs to use.  Should be `2` or greater.
 - `NUM_WORKERS` is the number of parallel processes to run on each GPU.  Per-GPU parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK`.
 - `MIN_LENGTH` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
 
 Note that the env variables above are specific to this script, and cannot be set in `local.env`.
 
+# Important settings/Troubleshooting
+
+There are some settings that you may find especially useful if things aren't working the way you expect:
+
+- `OCR_ALL_PAGES` - set this to true to force OCR all pages.  This can be very useful if the table layouts aren't recognized properly by default, or if there is garbled text.
+- `TORCH_DEVICE` - set this to force marker to use a given torch device for inference.
+- `OCR_ENGINE` - can set this to `surya` or `ocrmypdf`.
+- `DEBUG` - setting this to `True` shows ray logs when converting multiple pdfs
+
+In general, if output is not what you expect, trying to OCR the PDF is a good first step.
+
 # Benchmarks
 
 Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.  It's noisy, but at least directionally correct.
 
 Benchmarks show that marker is 4x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
 
 **Speed**
@@ -195,15 +206,15 @@
 First 3 are non-arXiv books, last 3 are arXiv papers.
 
 | Method | multicolcnn.pdf | switch_trans.pdf | thinkpython.pdf | thinkos.pdf | thinkdsp.pdf | crowd.pdf |
 |--------|-----------------|------------------|-----------------|-------------|--------------|-----------|
 | marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
 | nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
-Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `5.1GB` for marker.  Benchmarks were run on an A6000 Ada.
+Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `4.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
 Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
```

