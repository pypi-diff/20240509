# Comparing `tmp/encryptedcode-1.1.1.tar.gz` & `tmp/encryptedcode-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encryptedcode-1.1.1.tar", last modified: Fri Apr 12 17:16:33 2024, max compression
+gzip compressed data, was "encryptedcode-1.1.2.tar", last modified: Thu May  9 01:19:44 2024, max compression
```

## Comparing `encryptedcode-1.1.1.tar` & `encryptedcode-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 17:16:33.617445 encryptedcode-1.1.1/
--rw-rw-rw-   0        0        0     1307 2024-04-12 17:16:33.616447 encryptedcode-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      892 2024-04-12 17:12:31.000000 encryptedcode-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 17:16:33.580390 encryptedcode-1.1.1/encryptedcode/
--rw-rw-rw-   0        0        0        0 2023-12-02 21:44:29.000000 encryptedcode-1.1.1/encryptedcode/__init__.py
--rw-rw-rw-   0        0        0     2367 2024-04-12 17:14:41.000000 encryptedcode-1.1.1/encryptedcode/base.py
--rw-rw-rw-   0        0        0     4606 2024-04-12 16:37:24.000000 encryptedcode-1.1.1/encryptedcode/encrypted_code.py
-drwxrwxrwx   0        0        0        0 2024-04-12 17:16:33.613451 encryptedcode-1.1.1/encryptedcode.egg-info/
--rw-rw-rw-   0        0        0     1307 2024-04-12 17:16:33.000000 encryptedcode-1.1.1/encryptedcode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-04-12 17:16:33.000000 encryptedcode-1.1.1/encryptedcode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 17:16:33.000000 encryptedcode-1.1.1/encryptedcode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-12 17:16:33.000000 encryptedcode-1.1.1/encryptedcode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 17:16:33.623740 encryptedcode-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      691 2024-04-12 17:16:29.000000 encryptedcode-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:19:44.807746 encryptedcode-1.1.2/
+-rw-rw-rw-   0        0        0     1198 2024-05-09 01:19:44.805745 encryptedcode-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-05-09 01:10:48.000000 encryptedcode-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 01:19:44.681049 encryptedcode-1.1.2/encryptedcode/
+-rw-rw-rw-   0        0        0     1927 2024-05-09 00:55:34.000000 encryptedcode-1.1.2/encryptedcode/encrypted_code.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:19:44.796905 encryptedcode-1.1.2/encryptedcode.egg-info/
+-rw-rw-rw-   0        0        0     1198 2024-05-09 01:19:44.000000 encryptedcode-1.1.2/encryptedcode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2024-05-09 01:19:44.000000 encryptedcode-1.1.2/encryptedcode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 01:19:44.000000 encryptedcode-1.1.2/encryptedcode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 01:19:44.000000 encryptedcode-1.1.2/encryptedcode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 01:19:44.864466 encryptedcode-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-09 01:19:11.000000 encryptedcode-1.1.2/setup.py
```

### Comparing `encryptedcode-1.1.1/README.md` & `encryptedcode-1.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,47 @@
 00000000: 3c68 313e 456e 6372 7970 7465 6420 436f  <h1>Encrypted Co
 00000010: 6465 202d 204c 3031 3233 2041 6c67 6f72  de - L0123 Algor
