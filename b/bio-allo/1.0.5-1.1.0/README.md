# Comparing `tmp/bio-allo-1.0.5.tar.gz` & `tmp/bio_allo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-allo-1.0.5.tar", last modified: Mon Sep 11 14:52:00 2023, max compression
+gzip compressed data, was "bio_allo-1.1.0.tar", last modified: Thu May  9 21:17:43 2024, max compression
```

## Comparing `bio-allo-1.0.5.tar` & `bio_allo-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2023-09-11 14:52:00.785979 bio-allo-1.0.5/
-drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2023-09-11 14:52:00.747484 bio-allo-1.0.5/Allo/
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       74 2023-09-11 14:42:55.000000 bio-allo-1.0.5/Allo/__init__.py
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)    13771 2023-09-06 20:24:13.000000 bio-allo-1.0.5/Allo/allo
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)    28969 2023-09-06 20:24:24.000000 bio-allo-1.0.5/Allo/allocation.py
--rw-r-----   0 anm5579  (769571) sam77_collab (11783692)   285408 2023-03-06 16:26:33.000000 bio-allo-1.0.5/Allo/mixed.h5
--rw-r-----   0 anm5579  (769571) sam77_collab (11783692)     3317 2023-09-06 20:07:03.000000 bio-allo-1.0.5/Allo/mixed.json
--rw-r-----   0 anm5579  (769571) sam77_collab (11783692)   285448 2023-03-06 16:26:33.000000 bio-allo-1.0.5/Allo/narrow.h5
--rw-r-----   0 anm5579  (769571) sam77_collab (11783692)     3303 2023-09-06 20:07:04.000000 bio-allo-1.0.5/Allo/narrow.json
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     1389 2023-09-06 20:24:37.000000 bio-allo-1.0.5/Allo/predictPeak.py
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     1103 2023-09-06 20:07:25.000000 bio-allo-1.0.5/LICENSE.txt
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       38 2023-09-06 20:07:25.000000 bio-allo-1.0.5/MANIFEST.in
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      315 2023-09-11 14:52:00.783068 bio-allo-1.0.5/PKG-INFO
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     5000 2023-09-11 14:49:35.000000 bio-allo-1.0.5/README.md
-drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2023-09-11 14:52:00.776172 bio-allo-1.0.5/bio_allo.egg-info/
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      315 2023-09-11 14:52:00.000000 bio-allo-1.0.5/bio_allo.egg-info/PKG-INFO
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      329 2023-09-11 14:52:00.000000 bio-allo-1.0.5/bio_allo.egg-info/SOURCES.txt
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)        1 2023-09-11 14:52:00.000000 bio-allo-1.0.5/bio_allo.egg-info/dependency_links.txt
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       36 2023-09-11 14:52:00.000000 bio-allo-1.0.5/bio_allo.egg-info/requires.txt
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)        5 2023-09-11 14:52:00.000000 bio-allo-1.0.5/bio_allo.egg-info/top_level.txt
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       38 2023-09-11 14:52:00.787375 bio-allo-1.0.5/setup.cfg
--rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      506 2023-09-11 14:48:10.000000 bio-allo-1.0.5/setup.py
+drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2024-05-09 21:17:43.500962 bio_allo-1.1.0/
+drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2024-05-09 21:17:43.451375 bio_allo-1.1.0/Allo/
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       74 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/__init__.py
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)    14851 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/allo
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)    34518 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/allocation.py
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)   291776 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/atac.h5
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     4730 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/atac.json
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)   291744 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/dnase.h5
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     4732 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/dnase.json
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)   285408 2024-04-22 02:40:44.000000 bio_allo-1.1.0/Allo/mixed.h5
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     3317 2024-04-22 02:40:44.000000 bio_allo-1.1.0/Allo/mixed.json
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)   285448 2024-04-22 02:40:44.000000 bio_allo-1.1.0/Allo/narrow.h5
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     3303 2024-04-22 02:40:44.000000 bio_allo-1.1.0/Allo/narrow.json
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     1514 2024-05-09 15:09:10.000000 bio_allo-1.1.0/Allo/predictPeak.py
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)   285184 2024-05-09 15:07:47.000000 bio_allo-1.1.0/Allo/rna.h5
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     4716 2024-05-09 15:07:47.000000 bio_allo-1.1.0/Allo/rna.json
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     1103 2024-04-22 02:44:24.000000 bio_allo-1.1.0/LICENSE.txt
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       38 2024-04-22 02:44:24.000000 bio_allo-1.1.0/MANIFEST.in
+-rw-r--r--   0 anm5579  (769571) sam77_collab (11783692)      412 2024-05-09 21:17:43.495011 bio_allo-1.1.0/PKG-INFO
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)     7398 2024-05-09 21:16:34.000000 bio_allo-1.1.0/README.md
+drwxrws---   0 anm5579  (769571) sam77_collab (11783692)        0 2024-05-09 21:17:43.487336 bio_allo-1.1.0/bio_allo.egg-info/
+-rw-r--r--   0 anm5579  (769571) sam77_collab (11783692)      412 2024-05-09 21:17:43.000000 bio_allo-1.1.0/bio_allo.egg-info/PKG-INFO
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      413 2024-05-09 21:17:43.000000 bio_allo-1.1.0/bio_allo.egg-info/SOURCES.txt
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)        1 2024-05-09 21:17:43.000000 bio_allo-1.1.0/bio_allo.egg-info/dependency_links.txt
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       36 2024-05-09 21:17:43.000000 bio_allo-1.1.0/bio_allo.egg-info/requires.txt
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)        5 2024-05-09 21:17:43.000000 bio_allo-1.1.0/bio_allo.egg-info/top_level.txt
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)       38 2024-05-09 21:17:43.503243 bio_allo-1.1.0/setup.cfg
+-rw-rw----   0 anm5579  (769571) sam77_collab (11783692)      507 2024-05-09 21:16:34.000000 bio_allo-1.1.0/setup.py
```

### Comparing `bio-allo-1.0.5/Allo/allo` & `bio_allo-1.1.0/Allo/allo`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,66 @@
 #!/usr/bin/env python
 #Lexi Morrissey, Mahony Lab @ Pennsylvania State University
-#Last updated 03.06.2023
 #Main method for Allo. Splits the sam files up and sends them to allocation procedure via multiprocessing package.
 
 #Arguments
 import argparse
 parser = argparse.ArgumentParser(prog = 'Allo', \
                     description = 'Allo is a software that allocates multi-mapped reads in ChIP-seq data\n' \
                     'Developed by Alexis Morrissey, Mahony Laboratory @ The Pennsylvania State University', \
                     epilog= 'For more pre-processing info and basic usage, please visit https://github.com/seqcode/allo')
 parser.add_argument('input')
 parser.add_argument('-seq', type=str, nargs=1, help='Single-end or paired-end sequencing mode', \
                    choices=['pe','se'], required=True, dest='seq')
 parser.add_argument('-o', type=str, nargs=1, help='Output file name', dest='outfile', default=None)
-parser.add_argument('--mixed', help='Use CNN trained on a dataset with mixed peaks, narrow by default', action='store_true', default=None)
+parser.add_argument('--mixed', help='Use CNN trained on a dataset with mixed ChIP-seq peaks, narrow by default', action='store_true', default=None)
+parser.add_argument('--dnase', help='Use CNN trained on a DNa-seq datasets', action='store_true', default=None)
+parser.add_argument('--atac', help='Use CNN trained on a ATAC-seq datasets', action='store_true', default=None)
+parser.add_argument('--splice', help='Remove splice sites based on cigar string when constructing image', action='store_true', default=None)
 parser.add_argument('-p', type=int, nargs=1, help='Number of processes, 1 by default', dest='processes', default=None)
 parser.add_argument('-max', type=int, nargs=1, help='Maximum value for number of locations a read can map', dest='maxlocations', default=None)
 parser.add_argument('--keep-unmap', help='Keep unmapped reads and reads that include N in their sequence', action='store_true', default=None)
 parser.add_argument('--remove-zeros', help='Disregard multi-mapped reads that map to regions with 0 uniquely mapped reads (random assignment)', action='store_true', default=None)
 parser.add_argument('--r2', help='Use read 2 for allocation procedure instead of read 1 (only for paired-end sequencing)', action='store_true', default=None)
 parser.add_argument('--readcount', help='CNN will not be used in allocation, only read counts', action='store_true', default=None)
 parser.add_argument('--random', help='Reads will be randomly assigned (similar to Bowtie and BWA on default)', action='store_true', default=None)
 parser.add_argument('--ignore', help='Ignore warnings about read sorting', action='store_true', default=None)
 parser.add_argument('--parser', help='Ignore warnings about read sorting', action='store_true', default=None)
 args = parser.parse_args()
 
 #Imports
+import Allo
+from Allo import allocation
 import sys
 from joblib import Parallel, delayed
 import multiprocessing
 import subprocess
 import os
-from Allo import allocation
 import math
 from random import randint
-import shutil
 import glob
 import pysam
 import shutil
 import pkgutil
-import Allo
+
+
 
 
 #Function for concatenating files
 def cat(files, outname):
     with open(outname,'wb') as wfd:
         for f in files:
             with open(f,'rb') as fd:
                 shutil.copyfileobj(fd, wfd)
+            
 
 ##Main Method##          
 if __name__ == '__main__':
     
-    print("\nRunning Allo version 1.0\n\n")
+    print("\nRunning Allo version 1.1\n\n")
     
     #Make a folder to store all temp files in allo
     ids = str(randint(0, 10000))
     curr_dir = os.getcwd()
     allo_dir = os.path.join(curr_dir, r'allo.'+ids)
     if not os.path.exists(allo_dir):
         os.makedirs(allo_dir)
@@ -80,14 +84,22 @@
     else:
         outfile = args.input[:-4] + ".allo.sam"
     #Model and window size
     if args.mixed is not None:
         d = os.path.dirname(sys.modules["Allo"].__file__)
         m = os.path.join(d, "mixed")
         winSize = 500
+    elif args.dnase is not None:
+        d = os.path.dirname(sys.modules["Allo"].__file__)
+        m = os.path.join(d, "dnase")
+        winSize = 500
+    elif args.atac is not None:
+        d = os.path.dirname(sys.modules["Allo"].__file__)
+        m = os.path.join(d, "atac")
+        winSize = 500
     else:
         d = os.path.dirname(sys.modules["Allo"].__file__)
         m = os.path.join(d, "narrow")
         winSize = 500
     #Number of threads
     if args.processes is not None:
         thr = args.processes[0]
@@ -101,14 +113,15 @@
     #Options for probabilities
     if args.readcount is not None:
         rc = 1
     elif args.random is not None:
         rc = 2
     else:
         rc = 0
+        print("Neural network mode on...", flush=True)
     #Keep unmapped reads
     if args.keep_unmap is not None:
         keep = 1
     else:
         keep = 0
     #Remove reads that only map to zero regions
     if args.remove_zeros is not None:
@@ -131,15 +144,19 @@
     else:
         ig = 0
     #Use allo's parser function only
     if args.parser is not None:
         parse = 1
     else:
         parse = 0
-    
+    #Cut out introns based on identified splice sites using cigar string
+    if args.splice is not None:
+        splice = 1
+    else:
+        splice = 0
     
     #Getting header information and checking to see if file was sorted
     collate = 0
     f = open(samfile)
     header = open(allo_dir+'/header', 'a')
     for line in f:
         if line.startswith('@'):
@@ -228,37 +245,40 @@
         os.rename(tempList[0]+".catborders", tempList[0]+"UM")
         #Remove old files
         for filename in glob.glob('./*borders*'):
             os.remove(filename)
             
         #Add all values to UMR dictionary
         genLand = {}
+        if splice == 1:
+            spliceD = {}
+        else:
+            spliceD = None
         if parse == 0: 
             for i in tempList:
                 if os.path.exists(str(i)+"UM"):
-                    allocation.addToDict(str(i)+"UM", genLand, seq)
-            
+                    allocation.addToDict(str(i)+"UM", genLand, spliceD, seq) 
         else: #Stopping if parsing only
             l = [allo_dir+"/header"]
             for i in tempList:
                 if os.path.exists(str(i)+"UM"):
                     l.append(i + "UM")
             cat(l, args.input[:-4]+".allo.UMR_only.sam")
             l = [allo_dir+"/header"]
             for i in tempList:
                 if os.path.exists(str(i)+"MM"):
                     l.append(i + "MM")
             cat(l, args.input[:-4]+".allo.MMR_only.sam")
             shutil.rmtree(allo_dir)
             sys.exit(0)
             
-        print("Parsing finished!\n")
+        print("Parsing finished!\n", flush=True)
         
         #PHASE II: Parsing multi-mapped reads
-        info2 = Parallel(n_jobs=thr)(delayed(allocation.parseMulti)(i, winSize, genLand, m, cnn_scores, rc, keep, rmz, maxa) for i in tempList)
+        info2 = Parallel(n_jobs=thr)(delayed(allocation.parseMulti)(i, winSize, genLand, m, cnn_scores, rc, keep, rmz, maxa, spliceD) for i in tempList)
         
         
         #Final parsing and file clean up
         #Deleting temporary files and join allocated files
         l = [allo_dir+"/header"]
         for i in tempList:
             if os.path.exists(str(i)+"AL"):
@@ -310,36 +330,40 @@
         #Cat with first UM file
         cat([tempList[0]+'UM', tempList[0]+'.bordersUM'], tempList[0]+'.catborders')
         #Fix name
         os.rename(tempList[0]+".catborders", tempList[0]+"UM")
         
         #Add all values to UMR dictionary unless only parsing
         genLand = {}
+        if splice == 1:
+            spliceD = {}
+        else:
+            spliceD = None
         if parse == 0: 
             for i in tempList:
                 if os.path.exists(str(i)+"UM"):
-                    allocation.addToDict(str(i)+"UM", genLand, seq)
+                    allocation.addToDict(str(i)+"UM", genLand, spliceD, seq) 
         else:
             l = [allo_dir+"/header"]
             for i in tempList:
                 if os.path.exists(str(i)+"UM"):
                     l.append(i + "UM")
             cat(l, args.input[:-4]+".allo.UMR_only.sam")
             l = [allo_dir+"/header"]
             for i in tempList:
                 if os.path.exists(str(i)+"MM"):
                     l.append(i + "MM")
             cat(l, args.input[:-4]+".allo.MMR_only.sam")
             shutil.rmtree(allo_dir)
             sys.exit(0)
             
-        print("Parsing finished!\n")
+        print("Parsing finished!\n", flush=True)
         
         #PHASE II: Parsing multi-mapped reads
-        info2 = Parallel(n_jobs=thr)(delayed(allocation.parseMultiPE)(i, winSize, genLand, m, cnn_scores, rc, keep, rmz, maxa) for i in tempList)
+        info2 = Parallel(n_jobs=thr)(delayed(allocation.parseMultiPE)(i, winSize, genLand, m, cnn_scores, rc, keep, rmz, maxa, spliceD) for i in tempList)
         
         #Final parsing and file clean up
         #Deleting temporary files and join allocated files
         l = [allo_dir+"/header"]
         for i in tempList:
             if os.path.exists(str(i)+"AL"):
                 l.append(i + "AL")
```

