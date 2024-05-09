# Comparing `tmp/mhdwriter-0.2.0.2.tar.gz` & `tmp/mhdwriter-0.2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mhdwriter-0.2.0.2.tar", max compression
+gzip compressed data, was "mhdwriter-0.2.0.3.tar", max compression
```

## Comparing `mhdwriter-0.2.0.2.tar` & `mhdwriter-0.2.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-05-08 13:57:58.812358 mhdwriter-0.2.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-08 13:57:58.812621 mhdwriter-0.2.0.2/mhdwriter/__init__.py
--rw-r--r--   0        0        0      525 2024-05-08 13:57:58.812724 mhdwriter-0.2.0.2/mhdwriter/args.py
--rw-r--r--   0        0        0     4616 2024-05-08 13:57:58.812840 mhdwriter-0.2.0.2/mhdwriter/header.py
--rw-r--r--   0        0        0     2979 2024-05-08 16:02:57.937116 mhdwriter-0.2.0.2/mhdwriter/writer.py
--rw-r--r--   0        0        0      366 2024-05-08 16:04:30.546094 mhdwriter-0.2.0.2/pyproject.toml
--rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 mhdwriter-0.2.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-08 17:57:29.606130 mhdwriter-0.2.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 17:57:29.606659 mhdwriter-0.2.0.3/mhdwriter/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-08 17:57:29.606820 mhdwriter-0.2.0.3/mhdwriter/args.py
+-rw-r--r--   0        0        0     4824 2024-05-08 17:57:29.606979 mhdwriter-0.2.0.3/mhdwriter/header.py
+-rw-r--r--   0        0        0     4595 2024-05-09 17:51:26.799556 mhdwriter-0.2.0.3/mhdwriter/writer.py
+-rw-r--r--   0        0        0      366 2024-05-09 19:06:46.232136 mhdwriter-0.2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      447 1970-01-01 00:00:00.000000 mhdwriter-0.2.0.3/PKG-INFO
```

### Comparing `mhdwriter-0.2.0.2/mhdwriter/args.py` & `mhdwriter-0.2.0.3/mhdwriter/args.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,21 @@
     NONE = 0
     RAW = 1
     RAW_COMPRESSED = 2
 
 
 @dataclass
 class WriteArgs:
-    write_type: WriteType
     fov: str
     series_description: str
     study_description: str
     protocol: str
     date_time: datetime | str
+    write_type: WriteType = WriteType.RAW
     root_site_id: str = "1.2.826.0.1.3680043.10.1341"
     downsample_factor: int = 0
     height: int = 0
     width: int = 0
     length: int = 0
     is_rgb: bool = False
     is_hdr: bool = False
+    skip_files: bool = True
```

### Comparing `mhdwriter-0.2.0.2/mhdwriter/header.py` & `mhdwriter-0.2.0.3/mhdwriter/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,21 @@
 
     assert type(args) == WriteArgs, "Invalid WriteArgs"
 
     if isinstance(args.date_time, str):
         study_date_time = parse_datetime(args.date_time)
     else:
         study_date_time = args.date_time
+    if not args.is_rgb and args.write_type == WriteType.NONE:
+        args.write_type = WriteType.RAW
 
     is_multi = True if args.write_type == WriteType.NONE else False
 
-    raw_name = args.study_description + ".raw"
-
+    raw_name = args.series_description + ".raw"
+    raw_name = raw_name.replace(" ", "_")
     if args.write_type == WriteType.RAW_COMPRESSED:
         raw_name += ".gz"
     pixel_sz = _pixel_size(args.fov.upper()) * (2 ** args.downsample_factor)
     pixel_sz = round(pixel_sz, 5)
 
     metadata = {
         "ObjectType": "Image",
@@ -73,14 +75,16 @@
     else:
         metadata["ElementDataFile"] = raw_name
     return metadata
 
 
 def _pixel_size(fov: str) -> float:
     fov = fov.upper()
+    fov = fov.replace("FOV", "")
+    fov = fov.replace(" ", "")
     xy = 0.00
     if fov == "A":
         xy = 0.020
     elif fov == "B":
         xy = 0.025
     elif fov == "C":
         xy = 0.035
```

### Comparing `mhdwriter-0.2.0.2/mhdwriter/writer.py` & `mhdwriter-0.2.0.3/mhdwriter/writer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,144 @@
 import shutil
+import threading
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Any
 
 import cv2
 import numpy as np
 
+try:
+    from tqdm import tqdm
+
+    has_tqdm = True
+except:
+    has_tqdm = False
 from mhdwriter.args import WriteArgs, WriteType
 from mhdwriter.header import generate_header
 
 
 def write_mhd_raw(
-    input_dir: Path, args: WriteArgs, out_path: Optional[Path] = None
-) -> bool:
+        input_dir: Path,
+        args: WriteArgs,
+        out_path: Optional[Path] = None,
+        show_progress: bool = True,
+        log_callback: Any = None,
+        cancel_event: Optional[threading.Event] = None,
+) -> Optional[Path]:
     """
     Convert a stack of files in a directory to a mhd/raw pair.
 
     Args:
         input_dir (Path): The directory containing the stack of files to convert to a volume.
         args (WriteArgs): WriteArgs object specifying parameters for the MHD header creation.
         out_path (Path): Optional path to specify output directory/file_base. If missing, metadata will be used
             to determine output file/path name in the input_dir.
+        cancel_event: optional event to cancel export early
 
     Returns:
-        bool: Returns True upon successful mhd/raw creation, else False.
+        Optional[Path]: Returns pathlib Path to mhd file upon successful mhd/raw creation, else None.
 
     """
