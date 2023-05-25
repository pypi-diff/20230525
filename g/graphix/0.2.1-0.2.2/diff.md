# Comparing `tmp/graphix-0.2.1.tar.gz` & `tmp/graphix-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix-0.2.1.tar", last modified: Tue Apr 25 07:36:33 2023, max compression
+gzip compressed data, was "graphix-0.2.2.tar", last modified: Thu May 25 00:15:50 2023, max compression
```

## Comparing `graphix-0.2.1.tar` & `graphix-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.241831 graphix-0.2.1/
--rw-r--r--   0 ss         (501) staff       (20)    10766 2023-04-25 07:26:44.000000 graphix-0.2.1/LICENSE
--rw-r--r--   0 ss         (501) staff       (20)       94 2022-12-15 06:51:32.000000 graphix-0.2.1/MANIFEST.in
--rw-r--r--   0 ss         (501) staff       (20)     5510 2023-04-25 07:36:33.241436 graphix-0.2.1/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)     4576 2023-04-25 07:20:26.000000 graphix-0.2.1/README.md
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.214418 graphix-0.2.1/docs/
--rw-r--r--   0 ss         (501) staff       (20)      638 2022-12-02 15:18:40.000000 graphix-0.2.1/docs/Makefile
--rw-r--r--   0 ss         (501) staff       (20)      804 2022-12-02 15:18:40.000000 graphix-0.2.1/docs/make.bat
--rw-r--r--   0 ss         (501) staff       (20)     1294 2023-01-09 01:14:11.000000 graphix-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.226204 graphix-0.2.1/graphix/
--rw-r--r--   0 ss         (501) staff       (20)      247 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/__init__.py
--rw-r--r--   0 ss         (501) staff       (20)     7451 2023-01-14 13:01:46.000000 graphix-0.2.1/graphix/clifford.py
--rw-r--r--   0 ss         (501) staff       (20)     4173 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/generator.py
--rw-r--r--   0 ss         (501) staff       (20)    13035 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/gflow.py
--rw-r--r--   0 ss         (501) staff       (20)    13678 2023-01-14 13:01:46.000000 graphix-0.2.1/graphix/graphsim.py
--rw-r--r--   0 ss         (501) staff       (20)     2463 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/ops.py
--rw-r--r--   0 ss         (501) staff       (20)    46518 2023-04-07 01:21:59.000000 graphix-0.2.1/graphix/pattern.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.232022 graphix-0.2.1/graphix/sim/
--rw-r--r--   0 ss         (501) staff       (20)        0 2022-12-12 11:17:35.000000 graphix-0.2.1/graphix/sim/__init__.py
--rw-r--r--   0 ss         (501) staff       (20)    11313 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/sim/statevec.py
--rw-r--r--   0 ss         (501) staff       (20)    25419 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/sim/tensornet.py
--rw-r--r--   0 ss         (501) staff       (20)     2269 2023-03-01 11:13:38.000000 graphix-0.2.1/graphix/simulator.py
--rw-r--r--   0 ss         (501) staff       (20)    37241 2023-03-16 06:55:32.000000 graphix-0.2.1/graphix/transpiler.py
--rw-r--r--   0 ss         (501) staff       (20)       22 2023-04-25 06:52:17.000000 graphix-0.2.1/graphix/version.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.229563 graphix-0.2.1/graphix.egg-info/
--rw-r--r--   0 ss         (501) staff       (20)     5510 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)      681 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/SOURCES.txt
--rw-r--r--   0 ss         (501) staff       (20)        1 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/dependency_links.txt
--rw-r--r--   0 ss         (501) staff       (20)       85 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/requires.txt
--rw-r--r--   0 ss         (501) staff       (20)        8 2023-04-25 07:36:33.000000 graphix-0.2.1/graphix.egg-info/top_level.txt
--rw-r--r--   0 ss         (501) staff       (20)       81 2022-12-15 06:51:32.000000 graphix-0.2.1/pyproject.toml
--rw-r--r--   0 ss         (501) staff       (20)       38 2023-04-25 07:36:33.241956 graphix-0.2.1/setup.cfg
--rw-r--r--   0 ss         (501) staff       (20)     1488 2022-12-21 06:16:27.000000 graphix-0.2.1/setup.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-04-25 07:36:33.240319 graphix-0.2.1/tests/
--rw-r--r--   0 ss         (501) staff       (20)     2904 2023-01-14 13:01:46.000000 graphix-0.2.1/tests/test_clifford.py
--rw-r--r--   0 ss         (501) staff       (20)     2963 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_generator.py
--rw-r--r--   0 ss         (501) staff       (20)     2479 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_gflow.py
--rw-r--r--   0 ss         (501) staff       (20)     3974 2022-12-15 11:43:28.000000 graphix-0.2.1/tests/test_graphsim.py
--rw-r--r--   0 ss         (501) staff       (20)     7565 2023-04-07 01:21:59.000000 graphix-0.2.1/tests/test_pattern.py
--rw-r--r--   0 ss         (501) staff       (20)    15835 2023-03-01 11:13:38.000000 graphix-0.2.1/tests/test_tnsim.py
--rw-r--r--   0 ss         (501) staff       (20)     5102 2023-01-14 13:01:46.000000 graphix-0.2.1/tests/test_transpiler.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.736813 graphix-0.2.2/
+-rw-r--r--   0 ss         (501) staff       (20)    10761 2023-04-29 07:04:06.000000 graphix-0.2.2/LICENSE
+-rw-r--r--   0 ss         (501) staff       (20)       94 2022-12-15 06:51:32.000000 graphix-0.2.2/MANIFEST.in
+-rw-r--r--   0 ss         (501) staff       (20)     5510 2023-05-25 00:15:50.736242 graphix-0.2.2/PKG-INFO
+-rw-r--r--   0 ss         (501) staff       (20)     4576 2023-04-25 07:20:26.000000 graphix-0.2.2/README.md
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.669115 graphix-0.2.2/docs/
+-rw-r--r--   0 ss         (501) staff       (20)      638 2022-12-02 15:18:40.000000 graphix-0.2.2/docs/Makefile
+-rw-r--r--   0 ss         (501) staff       (20)      804 2022-12-02 15:18:40.000000 graphix-0.2.2/docs/make.bat
+-rw-r--r--   0 ss         (501) staff       (20)     1294 2023-01-09 01:14:11.000000 graphix-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.709185 graphix-0.2.2/graphix/
+-rw-r--r--   0 ss         (501) staff       (20)      247 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/__init__.py
+-rw-r--r--   0 ss         (501) staff       (20)     7451 2023-01-14 13:01:46.000000 graphix-0.2.2/graphix/clifford.py
+-rw-r--r--   0 ss         (501) staff       (20)     4173 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/generator.py
+-rw-r--r--   0 ss         (501) staff       (20)    13035 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/gflow.py
+-rw-r--r--   0 ss         (501) staff       (20)    13678 2023-01-14 13:01:46.000000 graphix-0.2.2/graphix/graphsim.py
+-rw-r--r--   0 ss         (501) staff       (20)     2463 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/ops.py
+-rw-r--r--   0 ss         (501) staff       (20)    64919 2023-05-25 00:12:26.000000 graphix-0.2.2/graphix/pattern.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.715511 graphix-0.2.2/graphix/sim/
+-rw-r--r--   0 ss         (501) staff       (20)        0 2022-12-12 11:17:35.000000 graphix-0.2.2/graphix/sim/__init__.py
+-rw-r--r--   0 ss         (501) staff       (20)    11313 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/sim/statevec.py
+-rw-r--r--   0 ss         (501) staff       (20)    26198 2023-05-25 00:12:26.000000 graphix-0.2.2/graphix/sim/tensornet.py
+-rw-r--r--   0 ss         (501) staff       (20)     2269 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/simulator.py
+-rw-r--r--   0 ss         (501) staff       (20)    37241 2023-03-16 06:55:32.000000 graphix-0.2.2/graphix/transpiler.py
+-rw-r--r--   0 ss         (501) staff       (20)       22 2023-05-25 00:12:43.000000 graphix-0.2.2/graphix/version.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.712842 graphix-0.2.2/graphix.egg-info/
+-rw-r--r--   0 ss         (501) staff       (20)     5510 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/PKG-INFO
+-rw-r--r--   0 ss         (501) staff       (20)      681 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/SOURCES.txt
+-rw-r--r--   0 ss         (501) staff       (20)        1 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/dependency_links.txt
+-rw-r--r--   0 ss         (501) staff       (20)       85 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/requires.txt
+-rw-r--r--   0 ss         (501) staff       (20)        8 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/top_level.txt
+-rw-r--r--   0 ss         (501) staff       (20)       81 2022-12-15 06:51:32.000000 graphix-0.2.2/pyproject.toml
+-rw-r--r--   0 ss         (501) staff       (20)       38 2023-05-25 00:15:50.737027 graphix-0.2.2/setup.cfg
+-rw-r--r--   0 ss         (501) staff       (20)     1488 2023-05-16 06:15:33.000000 graphix-0.2.2/setup.py
+drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.734735 graphix-0.2.2/tests/
+-rw-r--r--   0 ss         (501) staff       (20)     2904 2023-01-14 13:01:46.000000 graphix-0.2.2/tests/test_clifford.py
+-rw-r--r--   0 ss         (501) staff       (20)     2986 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_generator.py
+-rw-r--r--   0 ss         (501) staff       (20)     2479 2023-04-07 01:21:59.000000 graphix-0.2.2/tests/test_gflow.py
+-rw-r--r--   0 ss         (501) staff       (20)     3974 2022-12-15 11:43:28.000000 graphix-0.2.2/tests/test_graphsim.py
+-rw-r--r--   0 ss         (501) staff       (20)    15790 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_pattern.py
+-rw-r--r--   0 ss         (501) staff       (20)    15778 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_tnsim.py
+-rw-r--r--   0 ss         (501) staff       (20)     5102 2023-01-14 13:01:46.000000 graphix-0.2.2/tests/test_transpiler.py
```

### Comparing `graphix-0.2.1/LICENSE` & `graphix-0.2.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   Copyright 2022-2023 Shinichi Sunami
+   Copyright 2022 Shinichi Sunami
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `graphix-0.2.1/PKG-INFO` & `graphix-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
```

