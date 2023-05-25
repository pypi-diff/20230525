# Comparing `tmp/ccs_fit-0.21.4.tar.gz` & `tmp/ccs_fit-0.21.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs_fit-0.21.4.tar", max compression
+gzip compressed data, was "ccs_fit-0.21.5.tar", max compression
```

## Comparing `ccs_fit-0.21.4.tar` & `ccs_fit-0.21.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2023-05-23 12:04:07.897219 ccs_fit-0.21.4/LICENSE
--rw-r--r--   0        0        0     7895 2023-05-23 12:04:07.897219 ccs_fit-0.21.4/README.md
--rw-r--r--   0        0        0     2483 2023-05-23 12:04:49.353948 ccs_fit-0.21.4/pyproject.toml
--rw-r--r--   0        0        0     1027 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/__init__.py
--rw-r--r--   0        0        0     9636 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/ase_calculator/buck.py
--rw-r--r--   0        0        0     7934 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
--rw-r--r--   0        0        0    10653 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
--rw-r--r--   0        0        0      488 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/__init__.py
--rw-r--r--   0        0        0      628 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/exceptions.py
--rw-r--r--   0        0        0     1476 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/io.py
--rw-r--r--   0        0        0      486 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/math/__init__.py
--rw-r--r--   0        0        0     1071 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/math/ewald.py
--rw-r--r--   0        0        0     2156 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/common/neighborlist.py
--rw-r--r--   0        0        0      488 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/data/__init__.py
--rw-r--r--   0        0        0      854 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/data/conversion.py
--rw-r--r--   0        0        0      805 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/debugging_tools/timing.py
--rw-r--r--   0        0        0      488 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/fitting/__init__.py
--rw-r--r--   0        0        0    13479 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/fitting/main copy.py
--rw-r--r--   0        0        0    14597 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/fitting/main.py
--rw-r--r--   0        0        0    23883 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/fitting/objective.py
--rw-r--r--   0        0        0    11717 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/fitting/spline_functions.py
--rw-r--r--   0        0        0    20046 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/ppmd_interface/ccs_ppmd.py
--rw-r--r--   0        0        0     6913 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/regression_tool/regression.py
--rw-r--r--   0        0        0      488 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/__init__.py
--rw-r--r--   0        0        0     7361 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_build_db copy.py
--rw-r--r--   0        0        0     7229 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_build_db.py
--rw-r--r--   0        0        0     8555 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_export_FF.py
--rw-r--r--   0        0        0     4155 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_export_sktable.py
--rw-r--r--   0        0        0     8716 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_fetch.py
--rw-r--r--   0        0        0     2537 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_fit.py
--rw-r--r--   0        0        0     6482 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_prune.py
--rw-r--r--   0        0        0     6754 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_validate.py
--rw-r--r--   0        0        0     1784 2023-05-23 12:04:08.865236 ccs_fit-0.21.4/src/ccs_fit/scripts/jsonTotable.py
--rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-25 12:27:17.970860 ccs_fit-0.21.5/LICENSE
+-rw-r--r--   0        0        0     7895 2023-05-25 12:27:17.970860 ccs_fit-0.21.5/README.md
+-rw-r--r--   0        0        0     2483 2023-05-25 12:28:14.941985 ccs_fit-0.21.5/pyproject.toml
+-rw-r--r--   0        0        0     1027 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/__init__.py
+-rw-r--r--   0        0        0     9636 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/ase_calculator/buck.py
+-rw-r--r--   0        0        0     8028 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/ase_calculator/ccs_ase_G2B.py
+-rw-r--r--   0        0        0    10653 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/ase_calculator/ccs_ase_calculator.py
+-rw-r--r--   0        0        0      488 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/__init__.py
+-rw-r--r--   0        0        0      628 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/exceptions.py
+-rw-r--r--   0        0        0     1476 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/io.py
+-rw-r--r--   0        0        0      486 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/math/__init__.py
+-rw-r--r--   0        0        0     1071 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/math/ewald.py
+-rw-r--r--   0        0        0     2156 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/common/neighborlist.py
+-rw-r--r--   0        0        0      488 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/data/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/data/conversion.py
+-rw-r--r--   0        0        0      805 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/debugging_tools/timing.py
+-rw-r--r--   0        0        0      488 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/fitting/__init__.py
+-rw-r--r--   0        0        0    13479 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/fitting/main copy.py
+-rw-r--r--   0        0        0    14597 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/fitting/main.py
+-rw-r--r--   0        0        0    23883 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/fitting/objective.py
+-rw-r--r--   0        0        0    11717 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/fitting/spline_functions.py
+-rw-r--r--   0        0        0    20046 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/ppmd_interface/ccs_ppmd.py
+-rw-r--r--   0        0        0     6913 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/regression_tool/regression.py
+-rw-r--r--   0        0        0      488 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/scripts/__init__.py
+-rw-r--r--   0        0        0     7361 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_build_db copy.py
+-rw-r--r--   0        0        0     7229 2023-05-25 12:27:19.042842 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_build_db.py
+-rw-r--r--   0        0        0     8555 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_export_FF.py
+-rw-r--r--   0        0        0     4155 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_export_sktable.py
+-rw-r--r--   0        0        0     8716 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_fetch.py
+-rw-r--r--   0        0        0     2537 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_fit.py
+-rw-r--r--   0        0        0     6482 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_prune.py
+-rw-r--r--   0        0        0     6754 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_validate.py
+-rw-r--r--   0        0        0     1784 2023-05-25 12:27:19.046841 ccs_fit-0.21.5/src/ccs_fit/scripts/jsonTotable.py
+-rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 ccs_fit-0.21.5/PKG-INFO
```

### Comparing `ccs_fit-0.21.4/LICENSE` & `ccs_fit-0.21.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/README.md` & `ccs_fit-0.21.5/README.md`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/pyproject.toml` & `ccs_fit-0.21.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ccs_fit"
-version = "0.21.4"
+version = "0.21.5"
 description = "Fitting tools for repulsive two body interactions using curvature constrained splines."
 authors = [
     "Akshay Krishna AK",
     "Jolla Kullgren <jolla.kullgren@kemi.uu.se>",
     "Eddie Wadbro <eddie.wadbro@umu.se>"
     ]
 maintainers = [
```

