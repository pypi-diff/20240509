# Comparing `tmp/gamspy_snopt-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_snopt-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 583366 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-17 09:02 gamspy_snopt/__init__.py
--rw-rw-rw-  2.0 fat     6967 b- defN 24-Apr-17 09:02 gamspy_snopt/optsnopt.def
--rw-rw-rw-  2.0 fat  1416704 b- defN 24-Apr-17 09:02 gamspy_snopt/snlcclib64.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:02 gamspy_snopt/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 09:02 gamspy_snopt-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:02 gamspy_snopt-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 09:02 gamspy_snopt-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      648 b- defN 24-Apr-17 09:02 gamspy_snopt-46.4.1.dist-info/RECORD
-8 files, 1424877 bytes uncompressed, 582234 bytes compressed:  59.1%
+Zip file size: 583368 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      357 b- defN 24-May-09 12:16 gamspy_snopt/__init__.py
+-rw-rw-rw-  2.0 fat     6967 b- defN 24-May-09 12:16 gamspy_snopt/optsnopt.def
+-rw-rw-rw-  2.0 fat  1416704 b- defN 24-May-09 12:16 gamspy_snopt/snlcclib64.dll
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:16 gamspy_snopt/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 12:16 gamspy_snopt-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:16 gamspy_snopt-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-09 12:16 gamspy_snopt-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      648 b- defN 24-May-09 12:16 gamspy_snopt-46.5.0.dist-info/RECORD
+8 files, 1424877 bytes uncompressed, 582236 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gamspy_snopt/snlcclib64.dll
 Comment: 
 
 Filename: gamspy_snopt/version.py
 Comment: 
 
-Filename: gamspy_snopt-46.4.1.dist-info/METADATA
+Filename: gamspy_snopt-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_snopt-46.4.1.dist-info/WHEEL
+Filename: gamspy_snopt-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_snopt-46.4.1.dist-info/top_level.txt
+Filename: gamspy_snopt-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_snopt-46.4.1.dist-info/RECORD
+Filename: gamspy_snopt-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_snopt/snlcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018012a1c0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:36:42 2024
+Time/Date		Wed May  8 04:01:22 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000012ba00
 SizeOfInitializedData	000000000003ba00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000012a1c0
@@ -282694,19 +282694,18 @@
    18013c53e:	add    %al,(%rax)
    18013c540:	xor    %al,0x18016(%rip)        # 0x18015455c
    18013c546:	add    %al,(%rax)
    18013c548:	rolb   $1,0x18016(%rip)        # 0x180154564
    18013c54e:	add    %al,(%rax)
    18013c550:	add    %al,(%rax)
    18013c552:	add    %al,(%rax)
-   18013c554:	(bad)
-   18013c555:	cmp    %bl,(%rsi)
-   18013c557:	data16 add %al,(%rax)
-   18013c55a:	add    %al,(%rax)
-   18013c55c:	or     $0x64000000,%eax
+   18013c554:	adc    %cl,%bh
+   18013c556:	cmp    0x0(%rsi),%ah
+   18013c559:	add    %al,(%rax)
+   18013c55b:	add    %cl,0x64000000(%rip)        # 0x1e413c561
    18013c561:	add    (%rax),%al
    18013c563:	add    %bl,(%rax)
    18013c565:	(bad)
    18013c566:	adc    (%rax),%eax
    18013c568:	sbb    %dh,0x13(%rbp)
    18013c56e:	add    %al,(%rax)
    18013c570:	cmp    %al,(%rcx)
```

## gamspy_snopt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