### Comparing `graphix-0.2.1/README.md` & `graphix-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/docs/Makefile` & `graphix-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/docs/make.bat` & `graphix-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/docs/requirements.txt` & `graphix-0.2.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/clifford.py` & `graphix-0.2.2/graphix/clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/generator.py` & `graphix-0.2.2/graphix/generator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/gflow.py` & `graphix-0.2.2/graphix/gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/graphsim.py` & `graphix-0.2.2/graphix/graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/ops.py` & `graphix-0.2.2/graphix/ops.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/pattern.py` & `graphix-0.2.2/graphix/pattern.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,23 +43,23 @@
             attr for Z: signal_domain
             attr for S: signal_domain
             attr for C: clifford_index, as defined in :py:mod:`graphix.clifford`
     Nnode : int
         total number of nodes in the resource state
     """
 
-    def __init__(self, width=0):
+    def __init__(self, width=0, output_nodes=[]):
         """
         :param width:  number of input/output qubits
         """
         # number of input qubits
         self.width = width
         self.seq = [["N", i] for i in range(width)]  # where command sequence is stored
         self.results = {}  # measurement results from the graph state simulator
-        self.output_nodes = []  # output nodes
+        self.output_nodes = output_nodes  # output nodes
         self.Nnode = width  # total number of nodes in the graph state
 
     def add(self, cmd):
         """add command to the end of the pattern.
         an MBQC command is specified by a list of [type, node, attr], where
 
             type : 'N', 'M', 'E', 'X', 'Z', 'S' or 'C'
