# Comparing `tmp/pybio-0.3.6.tar.gz` & `tmp/pybio-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybio-0.3.6.tar", last modified: Wed Apr 26 11:02:01 2023, max compression
+gzip compressed data, was "pybio-0.3.7.tar", last modified: Thu May 25 13:59:57 2023, max compression
```

## Comparing `pybio-0.3.6.tar` & `pybio-0.3.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.891271 pybio-0.3.6/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-04-26 11:02:01.890771 pybio-0.3.6/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     8626 2023-04-26 07:30:50.000000 pybio-0.3.6/README.md
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.854579 pybio-0.3.6/pybio/
--rw-rw-r--   0 rotg     (2023757) games       (20)     7792 2023-04-26 10:49:44.000000 pybio-0.3.6/pybio/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.861527 pybio-0.3.6/pybio/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2060 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.863365 pybio-0.3.6/pybio/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    26823 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/core/genomes.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.876113 pybio-0.3.6/pybio/data/
--rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bam.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bedgraph.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Bedgraph2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Fasta.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Fastq.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gene.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/GeneFeature.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gff3.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Gtf.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Sequence.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Sissrs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/TabReader.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/Wig.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/data/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.877376 pybio-0.3.6/pybio/expression/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/expression/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.882805 pybio-0.3.6/pybio/map/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/STAR.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/bowtie.py
--rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/nano.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/map/sege.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.885662 pybio-0.3.6/pybio/maths/
--rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/pstat.py
--rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/maths/stats.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.887907 pybio-0.3.6/pybio/path/
--rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/path/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5203 2023-04-26 10:51:08.000000 pybio-0.3.6/pybio/pybio
--rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.6/pybio/pybio.config.example
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.888689 pybio-0.3.6/pybio/sequence/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/sequence/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.889739 pybio-0.3.6/pybio/utils/
--rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.6/pybio/utils/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:01:54.000000 pybio-0.3.6/pybio/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:02:01.860600 pybio-0.3.6/pybio.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-04-26 11:02:01.856244 pybio-0.3.6/pybio.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-04-26 11:02:01.856810 pybio-0.3.6/pybio.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 11:02:01.857955 pybio-0.3.6/pybio.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.6/pybio.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-04-26 11:02:01.860144 pybio-0.3.6/pybio.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:02:01.860911 pybio-0.3.6/pybio.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-26 11:02:01.891362 pybio-0.3.6/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.6/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.410450 pybio-0.3.7/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-05-25 13:59:57.410012 pybio-0.3.7/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8626 2023-04-28 08:19:03.000000 pybio-0.3.7/README.md
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.221534 pybio-0.3.7/pybio/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     7814 2023-05-03 14:56:57.000000 pybio-0.3.7/pybio/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.224819 pybio-0.3.7/pybio/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1397 2023-05-16 14:13:33.000000 pybio-0.3.7/pybio/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.226498 pybio-0.3.7/pybio/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)       98 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    27779 2023-05-11 11:48:32.000000 pybio-0.3.7/pybio/core/genomes.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.302214 pybio-0.3.7/pybio/data/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      877 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Bam.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16391 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Bedgraph.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     4675 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Bedgraph2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1912 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Fasta.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1244 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Fastq.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1591 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Gene.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      177 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/GeneFeature.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3238 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Gff3.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2777 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Gtf.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      186 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Sequence.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      906 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Sissrs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      956 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/TabReader.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2019 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/Wig.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2168 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/data/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.302839 pybio-0.3.7/pybio/expression/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8831 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/expression/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.322152 pybio-0.3.7/pybio/map/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2257 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/map/STAR.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      131 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/map/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1438 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/map/bowtie.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)      580 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/map/nano.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/map/sege.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.333027 pybio-0.3.7/pybio/maths/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      974 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/maths/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37335 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/maths/pstat.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)   151400 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/maths/stats.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.361296 pybio-0.3.7/pybio/path/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      347 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/path/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     9827 2023-05-16 07:47:25.000000 pybio-0.3.7/pybio/pybio
+-rw-rw-r--   0 rotg     (2023757) games       (20)      100 2023-04-26 07:30:50.000000 pybio-0.3.7/pybio/pybio.config.example
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.362774 pybio-0.3.7/pybio/sequence/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5566 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/sequence/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.392450 pybio-0.3.7/pybio/utils/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    10199 2023-04-17 06:24:09.000000 pybio-0.3.7/pybio/utils/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-05-25 13:59:35.000000 pybio-0.3.7/pybio/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:59:57.224047 pybio-0.3.7/pybio.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8857 2023-05-25 13:59:57.221917 pybio-0.3.7/pybio.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      892 2023-05-25 13:59:57.222197 pybio-0.3.7/pybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-25 13:59:57.222524 pybio-0.3.7/pybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-18 08:10:15.000000 pybio-0.3.7/pybio.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       32 2023-05-25 13:59:57.223487 pybio-0.3.7/pybio.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-05-25 13:59:57.224127 pybio-0.3.7/pybio.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-05-25 13:59:57.410583 pybio-0.3.7/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)      949 2023-04-17 08:00:52.000000 pybio-0.3.7/setup.py
```

### Comparing `pybio-0.3.6/PKG-INFO` & `pybio-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.6
+Version: 0.3.7
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pybio-0.3.6/README.md` & `pybio-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/__init__.py` & `pybio-0.3.7/pybio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     else:
         genomes_ready = {}
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("assembly", False)
     genomes_ready.setdefault(species, {}).setdefault(genome_version, {}).setdefault("annotation", False)
     if pybio.utils.is_tool("STAR") and not args.nostar:
         star_folder = os.path.join(pybio.config.genomes_folder, f"{species}.assembly.{genome_version}.star")
         if not genomes_ready.get(species, {}).get(genome_version, {}).get("STAR", False) or not os.path.exists(star_folder):