### Comparing `bio-allo-1.0.5/Allo/allocation.py` & `bio_allo-1.1.0/Allo/allocation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 #Lexi Morrissey, Mahony Lab @ Pennsylvania State University
-#Last updated 03.01.2023
 #Contains methods for read allocation procedure of Allo.
 
 from Allo import predictPeak
 import math
 import random
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
@@ -12,66 +11,160 @@
 from tensorflow import keras
 from tensorflow.keras.models import load_model, Model
 import pickle
 import time 
 import numpy as np
 import sys
 import multiprocessing
-
+import re
+import absl.logging
+absl.logging.set_verbosity(absl.logging.ERROR)
+import contextlib, io
 
 #Add reads to UMR dictionary
-def addToDict(tempFile, genLand, seq):
+def addToDict(tempFile, genLand, spliceD, seq):
     count = 0
     with open(tempFile) as f:
         for line in f:
             l = line.strip().split('\t')
             if l[2] == "*":
                 continue
             elif "N" in l[9]:
                 continue
             count = count + 1
             if seq == 0 and not (count % 2) == 0:
                 continue
+            l[3] = int(l[3])
+            #Add to dictionary
             key = l[2] + ";" + str(l[3])
             if key in genLand:
                 genLand[key] = genLand[key] + 1
             else:
                 genLand[key] = 1
