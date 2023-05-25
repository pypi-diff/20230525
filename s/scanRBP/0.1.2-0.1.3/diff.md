# Comparing `tmp/scanRBP-0.1.2.tar.gz` & `tmp/scanRBP-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanRBP-0.1.2.tar", last modified: Wed Apr 26 11:01:37 2023, max compression
+gzip compressed data, was "scanRBP-0.1.3.tar", last modified: Thu May 25 13:58:27 2023, max compression
```

## Comparing `scanRBP-0.1.2.tar` & `scanRBP-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.670941 scanRBP-0.1.2/
--rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 11:01:37.670398 scanRBP-0.1.2/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)     3640 2023-04-21 15:01:09.000000 scanRBP-0.1.2/README.md
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.665728 scanRBP-0.1.2/scanRBP/
--rw-rw-r--   0 rotg     (2023757) games       (20)      445 2023-04-26 10:50:15.000000 scanRBP-0.1.2/scanRBP/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.669051 scanRBP-0.1.2/scanRBP/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)     2072 2023-04-26 10:07:04.000000 scanRBP-0.1.2/scanRBP/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.669499 scanRBP-0.1.2/scanRBP/pwm/
--rw-rw-r--   0 rotg     (2023757) games       (20)     1732 2023-04-26 10:56:17.000000 scanRBP-0.1.2/scanRBP/pwm/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     7703 2023-04-26 10:51:01.000000 scanRBP-0.1.2/scanRBP/scanRBP
--rw-rw-r--   0 rotg     (2023757) games       (20)      104 2023-04-26 08:34:41.000000 scanRBP-0.1.2/scanRBP/scanRBP.config.example
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-04-26 11:01:30.000000 scanRBP-0.1.2/scanRBP/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-04-26 11:01:37.668515 scanRBP-0.1.2/scanRBP.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)     3972 2023-04-26 11:01:37.666288 scanRBP-0.1.2/scanRBP.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      336 2023-04-26 11:01:37.666775 scanRBP-0.1.2/scanRBP.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 11:01:37.667185 scanRBP-0.1.2/scanRBP.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-04-26 10:02:27.000000 scanRBP-0.1.2/scanRBP.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       41 2023-04-26 11:01:37.668258 scanRBP-0.1.2/scanRBP.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        8 2023-04-26 11:01:37.668621 scanRBP-0.1.2/scanRBP.egg-info/top_level.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-04-26 11:01:37.671078 scanRBP-0.1.2/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1041 2023-04-26 11:01:07.000000 scanRBP-0.1.2/setup.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.110922 scanRBP-0.1.3/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4160 2023-05-25 13:58:27.110504 scanRBP-0.1.3/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     3830 2023-05-11 12:29:25.000000 scanRBP-0.1.3/README.md
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.104206 scanRBP-0.1.3/scanRBP/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      507 2023-05-09 14:06:00.000000 scanRBP-0.1.3/scanRBP/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.108231 scanRBP-0.1.3/scanRBP/config/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1389 2023-05-16 13:54:58.000000 scanRBP-0.1.3/scanRBP/config/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.109134 scanRBP-0.1.3/scanRBP/database/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      795 2023-05-16 12:49:53.000000 scanRBP-0.1.3/scanRBP/database/__init__.py
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.109837 scanRBP-0.1.3/scanRBP/pwm/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1465 2023-05-10 10:55:50.000000 scanRBP-0.1.3/scanRBP/pwm/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     8874 2023-05-16 13:54:19.000000 scanRBP-0.1.3/scanRBP/scanRBP
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      104 2023-05-09 11:28:18.000000 scanRBP-0.1.3/scanRBP/scanRBP.config.example
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        6 2023-05-25 13:57:50.000000 scanRBP-0.1.3/scanRBP/version
+drwxrwsr-x   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        0 2023-05-25 13:58:27.107298 scanRBP-0.1.3/scanRBP.egg-info/
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     4160 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)      365 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        1 2023-05-09 11:24:46.000000 scanRBP-0.1.3/scanRBP.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       41 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)        8 2023-05-25 13:58:26.000000 scanRBP-0.1.3/scanRBP.egg-info/top_level.txt
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)       38 2023-05-25 13:58:27.111017 scanRBP-0.1.3/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) EMEA_SMR_CORE_spliceosome (2004188)     1041 2023-04-28 08:24:39.000000 scanRBP-0.1.3/setup.py
```

### Comparing `scanRBP-0.1.2/PKG-INFO` & `scanRBP-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.2
+Version: 0.1.3
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
 scanRBP loads RNA-protein binding motif PWM and computes the log-odds scores for all the loaded RBPs across a given genomic sequence + draws a heatmap of the scores.
 
