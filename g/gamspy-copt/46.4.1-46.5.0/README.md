# Comparing `tmp/gamspy_copt-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_copt-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8337105 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      383 b- defN 24-Apr-17 09:01 gamspy_copt/__init__.py
--rw-rw-rw-  2.0 fat 19559424 b- defN 24-Apr-17 09:01 gamspy_copt/copt.dll
--rw-rw-rw-  2.0 fat   459776 b- defN 24-Apr-17 09:01 gamspy_copt/cptcclib64.dll
--rw-rw-rw-  2.0 fat  5458432 b- defN 24-Apr-17 09:01 gamspy_copt/libcrypto-3-x64.dll
--rw-rw-rw-  2.0 fat     8873 b- defN 24-Apr-17 09:01 gamspy_copt/optcopt.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_copt/version.py
--rw-rw-rw-  2.0 fat       61 b- defN 24-Apr-17 09:01 gamspy_copt-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_copt-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 24-Apr-17 09:01 gamspy_copt-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      810 b- defN 24-Apr-17 09:01 gamspy_copt-46.4.1.dist-info/RECORD
-10 files, 25487897 bytes uncompressed, 8335737 bytes compressed:  67.3%
+Zip file size: 8337108 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      383 b- defN 24-May-09 12:15 gamspy_copt/__init__.py
+-rw-rw-rw-  2.0 fat 19559424 b- defN 24-May-09 12:15 gamspy_copt/copt.dll
+-rw-rw-rw-  2.0 fat   459776 b- defN 24-May-09 12:15 gamspy_copt/cptcclib64.dll
+-rw-rw-rw-  2.0 fat  5458432 b- defN 24-May-09 12:15 gamspy_copt/libcrypto-3-x64.dll
+-rw-rw-rw-  2.0 fat     8873 b- defN 24-May-09 12:15 gamspy_copt/optcopt.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:15 gamspy_copt/version.py
+-rw-rw-rw-  2.0 fat       61 b- defN 24-May-09 12:15 gamspy_copt-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:15 gamspy_copt-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-09 12:15 gamspy_copt-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      810 b- defN 24-May-09 12:15 gamspy_copt-46.5.0.dist-info/RECORD
+10 files, 25487897 bytes uncompressed, 8335740 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: gamspy_copt/optcopt.def
 Comment: 
 
 Filename: gamspy_copt/version.py
 Comment: 
 
-Filename: gamspy_copt-46.4.1.dist-info/METADATA
+Filename: gamspy_copt-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_copt-46.4.1.dist-info/WHEEL
+Filename: gamspy_copt-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_copt-46.4.1.dist-info/top_level.txt
+Filename: gamspy_copt-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_copt-46.4.1.dist-info/RECORD
+Filename: gamspy_copt-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_copt/cptcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018005f6e0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:40:21 2024
+Time/Date		Wed May  8 04:04:46 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000060400
 SizeOfInitializedData	0000000000012a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000005f6e0
@@ -99408,19 +99408,19 @@
    18006bc67:	add    %ch,0x72(%rcx)
    18006bc6a:	movsxd 0x6d(%rdi),%ebx
    18006bc6d:	jae    0x18006bcd6
    18006bc6f:	cs fs insb (%dx),%es:(%rdi)
    18006bc72:	insb   (%dx),%es:(%rdi)
    18006bc73:	add    %al,(%rax)
    18006bc75:	add    %al,(%rax)
-   18006bc77:	add    %dh,0x39(%rbp)
-   18006bc7a:	(bad)
-   18006bc7b:	data16 add %al,(%rax)
-   18006bc7e:	add    %al,(%rax)
-   18006bc80:	or     $0x64000000,%eax
+   18006bc77:	add    %bl,%dh
+   18006bc79:	stc
+   18006bc7a:	cmp    0x0(%rsi),%ah
+   18006bc7d:	add    %al,(%rax)
+   18006bc7f:	add    %cl,0x64000000(%rip)        # 0x1e406bc85
    18006bc85:	add    (%rax),%al
    18006bc87:	add    %bl,(%rax)
    18006bc89:	mov    $0xa6180006,%esi
    18006bc8e:	(bad)
    18006bc8f:	add    %bh,(%rax)
    18006bc91:	add    %eax,(%rax)
 	...