-            return_code = pybio.core.genomes.star_index(species, genome_version)
+            return_code = pybio.core.genomes.star_index(species, genome_version, threads=args.threads)
             if return_code==0:
                 genomes_ready[species][genome_version]["STAR"] = True
             else:
                 genomes_ready[species][genome_version]["STAR"] = False
         else:
             print(f"[pybio genome] STAR index ready at {pybio.config.genomes_folder}/{species}.assembly.{genome_version}.star")
```

### Comparing `pybio-0.3.6/pybio/config/__init__.py` & `pybio-0.3.7/pybio/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,33 @@
 import os
 import sys
 
-def init():
-    config_module = sys.modules[__name__]
-    pybio_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
-    config_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config"))
-    config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
-    if not os.path.exists(config_file):
-        print("Please first check configuration parameters.")
-        change()
-        sys.exit(1)
-    config_lines = open(config_file).readlines()
-    for cline in config_lines:
-        if cline.startswith("#"):
-            continue
-        k, v = cline.split("=")
-        if k.find("folder")!=-1:
-            if not v.startswith("/"):
-                v = "\"" + os.path.join(pybio_folder, eval(v)) + "\""
-        setattr(config_module, k, eval(v))
-
-def change(genomes_folder=None):
+def init(genomes_folder=None):
     config_module = sys.modules[__name__]
     pybio_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
     config_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config"))
     config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
     if not os.path.exists(config_file):
+        config_example_file = os.path.abspath(os.path.join(pybio_folder, "pybio.config.example"))
         os.system(f"cp {config_example_file} {config_file}")
     config_lines = open(config_file).readlines()
-    print(f"Note: you can specify absolute or relative paths.\nRelative paths are relative to: {pybio_folder}")
-    print()
     new_config = []
     for cline in config_lines:
         if cline.startswith("#"):
             continue
         k, v = cline.split("=")
-        v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
-        v = os.path.expanduser(v)
         if k=="genomes_folder" and genomes_folder!=None:
             v = genomes_folder
-        else:
-            v = input(f"{k} [{v}]: ") or v
+        v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
         v = os.path.expanduser(v)
-        new_config.append((k, str(v)))
+        if k.find("folder")!=-1:
+            if not v.startswith("/"):
+                v = "\"" + os.path.join(pybio_folder, eval(v)) + "\""
         setattr(config_module, k, v)