@@ -173,22 +173,89 @@
             elif self.seq[i][0] == "C" and ("C" in filter):
                 count += 1
                 print(f"Clifford, node = {self.seq[i][1]}, Clifford index = {self.seq[i][2]}")
 
         if len(self.seq) > i + 1:
             print(f"{len(self.seq)-lim} more commands truncated. Change lim argument of print_pattern() to show more")
 
-    def standardize(self):
+    def get_local_pattern(self):
+        """Get a local pattern transpiled from the pattern.
+
+        Returns
+        -------
+        localpattern : LocalPattern
+            transpiled local pattern.
+        """
+        standardized = self.is_standard()
+        node_prop = dict()
+        morder = []
+        for cmd in self.seq:
+            if cmd[0] == "N":
+                node_prop[cmd[1]] = {
+                    "seq": [],
+                    "Mprop": [None, None, [], [], 0],
+                    "Xsignal": [],
+                    "Xsignals": [],
+                    "Zsignal": [],
+                    "output": False,
+                }
+            elif cmd[0] == "E":
+                node_prop[cmd[1][1]]["seq"].append(cmd[1][0])
+                node_prop[cmd[1][0]]["seq"].append(cmd[1][1])
+            elif cmd[0] == "M":
+                node_prop[cmd[1]]["Mprop"] = cmd[2:]
+                node_prop[cmd[1]]["seq"].append(-1)
+                morder.append(cmd[1])
+            elif cmd[0] == "X":
+                if standardized:
+                    node_prop[cmd[1]]["Xsignal"] += cmd[2]
+                    node_prop[cmd[1]]["Xsignals"] += [cmd[2]]
+                else:
+                    node_prop[cmd[1]]["Xsignals"].append(cmd[2])
+                node_prop[cmd[1]]["seq"].append(-2)
+            elif cmd[0] == "Z":
+                node_prop[cmd[1]]["Zsignal"] += cmd[2]
+                node_prop[cmd[1]]["seq"].append(-3)
+            elif cmd[0] == "C":
+                node_prop[cmd[1]]["vop"] = cmd[2]
+                node_prop[cmd[1]]["seq"].append(-4)
+            elif cmd[0] == "S":
+                raise NotImplementedError()
+            else:
+                raise ValueError(f"command {cmd} is invalid!")
+        nodes = dict()
+        for index in node_prop.keys():
+            if index in self.output_nodes:
+                node_prop[index]["output"] = True
+            node = CommandNode(index, **node_prop[index])
+            nodes[index] = node
+        return LocalPattern(nodes, self.output_nodes, morder)
+
+    def standardize(self, method="local"):
         """Executes standardization of the pattern.
         'standard' pattern is one where commands are sorted in the order of
         'N', 'E', 'M' and then byproduct commands ('X' and 'Z').
-        """
-        self._move_N_to_left()
-        self._move_byproduct_to_right()
-        self._move_E_after_N()
+
+        Parameters
+        ----------
+        method : str, optional
+            'global' corresponds to a conventional standardization executed on Pattern class.
+            'local' standardization is executed on LocalPattern class. In all cases, local pattern standardization is significantly faster than conventional one.
+            defaults to 'local'
+        """
+        if method == "local":
+            localpattern = self.get_local_pattern()
+            localpattern.standardize()
+            self.seq = localpattern.get_pattern().seq
+        elif method == "global":
+            self._move_N_to_left()
+            self._move_byproduct_to_right()
+            self._move_E_after_N()
+        else:
+            raise ValueError("Invalid method")
 
     def is_standard(self):
         """determines whether the command sequence is standard
 
         Returns
         -------
         is_standard : bool
@@ -206,45 +273,57 @@
         op_ref = "N"
         for cmd in self.seq:
             op = cmd[0]
             result = result & (op in order_dict[op_ref])
             op_ref = op
         return result
 