+            if not spliceD == None:
+                chars = re.findall('[A-Za-z]+', l[5])
+                gaps = [i for i, x in enumerate(chars) if x == "N"]
+                if len(gaps) > 0:
+                    num = re.findall('\d+\.\d+|\d+', l[5])
+                    curLoc = int(l[3])
+                    for i in range(0,len(chars)):
+                        if chars[i]=="M" or chars[i]=="D" or chars[i]=="=" or chars[i]=="X":
+                            curLoc = curLoc + int(num[i])
+                        elif chars[i]=="N":
+                            if l[2]+";"+str(curLoc) in spliceD:
+                                if spliceD[l[2]+";"+str(curLoc)] > curLoc + int(num[i]):
+                                    pos = int(curLoc)
+                                    size = int(num[i])
+                                    spliceD[l[2]+";"+str(pos)] = size
+                                    spliceD[l[2]+";"+str(pos+size)] = size
+                            else:
+                                pos = int(curLoc)
+                                size = int(num[i])
+                                spliceD[l[2]+";"+str(pos)] = size
+                                #Adding splice in reverse direction
+                                spliceD[l[2]+";"+str(pos+size)] = -1*(size)
+                            curLoc = curLoc + int(num[i])
 
 #Used to get counts in regions around multimapped reads
