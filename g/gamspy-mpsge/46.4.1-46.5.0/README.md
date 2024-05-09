# Comparing `tmp/gamspy_mpsge-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_mpsge-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 500400 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      357 b- defN 24-Apr-17 09:01 gamspy_mpsge/__init__.py
--rw-rw-rw-  2.0 fat      378 b- defN 24-Apr-17 09:01 gamspy_mpsge/gmsge_nt.cmd
--rw-rw-rw-  2.0 fat   240640 b- defN 24-Apr-17 09:01 gamspy_mpsge/gmsge_nx.exe
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 09:01 gamspy_mpsge/gmsgewnt.cmd
--rw-rw-rw-  2.0 fat   697344 b- defN 24-Apr-17 09:01 gamspy_mpsge/gmsgewnx.exe
--rw-rw-rw-  2.0 fat     1796 b- defN 24-Apr-17 09:01 gamspy_mpsge/mpsgeset
--rw-rw-rw-  2.0 fat   332800 b- defN 24-Apr-17 09:01 gamspy_mpsge/mpsgeval.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_mpsge/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 09:01 gamspy_mpsge-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_mpsge-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 09:01 gamspy_mpsge-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      970 b- defN 24-Apr-17 09:01 gamspy_mpsge-46.4.1.dist-info/RECORD
-12 files, 1274578 bytes uncompressed, 498776 bytes compressed:  60.9%
+Zip file size: 500404 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      357 b- defN 24-May-09 12:16 gamspy_mpsge/__init__.py
+-rw-rw-rw-  2.0 fat      378 b- defN 24-May-09 12:16 gamspy_mpsge/gmsge_nt.cmd
+-rw-rw-rw-  2.0 fat   240640 b- defN 24-May-09 12:16 gamspy_mpsge/gmsge_nx.exe
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 12:16 gamspy_mpsge/gmsgewnt.cmd
+-rw-rw-rw-  2.0 fat   697344 b- defN 24-May-09 12:16 gamspy_mpsge/gmsgewnx.exe
+-rw-rw-rw-  2.0 fat     1796 b- defN 24-May-09 12:16 gamspy_mpsge/mpsgeset
+-rw-rw-rw-  2.0 fat   332800 b- defN 24-May-09 12:16 gamspy_mpsge/mpsgeval.dll
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:16 gamspy_mpsge/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 12:16 gamspy_mpsge-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:16 gamspy_mpsge-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-09 12:16 gamspy_mpsge-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      970 b- defN 24-May-09 12:16 gamspy_mpsge-46.5.0.dist-info/RECORD
+12 files, 1274578 bytes uncompressed, 498780 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: gamspy_mpsge/mpsgeval.dll
 Comment: 
 
 Filename: gamspy_mpsge/version.py
 Comment: 
 
-Filename: gamspy_mpsge-46.4.1.dist-info/METADATA
+Filename: gamspy_mpsge-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_mpsge-46.4.1.dist-info/WHEEL
+Filename: gamspy_mpsge-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_mpsge-46.4.1.dist-info/top_level.txt
+Filename: gamspy_mpsge-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_mpsge-46.4.1.dist-info/RECORD
+Filename: gamspy_mpsge-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_mpsge/gmsge_nx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014002e150
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 16 08:29:02 2024
+Time/Date		Wed May  8 03:54:30 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000002f800
 SizeOfInitializedData	0000000000042600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000002e150
@@ -57160,19 +57160,18 @@
    140035976:	add    %al,(%rax)
    140035978:	adc    %dh,%dl
    14003597a:	add    $0x40,%al
    14003597c:	add    %eax,(%rax)
    14003597e:	add    %al,(%rax)
    140035980:	add    %al,(%rax)
    140035982:	add    %al,(%rax)
-   140035984:	(bad)
-   140035985:	ss (bad)
-   140035987:	data16 add %al,(%rax)
-   14003598a:	add    %al,(%rax)
-   14003598c:	or     $0x90000000,%eax
+   140035984:	jbe    0x14003597d
+   140035986:	cmp    0x0(%rsi),%ah
+   140035989:	add    %al,(%rax)
+   14003598b:	add    %cl,-0x70000000(%rip)        # 0xd0035991
    140035991:	add    (%rax),%al
    140035993:	add    %bl,(%rax)
    140035995:	pop    %rbx
    140035996:	add    (%rax),%eax
    140035998:	sbb    %al,0x3(%rdi)
    14003599b:	add    %al,(%rax)
    14003599d:	add    %al,(%rax)
```

## gamspy_mpsge/gmsgewnx.exe

### objdump

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014008c800
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Tue Apr 16 08:29:03 2024
+Time/Date		Wed May  8 03:54:31 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000008de00
 SizeOfInitializedData	0000000000579a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000008c800
@@ -162842,19 +162842,18 @@
    14009ee55:	add    %al,(%rax)
    14009ee57:	add    %dl,(%rax)
    14009ee59:	(bad)
    14009ee5c:	add    %eax,(%rax)
    14009ee5e:	add    %al,(%rax)
    14009ee60:	add    %al,(%rax)
    14009ee62:	add    %al,(%rax)
-   14009ee64:	iret
-   14009ee65:	ss (bad)
-   14009ee67:	data16 add %al,(%rax)
-   14009ee6a:	add    %al,(%rax)
-   14009ee6c:	or     $0x90000000,%eax
+   14009ee64:	ja     0x14009ee5d
+   14009ee66:	cmp    0x0(%rsi),%ah
+   14009ee69:	add    %al,(%rax)
+   14009ee6b:	add    %cl,-0x70000000(%rip)        # 0xd009ee71
    14009ee71:	add    (%rax),%al
    14009ee73:	add    %bl,(%rax)
    14009ee75:	lock or %eax,(%rax)
    14009ee78:	sbb    %ah,%dl
    14009ee7a:	or     %eax,(%rax)
    14009ee7c:	add    %al,(%rax)
    14009ee7e:	add    %al,(%rax)
```

