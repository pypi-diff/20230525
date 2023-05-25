# Comparing `tmp/routeml-0.6.0.tar.gz` & `tmp/routeml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeml-0.6.0.tar", last modified: Thu May 25 15:36:24 2023, max compression
+gzip compressed data, was "routeml-0.7.0.tar", last modified: Thu May 25 18:31:50 2023, max compression
```

## Comparing `routeml-0.6.0.tar` & `routeml-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.540809 routeml-0.6.0/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 15:36:24.540530 routeml-0.6.0/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.6.0/README.md
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.534751 routeml-0.6.0/routeml/
--rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.6.0/routeml/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.6.0/routeml/cvrp.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.6.0/routeml/draw.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.6.0/routeml/solvers.py
--rw-r--r--   0 samuelchin   (502) staff       (20)    12569 2023-05-25 15:35:17.000000 routeml-0.6.0/routeml/utils.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.535699 routeml-0.6.0/routeml.egg-info/
--rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 15:36:24.000000 routeml-0.6.0/routeml.egg-info/PKG-INFO
--rw-r--r--   0 samuelchin   (502) staff       (20)      855 2023-05-25 15:36:24.000000 routeml-0.6.0/routeml.egg-info/SOURCES.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-25 15:36:24.000000 routeml-0.6.0/routeml.egg-info/dependency_links.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-25 15:36:24.000000 routeml-0.6.0/routeml.egg-info/requires.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-25 15:36:24.000000 routeml-0.6.0/routeml.egg-info/top_level.txt
--rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-25 15:36:24.540865 routeml-0.6.0/setup.cfg
--rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-25 15:36:08.000000 routeml-0.6.0/setup.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.536120 routeml-0.6.0/tests/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.6.0/tests/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.536920 routeml-0.6.0/tests/integration/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.6.0/tests/integration/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.6.0/tests/integration/test_draw_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.6.0/tests/integration/test_vrplib_cost_integration.py
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.6.0/tests/test_cvrp.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.537247 routeml-0.6.0/tests/unit/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.6.0/tests/unit/__init__.py
-drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 15:36:24.540074 routeml-0.6.0/tests/unit/utils/
--rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.6.0/tests/unit/utils/__init__.py
--rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.6.0/tests/unit/utils/test_get_cvrp_cost.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.6.0/tests/unit/utils/test_get_is_feasible.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1594 2023-05-19 19:51:57.000000 routeml-0.6.0/tests/unit/utils/test_get_route_demand.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.6.0/tests/unit/utils/test_pad_matrices.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.6.0/tests/unit/utils/test_parse_vrplib_file.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.6.0/tests/unit/utils/test_parse_vrplib_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.6.0/tests/unit/utils/test_routes_to_solution.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1779 2023-05-24 23:16:01.000000 routeml-0.6.0/tests/unit/utils/test_solution_to_adj_mat.py
--rw-r--r--   0 samuelchin   (502) staff       (20)     1089 2023-05-18 20:17:28.000000 routeml-0.6.0/tests/unit/utils/test_solution_to_routes.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.210265 routeml-0.7.0/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 18:31:50.210054 routeml-0.7.0/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.7.0/README.md
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.204069 routeml-0.7.0/routeml/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      106 2023-05-24 14:21:35.000000 routeml-0.7.0/routeml/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.7.0/routeml/cvrp.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1065 2023-05-24 14:17:18.000000 routeml-0.7.0/routeml/draw.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1109 2023-05-19 23:36:17.000000 routeml-0.7.0/routeml/solvers.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)    14516 2023-05-25 18:31:15.000000 routeml-0.7.0/routeml/utils.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.205018 routeml-0.7.0/routeml.egg-info/
+-rw-r--r--   0 samuelchin   (502) staff       (20)      525 2023-05-25 18:31:50.000000 routeml-0.7.0/routeml.egg-info/PKG-INFO
+-rw-r--r--   0 samuelchin   (502) staff       (20)      895 2023-05-25 18:31:50.000000 routeml-0.7.0/routeml.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)        1 2023-05-25 18:31:50.000000 routeml-0.7.0/routeml.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       30 2023-05-25 18:31:50.000000 routeml-0.7.0/routeml.egg-info/requires.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       14 2023-05-25 18:31:50.000000 routeml-0.7.0/routeml.egg-info/top_level.txt
+-rw-r--r--   0 samuelchin   (502) staff       (20)       38 2023-05-25 18:31:50.210313 routeml-0.7.0/setup.cfg
+-rw-r--r--   0 samuelchin   (502) staff       (20)      798 2023-05-25 18:31:34.000000 routeml-0.7.0/setup.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.205302 routeml-0.7.0/tests/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.7.0/tests/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.206030 routeml-0.7.0/tests/integration/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:17.000000 routeml-0.7.0/tests/integration/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      882 2023-05-22 14:35:44.000000 routeml-0.7.0/tests/integration/test_draw_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1559 2023-05-19 16:01:42.000000 routeml-0.7.0/tests/integration/test_vrplib_cost_integration.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 19:44:51.000000 routeml-0.7.0/tests/test_cvrp.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.206556 routeml-0.7.0/tests/unit/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-19 15:17:06.000000 routeml-0.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 samuelchin   (502) staff       (20)        0 2023-05-25 18:31:50.209792 routeml-0.7.0/tests/unit/utils/
+-rw-r--r--   0 samuelchin   (502) staff       (20)        0 2023-05-18 20:08:10.000000 routeml-0.7.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      995 2023-05-19 15:15:01.000000 routeml-0.7.0/tests/unit/utils/test_get_cvrp_cost.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1431 2023-05-19 20:48:08.000000 routeml-0.7.0/tests/unit/utils/test_get_is_feasible.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)      760 2023-05-25 18:29:35.000000 routeml-0.7.0/tests/unit/utils/test_get_logit_mask.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     2505 2023-05-25 17:42:17.000000 routeml-0.7.0/tests/unit/utils/test_get_route_demand.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1765 2023-05-24 15:24:32.000000 routeml-0.7.0/tests/unit/utils/test_pad_matrices.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1580 2023-05-19 22:37:04.000000 routeml-0.7.0/tests/unit/utils/test_parse_vrplib_file.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1088 2023-05-19 14:54:10.000000 routeml-0.7.0/tests/unit/utils/test_parse_vrplib_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1133 2023-05-18 20:16:06.000000 routeml-0.7.0/tests/unit/utils/test_routes_to_solution.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1779 2023-05-24 23:16:01.000000 routeml-0.7.0/tests/unit/utils/test_solution_to_adj_mat.py
+-rw-r--r--   0 samuelchin   (502) staff       (20)     1617 2023-05-25 18:26:43.000000 routeml-0.7.0/tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.6.0/PKG-INFO` & `routeml-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.6.0/routeml/draw.py` & `routeml-0.7.0/routeml/draw.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/routeml/solvers.py` & `routeml-0.7.0/routeml/solvers.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/routeml/utils.py` & `routeml-0.7.0/routeml/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             raise ValueError("Routes must be a nested list")
 
         route.insert(0, 0)
         route.append(0)
 
     return routes
 
