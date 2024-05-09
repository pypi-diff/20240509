# Comparing `tmp/gamspy_highs-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_highs-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2500392 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      331 b- defN 24-Apr-17 09:01 gamspy_highs/__init__.py
--rw-rw-rw-  2.0 fat  5996544 b- defN 24-Apr-17 09:01 gamspy_highs/hiscclib64.dll
--rw-rw-rw-  2.0 fat    10138 b- defN 24-Apr-17 09:01 gamspy_highs/opthighs.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_highs/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 09:01 gamspy_highs-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_highs-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 09:01 gamspy_highs-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      649 b- defN 24-Apr-17 09:01 gamspy_highs-46.4.1.dist-info/RECORD
-8 files, 6007863 bytes uncompressed, 2499260 bytes compressed:  58.4%
+Zip file size: 2500394 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      331 b- defN 24-May-09 12:15 gamspy_highs/__init__.py
+-rw-rw-rw-  2.0 fat  5996544 b- defN 24-May-09 12:15 gamspy_highs/hiscclib64.dll
+-rw-rw-rw-  2.0 fat    10138 b- defN 24-May-09 12:15 gamspy_highs/opthighs.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:15 gamspy_highs/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 12:15 gamspy_highs-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:15 gamspy_highs-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-09 12:15 gamspy_highs-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      649 b- defN 24-May-09 12:15 gamspy_highs-46.5.0.dist-info/RECORD
+8 files, 6007863 bytes uncompressed, 2499262 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: gamspy_highs/opthighs.def
 Comment: 
 
 Filename: gamspy_highs/version.py
 Comment: 
 
-Filename: gamspy_highs-46.4.1.dist-info/METADATA
+Filename: gamspy_highs-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_highs-46.4.1.dist-info/WHEEL
+Filename: gamspy_highs-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_highs-46.4.1.dist-info/top_level.txt
+Filename: gamspy_highs-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_highs-46.4.1.dist-info/RECORD
+Filename: gamspy_highs-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_highs/hiscclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001804d5da4
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:28:35 2024
+Time/Date		Wed May  8 03:54:07 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000004d7c00
 SizeOfInitializedData	00000000000f2000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000004d5da4
@@ -1334603,16 +1334603,16 @@
    18050085d:	add    %al,(%rax)
    18050085f:	add    %dh,(%rax)
    180500861:	call   *-0x80(%rsi)
    180500864:	add    %eax,(%rax)
    180500866:	add    %al,(%rax)
    180500868:	add    %al,(%rax)
    18050086a:	add    %al,(%rax)
-   18050086c:	mov    $0x36,%bl
-   18050086e:	(bad)
+   18050086c:	pop    %rdi
+   18050086d:	idivl  (%rdx)
    18050086f:	data16 add %al,(%rax)
    180500872:	add    %al,(%rax)
    180500874:	or     $0xd4000000,%eax
    180500879:	add    (%rax),%eax
    18050087b:	add    %dh,-0x54bffb0(%rdx,%rcx,1)
    180500882:	rex.WRXB add %r8b,(%r8)
 	...
```

## gamspy_highs/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

## Comparing `gamspy_highs-46.4.1.dist-info/RECORD` & `gamspy_highs-46.5.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gamspy_highs/__init__.py,sha256=eVeIEB3nQs2iF9P_l8rtty_AqliOjij6I7_OFWZ2zkw,331
-gamspy_highs/hiscclib64.dll,sha256=7XF4cLSZBmvuKIkQXwh2dzRe-FZd03nfXfcc7AXkSc0,5996544
+gamspy_highs/hiscclib64.dll,sha256=3Rd6waoJF1vcUDOfSQ3ZNJVPdTtFgCCGSRLtElwgpNs,5996544
 gamspy_highs/opthighs.def,sha256=uudsCSiN03LcUfNCnwVyF22cCQcAo20XoTy_kv05zPU,10138
-gamspy_highs/version.py,sha256=PfEsnAfLuXVTA7hSNu9m9ueNe8npaTtOAv06fL-xeY4,22
-gamspy_highs-46.4.1.dist-info/METADATA,sha256=8xY3JhIvskBlS2h3bdwW6xjho5utV4dJf-rg7lPdlWY,62
-gamspy_highs-46.4.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_highs-46.4.1.dist-info/top_level.txt,sha256=t-Xx6EkaD4Hc2BEfgzl7oAbnr2-Aot5_4MdAMgoV1xY,13
-gamspy_highs-46.4.1.dist-info/RECORD,,
+gamspy_highs/version.py,sha256=XIdA4Cvl0eCbv31_g7hR2M0oeouzY6KRnEe6VcwZIX4,22
+gamspy_highs-46.5.0.dist-info/METADATA,sha256=FUX_T8ZgyanT_zVLYf6ROQ_E0MEoYGOhkUPFSRyhkE0,62
+gamspy_highs-46.5.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_highs-46.5.0.dist-info/top_level.txt,sha256=t-Xx6EkaD4Hc2BEfgzl7oAbnr2-Aot5_4MdAMgoV1xY,13
+gamspy_highs-46.5.0.dist-info/RECORD,,
```