-00000020: 6974 686d 3c2f 6831 3e0d 0a0d 0a5b 2149  ithm</h1>....[!I
-00000030: 4e53 5441 4c4c 4154 494f 4e5d 0d0a 2020  NSTALLATION]..  
-00000040: 2020 7069 7020 696e 7374 616c 6c20 656e    pip install en
-00000050: 6372 7970 7465 6463 6f64 650d 0a0d 0a5b  cryptedcode....[
-00000060: 2155 5341 4745 5d0d 0a54 6869 7320 7061  !USAGE]..This pa
-00000070: 636b 6167 6520 6973 2069 6d70 6f72 7465  ckage is importe
-00000080: 6420 6162 736f 6c75 7465 6c79 2069 6e20  d absolutely in 
-00000090: 796f 7572 202e 7079 2066 696c 6573 2c20  your .py files, 
-000000a0: 666f 7220 6578 616d 706c 653a 2027 6672  for example: 'fr
-000000b0: 6f6d 2065 6e63 7279 7074 6564 636f 6465  om encryptedcode
-000000c0: 2e65 6e63 7279 7074 6564 5f63 6f64 6520  .encrypted_code 
-000000d0: 696d 706f 7274 2065 6e63 6f64 6527 2c20  import encode', 
-000000e0: 616e 6420 636f 6e74 6169 6e73 2074 776f  and contains two
-000000f0: 2066 756e 6374 696f 6e73 2c20 6f6e 6520   functions, one 
-00000100: 666f 7220 656e 636f 6469 6e67 2063 616c  for encoding cal
-00000110: 6c65 6420 656e 636f 6465 2829 2061 6e64  led encode() and
-00000120: 2061 6e6f 7468 6572 2066 6f72 2064 6563   another for dec
-00000130: 6f64 696e 6720 6361 6c6c 6564 2064 6563  oding called dec
-00000140: 6f64 6528 2920 7573 696e 6720 7468 6520  ode() using the 
-00000150: 6e65 7720 4c30 3132 3320 616c 676f 7269  new L0123 algori
-00000160: 7468 6d20 6372 6561 7465 6420 6279 2049  thm created by I
-00000170: 6e67 2053 6f66 7477 6172 6520 4c65 616e  ng Software Lean
-00000180: 6472 6f20 476f 6e7a 616c 657a 2045 7370  dro Gonzalez Esp
-00000190: 696e 6f73 610d 0a0d 0a5b 2149 4d50 4f52  inosa....[!IMPOR
-000001a0: 5441 4e54 5d0d 0a20 2020 2041 6c20 7573  TANT]..    Al us
-000001b0: 6172 2070 6f72 2070 7269 6d65 7261 2076  ar por primera v
-000001c0: 657a 2065 7374 6120 6c69 6272 6572 6961  ez esta libreria
-000001d0: 2065 6e20 7475 2070 6320 6f20 656e 746f   en tu pc o ento
-000001e0: 726e 6f20 7669 7274 7561 6c20 7465 2070  rno virtual te p
-000001f0: 6564 6972 c3a1 2071 7565 2070 726f 706f  edir.. que propo
-00000200: 7263 696f 6e65 7320 756e 6120 6672 6173  rciones una fras
-00000210: 6520 7365 6372 6574 610d 0a20 2020 2065  e secreta..    e
-00000220: 7374 6120 6672 6173 6520 6465 6265 7320  sta frase debes 
-00000230: 7265 636f 7264 6172 6c61 206f 2067 7561  recordarla o gua
-00000240: 7264 6172 6c61 2079 6120 7175 6520 7061  rdarla ya que pa
-00000250: 7261 2070 6f64 6572 2075 7469 6c69 7a61  ra poder utiliza
-00000260: 7220 6c61 2066 756e 6369 6f6e 2064 6520  r la funcion de 
-00000270: 6465 636f 6465 206e 6563 6573 6974 6172  decode necesitar
-00000280: 6173 206c 6120 6672 6173 650d 0a20 2020  as la frase..   
-00000290: 2070 6f72 2063 7565 7374 696f 6e65 7320   por cuestiones 
-000002a0: 6465 2073 6567 7572 6964 6164 2070 6172  de seguridad par
-000002b0: 6120 7573 7465 6421 2121 0d0a 0d0a 5b21  a usted!!!....[!
-000002c0: 494e 464f 5d0d 0a45 6e63 7279 7074 6564  INFO]..Encrypted
-000002d0: 436f 6465 2069 7320 6120 7079 7468 6f6e  Code is a python
-000002e0: 206c 6962 7261 7279 2061 6363 6573 7369   library accessi
-000002f0: 626c 6520 746f 2065 7665 7279 6f6e 6520  ble to everyone 
-00000300: 7468 6174 2069 7320 756e 6465 7220 6465  that is under de
-00000310: 7665 6c6f 706d 656e 7420 7768 6572 6520  velopment where 
-00000320: 4920 7573 6520 6120 6e65 7720 656e 6372  I use a new encr
-00000330: 7970 7469 6f6e 2061 6c67 6f72 6974 686d  yption algorithm
-00000340: 2063 7265 6174 6564 2062 7920 2663 6f70   created by &cop
-00000350: 793b 4c65 616e 6472 6f20 476f 6e7a 616c  y;Leandro Gonzal
-00000360: 657a 2045 7370 696e 6f73 6120 616e 6420  ez Espinosa and 
-00000370: 6e61 6d65 6420 4c30 3132 332e            named L0123.
+00000020: 6974 686d 3c2f 6831 3e0d 0a0d 0a3e 205b  ithm</h1>....> [
+00000030: 2149 4e46 4f5d 0d0a 456e 6372 7970 7465  !INFO]..Encrypte
+00000040: 6443 6f64 6520 6973 2061 2070 7974 686f  dCode is a pytho
+00000050: 6e20 6c69 6272 6172 7920 6163 6365 7373  n library access
+00000060: 6962 6c65 2074 6f20 6576 6572 796f 6e65  ible to everyone
+00000070: 2074 6861 7420 6973 2075 6e64 6572 2064   that is under d
+00000080: 6576 656c 6f70 6d65 6e74 2077 6865 7265  evelopment where
+00000090: 2049 2075 7365 2061 206e 6577 2065 6e63   I use a new enc
+000000a0: 7279 7074 696f 6e20 616c 676f 7269 7468  ryption algorith
+000000b0: 6d20 6372 6561 7465 6420 6279 2026 636f  m created by &co
+000000c0: 7079 3b20 536f 6674 7761 7265 2045 6e67  py; Software Eng
+000000d0: 696e 6565 7220 3c61 2068 7265 663d 2268  ineer <a href="h
+000000e0: 7474 7073 3a2f 2f6c 656f 676c 657a 2e76  ttps://leoglez.v
+000000f0: 6572 6365 6c2e 6170 702f 223e 4c65 616e  ercel.app/">Lean
+00000100: 6472 6f20 476f 6e7a 616c 657a 2045 7370  dro Gonzalez Esp
+00000110: 696e 6f73 612e 3c2f 613e 2061 6e64 206e  inosa.</a> and n
+00000120: 616d 6564 204c 3031 3233 2e0d 0a0d 0a3e  amed L0123.....>
+00000130: 205b 2149 4d50 4f52 5441 4e54 5d0d 0a70   [!IMPORTANT]..p
+00000140: 6970 2069 6e73 7461 6c6c 2065 6e63 7279  ip install encry
+00000150: 7074 6564 636f 6465 0d0a 0d0a 0d0a 2323  ptedcode......##
+00000160: 2320 5553 4147 450d 0a54 6869 7320 7061  # USAGE..This pa
+00000170: 636b 6167 6520 6973 2069 6d70 6f72 7465  ckage is importe
+00000180: 6420 6162 736f 6c75 7465 6c79 2069 6e20  d absolutely in 
+00000190: 796f 7572 202e 7079 2066 696c 6573 2c20  your .py files, 
+000001a0: 666f 7220 6578 616d 706c 653a 2027 6672  for example: 'fr
+000001b0: 6f6d 2065 6e63 7279 7074 6564 636f 6465  om encryptedcode
+000001c0: 2e65 6e63 7279 7074 6564 5f63 6f64 6520  .encrypted_code 
+000001d0: 696d 706f 7274 2065 6e63 6f64 6527 2c20  import encode', 
+000001e0: 616e 6420 636f 6e74 6169 6e73 2074 776f  and contains two
+000001f0: 2066 756e 6374 696f 6e73 2c20 6f6e 6520   functions, one 
+00000200: 666f 7220 656e 636f 6469 6e67 2063 616c  for encoding cal
+00000210: 6c65 6420 656e 636f 6465 2829 2061 6e64  led encode() and
+00000220: 2061 6e6f 7468 6572 2066 6f72 2064 6563   another for dec
+00000230: 6f64 696e 6720 6361 6c6c 6564 2064 6563  oding called dec
+00000240: 6f64 6528 2920 7573 696e 6720 7468 6520  ode() using the 
+00000250: 6e65 7720 4c30 3132 3320 616c 676f 7269  new L0123 algori
+00000260: 7468 6d2e 2041 2073 696d 706c 6520 6578  thm. A simple ex
+00000270: 616d 706c 6520 6f66 2068 6f77 2074 6f20  ample of how to 
+00000280: 7573 6520 7468 6520 6c69 6272 6172 7920  use the library 
+00000290: 6973 2074 6865 2066 6f6c 6c6f 7769 6e67  is the following
+000002a0: 3a0d 0a0d 0a3c 696d 6720 7372 633d 2273  :....<img src="s
+000002b0: 7263 2f75 7361 6765 2e70 6e67 2220 7374  rc/usage.png" st
+000002c0: 796c 653d 2261 7370 6563 742d 7261 7469  yle="aspect-rati
+000002d0: 6f3a 3136 2f31 3022 3e3c 2f69 6d67 3e0d  o:16/10"></img>.
+000002e0: 0a                                       .
```

### Comparing `encryptedcode-1.1.1/setup.py` & `encryptedcode-1.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 readme = open("./README.md", "r")
 setup(
     name="encryptedcode",
     python_version="3.12.0",
-    version="1.1.1",
+    version="1.1.2",
     description="This library can be used to encrypt and decrypt passwords using the new L0123 algorithm.",
     long_description=readme.read(),
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Leandro Gonzalez Espinosa",
     author_email="lworkgonzalez01@gmail.com",
     packages=["encryptedcode"],
-    keywords=["encryptation", "encrypted","encode", "decode", "algorithm"],
-    url="https://github.com/leoGlez01/password_encode.git",
+    keywords=["encryptation", "encrypted","encode", "decode", "algorithm", "Leandro Gonzalez Espinosa", "Leandro Gonzalez", "Leo Dev"],
+    url="https://github.com/leoGlez01/encrypted-code.git",
     license="MIT",
     include_package_data=True,
 )
```

