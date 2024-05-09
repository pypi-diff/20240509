# Comparing `tmp/qrcode_plus-3.1.0.tar.gz` & `tmp/qrcode_plus-3.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrcode_plus-3.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "qrcode_plus-3.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `qrcode_plus-3.1.0.tar` & `qrcode_plus-3.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.1.0/LICENSE
--rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.1.0/README.rst
--rw-r--r--   0        0        0     1783 2024-04-26 08:57:15.479609 qrcode_plus-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    16797 2024-04-17 13:45:44.788089 qrcode_plus-3.1.0/qrcode_plus.py
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1505 2024-04-13 16:10:05.922714 qrcode_plus-3.1.5/LICENSE
+-rw-r--r--   0        0        0     1003 2024-03-14 15:29:45.816329 qrcode_plus-3.1.5/README.rst
+-rw-r--r--   0        0        0     1783 2024-05-09 10:50:42.945423 qrcode_plus-3.1.5/pyproject.toml
+-rw-r--r--   0        0        0    17098 2024-05-09 10:49:34.712497 qrcode_plus-3.1.5/qrcode_plus.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 qrcode_plus-3.1.5/PKG-INFO
```

### Comparing `qrcode_plus-3.1.0/LICENSE` & `qrcode_plus-3.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.1.0/README.rst` & `qrcode_plus-3.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `qrcode_plus-3.1.0/pyproject.toml` & `qrcode_plus-3.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "qrcode-plus"
 description = "Advance Artistic (Micro) QR Code plugin for Segno"
-version = "3.1.0"
+version = "3.1.5"
 readme = "README.rst"
 license = {file = "LICENSE"}
 authors = [{"name" = "Kyle Bradley", email = "kbradley53@gmail.com"}]
 requires-python = ">= 3.5"
 keywords = ["QR Code", "Micro QR Code", "ISO/IEC 18004", "ISO/IEC 18004:2006(E)",
     "ISO/IEC 18004:2015(E)", "qrcode", "QR", "barcode", "matrix", "2D",]
 classifiers = [
```

### Comparing `qrcode_plus-3.1.0/qrcode_plus.py` & `qrcode_plus-3.1.5/qrcode_plus.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """\
 Segno writer plugin to convert a (Micro) QR code into a Pillow Image and
 and to add (animated) background images to QR codes.
 """
 from __future__ import absolute_import, unicode_literals, division
 import io
 import math
-from PIL import Image, ImageDraw, ImageSequence
+from PIL import Image, ImageDraw, ImageSequence, ImageOps
 from segno import consts
 try:
     from PIL.Image.Resampling import LANCZOS
 except ImportError:
     from PIL.Image import LANCZOS
 try:
     from PIL import UnidentifiedImageError
@@ -183,29 +183,39 @@
     target_supports_animation = ext in ('gif', 'png', 'webp')
     try:
         is_animated = target_supports_animation and bg_img.is_animated
     except AttributeError:
         pass
     durations = None
     loop = 0
+
     if is_animated:
         loop = bg_img.info.get('loop', 0)
         bg_images = [frame.copy() for frame in ImageSequence.Iterator(bg_img)]
         durations = [img.info.get('duration', 0) for img in bg_images]
     border = border if border is not None else qrcode.default_border_size
+
     bg_width, bg_height = bg_images[0].size
     ratio = min(max_bg_width / bg_width, max_bg_height / bg_height)
     bg_width, bg_height = int(bg_width * ratio), int(bg_height * ratio)
-    bg_tpl = Image.new('RGBA', (qr_img.width*boxSize, qr_img.height*boxSize), color='white')
-    tmp_bg_images = []
+    bg_tpl = Image.new('RGBA', (qr_img.width*boxSize, qr_img.height*boxSize))
+
     #new_canvas = Image.new('RGBA', (qr_img.width*boxSize, qr_img.height*boxSize), color='white')
 
     border_offset =  border * boxSize * scale
     border_nonBox =  border * scale
 
+    img1 = ImageDraw.Draw(bg_tpl)   
+    border_line = int(border_offset/5)
+    shape = [(0, 0), (qr_img.width*boxSize, qr_img.width*boxSize)] 
+    img1.rectangle(shape, fill ="white", outline ="black",  width=border_line) 
+
+    #bg_tpl = ImageOps.expand(bg_tpl,  border=border_line, fill='black')
+    
+    tmp_bg_images = []
     for img in (img.resize((bg_width, bg_height), LANCZOS) for img in bg_images):
         bg_img = bg_tpl.copy()
         tmp_bg_images.append(bg_img)
         #pos = (int(math.ceil((max_bg_width - img.size[0]) / 2)), int(math.ceil((max_bg_height - img.size[1]) / 2)))
         bg_img.paste(img, (border_offset,border_offset))
         #new_canvas.paste(img, (border_offset,border_offset))
```

### Comparing `qrcode_plus-3.1.0/PKG-INFO` & `qrcode_plus-3.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrcode-plus
-Version: 3.1.0
+Version: 3.1.5
 Summary: Advance Artistic (Micro) QR Code plugin for Segno
 Keywords: QR Code,Micro QR Code,ISO/IEC 18004,ISO/IEC 18004:2006(E),ISO/IEC 18004:2015(E),qrcode,QR,barcode,matrix,2D
 Author-email: Kyle Bradley <kbradley53@gmail.com>
 Requires-Python: >= 3.5
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