-    def shift_signals(self):
+    def shift_signals(self, method="local"):
         """Performs signal shifting procedure
         Extract the t-dependence of the measurement into 'S' commands
-        and commute them towards the end of the command sequence,
-        where it can be deleted.
-        In many cases, this procedure simplifies the dependence structure
-        of the pattern. For patterns transpiled from gate sequencees,
-        this result in the removal of s- and t- domains on Pauli measurement commands.
+        and commute them to the end of the command sequence where it can be removed.
+        This procedure simplifies the dependence structure of the pattern.
 
-        Ref: V. Danos, E. Kashefi and P. Panangaden. J. ACM 54.2 8 (2007)
-        """
-        if not self.is_standard():
-            self.standardize()
-        self.extract_signals()
-        target = self._find_op_to_be_moved("S", rev=True)
-        while target != "end":
-            if target == len(self.seq) - 1:
-                self.seq.pop(target)
-                target = self._find_op_to_be_moved("S", rev=True)
-                continue
-            if self.seq[target + 1][0] == "X":
-                self._commute_XS(target)
-            elif self.seq[target + 1][0] == "Z":
-                self._commute_ZS(target)
-            elif self.seq[target + 1][0] == "M":
-                self._commute_MS(target)
-            elif self.seq[target + 1][0] == "S":
-                self._commute_SS(target)
-            else:
-                self._commute_with_following(target)
-            target += 1
+        Ref for the original 'global' method:
+            V. Danos, E. Kashefi and P. Panangaden. J. ACM 54.2 8 (2007)
+        Ref for the 'local' method:
+            S. Sunami and M. Fukushima, in preparation
+
+        Parameters
+        ----------
+        method : str, optional
+            'global' shift_signals is executed on a conventional Pattern sequence.
+            'local' shift_signals is done on a LocalPattern class which is faster but results in equivalent pattern.
+            defaults to 'local'
+        """
+        if method == "local":
+            localpattern = self.get_local_pattern()
+            localpattern.shift_signals()
+            self.seq = localpattern.get_pattern().seq
+        elif method == "global":
+            self.extract_signals()
+            target = self._find_op_to_be_moved("S", rev=True)
+            while target != "end":
+                if target == len(self.seq) - 1:
+                    self.seq.pop(target)
+                    target = self._find_op_to_be_moved("S", rev=True)
+                    continue
+                if self.seq[target + 1][0] == "X":
+                    self._commute_XS(target)
+                elif self.seq[target + 1][0] == "Z":
+                    self._commute_ZS(target)
+                elif self.seq[target + 1][0] == "M":
+                    self._commute_MS(target)
+                elif self.seq[target + 1][0] == "S":
+                    self._commute_SS(target)
+                else:
+                    self._commute_with_following(target)
+                target += 1
+        else:
+            raise ValueError("Invalid method")
 
     def _find_op_to_be_moved(self, op, rev=False, skipnum=0):
         """Internal method for pattern modification.
 
         Parameters
         ----------
         op : str, 'N', 'E', 'M', 'X', 'Z', 'S'
@@ -792,14 +871,30 @@
                     for axis in mplane:
                         converted = order[clifford_measure[order.index(axis)][0]]
                         converted_mplane += converted
                     mplane = "".join(sorted(converted_mplane))
                 meas_plane[cmd[1]] = mplane
         return meas_plane
 