-def getArray(read, winSize, genLand):
-    array = []
-    pos = round(int(read[3])/100)*100
-    for k in range (pos-math.floor(winSize/2),int(pos)+math.floor(winSize/2)):
-        key = read[2] + ";" + str(k)
-        #Seeing if current pos in genetic landscape
-        if key in genLand:
-            array.append(genLand[key])
-        else:
-            array.append(0)
+def getArray(read, winSize, genLand, spliceD):
+    #Spliced array using junction info
+    if spliceD:
+        #Parsing cigar string
+        chars = re.findall('[A-Za-z]+', read[5])
+        num = re.findall('\d+\.\d+|\d+', read[5])
+        gap_loc = {}
+        start = int(read[3])
+        chr = read[2]
+        r_end = start #Get information about end of read to use for splice variants
+        #print("cigar: " + read[5], flush=True)
+        for i in range(0,len(chars)):
+            if chars[i]=="M" or chars[i]=="D" or chars[i]=="=" or chars[i]=="X":
+                r_end = r_end + int(num[i]) - 1
+            elif chars[i]=="N":
+                gap_loc[r_end+1]=int(num[i])
+                r_end = r_end + int(num[i])
+        array = []
+        k = start
+        l = 0
+        #Upstream counts
+        while l <= math.floor(winSize/2):
+            #print("up: " + str(k), flush=True)
+            key = chr + ";" + str(k)
+            '''if key in spliceD and spliceD[key] < 0:
+                #print("splice: " + str(splice[key]), flush=True)
+                k = k + spliceD[key]
+                key = chr + ";" + str(k)'''
+            if key in genLand:
+                array.insert(0,genLand[key])
+            else:
+                array.insert(0,0)
+            k -= 1
+            l += 1
+        start_pos = k
+        #Downstream counts 
+        k = start
+        l = 0
+        while l <= math.floor(winSize/2):
+            #Taking splice information from read if present
+            while k < r_end:
+                key = chr + ";" + str(k)
+                if k in gap_loc:
+                    k = k + gap_loc[k]
+                    continue
+                elif key in genLand:
+                    array.append(genLand[key])
+                else:
+                    array.append(0)
+                k += 1
+                l += 1
+            #Else use previously found splice info
+            key = chr + ";" + str(k)
+            '''if key in spliceD and spliceD[key] > 0:
+                k = k + spliceD[key]
+                key = chr + ";" + str(k)'''
+            if key in genLand:
+                array.append(genLand[key])
+            else:
+                array.append(0)
+            k += 1
+            l += 1
+    #Non-spliced array
+    else:
+        array = []
+        pos = round(int(read[3])/100)*100
+        for k in range (pos-math.floor(winSize/2),int(pos)+math.floor(winSize/2)):
+            key = read[2] + ";" + str(k)
+            #Seeing if current pos in genetic landscape
+            if key in genLand:
+                array.append(genLand[key])
+            else:
+                array.append(0)
     return array
 
 
 #Assign reads (straight to dictionary for uniq and actual assign for multi-mapped)
