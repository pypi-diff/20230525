# Comparing `tmp/ds4ml-0.3.3.tar.gz` & `tmp/ds4ml-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds4ml-0.3.3.tar", last modified: Mon Apr 17 02:06:27 2023, max compression
+gzip compressed data, was "ds4ml-0.3.4.tar", last modified: Thu May 25 05:07:44 2023, max compression
```

## Comparing `ds4ml-0.3.3.tar` & `ds4ml-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.261612 ds4ml-0.3.3/
--rw-r--r--   0 i076744    (501) staff       (20)    11356 2020-06-08 02:24:17.000000 ds4ml-0.3.3/LICENSE
--rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-04-17 02:06:27.261325 ds4ml-0.3.3/PKG-INFO
--rw-r--r--   0 i076744    (501) staff       (20)     9222 2022-11-17 08:39:17.000000 ds4ml-0.3.3/README.md
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.236232 ds4ml-0.3.3/ds4ml/
--rw-r--r--   0 i076744    (501) staff       (20)      109 2020-12-02 02:30:48.000000 ds4ml-0.3.3/ds4ml/__init__.py
--rw-r--r--   0 i076744    (501) staff       (20)      296 2023-04-17 01:32:01.000000 ds4ml-0.3.3/ds4ml/__version__.py
--rw-r--r--   0 i076744    (501) staff       (20)    18119 2023-03-29 05:59:37.000000 ds4ml-0.3.3/ds4ml/attribute.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.256417 ds4ml-0.3.3/ds4ml/command/
--rw-r--r--   0 i076744    (501) staff       (20)        0 2020-05-14 09:10:36.000000 ds4ml-0.3.3/ds4ml/command/__init__.py
--rw-r--r--   0 i076744    (501) staff       (20)     3645 2020-12-07 06:14:20.000000 ds4ml-0.3.3/ds4ml/command/evaluate.py
--rw-r--r--   0 i076744    (501) staff       (20)     3871 2022-11-17 08:39:17.000000 ds4ml-0.3.3/ds4ml/command/pattern.py
--rw-r--r--   0 i076744    (501) staff       (20)     1043 2020-11-30 13:10:48.000000 ds4ml-0.3.3/ds4ml/command/runtest.py
--rw-r--r--   0 i076744    (501) staff       (20)     5115 2021-02-01 02:37:59.000000 ds4ml-0.3.3/ds4ml/command/synthesize.py
--rw-r--r--   0 i076744    (501) staff       (20)    11420 2023-03-29 05:41:15.000000 ds4ml-0.3.3/ds4ml/dataset.py
--rw-r--r--   0 i076744    (501) staff       (20)    13556 2023-03-29 05:34:40.000000 ds4ml-0.3.3/ds4ml/evaluator.py
--rw-r--r--   0 i076744    (501) staff       (20)     2169 2020-12-03 08:17:26.000000 ds4ml-0.3.3/ds4ml/metrics.py
--rw-r--r--   0 i076744    (501) staff       (20)     8406 2022-07-21 03:21:38.000000 ds4ml-0.3.3/ds4ml/synthesizer.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.256891 ds4ml-0.3.3/ds4ml/template/
--rw-r--r--   0 i076744    (501) staff       (20)    10969 2020-12-01 09:36:31.000000 ds4ml-0.3.3/ds4ml/template/report.html
--rw-r--r--   0 i076744    (501) staff       (20)    15902 2023-03-29 06:01:42.000000 ds4ml-0.3.3/ds4ml/utils.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.253538 ds4ml-0.3.3/ds4ml.egg-info/
--rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/PKG-INFO
--rw-r--r--   0 i076744    (501) staff       (20)      662 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/SOURCES.txt
--rw-r--r--   0 i076744    (501) staff       (20)        1 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/dependency_links.txt
--rw-r--r--   0 i076744    (501) staff       (20)      152 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/entry_points.txt
--rw-r--r--   0 i076744    (501) staff       (20)      103 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/requires.txt
--rw-r--r--   0 i076744    (501) staff       (20)        6 2023-04-17 02:06:27.000000 ds4ml-0.3.3/ds4ml.egg-info/top_level.txt
--rw-r--r--   0 i076744    (501) staff       (20)       38 2023-04-17 02:06:27.261671 ds4ml-0.3.3/setup.cfg
--rw-r--r--   0 i076744    (501) staff       (20)     2368 2023-04-17 02:03:40.000000 ds4ml-0.3.3/setup.py
-drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-04-17 02:06:27.260848 ds4ml-0.3.3/tests/
--rw-r--r--   0 i076744    (501) staff       (20)     9383 2023-03-29 05:43:50.000000 ds4ml-0.3.3/tests/test_attribute.py
--rw-r--r--   0 i076744    (501) staff       (20)     5723 2023-03-29 05:35:15.000000 ds4ml-0.3.3/tests/test_dataset.py
--rw-r--r--   0 i076744    (501) staff       (20)     2969 2020-12-04 10:07:23.000000 ds4ml-0.3.3/tests/test_evaluator.py
--rw-r--r--   0 i076744    (501) staff       (20)     1411 2020-12-03 07:44:47.000000 ds4ml-0.3.3/tests/test_metrics.py
--rw-r--r--   0 i076744    (501) staff       (20)     2513 2022-11-17 08:39:17.000000 ds4ml-0.3.3/tests/test_synthesizer.py
--rw-r--r--   0 i076744    (501) staff       (20)     5770 2020-12-01 09:36:31.000000 ds4ml-0.3.3/tests/test_utils.py
--rw-r--r--   0 i076744    (501) staff       (20)     4843 2020-05-14 09:10:36.000000 ds4ml-0.3.3/tests/testdata.py
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.105912 ds4ml-0.3.4/
+-rw-r--r--   0 i076744    (501) staff       (20)    11356 2020-06-08 02:24:17.000000 ds4ml-0.3.4/LICENSE
+-rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-05-25 05:07:44.105514 ds4ml-0.3.4/PKG-INFO
+-rw-r--r--   0 i076744    (501) staff       (20)     9222 2022-11-17 08:39:17.000000 ds4ml-0.3.4/README.md
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.046149 ds4ml-0.3.4/ds4ml/
+-rw-r--r--   0 i076744    (501) staff       (20)      109 2020-12-02 02:30:48.000000 ds4ml-0.3.4/ds4ml/__init__.py
+-rw-r--r--   0 i076744    (501) staff       (20)      296 2023-05-25 05:04:17.000000 ds4ml-0.3.4/ds4ml/__version__.py
+-rw-r--r--   0 i076744    (501) staff       (20)    18119 2023-05-25 05:03:27.000000 ds4ml-0.3.4/ds4ml/attribute.py
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.068088 ds4ml-0.3.4/ds4ml/command/
+-rw-r--r--   0 i076744    (501) staff       (20)        0 2020-05-14 09:10:36.000000 ds4ml-0.3.4/ds4ml/command/__init__.py
+-rw-r--r--   0 i076744    (501) staff       (20)     3645 2020-12-07 06:14:20.000000 ds4ml-0.3.4/ds4ml/command/evaluate.py
+-rw-r--r--   0 i076744    (501) staff       (20)     3871 2022-11-17 08:39:17.000000 ds4ml-0.3.4/ds4ml/command/pattern.py
+-rw-r--r--   0 i076744    (501) staff       (20)     1043 2020-11-30 13:10:48.000000 ds4ml-0.3.4/ds4ml/command/runtest.py
+-rw-r--r--   0 i076744    (501) staff       (20)     5115 2021-02-01 02:37:59.000000 ds4ml-0.3.4/ds4ml/command/synthesize.py
+-rw-r--r--   0 i076744    (501) staff       (20)    11225 2023-05-24 08:19:39.000000 ds4ml-0.3.4/ds4ml/dataset.py
+-rw-r--r--   0 i076744    (501) staff       (20)    13556 2023-03-29 05:34:40.000000 ds4ml-0.3.4/ds4ml/evaluator.py
+-rw-r--r--   0 i076744    (501) staff       (20)     2169 2020-12-03 08:17:26.000000 ds4ml-0.3.4/ds4ml/metrics.py
+-rw-r--r--   0 i076744    (501) staff       (20)     8406 2023-05-24 23:07:17.000000 ds4ml-0.3.4/ds4ml/synthesizer.py
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.075742 ds4ml-0.3.4/ds4ml/template/
+-rw-r--r--   0 i076744    (501) staff       (20)    10969 2020-12-01 09:36:31.000000 ds4ml-0.3.4/ds4ml/template/report.html
+-rw-r--r--   0 i076744    (501) staff       (20)    15902 2023-05-25 05:03:33.000000 ds4ml-0.3.4/ds4ml/utils.py
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.050220 ds4ml-0.3.4/ds4ml.egg-info/
+-rw-r--r--   0 i076744    (501) staff       (20)     1387 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/PKG-INFO
+-rw-r--r--   0 i076744    (501) staff       (20)      662 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 i076744    (501) staff       (20)        1 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 i076744    (501) staff       (20)      152 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/entry_points.txt
+-rw-r--r--   0 i076744    (501) staff       (20)      103 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/requires.txt
+-rw-r--r--   0 i076744    (501) staff       (20)        6 2023-05-25 05:07:43.000000 ds4ml-0.3.4/ds4ml.egg-info/top_level.txt
+-rw-r--r--   0 i076744    (501) staff       (20)       38 2023-05-25 05:07:44.105967 ds4ml-0.3.4/setup.cfg
+-rw-r--r--   0 i076744    (501) staff       (20)     2368 2023-04-17 02:03:40.000000 ds4ml-0.3.4/setup.py
+drwxr-xr-x   0 i076744    (501) staff       (20)        0 2023-05-25 05:07:44.101615 ds4ml-0.3.4/tests/
+-rw-r--r--   0 i076744    (501) staff       (20)     9383 2023-03-29 05:43:50.000000 ds4ml-0.3.4/tests/test_attribute.py
+-rw-r--r--   0 i076744    (501) staff       (20)     5723 2023-05-25 04:12:19.000000 ds4ml-0.3.4/tests/test_dataset.py
+-rw-r--r--   0 i076744    (501) staff       (20)     2969 2020-12-04 10:07:23.000000 ds4ml-0.3.4/tests/test_evaluator.py
+-rw-r--r--   0 i076744    (501) staff       (20)     1411 2020-12-03 07:44:47.000000 ds4ml-0.3.4/tests/test_metrics.py
+-rw-r--r--   0 i076744    (501) staff       (20)     2513 2022-11-17 08:39:17.000000 ds4ml-0.3.4/tests/test_synthesizer.py
+-rw-r--r--   0 i076744    (501) staff       (20)     5770 2023-05-23 21:44:57.000000 ds4ml-0.3.4/tests/test_utils.py
+-rw-r--r--   0 i076744    (501) staff       (20)     4843 2020-05-14 09:10:36.000000 ds4ml-0.3.4/tests/testdata.py
```

### Comparing `ds4ml-0.3.3/LICENSE` & `ds4ml-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/PKG-INFO` & `ds4ml-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4ml
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for data synthesis and evaluation
 Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
 Maintainer: Yan Zhao
 Maintainer-email: yan.zhao01@sap.com
 Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
 Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
 Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