-The scores can be described as follows:
+The scores can be described as follows ([biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html)):
 
-```
-Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
-```
+> Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
-```
-Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
-```
+> Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
-# Example run
+### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
 
@@ -44,46 +40,50 @@
                              (note that one protein can have several PWMs)
      -figsize "(10,20)"      Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
      -heatmap title          Make heatmap (png+pdf) with title
      -output_folder folder   Store all results to the output folder (default: current folder)
      -nonzero                All negative vector values are set to 0, not enabled by default
 ```
 
-Example runs:
+Examples:
 
 ```
 # taking a random sequence, will produce binding scores and a heatmap
 # output: example1_PWM.tab # file with log-odds vectors for all proteins for the given command line sequence
 # output: example1.png/pdf # heatmap image with clustering of protein binding vectors
 ./scanRBP AAAGCGGCGACTTATTATATCCCCATATATTATATCTTCTTCTCTTATATATAAACCAGAGATAGATGTGTGTGGTGG example1 -heatmap example1
 
 # instead of taking one single sequence, the input can be a fasta file with multiple sequences
 ./scanRBP data.fasta
 ```
 
-# Motif PWM database
+### Motif PWM database
 
 Using the mCross database of 112 RBPs from the paper:
 
 Feng H, Bao S et al.<br>
 [Modeling RNA-Binding Protein Specificity In Vivo by Precisely Registering Protein-RNA Crosslink Sites](https://www.sciencedirect.com/science/article/pii/S1097276519300929?via%3Dihub)<br>
 Molecular Cell, 2019<br>
 
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-# Additional PWM dataset
+### Additional PWM dataset
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-# CLIP dataset
+### CLIP dataset
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
 Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
+
+### Gene data
+
+Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]
```

### Comparing `scanRBP-0.1.2/README.md` & `scanRBP-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-# What is scanRBP?
+### What is scanRBP?
 
 scanRBP loads RNA-protein binding motif PWM and computes the log-odds scores for all the loaded RBPs across a given genomic sequence + draws a heatmap of the scores.
 
-The scores can be described as follows:
+The scores can be described as follows ([biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html)):
 
-```
-Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
-```
+> Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
-```
-Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
-```
+> Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
-# Example run
+### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
 
@@ -34,46 +30,50 @@
                              (note that one protein can have several PWMs)
      -figsize "(10,20)"      Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
      -heatmap title          Make heatmap (png+pdf) with title
      -output_folder folder   Store all results to the output folder (default: current folder)
      -nonzero                All negative vector values are set to 0, not enabled by default
 ```
 
-Example runs:
+Examples:
 
 ```
 # taking a random sequence, will produce binding scores and a heatmap
 # output: example1_PWM.tab # file with log-odds vectors for all proteins for the given command line sequence
 # output: example1.png/pdf # heatmap image with clustering of protein binding vectors
 ./scanRBP AAAGCGGCGACTTATTATATCCCCATATATTATATCTTCTTCTCTTATATATAAACCAGAGATAGATGTGTGTGGTGG example1 -heatmap example1
 
 # instead of taking one single sequence, the input can be a fasta file with multiple sequences
 ./scanRBP data.fasta
 ```
 
-# Motif PWM database
+### Motif PWM database
 
 Using the mCross database of 112 RBPs from the paper:
 
 Feng H, Bao S et al.<br>
 [Modeling RNA-Binding Protein Specificity In Vivo by Precisely Registering Protein-RNA Crosslink Sites](https://www.sciencedirect.com/science/article/pii/S1097276519300929?via%3Dihub)<br>
 Molecular Cell, 2019<br>
 
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-# Additional PWM dataset
+### Additional PWM dataset
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-# CLIP dataset
+### CLIP dataset
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
-Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
+Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
+
+### Gene data
+
+Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]
```

### Comparing `scanRBP-0.1.2/scanRBP/config/__init__.py` & `scanRBP-0.1.3/scanRBP/config/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,32 @@
 import os
 import sys
 