-def readAssign(rBlock, samOut, winSize, genLand, model, cnn_scores, rc, rmz, modelName):
+def readAssign(rBlock, samOut, winSize, genLand, model, cnn_scores, rc, rmz, spliceD):
     random.seed(7)      #To make results reproducible
 
     ##Multi-mapped reads##
     ###CNN###
     scores_rc = []
     scores_nn = []
     allZ = True #seeing if all zero regions
     for i in rBlock:
         #Find closest 100 window, use that score instead if it's already been assigned, saves time
-        pos = i[2]+str(round(int(i[3])/100)*100)
+        if spliceD:
+            pos = i[2]+";"+str(i[3])
+        else:
+            pos = i[2]+";"+str(round(int(i[3])/100)*100)
         if pos in cnn_scores:
             scores_nn.append(cnn_scores[pos])
             allZ = False
         else:
-            countArray = getArray(i, winSize, genLand)
+            countArray = getArray(i, winSize, genLand, spliceD)
             s = sum(countArray)
             if s > 0:
                 allZ = False
             #Allocation options
             if rc == 1:
                 if s == 0:
                     scores_rc.append(1)
@@ -80,16 +173,14 @@
                 continue
             if rc == 2:
                 scores_rc.append(1)
                 continue
             #Use no read score if zero region
             if s == 0:
                 scores_nn.append(0.0012*(s+1))
-            elif s <= 5:
-                scores_nn.append(0.0062*(s+1))
             else:
                 nn = predictPeak.predictNN(countArray, winSize, model)
                 scores_nn.append(nn*(s+1))
                 cnn_scores[pos] = (nn*(s+1))
     
     #Removing reads that mapped to all zero regions
     if allZ and rmz == 1:
@@ -124,15 +215,14 @@
 
 #Getting uniquely mapped reads into temp files and putting them in the dictionary
 def parseUniq(tempFile, winSize, cnn_scores, AS, rc, keep):
     #Variables for stats
     cu = 0  #UMRs
     cf = 0  #Filtered
     
-    modelName = None
     model = None
     rmz = None
     rBlock = []
     if "border" in tempFile:
         b = 1
     else:
         b = 0
@@ -282,31 +372,30 @@
     MM.close()
     if b == 0:
         B.close()
     os.remove(tempFile) #Removing old temp
     return [cu, cf]
 
 
-def parseMulti(tempFile, winSize, genLand, modelName, cnn_scores, rc, keep, rmz, maxa):
+def parseMulti(tempFile, winSize, genLand, modelName, cnn_scores, rc, keep, rmz, maxa, spliceD):   
     numLoc = [0,0] #Keep info on average number of places read maps to
     #Getting trained CNN
-    try:
-        json_file = open(modelName+'.json', 'r')
-        loaded_model_json = json_file.read()
-        json_file.close()
-        model = tf.keras.models.model_from_json(loaded_model_json)
-        model.load_weights(modelName+'.h5')
-        if "mixed" in modelName:
-            modelName = 1
-        else:
-            modelName = 0
-    except:
-        print("Could not load Tensorflow model :( Allo was written with Tensorflow version 2.11")
-        sys.exit(0)
-
+    if rc == 0:
+        try:
+            json_file = open(modelName+'.json', 'r')
+            loaded_model_json = json_file.read()
+            json_file.close()
+            model = tf.keras.models.model_from_json(loaded_model_json)
+            model.load_weights(modelName+'.h5')
+            model = LiteModel.from_keras_model(model)
+        except:
+            print("Could not load Tensorflow model :( Allo was written with Tensorflow version 2.11")
+            sys.exit(0)
+    else:
+        model = None
     #Exception that causes errors
     if os.stat(tempFile+"MM").st_size == 0:
         return numLoc
     
     #File with MM allocations
     AL = open(tempFile + "AL","w+")
     tempFile = tempFile + "MM"
@@ -342,40 +431,39 @@
                 
                 #New block, have to allocate reads
                 if not r[0] == leadr[0]:
                     if maxa is not None and len(rBlock) > maxa:
                         rBlock = []
                         rBlock.append(r)
                         continue
-                    readAssign(rBlock, AL, winSize, genLand, model, cnn_scores, rc, rmz, modelName)
+                    readAssign(rBlock, AL, winSize, genLand, model, cnn_scores, rc, rmz, spliceD)
                     #Getting average number of locations mapped to
                     numLoc[0] = (numLoc[0]*numLoc[1] + len(rBlock)) / (numLoc[1]+1)
                     numLoc[1] = numLoc[1] + 1
                     #Creating a new read block for the next read
                     rBlock = [] 
                     rBlock.append(r)
 
     #For last read
     if maxa is None or len(rBlock) <= maxa:
-        readAssign(rBlock, AL, winSize, genLand, model, cnn_scores, rc, rmz, modelName)
+        readAssign(rBlock, AL, winSize, genLand, model, cnn_scores, rc, rmz, spliceD)
         numLoc[0] = (numLoc[0]*numLoc[1] + len(rBlock)) / (numLoc[1]+1)
         numLoc[1] = numLoc[1] + 1
 
     os.remove(tempFile) #Removing old temp
     AL.close()
     return numLoc
     
 
 #Getting uniquely mapped reads into temp files and putting them in the dictionary
 def parseUniqPE(tempFile, winSize, cnn_scores, AS, rc, keep, r2):
     #Keeping information on read counts
     cu = 0
     cf = 0
     
-    modelName = None
     model = None
     rmz = None
     if "border" in tempFile:
         b = 1
     else:
         b = 0
     rBlock = []
@@ -608,29 +696,32 @@
     if b == 0:
         B.close()
     os.remove(tempFile) #Removing old temp
     return [cu, cf]
 
 
 #Assign reads (straight to dictionary for uniq and actual assign for multi-mapped)
-def readAssignPE(rBlock, rBlock2, samOut, winSize, genLand, model, cnn_scores, rc, rmz, modelName):
+def readAssignPE(rBlock, rBlock2, samOut, winSize, genLand, model, cnn_scores, rc, rmz, spliceD):
     random.seed(7)      #To make results reproducible
     ##Multi-mapped reads##
     ###CNN###
     scores_rc = []
     scores_nn = []
     allZ = True #seeing if all zero regions
     for i in rBlock:
         #Find closest 100 window, use that score instead if it's already been assigned, saves time
