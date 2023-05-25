# Comparing `tmp/qcs_phy-1.0.0.tar.gz` & `tmp/qcs_phy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcs_phy-1.0.0.tar", last modified: Wed May 10 02:29:29 2023, max compression
+gzip compressed data, was "qcs_phy-1.0.1.tar", last modified: Thu May 25 02:27:51 2023, max compression
```

## Comparing `qcs_phy-1.0.0.tar` & `qcs_phy-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 02:29:29.044213 qcs_phy-1.0.0/
--rw-rw-rw-   0        0        0     1011 2023-05-10 02:29:29.044213 qcs_phy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 02:29:29.038230 qcs_phy-1.0.0/qcs_phy/
--rw-rw-rw-   0        0        0    54629 2023-05-09 13:49:52.000000 qcs_phy-1.0.0/qcs_phy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 02:29:29.043218 qcs_phy-1.0.0/qcs_phy.egg-info/
--rw-rw-rw-   0        0        0     1011 2023-05-10 02:29:28.000000 qcs_phy-1.0.0/qcs_phy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-05-10 02:29:28.000000 qcs_phy-1.0.0/qcs_phy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 02:29:28.000000 qcs_phy-1.0.0/qcs_phy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-10 02:29:28.000000 qcs_phy-1.0.0/qcs_phy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 02:29:28.000000 qcs_phy-1.0.0/qcs_phy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 02:29:29.044213 qcs_phy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1696 2023-05-10 02:29:26.000000 qcs_phy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:27:51.566743 qcs_phy-1.0.1/
+-rw-rw-rw-   0        0        0     1011 2023-05-25 02:27:51.566743 qcs_phy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-10 02:21:31.000000 qcs_phy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 02:27:51.561757 qcs_phy-1.0.1/qcs_phy/
+-rw-rw-rw-   0        0        0    54371 2023-05-25 02:13:07.000000 qcs_phy-1.0.1/qcs_phy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:27:51.565746 qcs_phy-1.0.1/qcs_phy.egg-info/
+-rw-rw-rw-   0        0        0     1011 2023-05-25 02:27:51.000000 qcs_phy-1.0.1/qcs_phy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-05-25 02:27:51.000000 qcs_phy-1.0.1/qcs_phy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:27:51.000000 qcs_phy-1.0.1/qcs_phy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-25 02:27:51.000000 qcs_phy-1.0.1/qcs_phy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-25 02:27:51.000000 qcs_phy-1.0.1/qcs_phy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 02:27:51.566743 qcs_phy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-05-25 02:16:53.000000 qcs_phy-1.0.1/setup.py
```

### Comparing `qcs_phy-1.0.0/PKG-INFO` & `qcs_phy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs_phy
-Version: 1.0.0
+Version: 1.0.1
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.0/qcs_phy/__init__.py` & `qcs_phy-1.0.1/qcs_phy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         else:
             H_v_new.append(Hi)
             H_c_new.append(H_c[k])
     return H_c_new, H_v_new
 
 
 class qcs:
-    __Dim = {}
+    __Dim = dict()
     __BasisList = dict()
     __HeffList = dict()
     __InOutList = dict()
     __Judge_Heff = []
     __Judge_InOut = dict()
 
     def __init__(self, Heff: list, Input: list, Output: list, ratio=None):
@@ -516,82 +516,75 @@
         :return: the modes of output channel in the form of matrix
         """
         Out_m = {}
         for key, value in self.__Output.items():
             Out_m[key] = sum_sparse([qcs.__InOutList[n_exc][x[1]] * x[0] for x in value])
         return Out_m
 
-    def print_Dim(self, n_exc: int, p=1):
+    def print_Dim(self, n_exc: int):
         """
         This function is used to print the dimension, which corresponds to excitation number n_exc.
         :param n_exc: the excitation number
-        :param p: print (p=1) or return (p=0), the default is printing
         """
         self.__excitation_number()
+        if self.__Heff_v != qcs.__Judge_Heff:
+            qcs.__Dim.clear()
+            qcs.__Judge_Heff = self.__Heff_v
         if n_exc not in qcs.__Dim.keys():
             self.__basis(n_exc)
-        if p == 1:
-            print(self.__Dim[n_exc])
-        else:
-            return self.__Dim[n_exc]
+        return self.__Dim[n_exc]
 
-    def print_basis(self, n_exc: int, p=1):
+    def print_basis(self, n_exc: int):
         """
         This function is used to print the basis vectors, which corresponds to excitation number (n_exc).
         :param n_exc: the excitation number