## gamspy_mpsge/mpsgeval.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180043970
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:29:01 2024
+Time/Date		Wed May  8 03:54:29 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000045000
 SizeOfInitializedData	0000000000567c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000043970
@@ -73827,19 +73827,18 @@
    18004a075:	add    %al,(%rax)
    18004a077:	add    %al,0x40(%rax)
    18004a07a:	or     0x1(%rax),%eax
    18004a080:	loopne 0x18004a0c2
    18004a082:	or     0x1(%rax),%eax
    18004a088:	add    %al,(%rax)
    18004a08a:	add    %al,(%rax)
-   18004a08c:	int    $0x36
-   18004a08e:	(bad)
-   18004a08f:	data16 add %al,(%rax)
-   18004a092:	add    %al,(%rax)
-   18004a094:	or     $0x64000000,%eax
+   18004a08c:	jne    0x18004a085
+   18004a08e:	cmp    0x0(%rsi),%ah
+   18004a091:	add    %al,(%rax)
+   18004a093:	add    %cl,0x64000000(%rip)        # 0x1e404a099
    18004a099:	add    (%rax),%al
    18004a09b:	add    %bl,(%rax)
    18004a09d:	movabs %al,0x496180004
 	...
    18004a0ae:	add    %al,(%rax)
    18004a0b0:	cmp    %al,(%rcx)
 	...
```

## gamspy_mpsge/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

## Comparing `gamspy_mpsge-46.4.1.dist-info/RECORD` & `gamspy_mpsge-46.5.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 gamspy_mpsge/__init__.py,sha256=MlMkBzJyMRjzxLFVdsTyKx68R9CJSa-1KucyBCBQpUA,357
 gamspy_mpsge/gmsge_nt.cmd,sha256=uprNlh9Lm49P9SObn6ns2G_nUr6lysAftH0wzeMFSnk,378
-gamspy_mpsge/gmsge_nx.exe,sha256=PUEnINeEXs8zIYOGjoRRl8yXCYn9uwhDGiaXcvBt-t0,240640
+gamspy_mpsge/gmsge_nx.exe,sha256=ec-2Jn_q9QgyAOvwkPVJgE1dWDovFalavAy82ZiBEIw,240640
 gamspy_mpsge/gmsgewnt.cmd,sha256=7LZupf8lkuUadAus2veYXY-aD590v4HWLjrW9TxlpI8,92
-gamspy_mpsge/gmsgewnx.exe,sha256=nhlU2cYXC6p9D8yHUv6ZkXo_ALAyEDxP5REvjL6Bvik,697344
+gamspy_mpsge/gmsgewnx.exe,sha256=FCp42o8215TajwVZDMhRW18HW4RqM-7j3XewayImL1w,697344
 gamspy_mpsge/mpsgeset,sha256=9SnB6TxKDHB_K51yXMYRrLAmlDHBm_XlcaRoKs4F4hM,1796
-gamspy_mpsge/mpsgeval.dll,sha256=9Z4ZpxHziR-ZB6SWFDKWppfRsb_Y8aGhjI_68GHCQJ0,332800
-gamspy_mpsge/version.py,sha256=PfEsnAfLuXVTA7hSNu9m9ueNe8npaTtOAv06fL-xeY4,22
-gamspy_mpsge-46.4.1.dist-info/METADATA,sha256=cDHl_cJrHCLZjoA_cuKopbttzarr7TB_RR_msmr1bdc,62
-gamspy_mpsge-46.4.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_mpsge-46.4.1.dist-info/top_level.txt,sha256=fFGHc0aIUS4As3C1AF49tM5L1gNFfszi8rB1B55EbeE,13
-gamspy_mpsge-46.4.1.dist-info/RECORD,,
+gamspy_mpsge/mpsgeval.dll,sha256=U6kzLCoQJwOubZXod5hYLewFXamVdbZ6tX_J_SUuQZo,332800
+gamspy_mpsge/version.py,sha256=XIdA4Cvl0eCbv31_g7hR2M0oeouzY6KRnEe6VcwZIX4,22
+gamspy_mpsge-46.5.0.dist-info/METADATA,sha256=fu42OJuPXOE-n-40mQb0SHHsvmfiVokBO4lKqcoOUHU,62
+gamspy_mpsge-46.5.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_mpsge-46.5.0.dist-info/top_level.txt,sha256=fFGHc0aIUS4As3C1AF49tM5L1gNFfszi8rB1B55EbeE,13
+gamspy_mpsge-46.5.0.dist-info/RECORD,,
```