-    all_files = list(input_dir.glob("*"))
+    if not args.is_rgb and args.write_type == WriteType.NONE:
+        args.write_type = WriteType.RAW
+
+    all_files = sorted(list(input_dir.glob("*")))
     all_files = [
         f
         for f in all_files
-        if f.suffix.lower()
-        in [".jpg", ".jxl", ".jp2", ".jpeg", ".png", ".tif", ".tiff"]
+        if f.is_file() and f.suffix.lower()
+           in [".jpg", ".jxl", ".jp2", ".jpeg", ".png", ".tif", ".tiff"]
     ]
     img = cv2.imread(str(all_files[0]), cv2.IMREAD_UNCHANGED)
     args.height, args.width = img.shape[:2]
     if args.downsample_factor > 0:
         dx_factor = 2 ** args.downsample_factor
-        args.height = args.height//dx_factor
-        args.width = args.width//dx_factor
+        if args.skip_files:
+            all_files = all_files[::dx_factor]
+        args.height = args.height // dx_factor
+        args.width = args.width // dx_factor
     args.length = len(all_files)
+
+    if is_cancelled(cancel_event):
+        return None
+
     metadata = generate_header(args)
 
     if not input_dir.exists():
         raise FileNotFoundError(f"Missing input dir {input_dir}")
 
     if out_path is None:
-        if args.write_type == WriteType.NONE:
-            out_path = input_dir
-        else:
-            out_path = input_dir.joinpath(f"{metadata['ElementDataFile']}")
+        out_path = input_dir
 
-    with out_path.open(mode="wb") as outfile:
-        for idx, img_file in enumerate(all_files):
-            try:
-                img = cv2.imread(str(img_file), cv2.IMREAD_UNCHANGED)
-            except Exception as e:
-                print(f"Error reading {str(img_file)}: {e}")
-                continue
-            if img is None:
-                print(f"Error reading {str(img_file)}")
-                continue
-            if args.is_rgb:
-                img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-            if not out_path.exists() and idx > 0:
-                return False
-
-            if args.downsample_factor > 0:
-                img = cv2.resize(
-                    img, (args.width, args.height), interpolation=cv2.INTER_AREA
-                )
-
-            if args.write_type == WriteType.NONE:
-                file_path = out_path.joinpath("slice_{0:04d}.jpg".format(idx + 1))
-                cv2.imwrite(str(file_path), img)
-            else:
-                squeezed = np.squeeze(img)
-                outfile.write(squeezed.tobytes())
+    outfile = None
 
+    if args.write_type == WriteType.NONE:
+        out_path = out_path.joinpath(f"{metadata['SeriesDescription']}")
+        out_path.mkdir(exist_ok=True, parents=True)
+    else:
+        out_path = out_path.joinpath(f"{metadata['ElementDataFile']}")
+        if out_path.exists():
+            print(f"File {out_path} already exists. Skipping.")
+            return
+        outfile = out_path.open(mode="wb")
+
+    out_name = out_path.name
+    if has_tqdm:
+        file_iterator = tqdm(all_files, desc=f"Generating {out_name}") if show_progress else all_files
+    else:
+        file_iterator = all_files
+
+    idx = 0
+    total = len(all_files)
+
+    for img_file in file_iterator:
+        try:
+            img = cv2.imread(str(img_file), cv2.IMREAD_UNCHANGED)
+        except Exception as e:
+            print(f"Error reading {str(img_file)}: {e}")
+            continue
+        if img is None:
+            print(f"Error reading {str(img_file)}")
+            continue
+        idx += 1
+        if args.is_rgb and not args.write_type == WriteType.NONE:
+            img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+
+        if args.downsample_factor > 0:
+            img = cv2.resize(
+                img, (args.width, args.height), interpolation=cv2.INTER_AREA
+            )
+
+        if is_cancelled(cancel_event):
+            if out_path.exists():
+                if args.write_type == WriteType.NONE:
+                    shutil.rmtree(out_path)
+                else:
+                    out_path.unlink()
+            return None
+
+        if args.write_type == WriteType.NONE:
+            file_path = out_path.joinpath("slice_{0:04d}.jpg".format(idx + 1))
+            cv2.imwrite(str(file_path), img)
+        else:
+            squeezed = np.squeeze(img)
+            outfile.write(squeezed.tobytes())
+        if log_callback is not None:
+            log_callback(f"Processed {out_path.name}: {idx}/{total}")
+    if outfile is not None:
+        outfile.close()
     if not out_path.exists():
         return False
-    mhd_path = out_path.parent.joinpath(f"{out_path.stem}.mhd")
+    if args.write_type == WriteType.NONE:
+        mhd_path = out_path.joinpath(f"{out_path.stem}.mhd")
+    else:
+        mhd_path = out_path.parent.joinpath(f"{out_path.stem}.mhd")
     with mhd_path.open("w") as mhd:
         for key in metadata:
             mhd.write(f"{key} = {metadata[key]}\n")
     return True
+
+
+def is_cancelled(stop_val) -> bool:
+    if stop_val is None:
+        return False
+    return stop_val.is_set()
```

