# Comparing `tmp/routeml-0.8.0.tar.gz` & `tmp/routeml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeml-0.8.0.tar", last modified: Thu May 25 18:51:48 2023, max compression
+gzip compressed data, was "routeml-0.9.0.tar", last modified: Thu May 25 19:00:48 2023, max compression
```

## Comparing `routeml-0.8.0.tar` & `routeml-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.443861 routeml-0.8.0/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 18:51:48.443634 routeml-0.8.0/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.8.0/README.md
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.435690 routeml-0.8.0/routeml/
--rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.8.0/routeml/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.8.0/routeml/cvrp.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.8.0/routeml/draw.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.8.0/routeml/solvers.py
--rw-r--r--   0 samuelchin   (502) staff       (20)    14452 2023-05-25 18:51:28.000000 routeml-0.8.0/routeml/utils.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.436457 routeml-0.8.0/routeml.egg-info/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 18:51:48.000000 routeml-0.8.0/routeml.egg-info/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)      895 2023-05-25 18:51:48.000000 routeml-0.8.0/routeml.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-25 18:51:48.000000 routeml-0.8.0/routeml.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-25 18:51:48.000000 routeml-0.8.0/routeml.egg-info/requires.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-25 18:51:48.000000 routeml-0.8.0/routeml.egg-info/top_level.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-25 18:51:48.443910 routeml-0.8.0/setup.cfg
--rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-25 18:51:37.000000 routeml-0.8.0/setup.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.436761 routeml-0.8.0/tests/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.8.0/tests/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.437490 routeml-0.8.0/tests/integration/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.8.0/tests/integration/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.8.0/tests/integration/test_draw_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.8.0/tests/integration/test_vrplib_cost_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.8.0/tests/test_cvrp.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.438215 routeml-0.8.0/tests/unit/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.8.0/tests/unit/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:51:48.443283 routeml-0.8.0/tests/unit/utils/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.8.0/tests/unit/utils/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.8.0/tests/unit/utils/test_get_cvrp_cost.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.8.0/tests/unit/utils/test_get_is_feasible.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      760 2023-05-25 18:29:35.000000 routeml-0.8.0/tests/unit/utils/test_get_logit_mask.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     2505 2023-05-25 17:42:17.000000 routeml-0.8.0/tests/unit/utils/test_get_route_demand.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.8.0/tests/unit/utils/test_pad_matrices.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.8.0/tests/unit/utils/test_parse_vrplib_file.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.8.0/tests/unit/utils/test_parse_vrplib_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.8.0/tests/unit/utils/test_routes_to_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1779 2023-05-24 23:16:01.000000 routeml-0.8.0/tests/unit/utils/test_solution_to_adj_mat.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1617 2023-05-25 18:26:43.000000 routeml-0.8.0/tests/unit/utils/test_solution_to_routes.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.667647 routeml-0.9.0/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 19:00:48.667431 routeml-0.9.0/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.9.0/README.md
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.662085 routeml-0.9.0/routeml/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.9.0/routeml/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.9.0/routeml/cvrp.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.9.0/routeml/draw.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.9.0/routeml/solvers.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)    14460 2023-05-25 18:58:37.000000 routeml-0.9.0/routeml/utils.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.662857 routeml-0.9.0/routeml.egg-info/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 19:00:48.000000 routeml-0.9.0/routeml.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)      895 2023-05-25 19:00:48.000000 routeml-0.9.0/routeml.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-25 19:00:48.000000 routeml-0.9.0/routeml.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-25 19:00:48.000000 routeml-0.9.0/routeml.egg-info/requires.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-25 19:00:48.000000 routeml-0.9.0/routeml.egg-info/top_level.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-25 19:00:48.667701 routeml-0.9.0/setup.cfg
+-rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-25 19:00:24.000000 routeml-0.9.0/setup.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.663157 routeml-0.9.0/tests/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.9.0/tests/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.663734 routeml-0.9.0/tests/integration/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.9.0/tests/integration/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.9.0/tests/integration/test_draw_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.9.0/tests/integration/test_vrplib_cost_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.9.0/tests/test_cvrp.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.664080 routeml-0.9.0/tests/unit/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.9.0/tests/unit/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 19:00:48.667071 routeml-0.9.0/tests/unit/utils/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.9.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.9.0/tests/unit/utils/test_get_cvrp_cost.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.9.0/tests/unit/utils/test_get_is_feasible.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1299 2023-05-25 18:59:59.000000 routeml-0.9.0/tests/unit/utils/test_get_logit_mask.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     2505 2023-05-25 17:42:17.000000 routeml-0.9.0/tests/unit/utils/test_get_route_demand.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.9.0/tests/unit/utils/test_pad_matrices.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.9.0/tests/unit/utils/test_parse_vrplib_file.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.9.0/tests/unit/utils/test_parse_vrplib_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.9.0/tests/unit/utils/test_routes_to_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1779 2023-05-24 23:16:01.000000 routeml-0.9.0/tests/unit/utils/test_solution_to_adj_mat.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1617 2023-05-25 18:26:43.000000 routeml-0.9.0/tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.8.0/PKG-INFO` & `routeml-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.8.0/routeml/draw.py` & `routeml-0.9.0/routeml/draw.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/routeml/solvers.py` & `routeml-0.9.0/routeml/solvers.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/routeml/utils.py` & `routeml-0.9.0/routeml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,16 +432,16 @@
         demands (np.ndarray): the demands of each node.
         capacity (int): the capacity of the vehicle.
     
     Returns:
         mask (np.ndarray): the logit mask.
     """
     prob = set(sol)
-    mask = np.full((len(sol), len(prob)), 0.0) # mark all as valid
-    for i in range(len(sol)): # NOTE this loop is 100% correct, don't change this.
+    mask = np.full((len(sol) - 1, len(prob)), 0.0) # mark all as valid
+    for i in range(len(sol) - 1): # NOTE this loop is 100% correct, don't change this.
         # a is all nodes that I visited
         a = set(sol[:i+1])
         if sol[i] != 0:
             a.remove(0)
         # mark all visited nodes as invalid
         mask[i, list(a)] = float("-inf")
```

### Comparing `routeml-0.8.0/routeml.egg-info/PKG-INFO` & `routeml-0.9.0/routeml.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.8.0/routeml.egg-info/SOURCES.txt` & `routeml-0.9.0/routeml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/setup.py` & `routeml-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='routeml',
-    version='0.8.0',
+    version='0.9.0',
     description='Python package for CVRP utilities',
     author='Your Name',
     author_email='jkschin@mit.edu',
     url='https://github.com/jkschin/routeml',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `routeml-0.8.0/tests/integration/test_draw_integration.py` & `routeml-0.9.0/tests/integration/test_draw_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/integration/test_vrplib_cost_integration.py` & `routeml-0.9.0/tests/integration/test_vrplib_cost_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_get_cvrp_cost.py` & `routeml-0.9.0/tests/unit/utils/test_get_cvrp_cost.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_get_is_feasible.py` & `routeml-0.9.0/tests/unit/utils/test_get_is_feasible.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_get_logit_mask.py` & `routeml-0.9.0/tests/unit/utils/test_get_logit_mask.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,30 @@
         sol = [0, 1, 2, 0, 3, 4]
         demands = np.array([0, 5, 8, 3, 6])
         capacity = 15
         expected_mask = np.array([[-np.inf, 0., 0., 0., 0.],
                 [0., -np.inf, 0., 0., 0.],
                 [0., -np.inf, -np.inf, -np.inf, -np.inf],
                 [-np.inf, -np.inf, -np.inf, 0., 0.],
+                [0., -np.inf, -np.inf, -np.inf, 0.]])
+
+        result_mask = get_logit_mask(sol, demands, capacity)
+
+        np.testing.assert_array_equal(result_mask, expected_mask)
+
+    def test_get_logit_mask_2(self):
+        sol = [0, 1, 2, 0, 3, 4, 0]
+        demands = np.array([0, 5, 8, 3, 6])
+        capacity = 15
+        expected_mask = np.array([[-np.inf, 0., 0., 0., 0.],
+                [0., -np.inf, 0., 0., 0.],
+                [0., -np.inf, -np.inf, -np.inf, -np.inf],
+                [-np.inf, -np.inf, -np.inf, 0., 0.],
                 [0., -np.inf, -np.inf, -np.inf, 0.],
-                [0., -np.inf, -np.inf, -np.inf, -np.inf]])
+                [0., -np.inf, -np.inf, -np.inf, -np.inf],])
 
         result_mask = get_logit_mask(sol, demands, capacity)
 
         np.testing.assert_array_equal(result_mask, expected_mask)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `routeml-0.8.0/tests/unit/utils/test_get_route_demand.py` & `routeml-0.9.0/tests/unit/utils/test_get_route_demand.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_pad_matrices.py` & `routeml-0.9.0/tests/unit/utils/test_pad_matrices.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_parse_vrplib_file.py` & `routeml-0.9.0/tests/unit/utils/test_parse_vrplib_file.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_parse_vrplib_solution.py` & `routeml-0.9.0/tests/unit/utils/test_parse_vrplib_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_routes_to_solution.py` & `routeml-0.9.0/tests/unit/utils/test_routes_to_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_solution_to_adj_mat.py` & `routeml-0.9.0/tests/unit/utils/test_solution_to_adj_mat.py`

 * *Files identical despite different names*

### Comparing `routeml-0.8.0/tests/unit/utils/test_solution_to_routes.py` & `routeml-0.9.0/tests/unit/utils/test_solution_to_routes.py`

 * *Files identical despite different names*

