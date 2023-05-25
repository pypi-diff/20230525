# Comparing `tmp/AlgBench-0.1.3.tar.gz` & `tmp/AlgBench-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgBench-0.1.3.tar", last modified: Thu May 25 15:39:16 2023, max compression
+gzip compressed data, was "AlgBench-1.0.0.tar", last modified: Thu May 25 20:36:49 2023, max compression
```

## Comparing `AlgBench-0.1.3.tar` & `AlgBench-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 15:39:06.000000 AlgBench-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-25 15:39:16.980716 AlgBench-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17077 2023-05-25 15:39:06.000000 AlgBench-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 15:39:06.000000 AlgBench-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:39:16.980716 AlgBench-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.976716 AlgBench-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/src/AlgBench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-05-25 15:39:16.000000 AlgBench-0.1.3/src/AlgBench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 15:39:16.000000 AlgBench-0.1.3/src/AlgBench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:39:16.000000 AlgBench-0.1.3/src/AlgBench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 15:39:16.000000 AlgBench-0.1.3/src/AlgBench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 15:39:16.000000 AlgBench-0.1.3/src/AlgBench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/src/algbench/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/benchmark_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/src/algbench/db/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/db/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/db/nfs_json_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/db/nfs_json_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/db/nfs_json_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/src/algbench/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-25 15:39:06.000000 AlgBench-0.1.3/src/algbench/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:39:16.980716 AlgBench-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-25 15:39:06.000000 AlgBench-0.1.3/tests/test_basics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 20:36:37.000000 AlgBench-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18870 2023-05-25 20:36:49.511835 AlgBench-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-05-25 20:36:37.000000 AlgBench-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 20:36:38.000000 AlgBench-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:36:49.511835 AlgBench-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.507835 AlgBench-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.507835 AlgBench-1.0.0/src/AlgBench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18870 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 20:36:49.000000 AlgBench-1.0.0/src/AlgBench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/benchmark_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/db/nfs_json_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/src/algbench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-25 20:36:38.000000 AlgBench-1.0.0/src/algbench/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:36:49.511835 AlgBench-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-25 20:36:38.000000 AlgBench-1.0.0/tests/test_basics.py
```

### Comparing `AlgBench-0.1.3/LICENSE` & `AlgBench-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgBench-0.1.3/PKG-INFO` & `AlgBench-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 0.1.3
+Version: 1.0.0
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,28 +36,38 @@
 - providing a compressible database to save memory, and saving highly redundant
   information, e.g., of the environment, only once
 - providing an NFS-compatible parallel database and compatibility to
   distribution libraries, such as slurminade
 - using a simple format based on JSON and Zip to allow simple parsing and even
   repairing broken databases by hand
 
