# Comparing `tmp/marker_pdf-0.1.3.tar.gz` & `tmp/marker_pdf-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marker_pdf-0.1.3.tar", max compression
+gzip compressed data, was "marker_pdf-0.2.1.tar", max compression
```

## Comparing `marker_pdf-0.1.3.tar` & `marker_pdf-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,47 @@
--rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.1.3/LICENSE
--rw-r--r--   0        0        0    13227 2023-12-18 06:09:11.092607 marker_pdf-0.1.3/README.md
--rw-r--r--   0        0        0     4908 2023-12-19 21:40:35.305611 marker_pdf-0.1.3/benchmark.py
--rwxr-xr-x   0        0        0      541 2023-12-19 21:40:35.305844 marker_pdf-0.1.3/chunk_convert.py
--rwxr-xr-x   0        0        0     1162 2023-12-19 21:40:35.306156 marker_pdf-0.1.3/chunk_convert.sh
--rwxr-xr-x   0        0        0     4873 2023-12-23 07:05:33.763218 marker_pdf-0.1.3/convert.py
--rwxr-xr-x   0        0        0     1117 2023-12-19 21:40:35.307005 marker_pdf-0.1.3/convert_single.py
--rw-r--r--   0        0        0     2409 2023-12-07 18:30:49.680328 marker_pdf-0.1.3/marker/bbox.py
--rw-r--r--   0        0        0     1813 2023-11-28 17:18:56.226347 marker_pdf-0.1.3/marker/benchmark/scoring.py
--rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.1.3/marker/cleaners/bullets.py
--rw-r--r--   0        0        0     4566 2023-11-03 16:54:50.578959 marker_pdf-0.1.3/marker/cleaners/code.py
--rw-r--r--   0        0        0    10493 2024-01-02 18:21:05.915062 marker_pdf-0.1.3/marker/cleaners/equations.py
--rw-r--r--   0        0        0     3528 2023-11-01 18:02:50.356882 marker_pdf-0.1.3/marker/cleaners/headers.py
--rw-r--r--   0        0        0     3160 2023-12-06 16:47:32.301566 marker_pdf-0.1.3/marker/cleaners/table.py
--rw-r--r--   0        0        0     5367 2024-01-02 18:02:58.551862 marker_pdf-0.1.3/marker/convert.py
--rw-r--r--   0        0        0     2568 2024-01-02 18:02:58.558756 marker_pdf-0.1.3/marker/debug/data.py
--rw-r--r--   0        0        0     5595 2023-12-07 19:13:13.856243 marker_pdf-0.1.3/marker/extract_text.py
--rw-r--r--   0        0        0      464 2023-11-03 19:56:28.960392 marker_pdf-0.1.3/marker/logger.py
--rw-r--r--   0        0        0     6572 2023-12-19 21:40:35.295816 marker_pdf-0.1.3/marker/markdown.py
--rw-r--r--   0        0        0      438 2024-01-02 18:02:58.554918 marker_pdf-0.1.3/marker/models.py
--rw-r--r--   0        0        0     3013 2023-12-19 21:40:35.296277 marker_pdf-0.1.3/marker/ocr/page.py
--rw-r--r--   0        0        0     2013 2023-12-01 19:15:31.200145 marker_pdf-0.1.3/marker/ocr/utils.py
--rw-r--r--   0        0        0     3747 2024-01-02 18:16:16.080453 marker_pdf-0.1.3/marker/ordering.py
--rw-r--r--   0        0        0     3718 2024-01-02 18:09:51.477616 marker_pdf-0.1.3/marker/postprocessors/editor.py
--rw-r--r--   0        0        0     4983 2023-11-30 17:35:37.794881 marker_pdf-0.1.3/marker/postprocessors/t5.py
--rw-r--r--   0        0        0     5909 2023-12-07 17:48:07.817435 marker_pdf-0.1.3/marker/schema.py
--rw-r--r--   0        0        0     9329 2024-01-02 18:15:33.842912 marker_pdf-0.1.3/marker/segmentation.py
--rw-r--r--   0        0        0     4514 2024-01-02 18:36:32.775173 marker_pdf-0.1.3/marker/settings.py
--rw-r--r--   0        0        0     1337 2024-01-02 18:50:14.978035 marker_pdf-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    14987 1970-01-01 00:00:00.000000 marker_pdf-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35101 2023-11-16 20:09:42.311962 marker_pdf-0.2.1/LICENSE
+-rw-r--r--   0        0        0    12668 2024-05-09 17:58:32.978922 marker_pdf-0.2.1/README.md
+-rwxr-xr-x   0        0        0      541 2023-12-19 21:40:35.305844 marker_pdf-0.2.1/chunk_convert.py
+-rwxr-xr-x   0        0        0     1151 2024-05-09 16:07:14.765161 marker_pdf-0.2.1/chunk_convert.sh
+-rwxr-xr-x   0        0        0     4743 2024-05-07 17:49:43.674850 marker_pdf-0.2.1/convert.py
+-rwxr-xr-x   0        0        0     1246 2024-05-08 19:28:45.549038 marker_pdf-0.2.1/convert_single.py
+-rw-r--r--   0        0        0     1376 2024-05-09 14:37:06.538810 marker_pdf-0.2.1/marker/benchmark/scoring.py
+-rw-r--r--   0        0        0      231 2023-11-13 21:39:41.829455 marker_pdf-0.2.1/marker/cleaners/bullets.py
+-rw-r--r--   0        0        0     4405 2024-05-08 17:44:54.251299 marker_pdf-0.2.1/marker/cleaners/code.py
+-rw-r--r--   0        0        0      950 2024-05-07 20:26:01.091879 marker_pdf-0.2.1/marker/cleaners/fontstyle.py
+-rw-r--r--   0        0        0     2766 2024-05-07 20:26:12.412431 marker_pdf-0.2.1/marker/cleaners/headers.py
+-rw-r--r--   0        0        0     2456 2024-05-07 19:20:29.345524 marker_pdf-0.2.1/marker/cleaners/headings.py
+-rw-r--r--   0        0        0      248 2024-05-03 21:25:54.927963 marker_pdf-0.2.1/marker/cleaners/text.py
+-rw-r--r--   0        0        0     5166 2024-05-09 17:45:33.634950 marker_pdf-0.2.1/marker/convert.py
+-rw-r--r--   0        0        0     2450 2024-04-30 19:24:46.032856 marker_pdf-0.2.1/marker/debug/data.py
+-rw-r--r--   0        0        0     7884 2024-05-08 19:28:39.435042 marker_pdf-0.2.1/marker/equations/equations.py
+-rw-r--r--   0        0        0     1549 2024-05-08 19:28:39.424935 marker_pdf-0.2.1/marker/equations/inference.py
+-rw-r--r--   0        0        0     2594 2024-05-07 20:51:37.990183 marker_pdf-0.2.1/marker/images/extract.py
+-rw-r--r--   0        0        0      473 2024-05-07 17:35:52.062308 marker_pdf-0.2.1/marker/images/save.py
+-rw-r--r--   0        0        0     1928 2024-05-09 17:56:48.915437 marker_pdf-0.2.1/marker/layout/layout.py
+-rw-r--r--   0        0        0     2488 2024-05-09 17:57:11.112357 marker_pdf-0.2.1/marker/layout/order.py
+-rw-r--r--   0        0        0      396 2024-05-01 20:56:02.059168 marker_pdf-0.2.1/marker/logger.py
+-rw-r--r--   0        0        0     2085 2024-05-03 23:32:22.398344 marker_pdf-0.2.1/marker/models.py
+-rw-r--r--   0        0        0      888 2024-05-09 17:56:54.611918 marker_pdf-0.2.1/marker/ocr/detection.py
+-rw-r--r--   0        0        0     2468 2024-05-07 05:37:29.807989 marker_pdf-0.2.1/marker/ocr/heuristics.py
+-rw-r--r--   0        0        0      959 2024-05-03 23:32:22.393388 marker_pdf-0.2.1/marker/ocr/lang.py
+-rw-r--r--   0        0        0     5188 2024-05-08 19:24:58.173812 marker_pdf-0.2.1/marker/ocr/recognition.py
+-rw-r--r--   0        0        0     2180 2024-05-01 20:19:00.486329 marker_pdf-0.2.1/marker/ocr/tesseract.py
+-rw-r--r--   0        0        0      258 2024-05-02 23:16:18.893143 marker_pdf-0.2.1/marker/ocr/utils.py
+-rw-r--r--   0        0        0     1265 2024-05-07 18:48:43.948534 marker_pdf-0.2.1/marker/output.py
+-rw-r--r--   0        0        0     3932 2024-05-07 19:36:28.635033 marker_pdf-0.2.1/marker/pdf/extract_text.py
+-rw-r--r--   0        0        0      817 2024-05-07 02:48:52.757068 marker_pdf-0.2.1/marker/pdf/images.py
+-rw-r--r--   0        0        0     2339 2024-05-07 19:21:25.071249 marker_pdf-0.2.1/marker/pdf/utils.py
+-rw-r--r--   0        0        0     3904 2024-05-08 19:28:39.432619 marker_pdf-0.2.1/marker/postprocessors/editor.py
+-rw-r--r--   0        0        0     7103 2024-05-09 16:45:38.707953 marker_pdf-0.2.1/marker/postprocessors/markdown.py
+-rw-r--r--   0        0        0     4977 2024-05-07 20:27:15.110937 marker_pdf-0.2.1/marker/postprocessors/t5.py
+-rw-r--r--   0        0        0     2849 2024-05-03 13:40:49.822158 marker_pdf-0.2.1/marker/schema/bbox.py
+-rw-r--r--   0        0        0     3259 2024-05-08 16:58:04.155413 marker_pdf-0.2.1/marker/schema/block.py
+-rw-r--r--   0        0        0      502 2024-05-02 20:26:11.294687 marker_pdf-0.2.1/marker/schema/merged.py
+-rw-r--r--   0        0        0     1618 2024-05-08 17:45:07.502133 marker_pdf-0.2.1/marker/schema/page.py
+-rw-r--r--   0        0        0     4204 2024-05-09 17:53:04.646429 marker_pdf-0.2.1/marker/settings.py
+-rw-r--r--   0        0        0     3384 2024-05-07 19:20:29.343760 marker_pdf-0.2.1/marker/tables/cells.py
+-rw-r--r--   0        0        0     7178 2024-05-08 02:12:14.849108 marker_pdf-0.2.1/marker/tables/table.py
+-rw-r--r--   0        0        0     1128 2024-05-07 05:24:59.879003 marker_pdf-0.2.1/marker/tables/utils.py
+-rw-r--r--   0        0        0      156 2024-05-09 17:43:20.364396 marker_pdf-0.2.1/marker/utils.py
+-rw-r--r--   0        0        0     1319 2024-05-09 17:59:12.449026 marker_pdf-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    14199 1970-01-01 00:00:00.000000 marker_pdf-0.2.1/PKG-INFO
```

### Comparing `marker_pdf-0.1.3/LICENSE` & `marker_pdf-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.1.3/README.md` & `marker_pdf-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # Marker
 
-Marker converts PDF, EPUB, and MOBI to markdown.  It's 10x faster than nougat, more accurate on most documents, and has low hallucination risk.
+Marker converts PDF to markdown quickly and accurately.
 
-- Support for a range of PDF documents (optimized for books and scientific papers)
+- Supports a wide range of documents (optimized for books and scientific papers)
+- Supports all languages
 - Removes headers/footers/other artifacts
+- Formats tables and code blocks
+- Extracts and saves images along with the markdown
 - Converts most equations to latex
-- Formats code blocks and tables
-- Support for multiple languages (although most testing is done in English).  See `settings.py` for a language list.
 - Works on GPU, CPU, or MPS
 
 ## How it works
 
 Marker is a pipeline of deep learning models:
 
