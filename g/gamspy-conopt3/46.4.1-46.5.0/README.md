# Comparing `tmp/gamspy_conopt3-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_conopt3-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 918868 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      376 b- defN 24-Apr-17 09:01 gamspy_conopt3/__init__.py
--rw-rw-rw-  2.0 fat   389632 b- defN 24-Apr-17 09:01 gamspy_conopt3/concclib64.dll
--rw-rw-rw-  2.0 fat  1851904 b- defN 24-Apr-17 09:01 gamspy_conopt3/conopt3.dll
--rw-rw-rw-  2.0 fat    12089 b- defN 24-Apr-17 09:01 gamspy_conopt3/optconopt3.def
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_conopt3/version.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-17 09:01 gamspy_conopt3-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_conopt3-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-17 09:01 gamspy_conopt3-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      752 b- defN 24-Apr-17 09:01 gamspy_conopt3-46.4.1.dist-info/RECORD
-9 files, 2254958 bytes uncompressed, 917572 bytes compressed:  59.3%
+Zip file size: 918869 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      376 b- defN 24-May-09 12:15 gamspy_conopt3/__init__.py
+-rw-rw-rw-  2.0 fat   389632 b- defN 24-May-09 12:15 gamspy_conopt3/concclib64.dll
+-rw-rw-rw-  2.0 fat  1851904 b- defN 24-May-09 12:15 gamspy_conopt3/conopt3.dll
+-rw-rw-rw-  2.0 fat    12089 b- defN 24-May-09 12:15 gamspy_conopt3/optconopt3.def
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:15 gamspy_conopt3/version.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-May-09 12:15 gamspy_conopt3-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:15 gamspy_conopt3-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-09 12:15 gamspy_conopt3-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      752 b- defN 24-May-09 12:15 gamspy_conopt3-46.5.0.dist-info/RECORD
+9 files, 2254958 bytes uncompressed, 917573 bytes compressed:  59.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: gamspy_conopt3/optconopt3.def
 Comment: 
 
 Filename: gamspy_conopt3/version.py
 Comment: 
 
-Filename: gamspy_conopt3-46.4.1.dist-info/METADATA
+Filename: gamspy_conopt3-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_conopt3-46.4.1.dist-info/WHEEL
+Filename: gamspy_conopt3-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_conopt3-46.4.1.dist-info/top_level.txt
+Filename: gamspy_conopt3-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_conopt3-46.4.1.dist-info/RECORD
+Filename: gamspy_conopt3-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_conopt3/concclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018004ff90
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:12:03 2024
+Time/Date		Wed May  8 03:38:37 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000051600
 SizeOfInitializedData	0000000000010200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000004ff90
@@ -85544,19 +85544,17 @@
    18005a617:	add    %al,%al
    18005a619:	in     (%dx),%eax
    18005a61a:	add    $0x180,%eax
    18005a61f:	add    %ah,-0x12(%rax)
    18005a622:	add    $0x180,%eax
    18005a627:	add    %al,(%rax)
    18005a629:	add    %al,(%rax)
-   18005a62b:	add    %dl,%bl
-   18005a62d:	xor    (%rsi),%bl
-   18005a62f:	data16 add %al,(%rax)
-   18005a632:	add    %al,(%rax)
-   18005a634:	or     $0x64000000,%eax
+   18005a62b:	add    %bh,0x663af3(%rbp)
+   18005a631:	add    %al,(%rax)
+   18005a633:	add    %cl,0x64000000(%rip)        # 0x1e405a639
    18005a639:	add    (%rax),%al
    18005a63b:	add    %bl,(%rax)
    18005a63d:	test   $0x5,%al
    18005a63f:	add    %bl,(%rax)
    18005a641:	xchg   %eax,%edx
    18005a642:	add    $0x0,%eax
 	...
