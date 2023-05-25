# Comparing `tmp/qaoalib-0.1.8.tar.gz` & `tmp/qaoalib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qaoalib-0.1.8.tar", last modified: Thu Apr 13 12:44:37 2023, max compression
+gzip compressed data, was "qaoalib-0.1.9.tar", last modified: Thu May 25 05:07:09 2023, max compression
```

## Comparing `qaoalib-0.1.8.tar` & `qaoalib-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.631838 qaoalib-0.1.8/
--rw-rw-rw-   0        0        0     1088 2021-05-03 05:04:16.000000 qaoalib-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1443 2023-04-13 12:44:37.631838 qaoalib-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      995 2023-01-25 03:47:52.000000 qaoalib-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.425228 qaoalib-0.1.8/qaoalib/
--rw-rw-rw-   0        0        0       53 2022-04-28 07:47:51.000000 qaoalib-0.1.8/qaoalib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.465470 qaoalib-0.1.8/qaoalib/data/
--rw-rw-rw-   0        0        0        0 2023-04-04 00:41:47.000000 qaoalib-0.1.8/qaoalib/data/__init__.py
--rw-rw-rw-   0        0        0      302 2023-02-09 02:39:10.000000 qaoalib-0.1.8/qaoalib/data/graph.py
--rw-rw-rw-   0        0        0      737 2023-02-09 03:35:51.000000 qaoalib-0.1.8/qaoalib/data/result.py
--rw-rw-rw-   0        0        0      519 2021-05-11 09:10:13.000000 qaoalib-0.1.8/qaoalib/json.py
--rw-rw-rw-   0        0        0     1593 2021-05-26 01:13:30.000000 qaoalib-0.1.8/qaoalib/math.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.573816 qaoalib-0.1.8/qaoalib/qaoa/
--rw-rw-rw-   0        0        0       91 2022-06-20 06:27:33.000000 qaoalib-0.1.8/qaoalib/qaoa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.625829 qaoalib-0.1.8/qaoalib/qaoa/landscape/
--rw-rw-rw-   0        0        0      114 2021-05-11 09:10:51.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/__init__.py
--rw-rw-rw-   0        0        0     3255 2022-05-11 08:16:21.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/base.py
--rw-rw-rw-   0        0        0     2476 2022-05-11 06:23:38.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/direct_numpy.py
--rw-rw-rw-   0        0        0     1426 2022-05-11 06:25:22.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/hadamard_test.py
--rw-rw-rw-   0        0        0     1680 2022-05-11 06:24:39.000000 qaoalib-0.1.8/qaoalib/qaoa/landscape/hybrid_fast.py
--rw-rw-rw-   0        0        0     5996 2021-12-08 04:26:09.000000 qaoalib-0.1.8/qaoalib/qaoa/layerwise.py
--rw-rw-rw-   0        0        0     1686 2022-06-15 08:52:35.000000 qaoalib-0.1.8/qaoalib/qaoa/qis.py
--rw-rw-rw-   0        0        0     1787 2023-01-30 05:54:20.000000 qaoalib-0.1.8/qaoalib/qaoa/qmc.py
--rw-rw-rw-   0        0        0     1965 2023-04-04 00:01:17.000000 qaoalib-0.1.8/qaoalib/qaoa/strategy.py
--rw-rw-rw-   0        0        0     3661 2022-06-15 08:52:24.000000 qaoalib-0.1.8/qaoalib/qaoa/utils.py
--rw-rw-rw-   0        0        0     9013 2023-02-09 03:36:01.000000 qaoalib-0.1.8/qaoalib/utils.py
--rw-rw-rw-   0        0        0       21 2023-04-13 12:42:27.000000 qaoalib-0.1.8/qaoalib/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.438228 qaoalib-0.1.8/qaoalib.egg-info/
--rw-rw-rw-   0        0        0     1443 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 12:44:37.000000 qaoalib-0.1.8/qaoalib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 12:44:37.631838 qaoalib-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      922 2022-04-28 07:56:26.000000 qaoalib-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:44:37.629879 qaoalib-0.1.8/test/
--rw-rw-rw-   0        0        0       87 2021-12-08 04:31:51.000000 qaoalib-0.1.8/test/test.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.741815 qaoalib-0.1.9/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1067 2022-06-20 06:22:34.000000 qaoalib-0.1.9/LICENSE
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1388 2023-05-25 05:07:09.741815 qaoalib-0.1.9/PKG-INFO
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      954 2023-04-12 02:16:08.000000 qaoalib-0.1.9/README.md
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.737815 qaoalib-0.1.9/qaoalib/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       53 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/__init__.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      519 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/json.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1593 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/math.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.737815 qaoalib-0.1.9/qaoalib/models/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      103 2023-05-23 07:23:57.000000 qaoalib-0.1.9/qaoalib/models/__init__.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     2134 2023-05-13 06:27:58.000000 qaoalib-0.1.9/qaoalib/models/result.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.741815 qaoalib-0.1.9/qaoalib/qaoa/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       88 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/__init__.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.741815 qaoalib-0.1.9/qaoalib/qaoa/landscape/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      114 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/landscape/__init__.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     3255 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/landscape/base.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     2476 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/landscape/direct_numpy.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1426 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/landscape/hadamard_test.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1680 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/landscape/hybrid_fast.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     5996 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/layerwise.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1627 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/qis.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1736 2023-04-12 02:16:08.000000 qaoalib-0.1.9/qaoalib/qaoa/qmc.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1895 2023-04-12 02:16:08.000000 qaoalib-0.1.9/qaoalib/qaoa/strategy.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     3526 2022-06-20 06:22:34.000000 qaoalib-0.1.9/qaoalib/qaoa/utils.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     7989 2023-04-26 05:25:48.000000 qaoalib-0.1.9/qaoalib/utils.py
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       22 2023-05-25 05:05:35.000000 qaoalib-0.1.9/qaoalib/version.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.737815 qaoalib-0.1.9/qaoalib.egg-info/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)     1388 2023-05-25 05:07:09.000000 qaoalib-0.1.9/qaoalib.egg-info/PKG-INFO
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      654 2023-05-25 05:07:09.000000 qaoalib-0.1.9/qaoalib.egg-info/SOURCES.txt
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)        1 2023-05-25 05:07:09.000000 qaoalib-0.1.9/qaoalib.egg-info/dependency_links.txt
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       56 2023-05-25 05:07:09.000000 qaoalib-0.1.9/qaoalib.egg-info/requires.txt
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)        8 2023-05-25 05:07:09.000000 qaoalib-0.1.9/qaoalib.egg-info/top_level.txt
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       38 2023-05-25 05:07:09.741815 qaoalib-0.1.9/setup.cfg
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)      912 2023-04-24 08:09:58.000000 qaoalib-0.1.9/setup.py
+drwxrwxr-x   0 xenoicwyce  (1000) xenoicwyce  (1000)        0 2023-05-25 05:07:09.741815 qaoalib-0.1.9/test/
+-rw-rw-r--   0 xenoicwyce  (1000) xenoicwyce  (1000)       85 2022-06-20 06:22:34.000000 qaoalib-0.1.9/test/test.py
```

### Comparing `qaoalib-0.1.8/LICENSE` & `qaoalib-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 xenoicwyce
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 xenoicwyce
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `qaoalib-0.1.8/PKG-INFO` & `qaoalib-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: qaoalib
-Version: 0.1.8
-Summary: A package for QAOA Maxcut calculations
-Home-page: https://github.com/xenoicwyce/qaoalib
-Author: Xinwei Lee
-Author-email: xenoicwyce@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# qaoalib
-A package for QAOA Max-cut Calculations.
-
-Packages required:
-- numpy
-- networkx
-- matplotlib
-- qiskit
-
-# How to install
-You can install from the PyPI:
-```
-pip install --upgrade qaoalib
-```
-
-# Usage
-Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
-```
-import networkx as nx
-from qaoalib.qaoa import Qmc, QmcFastKron
-
-G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
-params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
-
-qmc = Qmc(G, params) # or QmcFastKron(G, params)
-qmc.run()
-print(qmc.expectation)
-```
-
-Plot landscapes of the QAOA Max-cut expectation function:
-```
-import networkx as nx
-from qaoalib.qaoa.landscape import HybridFast
-
-G = nx.fast_gnp_random_graph(10, 0.5)
-prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
-
-ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
-ins.create_grid()
-ins.show_landscape()
-```
+Metadata-Version: 2.1
+Name: qaoalib
+Version: 0.1.9
+Summary: A package for QAOA Maxcut calculations
+Home-page: https://github.com/xenoicwyce/qaoalib
+Author: Xinwei Lee
+Author-email: xenoicwyce@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# qaoalib
+A package for QAOA Max-cut Calculations.
+
+Packages required:
+- numpy
+- networkx
+- matplotlib
+- qiskit
+
+# How to install
+You can install from the PyPI:
+```
+pip install --upgrade qaoalib
+```
+
+# Usage
+Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
+```
+import networkx as nx
+from qaoalib.qaoa import Qmc, QmcFastKron
+
+G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
+params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
+
+qmc = Qmc(G, params) # or QmcFastKron(G, params)
+qmc.run()
+print(qmc.expectation)
+```
+
+Plot landscapes of the QAOA Max-cut expectation function:
+```
+import networkx as nx
+from qaoalib.qaoa.landscape import HybridFast
+
+G = nx.fast_gnp_random_graph(10, 0.5)
+prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
+
+ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
+ins.create_grid()
+ins.show_landscape()
+```
```

