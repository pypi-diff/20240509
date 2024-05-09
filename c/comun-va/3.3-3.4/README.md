# Comparing `tmp/comun_va-3.3.tar.gz` & `tmp/comun_va-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-3.3.tar", last modified: Mon May  6 13:06:02 2024, max compression
+gzip compressed data, was "comun_va-3.4.tar", last modified: Thu May  9 07:51:33 2024, max compression
```

## Comparing `comun_va-3.3.tar` & `comun_va-3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 13:06:02.648731 comun_va-3.3/
--rw-rw-rw-   0        0        0       53 2024-05-06 13:06:02.647725 comun_va-3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 13:06:02.646423 comun_va-3.3/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8885 2024-05-06 13:01:57.000000 comun_va-3.3/comun_va.py
--rw-rw-rw-   0        0        0       42 2024-05-06 13:06:02.648731 comun_va-3.3/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-05-06 13:05:09.000000 comun_va-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:51:33.146875 comun_va-3.4/
+-rw-rw-rw-   0        0        0       53 2024-05-09 07:51:33.144870 comun_va-3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 07:51:33.143873 comun_va-3.4/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-05-09 07:51:33.000000 comun_va-3.4/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-09 07:51:33.000000 comun_va-3.4/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:51:33.000000 comun_va-3.4/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-09 07:51:33.000000 comun_va-3.4/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-09 07:51:33.000000 comun_va-3.4/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8868 2024-05-09 07:49:53.000000 comun_va-3.4/comun_va.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:51:33.147880 comun_va-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-09 07:51:29.000000 comun_va-3.4/setup.py
```

### Comparing `comun_va-3.3/comun_va.py` & `comun_va-3.4/comun_va.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,38 +119,38 @@
         cap.release()
         return frame
 
     except Exception as e:
         raise Exception(f"Error relacionado con la camara: {str(e)}")
 
 
-def read_barcode_from_ip_camera(camera_url: str, frames_to_read: int = 10) -> set[str]:
+def read_barcode_from_ip_camera(camera_url: str, intents: int = 3) -> set[str]:
     """
     Function that connect to an IP camera and return all the barcodes or QRs that can be read (without repeat)
     :param camera_url: need to be the RTSP URL
-    :param frames_to_read: quantity of frames that you want to use for reading the barcodes, has to be greater than 0
+    :param intents: how much tries to connect to the camera and read the barcode, must to be greater than 0
     :return: list of all barcodes read without repeat
     """
     try:
         barcodes = set()
-        cap = cv2.VideoCapture(camera_url)  # IP Camera
-        for _ in range(frames_to_read):
+        for _ in range(intents):
+            cap = cv2.VideoCapture(camera_url)  # IP Camera
             success, frame = cap.read()
             if not success:
                 raise Exception
             detected_barcodes = decode(frame)
             if detected_barcodes:
                 for barcode in detected_barcodes:
                     if barcode.data != "":
                         # Convert the byte string to a string
                         decoded_barcode = barcode.data.decode("utf-8")
                         # A set cannot have repeated elements, so we don't need to check if already exist.
                         barcodes.add(decoded_barcode)
 
-        cap.release()
+            cap.release()
         return barcodes
 
     except Exception as e:
         raise Exception(f"Error durante el proceso de lectura de código de barras: {str(e)}")
 
 
 def run_model_with_frame(img_frame, class_names: dict, model, output=False, limit_gpu=False,
```