-There is a predecessor project, called [AeMeasure](https://github.com/d-krupke/AeMeasure).
-AeMeasure made saving the data easy, but required more boilerplate code and reading the data was more difficult and less efficient.
+There is a predecessor project, called
+[AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
+data easy, but required more boilerplate code and reading the data was more
+difficult and less efficient.
+
+## Installation
+
+You can install AlgBench using pip
+
+```bash
+pip install -U algbench
+```
 
 ## Usage
 
 There is one important class `Benchmark` to run the benchmark, and two important
 functions `describe` and `read_as_pandas` to analyze the results.
 
 <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="Benchmark">class <strong>Benchmark</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
-    
+
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
 <td colspan=2><tt>Benchmark(path:&nbsp;str)&nbsp;-&amp;gt;&nbsp;None<br>
 &nbsp;<br>
 This&nbsp;is&nbsp;the&nbsp;heart&nbsp;of&nbsp;the&nbsp;library.&nbsp;It&nbsp;allows&nbsp;to&nbsp;run,&nbsp;save,&nbsp;and&nbsp;load<br>
 a&nbsp;benchmark.<br>
 &nbsp;<br>
 The&nbsp;function&nbsp;`add`&nbsp;will&nbsp;run&nbsp;a&nbsp;configuration,&nbsp;if&nbsp;it&nbsp;is&nbsp;not<br>
@@ -65,18 +75,20 @@
 `run`.&nbsp;This&nbsp;may&nbsp;be&nbsp;advised&nbsp;if&nbsp;you&nbsp;want&nbsp;to&nbsp;distribute&nbsp;the&nbsp;execution.<br>
 &nbsp;<br>
 ```python<br>
 from&nbsp;algbench&nbsp;import&nbsp;Benchmark<br>
 &nbsp;<br>
 benchmark&nbsp;=&nbsp;Benchmark("./test_benchmark")<br>
 &nbsp;<br>
+&nbsp;<br>
 def&nbsp;f(x,&nbsp;_test=2,&nbsp;default="default"):<br>
 &nbsp;&nbsp;&nbsp;&nbsp;print(x)&nbsp;&nbsp;#&nbsp;here&nbsp;you&nbsp;would&nbsp;run&nbsp;your&nbsp;algorithm<br>
 &nbsp;&nbsp;&nbsp;&nbsp;return&nbsp;{"r1":&nbsp;x,&nbsp;"r2":&nbsp;"test"}<br>
 &nbsp;<br>
+&nbsp;<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;1,&nbsp;_test=None)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;2)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;3,&nbsp;_test=None)<br>
 &nbsp;<br>
 benchmark.<a href="#Benchmark-compress">compress</a>()<br>
 &nbsp;<br>
 for&nbsp;entry&nbsp;in&nbsp;benchmark:<br>
@@ -157,17 +169,16 @@
 <dd><tt>dictionary&nbsp;for&nbsp;instance&nbsp;variables&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 <dl><dt><strong>__weakref__</strong></dt>
 <dd><tt>list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 </td></tr></table>
 
-
-You can find [an example for graph coloring](./examples/graph_coloring/).
-The important parts are shown below.
+You can find [an example for graph coloring](./examples/graph_coloring/). The
+important parts are shown below.
 
 ### Running a benchmark
 
 ```python
 from _utils import InstanceDb
 from algbench import Benchmark
 import networkx as nx
@@ -219,130 +230,187 @@
 ### Analyzing the data
 
 ```python
 from algbench import describe, read_as_pandas, Benchmark
 
 describe("./03_benchmark_data/")
 ```
-```
-parameters:
+
+<details>
+<summary>Output</summary>
+<pre>
+ result:
+| num_vertices: 68
+| num_edges: 697
+| coloring:
+|| 0: 7
+|| 1: 8
+|| 2: 2
+|| 3: 5
+|| 4: 3
+|| 5: 7
+|| 6: 7
+|| 7: 6
+|| 8: 5
+|| 9: 4
+|| 10: 5
+|| 11: 4
+|| 12: 0
+|| 13: 6
+|| 14: 0
+|| 15: 3
+|| 16: 5
+|| 17: 5
+|| 18: 7
+|| 19: 0
+|| ...
+| n_colors: 9
+ timestamp: 2023-05-25T21:58:39.201553
+ runtime: 0.002952098846435547
+ stdout: 
+ stderr: 
+ env_fingerprint: 53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1
+ args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
+ parameters:
 | func: eval_greedy_alg
 | args:
 || instance_name: graph_0
 || alg_params:
 ||| strategy: largest_first
 ||| interchange: True
-env:
+ argv: ['02_run_benchmark.py']
+ env:
 | hostname: workstation-r7
 | python_version: 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]
 | python: /home/krupke/anaconda3/envs/mo310/bin/python3
 | cwd: /home/krupke/Repositories/AlgBench/examples/graph_coloring
 | environment: [{'name': 'virtualenv', 'path': '/home/krupke/.local/lib/python3.10/site-pack...
-data:
-| result:
-|| num_vertices: 50
-|| num_edges: 275
-|| coloring:
-||| 0: 2
-||| 1: 0
-||| 2: 1
-||| 3: 1
-||| 4: 3
-||| 5: 1
-||| 6: 4
-||| 7: 3
-||| 8: 3
-||| 9: 3
-||| 10: 1
-||| 11: 4
-||| 12: 1
-||| 13: 2
-||| 14: 3
-||| 15: 0
-||| 16: 0
-||| 17: 0
-||| 18: 0
-||| 19: 1
-||| ...
-|| n_colors: 6
-| timestamp: 2023-05-25T15:22:37.540734
-| runtime: 0.0009615421295166016
-| stdout: 
-| stderr: 
-| env_fingerprint: b2cee276004fd00bcb5343f9d8e9199c13c25fec
-| args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
-```
+| git_revision: 5357426feb4b49174c313ffa33e2cadf6a83e226
+| python_file: /home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py
+</pre>
+</details>
+
 ```python
 # we can also see the raw data of the first entry using `front`
 Benchmark("./03_benchmark_data/").front()
 ```
-```
-{'parameters': {'func': 'eval_greedy_alg',
+
+<details>
+<summary>Output</summary>
+<pre>
+{'result': {'num_vertices': 68,
+  'num_edges': 697,
+  'coloring': {'0': 7,
+   '1': 8,
+   '2': 2,
+   '3': 5,
+   '4': 3,
+   '5': 7,
+   '6': 7,
+   '7': 6,
+   '8': 5,
+   '9': 4,
+   '10': 5,
+   '11': 4,
+   '12': 0,
+   '13': 6,
+   '14': 0,
+   '15': 3,
+   '16': 5,
+   '17': 5,
+   '18': 7,
+   '19': 0,
+   '20': 2,
+   '21': 3,
+    ...},
+  'n_colors': 9},
+ 'timestamp': '2023-05-25T21:58:39.201553',
+ 'runtime': 0.002952098846435547,
+ 'stdout': '',
+ 'stderr': '',
+ 'env_fingerprint': '53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1',
+ 'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec',
+ 'parameters': {'func': 'eval_greedy_alg',
   'args': {'instance_name': 'graph_0',
    'alg_params': {'strategy': 'largest_first', 'interchange': True}}},
+ 'argv': ['02_run_benchmark.py'],
  'env': {'hostname': 'workstation-r7',
   'python_version': '3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]',
   'python': '/home/krupke/anaconda3/envs/mo310/bin/python3',
   'cwd': '/home/krupke/Repositories/AlgBench/examples/graph_coloring',
   'environment': [{'name': 'virtualenv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '20.14.1'},
    {'name': 'cfgv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '3.3.1'},
-   {'name': 'pre-commit',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.18.1'},
-   {'name': 'identify',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.4.12'},
-   {'name': 'py',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.11.0'},
-   {'name': 'nodeenv',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.6.0'},
-...
-  'runtime': 0.0009615421295166016,
-  'stdout': '',
-  'stderr': '',
-  'env_fingerprint': 'b2cee276004fd00bcb5343f9d8e9199c13c25fec',
-  'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec'}}
-```
+  ...],
+  'git_revision': '5357426feb4b49174c313ffa33e2cadf6a83e226',
+  'python_file': '/home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py'}}
+</pre>
+</details>
+
 ```python
 # we can extract a full pandas tables using `read_as_pandas`
 t = read_as_pandas(
     "./03_benchmark_data/",
     lambda result: {
         "instance": result["parameters"]["args"]["instance_name"],
         "strategy": result["parameters"]["args"]["alg_params"]["strategy"],
         "interchange": result["parameters"]["args"]["alg_params"].get(
             "interchange", None
         ),
-        "colors": result["data"]["result"]["n_colors"],
+        "colors": result["result"]["n_colors"],
+        "runtime": result["runtime"],
+        "num_vertices": result["result"]["num_vertices"],
+        "num_edges": result["result"]["num_edges"],
     },
 )
-t
+print(t)
 ```