-def init():
-    config_module = sys.modules[__name__]
-    scanRBP_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
-    config_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config"))
-    config_example_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config.example"))
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
-                v = "\"" + os.path.join(scanRBP_folder, eval(v)) + "\""
-        setattr(config_module, k, eval(v))
-
-def change(data_folder=None):
+def init(data_folder=None):
     config_module = sys.modules[__name__]
     scanRBP_folder = os.path.abspath(os.path.join(os.path.abspath(__file__), "..", "..")) 
     config_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config"))
     config_example_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config.example"))
     if not os.path.exists(config_file):
+        config_example_file = os.path.abspath(os.path.join(scanRBP_folder, "scanRBP.config.example"))
         os.system(f"cp {config_example_file} {config_file}")
     config_lines = open(config_file).readlines()
-    print(f"Note: you can specify absolute or relative paths.\nRelative paths are relative to: {scanRBP_folder}")
-    print()
     new_config = []
     for cline in config_lines:
         if cline.startswith("#"):
             continue
         k, v = cline.split("=")
-        v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
-        v = os.path.expanduser(v)
         if k=="data_folder" and data_folder!=None:
             v = data_folder
-        else:
-            v = input(f"{k} [{v}]: ") or v
+        v = v.replace("\n", "").replace("\r", "").replace("\"", "").replace("'", "")
         v = os.path.expanduser(v)
-        new_config.append((k, str(v)))
+        if k.find("folder")!=-1:
+            if not v.startswith("/"):
+                v = "\"" + os.path.join(scanRBP_folder, eval(v)) + "\""
         setattr(config_module, k, v)
-    f = open(config_file, "wt")
-    for (k, v) in new_config:
-        f.write(f"{k}=\"{v}\"\n")
-    f.close()
+        new_config.append((k, str(v)))
+    if data_folder!=None:
+        f = open(config_file, "wt")
+        for (k, v) in new_config:
+            f.write(f"{k}=\"{v}\"\n")
+        f.close()
+        print(f"[scanRBP] Data folder changed to '{data_folder}'")
```

### Comparing `scanRBP-0.1.2/scanRBP/pwm/__init__.py` & `scanRBP-0.1.3/scanRBP/pwm/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 import sys
 from Bio import motifs
 import scanRBP
 
-database = {}
+pssm = {}
 
 def download_pwm():
     # PWMs not present? download
     download = False
     pwm_folder = f"{scanRBP.config.data_folder}/pwm"
     if not os.path.exists(pwm_folder):
         os.makedirs(pwm_folder)
@@ -19,28 +19,21 @@
         os.system(f"wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate -O {data_folder}/eCLIP_mCross_PWM.tgz >/dev/null 2>&1")
         os.system(f"tar xfz {data_folder}/eCLIP_mCross_PWM.tgz -C {data_folder} >/dev/null 2>&1")
         os.system(f"mv {data_folder}/eCLIP_PWM/* {data_folder}/pwm >/dev/null 2>&1")
         os.system(f"rm {data_folder}/eCLIP_PWM/* >/dev/null 2>&1")
         os.system(f"rmdir {data_folder}/eCLIP_PWM >/dev/null 2>&1")
         os.system(f"rm {data_folder}/eCLIP_mCross_PWM.tgz >/dev/null 2>&1")
 
-def init(args):
+def init():
     download_pwm()
-    if args.only_protein!=False:
-        files = glob.glob(f"{scanRBP.config.data_folder}/pwm/*{args.only_protein}*.mat")
-    else:
-        files = glob.glob(f"{scanRBP.config.data_folder}/pwm/*.00.mat")
-    if args.all_protein!=False:
-        files = files + glob.glob(f"{scanRBP.config.data_folder}/pwm/*{args.all_protein}*.mat")
-
-    for fname in files:
+    for scan_id, data in scanRBP.database.proteins.items():
+        fname = data["pwm_path"]
+        fname = os.path.join(scanRBP.config.data_folder, data["pwm_path"])
         record = motifs.parse(open(fname), "TRANSFAC", strict=False)
         try:
             motif = record[0]
             motif.pseudocounts = 3
-            pssm = motif.pwm.log_odds()
-            if motif["ID"].find("HNRNPC")!=-1:
-                continue
-            database[motif["ID"]] = pssm
+            pssm_temp = motif.pwm.log_odds()
+            pssm[scan_id] = pssm_temp
         except:
             pass
