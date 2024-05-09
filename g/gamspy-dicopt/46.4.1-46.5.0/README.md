# Comparing `tmp/gamspy_dicopt-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_dicopt-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 199564 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      322 b- defN 24-Apr-17 09:01 gamspy_dicopt/__init__.py
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 09:01 gamspy_dicopt/gmsdi_nt.cmd
--rw-rw-rw-  2.0 fat   544768 b- defN 24-Apr-17 09:01 gamspy_dicopt/gmsdi_nx.exe
--rw-rw-rw-  2.0 fat     4787 b- defN 24-Apr-17 09:01 gamspy_dicopt/optdicopt.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_dicopt/version.py
--rw-rw-rw-  2.0 fat       63 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      735 b- defN 24-Apr-17 09:01 gamspy_dicopt-46.4.1.dist-info/RECORD
-9 files, 550907 bytes uncompressed, 198290 bytes compressed:  64.0%
+Zip file size: 199565 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      322 b- defN 24-May-09 12:15 gamspy_dicopt/__init__.py
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 12:15 gamspy_dicopt/gmsdi_nt.cmd
+-rw-rw-rw-  2.0 fat   544768 b- defN 24-May-09 12:15 gamspy_dicopt/gmsdi_nx.exe
+-rw-rw-rw-  2.0 fat     4787 b- defN 24-May-09 12:15 gamspy_dicopt/optdicopt.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:15 gamspy_dicopt/version.py
+-rw-rw-rw-  2.0 fat       63 b- defN 24-May-09 12:15 gamspy_dicopt-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:15 gamspy_dicopt-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-May-09 12:15 gamspy_dicopt-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      735 b- defN 24-May-09 12:15 gamspy_dicopt-46.5.0.dist-info/RECORD
+9 files, 550907 bytes uncompressed, 198291 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gamspy_dicopt/optdicopt.def
 Comment: 
 
 Filename: gamspy_dicopt/version.py
 Comment: 
 
-Filename: gamspy_dicopt-46.4.1.dist-info/METADATA
+Filename: gamspy_dicopt-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_dicopt-46.4.1.dist-info/WHEEL
+Filename: gamspy_dicopt-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_dicopt-46.4.1.dist-info/top_level.txt
+Filename: gamspy_dicopt-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_dicopt-46.4.1.dist-info/RECORD
+Filename: gamspy_dicopt-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_dicopt/gmsdi_nx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x0000000140070640
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 16 08:16:10 2024
+Time/Date		Wed May  8 03:42:24 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000071e00
 SizeOfInitializedData	0000000000017600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000070640
@@ -122747,22 +122747,19 @@
    14007e613:	rex add %eax,(%rax)
    14007e616:	add    %al,(%rax)
    14007e618:	shlb   $0x40,0x8(%rax)
    14007e61c:	add    %eax,(%rax)
    14007e61e:	add    %al,(%rax)
    14007e620:	add    %al,(%rax)
    14007e622:	add    %al,(%rax)
-   14007e624:	lret   $0x1e33
-   14007e627:	data16 add %al,(%rax)
-   14007e62a:	add    %al,(%rax)
-   14007e62c:	or     $0x90000000,%eax
-   14007e631:	add    (%rax),%al
-   14007e633:	add    %bl,-0x67fff819(%rax)
-   14007e639:	flds   (%rdi)
-   14007e63b:	add    %al,(%rax)
+   14007e624:	movabs 0xd00000000663af4,%al
+   14007e62d:	add    %al,(%rax)
+   14007e62f:	add    %dl,-0x67fffffe(%rax)
+   14007e635:	out    %eax,$0x7
+   14007e637:	add    %bl,0x7d9(%rax)
    14007e63d:	add    %al,(%rax)
    14007e63f:	add    %bh,(%rax)
    14007e641:	add    %eax,(%rax)
 	...
    14007e697:	add    %dl,%al
    14007e699:	adc    $0x8,%al
    14007e69b:	rex add %eax,(%rax)
```

## gamspy_dicopt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