-```
-      instance                  strategy interchange  colors
-0      graph_0             largest_first        True       6
-1      graph_0             largest_first       False       7
-2      graph_0         random_sequential        True       6
-3      graph_0         random_sequential       False       7
-4      graph_0             smallest_last        True       6
-...        ...                       ...         ...     ...
-1195  graph_99  connected_sequential_bfs        True      15
-1196  graph_99  connected_sequential_bfs       False      17
-1197  graph_99  connected_sequential_dfs        True      14
-1198  graph_99  connected_sequential_dfs       False      15
-1199  graph_99  saturation_largest_first        None      15
 
-[1200 rows x 4 columns]
+<details>
+<summary>Output</summary>
+
 ```
+       instance                  strategy interchange  colors   runtime ...
+0       graph_0             largest_first        True       9  0.002952  
+1       graph_0             largest_first       False      10  0.000183
+2       graph_0         random_sequential        True       9  0.003562
+3       graph_0         random_sequential       False      12  0.000173
+4       graph_0             smallest_last        True       9  0.003813
+...         ...                       ...         ...     ...       ...
+5995  graph_499  connected_sequential_bfs        True       3  0.000216
+5996  graph_499  connected_sequential_bfs       False       3  0.000132
+5997  graph_499  connected_sequential_dfs        True       3  0.000231
+5998  graph_499  connected_sequential_dfs       False       4  0.000132
+5999  graph_499  saturation_largest_first        None       3  0.000202
+
+
+[6000 rows x 7 columns]
+```
+</details>
+
+## Which information is saved?
+
+The following information is saved automatically:
+
+- function name
+- all arguments that do not begin with "\_"
+- the returned values
+- runtime
+- current date and time
+- hostname
+- Python version
+- Python binary path
+- current working directory
+- stdout and stderr
+- all installed modules and their versions
+- git revision
+- path of the python file
 
 ## On doing good empirical evaluations of algorithms
 
 To get a feeling on the interesting instances and parameters, or generally on
 where to look deeper, you should first perform an explorative study. For such an
 explorative study, you should select some random parameters and instances, and
 just look how the numbers look. Iteratively change the parameters and instances,
@@ -375,15 +443,15 @@
 
 You can find a guide [here](https://git-lfs.com/) on how to install Git LFS.
 
 Run
 
 ```bash
 git lfs install
-```
+````
 
 to set up git LFS and
 
 ```bash
 git lfs track "*.zip"
 ```
 
@@ -399,11 +467,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.0.0** Changing the database layout, making it more efficient (breaking
+  change!).
+- **0.2.0** Changing database slightly to contain meta data and doing more
+  caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
 - **0.1.0** First complete version
```

### Comparing `AlgBench-0.1.3/README.md` & `AlgBench-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,28 +25,38 @@
 - providing a compressible database to save memory, and saving highly redundant
   information, e.g., of the environment, only once
 - providing an NFS-compatible parallel database and compatibility to
   distribution libraries, such as slurminade
 - using a simple format based on JSON and Zip to allow simple parsing and even
   repairing broken databases by hand
 