```

### Comparing `scanRBP-0.1.2/scanRBP/scanRBP` & `scanRBP-0.1.3/scanRBP/scanRBP`

 * *Files 10% similar despite different names*

```diff
@@ -15,18 +15,15 @@
 from pathlib import Path
 import pybio
 import gzip
 import scanRBP
 
 scanRBP_path = Path(__file__).parent.absolute()
 
-scanRBP.config.init()
-
 CLIP_data = {}
-#CLIP_data["tardbp"] = pybio.data.Bedgraph("CLIP_data/eCLIP_tdp43_bedgraph.bed")
 def read_CLIP():
     f = open("eCLIP_data/metadata.tsv", "rt")
     header = f.readline().replace("\r", "").replace("\n", "").split("\t")
     r = f.readline()
     while r:
         r = r.replace("\r", "").replace("\n", "").split("\t")
         data = dict(zip(header, r))
@@ -35,42 +32,41 @@
             fbed = f"eCLIP_data/{fbase}.bed"
             protein = data["Experiment target"].replace("-human", "")
             cell_type = data["Biosample term name"]
             CLIP_data[(cell_type, protein)] = pybio.data.Bed(f"CLIP_data/{fbed}")
         r = f.readline()
     f.close()
 
-help_0 = """
-Usage for single sequence: scanRBP sequence output [options]
-     * one sequence provided on the command line, generates output.png/pdf + output.tab
-
-Usage for processing FASTA file: scanRBP filename.fasta [options]
-     * one heatmap/matrix will be generated per sequence
-     * output name of the files will be sequence ids provided in the fasta file
+help_0 = """Usage: scanRBP sequence output [options]
+    * one sequence provided on the command line, generates output.png/pdf + output.tab
+
+Usage: scanRBP filename.fasta [options]
+    * one heatmap/matrix will be generated per sequence from the FASTA file
+    * output name of the files will be sequence ids provided in the fasta file
+
+Usage: scanRBP search search_term
+    * returns list of proteins available matching search_term
 
 Options:
-     -annotate               Annotate each heatmap cell with the number
-     -xlabels                Display sequence (x-labels), default False
-     -only_protein TARDBP    Only analyze binding for the specific protein / search by name
-     -all_protein TARDBP     Additionally to one motif per protein (for all proteins), also include all motifs (PWMs) for this specific protein (search by name)
-                             (note that one protein can have several PWMs)
-     -figsize "(10,20)"      Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
-     -heatmap title          Make heatmap (png+pdf) with title
-     -output_folder folder   Store all results to the output folder (default: current folder)
-     -nonzero                All negative vector values are set to 0, not enabled by default
-     -CLIP                   Use actual CLIP data, do not use PWM
+     -annotate                Annotate each heatmap cell with the number
+     -xlabels                 Display sequence (x-labels), default False
+     -protein TARDBP.K562.00  Only analyze binding for the provided protein (default: analyze binding for all proteins in scanRBP database)
+     -figsize "(10,20)"       Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
+     -heatmap title           Make heatmap (png+pdf) with title
+     -output_folder folder    Store all results to the output folder (default: current folder)
+     -nonzero                 All negative vector values are set to 0, not enabled by default
+     -CLIP                    Use actual CLIP data, do not use PWM
 """
 
 parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter, add_help=False)
 parser.add_argument('commands', help="command(s) to run", nargs='*')
 parser.add_argument("-help", "-h", "--help", action="store_true")
 parser.add_argument("-annotate", "--annotate", action="store_true", default=False)
 parser.add_argument("-xlabels", "--xlabels", action="store_true", default=False)
-parser.add_argument("-only_protein", "--only_protein", default=False)
-parser.add_argument("-all_protein", "--all_protein", default=False)
+parser.add_argument("-protein", "--protein", default=False)
 parser.add_argument("-figsize", "--figsize", default=False)
 parser.add_argument("-title", "--title", default=False)
 parser.add_argument("-matrix", "--matrix", action="store_true", default=True)
 parser.add_argument("-CLIP", "--CLIP", action="store_true", default=False)
 parser.add_argument("-nonzero", "--nonzero", action="store_true", default=False)
 parser.add_argument("-heatmap", "--heatmap", default=False)
 parser.add_argument("-output_folder", "--output_folder", default=".")
@@ -78,14 +74,26 @@
 
 args = parser.parse_args()
 
 print(f"[scanRBP] v{scanRBP.version}, https://github.com/grexor/scanRBP")
 print(f"[scanRBP] data folder: {scanRBP.config.data_folder}")
 print()
 
+# find all proteins with search
+def find_proteins(search):
+    results, results_data = [], []
+    for scan_id, data in scanRBP.database.proteins.items():
+        protein_desc_lower = data["description"].lower()
+        scan_id_lower = scan_id.lower()
+        search_lower = search.lower()
+        if scan_id_lower.find(search_lower)!=-1 or protein_desc_lower.find(search_lower)!=-1:
+            results.append(scan_id)
+            results_data.append(data)
+    return results, results_data
+
 if args.version:
     sys.exit(0)
 
 if len(args.commands) not in [1,2] or args.help:
     print(help_0)
     sys.exit(0)
 
@@ -109,27 +117,30 @@
     if strand=="-":
         heatmap_rows.reverse()
     basename = output_fname.replace(".png", "").replace(".pdf", "")
     data = pandas.DataFrame(heatmap_data, index=heatmap_columns, columns=heatmap_rows)
     data.to_csv(args.output_folder+"/"+basename+"_CLIP.tab", sep="\t")
 
 
-def process(seq, output_fname):
+def process(seq, output_fname, args):
     heatmap_data = []
     heatmap_columns = []
 
-    for motif_id, pssm in scanRBP.pwm.database.items():
+    for scan_id, pssm in scanRBP.pwm.pssm.items():
+        if args.protein: # only process a specific protein?
+            if scan_id not in args.protein:
+                continue
         scores = pssm.calculate(seq)
         scores = [x if x!=-math.inf else 0 for x in scores]
         if args.nonzero:
             scores = [x if x>=0 else 0 for x in scores]
         if len(scores)<len(seq):
             scores = scores + [0] * (len(seq)-len(scores))
         heatmap_data.append(scores)
-        heatmap_columns.append(motif_id)
+        heatmap_columns.append(scan_id)
 
     for index, data in enumerate(heatmap_data):
         assert(len(seq)==len(data))
 
     heatmap_rows = list(seq)
     basename = output_fname.replace(".png", "").replace(".pdf", "")
     data = pandas.DataFrame(heatmap_data, index=heatmap_columns, columns=heatmap_rows)
@@ -162,34 +173,52 @@
         plt.tight_layout() 
         plt.savefig(args.output_folder+"/"+basename+".png", dpi=300)
         plt.savefig(args.output_folder+"/"+basename+".pdf")
         plt.close()
 
 if len(args.commands)>0:
 
+    if args.protein:
+        args.protein, _ = find_proteins(args.protein)
+
     if args.commands[0]=="config":
         if len(args.commands)>1:
-            scanRBP.config.change(args.commands[1]) # pybio config genome_folder
-        else:
-            scanRBP.config.change() # ask for genome folder
+            scanRBP.config.init(args.commands[1])
         sys.exit(0)
 
-    scanRBP.pwm.init(args)
+    if args.commands[0]=="search":
+        if len(args.commands)>1:
+            proteins, proteins_data = find_proteins(args.commands[1])
+            if len(proteins)>0:
+                print("[scanRBP] Found proteins in the scanRBP database:")
+                table = []
+                for rec in proteins_data:
+                    table.append([rec['scan_id'], rec['protein'], rec['tissue'], rec['description']])
+                df = pandas.DataFrame(table, columns = ['scan_id', 'protein', 'tissue', 'description'])
+                print(df.to_string(index=False))
+            else:
+                print(f"[scanRBP] Found no proteins in the scanRBP database with provided seach '{args.commands[1]}'")
+        else:
+            print("[scanRBP] please provide search term (protein name)")
+        sys.exit(0)
 
     if args.commands[0].lower().endswith(".fasta") or args.commands[0].lower().endswith(".fa"):
         import pybio
         data = pybio.data.Fasta(args.commands[0])
         while data.read():
             id = data.id.lstrip(" ")
             id = id.split(" ")[0].replace("+", "plus").replace("-", "minus")
             id_records = id.replace("plus", "+").replace("minus", "-").split("_")
             chrstrand, start, stop = "_".join(id_records[:-2]), id_records[-2], id_records[-1] # chr name can have _ inside
             start, stop = int(start), int(stop)
             chr, strand = chrstrand[:-1], chrstrand[-1]
             seq = data.sequence
             # TODO
             #process_CLIP(chr, strand, start, stop, id)
-            process(seq, id)
+            process(seq, id, args)
     elif args.commands[0]=="bed":
         make_bedgraph()
     else:
-        process(args.commands[0], args.commands[1])
+        if len(args.commands)>=2:
+            process(args.commands[0], args.commands[1], args)
+        else:
+            print(help_0)
```

### Comparing `scanRBP-0.1.2/scanRBP.egg-info/PKG-INFO` & `scanRBP-0.1.3/scanRBP.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: scanRBP
-Version: 0.1.2
+Version: 0.1.3
 Summary: scanRBP: RNA-protein binding toolkit
 Home-page: https://github.com/grexor/scanRBP
 Author: Gregor Rot
 Author-email: gregor.rot@gmail.com
 Keywords: scanRBP,bioinformatics,RBP,RNA-protein binding,toolkit
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 
 
 scanRBP loads RNA-protein binding motif PWM and computes the log-odds scores for all the loaded RBPs across a given genomic sequence + draws a heatmap of the scores.
 
-The scores can be described as follows:
+The scores can be described as follows ([biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html)):
 
-```
-Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
-```
+> Here we can see positive values for symbols more frequent in the motif than in the background and negative for symbols more frequent in the background. 0.0 means that it's equally likely to see a symbol in the background and in the motif.
 
-```
-Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
-```
+> Using the background distribution and PWM with pseudo-counts added, it's easy to compute the log-odds ratios, telling us what are the log odds of a particular symbol to be coming from a motif against the background.
 
 For more information, see the [biopython docs](http://biopython.org/DIST/docs/tutorial/Tutorial.html).
 
-# Example run
+### Example run
 
 scanRBP quick start:
 
 ```
 Usage for single sequence: scanRBP sequence output [options]
      * one sequence provided on the command line, generates output.png/pdf + output.tab
 
@@ -44,46 +40,50 @@
                              (note that one protein can have several PWMs)
      -figsize "(10,20)"      Change matplotlib/seaborn figure size for the heatmap, example width=10, height=20
      -heatmap title          Make heatmap (png+pdf) with title
      -output_folder folder   Store all results to the output folder (default: current folder)
      -nonzero                All negative vector values are set to 0, not enabled by default
 ```
 
-Example runs:
+Examples:
 
 ```
 # taking a random sequence, will produce binding scores and a heatmap
 # output: example1_PWM.tab # file with log-odds vectors for all proteins for the given command line sequence
 # output: example1.png/pdf # heatmap image with clustering of protein binding vectors
 ./scanRBP AAAGCGGCGACTTATTATATCCCCATATATTATATCTTCTTCTCTTATATATAAACCAGAGATAGATGTGTGTGGTGG example1 -heatmap example1
 
 # instead of taking one single sequence, the input can be a fasta file with multiple sequences
 ./scanRBP data.fasta
 ```
 
-# Motif PWM database
+### Motif PWM database
 
 Using the mCross database of 112 RBPs from the paper:
 
 Feng H, Bao S et al.<br>
 [Modeling RNA-Binding Protein Specificity In Vivo by Precisely Registering Protein-RNA Crosslink Sites](https://www.sciencedirect.com/science/article/pii/S1097276519300929?via%3Dihub)<br>
 Molecular Cell, 2019<br>
 
 To download the PWMs:
 
 ```
 wget http://zhanglab.c2b2.columbia.edu/data/mCross/eCLIP_mCross_PWM.tgz --no-check-certificate
 tar xfz eCLIP_mCross_PWM.tgz
 ```
 
-# Additional PWM dataset
+### Additional PWM dataset
 
 https://genomebiology.biomedcentral.com/articles/10.1186/s13059-023-02913-0
 https://static-content.springer.com/esm/art%3A10.1186%2Fs13059-023-02913-0/MediaObjects/13059_2023_2913_MOESM6_ESM.txt
 
-# CLIP dataset
+### CLIP dataset
 
 bedGraph files list from:
 
 https://www.encodeproject.org/metadata/?status=released&internal_tags=ENCORE&assay_title=eCLIP&biosample_ontology.term_name=K562&biosample_ontology.term_name=HepG2&type=Experiment&files.analyses.status=released&files.preferred_default=true
 
 Any other bedGraph CLIP peak called file for a specific genome can be added to the database.
+
+### Gene data
+
+Gene metadata (names, aliases) donwloaded from https://www.ncbi.nlm.nih.gov/gene/?term=human[organism]
```

### Comparing `scanRBP-0.1.2/setup.py` & `scanRBP-0.1.3/setup.py`

 * *Files identical despite different names*