### Comparing `qaoalib-0.1.8/README.md` & `qaoalib-0.1.9/README.md`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# qaoalib
-A package for QAOA Max-cut Calculations.
-
-Packages required:
-- numpy
-- networkx
-- matplotlib
-- qiskit
-
-# How to install
-You can install from the PyPI:
-```
-pip install --upgrade qaoalib
-```
-
-# Usage
-Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
-```
-import networkx as nx
-from qaoalib.qaoa import Qmc, QmcFastKron
-
-G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
-params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
-
-qmc = Qmc(G, params) # or QmcFastKron(G, params)
-qmc.run()
-print(qmc.expectation)
-```
-
-Plot landscapes of the QAOA Max-cut expectation function:
-```
-import networkx as nx
-from qaoalib.qaoa.landscape import HybridFast
-
-G = nx.fast_gnp_random_graph(10, 0.5)
-prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
-
-ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
-ins.create_grid()
-ins.show_landscape()
-```
+# qaoalib
+A package for QAOA Max-cut Calculations.
+
+Packages required:
+- numpy
+- networkx
+- matplotlib
+- qiskit
+
+# How to install
+You can install from the PyPI:
+```
+pip install --upgrade qaoalib
+```
+
+# Usage
+Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
+```
+import networkx as nx
+from qaoalib.qaoa import Qmc, QmcFastKron
+
+G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
+params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
+
+qmc = Qmc(G, params) # or QmcFastKron(G, params)
+qmc.run()
+print(qmc.expectation)
+```
+
+Plot landscapes of the QAOA Max-cut expectation function:
+```
+import networkx as nx
+from qaoalib.qaoa.landscape import HybridFast
+
+G = nx.fast_gnp_random_graph(10, 0.5)
+prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
+
+ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
+ins.create_grid()
+ins.show_landscape()
+```
```

### Comparing `qaoalib-0.1.8/qaoalib/json.py` & `qaoalib-0.1.9/qaoalib/json.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/math.py` & `qaoalib-0.1.9/qaoalib/math.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/landscape/base.py` & `qaoalib-0.1.9/qaoalib/qaoa/landscape/base.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/landscape/direct_numpy.py` & `qaoalib-0.1.9/qaoalib/qaoa/landscape/direct_numpy.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/landscape/hadamard_test.py` & `qaoalib-0.1.9/qaoalib/qaoa/landscape/hadamard_test.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/landscape/hybrid_fast.py` & `qaoalib-0.1.9/qaoalib/qaoa/landscape/hybrid_fast.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/layerwise.py` & `qaoalib-0.1.9/qaoalib/qaoa/layerwise.py`

 * *Files identical despite different names*

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/qis.py` & `qaoalib-0.1.9/qaoalib/qaoa/qis.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from qiskit import QuantumRegister, QuantumCircuit
-from qiskit import Aer, execute
-
-
-sv_backend = Aer.get_backend('statevector_simulator')
-aer_backend = Aer.get_backend('aer_simulator')
-
-def qaoa_circuit(G, params):
-    """
-    QAOA circuit for Max-cut \sum(I-ZZ). No longer follow qiskit QAOA circuit.
-    If want to reproduce the circuit used in qiskit \sum(-ZZ), substitute
-    gamma as -gamma will do.
-    """
-    depth = len(params)//2
-    gamma = params[:depth]
-    beta = params[depth:]
-
-    q = QuantumRegister(len(G.nodes))
-    qc = QuantumCircuit(q)
-
-    qc.h(q)
-    for p in range(depth):
-        for u, v, d in G.edges(data=True):
-            weight = d.get('weight', 1)
-            qc.cx(u, v)
-            qc.rz(-gamma[p]*weight, v)
-            qc.cx(u, v)
-        qc.rx(2*beta[p], q)
-    return qc
-
-def hadamard_test_circuits(G, params):
-    """
-    Return a list of QuantumCircuit's for hadamard tests.
-    """
-    qc_list = []
-    ansatz_circ = qaoa_circuit(G, params)
-
-    for u, v in G.edges:
-        q = QuantumRegister(1)
-        ansatz = QuantumRegister(ansatz_circ.num_qubits)
-        qc = QuantumCircuit(q, ansatz)
-
-        qc.h(q)
-        qc.append(ansatz_circ, ansatz)
-        qc.cz(q, ansatz[u])
-        qc.cz(q, ansatz[v])
-        qc.h(q)
-
-        # bit reversal is required to calculate probabilities
-        qc = qc.reverse_bits()
-        qc_list.append(qc)
-
-    return qc_list
-
-def run_many_circuits(qc_list):
-    job = execute(qc_list, sv_backend)
-    result = job.result()
-    # return a list of np.ndarray of statevectors
-    return [result.get_statevector(idx) for idx in range(len(qc_list))]
+from qiskit import QuantumRegister, QuantumCircuit
+from qiskit import Aer, execute
+
+
+sv_backend = Aer.get_backend('statevector_simulator')
+aer_backend = Aer.get_backend('aer_simulator')
+
+def qaoa_circuit(G, params):
+    """
+    QAOA circuit for Max-cut \sum(I-ZZ). No longer follow qiskit QAOA circuit.
+    If want to reproduce the circuit used in qiskit \sum(-ZZ), substitute
+    gamma as -gamma will do.
+    """
+    depth = len(params)//2
+    gamma = params[:depth]
+    beta = params[depth:]
+
+    q = QuantumRegister(len(G.nodes))
+    qc = QuantumCircuit(q)
+
+    qc.h(q)
+    for p in range(depth):
+        for u, v, d in G.edges(data=True):
+            weight = d.get('weight', 1)
+            qc.cx(u, v)
+            qc.rz(-gamma[p]*weight, v)
+            qc.cx(u, v)
+        qc.rx(2*beta[p], q)
+    return qc
+
+def hadamard_test_circuits(G, params):
+    """
+    Return a list of QuantumCircuit's for hadamard tests.
+    """
+    qc_list = []
+    ansatz_circ = qaoa_circuit(G, params)
+
+    for u, v in G.edges:
+        q = QuantumRegister(1)
+        ansatz = QuantumRegister(ansatz_circ.num_qubits)
+        qc = QuantumCircuit(q, ansatz)
+
+        qc.h(q)
+        qc.append(ansatz_circ, ansatz)
+        qc.cz(q, ansatz[u])
+        qc.cz(q, ansatz[v])
+        qc.h(q)
+
+        # bit reversal is required to calculate probabilities
+        qc = qc.reverse_bits()
+        qc_list.append(qc)
+
+    return qc_list
+
+def run_many_circuits(qc_list):
+    job = execute(qc_list, sv_backend)
+    result = job.result()
+    # return a list of np.ndarray of statevectors
+    return [result.get_statevector(idx) for idx in range(len(qc_list))]
```