-- Extract text, OCR if necessary (heuristics, tesseract)
-- Detect page layout ([layout segmenter](https://huggingface.co/vikp/layout_segmenter), [column detector](https://huggingface.co/vikp/column_detector))
-- Clean and format each block (heuristics, [nougat](https://huggingface.co/facebook/nougat-base))
+- Extract text, OCR if necessary (heuristics, [surya](https://github.com/VikParuchuri/surya), tesseract)
+- Detect page layout and find reading order ([surya](https://github.com/VikParuchuri/surya))
+- Clean and format each block (heuristics, [texify](https://github.com/VikParuchuri/texify)
 - Combine blocks and postprocess complete text (heuristics, [pdf_postprocessor](https://huggingface.co/vikp/pdf_postprocessor_t5))
 
-Relying on autoregressive forward passes to generate text is slow and prone to hallucination/repetition.  From the nougat paper: `We observed [repetition] in 1.5% of pages in the test set, but the frequency increases for out-of-domain documents.`  In my anecdotal testing, repetitions happen on 5%+ of out-of-domain (non-arXiv) pages.  
-
-Nougat is an amazing model, but I wanted a faster and more general purpose solution. Marker is 10x faster and has low hallucination risk because it only passes equation blocks through an LLM forward pass.
+It only uses models where necessary, which improves speed and accuracy.
 
 ## Examples
 
 | PDF                                                                   | Type        | Marker                                                                                                 | Nougat                                                                                                 |
 |-----------------------------------------------------------------------|-------------|--------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
 | [Think Python](https://greenteapress.com/thinkpython/thinkpython.pdf) | Textbook    | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/thinkpython.md)         | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/thinkpython.md)         |
 | [Think OS](https://greenteapress.com/thinkos/thinkos.pdf)             | Textbook    | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/thinkos.md)             | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/thinkos.md)             |
@@ -44,177 +43,169 @@
 
 [Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
 
 # Limitations
 
 PDF is a tricky format, so marker will not always work perfectly.  Here are some known limitations that are on the roadmap to address:
 
-- Marker will convert fewer equations to latex than nougat.  This is because it has to first detect equations, then convert them without hallucation.
+- Marker will not convert 100% of equations to LaTeX.  This is because it has to detect then convert.
 - Whitespace and indentations are not always respected.
 - Not all lines/spans will be joined properly.
-- Languages similar to English (Spanish, French, German, Russian, etc) have the best support. There is provisional support for Chinese, Japanese, Korean, and Hindi, but it may not work as well.
 - This works best on digital PDFs that won't require a lot of OCR.  It's optimized for speed, and limited OCR is used to fix errors.
 
 # Installation
 
-This has been tested on Mac and Linux (Ubuntu and Debian).  You'll need python 3.9+ and [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).
+This has been tested on Mac and Linux (Ubuntu and Debian).  You'll need python 3.9+ and PyTorch.  You may need to install the CPU version of torch first if you're not using a Mac or a GPU machine.  See [here](https://pytorch.org/get-started/locally/) for more details.
+
+Install with:
 
-First, clone the repo:
+```shell
+pip install marker-pdf
+```
 
-- `git clone https://github.com/VikParuchuri/marker.git`
-- `cd marker`
+## Optional
 
-## Linux
+Only needed if using `ocrmypdf` as the ocr backend.
 
-- Install system requirements
-  - Optional: Install tesseract 5 by following [these instructions](https://notesalexp.org/tesseract-ocr/html/) or running `scripts/install/tesseract_5_install.sh`.
-  - Install ghostscript > 9.55 by following [these instructions](https://ghostscript.readthedocs.io/en/latest/Install.html) or running `scripts/install/ghostscript_install.sh`.
-  - Install other requirements with `cat scripts/install/apt-requirements.txt | xargs sudo apt-get install -y`
+**Linux**
+
+- Run `pip install ocrmypdf`
+- Install ghostscript > 9.55 by following [these instructions](https://ghostscript.readthedocs.io/en/latest/Install.html) or running `scripts/install/ghostscript_install.sh`.
+- Install other requirements with `cat scripts/install/tess-apt-requirements.txt | xargs sudo apt-get install -y`
 - Set the tesseract data folder path
   - Find the tesseract data folder `tessdata` with `find / -name tessdata`.  Make sure to use the one corresponding to the latest tesseract version if you have multiple.
   - Create a `local.env` file in the root `marker` folder with `TESSDATA_PREFIX=/path/to/tessdata` inside it
-- Install python requirements
-  - `poetry install`
-  - `poetry shell` to activate your poetry venv
-- Update pytorch since poetry doesn't play nicely with it
-  - GPU only: run `pip install torch` to install other torch dependencies.
-  - CPU only: Uninstall torch with `poetry remove torch`, then follow the [CPU install](https://pytorch.org/get-started/locally/) instructions.
 
-## Mac
+**Mac**
+
+Only needed if using `ocrmypdf` as the ocr backend.
 
-- Install system requirements from `scripts/install/brew-requirements.txt`
+- Run `pip install ocrmypdf`
+- Install system requirements from `scripts/install/tess-brew-requirements.txt`
 - Set the tesseract data folder path
   - Find the tesseract data folder `tessdata` with `brew list tesseract`
   - Create a `local.env` file in the root `marker` folder with `TESSDATA_PREFIX=/path/to/tessdata` inside it
-- Install python requirements
-  - `poetry install`
-  - `poetry shell` to activate your poetry venv
-- On ARM macs (M1+), make sure to set the `TORCH_DEVICE` setting to `mps` (more details below) for a speedup
 
 # Usage
 
-First, some configuration:
+First, some configuration.  Note that settings can be overridden with env vars.
 
-- Set your torch device in the `local.env` file.  For example, `TORCH_DEVICE=cuda` or `TORCH_DEVICE=mps`.  `cpu` is the default.
+- Inspect the settings in `marker/settings.py`.  You can override any settings with environment variables.
+- Your torch device will be automatically detected, but you can override this.  For example, `TORCH_DEVICE=cuda`.
   - If using GPU, set `INFERENCE_RAM` to your GPU VRAM (per GPU).  For example, if you have 16 GB of VRAM, set `INFERENCE_RAM=16`.
   - Depending on your document types, marker's average memory usage per task can vary slightly.  You can configure `VRAM_PER_TASK` to adjust this if you notice tasks failing with GPU out of memory errors.
-- Inspect the other settings in `marker/settings.py`.  You can override any settings in the `local.env` file, or by setting environment variables.
-  - By default, the final editor model is off.  Turn it on with `ENABLE_EDITOR_MODEL`.
-  - By default, marker will use ocrmypdf for OCR, which is slower than base tesseract, but higher quality.  You can change this with the `OCR_ENGINE` setting.
+- By default, marker will use `surya` for OCR.  Surya is slower on CPU, but more accurate than tesseract.  If you want faster OCR, set `OCR_ENGINE` to `ocrmypdf`. This also requires external dependencies (see above).  If you don't want OCR at all, set `OCR_ENGINE` to `None`.
 
 ## Convert a single file
 
-Run `convert_single.py`, like this:
-
-```
-python convert_single.py /path/to/file.pdf /path/to/output.md --parallel_factor 2 --max_pages 10
+```shell
+marker_single /path/to/file.pdf /path/to/output/folder --parallel_factor 2 --max_pages 10 --langs English
 ```
 
-- `--parallel_factor` is how much to increase batch size and parallel OCR workers by.  Higher numbers will take more VRAM and CPU, but process faster.  Set to 1 by default.
+- `--batch_multiplier` is how much to multiply default batch sizes by if you have extra VRAM.  Higher numbers will take more VRAM, but process faster.  Set to 2 by default.  The default batch sizes will take ~3GB of VRAM.
 - `--max_pages` is the maximum number of pages to process.  Omit this to convert the entire document.
+- `--langs` is a comma separated list of the languages in the document, for OCR
 
-Make sure the `DEFAULT_LANG` setting is set appropriately for your document.
+Make sure the `DEFAULT_LANG` setting is set appropriately for your document.  The list of supported languages for OCR is [here](https://github.com/VikParuchuri/surya/blob/master/surya/languages.py).  If you need more languages, you can use any language supported by [Tesseract](https://tesseract-ocr.github.io/tessdoc/Data-Files#data-files-for-version-400-november-29-2016) if you set `OCR_ENGINE` to `ocrmypdf`.  If you don't need OCR, marker can work with any language.
 
 ## Convert multiple files
 
-Run `convert.py`, like this:
-
-```
-python convert.py /path/to/input/folder /path/to/output/folder --workers 10 --max 10 --metadata_file /path/to/metadata.json --min_length 10000
+```shell
+marker /path/to/input/folder /path/to/output/folder --workers 10 --max 10 --metadata_file /path/to/metadata.json --min_length 10000
 ```
 
 - `--workers` is the number of pdfs to convert at once.  This is set to 1 by default, but you can increase it to increase throughput, at the cost of more CPU/GPU usage. Parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK` if you're using GPU.
 - `--max` is the maximum number of pdfs to convert.  Omit this to convert all pdfs in the folder.
-- `--metadata_file` is an optional path to a json file with metadata about the pdfs.  If you provide it, it will be used to set the language for each pdf.  If not, `DEFAULT_LANG` will be used. The format is:
 - `--min_length` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
+- `--metadata_file` is an optional path to a json file with metadata about the pdfs.  If you provide it, it will be used to set the language for each pdf.  If not, `DEFAULT_LANG` will be used. The format is:
 
 ```
 {
-  "pdf1.pdf": {"language": "English"},
-  "pdf2.pdf": {"language": "Spanish"},
+  "pdf1.pdf": {"languages": ["English"]},
+  "pdf2.pdf": {"languages": ["Spanish", "Russian"]},
   ...
 }
 ```
 
-## Convert multiple files on multiple GPUs
+You can use language names or codes.  The exact codes depend on the OCR engine.  See [here](https://github.com/VikParuchuri/surya/blob/master/surya/languages.py) for a full list for surya codes, and [here](https://tesseract-ocr.github.io/tessdoc/Data-Files#data-files-for-version-400-november-29-2016) for tesseract.
 
-Run `chunk_convert.sh`, like this:
+## Convert multiple files on multiple GPUs
 
-```
-MIN_LENGTH=10000 METADATA_FILE=../pdf_meta.json NUM_DEVICES=4 NUM_WORKERS=15 bash chunk_convert.sh ../pdf_in ../md_out
+```shell
+MIN_LENGTH=10000 METADATA_FILE=../pdf_meta.json NUM_DEVICES=4 NUM_WORKERS=15 marker_chunk_convert ../pdf_in ../md_out
 ```
 
 - `METADATA_FILE` is an optional path to a json file with metadata about the pdfs.  See above for the format.
 - `NUM_DEVICES` is the number of GPUs to use.  Should be `2` or greater.
 - `NUM_WORKERS` is the number of parallel processes to run on each GPU.  Per-GPU parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK`.
 - `MIN_LENGTH` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
 
+Note that the env variables above are specific to this script, and cannot be set in `local.env`.
+
 # Benchmarks
 
-Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.
+Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.  It's noisy, but at least directionally correct.
 
-Benchmarks show that marker is 10x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
+Benchmarks show that marker is 4x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
 
 **Speed**
 
 | Method | Average Score | Time per page | Time per document |
 |--------|---------------|---------------|-------------------|
-| naive  | 0.350727      | 0.00152378    | 0.326524          |
-| marker | 0.641062      | 0.360622      | 77.2762           |
-| nougat | 0.629211      | 3.77259       | 808.413           |
+| marker | 0.613721      | 0.631991      | 58.1432           |
+| nougat | 0.406603      | 2.59702       | 238.926           |
 
 **Accuracy**
 
 First 3 are non-arXiv books, last 3 are arXiv papers.
 
-| Method | switch_trans.pdf | crowd.pdf | multicolcnn.pdf | thinkos.pdf | thinkdsp.pdf | thinkpython.pdf |
-|--------|------------------|-----------|-----------------|-------------|--------------|-----------------|
-| naive  | 0.244114         | 0.140669  | 0.0868221       | 0.366856    | 0.412521     | 0.468281        |
-| marker | 0.482091         | 0.466882  | 0.537062        | 0.754347    | 0.78825      | 0.779536        |
-| nougat | 0.696458         | 0.552337  | 0.735099        | 0.655002    | 0.645704     | 0.650282        |
+| Method | multicolcnn.pdf | switch_trans.pdf | thinkpython.pdf | thinkos.pdf | thinkdsp.pdf | crowd.pdf |
+|--------|-----------------|------------------|-----------------|-------------|--------------|-----------|
+| marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
+| nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
-Peak GPU memory usage during the benchmark is `3.3GB` for nougat, and `3.1GB` for marker.  Benchmarks were run on an A6000.
+Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `5.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
-Marker takes about 2GB of VRAM on average per task, so you can convert 24 documents in parallel on an A6000.
+Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
 
 ## Running your own benchmarks
 
-You can benchmark the performance of marker on your machine.  First, download the benchmark data [here](https://drive.google.com/file/d/1WiN4K2-jQfwyQMe4wSSurbpz3hxo2fG9/view?usp=drive_link) and unzip.
-
-Then run `benchmark.py` like this:
+You can benchmark the performance of marker on your machine. Install marker manually with:
 
+```shell
+git clone https://github.com/VikParuchuri/marker.git
+poetry install
 ```
+
+Download the benchmark data [here](https://drive.google.com/file/d/1ZSeWDo2g1y0BRLT7KnbmytV2bjWARWba/view?usp=sharing) and unzip. Then run `benchmark.py` like this:
+
+```shell
 python benchmark.py data/pdfs data/references report.json --nougat
 ```
 
 This will benchmark marker against other text extraction methods.  It sets up batch sizes for nougat and marker to use a similar amount of GPU RAM for each.
 
 Omit `--nougat` to exclude nougat from the benchmark.  I don't recommend running nougat on CPU, since it is very slow.
 
 # Commercial usage
 
-Due to the licensing of the underlying models like layoutlmv3 and nougat, this is only suitable for noncommercial usage.  
-
-I'm building a version that can be used commercially, by stripping out the dependencies below. If you would like to get early access, email me at marker@vikas.sh.
-
-Here are the non-commercial/restrictive dependencies:
+All models were trained from scratch, so they're okay for commercial usage.  The weights for the models are licensed cc-by-nc-sa-4.0, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period AND under $5M in lifetime VC/angel funding raised.
 
-- LayoutLMv3: CC BY-NC-SA 4.0 .  [Source](https://huggingface.co/microsoft/layoutlmv3-base)
-- Nougat: CC-BY-NC . [Source](https://github.com/facebookresearch/nougat)
-- PyMuPDF - GPL . [Source](https://pymupdf.readthedocs.io/en/latest/about.html#license-and-copyright)
+If you want to remove the GPL license requirements for inference or use the weights commercially over the revenue limit, please contact me at marker@vikas.sh for dual licensing.
 
-Other dependencies/datasets are openly licensed (doclaynet, byt5), or used in a way that is compatible with commercial usage (ghostscript).
+Note that the `ocrmypdf` OCR option will use ocrmypdf, which includes Ghostscript, an AGPL dependency, but calls it via CLI, so it does not trigger the license provisions.  Ocrmypdf is disabled by default, and will not be installed automatically.
 
 # Thanks
 
 This work would not have been possible without amazing open source models and datasets, including (but not limited to):
 
-- Nougat from Meta
-- Layoutlmv3 from Microsoft
+- Surya
+- Texify
+- Pypdfium2/pdfium
 - DocLayNet from IBM
 - ByT5 from Google
 
 Thank you to the authors of these models and datasets for making them available to the community!
```

### Comparing `marker_pdf-0.1.3/chunk_convert.py` & `marker_pdf-0.2.1/chunk_convert.py`

 * *Files identical despite different names*

### Comparing `marker_pdf-0.1.3/chunk_convert.sh` & `marker_pdf-0.2.1/chunk_convert.sh`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # Loop from 0 to NUM_DEVICES and run the Python script in parallel
 for (( i=0; i<$NUM_DEVICES; i++ )); do
     DEVICE_NUM=$i
     export DEVICE_NUM
     export NUM_DEVICES
     export NUM_WORKERS
     echo "Running convert.py on GPU $DEVICE_NUM"
-    cmd="CUDA_VISIBLE_DEVICES=$DEVICE_NUM python convert.py $INPUT_FOLDER $OUTPUT_FOLDER --num_chunks $NUM_DEVICES --chunk_idx $DEVICE_NUM --workers $NUM_WORKERS"
+    cmd="CUDA_VISIBLE_DEVICES=$DEVICE_NUM marker $INPUT_FOLDER $OUTPUT_FOLDER --num_chunks $NUM_DEVICES --chunk_idx $DEVICE_NUM --workers $NUM_WORKERS"
     [[ -n "$METADATA_FILE" ]] && cmd="$cmd --metadata_file $METADATA_FILE"
     [[ -n "$MIN_LENGTH" ]] && cmd="$cmd --min_length $MIN_LENGTH"
     eval $cmd &
 
     sleep 5
 done
```

### Comparing `marker_pdf-0.1.3/convert.py` & `marker_pdf-0.2.1/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 import os
 from typing import Dict, Optional
 
 import ray
 from tqdm import tqdm
 import math
 
-from marker.convert import convert_single_pdf, get_length_of_text
+from marker.convert import convert_single_pdf
+from marker.output import markdown_exists, save_markdown
+from marker.pdf.utils import find_filetype
+from marker.pdf.extract_text import get_length_of_text
 from marker.models import load_all_models
 from marker.settings import settings
 from marker.logger import configure_logging
 import traceback
 import json
 
 configure_logging()
 
 
 @ray.remote(num_cpus=settings.RAY_CORES_PER_WORKER, num_gpus=.05 if settings.CUDA else 0)
 def process_single_pdf(fname: str, out_folder: str, model_refs, metadata: Optional[Dict] = None, min_length: Optional[int] = None):
-    out_filename = fname.rsplit(".", 1)[0] + ".md"
-    out_filename = os.path.join(out_folder, os.path.basename(out_filename))
-    out_meta_filename = out_filename.rsplit(".", 1)[0] + "_meta.json"
-    if os.path.exists(out_filename):
+    if markdown_exists(out_folder, fname):
         return
     try:
         # Skip trying to convert files that don't have a lot of embedded text
         # This can indicate that they were scanned, and not OCRed properly
         # Usually these files are not recent/high-quality
         if min_length:
+            filetype = find_filetype(fname)
+            if filetype == "other":
+                return 0
+
             length = get_length_of_text(fname)
             if length < min_length:
                 return
 
-        full_text, out_metadata = convert_single_pdf(fname, model_refs, metadata=metadata)
+        full_text, images, out_metadata = convert_single_pdf(fname, model_refs, metadata=metadata)
         if len(full_text.strip()) > 0:
-            with open(out_filename, "w+", encoding='utf-8') as f:
-                f.write(full_text)
-            with open(out_meta_filename, "w+") as f:
-                f.write(json.dumps(out_metadata, indent=4))
+            save_markdown(out_folder, fname, full_text, images, out_metadata)
         else:
             print(f"Empty file: {fname}.  Could not convert.")
     except Exception as e:
         print(f"Error converting {fname}: {e}")
         print(traceback.format_exc())
 
 
@@ -83,15 +84,14 @@
     total_processes = min(len(files_to_convert), args.workers)
 
     ray.init(
         num_cpus=total_processes,
         num_gpus=1 if settings.CUDA else 0,
         storage=settings.RAY_CACHE_PATH,
         _temp_dir=settings.RAY_CACHE_PATH,
-        dashboard_host=settings.RAY_DASHBOARD_HOST,
         log_to_driver=settings.DEBUG
     )
 
     model_lst = load_all_models()
     model_refs = ray.put(model_lst)
 
     # Dynamically set GPU allocation per task based on GPU ram
```

### Comparing `marker_pdf-0.1.3/convert_single.py` & `marker_pdf-0.2.1/convert_single.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import argparse
+import os
 
 from marker.convert import convert_single_pdf
 from marker.logger import configure_logging
 from marker.models import load_all_models
-import json
+
+from marker.output import save_markdown
 
 configure_logging()
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("filename", help="PDF file to parse")
-    parser.add_argument("output", help="Output file name")
+    parser.add_argument("output", help="Output base folder path")
     parser.add_argument("--max_pages", type=int, default=None, help="Maximum number of pages to parse")
-    parser.add_argument("--parallel_factor", type=int, default=1, help="How much to multiply default parallel OCR workers and model batch sizes by.")
+    parser.add_argument("--langs", type=str, help="Languages to use for OCR, comma separated", default=None)
+    parser.add_argument("--batch_multiplier", type=int, default=2, help="How much to increase batch sizes")
     args = parser.parse_args()
 
+    langs = args.langs.split(",") if args.langs else None
+
     fname = args.filename
     model_lst = load_all_models()
-    full_text, out_meta = convert_single_pdf(fname, model_lst, max_pages=args.max_pages, parallel_factor=args.parallel_factor)
+    full_text, images, out_meta = convert_single_pdf(fname, model_lst, max_pages=args.max_pages, langs=langs, batch_multiplier=args.batch_multiplier)
 
-    with open(args.output, "w+", encoding='utf-8') as f:
-        f.write(full_text)
+    fname = os.path.basename(fname)
+    subfolder_path = save_markdown(args.output, fname, full_text, images, out_meta)
 
-    out_meta_filename = args.output.rsplit(".", 1)[0] + "_meta.json"
-    with open(out_meta_filename, "w+") as f:
-        f.write(json.dumps(out_meta, indent=4))
+    print(f"Saved markdown to the {subfolder_path} folder")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `marker_pdf-0.1.3/marker/bbox.py` & `marker_pdf-0.2.1/marker/schema/bbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import fitz as pymupdf
+from typing import List
+
+from pydantic import BaseModel, field_validator
+
 
 def should_merge_blocks(box1, box2, tol=5):
     # Within tol y px, and to the right within tol px
     merge = [
         box2[0] > box1[0], # After in the x coordinate
         abs(box2[1] - box1[1]) < tol, # Within tol y px
         abs(box2[3] - box1[3]) < tol, # Within tol y px
@@ -16,66 +19,86 @@
 
 
 def boxes_intersect(box1, box2):
     # Box1 intersects box2
     return box1[0] < box2[2] and box1[2] > box2[0] and box1[1] < box2[3] and box1[3] > box2[1]
 
 
-def boxes_intersect_pct(box1, box2, pct=.9):
+def box_intersection_pct(box1, box2):
     # determine the coordinates of the intersection rectangle
     x_left = max(box1[0], box2[0])
     y_top = max(box1[1], box2[1])
     x_right = min(box1[2], box2[2])
     y_bottom = min(box1[3], box2[3])
 
     if x_right < x_left or y_bottom < y_top:
         return 0.0
 
-    # The intersection of two axis-aligned bounding boxes is always an
-    # axis-aligned bounding box
     intersection_area = (x_right - x_left) * (y_bottom - y_top)
-
-    # compute the area of both AABBs
     bb1_area = (box1[2] - box1[0]) * (box1[3] - box1[1])
-    bb2_area = (box2[2] - box2[0]) * (box2[3] - box2[1])
 
-    iou = intersection_area / float(bb1_area + bb2_area - intersection_area)
-    return iou > pct
+    if bb1_area == 0:
+        return 0.0
+    iou = intersection_area / bb1_area
+    return iou
 
 
 def multiple_boxes_intersect(box1, boxes):
     for box2 in boxes:
         if boxes_intersect(box1, box2):
             return True
     return False
 
 
-def box_contained(box1, box2):
-    # Box1 inside box2
-    return box1[0] > box2[0] and box1[1] > box2[1] and box1[2] < box2[2] and box1[3] < box2[3]
-
-
 def unnormalize_box(bbox, width, height):
     return [
         width * (bbox[0] / 1000),
         height * (bbox[1] / 1000),
         width * (bbox[2] / 1000),
         height * (bbox[3] / 1000),
     ]
 
 
-def correct_rotation(bbox, page):
-    #bbox base is (x0, y0, x1, y1)
-    rotation = page.rotation
-    if rotation == 0:
-        return bbox
-
-    tl = pymupdf.Point(bbox[0], bbox[1]) * page.rotation_matrix
-    br = pymupdf.Point(bbox[2], bbox[3]) * page.rotation_matrix
-    if rotation == 90:
-        bbox = [br[0], tl[1], tl[0], br[1]]
-    elif rotation == 180:
-        bbox = [br[0], br[1], tl[0], tl[1]]
-    elif rotation == 270:
-        bbox = [tl[0], br[1], br[0], tl[1]]
+class BboxElement(BaseModel):
+    bbox: List[float]
+
+    @field_validator('bbox')
+    @classmethod
+    def check_4_elements(cls, v: List[float]) -> List[float]:
+        if len(v) != 4:
+            raise ValueError('bbox must have 4 elements')
+        return v
+
+    @property
+    def height(self):
+        return self.bbox[3] - self.bbox[1]
+
+    @property
+    def width(self):
+        return self.bbox[2] - self.bbox[0]
+
+    @property
+    def x_start(self):
+        return self.bbox[0]
+
+    @property
+    def y_start(self):
+        return self.bbox[1]
+
+    @property
+    def area(self):
+        return self.width * self.height
+
+    def intersection_pct(self, other_bbox: List[float]):
+        if self.area == 0:
+            return 0.0
+        return box_intersection_pct(self.bbox, other_bbox)
+
+
+def rescale_bbox(orig_dim, new_dim, bbox):
+    page_width, page_height = new_dim[2] - new_dim[0], new_dim[3] - new_dim[1]
+    detected_width, detected_height = orig_dim[2] - orig_dim[0], orig_dim[3] - orig_dim[1]
+    width_scaler = detected_width / page_width
+    height_scaler = detected_height / page_height
 
-    return bbox
+    new_bbox = [bbox[0] / width_scaler, bbox[1] / height_scaler, bbox[2] / width_scaler, bbox[3] / height_scaler]
+    return new_bbox
```

### Comparing `marker_pdf-0.1.3/marker/cleaners/code.py` & `marker_pdf-0.2.1/marker/cleaners/code.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-from marker.schema import Span, Line, Page
+from collections import Counter
+from statistics import mean, median
+
+from marker.schema.block import Span, Line
+from marker.schema.page import Page
 import re
 from typing import List
-import fitz as pymupdf
 
 
-def is_code_linelen(lines, thresh=60):
+def is_code_linelen(lines, thresh=80):
     # Decide based on chars per newline threshold
     total_alnum_chars = sum(len(re.findall(r'\w', line.prelim_text)) for line in lines)
     total_newlines = max(len(lines) - 1, 1)
 
     if total_alnum_chars == 0:
         return False
 
@@ -17,113 +20,112 @@
 
 
 def comment_count(lines):
     pattern = re.compile(r"^(//|#|'|--|/\*|'''|\"\"\"|--\[\[|<!--|%|%{|\(\*)")
     return sum([1 for line in lines if pattern.match(line)])
 
 
-def identify_code_blocks(blocks: List[Page]):
+def identify_code_blocks(pages: List[Page]):
     code_block_count = 0
-    font_info = None
-    for p in blocks:
-        stats = p.get_font_stats()
-        if font_info is None:
-            font_info = stats
-        else:
-            font_info += stats
-    try:
-        most_common_font = font_info.most_common(1)[0][0]
-    except IndexError:
-        print(f"Could not find most common font")
-        most_common_font = None
-
-    last_block = None
-    for page in blocks:
-        try:
-            min_start = page.get_min_line_start()
-        except IndexError:
-            continue
+    font_sizes = []
+    line_heights = []
+    for page in pages:
+        font_sizes += page.get_font_sizes()
+        line_heights += page.get_line_heights()
+
+    avg_font_size = None
+    avg_line_height = None
+    if len(font_sizes) > 0:
+        avg_line_height = median(line_heights)
+        avg_font_size = mean(font_sizes)
 
+    for page in pages:
         for block in page.blocks:
-            if block.most_common_block_type() != "Text":
+            if block.block_type != "Text":
                 last_block = block
                 continue
 
+            # Ensure we have lines and spans
+            if len(block.lines) == 0:
+                continue
+            if sum([len(line.spans) for line in block.lines]) == 0:
+                continue
+
+            min_start = block.get_min_line_start()
+
             is_indent = []
             line_fonts = []
+            line_font_sizes = []
+            block_line_heights = []
             for line in block.lines:
-                fonts = [span.font for span in line.spans]
-                line_fonts += fonts
-                line_start = line.bbox[0]
-                if line_start > min_start:
-                    is_indent.append(True)
-                else:
-                    is_indent.append(False)
+                line_fonts += [span.font for span in line.spans]
+                line_font_sizes += [span.font_size for span in line.spans]
+                block_line_heights.append(line.bbox[3] - line.bbox[1])
+
+                is_indent.append(line.bbox[0] > min_start)
+
             comment_lines = comment_count([line.prelim_text for line in block.lines])
             is_code = [
                 len(block.lines) > 3,
-                sum([f != most_common_font for f in line_fonts]) > len(line_fonts) * .8,  # At least 80% of the fonts are not the most common, since code usually uses a different font from the main body text
                 is_code_linelen(block.lines),
-                (
-                    sum(is_indent) > len(block.lines) * .2
-                    or
-                    comment_lines > len(block.lines) * .2
-                 ), # 20% lines indented or 20% of the lines are comments
+                sum(is_indent) + comment_lines > len(block.lines) * .3,
             ]
 
-            # Check if previous block is code, and this block is indented
-            is_code_prev = [
-                last_block and last_block.most_common_block_type() == "Code",
-                sum(is_indent) >= len(block.lines) * .8 # At least 80% indented
-            ]
+            if avg_font_size is not None:
+                font_checks = [
+                    mean(line_font_sizes) <= avg_font_size, # Lower than average font size and line height
+                    mean(block_line_heights) < avg_line_height
+                ]
+                is_code += font_checks
 
-            if all(is_code) or all(is_code_prev):
+            if all(is_code):
                 code_block_count += 1
-                block.set_block_type("Code")
+                block.block_type = "Code"
 
-            last_block = block
     return code_block_count
 
 
-def indent_blocks(blocks: List[Page]):
+def indent_blocks(pages: List[Page]):
     span_counter = 0
-    for page in blocks:
+    for page in pages:
         for block in page.blocks:
-            block_types = [span.block_type for line in block.lines for span in line.spans]
-            if "Code" not in block_types:
+            if block.block_type != "Code":
                 continue
 
             lines = []
             min_left = 1000  # will contain x- coord of column 0
             col_width = 0  # width of 1 char
             for line in block.lines:
                 text = ""
                 min_left = min(line.bbox[0], min_left)
                 for span in line.spans:
                     if col_width == 0 and len(span.text) > 0:
                         col_width = (span.bbox[2] - span.bbox[0]) / len(span.text)
                     text += span.text
-                lines.append((pymupdf.Rect(line.bbox), text))
+                lines.append((line.bbox, text))
 
             block_text = ""
             blank_line = False
             for line in lines:
                 text = line[1]
-                prefix = " " * int((line[0].x0 - min_left) / col_width)
+                if col_width == 0:
+                    prefix = ""
+                else:
+                    prefix = " " * int((line[0][0] - min_left) / col_width)
                 current_line_blank = len(text.strip()) == 0
                 if blank_line and current_line_blank:
                     # Don't put multiple blank lines in a row
                     continue
 
                 block_text += prefix + text + "\n"
                 blank_line = current_line_blank
 
             new_span = Span(
                 text=block_text,
                 bbox=block.bbox,
-                color=block.lines[0].spans[0].color,
                 span_id=f"{span_counter}_fix_code",
                 font=block.lines[0].spans[0].font,
-                block_type="Code"
+                font_weight=block.lines[0].spans[0].font_weight,
+                font_size=block.lines[0].spans[0].font_size,
             )
             span_counter += 1
             block.lines = [Line(spans=[new_span], bbox=block.bbox)]
```

### Comparing `marker_pdf-0.1.3/marker/cleaners/headers.py` & `marker_pdf-0.2.1/marker/cleaners/headers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import re
-from collections import Counter, defaultdict
-from itertools import chain
-from thefuzz import fuzz
+from collections import Counter
+from rapidfuzz import fuzz
 
-from sklearn.cluster import DBSCAN
-import numpy as np
-
-from marker.schema import Page, FullyMergedBlock
+from marker.schema.merged import FullyMergedBlock
 from typing import List, Tuple
 
 
-def filter_common_elements(lines, page_count):
+def filter_common_elements(lines, page_count, threshold=.6):
+    # We can't filter if we don't have enough pages to find common elements
+    if page_count < 3:
+        return []
     text = [s.text for line in lines for s in line.spans if len(s.text) > 4]
     counter = Counter(text)
-    common = [k for k, v in counter.items() if v > page_count * .6]
+    common = [k for k, v in counter.items() if v > page_count * threshold]
     bad_span_ids = [s.span_id for line in lines for s in line.spans if s.text in common]
     return bad_span_ids
 
 
 def filter_header_footer(all_page_blocks, max_selected_lines=2):
     first_lines = []
     last_lines = []
@@ -27,40 +26,14 @@
         last_lines.extend(nonblank_lines[-max_selected_lines:])
 
     bad_span_ids = filter_common_elements(first_lines, len(all_page_blocks))
     bad_span_ids += filter_common_elements(last_lines, len(all_page_blocks))
     return bad_span_ids
 
 
-def categorize_blocks(all_page_blocks: List[Page]):
-    spans = list(chain.from_iterable([p.get_nonblank_spans() for p in all_page_blocks]))
-    X = np.array(
-        [(*s.bbox, len(s.text)) for s in spans]
-    )
-
-    dbscan = DBSCAN(eps=.1, min_samples=5)
-    dbscan.fit(X)
-    labels = dbscan.labels_
-    label_chars = defaultdict(int)
-    for i, label in enumerate(labels):
-        label_chars[label] += len(spans[i].text)
-
-    most_common_label = None
-    most_chars = 0
-    for i in label_chars.keys():
-        if label_chars[i] > most_chars:
-            most_common_label = i
-            most_chars = label_chars[i]
-
-    labels = [0 if label == most_common_label else 1 for label in labels]
-    bad_span_ids = [spans[i].span_id for i in range(len(spans)) if labels[i] == 1]
-
-    return bad_span_ids
-
-
 def replace_leading_trailing_digits(string, replacement):
     string = re.sub(r'^\d+', replacement, string)
     string = re.sub(r'\d+$', replacement, string)
     return string
 
 
 def find_overlap_elements(lst: List[Tuple[str, int]], string_match_thresh=.9, min_overlap=.05) -> List[int]:
```

### Comparing `marker_pdf-0.1.3/marker/cleaners/table.py` & `marker_pdf-0.2.1/marker/schema/block.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,120 @@
-from marker.bbox import merge_boxes
-from marker.schema import Line, Span, Block, Page
-from copy import deepcopy
-from tabulate import tabulate
-from typing import List
-import re
-import textwrap
-
-
-def merge_table_blocks(blocks: List[Page]):
-    current_lines = []
-    current_bbox = None
-    for page in blocks:
-        new_page_blocks = []
-        pnum = page.pnum
-        for block in page.blocks:
-            if block.most_common_block_type() != "Table":
-                if len(current_lines) > 0:
-                    new_block = Block(
-                        lines=deepcopy(current_lines),
-                        pnum=pnum,
-                        bbox=current_bbox
-                    )
-                    new_page_blocks.append(new_block)
-                    current_lines = []
-                    current_bbox = None
-
-                new_page_blocks.append(block)
-                continue
-
-            current_lines.extend(block.lines)
-            if current_bbox is None:
-                current_bbox = block.bbox
-            else:
-                current_bbox = merge_boxes(current_bbox, block.bbox)
-
-        if len(current_lines) > 0:
-            new_block = Block(
-                lines=deepcopy(current_lines),
-                pnum=pnum,
-                bbox=current_bbox
-            )
-            new_page_blocks.append(new_block)
-            current_lines = []
-            current_bbox = None
-
-        page.blocks = new_page_blocks
-
-
-def create_new_tables(blocks: List[Page]):
-    table_idx = 0
-    dot_pattern = re.compile(r'(\s*\.\s*){4,}')
-    dot_multiline_pattern = re.compile(r'.*(\s*\.\s*){4,}.*', re.DOTALL)
-
-    for page in blocks:
-        for block in page.blocks:
-            if block.most_common_block_type() != "Table" or len(block.lines) < 3:
-                continue
-
-            table_rows = []
-            y_coord = None
-            row = []
-            for line in block.lines:
-                for span in line.spans:
-                    if y_coord != span.y_start:
-                        if len(row) > 0:
-                            table_rows.append(row)
-                            row = []
-                        y_coord = span.y_start
-
-                    text = span.text
-                    if dot_multiline_pattern.match(text):
-                        text = dot_pattern.sub(' ', text)
-                    row.append(text)
-            if len(row) > 0:
-                table_rows.append(row)
-
-            # Don't render tables if they will be too large
-            if max([len("".join(r)) for r in table_rows]) > 300 or len(table_rows[0]) > 8 or len(table_rows[0]) < 2:
-                continue
-
-            new_text = tabulate(table_rows, headers="firstrow", tablefmt="github")
-            new_span = Span(
-                bbox=block.bbox,
-                span_id=f"{table_idx}_fix_table",
-                font="Table",
-                color=0,
-                block_type="Table",
-                text=new_text
-            )
-            new_line = Line(
-                bbox=block.bbox,
-                spans=[new_span]
-            )
-            block.lines = [new_line]
-            table_idx += 1
-    return table_idx
+import math
+from typing import List, Optional
+
+from pydantic import field_validator
+import ftfy
+
+from marker.schema.bbox import BboxElement
+from marker.settings import settings
+
+
+class BlockType(BboxElement):
+    block_type: str
+
+
+class Span(BboxElement):
+    text: str
+    span_id: str
+    font: str
+    font_weight: float
+    font_size: float
+    bold: Optional[bool] = None
+    italic: Optional[bool] = None
+    image: Optional[bool] = None
+
+
+    @field_validator('text')
+    @classmethod
+    def fix_unicode(cls, text: str) -> str:
+        return ftfy.fix_text(text)
+
+
+class Line(BboxElement):
+    spans: List[Span]
+
+    @property
+    def prelim_text(self):
+        return "".join([s.text for s in self.spans])
+
+    @property
+    def start(self):
+        return self.spans[0].bbox[0]
+
+
+class Block(BboxElement):
+    lines: List[Line]
+    pnum: int
+    block_type: Optional[str] = None
+
+    @property
+    def prelim_text(self):
+        return "\n".join([l.prelim_text for l in self.lines])
+
+    def filter_spans(self, bad_span_ids):
+        new_lines = []
+        for line in self.lines:
+            new_spans = []
+            for span in line.spans:
+                if not span.span_id in bad_span_ids:
+                    new_spans.append(span)
+            line.spans = new_spans
+            if len(new_spans) > 0:
+                new_lines.append(line)
+        self.lines = new_lines
+
+    def filter_bad_span_types(self):
+        new_lines = []
+        for line in self.lines:
+            new_spans = []
+            for span in line.spans:
+                if self.block_type not in settings.BAD_SPAN_TYPES:
+                    new_spans.append(span)
+            line.spans = new_spans
+            if len(new_spans) > 0:
+                new_lines.append(line)
+        self.lines = new_lines
+
+    def get_min_line_start(self):
+        line_starts = [line.start for line in self.lines]
+        if len(line_starts) == 0:
+            return None
+        return min(line_starts)
+
+
+def bbox_from_lines(lines: List[Line]):
+    min_x = min([line.bbox[0] for line in lines])
+    min_y = min([line.bbox[1] for line in lines])
+    max_x = max([line.bbox[2] for line in lines])
+    max_y = max([line.bbox[3] for line in lines])
+    return [min_x, min_y, max_x, max_y]
+
+
+def split_block_lines(block: Block, split_line_idx: int):
+    new_blocks = []
+    if split_line_idx >= len(block.lines):
+        return [block]
+    elif split_line_idx == 0:
+        return [block]
+    else:
+        new_blocks.append(Block(lines=block.lines[:split_line_idx], bbox=bbox_from_lines(block.lines[:split_line_idx]), pnum=block.pnum))
+        new_blocks.append(Block(lines=block.lines[split_line_idx:], bbox=bbox_from_lines(block.lines[split_line_idx:]), pnum=block.pnum))
+    return new_blocks
+
+
+def find_insert_block(blocks: List[Block], bbox):
+    nearest_match = None
+    match_dist = None
+    for idx, block in enumerate(blocks):
+        try:
+            dist = math.sqrt((block.bbox[1] - bbox[1]) ** 2 + (block.bbox[0] - bbox[0]) ** 2)
+        except Exception as e:
+            continue
+
+        if nearest_match is None or dist < match_dist:
+            nearest_match = idx
+            match_dist = dist
+    if nearest_match is None:
+        return 0
+    return nearest_match
+
+
```

### Comparing `marker_pdf-0.1.3/marker/convert.py` & `marker_pdf-0.2.1/marker/convert.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,175 +1,164 @@
-import fitz as pymupdf
+import warnings
 
-from marker.cleaners.table import merge_table_blocks, create_new_tables
+from marker.utils import flush_cuda_memory
+
+warnings.filterwarnings("ignore", category=UserWarning) # Filter torch pytree user warnings
+
+import pypdfium2 as pdfium
+from PIL import Image
+
+from marker.tables.table import format_tables
 from marker.debug.data import dump_bbox_debug_data
-from marker.extract_text import get_text_blocks
+from marker.layout.layout import surya_layout, annotate_block_types
+from marker.layout.order import surya_order, sort_blocks_in_reading_order
+from marker.ocr.lang import replace_langs_with_codes, validate_langs
+from marker.ocr.detection import surya_detection
+from marker.ocr.recognition import run_ocr
+from marker.pdf.extract_text import get_text_blocks
 from marker.cleaners.headers import filter_header_footer, filter_common_titles
-from marker.cleaners.equations import replace_equations
-from marker.ordering import order_blocks
+from marker.equations.equations import replace_equations
+from marker.pdf.utils import find_filetype
 from marker.postprocessors.editor import edit_full_text
-from marker.segmentation import detect_document_block_types
 from marker.cleaners.code import identify_code_blocks, indent_blocks
 from marker.cleaners.bullets import replace_bullets
-from marker.markdown import merge_spans, merge_lines, get_full_text
-from marker.schema import Page, BlockType
+from marker.cleaners.headings import split_heading_blocks
+from marker.cleaners.fontstyle import find_bold_italic
+from marker.postprocessors.markdown import merge_spans, merge_lines, get_full_text
+from marker.cleaners.text import cleanup_text
+from marker.images.extract import extract_images
+from marker.images.save import images_to_dict
+
 from typing import List, Dict, Tuple, Optional
-import re
-import magic
 from marker.settings import settings
 
 
-def find_filetype(fpath):
-    mimetype = magic.from_file(fpath).lower()
-
-    # Get extensions from mimetype
-    # The mimetype is not always consistent, so use in to check the most common formats
-    if "pdf" in mimetype:
-        return "pdf"
-    elif "epub" in mimetype:
-        return "epub"
-    elif "mobi" in mimetype:
-        return "mobi"
-    elif mimetype in settings.SUPPORTED_FILETYPES:
-        return settings.SUPPORTED_FILETYPES[mimetype]
-    else:
-        print(f"Found nonstandard filetype {mimetype}")
-        return "other"
-
-
-def annotate_spans(blocks: List[Page], block_types: List[BlockType]):
-    for i, page in enumerate(blocks):
-        page_block_types = block_types[i]
-        page.add_block_types(page_block_types)
-
-
-def get_length_of_text(fname: str) -> int:
-    filetype = find_filetype(fname)
-    if filetype == "other":
-        return 0
-
-    doc = pymupdf.open(fname, filetype=filetype)
-    full_text = ""
-    for page in doc:
-        full_text += page.get_text("text", sort=True, flags=settings.TEXT_FLAGS)
-
-    return len(full_text)
-
-
 def convert_single_pdf(
         fname: str,
         model_lst: List,
         max_pages=None,
         metadata: Optional[Dict]=None,
-        parallel_factor: int = 1
-) -> Tuple[str, Dict]:
-    lang = settings.DEFAULT_LANG
-    if metadata:
-        lang = metadata.get("language", settings.DEFAULT_LANG)
+        langs: Optional[List[str]] = None,
+        batch_multiplier: int = 1
+) -> Tuple[str, Dict[str, Image.Image], Dict]:
+    # Set language needed for OCR
+    if langs is None:
+        langs = [settings.DEFAULT_LANG]
 
-    # Use tesseract language if available
-    tess_lang = settings.TESSERACT_LANGUAGES.get(lang, "eng")
-    spell_lang = settings.SPELLCHECK_LANGUAGES.get(lang, None)
-    if "eng" not in tess_lang:
-        tess_lang = f"eng+{tess_lang}"
+    if metadata:
+        langs = metadata.get("languages", langs)
 
-    # Output metadata
-    out_meta = {"language": lang}
+    langs = replace_langs_with_codes(langs)
+    validate_langs(langs)
 
+    # Find the filetype
     filetype = find_filetype(fname)
-    if filetype == "other":
-        return "", out_meta
 
-    out_meta["filetype"] = filetype
+    # Setup output metadata
+    out_meta = {
+        "languages": langs,
+        "filetype": filetype,
+    }
 
-    doc = pymupdf.open(fname, filetype=filetype)
-    if filetype != "pdf":
-        conv = doc.convert_to_pdf()
-        doc = pymupdf.open("pdf", conv)
+    if filetype == "other": # We can't process this file
+        return "", out_meta
 
-    blocks, toc, ocr_stats = get_text_blocks(
+    # Get initial text blocks from the pdf
+    doc = pdfium.PdfDocument(fname)
+    pages, toc = get_text_blocks(
         doc,
-        tess_lang,
-        spell_lang,
         max_pages=max_pages,
-        parallel=int(parallel_factor * settings.OCR_PARALLEL_WORKERS)
     )
+    out_meta.update({
+        "toc": toc,
+        "pages": len(pages),
+    })
+
+    # Unpack models from list
+    texify_model, layout_model, order_model, edit_model, detection_model, ocr_model = model_lst
+
+    # Identify text lines on pages
+    surya_detection(doc, pages, detection_model, batch_multiplier=batch_multiplier)
+    flush_cuda_memory()
+
+    # OCR pages as needed
+    pages, ocr_stats = run_ocr(doc, pages, langs, ocr_model, batch_multiplier=batch_multiplier)
+    flush_cuda_memory()
 
-    out_meta["toc"] = toc
-    out_meta["pages"] = len(blocks)
     out_meta["ocr_stats"] = ocr_stats
-    if len([b for p in blocks for b in p.blocks]) == 0:
+    if len([b for p in pages for b in p.blocks]) == 0:
         print(f"Could not extract any text blocks for {fname}")
         return "", out_meta
 
-    # Unpack models from list
-    texify_model, layoutlm_model, order_model, edit_model = model_lst
-
-    block_types = detect_document_block_types(
-        doc,
-        blocks,
-        layoutlm_model,
-        batch_size=int(settings.LAYOUT_BATCH_SIZE * parallel_factor)
-    )
+    surya_layout(doc, pages, layout_model, batch_multiplier=batch_multiplier)
+    flush_cuda_memory()
 
     # Find headers and footers
-    bad_span_ids = filter_header_footer(blocks)
+    bad_span_ids = filter_header_footer(pages)
     out_meta["block_stats"] = {"header_footer": len(bad_span_ids)}
 
-    annotate_spans(blocks, block_types)
+    # Add block types in
+    annotate_block_types(pages)
 
     # Dump debug data if flags are set
-    dump_bbox_debug_data(doc, blocks)
+    dump_bbox_debug_data(doc, pages)
 
-    blocks = order_blocks(
-        doc,
-        blocks,
-        order_model,
-        batch_size=int(settings.ORDERER_BATCH_SIZE * parallel_factor)
-    )
+    # Find reading order for blocks
+    # Sort blocks by reading order
+    surya_order(doc, pages, order_model, batch_multiplier=batch_multiplier)
+    sort_blocks_in_reading_order(pages)
+    flush_cuda_memory()
 
     # Fix code blocks
-    code_block_count = identify_code_blocks(blocks)
+    code_block_count = identify_code_blocks(pages)
     out_meta["block_stats"]["code"] = code_block_count
-    indent_blocks(blocks)
+    indent_blocks(pages)
 
     # Fix table blocks
-    merge_table_blocks(blocks)
-    table_count = create_new_tables(blocks)
+    table_count = format_tables(pages)
     out_meta["block_stats"]["table"] = table_count
 
-    for page in blocks:
+    for page in pages:
         for block in page.blocks:
             block.filter_spans(bad_span_ids)
             block.filter_bad_span_types()
 
     filtered, eq_stats = replace_equations(
         doc,
-        blocks,
-        block_types,
+        pages,
         texify_model,
-        batch_size=int(settings.TEXIFY_BATCH_SIZE * parallel_factor)
+        batch_multiplier=batch_multiplier
     )
+    flush_cuda_memory()
     out_meta["block_stats"]["equations"] = eq_stats
 
+    # Extract images and figures
+    if settings.EXTRACT_IMAGES:
+        extract_images(doc, pages)
+
+    # Split out headers
+    split_heading_blocks(pages)
+    find_bold_italic(pages)
+
     # Copy to avoid changing original data
     merged_lines = merge_spans(filtered)
-    text_blocks = merge_lines(merged_lines, filtered)
+    text_blocks = merge_lines(merged_lines)
     text_blocks = filter_common_titles(text_blocks)
     full_text = get_full_text(text_blocks)
 
     # Handle empty blocks being joined
-    full_text = re.sub(r'\n{3,}', '\n\n', full_text)
-    full_text = re.sub(r'(\n\s){3,}', '\n\n', full_text)
+    full_text = cleanup_text(full_text)
 
     # Replace bullet characters with a -
     full_text = replace_bullets(full_text)
 
     # Postprocess text with editor model
     full_text, edit_stats = edit_full_text(
         full_text,
         edit_model,
-        batch_size=settings.EDITOR_BATCH_SIZE * parallel_factor
+        batch_multiplier=batch_multiplier
     )
+    flush_cuda_memory()
     out_meta["postprocess_stats"] = {"edit": edit_stats}
+    doc_images = images_to_dict(pages)
 
-    return full_text, out_meta
+    return full_text, doc_images, out_meta
```

### Comparing `marker_pdf-0.1.3/marker/debug/data.py` & `marker_pdf-0.2.1/marker/debug/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 import os
-import zlib
 from typing import List
 
-from marker.schema import Page
+from marker.pdf.images import render_image
+from marker.schema.page import Page
 from marker.settings import settings
 from PIL import Image
 import io
 
 
 def dump_equation_debug_data(doc, images, converted_spans):
     if not settings.DEBUG_DATA_FOLDER or settings.DEBUG_LEVEL == 0:
@@ -17,19 +17,18 @@
     if len(images) == 0:
         return
 
     # We attempted one conversion per image
     assert len(converted_spans) == len(images)
 
     data_lines = []
-    for idx, (image, converted_span) in enumerate(zip(images, converted_spans)):
+    for idx, (pil_image, converted_span) in enumerate(zip(images, converted_spans)):
         if converted_span is None:
             continue
         # Image is a BytesIO object
-        pil_image = Image.open(image)
         img_bytes = io.BytesIO()
         pil_image.save(img_bytes, format="WEBP", lossless=True)
         b64_image = base64.b64encode(img_bytes.getvalue()).decode("utf-8")
         data_lines.append({
             "image": b64_image,
             "text": converted_span.text,
             "bbox": converted_span.bbox
@@ -51,17 +50,15 @@
     doc_base = os.path.basename(doc.name).rsplit(".", 1)[0]
 
     debug_file = os.path.join(settings.DEBUG_DATA_FOLDER, f"{doc_base}_bbox.json")
     debug_data = []
     for idx, page_blocks in enumerate(blocks):
         page = doc[idx]
 
-        pix = page.get_pixmap(dpi=settings.TEXIFY_DPI, annots=False, clip=page_blocks.bbox)
-        png = pix.pil_tobytes(format="PNG")
-        png_image = Image.open(io.BytesIO(png))
+        png_image = render_image(page, dpi=settings.TEXIFY_DPI)
         width, height = png_image.size
         max_dimension = 6000
         if width > max_dimension or height > max_dimension:
             scaling_factor = min(max_dimension / width, max_dimension / height)
             png_image = png_image.resize((int(width * scaling_factor), int(height * scaling_factor)), Image.ANTIALIAS)
 
         img_bytes = io.BytesIO()
```

### Comparing `marker_pdf-0.1.3/marker/markdown.py` & `marker_pdf-0.2.1/marker/postprocessors/markdown.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,74 @@
-from marker.schema import MergedLine, MergedBlock, FullyMergedBlock, Page
+from marker.schema.merged import MergedLine, MergedBlock, FullyMergedBlock
+from marker.schema.page import Page
 import re
+import regex
 from typing import List
 
 
+def escape_markdown(text):
+    # List of characters that need to be escaped in markdown
+    characters_to_escape = r"[#]"
+    # Escape each of these characters with a backslash
+    escaped_text = re.sub(characters_to_escape, r'\\\g<0>', text)
+    return escaped_text
+
+
 def surround_text(s, char_to_insert):
     leading_whitespace = re.match(r'^(\s*)', s).group(1)
     trailing_whitespace = re.search(r'(\s*)$', s).group(1)
     stripped_string = s.strip()
     modified_string = char_to_insert + stripped_string + char_to_insert
     final_string = leading_whitespace + modified_string + trailing_whitespace
     return final_string
 
 
-def merge_spans(blocks):
+def merge_spans(pages: List[Page]) -> List[List[MergedBlock]]:
     merged_blocks = []
-    for page in blocks:
+    for page in pages:
         page_blocks = []
         for blocknum, block in enumerate(page.blocks):
             block_lines = []
-            block_types = []
             for linenum, line in enumerate(block.lines):
                 line_text = ""
                 if len(line.spans) == 0:
                     continue
                 fonts = []
                 for i, span in enumerate(line.spans):
                     font = span.font.lower()
-                    next_font = None
+                    next_span = None
                     next_idx = 1
                     while len(line.spans) > i + next_idx:
                         next_span = line.spans[i + next_idx]
-                        next_font = next_span.font.lower()
                         next_idx += 1
                         if len(next_span.text.strip()) > 2:
                             break
 
                     fonts.append(font)
-                    block_types.append(span.block_type)
                     span_text = span.text
 
                     # Don't bold or italicize very short sequences
                     # Avoid bolding first and last sequence so lines can be joined properly
                     if len(span_text) > 3 and 0 < i < len(line.spans) - 1:
-                        if "ital" in font and (not next_font or "ital" not in next_font):
+                        if span.italic and (not next_span or not next_span.italic):
                             span_text = surround_text(span_text, "*")
-                        elif "bold" in font and (not next_font or "bold" not in next_font):
+                        elif span.bold and (not next_span or not next_span.bold):
                             span_text = surround_text(span_text, "**")
                     line_text += span_text
                 block_lines.append(MergedLine(
                     text=line_text,
                     fonts=fonts,
                     bbox=line.bbox
                 ))
             if len(block_lines) > 0:
                 page_blocks.append(MergedBlock(
                     lines=block_lines,
                     pnum=block.pnum,
                     bbox=block.bbox,
-                    block_types=block_types
+                    block_type=block.block_type
                 ))
         merged_blocks.append(page_blocks)
 
     return merged_blocks
 
 
 def block_surround(text, block_type):
@@ -70,67 +77,77 @@
             text = "\n## " + text.strip().title() + "\n"
     elif block_type == "Title":
         if not text.startswith("#"):
             text = "# " + text.strip().title() + "\n"
     elif block_type == "Table":
         text = "\n" + text + "\n"
     elif block_type == "List-item":
-        pass
+        text = escape_markdown(text)
     elif block_type == "Code":
-        text = "\n" + text + "\n"
+        text = "\n```\n" + text + "\n```\n"
+    elif block_type == "Text":
+        text = escape_markdown(text)
+    elif block_type == "Formula":
+        if text.strip().startswith("$$") and text.strip().endswith("$$"):
+            text = text.strip()
+            text = "\n" + text + "\n"
     return text
 
 
 def line_separator(line1, line2, block_type, is_continuation=False):
     # Should cover latin-derived languages and russian
-    lowercase_letters = "a-zà-öø-ÿа-яşćăâđêôơưþðæøå"
-    uppercase_letters = "A-ZÀ-ÖØ-ßА-ЯŞĆĂÂĐÊÔƠƯÞÐÆØÅ"
+    lowercase_letters = r'\p{Lo}|\p{Ll}|\d'
     # Remove hyphen in current line if next line and current line appear to be joined
-    hyphen_pattern = re.compile(rf'.*[{lowercase_letters}][-]\s?$', re.DOTALL)
-    if line1 and hyphen_pattern.match(line1) and re.match(rf"^[{lowercase_letters}]", line2):
+    hyphen_pattern = regex.compile(rf'.*[{lowercase_letters}][-]\s?$', regex.DOTALL)
+    if line1 and hyphen_pattern.match(line1) and regex.match(rf"^\s?[{lowercase_letters}]", line2):
         # Split on — or - from the right
-        line1 = re.split(r"[-—]\s?$", line1)[0]
+        line1 = regex.split(r"[-—]\s?$", line1)[0]
         return line1.rstrip() + line2.lstrip()
 
-    lowercase_pattern1 = re.compile(rf'.*[{lowercase_letters},]\s?$', re.DOTALL)
-    lowercase_pattern2 = re.compile(rf'^\s?[{uppercase_letters}{lowercase_letters}]', re.DOTALL)
-    end_pattern = re.compile(r'.*[.?!]\s?$', re.DOTALL)
+    all_letters = r'\p{L}|\d'
+    sentence_continuations = r',;\(\—\"\''
+    sentence_ends = r'。ๆ\.?!'
+    line_end_pattern = regex.compile(rf'.*[{lowercase_letters}][{sentence_continuations}]?\s?$', regex.DOTALL)
+    line_start_pattern = regex.compile(rf'^\s?[{all_letters}]', regex.DOTALL)
+    sentence_end_pattern = regex.compile(rf'.*[{sentence_ends}]\s?$', regex.DOTALL)
 
     if block_type in ["Title", "Section-header"]:
         return line1.rstrip() + " " + line2.lstrip()
-    elif lowercase_pattern1.match(line1) and lowercase_pattern2.match(line2) and block_type == "Text":
+    elif block_type == "Formula":
+        return line1 + "\n" + line2
+    elif line_end_pattern.match(line1) and line_start_pattern.match(line2) and block_type == "Text":
         return line1.rstrip() + " " + line2.lstrip()
     elif is_continuation:
         return line1.rstrip() + " " + line2.lstrip()
-    elif block_type == "Text" and end_pattern.match(line1):
+    elif block_type == "Text" and sentence_end_pattern.match(line1):
+        return line1 + "\n\n" + line2
+    elif block_type == "Table":
         return line1 + "\n\n" + line2
-    elif block_type == "Formula":
-        return line1 + " " + line2
     else:
         return line1 + "\n" + line2
 
 
 def block_separator(line1, line2, block_type1, block_type2):
     sep = "\n"
     if block_type1 == "Text":
         sep = "\n\n"
 
     return sep + line2
 
 
-def merge_lines(blocks, page_blocks: List[Page]):
+def merge_lines(blocks: List[List[MergedBlock]]):
     text_blocks = []
     prev_type = None
     prev_line = None
     block_text = ""
     block_type = ""
-    common_line_heights = [p.get_line_height_stats() for p in page_blocks]
+
     for page in blocks:
         for block in page:
-            block_type = block.most_common_block_type()
+            block_type = block.block_type
             if block_type != prev_type and prev_type:
                 text_blocks.append(
                     FullyMergedBlock(
                         text=block_surround(block_text, prev_type),
                         block_type=prev_type
                     )
                 )
```

### Comparing `marker_pdf-0.1.3/marker/postprocessors/editor.py` & `marker_pdf-0.2.1/marker/postprocessors/editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-from collections import defaultdict, Counter
+from collections import defaultdict
 from itertools import chain
 from typing import Optional
 
-from transformers import AutoTokenizer
 from marker.settings import settings
 import torch
 import torch.nn.functional as F
 from marker.postprocessors.t5 import T5ForTokenClassification, byt5_tokenize
 
 
+def get_batch_size():
+    if settings.EDITOR_BATCH_SIZE is not None:
+        return settings.EDITOR_BATCH_SIZE
+    elif settings.TORCH_DEVICE_MODEL == "cuda":
+        return 12
+    return 6
+
+
 def load_editing_model():
     if not settings.ENABLE_EDITOR_MODEL:
         return None
 
     model = T5ForTokenClassification.from_pretrained(
             settings.EDITOR_MODEL_NAME,
             torch_dtype=settings.MODEL_DTYPE,
@@ -25,18 +32,19 @@
         "newline-1": 2,
         "space-1": 3,
     }
     model.config.id2label = {v: k for k, v in model.config.label2id.items()}
     return model
 
 
-def edit_full_text(text: str, model: Optional[T5ForTokenClassification], batch_size: int = settings.EDITOR_BATCH_SIZE):
+def edit_full_text(text: str, model: Optional[T5ForTokenClassification], batch_multiplier=1) -> (str, dict):
     if not model:
         return text, {}
 
+    batch_size = get_batch_size() * batch_multiplier
     tokenized = byt5_tokenize(text, settings.EDITOR_MAX_LENGTH)
     input_ids = tokenized["input_ids"]
     char_token_lengths = tokenized["char_token_lengths"]
 
     # Run model
     token_masks = []
     for i in range(0, len(input_ids), batch_size):
```

### Comparing `marker_pdf-0.1.3/marker/postprocessors/t5.py` & `marker_pdf-0.2.1/marker/postprocessors/t5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from transformers import T5Config, T5PreTrainedModel
 import torch
 from torch import nn
 from copy import deepcopy
-from typing import Optional, Tuple, Union, List
+from typing import Optional, Tuple, Union
 from itertools import chain
 
 from transformers.modeling_outputs import TokenClassifierOutput
 from transformers.models.t5.modeling_t5 import T5Stack
 from transformers.utils.model_parallel_utils import get_device_map, assert_device_map
```

### Comparing `marker_pdf-0.1.3/marker/settings.py` & `marker_pdf-0.2.1/marker/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os
-from typing import Optional, List, Dict
+from typing import Optional, List, Dict, Literal
 
 from dotenv import find_dotenv
 from pydantic import computed_field
 from pydantic_settings import BaseSettings
-import fitz as pymupdf
 import torch
 
 
 class Settings(BaseSettings):
     # General
-    TORCH_DEVICE: Optional[str] = None
+    TORCH_DEVICE: Optional[str] = None # Note: MPS device does not work for text detection, and will default to CPU
+    IMAGE_DPI: int = 96 # DPI to render images pulled from pdf at
+    EXTRACT_IMAGES: bool = True # Extract images from pdfs and save them
 
     @computed_field
     @property
     def TORCH_DEVICE_MODEL(self) -> str:
         if self.TORCH_DEVICE is not None:
             return self.TORCH_DEVICE
 
@@ -23,101 +23,78 @@
 
         if torch.backends.mps.is_available():
             return "mps"
 
         return "cpu"
 
     INFERENCE_RAM: int = 40 # How much VRAM each GPU has (in GB).
-    VRAM_PER_TASK: float = 2.5 # How much VRAM to allocate per task (in GB).  Peak marker VRAM usage is around 3GB, but avg across workers is lower.
+    VRAM_PER_TASK: float = 4 # How much VRAM to allocate per task (in GB).  Peak marker VRAM usage is around 5GB, but avg across workers is lower.
     DEFAULT_LANG: str = "English" # Default language we assume files to be in, should be one of the keys in TESSERACT_LANGUAGES
 
     SUPPORTED_FILETYPES: Dict = {
         "application/pdf": "pdf",
-        "application/epub+zip": "epub",
-        "application/x-mobipocket-ebook": "mobi",
-        "application/vnd.ms-xpsdocument": "xps",
-        "application/x-fictionbook+xml": "fb2"
     }
 
-    # PyMuPDF
-    TEXT_FLAGS: int = pymupdf.TEXTFLAGS_DICT & ~pymupdf.TEXT_PRESERVE_LIGATURES & ~pymupdf.TEXT_PRESERVE_IMAGES
+    # Text line Detection
+    DETECTOR_BATCH_SIZE: Optional[int] = None # Defaults to 6 for CPU, 12 otherwise
+    SURYA_DETECTOR_DPI: int = 96
+    DETECTOR_POSTPROCESSING_CPU_WORKERS: int = 4
 
     # OCR
     INVALID_CHARS: List[str] = [chr(0xfffd), "�"]
-    OCR_DPI: int = 400
-    TESSDATA_PREFIX: str = ""
-    TESSERACT_LANGUAGES: Dict = {
-        "English": "eng",
-        "Spanish": "spa",
-        "Portuguese": "por",
-        "French": "fra",
-        "German": "deu",
-        "Russian": "rus",
-        "Chinese": "chi_sim",
-        "Japanese": "jpn",
-        "Korean": "kor",
-        "Hindi": "hin",
-    }
-    TESSERACT_TIMEOUT: int = 20 # When to give up on OCR
-    SPELLCHECK_LANGUAGES: Dict = {
-        "English": "en",
-        "Spanish": "es",
-        "Portuguese": "pt",
-        "French": "fr",
-        "German": "de",
-        "Russian": "ru",
-        "Chinese": None,
-        "Japanese": None,
-        "Korean": None,
-        "Hindi": None,
-    }
+    OCR_ENGINE: Optional[Literal["surya", "ocrmypdf"]] = "surya" # Which OCR engine to use, either "surya" or "ocrmypdf".  Defaults to "ocrmypdf" on CPU, "surya" on GPU.
     OCR_ALL_PAGES: bool = False # Run OCR on every page even if text can be extracted
+
+    ## Surya
+    SURYA_OCR_DPI: int = 96
+    RECOGNITION_BATCH_SIZE: Optional[int] = None # Batch size for surya OCR defaults to 64 for cuda, 32 otherwise
+
+    ## Tesseract
     OCR_PARALLEL_WORKERS: int = 2 # How many CPU workers to use for OCR
-    OCR_ENGINE: str = "ocrmypdf" # Which OCR engine to use, either "tesseract" or "ocrmypdf".  Ocrmypdf is higher quality, but slower.
+    TESSERACT_TIMEOUT: int = 20 # When to give up on OCR
+    TESSDATA_PREFIX: str = ""
 
     # Texify model
     TEXIFY_MODEL_MAX: int = 384 # Max inference length for texify
     TEXIFY_TOKEN_BUFFER: int = 256 # Number of tokens to buffer above max for texify
     TEXIFY_DPI: int = 96 # DPI to render images at
-    TEXIFY_BATCH_SIZE: int = 1 if TORCH_DEVICE_MODEL == "cpu" else 6 # Batch size for texify, don't batch on cpu
+    TEXIFY_BATCH_SIZE: Optional[int] = None # Defaults to 6 for cuda, 12 otherwise
     TEXIFY_MODEL_NAME: str = "vikp/texify"
 
     # Layout model
+    SURYA_LAYOUT_DPI: int = 96
     BAD_SPAN_TYPES: List[str] = ["Caption", "Footnote", "Page-footer", "Page-header", "Picture"]
-    LAYOUT_MODEL_MAX: int = 512
-    LAYOUT_CHUNK_OVERLAP: int = 64
-    LAYOUT_DPI: int = 96
-    LAYOUT_MODEL_NAME: str = "vikp/layout_segmenter"
-    LAYOUT_BATCH_SIZE: int = 8 # Max 512 tokens means high batch size
+    LAYOUT_MODEL_CHECKPOINT: str = "vikp/surya_layout2"
+    BBOX_INTERSECTION_THRESH: float = 0.7 # How much the layout and pdf bboxes need to overlap to be the same
+    LAYOUT_BATCH_SIZE: Optional[int] = None # Defaults to 12 for cuda, 6 otherwise
 
     # Ordering model
-    ORDERER_BATCH_SIZE: int = 32 # This can be high, because max token count is 128
-    ORDERER_MODEL_NAME: str = "vikp/column_detector"
+    SURYA_ORDER_DPI: int = 96
+    ORDER_BATCH_SIZE: Optional[int] = None  # Defaults to 12 for cuda, 6 otherwise
 
     # Final editing model
-    EDITOR_BATCH_SIZE: int = 4
+    EDITOR_BATCH_SIZE: Optional[int] = None # Defaults to 6 for cuda, 12 otherwise
     EDITOR_MAX_LENGTH: int = 1024
     EDITOR_MODEL_NAME: str = "vikp/pdf_postprocessor_t5"
     ENABLE_EDITOR_MODEL: bool = False # The editor model can create false positives
     EDITOR_CUTOFF_THRESH: float = 0.9 # Ignore predictions below this probability
 
     # Ray
     RAY_CACHE_PATH: Optional[str] = None # Where to save ray cache
-    RAY_DASHBOARD_HOST: str = "127.0.0.1"
     RAY_CORES_PER_WORKER: int = 1 # How many cpu cores to allocate per worker
 
     # Debug
     DEBUG: bool = False # Enable debug logging
     DEBUG_DATA_FOLDER: Optional[str] = None
     DEBUG_LEVEL: int = 0 # 0 to 2, 2 means log everything
 
     @computed_field
     @property
     def CUDA(self) -> bool:
-        return "cuda" in self.TORCH_DEVICE
+        return "cuda" in self.TORCH_DEVICE_MODEL
 
     @computed_field
     @property
     def MODEL_DTYPE(self) -> torch.dtype:
         if self.TORCH_DEVICE_MODEL == "cuda":
             return torch.bfloat16
         else:
```

### Comparing `marker_pdf-0.1.3/pyproject.toml` & `marker_pdf-0.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,58 +1,51 @@
 [tool.poetry]
 name = "marker-pdf"
-version = "0.1.3"
+version = "0.2.1"
 description = "Convert PDF to markdown with high speed and accuracy."
 authors = ["Vik Paruchuri <github@vikas.sh>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/marker"
 keywords = ["pdf", "markdown", "ocr", "nlp"]
 packages = [
     {include = "marker"}
 ]
 include = [
     "convert.py",
     "convert_single.py",
     "chunk_convert.sh",
-    "benchmark.py",
     "chunk_convert.py",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13,!=3.9.7"
 scikit-learn = "^1.3.2"
 Pillow = "^10.1.0"
-pytesseract = "^0.3.10"
-PyMuPDF = "^1.23.5"
-pymupdf-fonts = "^1.0.5"
 pydantic = "^2.4.2"
 pydantic-settings = "^2.0.3"
-transformers = "^4.34.1"
+transformers = "^4.36.2" # 4.36.2 needed because issues with donut models and later versions
 numpy = "^1.26.1"
 python-dotenv = "^1.0.0"
-torch = "^2.1.1"
-ray = "^2.7.1"
+torch = "^2.2.2" # Issue with torch 2.3.0 and vision models - https://github.com/pytorch/pytorch/issues/121834
+ray = "^2.20.0"
 tqdm = "^4.66.1"
 tabulate = "^0.9.0"
-thefuzz = "^0.20.0"
-python-magic = "^0.4.27"
-pyspellchecker = "^0.7.2"
 ftfy = "^6.1.1"
-nltk = "^3.8.1"
-ocrmypdf = "^15.4.0"
-bitsandbytes = "^0.41.2.post2"
-grpcio = "^1.60.0"
 texify = "^0.1.8"
+rapidfuzz = "^3.8.1"
+surya-ocr = "^0.4.3"
+filetype = "^1.2.0"
+regex = "^2024.4.28"
+pdftext = "^0.3.7"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 
 [tool.poetry.scripts]
 marker = "convert:main"
 marker_single = "convert_single:main"
-marker_benchmark = "benchmark:main"
 marker_chunk_convert = "chunk_convert:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `marker_pdf-0.1.3/PKG-INFO` & `marker_pdf-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,65 @@
 Metadata-Version: 2.1
 Name: marker-pdf
-Version: 0.1.3
+Version: 0.2.1
 Summary: Convert PDF to markdown with high speed and accuracy.
 Home-page: https://github.com/VikParuchuri/marker
 License: GPL-3.0-or-later
 Keywords: pdf,markdown,ocr,nlp
 Author: Vik Paruchuri
 Author-email: github@vikas.sh
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=10.1.0,<11.0.0)
-Requires-Dist: PyMuPDF (>=1.23.5,<2.0.0)
-Requires-Dist: bitsandbytes (>=0.41.2.post2,<0.42.0)
+Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
-Requires-Dist: grpcio (>=1.60.0,<2.0.0)
-Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
-Requires-Dist: ocrmypdf (>=15.4.0,<16.0.0)
+Requires-Dist: pdftext (>=0.3.7,<0.4.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0)
-Requires-Dist: pymupdf-fonts (>=1.0.5,<2.0.0)
-Requires-Dist: pyspellchecker (>=0.7.2,<0.8.0)
-Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: python-magic (>=0.4.27,<0.5.0)
-Requires-Dist: ray (>=2.7.1,<3.0.0)
+Requires-Dist: rapidfuzz (>=3.8.1,<4.0.0)
+Requires-Dist: ray (>=2.20.0,<3.0.0)
+Requires-Dist: regex (>=2024.4.28,<2025.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
+Requires-Dist: surya-ocr (>=0.4.3,<0.5.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: texify (>=0.1.8,<0.2.0)
-Requires-Dist: thefuzz (>=0.20.0,<0.21.0)
-Requires-Dist: torch (>=2.1.1,<3.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
-Requires-Dist: transformers (>=4.34.1,<5.0.0)
+Requires-Dist: transformers (>=4.36.2,<5.0.0)
 Project-URL: Repository, https://github.com/VikParuchuri/marker
 Description-Content-Type: text/markdown
 
 # Marker
 
-Marker converts PDF, EPUB, and MOBI to markdown.  It's 10x faster than nougat, more accurate on most documents, and has low hallucination risk.
+Marker converts PDF to markdown quickly and accurately.
 
-- Support for a range of PDF documents (optimized for books and scientific papers)
+- Supports a wide range of documents (optimized for books and scientific papers)
+- Supports all languages
 - Removes headers/footers/other artifacts
+- Formats tables and code blocks
+- Extracts and saves images along with the markdown
 - Converts most equations to latex
-- Formats code blocks and tables
-- Support for multiple languages (although most testing is done in English).  See `settings.py` for a language list.
 - Works on GPU, CPU, or MPS
 
 ## How it works
 
 Marker is a pipeline of deep learning models:
 
-- Extract text, OCR if necessary (heuristics, tesseract)
-- Detect page layout ([layout segmenter](https://huggingface.co/vikp/layout_segmenter), [column detector](https://huggingface.co/vikp/column_detector))
-- Clean and format each block (heuristics, [nougat](https://huggingface.co/facebook/nougat-base))
+- Extract text, OCR if necessary (heuristics, [surya](https://github.com/VikParuchuri/surya), tesseract)
+- Detect page layout and find reading order ([surya](https://github.com/VikParuchuri/surya))
+- Clean and format each block (heuristics, [texify](https://github.com/VikParuchuri/texify)
 - Combine blocks and postprocess complete text (heuristics, [pdf_postprocessor](https://huggingface.co/vikp/pdf_postprocessor_t5))
 
-Relying on autoregressive forward passes to generate text is slow and prone to hallucination/repetition.  From the nougat paper: `We observed [repetition] in 1.5% of pages in the test set, but the frequency increases for out-of-domain documents.`  In my anecdotal testing, repetitions happen on 5%+ of out-of-domain (non-arXiv) pages.  
-
-Nougat is an amazing model, but I wanted a faster and more general purpose solution. Marker is 10x faster and has low hallucination risk because it only passes equation blocks through an LLM forward pass.
+It only uses models where necessary, which improves speed and accuracy.
 
 ## Examples
 
 | PDF                                                                   | Type        | Marker                                                                                                 | Nougat                                                                                                 |
 |-----------------------------------------------------------------------|-------------|--------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
 | [Think Python](https://greenteapress.com/thinkpython/thinkpython.pdf) | Textbook    | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/thinkpython.md)         | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/thinkpython.md)         |
 | [Think OS](https://greenteapress.com/thinkos/thinkos.pdf)             | Textbook    | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/marker/thinkos.md)             | [View](https://github.com/VikParuchuri/marker/blob/master/data/examples/nougat/thinkos.md)             |
@@ -85,177 +79,169 @@
 
 [Discord](https://discord.gg//KuZwXNGnfH) is where we discuss future development.
 
 # Limitations
 
 PDF is a tricky format, so marker will not always work perfectly.  Here are some known limitations that are on the roadmap to address:
 
-- Marker will convert fewer equations to latex than nougat.  This is because it has to first detect equations, then convert them without hallucation.
+- Marker will not convert 100% of equations to LaTeX.  This is because it has to detect then convert.
 - Whitespace and indentations are not always respected.
 - Not all lines/spans will be joined properly.
-- Languages similar to English (Spanish, French, German, Russian, etc) have the best support. There is provisional support for Chinese, Japanese, Korean, and Hindi, but it may not work as well.
 - This works best on digital PDFs that won't require a lot of OCR.  It's optimized for speed, and limited OCR is used to fix errors.
 
 # Installation
 
-This has been tested on Mac and Linux (Ubuntu and Debian).  You'll need python 3.9+ and [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer).
+This has been tested on Mac and Linux (Ubuntu and Debian).  You'll need python 3.9+ and PyTorch.  You may need to install the CPU version of torch first if you're not using a Mac or a GPU machine.  See [here](https://pytorch.org/get-started/locally/) for more details.
+
+Install with:
 
-First, clone the repo:
+```shell
+pip install marker-pdf
+```
 
-- `git clone https://github.com/VikParuchuri/marker.git`
-- `cd marker`
+## Optional
 
-## Linux
+Only needed if using `ocrmypdf` as the ocr backend.
 
-- Install system requirements
-  - Optional: Install tesseract 5 by following [these instructions](https://notesalexp.org/tesseract-ocr/html/) or running `scripts/install/tesseract_5_install.sh`.
-  - Install ghostscript > 9.55 by following [these instructions](https://ghostscript.readthedocs.io/en/latest/Install.html) or running `scripts/install/ghostscript_install.sh`.
-  - Install other requirements with `cat scripts/install/apt-requirements.txt | xargs sudo apt-get install -y`
+**Linux**
+
+- Run `pip install ocrmypdf`
+- Install ghostscript > 9.55 by following [these instructions](https://ghostscript.readthedocs.io/en/latest/Install.html) or running `scripts/install/ghostscript_install.sh`.
+- Install other requirements with `cat scripts/install/tess-apt-requirements.txt | xargs sudo apt-get install -y`
 - Set the tesseract data folder path
   - Find the tesseract data folder `tessdata` with `find / -name tessdata`.  Make sure to use the one corresponding to the latest tesseract version if you have multiple.
   - Create a `local.env` file in the root `marker` folder with `TESSDATA_PREFIX=/path/to/tessdata` inside it
-- Install python requirements
-  - `poetry install`
-  - `poetry shell` to activate your poetry venv
-- Update pytorch since poetry doesn't play nicely with it
-  - GPU only: run `pip install torch` to install other torch dependencies.
-  - CPU only: Uninstall torch with `poetry remove torch`, then follow the [CPU install](https://pytorch.org/get-started/locally/) instructions.
 
-## Mac
+**Mac**
+
+Only needed if using `ocrmypdf` as the ocr backend.
 
-- Install system requirements from `scripts/install/brew-requirements.txt`
+- Run `pip install ocrmypdf`
+- Install system requirements from `scripts/install/tess-brew-requirements.txt`
 - Set the tesseract data folder path
   - Find the tesseract data folder `tessdata` with `brew list tesseract`
   - Create a `local.env` file in the root `marker` folder with `TESSDATA_PREFIX=/path/to/tessdata` inside it
-- Install python requirements
-  - `poetry install`
-  - `poetry shell` to activate your poetry venv
-- On ARM macs (M1+), make sure to set the `TORCH_DEVICE` setting to `mps` (more details below) for a speedup
 
 # Usage
 
-First, some configuration:
+First, some configuration.  Note that settings can be overridden with env vars.
 
-- Set your torch device in the `local.env` file.  For example, `TORCH_DEVICE=cuda` or `TORCH_DEVICE=mps`.  `cpu` is the default.
+- Inspect the settings in `marker/settings.py`.  You can override any settings with environment variables.
+- Your torch device will be automatically detected, but you can override this.  For example, `TORCH_DEVICE=cuda`.
   - If using GPU, set `INFERENCE_RAM` to your GPU VRAM (per GPU).  For example, if you have 16 GB of VRAM, set `INFERENCE_RAM=16`.
   - Depending on your document types, marker's average memory usage per task can vary slightly.  You can configure `VRAM_PER_TASK` to adjust this if you notice tasks failing with GPU out of memory errors.
-- Inspect the other settings in `marker/settings.py`.  You can override any settings in the `local.env` file, or by setting environment variables.
-  - By default, the final editor model is off.  Turn it on with `ENABLE_EDITOR_MODEL`.
-  - By default, marker will use ocrmypdf for OCR, which is slower than base tesseract, but higher quality.  You can change this with the `OCR_ENGINE` setting.
+- By default, marker will use `surya` for OCR.  Surya is slower on CPU, but more accurate than tesseract.  If you want faster OCR, set `OCR_ENGINE` to `ocrmypdf`. This also requires external dependencies (see above).  If you don't want OCR at all, set `OCR_ENGINE` to `None`.
 
 ## Convert a single file
 
-Run `convert_single.py`, like this:
-
-```
-python convert_single.py /path/to/file.pdf /path/to/output.md --parallel_factor 2 --max_pages 10
+```shell
+marker_single /path/to/file.pdf /path/to/output/folder --parallel_factor 2 --max_pages 10 --langs English
 ```
 
-- `--parallel_factor` is how much to increase batch size and parallel OCR workers by.  Higher numbers will take more VRAM and CPU, but process faster.  Set to 1 by default.
+- `--batch_multiplier` is how much to multiply default batch sizes by if you have extra VRAM.  Higher numbers will take more VRAM, but process faster.  Set to 2 by default.  The default batch sizes will take ~3GB of VRAM.
 - `--max_pages` is the maximum number of pages to process.  Omit this to convert the entire document.
+- `--langs` is a comma separated list of the languages in the document, for OCR
 
-Make sure the `DEFAULT_LANG` setting is set appropriately for your document.
+Make sure the `DEFAULT_LANG` setting is set appropriately for your document.  The list of supported languages for OCR is [here](https://github.com/VikParuchuri/surya/blob/master/surya/languages.py).  If you need more languages, you can use any language supported by [Tesseract](https://tesseract-ocr.github.io/tessdoc/Data-Files#data-files-for-version-400-november-29-2016) if you set `OCR_ENGINE` to `ocrmypdf`.  If you don't need OCR, marker can work with any language.
 
 ## Convert multiple files
 
-Run `convert.py`, like this:
-
-```
-python convert.py /path/to/input/folder /path/to/output/folder --workers 10 --max 10 --metadata_file /path/to/metadata.json --min_length 10000
+```shell
+marker /path/to/input/folder /path/to/output/folder --workers 10 --max 10 --metadata_file /path/to/metadata.json --min_length 10000
 ```
 
 - `--workers` is the number of pdfs to convert at once.  This is set to 1 by default, but you can increase it to increase throughput, at the cost of more CPU/GPU usage. Parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK` if you're using GPU.
 - `--max` is the maximum number of pdfs to convert.  Omit this to convert all pdfs in the folder.
-- `--metadata_file` is an optional path to a json file with metadata about the pdfs.  If you provide it, it will be used to set the language for each pdf.  If not, `DEFAULT_LANG` will be used. The format is:
 - `--min_length` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
+- `--metadata_file` is an optional path to a json file with metadata about the pdfs.  If you provide it, it will be used to set the language for each pdf.  If not, `DEFAULT_LANG` will be used. The format is:
 
 ```
 {
-  "pdf1.pdf": {"language": "English"},
-  "pdf2.pdf": {"language": "Spanish"},
+  "pdf1.pdf": {"languages": ["English"]},
+  "pdf2.pdf": {"languages": ["Spanish", "Russian"]},
   ...
 }
 ```
 
-## Convert multiple files on multiple GPUs
+You can use language names or codes.  The exact codes depend on the OCR engine.  See [here](https://github.com/VikParuchuri/surya/blob/master/surya/languages.py) for a full list for surya codes, and [here](https://tesseract-ocr.github.io/tessdoc/Data-Files#data-files-for-version-400-november-29-2016) for tesseract.
 
-Run `chunk_convert.sh`, like this:
+## Convert multiple files on multiple GPUs
 
-```
-MIN_LENGTH=10000 METADATA_FILE=../pdf_meta.json NUM_DEVICES=4 NUM_WORKERS=15 bash chunk_convert.sh ../pdf_in ../md_out
+```shell
+MIN_LENGTH=10000 METADATA_FILE=../pdf_meta.json NUM_DEVICES=4 NUM_WORKERS=15 marker_chunk_convert ../pdf_in ../md_out
 ```
 
 - `METADATA_FILE` is an optional path to a json file with metadata about the pdfs.  See above for the format.
 - `NUM_DEVICES` is the number of GPUs to use.  Should be `2` or greater.
 - `NUM_WORKERS` is the number of parallel processes to run on each GPU.  Per-GPU parallelism will not increase beyond `INFERENCE_RAM / VRAM_PER_TASK`.
 - `MIN_LENGTH` is the minimum number of characters that need to be extracted from a pdf before it will be considered for processing.  If you're processing a lot of pdfs, I recommend setting this to avoid OCRing pdfs that are mostly images. (slows everything down)
 
+Note that the env variables above are specific to this script, and cannot be set in `local.env`.
+
 # Benchmarks
 
-Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.
+Benchmarking PDF extraction quality is hard.  I've created a test set by finding books and scientific papers that have a pdf version and a latex source.  I convert the latex to text, and compare the reference to the output of text extraction methods.  It's noisy, but at least directionally correct.
 
-Benchmarks show that marker is 10x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
+Benchmarks show that marker is 4x faster than nougat, and more accurate outside arXiv (nougat was trained on arXiv data).  We show naive text extraction (pulling text out of the pdf with no processing) for comparison.
 
 **Speed**
 
 | Method | Average Score | Time per page | Time per document |
 |--------|---------------|---------------|-------------------|
-| naive  | 0.350727      | 0.00152378    | 0.326524          |
-| marker | 0.641062      | 0.360622      | 77.2762           |
-| nougat | 0.629211      | 3.77259       | 808.413           |
+| marker | 0.613721      | 0.631991      | 58.1432           |
+| nougat | 0.406603      | 2.59702       | 238.926           |
 
 **Accuracy**
 
 First 3 are non-arXiv books, last 3 are arXiv papers.
 
-| Method | switch_trans.pdf | crowd.pdf | multicolcnn.pdf | thinkos.pdf | thinkdsp.pdf | thinkpython.pdf |
-|--------|------------------|-----------|-----------------|-------------|--------------|-----------------|
-| naive  | 0.244114         | 0.140669  | 0.0868221       | 0.366856    | 0.412521     | 0.468281        |
-| marker | 0.482091         | 0.466882  | 0.537062        | 0.754347    | 0.78825      | 0.779536        |
-| nougat | 0.696458         | 0.552337  | 0.735099        | 0.655002    | 0.645704     | 0.650282        |
+| Method | multicolcnn.pdf | switch_trans.pdf | thinkpython.pdf | thinkos.pdf | thinkdsp.pdf | crowd.pdf |
+|--------|-----------------|------------------|-----------------|-------------|--------------|-----------|
+| marker | 0.536176        | 0.516833         | 0.70515         | 0.710657    | 0.690042     | 0.523467  |
+| nougat | 0.44009         | 0.588973         | 0.322706        | 0.401342    | 0.160842     | 0.525663  |
 
-Peak GPU memory usage during the benchmark is `3.3GB` for nougat, and `3.1GB` for marker.  Benchmarks were run on an A6000.
+Peak GPU memory usage during the benchmark is `4.2GB` for nougat, and `5.1GB` for marker.  Benchmarks were run on an A6000 Ada.
 
 **Throughput**
 
-Marker takes about 2GB of VRAM on average per task, so you can convert 24 documents in parallel on an A6000.
+Marker takes about 4GB of VRAM on average per task, so you can convert 12 documents in parallel on an A6000.
 
 ![Benchmark results](data/images/per_doc.png)
 
 ## Running your own benchmarks
 
-You can benchmark the performance of marker on your machine.  First, download the benchmark data [here](https://drive.google.com/file/d/1WiN4K2-jQfwyQMe4wSSurbpz3hxo2fG9/view?usp=drive_link) and unzip.
-
-Then run `benchmark.py` like this:
+You can benchmark the performance of marker on your machine. Install marker manually with:
 
+```shell
+git clone https://github.com/VikParuchuri/marker.git
+poetry install
 ```
+
+Download the benchmark data [here](https://drive.google.com/file/d/1ZSeWDo2g1y0BRLT7KnbmytV2bjWARWba/view?usp=sharing) and unzip. Then run `benchmark.py` like this:
+
+```shell
 python benchmark.py data/pdfs data/references report.json --nougat
 ```
 
 This will benchmark marker against other text extraction methods.  It sets up batch sizes for nougat and marker to use a similar amount of GPU RAM for each.
 
 Omit `--nougat` to exclude nougat from the benchmark.  I don't recommend running nougat on CPU, since it is very slow.
 
 # Commercial usage
 
-Due to the licensing of the underlying models like layoutlmv3 and nougat, this is only suitable for noncommercial usage.  
-
-I'm building a version that can be used commercially, by stripping out the dependencies below. If you would like to get early access, email me at marker@vikas.sh.
-
-Here are the non-commercial/restrictive dependencies:
+All models were trained from scratch, so they're okay for commercial usage.  The weights for the models are licensed cc-by-nc-sa-4.0, but I will waive that for any organization under $5M USD in gross revenue in the most recent 12-month period AND under $5M in lifetime VC/angel funding raised.
 
-- LayoutLMv3: CC BY-NC-SA 4.0 .  [Source](https://huggingface.co/microsoft/layoutlmv3-base)
-- Nougat: CC-BY-NC . [Source](https://github.com/facebookresearch/nougat)
-- PyMuPDF - GPL . [Source](https://pymupdf.readthedocs.io/en/latest/about.html#license-and-copyright)
+If you want to remove the GPL license requirements for inference or use the weights commercially over the revenue limit, please contact me at marker@vikas.sh for dual licensing.
 
-Other dependencies/datasets are openly licensed (doclaynet, byt5), or used in a way that is compatible with commercial usage (ghostscript).
+Note that the `ocrmypdf` OCR option will use ocrmypdf, which includes Ghostscript, an AGPL dependency, but calls it via CLI, so it does not trigger the license provisions.  Ocrmypdf is disabled by default, and will not be installed automatically.
 
 # Thanks
 
 This work would not have been possible without amazing open source models and datasets, including (but not limited to):
 
-- Nougat from Meta
-- Layoutlmv3 from Microsoft
+- Surya
+- Texify
+- Pypdfium2/pdfium
 - DocLayNet from IBM
 - ByT5 from Google
 
 Thank you to the authors of these models and datasets for making them available to the community!
```