```

## gamspy_copt/libcrypto-3-x64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180001253
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:33:59 2024
+Time/Date		Wed May  8 03:58:47 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000003df000
 SizeOfInitializedData	0000000000158a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000001253
@@ -96088,15 +96088,15 @@
 	reloc    4 offset   40 [52d040] DIR64
 	reloc    5 offset    0 [52d000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1804b45d4
 
 Type                Size     Rva      Offset
   2        CodeView 0000005c 004b729c 004b669c
-(format RSDS signature a6d40b1610b24b5e9c15a376f56005b7 age 1 pdb C:\home\distrib\porting\btree\openssl\wei\build\libcrypto-3-x64.pdb)
+(format RSDS signature b7f92947b35c4246bc49213553a012df age 1 pdb C:\home\distrib\porting\btree\openssl\wei\build\libcrypto-3-x64.pdb)
  12         Feature 00000014 004b72f8 004b66f8
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000010, Value: 0x80000018
 018    Name Table: Char: 0, Time: 00000000, Ver: 0/0, Num Names: 0, IDs: 1
 028     Entry: ID: 0x000001, Value: 0x80000030
@@ -1868367,24 +1868367,24 @@
    180441daf:	add    %dh,(%rbx)
    180441db1:	cs xor %ch,(%rsi)
    180441db4:	xor    %esi,(%rdx)
    180441db6:	add    %al,(%rax)
    180441db8:	(bad)
    180441dbd:	and    %ch,0x6e(%rdi)
    180441dc0:	cmp    (%rax),%ah
-   180441dc2:	push   %rsp
-   180441dc3:	jne    0x180441e2a
-   180441dc5:	and    %al,0x70(%rcx)
-   180441dc8:	jb     0x180441dea
-   180441dca:	xor    %esi,(%rsi)
+   180441dc2:	push   %rdi
+   180441dc3:	gs and %cl,%fs:0x61(%rbp)
+   180441dc8:	jns    0x180441dea
+   180441dca:	and    %bh,(%rax)
    180441dcc:	and    %dh,(%rax)
-   180441dce:	cmp    %bh,(%rdx)
-   180441dd0:	xor    (%rdx),%esi
-   180441dd2:	cmp    0x30322037(%rip),%dh        # 0x1b0763e0f
-   180441dd8:	xor    (%rax,%riz,1),%dh
+   180441dce:	xor    (%rdx),%edi
+   180441dd0:	xor    $0x38343a37,%eax
+   180441dd5:	and    %dh,(%rdx)
+   180441dd7:	xor    %dh,(%rdx)
+   180441dd9:	xor    $0x20,%al
    180441ddb:	push   %rbp
    180441ddc:	push   %rsp
    180441ddd:	rex.XB add %al,(%r8)
 	...
    180441de8:	jo     0x180441e56
    180441dea:	(bad)
    180441deb:	je     0x180441e53
@@ -2015462,32 +2015462,27 @@
    1804b45bb:	(bad)
    1804b45bc:	(bad)
    1804b45bd:	(bad)
    1804b45be:	(bad)
    1804b45bf:	incl   (%rax)
 	...
    1804b45d5:	add    %al,(%rax)
-   1804b45d7:	add    %dh,%bh
-   1804b45d9:	(bad)
-   1804b45da:	(bad)
-   1804b45db:	data16 add %al,(%rax)
-   1804b45de:	add    %al,(%rax)
-   1804b45e0:	add    (%rax),%al
-   1804b45e2:	add    %al,(%rax)
-   1804b45e4:	pop    %rsp
-   1804b45e5:	add    %al,(%rax)
+   1804b45d7:	add    %dh,-0x8(%rdi)
+   1804b45da:	cmp    0x0(%rsi),%ah
+   1804b45dd:	add    %al,(%rax)
+   1804b45df:	add    %al,(%rdx)
+   1804b45e1:	add    %al,(%rax)
+   1804b45e3:	add    %bl,0x0(%rax,%rax,1)
    1804b45e7:	add    %bl,0x669c004b(%rdx,%rsi,2)
    1804b45ee:	rex.WXB add %al,(%r8)
    1804b45f1:	add    %al,(%rax)
-   1804b45f3:	add    %dh,%bh
-   1804b45f5:	(bad)
-   1804b45f6:	(bad)
-   1804b45f7:	data16 add %al,(%rax)
-   1804b45fa:	add    %al,(%rax)
-   1804b45fc:	or     $0x0,%al
+   1804b45f3:	add    %dh,-0x8(%rdi)
+   1804b45f6:	cmp    0x0(%rsi),%ah
+   1804b45f9:	add    %al,(%rax)
+   1804b45fb:	add    %cl,(%rax,%rax,1)
    1804b45fe:	add    %al,(%rax)
    1804b4600:	adc    $0x0,%al
    1804b4602:	add    %al,(%rax)
    1804b4604:	clc
    1804b4605:	jb     0x1804b4652
    1804b4607:	add    %bh,%al
    1804b4609:	data16 rex.WXB add %al,(%r8)
@@ -2015527,23 +2015522,19 @@
    1804b4742:	push   %rax
    1804b4743:	addb   $0x0,(%rcx)
 	...
    1804b729a:	add    %al,(%rax)
    1804b729c:	push   %rdx
    1804b729d:	push   %rbx
    1804b729e:	rex.R push %rbx
-   1804b72a0:	(bad)
-   1804b72a1:	or     %esp,%edx
-   1804b72a3:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   1804b72a4:	mov    $0x10,%dl
-   1804b72a6:	pop    %rsi
-   1804b72a7:	rex.WXB pushf
-   1804b72a9:	adc    $0x60f576a3,%eax
-   1804b72ae:	add    $0x1b7,%eax
-   1804b72b3:	add    %al,0x3a(%rbx)
+   1804b72a0:	rex.RXB sub %r15d,%r9d
+   1804b72a3:	mov    $0x5c,%bh
+   1804b72a5:	mov    $0x46,%bl
+   1804b72a7:	rex.X mov $0x53352149,%esp
+   1804b72ad:	movabs 0x3a4300000001df12,%al
    1804b72b6:	pop    %rsp
    1804b72b7:	push   $0x5c656d6f
    1804b72bc:	imul   $0x5c626972,%fs:0x74(%rbx),%esi
    1804b72c4:	jo     0x1804b7335
    1804b72c6:	jb     0x1804b733c
    1804b72c8:	imul   $0x7274625c,0x67(%rsi),%ebp
    1804b72cf:	gs gs pop %rsp
```

## gamspy_copt/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