-        pos = i[2]+str(round(int(i[3])/100)*100)
+        if spliceD:
+            pos = i[2]+";"+str(i[3])
+        else:
+            pos = i[2]+";"+str(round(int(i[3])/100)*100)
         if pos in cnn_scores:
             scores_nn.append(cnn_scores[pos])
             allZ = False
         else:
-            countArray = getArray(i, winSize, genLand)
+            countArray = getArray(i, winSize, genLand, spliceD)
             s = sum(countArray)
             if s > 0:
                 allZ = False
             #Allocation options
             if rc == 1:
                 if s == 0:
                     scores_rc.append(1)
@@ -639,16 +730,14 @@
                 continue
             if rc == 2:
                 scores_rc.append(1)
                 continue
             #Use no read score if zero region
             if s == 0:
                 scores_nn.append(0.0012*(s+1))
-            elif s <= 5:
-                scores_nn.append(0.0062*(s+1))
             else:
                 nn = predictPeak.predictNN(countArray, winSize, model)
                 scores_nn.append(nn*(s+1))
                 cnn_scores[pos] = (nn*(s+1))
     
     #Removing reads that mapped to all zero regions
     if allZ and rmz == 1:
@@ -681,30 +770,30 @@
         rBlock[choice].append("ZZ:Z:" + str(len(rBlock)) + "\n")
         rBlock2[choice].append("ZZ:Z:" + str(len(rBlock)) + "\n")
     samOut.write('\t'.join(rBlock[choice]))
     samOut.write('\t'.join(rBlock2[choice]))
     return
 
 
-def parseMultiPE(tempFile, winSize, genLand, modelName, cnn_scores, rc, keep, rmz, maxa):
+def parseMultiPE(tempFile, winSize, genLand, modelName, cnn_scores, rc, keep, rmz, maxa, spliceD):
     numLoc = [0,0] #Retain info on number of mapping sites
     #Getting trained CNN and making sure there is a compatible tensorflow installed
-    try:
-        json_file = open(modelName+'.json', 'r')
-        loaded_model_json = json_file.read()
-        json_file.close()
-        model = tf.keras.models.model_from_json(loaded_model_json)
-        model.load_weights(modelName+'.h5')
-        if "mixed" in modelName:
-            modelName = 1
-        else:
-            modelName = 0
-    except:
-        print("Could not load Tensorflow model :( Allo was written with Tensorflow version 2.11")
-        sys.exit(0)
+    if rc == 0:
+        try:
+            json_file = open(modelName+'.json', 'r')
+            loaded_model_json = json_file.read()
+            json_file.close()
+            model = tf.keras.models.model_from_json(loaded_model_json)
+            model.load_weights(modelName+'.h5')
+            model = LiteModel.from_keras_model(model)
+        except:
+            print("Could not load Tensorflow model :( Allo was written with Tensorflow version 2.11")
+            sys.exit(0)
+    else:
+        model = None
 
     #Exception that causes errors
     if os.stat(tempFile+"MM").st_size == 0:
         return numLoc
     
     #File with MM allocations
     AL = open(tempFile + "AL","w+")
@@ -759,27 +848,72 @@
                         print("Pairs not sorted properly. Issue with following entry.")
                         print(r[0])
                         sys.exit(0)
             #If different read, begin read assignment
             else:
                 if maxa is not None and len(rBlock) > maxa:
                     continue
-                readAssignPE(rBlock, rBlock2, AL, winSize, genLand, model, cnn_scores, rc, rmz, modelName)
+                readAssignPE(rBlock, rBlock2, AL, winSize, genLand, model, cnn_scores, rc, rmz, spliceD)
                 numLoc[0] = (numLoc[0]*numLoc[1] + len(rBlock)) / (numLoc[1]+1)
                 numLoc[1] = numLoc[1] + 1
                 rBlock = []
                 rBlock2 = []
                 rBlock.append(r)
                 curRead = r[0]
                 numR = numR + 1
                 numL = 1
 
     #For last read
     if maxa is None or len(rBlock) <= maxa:
-        readAssignPE(rBlock, rBlock2, AL, winSize, genLand, model, cnn_scores, rc, rmz, modelName)
+        readAssignPE(rBlock, rBlock2, AL, winSize, genLand, model, cnn_scores, rc, rmz, spliceD)
         numLoc[0] = (numLoc[0]*numLoc[1] + len(rBlock)) / (numLoc[1]+1)
         numLoc[1] = numLoc[1] + 1
 
     os.remove(tempFile) #Removing old temp
     AL.close()
     
     return numLoc