### Comparing `ccs_fit-0.21.4/src/ccs_fit/__init__.py` & `ccs_fit-0.21.5/src/ccs_fit/__init__.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/ase_calculator/buck.py` & `ccs_fit-0.21.5/src/ccs_fit/ase_calculator/buck.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/ase_calculator/ccs_ase_G2B.py` & `ccs_fit-0.21.5/src/ccs_fit/ase_calculator/ccs_ase_G2B.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,16 @@
 
     def calculate(self, atoms=None, properties=["energy"], system_changes=all_changes):
         Calculator.calculate(self, atoms, properties, system_changes)
         self.species = list(set(self.atoms.get_chemical_symbols()))
         self.pair = dict()
         for a, b in it.product(self.species, self.species):
             self.pair[a + b] = G2B_pair(a, b, self.G2B_params)
+            if self.pair[a + b].rcut > self.rc:
+                self.rc=self.pair[a + b].rcut
 
         if self.atoms.number_of_lattice_vectors == 3:
             cell = atoms.get_cell()
             self.atoms.wrap()
             n_repeat = self.rc * np.linalg.norm(np.linalg.inv(cell), axis=0)
             n_repeat = np.ceil(n_repeat).astype(int)
             offsets = [*it.product(*[np.arange(-n, n + 1) for n in n_repeat])]
```

### Comparing `ccs_fit-0.21.4/src/ccs_fit/ase_calculator/ccs_ase_calculator.py` & `ccs_fit-0.21.5/src/ccs_fit/ase_calculator/ccs_ase_calculator.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/common/exceptions.py` & `ccs_fit-0.21.5/src/ccs_fit/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/common/io.py` & `ccs_fit-0.21.5/src/ccs_fit/common/io.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/common/math/ewald.py` & `ccs_fit-0.21.5/src/ccs_fit/common/math/ewald.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/common/neighborlist.py` & `ccs_fit-0.21.5/src/ccs_fit/common/neighborlist.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/data/conversion.py` & `ccs_fit-0.21.5/src/ccs_fit/data/conversion.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/debugging_tools/timing.py` & `ccs_fit-0.21.5/src/ccs_fit/debugging_tools/timing.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/fitting/main copy.py` & `ccs_fit-0.21.5/src/ccs_fit/fitting/main copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/fitting/main.py` & `ccs_fit-0.21.5/src/ccs_fit/fitting/main.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/fitting/objective.py` & `ccs_fit-0.21.5/src/ccs_fit/fitting/objective.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/fitting/spline_functions.py` & `ccs_fit-0.21.5/src/ccs_fit/fitting/spline_functions.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/ppmd_interface/ccs_ppmd.py` & `ccs_fit-0.21.5/src/ccs_fit/ppmd_interface/ccs_ppmd.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/regression_tool/regression.py` & `ccs_fit-0.21.5/src/ccs_fit/regression_tool/regression.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_build_db copy.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_build_db copy.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_build_db.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_build_db.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_export_FF.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_export_FF.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_export_sktable.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_export_sktable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_fetch.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_fetch.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_fit.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_fit.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_prune.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_prune.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/ccs_validate.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/ccs_validate.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/src/ccs_fit/scripts/jsonTotable.py` & `ccs_fit-0.21.5/src/ccs_fit/scripts/jsonTotable.py`

 * *Files identical despite different names*

### Comparing `ccs_fit-0.21.4/PKG-INFO` & `ccs_fit-0.21.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccs-fit
-Version: 0.21.4
+Version: 0.21.5
 Summary: Fitting tools for repulsive two body interactions using curvature constrained splines.
 Home-page: https://github.com/Teoroo-CMC/CCS
 License: GPL-3
 Keywords: Curvature,Constrained,Splines,Two-Body,Interatomic,Repulsive,Fitting
 Author: Akshay Krishna AK
 Maintainer: Jolla Kullgren
 Maintainer-email: jolla.kullgren@kemi.uu.se
```