-There is a predecessor project, called [AeMeasure](https://github.com/d-krupke/AeMeasure).
-AeMeasure made saving the data easy, but required more boilerplate code and reading the data was more difficult and less efficient.
+There is a predecessor project, called
+[AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
+data easy, but required more boilerplate code and reading the data was more
+difficult and less efficient.
+
+## Installation
+
+You can install AlgBench using pip
+
+```bash
+pip install -U algbench
+```
 
 ## Usage
 
 There is one important class `Benchmark` to run the benchmark, and two important
 functions `describe` and `read_as_pandas` to analyze the results.
 
 <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="Benchmark">class <strong>Benchmark</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
-    
+
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
 <td colspan=2><tt>Benchmark(path:&nbsp;str)&nbsp;-&amp;gt;&nbsp;None<br>
 &nbsp;<br>
 This&nbsp;is&nbsp;the&nbsp;heart&nbsp;of&nbsp;the&nbsp;library.&nbsp;It&nbsp;allows&nbsp;to&nbsp;run,&nbsp;save,&nbsp;and&nbsp;load<br>
 a&nbsp;benchmark.<br>
 &nbsp;<br>
 The&nbsp;function&nbsp;`add`&nbsp;will&nbsp;run&nbsp;a&nbsp;configuration,&nbsp;if&nbsp;it&nbsp;is&nbsp;not<br>
@@ -54,18 +64,20 @@
 `run`.&nbsp;This&nbsp;may&nbsp;be&nbsp;advised&nbsp;if&nbsp;you&nbsp;want&nbsp;to&nbsp;distribute&nbsp;the&nbsp;execution.<br>
 &nbsp;<br>
 ```python<br>
 from&nbsp;algbench&nbsp;import&nbsp;Benchmark<br>
 &nbsp;<br>
 benchmark&nbsp;=&nbsp;Benchmark("./test_benchmark")<br>
 &nbsp;<br>
+&nbsp;<br>
 def&nbsp;f(x,&nbsp;_test=2,&nbsp;default="default"):<br>
 &nbsp;&nbsp;&nbsp;&nbsp;print(x)&nbsp;&nbsp;#&nbsp;here&nbsp;you&nbsp;would&nbsp;run&nbsp;your&nbsp;algorithm<br>
 &nbsp;&nbsp;&nbsp;&nbsp;return&nbsp;{"r1":&nbsp;x,&nbsp;"r2":&nbsp;"test"}<br>
 &nbsp;<br>
+&nbsp;<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;1,&nbsp;_test=None)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;2)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;3,&nbsp;_test=None)<br>
 &nbsp;<br>
 benchmark.<a href="#Benchmark-compress">compress</a>()<br>
 &nbsp;<br>
 for&nbsp;entry&nbsp;in&nbsp;benchmark:<br>
@@ -146,17 +158,16 @@
 <dd><tt>dictionary&nbsp;for&nbsp;instance&nbsp;variables&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 <dl><dt><strong>__weakref__</strong></dt>
 <dd><tt>list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 </td></tr></table>
 
-
-You can find [an example for graph coloring](./examples/graph_coloring/).
-The important parts are shown below.
+You can find [an example for graph coloring](./examples/graph_coloring/). The
+important parts are shown below.
 
 ### Running a benchmark
 
 ```python
 from _utils import InstanceDb
 from algbench import Benchmark
 import networkx as nx
@@ -208,130 +219,187 @@
 ### Analyzing the data
 
 ```python
 from algbench import describe, read_as_pandas, Benchmark
 
 describe("./03_benchmark_data/")
 ```
-```
-parameters:
+
+<details>
+<summary>Output</summary>
+<pre>
+ result:
+| num_vertices: 68
+| num_edges: 697
+| coloring:
+|| 0: 7
+|| 1: 8
+|| 2: 2
+|| 3: 5
+|| 4: 3
+|| 5: 7
+|| 6: 7
+|| 7: 6
+|| 8: 5
+|| 9: 4
+|| 10: 5
+|| 11: 4
+|| 12: 0
+|| 13: 6
+|| 14: 0
+|| 15: 3
+|| 16: 5
+|| 17: 5
+|| 18: 7
+|| 19: 0
+|| ...
+| n_colors: 9
+ timestamp: 2023-05-25T21:58:39.201553
+ runtime: 0.002952098846435547
+ stdout: 
+ stderr: 
+ env_fingerprint: 53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1
+ args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
+ parameters:
 | func: eval_greedy_alg
 | args:
 || instance_name: graph_0
 || alg_params:
 ||| strategy: largest_first
 ||| interchange: True
-env:
+ argv: ['02_run_benchmark.py']
+ env:
 | hostname: workstation-r7
 | python_version: 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]
 | python: /home/krupke/anaconda3/envs/mo310/bin/python3
 | cwd: /home/krupke/Repositories/AlgBench/examples/graph_coloring
 | environment: [{'name': 'virtualenv', 'path': '/home/krupke/.local/lib/python3.10/site-pack...
-data:
-| result:
-|| num_vertices: 50
-|| num_edges: 275
-|| coloring:
-||| 0: 2
-||| 1: 0
-||| 2: 1
-||| 3: 1
-||| 4: 3
-||| 5: 1
-||| 6: 4
-||| 7: 3
-||| 8: 3
-||| 9: 3
-||| 10: 1
-||| 11: 4
-||| 12: 1
-||| 13: 2
-||| 14: 3
-||| 15: 0
-||| 16: 0
-||| 17: 0
-||| 18: 0
-||| 19: 1
-||| ...
-|| n_colors: 6
-| timestamp: 2023-05-25T15:22:37.540734
-| runtime: 0.0009615421295166016
-| stdout: 
-| stderr: 
-| env_fingerprint: b2cee276004fd00bcb5343f9d8e9199c13c25fec
-| args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
-```
+| git_revision: 5357426feb4b49174c313ffa33e2cadf6a83e226
+| python_file: /home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py
+</pre>
+</details>
+
 ```python
 # we can also see the raw data of the first entry using `front`
 Benchmark("./03_benchmark_data/").front()
 ```
-```
-{'parameters': {'func': 'eval_greedy_alg',
+
+<details>
+<summary>Output</summary>
+<pre>
+{'result': {'num_vertices': 68,
+  'num_edges': 697,
+  'coloring': {'0': 7,
+   '1': 8,
+   '2': 2,
+   '3': 5,
+   '4': 3,
+   '5': 7,
+   '6': 7,
+   '7': 6,
+   '8': 5,
+   '9': 4,
+   '10': 5,
+   '11': 4,
+   '12': 0,
+   '13': 6,
+   '14': 0,
+   '15': 3,
+   '16': 5,
+   '17': 5,
+   '18': 7,
+   '19': 0,
+   '20': 2,
+   '21': 3,
+    ...},
+  'n_colors': 9},
+ 'timestamp': '2023-05-25T21:58:39.201553',
+ 'runtime': 0.002952098846435547,
+ 'stdout': '',
+ 'stderr': '',
+ 'env_fingerprint': '53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1',
+ 'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec',
+ 'parameters': {'func': 'eval_greedy_alg',
   'args': {'instance_name': 'graph_0',
    'alg_params': {'strategy': 'largest_first', 'interchange': True}}},
+ 'argv': ['02_run_benchmark.py'],
  'env': {'hostname': 'workstation-r7',
   'python_version': '3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]',
   'python': '/home/krupke/anaconda3/envs/mo310/bin/python3',
   'cwd': '/home/krupke/Repositories/AlgBench/examples/graph_coloring',
   'environment': [{'name': 'virtualenv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '20.14.1'},
    {'name': 'cfgv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '3.3.1'},
-   {'name': 'pre-commit',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.18.1'},
-   {'name': 'identify',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.4.12'},
-   {'name': 'py',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.11.0'},
-   {'name': 'nodeenv',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.6.0'},
-...
-  'runtime': 0.0009615421295166016,
-  'stdout': '',
-  'stderr': '',
-  'env_fingerprint': 'b2cee276004fd00bcb5343f9d8e9199c13c25fec',
-  'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec'}}
-```
+  ...],
+  'git_revision': '5357426feb4b49174c313ffa33e2cadf6a83e226',
+  'python_file': '/home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py'}}
+</pre>
+</details>
+
 ```python
 # we can extract a full pandas tables using `read_as_pandas`
 t = read_as_pandas(
     "./03_benchmark_data/",
     lambda result: {
         "instance": result["parameters"]["args"]["instance_name"],
         "strategy": result["parameters"]["args"]["alg_params"]["strategy"],
         "interchange": result["parameters"]["args"]["alg_params"].get(
             "interchange", None
         ),
-        "colors": result["data"]["result"]["n_colors"],
+        "colors": result["result"]["n_colors"],
+        "runtime": result["runtime"],
+        "num_vertices": result["result"]["num_vertices"],
+        "num_edges": result["result"]["num_edges"],
     },
 )
-t
+print(t)
 ```