+
+
+#Class to speed up tensorflow prediction
+#https://micwurm.medium.com/using-tensorflow-lite-to-speed-up-predictions-a3954886eb98
+class LiteModel:
+    @classmethod
+    def from_file(cls, model_path):
+        return LiteModel(tf.lite.Interpreter(model_path=model_path))
+    
+    @classmethod
+    def from_keras_model(cls, kmodel):
+        converter = tf.lite.TFLiteConverter.from_keras_model(kmodel)
+        tflite_model = converter.convert()
+        return LiteModel(tf.lite.Interpreter(model_content=tflite_model))
+    
+    def __init__(self, interpreter):
+        self.interpreter = interpreter
+        self.interpreter.allocate_tensors()
+        input_det = self.interpreter.get_input_details()[0]
+        output_det = self.interpreter.get_output_details()[0]
+        self.input_index = input_det["index"]
+        self.output_index = output_det["index"]
+        self.input_shape = input_det["shape"]
+        self.output_shape = output_det["shape"]
+        self.input_dtype = input_det["dtype"]
+        self.output_dtype = output_det["dtype"]
+        
+    def predict(self, inp):
+        inp = inp.astype(self.input_dtype)
+        count = inp.shape[0]
+        out = np.zeros((count, self.output_shape[1]), dtype=self.output_dtype)
+        for i in range(count):
+            self.interpreter.set_tensor(self.input_index, inp[i:i+1])
+            self.interpreter.invoke()
+            out[i] = self.interpreter.get_tensor(self.output_index)[0]
+        return out
+    
+    def predict_single(self, inp):
+        inp = np.array([inp], dtype=self.input_dtype)
+        self.interpreter.set_tensor(self.input_index, inp)
+        self.interpreter.invoke()
+        out = self.interpreter.get_tensor(self.output_index)
+        return out[0]
+
+
```

### Comparing `bio-allo-1.0.5/Allo/mixed.h5` & `bio_allo-1.1.0/Allo/mixed.h5`

 * *Files identical despite different names*

### Comparing `bio-allo-1.0.5/Allo/mixed.json` & `bio_allo-1.1.0/Allo/mixed.json`

 * *Files identical despite different names*

### Comparing `bio-allo-1.0.5/Allo/narrow.h5` & `bio_allo-1.1.0/Allo/narrow.h5`

 * *Files identical despite different names*

### Comparing `bio-allo-1.0.5/Allo/narrow.json` & `bio_allo-1.1.0/Allo/narrow.json`

 * *Files identical despite different names*

### Comparing `bio-allo-1.0.5/Allo/predictPeak.py` & `bio_allo-1.1.0/Allo/predictPeak.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 #Lexi Morrissey, Mahony Lab @ Pennsylvania State University
-#Last updated 03.01.2023
 #Contains method for predicting whether area should receive multimapped reads via pre-trained CNN in Allo.
 
 import os
-import numpy as np
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 import tensorflow as tf
 from tensorflow import keras
 from tensorflow.keras.models import load_model, Model
 import os
 tf.config.run_functions_eagerly(False)
 import math
+import sys
+import numpy as np
 
 
 def predictNN(counts, winSize, model):
     pic = np.zeros((100, 100), float)
     if sum(counts) == 0:
         pred = model(pic.reshape(-1,100,100), training=False)
         return pred.numpy()[0][0]
@@ -24,23 +24,22 @@
     binned = []
     #Binning
     for i in range (0,binTotal):
         position = i*binSize
         if i == binTotal-1:
             binned.append(np.sum(counts[position:len(counts)]))
         else:
-            binned.append(np.sum(counts[position:position+5]))
+            binned.append(np.sum(counts[position:position+binSize]))
   
     binned = (99*(binned - np.min(binned))/np.ptp(binned)).astype(int) 
     for i in range(0,len(binned)):
         pic[binned[i],i] = 1
-        
+    pred = model.predict(pic.reshape(-1,100,100)) 
     try:
-        pred = model(pic.reshape(-1,100,100), training=False)
-        return pred.numpy()[0][0]
+        #pred = model(pic.reshape(-1,100,100), training=False)
+        pred = model.predict(pic.reshape(-1,100,100))
+        #return pred.numpy()[0][0]
+        return pred[0][0]
 
     except:
-        print("Could not predict with Tensorflow model :( Allo was written with Tensorflow version 2.11")
+        print("Could not predict with Tensorflow model :( Allo was written with Tensorflow version 2.11", flush=True)
         sys.exit(0)
-
-
-
```

### Comparing `bio-allo-1.0.5/LICENSE.txt` & `bio_allo-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