+    def get_max_degree(self):
+        """Get max degree of a pattern
+
+        Returns
+        -------
+        max_degree : int
+            max degree of a pattern
+        """
+        nodes, edges = self.get_graph()
+        g = nx.Graph()
+        g.add_nodes_from(nodes)
+        g.add_edges_from(edges)
+        degree = g.degree()
+        max_degree = max([i for i in dict(degree).values()])
+        return max_degree
+
     def get_graph(self):
         """returns the list of nodes and edges from the command sequence,
         extracted from 'N' and 'E' commands.
 
         Returns
         -------
         node_list : list
@@ -904,14 +999,35 @@
                         node_list.append(self.seq[ind][1][1])
                 elif self.seq[ind][1][1] == node:
                     if not self.seq[ind][1][0] in prepared:
                         node_list.append(self.seq[ind][1][0])
                 ind += 1
         return node_list
 
+    def standardize_and_shift_signals(self, method="local"):
+        """Executes standardization and signal shifting.
+
+        Parameters
+        ----------
+        method : str, optional
+            'global' corresponds to a conventional method executed on Pattern class.
+            'local' standardization is executed on LocalPattern class.
+            defaults to 'local'
+        """
+        if method == "local":
+            localpattern = self.get_local_pattern()
+            localpattern.standardize()
+            localpattern.shift_signals()
+            self.seq = localpattern.get_pattern().seq
+        elif method == "global":
+            self.standardize()
+            self.shift_signals()
+        else:
+            raise ValueError("Invalid method")
+
     def correction_commands(self):
         """Returns the list of byproduct correction commands"""
         assert self.is_standard()
         Clist = []
         for i in range(len(self.seq)):
             if self.seq[i][0] in ["X", "Z"]:
                 Clist.append(self.seq[i])
@@ -1076,14 +1192,417 @@
                     file.write("bit c" + str(id) + " = " + str(res) + ";\n")
                     file.write("\n")
             for command in self.seq:
                 for line in cmd_to_qasm3(command):
                     file.write(line)
 
 
+class CommandNode:
+    """A node decorated with a distributed command sequence.
+
+    Attributes
+    ----------
+    index : int
+        node index
+    seq : list
+        command sequence. In this class, a command sequence follows the rules noted below.
+
+        E: pair node's index(>=0)
+        M: -1
+        X: -2
+        Z: -3
+        C: -4
+    Mprop : list
+        attributes for a measurement command. consists of [meas_plane, angle, s_domain, t_domain, vop]
+    result : int
+        measurement result of the node
+    Xsignal : list
+        signal domain
+    Xsignals : list
+        signal domain. Xsignals may contains lists. For standardization, this variable is used.
+    Zsignal : list
+        signal domain
+    vop : int
+        value for clifford index
+    output : bool
+        whether the node is an output or not
+    """
+
+    def __init__(self, node_index, seq, Mprop, Zsignal, output, Xsignal=[], Xsignals=[]):
+        """
+        Parameters
+        ----------
+        node_index : int
+            node index
+
+        seq : list
+            distributed command sequence
+
+        Mprop : list
+            attributes for measurement command
+
+        Xsignal : list
+            signal domain for X byproduct correction
+
+        Xsignals : list of list
+            signal domains for X byproduct correction
+            Xsignal or Xsignals must be specified
+
+        Zsignal : list
+            signal domain for Z byproduct correction
+
+        output : bool
+            whether the node is an output or not
+        """
+        self.index = node_index
+        self.seq = seq  # composed of [E, M, X, Z, C]
+        self.Mprop = Mprop
+        self.result = None
+        self.Xsignal = Xsignal
+        self.Xsignals = Xsignals
+        self.Zsignal = Zsignal  # appeared at most e + 1
+        self.vop = Mprop[4] if len(Mprop) == 5 else 0
+        self.output = output
+
+    def is_standard(self):
+        """Check whether the local command sequence is standardized.
+
+        Returns
+        -------
+        standardized : Bool
+            whether the local command sequence is standardized or not
+        """
+        order_dict = {
+            -1: [-1, -2, -3, -4],
+            -2: [-2, -3, -4],
+            -3: [-2, -3, -4],
+            -4: [-4],
+        }
+        standardized = True
+        cmd_ref = 0
+        for cmd in self.seq:
+            if cmd_ref >= 0:
+                pass
+            else:
+                standardized &= cmd in order_dict[cmd_ref]
+            cmd_ref = cmd
+        return standardized
+
+    def commute_X(self):
+        """Move all X correction commands to the back.
+
+        Returns
+        -------
+        EXcommutated_nodes : dict
+            when X commutes with E, Z correction is added on the pair node. This dict specifies target nodes where Zs will be added.
+        """
+        EXcommutated_nodes = dict()
+        combined_Xsignal = []
+        for Xsignal in self.Xsignals:
+            Xpos = self.seq.index(-2)
+            for i in range(Xpos, len(self.seq)):
+                if self.seq[i] >= 0:
+                    try:
+                        EXcommutated_nodes[self.seq[i]] += Xsignal
+                    except KeyError:
+                        EXcommutated_nodes[self.seq[i]] = Xsignal
+            self.seq.remove(-2)
+            combined_Xsignal += Xsignal
+        if self.output:
+            self.seq.append(-2)  # put X on the end of the pattern
+            self.Xsignal = combined_Xsignal
+            self.Xsignals = [combined_Xsignal]
+        else:
+            if self.Mprop[0] == "YZ" or self.vop == 6:
+                self.Mprop[3] = xor_combination_list(combined_Xsignal, self.Mprop[3])
+            elif self.Mprop[0] == "XY":
+                self.Mprop[2] = xor_combination_list(combined_Xsignal, self.Mprop[2])
+            self.Xsignal = []
+            self.Xsignals = []
+        return EXcommutated_nodes
+
+    def commute_Z(self):
+        """Move all Zs to the back. EZ commutation produces no additional command unlike EX commutation."""
+        z_in_seq = False
+        while -3 in self.seq:
+            z_in_seq = True
+            self.seq.remove(-3)
+        if self.output and z_in_seq:
+            self.seq.append(-3)
+        else:
+            if self.Mprop[0] == "YZ" or self.vop == 6:
+                self.Mprop[2] = xor_combination_list(self.Zsignal, self.Mprop[2])
+            elif self.Mprop[0] == "XY":
+                self.Mprop[3] = xor_combination_list(self.Zsignal, self.Mprop[3])
+            self.Zsignal = []
+
+    def _add_Z(self, pair, signal):
+        """Add Z correction into the node.
+
+        Parameters
+        ----------
+        pair : int
+            a node index where the Z is produced. The additional Z will be inserted just behind the E(with pair) command
+        signal : list
+            signal domain for the additional Z correction
+        """
+        # caused by EX commutation.
+        self.Zsignal = xor_combination_list(signal, self.Zsignal)
+        Epos = self.seq.index(pair)
+        self.seq.insert(Epos + 1, -3)
+
+    def print_pattern(self):
+        """Print the local command sequence"""
+        for cmd in self.seq:
+            print(self.get_command(cmd))
+
+    def get_command(self, cmd):
+        """Get a command with full description. Patterns with more than one X or Z corrections are not supported.
+
+        Parameters
+        ----------
+        cmd : int
+            an integer corresponds to a command as described below.
+            E: pair node's index(>=0)
+            M: -1
+            X: -2
+            Z: -3
+            C: -4
+
+        Returns
+        -------
+        MBQC command : list
+            a command for a global pattern
+        """
+        if cmd >= 0:
+            return ["E", (self.index, cmd)]
+        elif cmd == -1:
+            return ["M", self.index] + self.Mprop
+        elif cmd == -2:
+            if self.seq.count(-2) > 1:
+                raise NotImplementedError("Patterns with more than one X corrections are not supported")
+            return ["X", self.index, self.Xsignal]
+        elif cmd == -3:
+            if self.seq.count(-3) > 1:
+                raise NotImplementedError("Patterns with more than one Z corrections are not supported")
+            return ["Z", self.index, self.Zsignal]
+        elif cmd == -4:
+            return ["C", self.index, self.vop]
+
+    def get_signal_destination(self):
+        """get signal destination
+
+        Returns
+        -------
+        signal_destination : set
+            Counterpart of 'dependent nodes'. measurement results of each node propagate to the nodes specified by 'signal_distination'.
+        """
+        signal_destination = set(self.Mprop[2]) | set(self.Mprop[3]) | set(self.Xsignal) | set(self.Zsignal)
+        return signal_destination
+
+    def get_signal_destination_dict(self):
+        """get signal destination. distinguish the kind of signals.
+
+        Returns
+        -------
+        signal_destination_dict : dict
+            Counterpart of 'dependent nodes'. Unlike 'get_signal_destination', types of domains are memorarized. measurement results of each node propagate to the nodes specified by 'signal_distination_dict'.
+        """
+        dependent_nodes_dict = dict()
+        dependent_nodes_dict["Ms"] = self.Mprop[2]
+        dependent_nodes_dict["Mt"] = self.Mprop[3]
+        dependent_nodes_dict["X"] = self.Xsignal
+        dependent_nodes_dict["Z"] = self.Zsignal
+        return dependent_nodes_dict
+
+
+class LocalPattern:
+    """MBQC Local Pattern class
+
+    Instead of storing commands as a 1D list as in Pattern class, here we distribute them to each node.
+    This data structure is efficient for command operations such as commutation and signal propagation.
+    This results in faster standardization and signal shifting.
+
+    Attributes
+    ----------
+    nodes : set
+        set of nodes with distributed command sequences
+
+    output_nodes : list
+        list of output node indices.
+
+    morder : list
+        list of node indices in a measurement order.
+
+    signal_destination : dict
+       stores the set of nodes where dependent feedforward operations are performed, from the result of measurement at each node.
+       stored separately for each nodes, and for each kind of signal(Ms, Mt, X, Z).
+    """
+
+    def __init__(self, nodes=dict(), output_nodes=[], morder=[]):
+        """
+        Parameters
+        ----------
+        nodes : dict
+            dict of command decorated nodes. defaults to an empty dict.
+        output_nodes : list, optional
+            list of output node indices. defaults to [].
+        morder : list, optional
+            list of node indices in a measurement order. defaults to [].
+        """
+        self.nodes = nodes  # dict of Pattern.CommandNode
+        self.output_nodes = output_nodes
+        self.morder = morder
+        self.signal_destination = {i: {"Ms": set(), "Mt": set(), "X": set(), "Z": set()} for i in self.nodes.keys()}
+
+    def is_standard(self):
+        """Check whether the local pattern is standardized or not
+
+        Returns
+        -------
+        standardized : bool
+            whether the local pattern is standardized or not
+        """
+        standardized = True
+        for node in self.nodes.values():
+            standardized &= node.is_standard()
+        return standardized
+
+    def Xshift(self):
+        """Move X to the back of the pattern"""
+        for index, node in self.nodes.items():
+            EXcomutation = node.commute_X()
+            for target_index, signal in EXcomutation.items():
+                self.nodes[target_index]._add_Z(index, signal)
+
+    def Zshift(self):
+        """Move Z to the back of the pattern. This method can be executed separately"""
+        for node in self.nodes.values():
+            node.commute_Z()
+
+    def standardize(self):
+        """Standardize pattern. In this structure, it is enough to move all byproduct corrections to the back"""
+        self.Xshift()
+        self.Zshift()
+
+    def collect_signal_destination(self):
+        """Calculate signal destinations by considering dependencies of each node."""
+        for index, node in self.nodes.items():
+            dependent_node_dicts = node.get_signal_destination_dict()
+            for dependent_node in dependent_node_dicts["Ms"]:
+                self.signal_destination[dependent_node]["Ms"] |= {index}
+            for dependent_node in dependent_node_dicts["Mt"]:
+                self.signal_destination[dependent_node]["Mt"] |= {index}
+            for dependent_node in dependent_node_dicts["X"]:
+                self.signal_destination[dependent_node]["X"] |= {index}
+            for dependent_node in dependent_node_dicts["Z"]:
+                self.signal_destination[dependent_node]["Z"] |= {index}
+
+    def shift_signals(self):
+        """Shift signals to the back based on signal destinations."""
+        self.collect_signal_destination()
+        for node_index in self.morder + self.output_nodes:
+            signal = self.nodes[node_index].Mprop[3]
+            self.nodes[node_index].Mprop[3] = []
+            for signal_label, destinated_nodes in self.signal_destination[node_index].items():
+                for destinated_node in destinated_nodes:
+                    node = self.nodes[destinated_node]
+                    if signal_label == "Ms":
+                        node.Mprop[2] += signal
+                    elif signal_label == "Mt":
+                        node.Mprop[3] += signal
+                    elif signal_label == "X":
+                        node.Xsignal += signal
+                    elif signal_label == "Z":
+                        node.Zsignal += signal
+                    else:
+                        raise ValueError(f"Invalid signal label: {signal_label}")
+
+    def get_graph(self):
+        """Get a graph from a local pattern
+
+        Returns
+        -------
+        nodes : list
+            list of node indices
+        edges : list
+            list of edges
+        """
+        nodes = []
+        edges = []
+        for index, node in self.nodes.items():
+            nodes.append(index)
+            for cmd in node.seq:
+                if cmd >= 0:
+                    if index > cmd:
+                        edges.append((cmd, index))
+        return nodes, edges
+
+    def get_pattern(self):
+        """Convert a local pattern into a corresponding global pattern. Currently, only standardized pattern is supported.
+
+        Returns
+        -------
+        pattern : Pattern
+            standardized global pattern
+        """
+        assert self.is_standard()
+        pattern = Pattern(output_nodes=self.output_nodes)
+        Nseq = [["N", i] for i in self.nodes.keys()]
+        Eseq = []
+        Mseq = []
+        Xseq = []
+        Zseq = []
+        Cseq = []
+        for node_index in self.morder + self.output_nodes:
+            node = self.nodes[node_index]
+            for cmd in node.seq:
+                if cmd >= 0:
+                    Eseq.append(node.get_command(cmd))
+                    self.nodes[cmd].seq.remove(node_index)
+                elif cmd == -1:
+                    Mseq.append(node.get_command(cmd))
+                elif cmd == -2:
+                    Xseq.append(node.get_command(cmd))
+                elif cmd == -3:
+                    Zseq.append(node.get_command(cmd))
+                elif cmd == -4:
+                    Cseq.append(node.get_command(cmd))
+                else:
+                    raise ValueError(f"command {cmd} is invalid!")
+            if node.result is not None:
+                pattern.results[node.index] = node.result
+        pattern.seq = Nseq + Eseq + Mseq + Xseq + Zseq + Cseq
+        return pattern
+
+
+def xor_combination_list(list1, list2):
+    """Combine two lists according to XOR operation.
+
+    Parameters
+    ----------
+    list1 : list
+        list to be combined
+    list2 : list
+        list to be combined
+
+    Returns
+    -------
+    result : list
+        xor-combined list
+    """
+    result = list2
+    for elem in list1:
+        if elem in result:
+            result.remove(elem)
+        else:
+            result.append(elem)
+    return result
+
+
 def measure_pauli(pattern, copy=False):
     """Perform Pauli measurement of a pattern by fast graph state simulator
     uses the decorated-graph method implemented in graphix.graphsim to perform
     the measurements in Pauli bases, and then sort remaining nodes back into
     pattern together with Clifford commands.
 
     TODO: non-XY plane measurements in original pattern