-def solution_to_routes(solution):
+def solution_to_routes(solution, partial=False):
     """
     Converts a solution (list of nodes) into a list of routes.
 
     Args:
         solution (list): Solution (list of nodes).
 
     Returns:
@@ -63,17 +63,18 @@
     route = []
     for node in solution:
         if node == 0 and route:
             route.append(0)
             routes.append(route)
             route = []
         route.append(node)
+    if partial:
+        routes.append(route)
     return routes
 
-
 def solution_to_adjacency_matrix(cvrp_solution):
     """
     Converts a CVRP solution into a symmetric adjacency matrix.
 
     Args:
         cvrp_solution (list): CVRP solution (list of nodes).
 
@@ -248,15 +249,15 @@
         distance = math.dist(coord1, coord2)
         if uchoa:
             distance = round(distance)
         total_cost += distance
 
     return total_cost
 
-def get_route_demand(routes, demand):
+def get_all_route_demands(routes, demand):
     """
     Compute the demand of each route.
 
     Args:
         routes (list): List of routes.
 
     Returns:
@@ -269,14 +270,28 @@
             try:
                 route_demand += demand[node]
             except KeyError:
                 raise Exception(f"Node {node} not found in the demand dictionary")
         route_demands.append(route_demand)
     return route_demands
 
+def get_route_demand(route, demands):
+    """
+    Compute the demand of a route.
+
+    Args:
+        route (list): List of nodes in the route.
+        demands (list): List containing the corresponding demands for each node.
+
+    Returns:
+        int: Demand of the route.
+    """
+    route_demand = sum(map(lambda node: demands[node], route))
+    return route_demand
+
 def is_feasible(routes, demand, capacity):
     """
     Check if a CVRP solution is feasible.
 
     Args:
         routes (list): List of routes.
         demand (dict): Dictionary containing node IDs as keys and corresponding demand as values.
