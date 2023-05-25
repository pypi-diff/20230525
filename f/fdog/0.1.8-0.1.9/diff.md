# Comparing `tmp/fdog-0.1.8.tar.gz` & `tmp/fdog-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdog-0.1.8.tar", last modified: Tue Feb 14 11:56:00 2023, max compression
+gzip compressed data, was "fdog-0.1.9.tar", last modified: Fri Feb 17 13:38:30 2023, max compression
```

## Comparing `fdog-0.1.8.tar` & `fdog-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:56:00.674565 fdog-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-14 11:47:51.000000 fdog-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-14 11:47:51.000000 fdog-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-02-14 11:56:00.674565 fdog-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-02-14 11:47:51.000000 fdog-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:56:00.670565 fdog-0.1.8/fdog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/addTaxa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5476 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/addTaxon.py
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/checkData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:56:00.670565 fdog-0.1.8/fdog/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/data/conda_requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/data/dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/data/infile.fa
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:56:00.674565 fdog-0.1.8/fdog/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/addtaxon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/corecompile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/fas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/orthosearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/libs/zzz.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/mergeOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/removefDog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23154 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/runMulti.py
--rw-r--r--   0 runner    (1001) docker     (123)    16015 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/runSingle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/setPaths.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/setupfDog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-02-14 11:47:51.000000 fdog-0.1.8/fdog/showTaxa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 11:56:00.670565 fdog-0.1.8/fdog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-14 11:56:00.000000 fdog-0.1.8/fdog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 11:56:00.674565 fdog-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-02-14 11:47:51.000000 fdog-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:38:30.347277 fdog-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-17 13:29:52.000000 fdog-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-17 13:29:52.000000 fdog-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-02-17 13:38:30.347277 fdog-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-02-17 13:29:52.000000 fdog-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:38:30.343277 fdog-0.1.9/fdog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/addTaxa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5476 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/addTaxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/checkData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:38:30.343277 fdog-0.1.9/fdog/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/data/conda_requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/data/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/data/infile.fa
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:38:30.343277 fdog-0.1.9/fdog/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/addtaxon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18969 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/corecompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/fas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12422 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/orthosearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/libs/zzz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/mergeOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/removefDog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23154 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/runMulti.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16015 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/runSingle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/setPaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/setupfDog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-02-17 13:29:52.000000 fdog-0.1.9/fdog/showTaxa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 13:38:30.343277 fdog-0.1.9/fdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-17 13:38:30.000000 fdog-0.1.9/fdog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 13:38:30.347277 fdog-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-02-17 13:29:52.000000 fdog-0.1.9/setup.py
```

### Comparing `fdog-0.1.8/LICENSE` & `fdog-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/PKG-INFO` & `fdog-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdog
-Version: 0.1.8
+Version: 0.1.9
 Summary: Feature-aware Directed OrtholoG search tool
 Home-page: https://github.com/BIONF/fDOG
 Author: Vinh Tran
 Author-email: tran@bio.uni-frankfurt.de
 License: GPL-3.0
 Description: # fDOG - Feature-aware Directed OrtholoG search
         [![PyPI version](https://badge.fury.io/py/fdog.svg)](https://pypi.org/project/fdog/)
```

### Comparing `fdog-0.1.8/README.md` & `fdog-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/addTaxa.py` & `fdog-0.1.9/fdog/addTaxa.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/addTaxon.py` & `fdog-0.1.9/fdog/addTaxon.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/checkData.py` & `fdog-0.1.9/fdog/checkData.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/addtaxon.py` & `fdog-0.1.9/fdog/libs/addtaxon.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/alignment.py` & `fdog-0.1.9/fdog/libs/alignment.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/blast.py` & `fdog-0.1.9/fdog/libs/blast.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/corecompile.py` & `fdog-0.1.9/fdog/libs/corecompile.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
             flag_node = 0
             for leaf in leaves:
                 if flag_node == 1:
                     break
                 if not leaf == refspec_id and \
                         not leaf in added_taxa and \
                         not leaf in ignored_taxa:
+                    output_fn.print_debug(debugCore, '','')
                     output_fn.print_debug(
                         debugCore, '',
                         'Leaf %s - %s' % (leaf, tax_ids[leaf]))
                     if len(curr_cand) > 0 and \
                             not curr_cand in node_dict[node_id]:
                         next_node = True
                         output_fn.print_debug(
```

### Comparing `fdog-0.1.8/fdog/libs/fas.py` & `fdog-0.1.9/fdog/libs/fas.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/fasta.py` & `fdog-0.1.9/fdog/libs/fasta.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/hmm.py` & `fdog-0.1.9/fdog/libs/hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,19 +64,20 @@
             if best_domain_score >= cutoff:
                 if best_domain_score not in score_dict:
                     score_dict[best_domain_score] = [best_domain_hit]
                 else:
                     score_dict[best_domain_score].append(best_domain_hit)
     output_fn.print_debug(debug, 'All HMM hits', ori_hits)
     hmm_cand = {}
-    n = 1
+    n = 0
     score_dict = {
         key:val for key, val in score_dict.items() \
         if key >= cutoff
     }
+    output_fn.print_debug(debug, 'Candidate HMM hits', score_dict)
     for score in sorted(score_dict, reverse = True):
         if n < hitLimit:
             for id in score_dict[score]:
                 hmm_cand[id] = score
                 n += 1
     return(hmm_cand)
```

### Comparing `fdog-0.1.8/fdog/libs/orthosearch.py` & `fdog-0.1.9/fdog/libs/orthosearch.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/output.py` & `fdog-0.1.9/fdog/libs/output.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/preparation.py` & `fdog-0.1.9/fdog/libs/preparation.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/tree.py` & `fdog-0.1.9/fdog/libs/tree.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/libs/zzz.py` & `fdog-0.1.9/fdog/libs/zzz.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/mergeOutput.py` & `fdog-0.1.9/fdog/mergeOutput.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/removefDog.py` & `fdog-0.1.9/fdog/removefDog.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/runMulti.py` & `fdog-0.1.9/fdog/runMulti.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/runSingle.py` & `fdog-0.1.9/fdog/runSingle.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/setPaths.py` & `fdog-0.1.9/fdog/setPaths.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/setupfDog.py` & `fdog-0.1.9/fdog/setupfDog.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog/showTaxa.py` & `fdog-0.1.9/fdog/showTaxa.py`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/fdog.egg-info/PKG-INFO` & `fdog-0.1.9/fdog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdog
-Version: 0.1.8
+Version: 0.1.9
 Summary: Feature-aware Directed OrtholoG search tool
 Home-page: https://github.com/BIONF/fDOG
 Author: Vinh Tran
 Author-email: tran@bio.uni-frankfurt.de
 License: GPL-3.0
 Description: # fDOG - Feature-aware Directed OrtholoG search
         [![PyPI version](https://badge.fury.io/py/fdog.svg)](https://pypi.org/project/fdog/)
```

### Comparing `fdog-0.1.8/fdog.egg-info/SOURCES.txt` & `fdog-0.1.9/fdog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdog-0.1.8/setup.py` & `fdog-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as input:
     long_description = input.read()
 
 setup(
     name="fdog",
-    version="0.1.8",
+    version="0.1.9",
     python_requires='>=3.7.0',
     description="Feature-aware Directed OrtholoG search tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vinh Tran",
     author_email="tran@bio.uni-frankfurt.de",
     url="https://github.com/BIONF/fDOG",
```