-    f = open(config_file, "wt")
-    for (k, v) in new_config:
-        f.write(f"{k}=\"{v}\"\n")
-    f.close()
+        new_config.append((k, str(v)))
+    if genomes_folder!=None:
+        f = open(config_file, "wt")
+        for (k, v) in new_config:
+            f.write(f"{k}=\"{v}\"\n")
+        f.close()
+        print("[pybio] Pybio genome folder changed to '{genomes_folder}'")
+
```

### Comparing `pybio-0.3.6/pybio/core/genomes.py` & `pybio-0.3.7/pybio/core/genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,17 @@
 
 def seq_direct(species, chr, strand, start, stop, flank="N", genome_version=None):
     """
     Returns chromosome sequence from [start..stop]
     Note: negative strand returns reverse complement; coordinates are 0-based, left+right inclusive; start must be < stop;
     """
     if genome_version==None:
-        genome_version = pybio.config.ensembl_version_latest
+        genome_version = pybio.core.genomes.species_db.get(species, {}).get("genome_version", None)
+    if genome_version==None:
+        return ""
     if start>stop:
         start, stop = stop, start
     assert(start<=stop)
     seq = ""
     if start<0:
         seq = flank * abs(start)
     start = max(0, start) # start can only be non-negative
@@ -284,51 +286,69 @@
     ensembl_version = ensembl_version.replace("genomes", "")
 
     ftp_address = providers_ftp[species_db[species]["provider"]]
     subfolder = species_db[species]["provider_subfolder"]
     if subfolder!="":
         ftp_address = f"{ftp_address}/{subfolder}"
 
-    # first, try primary assembly
-    fasta_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.chr.gtf.gz"
+    # prepare GFF3 download
+    gff3_url = f"{ftp_address}/release-{ensembl_version}/gff3/{species}/{species_capital}.{assembly}.{ensembl_version}.chr.gff3.gz"
     # no? download the toplevel