### Comparing `qaoalib-0.1.8/qaoalib/qaoa/strategy.py` & `qaoalib-0.1.9/qaoalib/qaoa/strategy.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import numpy as np
-from typing import TYPE_CHECKING, Optional, Union, Sequence
-from typing_extensions import TypeAlias
-# from .params import Params
-
-if TYPE_CHECKING:
-    import numpy.typing as npt
-
-Params: TypeAlias = Union[Sequence[float], "npt.NDArray[np.float_]"]
-
-
-def interp():
-    ...
-
-def bilinear(
-    prev_params: Params,
-    pp_params: Params,
-    gamma_bound: Optional[tuple[float, float]] = None,
-    beta_bound: Optional[tuple[float, float]] = None,
-) -> "npt.NDArray[np.float_]":
-    if gamma_bound is None:
-        gamma_bound = (0, np.pi)
-    if beta_bound is None:
-        beta_bound = (0, np.pi/2)
-
-    prev_params = np.asarray(prev_params)
-    pp_params = np.asarray(pp_params) # prev_prev_params (p-2)
-
-    # split into gamma and beta
-    prev_gb = np.split(prev_params, 2)
-    pp_gb = np.split(pp_params, 2)
-
-    new_gb = []
-    for i in range(2):
-        delta2 = prev_gb[i][-2] - pp_gb[i][-1]
-        pp_gb[i] = np.hstack([pp_gb[i], prev_gb[i][-1] - delta2])
-
-        diff = prev_gb[i] - pp_gb[i]
-        new_x = prev_gb[i] + diff
-
-        delta3 = new_x[-1] - new_x[-2]
-        new_x = np.hstack([new_x, new_x[-1] + delta3])
-
-        if i == 0:
-            new_x = np.clip(new_x, *gamma_bound)
-        else:
-            new_x = np.clip(new_x, *beta_bound)
-
-        new_gb.append(new_x)
-
-    return np.hstack(new_gb)
-
-
-def params_fixing(
-    prev_params: Params,
-    gamma_bound: Optional[tuple[float, float]] = None,
-    beta_bound: Optional[tuple[float, float]] = None,
-) -> "npt.NDArray[np.float_]":
-    if gamma_bound is None:
-        gamma_bound = (0, np.pi)
-    if beta_bound is None:
-        beta_bound = (0, np.pi/2)
-
-    prev_params = np.asarray(prev_params)
-    gamma, beta = np.split(prev_params)
-
-    gamma = np.hstack([gamma, np.random.uniform(*gamma_bound)])
-    beta = np.hstack([beta, np.random.uniform(*beta_bound)])
-
-    return np.hstack([gamma, beta])
+import numpy as np
+from typing import TYPE_CHECKING, Optional, Union, Sequence
+from typing_extensions import TypeAlias
+# from .params import Params
+
+if TYPE_CHECKING:
+    import numpy.typing as npt
+
+Params: TypeAlias = Union[Sequence[float], "npt.NDArray[np.float_]"]
+
+
+def interp():
+    ...
+
+def bilinear(
+    prev_params: Params,
+    pp_params: Params,
+    gamma_bound: Optional[tuple[float, float]] = None,
+    beta_bound: Optional[tuple[float, float]] = None,
+) -> "npt.NDArray[np.float_]":
+    if gamma_bound is None:
+        gamma_bound = (0, np.pi)
+    if beta_bound is None:
+        beta_bound = (0, np.pi/2)
+
+    prev_params = np.asarray(prev_params)
+    pp_params = np.asarray(pp_params) # prev_prev_params (p-2)
+
+    # split into gamma and beta
+    prev_gb = np.split(prev_params, 2)
+    pp_gb = np.split(pp_params, 2)
+
+    new_gb = []
+    for i in range(2):
+        delta2 = prev_gb[i][-2] - pp_gb[i][-1]
+        pp_gb[i] = np.hstack([pp_gb[i], prev_gb[i][-1] - delta2])
+
+        diff = prev_gb[i] - pp_gb[i]
+        new_x = prev_gb[i] + diff
+
+        delta3 = new_x[-1] - new_x[-2]
+        new_x = np.hstack([new_x, new_x[-1] + delta3])
+
+        if i == 0:
+            new_x = np.clip(new_x, *gamma_bound)
+        else:
+            new_x = np.clip(new_x, *beta_bound)
+
+        new_gb.append(new_x)
+
+    return np.hstack(new_gb)
+
+
+def params_fixing(
+    prev_params: Params,
+    gamma_bound: Optional[tuple[float, float]] = None,
+    beta_bound: Optional[tuple[float, float]] = None,
+) -> "npt.NDArray[np.float_]":
+    if gamma_bound is None:
+        gamma_bound = (0, np.pi)
+    if beta_bound is None:
+        beta_bound = (0, np.pi/2)
+
+    prev_params = np.asarray(prev_params)
+    gamma, beta = np.split(prev_params)
+
+    gamma = np.hstack([gamma, np.random.uniform(*gamma_bound)])
+    beta = np.hstack([beta, np.random.uniform(*beta_bound)])
+
+    return np.hstack([gamma, beta])
```

### Comparing `qaoalib-0.1.8/qaoalib/utils.py` & `qaoalib-0.1.9/qaoalib/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Union, Literal, Optional
 import warnings
 import numpy as np
 import networkx as nx
 