-        :param p: print (p=1) or return (p=0), the default is printing
         """
         self.__excitation_number()
+        if self.__Heff_v != qcs.__Judge_Heff:
+            qcs.__BasisList.clear()
+            qcs.__Judge_Heff = self.__Heff_v
         if n_exc not in qcs.__BasisList.keys():
             self.__basis(n_exc)
-        if p == 1:
-            print(qcs.__BasisList[n_exc])
-        else:
-            return qcs.__BasisList[n_exc]
+        return qcs.__BasisList[n_exc]
 
-    def print_InOutput(self, n_exc: int, channel_name: str, p=1):
+    def print_InOutput(self, n_exc: int, channel_name: str):
         """
         This function is used to print the matrix, which corresponds to the projections of the input/output mode
         onto the direct sum of the (n_exc-1)-th abd (n_exc)-th excitation subspace.
         :param n_exc: the excitation number
         :param channel_name: the name of channel
-        :param p: print (p=1) or return (p=0), the default is printing
         """
         self.__excitation_number()
+        if self.__Heff_v != qcs.__Judge_Heff:
+            qcs.__InOutList.clear()
+            qcs.__Judge_Heff = self.__Heff_v
         if n_exc not in qcs.__InOutList.keys():
             self.__basis(n_exc - 1)
             self.__basis(n_exc)
             self.__prestore_InOutList(n_exc)
         if channel_name in self.__Input:
-            if p == 1:
-                print(self.__Input_Matrix(n_exc)[channel_name])
-            else:
-                return self.__Input_Matrix(n_exc)[channel_name]
+            return self.__Input_Matrix(n_exc)[channel_name]
         elif channel_name in self.__Output:
-            if p == 1:
-                print(self.__Output_Matrix(n_exc)[channel_name])
-            else:
-                return self.__Output_Matrix(n_exc)[channel_name]
+            return self.__Output_Matrix(n_exc)[channel_name]
         else:
             print("Sorry, the channel name %s does not exist." % channel_name)
 
-    def print_Heff(self, n_exc: int, p=1):
+    def print_Heff(self, n_exc: int):
         """
-        This function is used to print the correspondint effective Hamiltonian in the excitation subspace (n_exc).
+        This function is used to input the correspondint effective Hamiltonian in the excitation subspace (n_exc).
         :param n_exc: the excitation number
-        :param p: print (p=1), return (p=0), the default is printing
         """
         self.__excitation_number()
+        if self.__Heff_v != qcs.__Judge_Heff:
+            qcs.__HeffList.clear()
+            qcs.__Judge_Heff = self.__Heff_v
         if n_exc not in qcs.__HeffList.keys():
             self.__basis(n_exc)
             self.__prestore_HeffList(n_exc)
-        if p == 1:
-            print(self.__Heff_Matrix(n_exc))
-        else:
-            return self.__Heff_Matrix(n_exc)
+        return self.__Heff_Matrix(n_exc)
 
     def __classification(self, photons: list):
         """
         :param photons: the output modes
         :return: the classification label
         """
         In_list, Out_list = set(self.__Input.keys()), set(photons)
```

### Comparing `qcs_phy-1.0.0/qcs_phy.egg-info/PKG-INFO` & `qcs_phy-1.0.1/qcs_phy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcs-phy
-Version: 1.0.0
+Version: 1.0.1
 Summary: QCS: Quantum Correlation Solver
 Home-page: 
 Author: ZhiGuang Lu
 Author-email: youngqlzg@gamil.com
 License: BSD
 Keywords: quantum physics higher-order equal-time correlation function
 Platform: Linux
```

### Comparing `qcs_phy-1.0.0/setup.py` & `qcs_phy-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # # these things are needed for the README.md show on pypi
 # here = os.path.abspath(os.path.dirname(__file__))
 #
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'QCS: Quantum Correlation Solver'
 LONG_DESCRIPTION = 'QCS is an open-source Python code that allows to study the single-photon transmission and reflection, ' \
                    'as well as the nth-order equal-time correlation functions (ETCFs) in driven-dissipative quantum systems.'
 REQUIRES = ['numpy (>=1.8)', 'scipy (>=0.15)']
 INSTALL_REQUIRES = ['numpy>=1.8', 'scipy>=0.15']
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "quantum physics higher-order equal-time correlation function"
```