-```
-      instance                  strategy interchange  colors
-0      graph_0             largest_first        True       6
-1      graph_0             largest_first       False       7
-2      graph_0         random_sequential        True       6
-3      graph_0         random_sequential       False       7
-4      graph_0             smallest_last        True       6
-...        ...                       ...         ...     ...
-1195  graph_99  connected_sequential_bfs        True      15
-1196  graph_99  connected_sequential_bfs       False      17
-1197  graph_99  connected_sequential_dfs        True      14
-1198  graph_99  connected_sequential_dfs       False      15
-1199  graph_99  saturation_largest_first        None      15
 
-[1200 rows x 4 columns]
+<details>
+<summary>Output</summary>
+
 ```
+       instance                  strategy interchange  colors   runtime ...
+0       graph_0             largest_first        True       9  0.002952  
+1       graph_0             largest_first       False      10  0.000183
+2       graph_0         random_sequential        True       9  0.003562
+3       graph_0         random_sequential       False      12  0.000173
+4       graph_0             smallest_last        True       9  0.003813
+...         ...                       ...         ...     ...       ...
+5995  graph_499  connected_sequential_bfs        True       3  0.000216
+5996  graph_499  connected_sequential_bfs       False       3  0.000132
+5997  graph_499  connected_sequential_dfs        True       3  0.000231
+5998  graph_499  connected_sequential_dfs       False       4  0.000132
+5999  graph_499  saturation_largest_first        None       3  0.000202
+
+
+[6000 rows x 7 columns]
+```
+</details>
+
+## Which information is saved?
+
+The following information is saved automatically:
+
+- function name
+- all arguments that do not begin with "\_"
+- the returned values
+- runtime
+- current date and time
+- hostname
+- Python version
+- Python binary path
+- current working directory
+- stdout and stderr
+- all installed modules and their versions
+- git revision
+- path of the python file
 
 ## On doing good empirical evaluations of algorithms
 
 To get a feeling on the interesting instances and parameters, or generally on
 where to look deeper, you should first perform an explorative study. For such an
 explorative study, you should select some random parameters and instances, and
 just look how the numbers look. Iteratively change the parameters and instances,
@@ -364,15 +432,15 @@
 
 You can find a guide [here](https://git-lfs.com/) on how to install Git LFS.
 
 Run
 
 ```bash
 git lfs install
-```
+````
 
 to set up git LFS and
 
 ```bash
 git lfs track "*.zip"
 ```
 
@@ -388,11 +456,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.0.0** Changing the database layout, making it more efficient (breaking
+  change!).
+- **0.2.0** Changing database slightly to contain meta data and doing more
+  caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
 - **0.1.0** First complete version
```

### Comparing `AlgBench-0.1.3/pyproject.toml` & `AlgBench-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "AlgBench"
-version = "0.1.3"
+version = "1.0.0"
 authors = [
     { name = "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)", email = "krupke@ibr.cs.tu-bs.de" },
 ]
 description = ""
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `AlgBench-0.1.3/src/AlgBench.egg-info/PKG-INFO` & `AlgBench-1.0.0/src/AlgBench.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgBench
-Version: 0.1.3
+Version: 1.0.0
 Author-email: "TU Braunschweig, IBR, Algorithms Group (Dominik Krupke)" <krupke@ibr.cs.tu-bs.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -36,28 +36,38 @@
 - providing a compressible database to save memory, and saving highly redundant
   information, e.g., of the environment, only once
 - providing an NFS-compatible parallel database and compatibility to
   distribution libraries, such as slurminade
 - using a simple format based on JSON and Zip to allow simple parsing and even
   repairing broken databases by hand
 
-There is a predecessor project, called [AeMeasure](https://github.com/d-krupke/AeMeasure).
-AeMeasure made saving the data easy, but required more boilerplate code and reading the data was more difficult and less efficient.
+There is a predecessor project, called
+[AeMeasure](https://github.com/d-krupke/AeMeasure). AeMeasure made saving the
+data easy, but required more boilerplate code and reading the data was more
+difficult and less efficient.
+
+## Installation
+
+You can install AlgBench using pip
+
+```bash
+pip install -U algbench
+```
 
 ## Usage
 
 There is one important class `Benchmark` to run the benchmark, and two important
 functions `describe` and `read_as_pandas` to analyze the results.
 
 <p>
 <table width="100%" cellspacing=0 cellpadding=2 border=0 summary="section">
 <tr bgcolor="#ffc8d8">
 <td colspan=3 valign=bottom>&nbsp;<br>
 <font color="#000000" face="helvetica, arial"><a name="Benchmark">class <strong>Benchmark</strong></a>(<a href="builtins.html#object">builtins.object</a>)</font></td></tr>
-    
+
 <tr bgcolor="#ffc8d8"><td rowspan=2><tt>&nbsp;&nbsp;&nbsp;</tt></td>
 <td colspan=2><tt>Benchmark(path:&nbsp;str)&nbsp;-&amp;gt;&nbsp;None<br>
 &nbsp;<br>
 This&nbsp;is&nbsp;the&nbsp;heart&nbsp;of&nbsp;the&nbsp;library.&nbsp;It&nbsp;allows&nbsp;to&nbsp;run,&nbsp;save,&nbsp;and&nbsp;load<br>
 a&nbsp;benchmark.<br>
 &nbsp;<br>
 The&nbsp;function&nbsp;`add`&nbsp;will&nbsp;run&nbsp;a&nbsp;configuration,&nbsp;if&nbsp;it&nbsp;is&nbsp;not<br>
@@ -65,18 +75,20 @@
 `run`.&nbsp;This&nbsp;may&nbsp;be&nbsp;advised&nbsp;if&nbsp;you&nbsp;want&nbsp;to&nbsp;distribute&nbsp;the&nbsp;execution.<br>
 &nbsp;<br>
 ```python<br>
 from&nbsp;algbench&nbsp;import&nbsp;Benchmark<br>
 &nbsp;<br>
 benchmark&nbsp;=&nbsp;Benchmark("./test_benchmark")<br>
 &nbsp;<br>
