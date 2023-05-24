# Comparing `tmp/routeml-0.4.0.tar.gz` & `tmp/routeml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeml-0.4.0.tar", last modified: Wed May 24 15:47:04 2023, max compression
+gzip compressed data, was "routeml-0.5.0.tar", last modified: Wed May 24 23:18:11 2023, max compression
```

## Comparing `routeml-0.4.0.tar` & `routeml-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.529817 routeml-0.4.0/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-24 15:47:04.529564 routeml-0.4.0/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.4.0/README.md
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.522069 routeml-0.4.0/routeml/
--rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.4.0/routeml/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.4.0/routeml/cvrp.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.4.0/routeml/draw.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.4.0/routeml/solvers.py
--rw-r--r--   0 samuelchin   (502) staff       (20)    10819 2023-05-24 15:45:05.000000 routeml-0.4.0/routeml/utils.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.523315 routeml-0.4.0/routeml.egg-info/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-24 15:47:04.000000 routeml-0.4.0/routeml.egg-info/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)      810 2023-05-24 15:47:04.000000 routeml-0.4.0/routeml.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-24 15:47:04.000000 routeml-0.4.0/routeml.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-24 15:47:04.000000 routeml-0.4.0/routeml.egg-info/requires.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-24 15:47:04.000000 routeml-0.4.0/routeml.egg-info/top_level.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-24 15:47:04.529889 routeml-0.4.0/setup.cfg
--rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-24 15:46:49.000000 routeml-0.4.0/setup.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.523803 routeml-0.4.0/tests/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.4.0/tests/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.524728 routeml-0.4.0/tests/integration/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.4.0/tests/integration/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.4.0/tests/integration/test_draw_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.4.0/tests/integration/test_vrplib_cost_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.4.0/tests/test_cvrp.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.525236 routeml-0.4.0/tests/unit/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 15:47:04.529134 routeml-0.4.0/tests/unit/utils/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.4.0/tests/unit/utils/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.4.0/tests/unit/utils/test_get_cvrp_cost.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.4.0/tests/unit/utils/test_get_is_feasible.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1594 2023-05-19 19:51:57.000000 routeml-0.4.0/tests/unit/utils/test_get_route_demand.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.4.0/tests/unit/utils/test_pad_matrices.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.4.0/tests/unit/utils/test_parse_vrplib_file.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.4.0/tests/unit/utils/test_parse_vrplib_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.4.0/tests/unit/utils/test_routes_to_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1089 2023-05-18 20:17:28.000000 routeml-0.4.0/tests/unit/utils/test_solution_to_routes.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.121893 routeml-0.5.0/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-24 23:18:11.121664 routeml-0.5.0/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.5.0/README.md
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.115571 routeml-0.5.0/routeml/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.5.0/routeml/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.5.0/routeml/cvrp.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.5.0/routeml/draw.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.5.0/routeml/solvers.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)    12519 2023-05-24 23:17:27.000000 routeml-0.5.0/routeml/utils.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.116724 routeml-0.5.0/routeml.egg-info/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-24 23:18:11.000000 routeml-0.5.0/routeml.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)      855 2023-05-24 23:18:11.000000 routeml-0.5.0/routeml.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-24 23:18:11.000000 routeml-0.5.0/routeml.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-24 23:18:11.000000 routeml-0.5.0/routeml.egg-info/requires.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-24 23:18:11.000000 routeml-0.5.0/routeml.egg-info/top_level.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-24 23:18:11.121951 routeml-0.5.0/setup.cfg
+-rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-24 23:17:57.000000 routeml-0.5.0/setup.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.117016 routeml-0.5.0/tests/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.5.0/tests/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.117805 routeml-0.5.0/tests/integration/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.5.0/tests/integration/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.5.0/tests/integration/test_draw_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.5.0/tests/integration/test_vrplib_cost_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.5.0/tests/test_cvrp.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.118296 routeml-0.5.0/tests/unit/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-24 23:18:11.121280 routeml-0.5.0/tests/unit/utils/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.5.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.5.0/tests/unit/utils/test_get_cvrp_cost.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.5.0/tests/unit/utils/test_get_is_feasible.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1594 2023-05-19 19:51:57.000000 routeml-0.5.0/tests/unit/utils/test_get_route_demand.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.5.0/tests/unit/utils/test_pad_matrices.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.5.0/tests/unit/utils/test_parse_vrplib_file.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.5.0/tests/unit/utils/test_parse_vrplib_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.5.0/tests/unit/utils/test_routes_to_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1779 2023-05-24 23:16:01.000000 routeml-0.5.0/tests/unit/utils/test_solution_to_adj_mat.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1089 2023-05-18 20:17:28.000000 routeml-0.5.0/tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.4.0/PKG-INFO` & `routeml-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.4.0/routeml/draw.py` & `routeml-0.5.0/routeml/draw.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/routeml/solvers.py` & `routeml-0.5.0/routeml/solvers.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/routeml/utils.py` & `routeml-0.5.0/routeml/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,14 +66,46 @@
             route.append(0)
             routes.append(route)
             route = []
         route.append(node)
     return routes
 
 
