# Comparing `tmp/robotframework_creartramas-2.1.7.tar.gz` & `tmp/robotframework_creartramas-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_creartramas-2.1.7.tar", max compression
+gzip compressed data, was "robotframework_creartramas-2.1.8.tar", max compression
```

## Comparing `robotframework_creartramas-2.1.7.tar` & `robotframework_creartramas-2.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1946 2024-04-12 07:43:21.957445 robotframework_creartramas-2.1.7/docs/README.md
--rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.7/LICENSE
--rw-r--r--   0        0        0      670 2024-04-12 07:43:06.986592 robotframework_creartramas-2.1.7/pyproject.toml
--rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.7/TRAMAS/__init__.py
--rw-r--r--   0        0        0     2760 2024-04-12 07:42:46.909720 robotframework_creartramas-2.1.7/TRAMAS/creartramas.py
--rw-r--r--   0        0        0     2701 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1947 2024-05-09 08:35:25.507758 robotframework_creartramas-2.1.8/docs/README.md
+-rw-r--r--   0        0        0    11558 2024-03-20 08:37:40.627612 robotframework_creartramas-2.1.8/LICENSE
+-rw-r--r--   0        0        0      670 2024-05-09 08:34:45.934936 robotframework_creartramas-2.1.8/pyproject.toml
+-rw-r--r--   0        0        0      187 2024-03-27 10:02:55.311999 robotframework_creartramas-2.1.8/TRAMAS/__init__.py
+-rw-r--r--   0        0        0     2552 2024-05-09 08:33:36.108666 robotframework_creartramas-2.1.8/TRAMAS/creartramas.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 robotframework_creartramas-2.1.8/PKG-INFO
```

### Comparing `robotframework_creartramas-2.1.7/docs/README.md` & `robotframework_creartramas-2.1.8/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ${direccion_origen}=    01
     ${direccion_destino}=   02
     ${numero_bytes}=         08
     ${comando}=             FE
     @{datos}=               0x41    0x5A    0x4B
     ¡¡DATOS ES UNA LISTA!!
 
-    ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bits}    ${comando}    ${datos}
+    ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bytes}    ${comando}    @{datos}
     Log    Trama creada: ${trama}
 ```
 
 ## Funciones Disponibles
 
 `calcular_checksum(trama)`
```

### Comparing `robotframework_creartramas-2.1.7/LICENSE` & `robotframework_creartramas-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_creartramas-2.1.7/pyproject.toml` & `robotframework_creartramas-2.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robotframework-creartramas"
-version = "2.1.7"
+version = "2.1.8"
 description = "Creacion de tramas en hexadecimal"
 license = "Apache-2.0"
 authors = ["Anthony Arevalo"]
 maintainers = ["Anthony Arevalo"]
 readme = "./docs/README.md"
 homepage = "https://pypi.org/project/robotframework-creartramas"
 packages = [
```

### Comparing `robotframework_creartramas-2.1.7/TRAMAS/creartramas.py` & `robotframework_creartramas-2.1.8/TRAMAS/creartramas.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,20 @@
     def __init__(self) -> None:
         pass
     def calcular_checksum(self,trama):
         """
         Esta función toma una trama(bytearray) como entrada y calcula 
         el checksum para esa trama. Devuelve el valor entero del checksum.
         """
-        # Suma todos los valores ASCII de los caracteres en la trama 
-        check = sum(trama)
-        # Devuelve el checksum módulo 256, comprobando que: si check > 256 , el cheksum es 256 menos la diferencia que hay entre ambos
-        if check >= 256:
-            checksum = 256 - (abs(256-check))
-        else:
-            checksum = abs(256-check)
-        return checksum # valor absoluto por si cheksum es mayor que 256
-        
+        # Suma todos los valores ASCII de los caracteres en la trama  
+        check = sum(trama) % 256
+         # Calcular el complemento a 2 del resultado anterior
+        checksum = (256-check) % 256
+        return checksum 
+    
     def crear_trama(self,direccion_destino, numero_bytes, direccion_origen, comando, datos=[]):
         """
         Esta función construye una trama de acuerdo con la estructura proporcionada.Tiene 5 argumentos
         Hay que tener en cuenta que los datos que se introducen deben estar en formato string 
         Python variable='XX'
         Robotframework  ${variable}=    XX
         También a la hora de introducir datos, estso deben estar en forma de lista datos
```

### Comparing `robotframework_creartramas-2.1.7/PKG-INFO` & `robotframework_creartramas-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-creartramas
-Version: 2.1.7
+Version: 2.1.8
 Summary: Creacion de tramas en hexadecimal
 Home-page: https://pypi.org/project/robotframework-creartramas
 License: Apache-2.0
 Author: Anthony Arevalo
 Maintainer: Anthony Arevalo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -48,15 +48,15 @@
     ${direccion_origen}=    01
     ${direccion_destino}=   02
     ${numero_bytes}=         08
     ${comando}=             FE
     @{datos}=               0x41    0x5A    0x4B
     ¡¡DATOS ES UNA LISTA!!
 
-    ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bits}    ${comando}    ${datos}
+    ${trama}=    Crear Trama    ${direccion_origen}    ${direccion_destino}    ${numero_bytes}    ${comando}    @{datos}
     Log    Trama creada: ${trama}
 ```
 
 ## Funciones Disponibles
 
 `calcular_checksum(trama)`
```