@@ -1129,17 +1648,14 @@
         elif np.mod(angle, 2) == 1.5:  # -y measurement
             results[cmd[1]] = 1 - graph_state.measure_y(cmd[1], choice=1)
 
     # measure (remove) isolated nodes. if they aren't Pauli measurements,
     # measuring one of the results with probability of 1 should not occur as was possible above for Pauli measurements,
     # which means we can just choose s=0. We should not remove output nodes even if isolated.
     isolates = list(nx.isolates(graph_state))
-    # for i in isolates:
-    #     if i not in pattern.output_nodes:
-    #         # check whether this is Pauli measurement
     for cmd in non_pauli_meas:
         if (cmd[1] in isolates) and (cmd[1] not in pattern.output_nodes):
             graph_state.remove_node(cmd[1])
             results[cmd[1]] = 0
 
     # update command sequence
     vops = graph_state.get_vops()
```

### Comparing `graphix-0.2.1/graphix/sim/statevec.py` & `graphix-0.2.2/graphix/sim/statevec.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/sim/tensornet.py` & `graphix-0.2.2/graphix/sim/tensornet.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,45 +9,61 @@
 
 class TensorNetworkBackend:
     """Tensor Network Simulator for MBQC
 
     Executes the measurement pattern using TN expression of graph states.
     """
 