+&nbsp;<br>
 def&nbsp;f(x,&nbsp;_test=2,&nbsp;default="default"):<br>
 &nbsp;&nbsp;&nbsp;&nbsp;print(x)&nbsp;&nbsp;#&nbsp;here&nbsp;you&nbsp;would&nbsp;run&nbsp;your&nbsp;algorithm<br>
 &nbsp;&nbsp;&nbsp;&nbsp;return&nbsp;{"r1":&nbsp;x,&nbsp;"r2":&nbsp;"test"}<br>
 &nbsp;<br>
+&nbsp;<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;1,&nbsp;_test=None)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;2)<br>
 benchmark.<a href="#Benchmark-add">add</a>(f,&nbsp;3,&nbsp;_test=None)<br>
 &nbsp;<br>
 benchmark.<a href="#Benchmark-compress">compress</a>()<br>
 &nbsp;<br>
 for&nbsp;entry&nbsp;in&nbsp;benchmark:<br>
@@ -157,17 +169,16 @@
 <dd><tt>dictionary&nbsp;for&nbsp;instance&nbsp;variables&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 <dl><dt><strong>__weakref__</strong></dt>
 <dd><tt>list&nbsp;of&nbsp;weak&nbsp;references&nbsp;to&nbsp;the&nbsp;object&nbsp;(if&nbsp;defined)</tt></dd>
 </dl>
 </td></tr></table>
 
-
-You can find [an example for graph coloring](./examples/graph_coloring/).
-The important parts are shown below.
+You can find [an example for graph coloring](./examples/graph_coloring/). The
+important parts are shown below.
 
 ### Running a benchmark
 
 ```python
 from _utils import InstanceDb
 from algbench import Benchmark
 import networkx as nx
@@ -219,130 +230,187 @@
 ### Analyzing the data
 
 ```python
 from algbench import describe, read_as_pandas, Benchmark
 
 describe("./03_benchmark_data/")
 ```
-```
-parameters:
+
+<details>
+<summary>Output</summary>
+<pre>
+ result:
+| num_vertices: 68
+| num_edges: 697
+| coloring:
+|| 0: 7
+|| 1: 8
+|| 2: 2
+|| 3: 5
+|| 4: 3
+|| 5: 7
+|| 6: 7
+|| 7: 6
+|| 8: 5
+|| 9: 4
+|| 10: 5
+|| 11: 4
+|| 12: 0
+|| 13: 6
+|| 14: 0
+|| 15: 3
+|| 16: 5
+|| 17: 5
+|| 18: 7
+|| 19: 0
+|| ...
+| n_colors: 9
+ timestamp: 2023-05-25T21:58:39.201553
+ runtime: 0.002952098846435547
+ stdout: 
+ stderr: 
+ env_fingerprint: 53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1
+ args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
+ parameters:
 | func: eval_greedy_alg
 | args:
 || instance_name: graph_0
 || alg_params:
 ||| strategy: largest_first
 ||| interchange: True