```

### Comparing `ds4ml-0.3.3/README.md` & `ds4ml-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/attribute.py` & `ds4ml-0.3.4/ds4ml/attribute.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/command/evaluate.py` & `ds4ml-0.3.4/ds4ml/command/evaluate.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/command/pattern.py` & `ds4ml-0.3.4/ds4ml/command/pattern.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/command/runtest.py` & `ds4ml-0.3.4/ds4ml/command/runtest.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/command/synthesize.py` & `ds4ml-0.3.4/ds4ml/command/synthesize.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/dataset.py` & `ds4ml-0.3.4/ds4ml/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,23 +148,20 @@
 
         for child, parents in network:
             child_cond_prs = cond_prs[child]
             for indexes in child_cond_prs.keys():
                 prs = child_cond_prs[indexes]
                 indexes = list(eval(indexes))
 
-                filters = ''
+                df = frame
                 for parent, value in zip(parents, indexes):
-                    filters += f"(frame['{parent}']=={value})&"
-                filters = eval(filters[:-1])
-                size = frame[filters].shape[0]
-                if size:
-                    frame.loc[filters, child] = random.choice(len(prs),
-                                                              size=size,
-                                                              p=prs)
+                    df = df[df[parent] == value]
+                if df.size:
+                    frame.loc[df.index, child] = random.choice(
+                        len(prs), size=df.index.size, p=prs)
             child_prs = self[child].prs
             frame.loc[frame[child].isnull(), child] = random.choice(
                 len(child_prs), size=frame[child].isnull().sum(), p=child_prs)
         frame[frame.columns] = frame[frame.columns].astype(int)
         return frame
 
     def _construct_bayesian_network(self, epsilon=0.1, degree=2,
```

### Comparing `ds4ml-0.3.3/ds4ml/evaluator.py` & `ds4ml-0.3.4/ds4ml/evaluator.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/metrics.py` & `ds4ml-0.3.4/ds4ml/metrics.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/synthesizer.py` & `ds4ml-0.3.4/ds4ml/synthesizer.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/template/report.html` & `ds4ml-0.3.4/ds4ml/template/report.html`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml/utils.py` & `ds4ml-0.3.4/ds4ml/utils.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/ds4ml.egg-info/PKG-INFO` & `ds4ml-0.3.4/ds4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds4ml
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Python library for data synthesis and evaluation
 Home-page: https://github.com/SAP/data-synthesis-for-machine-learning
 Maintainer: Yan Zhao
 Maintainer-email: yan.zhao01@sap.com
 Project-URL: Bug Tracker, https://github.com/SAP/data-synthesis-for-machine-learning/issues
 Project-URL: Documentation, https://github.com/SAP/data-synthesis-for-machine-learning
 Project-URL: Source Code, https://github.com/SAP/data-synthesis-for-machine-learning
```

### Comparing `ds4ml-0.3.3/ds4ml.egg-info/SOURCES.txt` & `ds4ml-0.3.4/ds4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/setup.py` & `ds4ml-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_attribute.py` & `ds4ml-0.3.4/tests/test_attribute.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_dataset.py` & `ds4ml-0.3.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_evaluator.py` & `ds4ml-0.3.4/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_metrics.py` & `ds4ml-0.3.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_synthesizer.py` & `ds4ml-0.3.4/tests/test_synthesizer.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/test_utils.py` & `ds4ml-0.3.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ds4ml-0.3.3/tests/testdata.py` & `ds4ml-0.3.4/tests/testdata.py`

 * *Files identical despite different names*