+def solution_to_adjacency_matrix(cvrp_solution):
+    """
+    Converts a CVRP solution into a symmetric adjacency matrix.
+
+    Args:
+        cvrp_solution (list): CVRP solution (list of nodes).
+
+    Returns:
+        np.ndarray: Symmetric adjacency matrix.
+    """
+    num_nodes = max(cvrp_solution) + 1
+    matrix = np.zeros((num_nodes, num_nodes))
+
+    for i in range(len(cvrp_solution) - 1):
+        matrix[cvrp_solution[i]][cvrp_solution[i + 1]] = 1
+        matrix[cvrp_solution[i + 1]][cvrp_solution[i]] = 1
+    return matrix
+
+def column_normalize_adjacency_matrix(adj_matrix):
+    """
+    Normalize an adjacency matrix by column.
+
+    Args:
+        adj_matrix (np.ndarray): Binary adjacency matrix.
+
+    Returns:
+        np.ndarray: Normalized adjacency matrix.
+    """
+    col_sums = np.sum(adj_matrix, axis=0)
+    normalized_matrix = adj_matrix / col_sums[np.newaxis, :]
+    return normalized_matrix
+
 def parse_vrplib_file(source):
     """
     Parses a VRPLIB file and returns a dictionary with the following keys:
     - name: Name of the problem.
     - comment: Comment of the problem.
     - type: Type of the problem.
     - dimension: Number of nodes.
@@ -346,10 +378,36 @@
            [6, 7, 8, 0, 0, 0],
            [0, 0, 0, 0, 0, 0]])
     ```
     """
     submatrix = matrix[:, indices]
     return pad_matrix(submatrix, new_shape)
 
+def get_random_solution(N):
+    """
+    Generates a random CVRP solution. Mostly for debugging purposes.
+
+    Args:
+        N (int): Number of nodes in the problem. Excluding depot.
+    
+    Returns:
+        lst (list): List containing the solution.
+    """
+    # Generate a random list from 0 to N
+    lst = list(range(N + 1))
+
+    # Insert 0 at the end
+    lst.append(0)
+
+    # Randomly insert 1 to 5 zeros in between
+    num_zeros = random.randint(1, 5)
+    for _ in range(num_zeros):
+        index = random.randint(1, len(lst) - 1)  # Select a random index between 1 and len(lst)-1
+        while lst[index] == 0 or lst[index-1] == 0:
+            index = random.randint(1, len(lst) - 1)  # Select a new index if adjacent elements are already 0
+        lst.insert(index, 0)
+
+    return lst
+
```

### Comparing `routeml-0.4.0/routeml.egg-info/PKG-INFO` & `routeml-0.5.0/routeml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.4.0/routeml.egg-info/SOURCES.txt` & `routeml-0.5.0/routeml.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 tests/unit/utils/test_get_cvrp_cost.py
 tests/unit/utils/test_get_is_feasible.py
 tests/unit/utils/test_get_route_demand.py
 tests/unit/utils/test_pad_matrices.py
 tests/unit/utils/test_parse_vrplib_file.py
 tests/unit/utils/test_parse_vrplib_solution.py
 tests/unit/utils/test_routes_to_solution.py
+tests/unit/utils/test_solution_to_adj_mat.py
 tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.4.0/setup.py` & `routeml-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='routeml',
-    version='0.4.0',
+    version='0.5.0',
     description='Python package for CVRP utilities',
     author='Your Name',
     author_email='jkschin@mit.edu',
     url='https://github.com/jkschin/routeml',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `routeml-0.4.0/tests/integration/test_draw_integration.py` & `routeml-0.5.0/tests/integration/test_draw_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/integration/test_vrplib_cost_integration.py` & `routeml-0.5.0/tests/integration/test_vrplib_cost_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_get_cvrp_cost.py` & `routeml-0.5.0/tests/unit/utils/test_get_cvrp_cost.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_get_is_feasible.py` & `routeml-0.5.0/tests/unit/utils/test_get_is_feasible.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_get_route_demand.py` & `routeml-0.5.0/tests/unit/utils/test_get_route_demand.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_pad_matrices.py` & `routeml-0.5.0/tests/unit/utils/test_pad_matrices.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_parse_vrplib_file.py` & `routeml-0.5.0/tests/unit/utils/test_parse_vrplib_file.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_parse_vrplib_solution.py` & `routeml-0.5.0/tests/unit/utils/test_parse_vrplib_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_routes_to_solution.py` & `routeml-0.5.0/tests/unit/utils/test_routes_to_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.4.0/tests/unit/utils/test_solution_to_routes.py` & `routeml-0.5.0/tests/unit/utils/test_solution_to_routes.py`

 * *Files identical despite different names*