```

## gamspy_conopt3/conopt3.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180177ee0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:11:17 2024
+Time/Date		Wed May  8 03:37:54 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000179600
 SizeOfInitializedData	000000000004bc00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000177ee0
@@ -374612,19 +374612,18 @@
    1801a56fc:	add    %eax,(%rax)
    1801a56fe:	add    %al,(%rax)
    1801a5700:	orb    $0x1c,(%rbx)
    1801a5703:	addb   $0x0,(%rcx)
    1801a5706:	add    %al,(%rax)
    1801a5708:	add    %al,(%rax)
    1801a570a:	add    %al,(%rax)
-   1801a570c:	movsl  %ds:(%rsi),%es:(%rdi)
-   1801a570d:	xor    (%rsi),%bl
-   1801a570f:	data16 add %al,(%rax)
-   1801a5712:	add    %al,(%rax)
-   1801a5714:	or     $0x64000000,%eax
+   1801a570c:	xchg   %eax,%edx
+   1801a570d:	repz cmp 0x0(%rsi),%ah
+   1801a5711:	add    %al,(%rax)
+   1801a5713:	add    %cl,0x64000000(%rip)        # 0x1e41a5719
    1801a5719:	add    (%rax),%al
    1801a571b:	add    %bl,-0x67ffe5a8(%rax)
    1801a5721:	rex.X sbb (%rax),%al
 	...
    1801a5730:	cmp    %al,(%rcx)
 	...
    1801a5786:	add    %al,(%rax)
```

## gamspy_conopt3/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

## Comparing `gamspy_conopt3-46.4.1.dist-info/RECORD` & `gamspy_conopt3-46.5.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 gamspy_conopt3/__init__.py,sha256=OvhHlXUwZkxTiLEc8YoOAWWb0dxmHRIv7cBd4SqwD_Q,376
-gamspy_conopt3/concclib64.dll,sha256=w4KLM4__cUj_KgQ4XCUIceNr5SRjBVMvZvXyGL0KPT0,389632
-gamspy_conopt3/conopt3.dll,sha256=dT3rZuUFFHxz75p06aROT08am-zrnGijNwaxglocO1o,1851904
+gamspy_conopt3/concclib64.dll,sha256=JBVz8xUf2TT64YOMWk9yBSeVrHgZANm4PaZjV8DgSXQ,389632
+gamspy_conopt3/conopt3.dll,sha256=S1Z1lo9YfaLV8jIEf1WfoekiYSX8Uj3y7KYHoq9-vAo,1851904
 gamspy_conopt3/optconopt3.def,sha256=U9YGfmwi2Shi-8xuQJAucu8TYYjfikQtxz5sL5YtfOg,12089
-gamspy_conopt3/version.py,sha256=PfEsnAfLuXVTA7hSNu9m9ueNe8npaTtOAv06fL-xeY4,22
-gamspy_conopt3-46.4.1.dist-info/METADATA,sha256=44Gs7SzR78Q_bhfNIUn9QoVelifuIKVGeibnbZy49Dk,64
-gamspy_conopt3-46.4.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_conopt3-46.4.1.dist-info/top_level.txt,sha256=Poz3GSL3_9WLP1rAqBZe77fCs5adCxx4am8paKvD_GQ,15
-gamspy_conopt3-46.4.1.dist-info/RECORD,,
+gamspy_conopt3/version.py,sha256=XIdA4Cvl0eCbv31_g7hR2M0oeouzY6KRnEe6VcwZIX4,22
+gamspy_conopt3-46.5.0.dist-info/METADATA,sha256=dDERostZuhFWNK26zP-XkV02F7LfOZMVrVpJiFwAflM,64
+gamspy_conopt3-46.5.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_conopt3-46.5.0.dist-info/top_level.txt,sha256=Poz3GSL3_9WLP1rAqBZe77fCs5adCxx4am8paKvD_GQ,15
+gamspy_conopt3-46.5.0.dist-info/RECORD,,
```