@@ -403,11 +418,47 @@
     for _ in range(num_zeros):
         index = random.randint(1, len(lst) - 1)  # Select a random index between 1 and len(lst)-1
         while lst[index] == 0 or lst[index-1] == 0:
             index = random.randint(1, len(lst) - 1)  # Select a new index if adjacent elements are already 0
         lst.insert(index, 0)
 
     return lst
+    
+def get_logit_mask(sol, demands, capacity):
+    """
+    Gets a logit mask for a given solution. Note that this only takes a full solution.
 
-
-
+    Args:
+        sol (list): the solution to mask.
+        demands (np.ndarray): the demands of each node.
+        capacity (int): the capacity of the vehicle.
+    
+    Returns:
+        mask (np.ndarray): the logit mask.
+    """
+    prob = set(sol)
+    mask = np.full((len(sol), len(prob)), 0.0) # mark all as valid
+    for i in range(len(sol)): # NOTE this loop is 100% correct, don't change this.
+        # a is all nodes that I visited
+        a = set(sol[:i+1])
+        if sol[i] != 0:
+            a.remove(0)
+        # mark all visited nodes as invalid
+        mask[i, list(a)] = float("-inf")
+
+        # mark all infeasible demand nodes as invalid
+        # this crazy implementation is due to cProfile saying 
+        # list comprehension is super slow. numpy is fast.
+        c_nodes = list(set(prob) - set(sol[:i+1]) - set([0]))
+        last_route = solution_to_routes(sol[:i+1], partial=True)[-1]
+        cur_demand = get_route_demand(last_route, demands)
+        c_demands = demands[c_nodes]
+        next_demands = c_demands + cur_demand
+        sel = np.squeeze(np.argwhere(next_demands > capacity))
+        infeasible_nodes = np.array(c_nodes)[sel]
+        print(sol[i], infeasible_nodes, last_route, cur_demand)
+        if a == set(prob):
+            mask[i, :] = 0
+        else:
+            mask[i, infeasible_nodes.tolist()] = float("-inf")
+    return mask
```

### Comparing `routeml-0.6.0/routeml.egg-info/PKG-INFO` & `routeml-0.7.0/routeml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeml
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python package for CVRP utilities
 Home-page: https://github.com/jkschin/routeml
 Author: Your Name
 Author-email: jkschin@mit.edu
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `routeml-0.6.0/routeml.egg-info/SOURCES.txt` & `routeml-0.7.0/routeml.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 tests/integration/__init__.py
 tests/integration/test_draw_integration.py
 tests/integration/test_vrplib_cost_integration.py
 tests/unit/__init__.py
 tests/unit/utils/__init__.py
 tests/unit/utils/test_get_cvrp_cost.py
 tests/unit/utils/test_get_is_feasible.py
+tests/unit/utils/test_get_logit_mask.py
 tests/unit/utils/test_get_route_demand.py
 tests/unit/utils/test_pad_matrices.py
 tests/unit/utils/test_parse_vrplib_file.py
 tests/unit/utils/test_parse_vrplib_solution.py
 tests/unit/utils/test_routes_to_solution.py
 tests/unit/utils/test_solution_to_adj_mat.py
 tests/unit/utils/test_solution_to_routes.py
```