-    def __init__(self, pattern, graph_prep="opt", **kwargs):
+    def __init__(self, pattern, graph_prep="auto", **kwargs):
         """
 
         Parameters
         ----------
         pattern : graphix.Pattern
         graph_prep : str
-            'opt'(default) :
-                Faster and optimal method to prepare a tensornetwork representing graph state.
-                The expression of the given graph state can be obtained from its geometry.
-                See https://journals.aps.org/pra/abstract/10.1103/PhysRevA.76.052315 for example.
-                Note that the 'N' and 'E' commands in the measurement pattern are ignored.
+            'parallel' :
+                Faster method for preparing a graph state.
+                The expression of a graph state can be obtained from the graph geometry.
+                See https://journals.aps.org/pra/abstract/10.1103/PhysRevA.76.052315 for detail calculation.
+                Note that 'N' and 'E' commands in the measurement pattern are ignored.
             'sequential' :
-                Sequentially add nodes and edges, strictly following the measuremen pattern.
+                Sequentially execute N and E commands, strictly following the measurement pattern.
                 In this strategy, All N and E commands executed sequentially.
+            'auto'(default) :
+                Automatically select a preparation strategy based on the max degree of a graph
         **kwargs : Additional keyword args to be passed to quimb.tensor.TensorNetwork.
         """
         self.pattern = pattern
         self.output_nodes = pattern.output_nodes
         self.results = deepcopy(pattern.results)
