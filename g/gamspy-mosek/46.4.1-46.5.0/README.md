# Comparing `tmp/gamspy_mosek-46.4.1-py3-none-win_amd64.whl.zip` & `tmp/gamspy_mosek-46.5.0-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8688761 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      423 b- defN 24-Apr-17 09:01 gamspy_mosek/__init__.py
--rw-rw-rw-  2.0 fat 24969728 b- defN 24-Apr-17 09:01 gamspy_mosek/mosek64_10_1.dll
--rw-rw-rw-  2.0 fat   568832 b- defN 24-Apr-17 09:01 gamspy_mosek/mskcclib64.dll
--rw-rw-rw-  2.0 fat   567328 b- defN 24-Apr-17 09:01 gamspy_mosek/msvcp140.dll
--rw-rw-rw-  2.0 fat    47074 b- defN 24-Apr-17 09:01 gamspy_mosek/optmosek.def
--rw-rw-rw-  2.0 fat   287880 b- defN 24-Apr-17 09:01 gamspy_mosek/tbb12.dll
--rw-rw-rw-  2.0 fat       22 b- defN 24-Apr-17 09:01 gamspy_mosek/version.py
--rw-rw-rw-  2.0 fat       62 b- defN 24-Apr-17 09:01 gamspy_mosek-46.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      104 b- defN 24-Apr-17 09:01 gamspy_mosek-46.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-17 09:01 gamspy_mosek-46.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      903 b- defN 24-Apr-17 09:01 gamspy_mosek-46.4.1.dist-info/RECORD
-11 files, 26442369 bytes uncompressed, 8687249 bytes compressed:  67.1%
+Zip file size: 8688762 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      423 b- defN 24-May-09 12:16 gamspy_mosek/__init__.py
+-rw-rw-rw-  2.0 fat 24969728 b- defN 24-May-09 12:16 gamspy_mosek/mosek64_10_1.dll
+-rw-rw-rw-  2.0 fat   568832 b- defN 24-May-09 12:16 gamspy_mosek/mskcclib64.dll
+-rw-rw-rw-  2.0 fat   567328 b- defN 24-May-09 12:16 gamspy_mosek/msvcp140.dll
+-rw-rw-rw-  2.0 fat    47074 b- defN 24-May-09 12:16 gamspy_mosek/optmosek.def
+-rw-rw-rw-  2.0 fat   287880 b- defN 24-May-09 12:16 gamspy_mosek/tbb12.dll
+-rw-rw-rw-  2.0 fat       22 b- defN 24-May-09 12:16 gamspy_mosek/version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 24-May-09 12:16 gamspy_mosek-46.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      104 b- defN 24-May-09 12:16 gamspy_mosek-46.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-May-09 12:16 gamspy_mosek-46.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      903 b- defN 24-May-09 12:16 gamspy_mosek-46.5.0.dist-info/RECORD
+11 files, 26442369 bytes uncompressed, 8687250 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: gamspy_mosek/tbb12.dll
 Comment: 
 
 Filename: gamspy_mosek/version.py
 Comment: 
 
-Filename: gamspy_mosek-46.4.1.dist-info/METADATA
+Filename: gamspy_mosek-46.5.0.dist-info/METADATA
 Comment: 
 
-Filename: gamspy_mosek-46.4.1.dist-info/WHEEL
+Filename: gamspy_mosek-46.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: gamspy_mosek-46.4.1.dist-info/top_level.txt
+Filename: gamspy_mosek-46.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gamspy_mosek-46.4.1.dist-info/RECORD
+Filename: gamspy_mosek-46.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gamspy_mosek/mskcclib64.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180076380
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Tue Apr 16 08:42:53 2024
+Time/Date		Wed May  8 04:07:07 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000077800
 SizeOfInitializedData	0000000000016200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000076380
@@ -127100,15 +127100,16 @@
    180083833:	add    %al,(%rax)
    180083835:	add    %al,(%rax)
    180083837:	add    %al,(%rax)
    180083839:	test   $0x18008,%eax
    18008383e:	add    %al,(%rax)
    180083840:	movabs 0x18008a9,%al
    180083849:	add    %al,(%rax)
-   18008384b:	add    %cl,0x661e3a(%rip)        # 0x1806e568b
+   18008384b:	add    %ch,-0x6(%rbx)
+   18008384e:	cmp    0x0(%rsi),%ah
    180083851:	add    %al,(%rax)
    180083853:	add    %cl,0x74000000(%rip)        # 0x1f4083859
    180083859:	add    (%rax),%al
    18008385b:	add    %bl,(%rax)
    18008385d:	cmp    (%rax),%cl
    18008385f:	add    %bl,(%rax)
    180083861:	es or  %al,(%rax)
```

## gamspy_mosek/version.py

```diff
@@ -1 +1 @@
-__version__ = '46.4.1'
+__version__ = '46.5.0'
```

## Comparing `gamspy_mosek-46.4.1.dist-info/RECORD` & `gamspy_mosek-46.5.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gamspy_mosek/__init__.py,sha256=aGEd-RRg0f171PafImR4QXDNmniF0KGFyJG-_xbyXMA,423
 gamspy_mosek/mosek64_10_1.dll,sha256=45l7MNuZKc3GbcC1epL0GpT3ryPkUiJ-ZJGNpFEqn3o,24969728
-gamspy_mosek/mskcclib64.dll,sha256=ELmX_qUFjjkezcdN9v70lH7M-7ODZBM9FEjo63qGl-0,568832
+gamspy_mosek/mskcclib64.dll,sha256=q73avP52ZD2wr7Uv9-_2dVnRsMUpqVjK1wtG7obQe-o,568832
 gamspy_mosek/msvcp140.dll,sha256=4KIqWU4Uj6Vc7vPkmWm_p3ARqAEmegvXgFtoG1k8nQs,567328
 gamspy_mosek/optmosek.def,sha256=GQEJ-1c6vIH8Sm5PV60hBMOIrx9fXxrG2ovrO6KThws,47074
 gamspy_mosek/tbb12.dll,sha256=Mn0HlR3yLt_ttok28yYL2T9s4y82EKHe_IyInCuj46I,287880
-gamspy_mosek/version.py,sha256=PfEsnAfLuXVTA7hSNu9m9ueNe8npaTtOAv06fL-xeY4,22
-gamspy_mosek-46.4.1.dist-info/METADATA,sha256=_bQO45WEauJsCOH539Td0aM36WJBKDFGTGE31efgArY,62
-gamspy_mosek-46.4.1.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
-gamspy_mosek-46.4.1.dist-info/top_level.txt,sha256=D_ibqdJHzeK1ovUML42JCi2Bg_SJ_XL0doZuT9jgKzg,13
-gamspy_mosek-46.4.1.dist-info/RECORD,,
+gamspy_mosek/version.py,sha256=XIdA4Cvl0eCbv31_g7hR2M0oeouzY6KRnEe6VcwZIX4,22
+gamspy_mosek-46.5.0.dist-info/METADATA,sha256=rEQX1OGCi3p_vgtuJp__9xFZdypH99ly9zzgFL2v6zg,62
+gamspy_mosek-46.5.0.dist-info/WHEEL,sha256=-H981hu6jK6YKd-c0qWpYxXA3UZMihQ3r30_4YPQguI,104
+gamspy_mosek-46.5.0.dist-info/top_level.txt,sha256=D_ibqdJHzeK1ovUML42JCi2Bg_SJ_XL0doZuT9jgKzg,13
+gamspy_mosek-46.5.0.dist-info/RECORD,,
```

