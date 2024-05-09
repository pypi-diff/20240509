# Comparing `tmp/gamspy_minos-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_minos-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 405788 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-17 09:01 gamspy_minos/__init__.py
--rw-rw-rw-  2.0 fat   973312 b- defN 24-Apr-17 09:01 gamspy_minos/milcclib64.dll
--rw-rw-rw-  2.0 fat     5745 b- defN 24-Apr-17 09:01 gamspy_minos/optminos.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_minos/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 09:01 gamspy_minos-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_minos-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 09:01 gamspy_minos-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      647 b- defN 24-Apr-17 09:01 gamspy_minos-46.4.1.dist-info/RECORD
-8 files, 980262 bytes uncompressed, 404656 bytes compressed:  58.7%
+Zip file size: 405790 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      357 b- defN 24-May-09 12:16 gamspy_minos/__init__.py
+-rw-rw-rw-  2.0 fat   973312 b- defN 24-May-09 12:16 gamspy_minos/milcclib64.dll
+-rw-rw-rw-  2.0 fat     5745 b- defN 24-May-09 12:16 gamspy_minos/optminos.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:16 gamspy_minos/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 12:16 gamspy_minos-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:16 gamspy_minos-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-09 12:16 gamspy_minos-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      647 b- defN 24-May-09 12:16 gamspy_minos-46.5.0.dist-info/RECORD
+8 files, 980262 bytes uncompressed, 404658 bytes compressed:  58.7%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gamspy_minos/optminos.def
 Comment: 
 
 Filename: gamspy_minos/version.py
 Comment: 
 
-Filename: gamspy_minos-46.4.1.dist-info/METADATA
+Filename: gamspy_minos-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_minos-46.4.1.dist-info/WHEEL
+Filename: gamspy_minos-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_minos-46.4.1.dist-info/top_level.txt
+Filename: gamspy_minos-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_minos-46.4.1.dist-info/RECORD
+Filename: gamspy_minos-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_minos/milcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800cb0e4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:28:49 2024
+Time/Date		Wed May  8 03:54:18 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000000cc800
 SizeOfInitializedData	0000000000024e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000cb0e4
@@ -202410,18 +202410,18 @@
    1800d9d46:	add    %al,(%rax)
    1800d9d48:	rol    $1,%al
    1800d9d4a:	(bad)
    1800d9d4b:	addb   $0x0,(%rcx)
    1800d9d4e:	add    %al,(%rax)
    1800d9d50:	add    %al,(%rax)
    1800d9d52:	add    %al,(%rax)
-   1800d9d54:	shll   $0x1e,(%rsi)
-   1800d9d57:	data16 add %al,(%rax)
-   1800d9d5a:	add    %al,(%rax)
-   1800d9d5c:	or     $0x64000000,%eax
+   1800d9d54:	push   $0xfffffffffffffff7
+   1800d9d56:	cmp    0x0(%rsi),%ah
+   1800d9d59:	add    %al,(%rax)
+   1800d9d5b:	add    %cl,0x64000000(%rip)        # 0x1e40d9d61
    1800d9d61:	add    (%rax),%al
    1800d9d63:	add    %bl,(%rax)
    1800d9d65:	lahf
    1800d9d66:	or     $0xd8b1800,%eax
    1800d9d6b:	add    %al,(%rax)
    1800d9d6d:	add    %al,(%rax)
    1800d9d6f:	add    %bh,(%rax)
```

## gamspy_minos/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