-        assert graph_prep in ["opt", "sequential"]
-        self.graph_prep = graph_prep
-        if graph_prep == "opt":
+        if graph_prep in ["parallel", "sequential"]:
+            self.graph_prep = graph_prep
+        elif graph_prep == "opt":
+            self.graph_prep = "parallel"
+            print(f"graph preparation strategy '{graph_prep}' is deprecated and will be replaced by 'parallel'")
+        elif graph_prep == "auto":
+            max_degree = pattern.get_max_degree()
+            if max_degree > 5:
+                self.graph_prep = "sequential"
+            else:
+                self.graph_prep = "parallel"
+        else:
+            raise ValueError(f"Invalid graph preparation strategy: {graph_prep}")
+
+        if self.graph_prep == "parallel":
+            if not pattern.is_standard():
+                raise ValueError("parallel preparation strategy does not support not-standardized pattern")
             nodes, edges = pattern.get_graph()
             self.state = MBQCTensorNet(
                 graph_nodes=nodes,
                 graph_edges=edges,
                 default_output_nodes=pattern.output_nodes,
                 **kwargs,
             )
-        elif graph_prep == "sequential":
+        elif self.graph_prep == "sequential":
             self.state = MBQCTensorNet(default_output_nodes=pattern.output_nodes, **kwargs)
             self._decomposed_cz = _get_decomposed_cz()
         self._isolated_nodes = pattern.get_isolated_nodes()
 
     def add_nodes(self, nodes):
         """Add nodes to the network
```

### Comparing `graphix-0.2.1/graphix/simulator.py` & `graphix-0.2.2/graphix/simulator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix/transpiler.py` & `graphix-0.2.2/graphix/transpiler.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/graphix.egg-info/PKG-INFO` & `graphix-0.2.2/graphix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.1
+Version: 0.2.2
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
```

### Comparing `graphix-0.2.1/graphix.egg-info/SOURCES.txt` & `graphix-0.2.2/graphix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/setup.py` & `graphix-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/tests/test_clifford.py` & `graphix-0.2.2/tests/test_clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/tests/test_generator.py` & `graphix-0.2.2/tests/test_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,33 +10,33 @@
         graph = nx.Graph([(0, 3), (1, 4), (2, 5), (1, 3), (2, 4), (3, 6), (4, 7), (5, 8)])
         inputs = {0, 1, 2}
         outputs = {6, 7, 8}
         angles = np.random.randn(6)
         results = []
         repeats = 3  # for testing the determinism of a pattern
         for _ in range(repeats):
-            pattern = generate_from_graph(graph, angles, inputs, outputs)
+            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs))
             pattern.standardize()
             pattern.minimize_space()
             state = pattern.simulate_pattern()
             results.append(state)
         combinations = [(0, 1), (0, 2), (1, 2)]
         for i, j in combinations:
             inner_product = np.dot(results[i].flatten(), results[j].flatten().conjugate())
             np.testing.assert_almost_equal(abs(inner_product), 1)
 
     def test_pattern_generation_determinism_gflow(self):
         graph = nx.Graph([(1, 2), (2, 3), (3, 4), (4, 5), (5, 6), (3, 6), (1, 6)])
         inputs = {1, 3, 5}
         outputs = {2, 4, 6}
-        angles = np.random.randn(11)
+        angles = np.random.randn(6)
         results = []
         repeats = 3  # for testing the determinism of a pattern
         for _ in range(repeats):
-            pattern = generate_from_graph(graph, angles, inputs, outputs)
+            pattern = generate_from_graph(graph, angles, list(inputs), list(outputs))
             pattern.standardize()
             pattern.minimize_space()
             state = pattern.simulate_pattern()
             results.append(state)
         combinations = [(0, 1), (0, 2), (1, 2)]
         for i, j in combinations:
             inner_product = np.dot(results[i].flatten(), results[j].flatten().conjugate())
```

### Comparing `graphix-0.2.1/tests/test_gflow.py` & `graphix-0.2.2/tests/test_gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/tests/test_graphsim.py` & `graphix-0.2.2/tests/test_graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.1/tests/test_tnsim.py` & `graphix-0.2.2/tests/test_tnsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import unittest
 import itertools
 import numpy as np
 from quimb.tensor import Tensor
 from graphix.transpiler import Circuit
-from graphix.pattern import Pattern
 from graphix.ops import Ops, States
-from graphix.sim.tensornet import TensorNetworkBackend, MBQCTensorNet, gen_str
+from graphix.sim.tensornet import MBQCTensorNet, gen_str
 from graphix.clifford import CLIFFORD
 import tests.random_circuit as rc
 
 
-def random_op(sites, dtype=np.complex64, seed=0):
+def random_op(sites, dtype=np.complex128, seed=0):
     np.random.seed(seed)
     size = 2**sites
     if dtype is np.complex64:
         return np.random.randn(size, size).astype(np.float32) + 1j * np.random.randn(size, size).astype(np.float32)
     if dtype is np.complex128:
         return np.random.randn(size, size).astype(np.float64) + 1j * np.random.randn(size, size).astype(np.float64)
     return np.random.randn(size, size).astype(dtype)
```

### Comparing `graphix-0.2.1/tests/test_transpiler.py` & `graphix-0.2.2/tests/test_transpiler.py`

 * *Files identical despite different names*