-    if not url_exists(fasta_url):
-        fasta_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.gtf.gz"
-
+    if not url_exists(gff3_url):
+        gff3_url = f"{ftp_address}/release-{ensembl_version}/gff3/{species}/{species_capital}.{assembly}.{ensembl_version}.gff3.gz"
     script = """
 cd {gdir}
 rm {species}.annotation.{genome_version}/* >/dev/null 2>&1
 mkdir {species}.annotation.{genome_version} >/dev/null 2>&1
 cd {species}.annotation.{genome_version}
 # https://www.biostars.org/p/279235/#279238
-wget {fasta_url} -O {species}.gtf.gz
+wget {gff3_url} -O {species}.gff3.gz
+"""
+    # download GFF3
+    print(f"[pybio.core.genomes] download annotation GFF3 for {species}.{genome_version}")
+    command = script.format(gff3_url=gff3_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
+    print(command)
+    os.system(command)
+
+    # prepare GTF download
+    gtf_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.chr.gtf.gz"
+    # no? download the toplevel
+    if not url_exists(gtf_url):
+        gtf_url = f"{ftp_address}/release-{ensembl_version}/gtf/{species}/{species_capital}.{assembly}.{ensembl_version}.gtf.gz"
+
+    script = """
+cd {gdir}
+mkdir {species}.annotation.{genome_version} >/dev/null 2>&1
+cd {species}.annotation.{genome_version}
+# https://www.biostars.org/p/279235/#279238
+wget {gtf_url} -O {species}.gtf.gz
 """
     # download GTF
     print(f"[pybio.core.genomes] download annotation GTF for {species}.{genome_version}")
-    command = script.format(fasta_url=fasta_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
+    command = script.format(gtf_url=gtf_url, gdir=pybio.config.genomes_folder, species=species, genome_version=genome_version)
     return os.system(command)
 
-def star_index(species, genome_version):
+def star_index(species, genome_version, threads=1):
     species_capital = species.capitalize()
     assembly = species_db[species]["assembly"]
     ensembl_version = genome_version.replace("ensembl", "")
     ensembl_version = ensembl_version.replace("genomes", "")
     script = """
 cd {gdir}
 rm {species}.assembly.{genome_version}.star/* >/dev/null 2>&1
 mkdir {species}.assembly.{genome_version}.star >/dev/null 2>&1
 cd {species}.assembly.{genome_version}.star
 gunzip ../{species}.annotation.{genome_version}/{species}.gtf.gz
-STAR --runMode genomeGenerate --genomeSAindexNbases {genomeSAindexNbases} --genomeDir ../{species}.assembly.{genome_version}.star --genomeFastaFiles ../{species}.assembly.{genome_version}/{species}.fasta --runThreadN 4 --sjdbGTFfile ../{species}.annotation.{genome_version}/{species}.gtf
+STAR --runMode genomeGenerate --genomeSAindexNbases {genomeSAindexNbases} --genomeDir ../{species}.assembly.{genome_version}.star --genomeFastaFiles ../{species}.assembly.{genome_version}/{species}.fasta --runThreadN {threads} --sjdbGTFfile ../{species}.annotation.{genome_version}/{species}.gtf
 gzip -f ../{species}.annotation.{genome_version}/{species}.gtf
 """
     fasta_file = f"{pybio.config.genomes_folder}/{species}.assembly.{genome_version}/{species}.fasta"
     fasta_size = os.path.getsize(fasta_file)
     genomeSAindexNbases = int(min(14, math.log(fasta_size, 2)/2 - 1))
-    command = script.format(genomeSAindexNbases=genomeSAindexNbases, gdir=pybio.config.genomes_folder, species=species, species_capital=species_capital, assembly=assembly, ensembl_version=ensembl_version, genome_version=genome_version)
+    command = script.format(threads=threads, genomeSAindexNbases=genomeSAindexNbases, gdir=pybio.config.genomes_folder, species=species, species_capital=species_capital, assembly=assembly, ensembl_version=ensembl_version, genome_version=genome_version)
     return os.system(command)
 
 def salmon_index(species, genome_version):
     species_capital = species.capitalize()
     assembly = species_db[species]["assembly"]
     ensembl_version = genome_version.replace("ensembl", "")
     ensembl_version = ensembl_version.replace("genomes", "")
```

### Comparing `pybio-0.3.6/pybio/data/Bam.py` & `pybio-0.3.7/pybio/data/Bam.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Bedgraph.py` & `pybio-0.3.7/pybio/data/Bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Bedgraph2.py` & `pybio-0.3.7/pybio/data/Bedgraph2.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Fasta.py` & `pybio-0.3.7/pybio/data/Fasta.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Fastq.py` & `pybio-0.3.7/pybio/data/Fastq.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Gene.py` & `pybio-0.3.7/pybio/data/Gene.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Gff3.py` & `pybio-0.3.7/pybio/data/Gff3.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Gtf.py` & `pybio-0.3.7/pybio/data/Gtf.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Sissrs.py` & `pybio-0.3.7/pybio/data/Sissrs.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/TabReader.py` & `pybio-0.3.7/pybio/data/TabReader.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/Wig.py` & `pybio-0.3.7/pybio/data/Wig.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/data/__init__.py` & `pybio-0.3.7/pybio/data/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/expression/__init__.py` & `pybio-0.3.7/pybio/expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/map/STAR.py` & `pybio-0.3.7/pybio/map/STAR.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/map/bowtie.py` & `pybio-0.3.7/pybio/map/bowtie.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/map/nano.py` & `pybio-0.3.7/pybio/map/nano.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/map/sege.py` & `pybio-0.3.7/pybio/map/sege.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/maths/__init__.py` & `pybio-0.3.7/pybio/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/maths/pstat.py` & `pybio-0.3.7/pybio/maths/pstat.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/maths/stats.py` & `pybio-0.3.7/pybio/maths/stats.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/sequence/__init__.py` & `pybio-0.3.7/pybio/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio/utils/__init__.py` & `pybio-0.3.7/pybio/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/pybio.egg-info/PKG-INFO` & `pybio-0.3.7/pybio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybio
-Version: 0.3.6
+Version: 0.3.7
 Summary: pybio genomics
 Home-page: https://github.com/grexor/pybio
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: pybio,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `pybio-0.3.6/pybio.egg-info/SOURCES.txt` & `pybio-0.3.7/pybio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybio-0.3.6/setup.py` & `pybio-0.3.7/setup.py`

 * *Files identical despite different names*