-from .data.graph import RegGraphData, GnpGraphData
-
 
 def get_info(filename, indicator, mode='get-numeric'):
     try:
         pos = filename.index(indicator)
     except ValueError:
         return None
 
@@ -261,46 +259,7 @@
             data['expectations'][p] = expectations
             data['alpha'][p] = expectations / data['true_obj']
     else:
         for p, arr in data['expectations'].items():
             data['energies'][p] = -(np.asarray(arr) + data['shift'])
             data['alpha'][p] = np.asarray(arr) / data['true_obj']
 
-def convert_graph(
-    G: nx.Graph,
-    graph_type: Literal['reg', 'gnp'],
-    prob: Optional[float] = None,
-    solve_brute: bool = True,
-) -> Union[RegGraphData, GnpGraphData]:
-
-    if solve_brute:
-        true_obj, _ = maxcut_brute(G)
-    else:
-        true_obj = 0
-
-    n_nodes = len(G.nodes)
-    edges = list(G.edges)
-    n_edges = len(G.edges)
-    shift = -n_edges / 2.0
-
-    if graph_type == 'reg':
-        deg = len(list(G.neighbors(0)))
-        return RegGraphData(
-            deg=deg,
-            n_nodes=n_nodes,
-            edges=edges,
-            n_edges=n_edges,
-            shift=shift,
-            true_obj=true_obj,
-        )
-
-    elif graph_type == 'gnp':
-        if prob is None:
-            raise ValueError('`prob` must be passed for Gnp graphs.')
-        return GnpGraphData(
-            prob=prob,
-            n_nodes=n_nodes,
-            edges=edges,
-            n_edges=n_edges,
-            shift=shift,
-            true_obj=true_obj,
-        )
```

### Comparing `qaoalib-0.1.8/qaoalib.egg-info/PKG-INFO` & `qaoalib-0.1.9/qaoalib.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: qaoalib
-Version: 0.1.8
-Summary: A package for QAOA Maxcut calculations
-Home-page: https://github.com/xenoicwyce/qaoalib
-Author: Xinwei Lee
-Author-email: xenoicwyce@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# qaoalib
-A package for QAOA Max-cut Calculations.
-
-Packages required:
-- numpy
-- networkx
-- matplotlib
-- qiskit
-
-# How to install
-You can install from the PyPI:
-```
-pip install --upgrade qaoalib
-```
-
-# Usage
-Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
-```
-import networkx as nx
-from qaoalib.qaoa import Qmc, QmcFastKron
-
-G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
-params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
-
-qmc = Qmc(G, params) # or QmcFastKron(G, params)
-qmc.run()
-print(qmc.expectation)
-```
-
-Plot landscapes of the QAOA Max-cut expectation function:
-```
-import networkx as nx
-from qaoalib.qaoa.landscape import HybridFast
-
-G = nx.fast_gnp_random_graph(10, 0.5)
-prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
-
-ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
-ins.create_grid()
-ins.show_landscape()
-```
+Metadata-Version: 2.1
+Name: qaoalib
+Version: 0.1.9
+Summary: A package for QAOA Maxcut calculations
+Home-page: https://github.com/xenoicwyce/qaoalib
+Author: Xinwei Lee
+Author-email: xenoicwyce@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# qaoalib
+A package for QAOA Max-cut Calculations.
+
+Packages required:
+- numpy
+- networkx
+- matplotlib
+- qiskit
+
+# How to install
+You can install from the PyPI:
+```
+pip install --upgrade qaoalib
+```
+
+# Usage
+Calculate Max-cut expectation with `Qmc` or `QmcFastKron` (faster version):
+```
+import networkx as nx
+from qaoalib.qaoa import Qmc, QmcFastKron
+
+G = nx.fast_gnp_random_graph(10, 0.5)  # Random graph with 10 nodes
+params = [0.2, 0.4, 0.3, 0.5]          # 4 params, depth = 2
+
+qmc = Qmc(G, params) # or QmcFastKron(G, params)
+qmc.run()
+print(qmc.expectation)
+```
+
+Plot landscapes of the QAOA Max-cut expectation function:
+```
+import networkx as nx
+from qaoalib.qaoa.landscape import HybridFast
+
+G = nx.fast_gnp_random_graph(10, 0.5)
+prev_params = [0.1, 0.2] # previous parameters (gamma1, beta1)
+
+ins = HybridFast(G, prev_params) # plots the landscape wrt gamma2 and beta2 with previous parameters given.
+ins.create_grid()
+ins.show_landscape()
+```
```

### Comparing `qaoalib-0.1.8/qaoalib.egg-info/SOURCES.txt` & `qaoalib-0.1.9/qaoalib.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 qaoalib/utils.py
 qaoalib/version.py
 qaoalib.egg-info/PKG-INFO
 qaoalib.egg-info/SOURCES.txt
 qaoalib.egg-info/dependency_links.txt
 qaoalib.egg-info/requires.txt
 qaoalib.egg-info/top_level.txt
-qaoalib/data/__init__.py
-qaoalib/data/graph.py
-qaoalib/data/result.py
+qaoalib/models/__init__.py
+qaoalib/models/result.py
 qaoalib/qaoa/__init__.py
 qaoalib/qaoa/layerwise.py
 qaoalib/qaoa/qis.py
 qaoalib/qaoa/qmc.py
 qaoalib/qaoa/strategy.py
 qaoalib/qaoa/utils.py
 qaoalib/qaoa/landscape/__init__.py
```