### Comparing `routeml-0.6.0/setup.py` & `routeml-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='routeml',
-    version='0.6.0',
+    version='0.7.0',
     description='Python package for CVRP utilities',
     author='Your Name',
     author_email='jkschin@mit.edu',
     url='https://github.com/jkschin/routeml',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `routeml-0.6.0/tests/integration/test_draw_integration.py` & `routeml-0.7.0/tests/integration/test_draw_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/integration/test_vrplib_cost_integration.py` & `routeml-0.7.0/tests/integration/test_vrplib_cost_integration.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_get_cvrp_cost.py` & `routeml-0.7.0/tests/unit/utils/test_get_cvrp_cost.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_get_is_feasible.py` & `routeml-0.7.0/tests/unit/utils/test_get_is_feasible.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_get_route_demand.py` & `routeml-0.7.0/tests/unit/utils/test_get_route_demand.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,70 @@
 import unittest
-from routeml.utils import get_route_demand
+from routeml.utils import get_all_route_demands, get_route_demand
 
 class TestGetRouteDemand(unittest.TestCase):
     def test_get_route_demand(self):
         routes = [[0, 1, 2, 0], [0, 3, 4, 0], [0, 5, 6, 7, 0]]
         demand = {0: 0, 1: 10, 2: 20, 3: 15, 4: 25, 5: 30, 6: 5, 7: 8}
 
-        total_demand = get_route_demand(routes, demand)
+        total_demand = get_all_route_demands(routes, demand)
         self.assertEqual(total_demand, [30, 40, 43])
 
     def test_get_route_demand_empty_routes(self):
         routes = []
         demand = {0: 0, 1: 10, 2: 20}
 
-        total_demand = get_route_demand(routes, demand)
+        total_demand = get_all_route_demands(routes, demand)
         self.assertEqual(total_demand, [])
 
     def test_get_route_demand_empty_demand(self):
         routes = [[0, 1, 2, 0], [0, 3, 4, 0]]
         demand = {}
 
         with self.assertRaises(Exception) as context:
-            total_demand = get_route_demand(routes, demand)
+            total_demand = get_all_route_demands(routes, demand)
         
         self.assertEqual(str(context.exception), "Node 0 not found in the demand dictionary")
 
     def test_get_route_demand_zero_demand(self):
         routes = [[0, 1, 2, 0], [0, 3, 4, 0]]
         demand = {0: 0, 1: 0, 2: 0, 3: 0, 4: 0}
 
-        total_demand = get_route_demand(routes, demand)
+        total_demand = get_all_route_demands(routes, demand)
         self.assertEqual(total_demand, [0, 0])
 
     def test_get_route_demand_with_missing_node(self):
         routes = [[1, 2, 3], [4, 5, 6]]
         demand = {1: 10, 2: 20, 4: 15, 6: 30}
         
         with self.assertRaises(Exception) as context:
-            total_demand = get_route_demand(routes, demand)
+            total_demand = get_all_route_demands(routes, demand)
         
         self.assertEqual(str(context.exception), "Node 3 not found in the demand dictionary")
 
+    def test_empty_route(self):
+        route = []
+        demands = []
+        self.assertEqual(get_route_demand(route, demands), 0)
+
+    def test_non_empty_route_positive_demands(self):
+        route = [0, 1, 2, 3, 4, 5]
+        demands = [0, 10, 5, 8, 12, 3]
+        self.assertEqual(get_route_demand(route, demands), 38)
+
+    def test_non_empty_route_zero_demands(self):
+        route = [0, 1, 2]
+        demands = [0, 0, 0]
+        self.assertEqual(get_route_demand(route, demands), 0)
+
+    def test_route_with_duplicate_nodes(self):
+        route = [0, 1, 2, 3, 2, 4, 1]
+        demands = [0, 5, 3, 2, 4, 6]
+        self.assertEqual(get_route_demand(route, demands), 22)
+
+    def test_route_with_negative_demands(self):
+        route = [0, 4, 3, 2, 1]
+        demands = [0, -10, -5, -8, -12]
+        self.assertEqual(get_route_demand(route, demands), -35)
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `routeml-0.6.0/tests/unit/utils/test_pad_matrices.py` & `routeml-0.7.0/tests/unit/utils/test_pad_matrices.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_parse_vrplib_file.py` & `routeml-0.7.0/tests/unit/utils/test_parse_vrplib_file.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_parse_vrplib_solution.py` & `routeml-0.7.0/tests/unit/utils/test_parse_vrplib_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_routes_to_solution.py` & `routeml-0.7.0/tests/unit/utils/test_routes_to_solution.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_solution_to_adj_mat.py` & `routeml-0.7.0/tests/unit/utils/test_solution_to_adj_mat.py`

 * *Files identical despite different names*

### Comparing `routeml-0.6.0/tests/unit/utils/test_solution_to_routes.py` & `routeml-0.7.0/tests/unit/utils/test_solution_to_routes.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,9 +22,21 @@
 
     def test_solution_to_routes_multiple_routes(self):
         solution = [0, 1, 0, 2, 3, 0, 4, 0]
         expected_routes = [[0, 1, 0], [0, 2, 3, 0], [0, 4, 0]]
         routes = solution_to_routes(solution)
         self.assertEqual(routes, expected_routes)
 
+    def test_partial_solution_to_routes_1(self):
+        solution = [0, 1, 0, 2, 3, 0, 4]
+        expected_routes = [[0, 1, 0], [0, 2, 3, 0], [0, 4]]
+        routes = solution_to_routes(solution, partial=True)
+        self.assertEqual(routes, expected_routes)
+
+    def test_partial_solution_to_routes_2(self):
+        solution = [0, 1, 0, 2, 3, 0, 4, 5]
+        expected_routes = [[0, 1, 0], [0, 2, 3, 0], [0, 4, 5]]
+        routes = solution_to_routes(solution, partial=True)
+        self.assertEqual(routes, expected_routes)
+
 if __name__ == '__main__':
     unittest.main()
```