-env:
+ argv: ['02_run_benchmark.py']
+ env:
 | hostname: workstation-r7
 | python_version: 3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]
 | python: /home/krupke/anaconda3/envs/mo310/bin/python3
 | cwd: /home/krupke/Repositories/AlgBench/examples/graph_coloring
 | environment: [{'name': 'virtualenv', 'path': '/home/krupke/.local/lib/python3.10/site-pack...
-data:
-| result:
-|| num_vertices: 50
-|| num_edges: 275
-|| coloring:
-||| 0: 2
-||| 1: 0
-||| 2: 1
-||| 3: 1
-||| 4: 3
-||| 5: 1
-||| 6: 4
-||| 7: 3
-||| 8: 3
-||| 9: 3
-||| 10: 1
-||| 11: 4
-||| 12: 1
-||| 13: 2
-||| 14: 3
-||| 15: 0
-||| 16: 0
-||| 17: 0
-||| 18: 0
-||| 19: 1
-||| ...
-|| n_colors: 6
-| timestamp: 2023-05-25T15:22:37.540734
-| runtime: 0.0009615421295166016
-| stdout: 
-| stderr: 
-| env_fingerprint: b2cee276004fd00bcb5343f9d8e9199c13c25fec
-| args_fingerprint: 10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec
-```
+| git_revision: 5357426feb4b49174c313ffa33e2cadf6a83e226
+| python_file: /home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py
+</pre>
+</details>
+
 ```python
 # we can also see the raw data of the first entry using `front`
 Benchmark("./03_benchmark_data/").front()
 ```
-```
-{'parameters': {'func': 'eval_greedy_alg',
+
+<details>
+<summary>Output</summary>
+<pre>
+{'result': {'num_vertices': 68,
+  'num_edges': 697,
+  'coloring': {'0': 7,
+   '1': 8,
+   '2': 2,
+   '3': 5,
+   '4': 3,
+   '5': 7,
+   '6': 7,
+   '7': 6,
+   '8': 5,
+   '9': 4,
+   '10': 5,
+   '11': 4,
+   '12': 0,
+   '13': 6,
+   '14': 0,
+   '15': 3,
+   '16': 5,
+   '17': 5,
+   '18': 7,
+   '19': 0,
+   '20': 2,
+   '21': 3,
+    ...},
+  'n_colors': 9},
+ 'timestamp': '2023-05-25T21:58:39.201553',
+ 'runtime': 0.002952098846435547,
+ 'stdout': '',
+ 'stderr': '',
+ 'env_fingerprint': '53ad3b5b29d082d7e2bca6881ec9fe35fe441ae1',
+ 'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec',
+ 'parameters': {'func': 'eval_greedy_alg',
   'args': {'instance_name': 'graph_0',
    'alg_params': {'strategy': 'largest_first', 'interchange': True}}},
+ 'argv': ['02_run_benchmark.py'],
  'env': {'hostname': 'workstation-r7',
   'python_version': '3.10.9 (main, Jan 11 2023, 15:21:40) [GCC 11.2.0]',
   'python': '/home/krupke/anaconda3/envs/mo310/bin/python3',
   'cwd': '/home/krupke/Repositories/AlgBench/examples/graph_coloring',
   'environment': [{'name': 'virtualenv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '20.14.1'},
    {'name': 'cfgv',
     'path': '/home/krupke/.local/lib/python3.10/site-packages',
     'version': '3.3.1'},
-   {'name': 'pre-commit',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.18.1'},
-   {'name': 'identify',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '2.4.12'},
-   {'name': 'py',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.11.0'},
-   {'name': 'nodeenv',
-    'path': '/home/krupke/.local/lib/python3.10/site-packages',
-    'version': '1.6.0'},
-...
-  'runtime': 0.0009615421295166016,
-  'stdout': '',
-  'stderr': '',
-  'env_fingerprint': 'b2cee276004fd00bcb5343f9d8e9199c13c25fec',
-  'args_fingerprint': '10ce65b7a61d5ecbfcb1f4e390d72122f7a1f6ec'}}
-```
+  ...],
+  'git_revision': '5357426feb4b49174c313ffa33e2cadf6a83e226',
+  'python_file': '/home/krupke/Repositories/AlgBench/examples/graph_coloring/02_run_benchmark.py'}}
+</pre>
+</details>
+
 ```python
 # we can extract a full pandas tables using `read_as_pandas`
 t = read_as_pandas(
     "./03_benchmark_data/",
     lambda result: {
         "instance": result["parameters"]["args"]["instance_name"],
         "strategy": result["parameters"]["args"]["alg_params"]["strategy"],
         "interchange": result["parameters"]["args"]["alg_params"].get(
             "interchange", None
         ),
-        "colors": result["data"]["result"]["n_colors"],
+        "colors": result["result"]["n_colors"],
+        "runtime": result["runtime"],
+        "num_vertices": result["result"]["num_vertices"],
+        "num_edges": result["result"]["num_edges"],
     },
 )
-t
+print(t)
 ```
-```
-      instance                  strategy interchange  colors
-0      graph_0             largest_first        True       6
-1      graph_0             largest_first       False       7
-2      graph_0         random_sequential        True       6
-3      graph_0         random_sequential       False       7
-4      graph_0             smallest_last        True       6
-...        ...                       ...         ...     ...
-1195  graph_99  connected_sequential_bfs        True      15
-1196  graph_99  connected_sequential_bfs       False      17
-1197  graph_99  connected_sequential_dfs        True      14
-1198  graph_99  connected_sequential_dfs       False      15
-1199  graph_99  saturation_largest_first        None      15
 
-[1200 rows x 4 columns]
+<details>
+<summary>Output</summary>
+
 ```
+       instance                  strategy interchange  colors   runtime ...
+0       graph_0             largest_first        True       9  0.002952  
+1       graph_0             largest_first       False      10  0.000183
+2       graph_0         random_sequential        True       9  0.003562
+3       graph_0         random_sequential       False      12  0.000173
+4       graph_0             smallest_last        True       9  0.003813
+...         ...                       ...         ...     ...       ...
+5995  graph_499  connected_sequential_bfs        True       3  0.000216
+5996  graph_499  connected_sequential_bfs       False       3  0.000132
+5997  graph_499  connected_sequential_dfs        True       3  0.000231
+5998  graph_499  connected_sequential_dfs       False       4  0.000132
+5999  graph_499  saturation_largest_first        None       3  0.000202
+
+
+[6000 rows x 7 columns]
+```
+</details>
+
+## Which information is saved?
+
+The following information is saved automatically:
+
+- function name
+- all arguments that do not begin with "\_"
+- the returned values
+- runtime
+- current date and time
+- hostname
+- Python version
+- Python binary path
+- current working directory
+- stdout and stderr
+- all installed modules and their versions
+- git revision
+- path of the python file
 
 ## On doing good empirical evaluations of algorithms
 
 To get a feeling on the interesting instances and parameters, or generally on
 where to look deeper, you should first perform an explorative study. For such an
 explorative study, you should select some random parameters and instances, and
 just look how the numbers look. Iteratively change the parameters and instances,
@@ -375,15 +443,15 @@
 
 You can find a guide [here](https://git-lfs.com/) on how to install Git LFS.
 
 Run
 
 ```bash
 git lfs install
-```
+````
 
 to set up git LFS and
 
 ```bash
 git lfs track "*.zip"
 ```
 
@@ -399,11 +467,15 @@
 
 ```bash
 git add .gitattributes
 ```
 
 # Version History
 
+- **1.0.0** Changing the database layout, making it more efficient (breaking
+  change!).
+- **0.2.0** Changing database slightly to contain meta data and doing more
+  caching. Saving some more information.
 - **0.1.3** Fixed bug in arg fingerprint set.
 - **0.1.2** Fixed bug with empty rows in pandas table.
 - **0.1.1** Fixed bug with `delete_if`.
 - **0.1.0** First complete version
```

### Comparing `AlgBench-0.1.3/src/AlgBench.egg-info/SOURCES.txt` & `AlgBench-1.0.0/src/AlgBench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AlgBench-0.1.3/src/algbench/__init__.py` & `AlgBench-1.0.0/src/algbench/__init__.py`

 * *Files identical despite different names*

### Comparing `AlgBench-0.1.3/src/algbench/benchmark.py` & `AlgBench-1.0.0/src/algbench/benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,35 +17,14 @@
     This is the heart of the library. It allows to run, save, and load
     a benchmark.
 
     The function `add` will run a configuration, if it is not
     already in the database. You can also split this into `check` and
     `run`. This may be advised if you want to distribute the execution.
 
-    ```python
-    from algbench import Benchmark
-
-    benchmark = Benchmark("./test_benchmark")
-
-
-    def f(x, _test=2, default="default"):
-        print(x)  # here you would run your algorithm
-        return {"r1": x, "r2": "test"}
-
-
-    benchmark.add(f, 1, _test=None)
-    benchmark.add(f, 2)
-    benchmark.add(f, 3, _test=None)
-
-    benchmark.compress()
-
-    for entry in benchmark:
-        print(entry["parameters"], entry["data"])
-    ```
-
     The following functions are thread-safe:
     - exists
     - run
     - add
     - insert
     - front
     - __iter__
```

### Comparing `AlgBench-0.1.3/src/algbench/db/json_serializer.py` & `AlgBench-1.0.0/src/algbench/db/json_serializer.py`

 * *Files identical despite different names*

### Comparing `AlgBench-0.1.3/src/algbench/db/nfs_json_dict.py` & `AlgBench-1.0.0/src/algbench/db/nfs_json_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,51 @@
-from .nfs_json_list import NfsJsonList
-
 from .json_serializer import to_json
+from .nfs_json_list import NfsJsonList
 import typing
 
 
-class NfsJsonDict:
+class NfsJsonSet:
     def __init__(self, path) -> None:
         self._db = NfsJsonList(path)
-        self._values: typing.Dict = dict()
+        self._values: typing.Set = set()
         self.load()
 
     def load(self):
-        data = self._db.load()
-        for d in data:
-            if not isinstance(d, dict):
-                raise ValueError(
-                    "Found data that is not a dict. "
-                    "Are you sure this is a NfsJsonDict-database?"
-                )
-            self._values.update(d)
+        for row in self._db.load():
+            self._values.update(row)
 
     def __contains__(self, item):
         return item in self._values
 
-    def __setitem__(self, key, value):
-        key = str(key)
-        value = to_json(value)
-        self._db.append({key: value})
-        self._values[key] = value
-
-    def __getitem__(self, key):
-        return self._values[key]
-
-    def get(self, *args, **kwargs):
-        return self._values.get(*args, **kwargs)
-
-    def update(self, *args, **kwargs):
-        return self._values.update(*args, **kwargs)
-
-    def items(self):
-        for key, value in self._values.items():
-            yield key, value
+    def add(self, item):
+        item = to_json(item)
+        if item not in self._values:
+            self._db.append([item], flush=False)
+            self._values.add(item)
+        return item
+
+    def update(self, items):
+        for item in items:
+            self.add(item)
+
+    def __iter__(self):
+        for item in self._values:
+            yield item
 
     def compress(self):
+        """
+        WARNING: This operation is not thread-safe!
+        """
         self.load()  # in case there have been writes in the meantime
         self._db.clear()
-        self._db.append(self._values)
+        self._db.append(list(self._values))
         self._db.compress()
 
     def clear(self):
         self._db.clear()
+        self._values.clear()
+
+    def flush(self):
+        self._db.flush()
 
     def delete(self):
         self._db.delete()
```

### Comparing `AlgBench-0.1.3/src/algbench/db/nfs_json_list.py` & `AlgBench-1.0.0/src/algbench/db/nfs_json_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,8 +163,9 @@
                 continue
             os.remove(path)
 
     def __del__(self):
         self.flush()
 
     def delete(self):
+        self._cache.clear()
         shutil.rmtree(self.path)
```

### Comparing `AlgBench-0.1.3/src/algbench/environment.py` & `AlgBench-1.0.0/src/algbench/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import os
 import socket
 import subprocess
 import sys
 import typing
 import pkg_resources
+import __main__
 
 __cached = None
 
 
 def get_git_revision() -> typing.Optional[str]:
     """
     Return the git revision of the current working directory.
@@ -46,9 +47,10 @@
                 "name": str(pkg.project_name),
                 "path": str(pkg.location),
                 "version": str(pkg.parsed_version),
             }
             for pkg in pkg_resources.working_set
         ],
         "git_revision": get_git_revision(),
+        "python_file": __main__.__file__,
     }
     return __cached
```

### Comparing `AlgBench-0.1.3/src/algbench/pandas.py` & `AlgBench-1.0.0/src/algbench/pandas.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,23 +29,15 @@
 def describe(path: str):
     """
     Describe the benchmark by printing the first entry.
     """
     entry = Benchmark(path).front()
     if not entry:
         return
-    parameters = entry["parameters"]
-    print("parameters:")
-    _describe_data(parameters, 1, 10, 5)
-    env = entry["env"]
-    print("env:")
-    _describe_data(env, 1, 5, 3)
-    data = entry["data"]
-    print("data:")
-    _describe_data(data, 1, 20, 5)
+    _describe_data(entry, 0, 20, 5)
 
 
 def read_as_pandas(
     path: str, row_creator: typing.Callable[[typing.Dict], typing.Dict]
 ) -> pd.DataFrame:
     """
     Read the benchmark as pandas table.
```

### Comparing `AlgBench-0.1.3/src/algbench/utils/timer.py` & `AlgBench-1.0.0/src/algbench/utils/timer.py`

 * *Files identical despite different names*

