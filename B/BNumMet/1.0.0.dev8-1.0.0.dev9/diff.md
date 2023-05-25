# Comparing `tmp/BNumMet-1.0.0.dev8.tar.gz` & `tmp/BNumMet-1.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BNumMet-1.0.0.dev8.tar", last modified: Mon Apr 17 15:37:09 2023, max compression
+gzip compressed data, was "BNumMet-1.0.0.dev9.tar", last modified: Thu Apr 27 15:28:28 2023, max compression
```

## Comparing `BNumMet-1.0.0.dev8.tar` & `BNumMet-1.0.0.dev9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-04-17 15:36:47.000000 BNumMet-1.0.0.dev8/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.628353 BNumMet-1.0.0.dev8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet/
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/LinearSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/InterpolationVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LUVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/NonLinearVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/RandomVisualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/src/BNumMet/module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.632353 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    50394 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-17 15:37:09.000000 BNumMet-1.0.0.dev8/src/BNumMet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:37:09.636353 BNumMet-1.0.0.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_General.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_Interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_LeastSquares.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_LinealSystems.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_NonLinear.py
--rw-r--r--   0 runner    (1001) docker     (123)    11535 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_Random.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-17 15:36:48.000000 BNumMet-1.0.0.dev8/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.988199 BNumMet-1.0.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    53433 2023-04-27 15:28:28.988199 BNumMet-1.0.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-27 15:28:28.988199 BNumMet-1.0.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.980198 BNumMet-1.0.0.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.984199 BNumMet-1.0.0.dev9/src/BNumMet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12405 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/LinearSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.984199 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/InterpolationVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/LUVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/LeastSquaresVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27252 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/NonLinearVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/RandomVisualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/src/BNumMet/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.984199 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    53433 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 15:28:28.000000 BNumMet-1.0.0.dev9/src/BNumMet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 15:28:28.988199 BNumMet-1.0.0.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_General.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_Interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_LeastSquares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_LinealSystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_NonLinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_Random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-27 15:28:05.000000 BNumMet-1.0.0.dev9/tests/test_module.py
```

### Comparing `BNumMet-1.0.0.dev8/LICENSE` & `BNumMet-1.0.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/PKG-INFO` & `BNumMet-1.0.0.dev9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev8
+Version: 1.0.0.dev9
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
@@ -128,14 +128,59 @@
 
 ```bash
 python tests/__init__.py # Run tests
 
 # It will generate a coverage report in the Tests/coverage folder in different formats (html, xml, lcov). 
 # It will also format the code using the Black Library (I Might've forgottent to do so :) )
 ```
+## BNumMet Library Structure
+
+```
+BNumMet
+	* LinearSystems
+		- lu( matrix ) --> P,L,U matrices as np.array
+		- permute( matrix, row_1, row_2) --> Permuted Matrix as np.array
+		- forward_substitution( matrix_L, matrix_b ) --> Solution to Lx=b as np.array
+		- backward_substitution( matrix_U, matrix_b ) --> Solution to Ux=b as np.array
+		- lu_solve ( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using LU Decomposition
+		- qr_factorization ( matrix_A ) --> Q,R Matrices as np.array
+		- qr_solve( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using QR decomposition
+ 		- interactive_lu( matrix_p, matrix_l, matrix_u, col, row, pivot_row) --> An iteration of LU Decomposition
+	* Interpolation
+		- polinomial(interpolation_x, interpolation_y, mesh) --> Polinomial-Interpolated values over mesh
+		- piecewise_linear(interpolation_x, interpolation_y, mesh) --> Piecewise Linear-Interpolated values over mesh
+		- pchip(interpolation_x, interpolation_y, mesh) --> Piecewise Cubic Hermite-Interpolated values over mesh
+		- splines(interpolation_x, interpolation_y, mesh) --> Piecewise Cubix-Interpolated values over mesh
+	* NonLinear
+		- bisect( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- secant( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- newton( function, derivative, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- IQI( function, values_of_x:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- zBrentDekker( function, interval:tuple, tol, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken	
+	* Random
+		- clear_lehmers_vars() --> Cleans the initiated values of the Lehmers random number generator
+		- lehmers_init(a, c, m, x) --> Initializes Lehmers R.N.G. with values given
+		- lehmers_rand(a, c, m, x) --> Initializes and produces a random number every time it is called
+		- clear_marsaglia_vars() --> Cleans the initiated values of the Marsaglia's random number generator
+		- marsaglia_init(base, lag_r, lag_s, carry, seed_tuple) --> Initializes Marsaglia's R.N.G. with values given
+		- marsaglia_rand(base, lag_r, lag_s, carry, seed_tuple) --> Initializes and produces a random number every time it is called
+		- clear_mt_vars() --> Cleans the initiated values of the Mersenne Twister random number generator
+		- sgenrand(seed:int) --> Initializes and produces a random number every time it is called
+	* Visualizers
+		- LUVisualizer
+			- LUVisualizer:Class 
+		- InterpolationVisualizer
+			- InterpolVisualizer:Class 
+		- NonLinearVisualizer
+			- NonLinearVisualizer:Class 
+		- LeastSquaresVisualizer
+			- LSPVisualizer:Class 
+		- RandomVisualizer
+			- RandomVisualizer:Class 
+```
 
 ## BNumMet - Structure
 ----
 ```bash
 .
 ├── Demos # Contains the Jupyter Notebooks with the demos
 │   ├── Interpolation.ipynb
```

### Comparing `BNumMet-1.0.0.dev8/Readme.md` & `BNumMet-1.0.0.dev9/Readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -89,14 +89,59 @@
 
 ```bash
 python tests/__init__.py # Run tests
 
 # It will generate a coverage report in the Tests/coverage folder in different formats (html, xml, lcov). 
 # It will also format the code using the Black Library (I Might've forgottent to do so :) )
 ```
+## BNumMet Library Structure
+
+```
+BNumMet
+	* LinearSystems
+		- lu( matrix ) --> P,L,U matrices as np.array
+		- permute( matrix, row_1, row_2) --> Permuted Matrix as np.array
+		- forward_substitution( matrix_L, matrix_b ) --> Solution to Lx=b as np.array
+		- backward_substitution( matrix_U, matrix_b ) --> Solution to Ux=b as np.array
+		- lu_solve ( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using LU Decomposition
+		- qr_factorization ( matrix_A ) --> Q,R Matrices as np.array
+		- qr_solve( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using QR decomposition
+ 		- interactive_lu( matrix_p, matrix_l, matrix_u, col, row, pivot_row) --> An iteration of LU Decomposition
+	* Interpolation
+		- polinomial(interpolation_x, interpolation_y, mesh) --> Polinomial-Interpolated values over mesh
+		- piecewise_linear(interpolation_x, interpolation_y, mesh) --> Piecewise Linear-Interpolated values over mesh
+		- pchip(interpolation_x, interpolation_y, mesh) --> Piecewise Cubic Hermite-Interpolated values over mesh
+		- splines(interpolation_x, interpolation_y, mesh) --> Piecewise Cubix-Interpolated values over mesh
+	* NonLinear
+		- bisect( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- secant( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- newton( function, derivative, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- IQI( function, values_of_x:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- zBrentDekker( function, interval:tuple, tol, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken	
+	* Random
+		- clear_lehmers_vars() --> Cleans the initiated values of the Lehmers random number generator
+		- lehmers_init(a, c, m, x) --> Initializes Lehmers R.N.G. with values given
+		- lehmers_rand(a, c, m, x) --> Initializes and produces a random number every time it is called
+		- clear_marsaglia_vars() --> Cleans the initiated values of the Marsaglia's random number generator
+		- marsaglia_init(base, lag_r, lag_s, carry, seed_tuple) --> Initializes Marsaglia's R.N.G. with values given
+		- marsaglia_rand(base, lag_r, lag_s, carry, seed_tuple) --> Initializes and produces a random number every time it is called
+		- clear_mt_vars() --> Cleans the initiated values of the Mersenne Twister random number generator
+		- sgenrand(seed:int) --> Initializes and produces a random number every time it is called
+	* Visualizers
+		- LUVisualizer
+			- LUVisualizer:Class 
+		- InterpolationVisualizer
+			- InterpolVisualizer:Class 
+		- NonLinearVisualizer
+			- NonLinearVisualizer:Class 
+		- LeastSquaresVisualizer
+			- LSPVisualizer:Class 
+		- RandomVisualizer
+			- RandomVisualizer:Class 
+```
 
 ## BNumMet - Structure
 ----
 ```bash
 .
 ├── Demos # Contains the Jupyter Notebooks with the demos
 │   ├── Interpolation.ipynb
```

### Comparing `BNumMet-1.0.0.dev8/setup.cfg` & `BNumMet-1.0.0.dev9/setup.cfg`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Interpolation.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/LinearSystems.py` & `BNumMet-1.0.0.dev9/src/BNumMet/LinearSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/NonLinear.py` & `BNumMet-1.0.0.dev9/src/BNumMet/NonLinear.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             a, b, c, fa, fb, fc = b, c, b, fb, fc, fb
 
         # Update tolerance and m for the next iteration
         tolerance = 2 * np.finfo(float).eps * abs(b) + tol
         m = 0.5 * (c - b)
 
         iterations += 1
-
+        # print(b,e)
     zero = b
     if steps and iters:
         return zero, iterations, procedure_stack
     if iters:
         return zero, iterations
     if steps:
         return zero, procedure_stack
```

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Random.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Random.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/InterpolationVisualizer.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/InterpolationVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LUVisualizer.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/LUVisualizer.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/LeastSquaresVisualizer.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/LeastSquaresVisualizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         This function is called when the function type is changed
         """
         to_draw = [self.fig.marks[0]]  # the data points are always drawn
         to_grid = [self.function_type]  # the function type dropdown
         if (
             change["new"] == "Only data"
         ):  # if the function type is "Only data"  then we don't need to draw anything else
-            ...
+            self.remarks.value = ""  # clear the remarks
         elif (
             change["new"] == "Polynomial"
         ):  # if the function type is "Polynomial" then we need to
             to_grid.append(
                 self.polynomial_degree
             )  # add the polynomial degree dropdown to the grid
             self.polynomial_degree.max = (  # set the max degree to the number of data points - 1
```

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/NonLinearVisualizer.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/NonLinearVisualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,16 +290,16 @@
         new_point_b = self.next_points_addition[b.pointIndex]  # Get the next point
         self.b = (
             new_point_b
             if abs(self.b - new_point_b) > self.tolerance
             else self.b + np.sign(0.5 * (self.c - self.b)) * self.tolerance
         )  # If the new point is too close to the current point, move it a little bit
         self.fb = self.f(self.b)  # Set f(b) = f(newB)
-        self.e = self.errs[b.pointIndex]  # Set e = error
-
+        if b.pointIndex != 1:
+            self.e = self.errs[b.pointIndex]  # Set e = error
         self.iterations += 1  # Increment the number of iterations
 
         # Section: Ext
         self.section_ext()  # Update the section
         # Section: Int
         self.section_int()  # Update the section
 
@@ -464,17 +464,33 @@
             if self.next_points_addition[2] is None
             else [
                 self.next_points_addition[2]
             ]  # If the IQI point is None, add it to the list
         )
 
         if self.hint_step is None:  # If the hint step is None
+            # set the original function
+            self.x = np.linspace(min(self.original_data), max(self.original_data), 1000)
+            self.default_lines()
+            # Adjust the scales
+            self.x_sc.min = min(self.original_data)
+            self.x_sc.max = max(self.original_data)
+            self.y_sc.min = min(self.function_line.y)
+            self.y_sc.max = max(self.function_line.y)
+
             self.fig.marks = [
                 self.horizontal_line,
                 self.function_line,
+                draw_point(  # Draw the current solution
+                    self.b,
+                    0,
+                    "red",
+                    "Current Solution",
+                    "circle",
+                ),
             ]  # Set the marks to the function and the horizontal line
             return
 
         min_max = [
             min(points2check),
             max(points2check),
         ]  # Get the min and max of the points to check
@@ -487,15 +503,15 @@
                 max(max(self.original_data), min_max[1]),
                 1000,
             )
             self.default_lines()  # Set the default lines
             self.widen = True  # Set widen to True
         elif self.widen:  # If widen is True
             self.x = np.linspace(
-                min(self.original_data), max(self.original_data), 1000
+                min(self.original_data), max(self.original_data), 10000
             )  # Set the x values to the min and max of the original data
             self.default_lines()  # Set the default lines
             self.widen = False  # Set widen to False
 
         marks2plot = [
             self.horizontal_line,
             self.function_line,
@@ -603,15 +619,15 @@
         with self.current_solution_output:  # Print the current solution
             print(
                 f"Current Solution: ({self.b:.4e}, {self.f(self.b):.4e})"
             )  # Print the current solution
             print(f"Iterations: {self.iterations}")  # Print the iterations
         with self.helper_output:  # Print the helper text
             print(  # Print the helper text
-                f"Next Step suggestion: {self.hint_step if self.hint_step is not None else 'FINISHED'}"
+                f"Next Step suggested by Brent-Dekker: {self.hint_step if self.hint_step is not None else 'FINISHED'}"
             )
 
     def run(self):
         """
         This method sets up everything and runs the app
 
         Returns
@@ -681,14 +697,16 @@
             if p2 > 0:
                 q2 = -q2
             else:
                 p2 = -p2
 
             pq_pair = (p2, q2)
 
+            self.s = self.e
+
         if p1 > 0:
             q1 = -q1
         else:
             p1 = -p1
 
         # Store e-Values for next step
         errs[1] = abs(p1 / q1)  # Secant always exists
```

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/Visualizers/RandomVisualizer.py` & `BNumMet-1.0.0.dev9/src/BNumMet/Visualizers/RandomVisualizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -58,27 +58,31 @@
         x = np.linspace(0, 1, 1000)
         y = np.sqrt(1 / 4 - (x - 0.5) ** 2)
         y = np.concatenate((y, -y))  # y
         y += 0.5
         x = np.concatenate((x, (x[::-1])))  # x
 
         self.circle = bq.Lines(
-            x=x, y=y, scales={"x": self.x_sc, "y": self.y_sc}, colors=["red"]
+            x=x,
+            y=y,
+            scales={"x": self.x_sc, "y": self.y_sc},
+            colors=["red"],
+            stroke_width=5,
         )
         self.figure1.marks = [self.square, self.circle]
 
         # Prepare the figure for the points
         self.points = bq.Scatter(
             x=[],
             y=[],
             scales={"x": self.x_sc, "y": self.y_sc},
             colors=["blue"],
-            default_size=5,
+            default_size=2,
         )
-        self.figure1.marks = [self.square, self.circle, self.points]
+        self.figure1.marks = [self.points, self.square, self.circle]
 
         # Figure 2: (Current value and Pi) vs. (Number of iterations)
         # =================================================================================================
         self.figure2 = bq.Figure(title="Convergence of Pi", legend_location="top-right")
         self.x_sc2 = bq.LinearScale()  # x scale
         self.y_sc2 = bq.LinearScale()  # y scale
         ax_x2 = bq.Axis(
@@ -126,15 +130,15 @@
         self.figure2.marks = [self.pi_line, self.current_value_line]
 
         # Widget: Number of Points to generate
         # =================================================================================================
         self.iterations_widget = widgets.BoundedIntText(
             value=self.iterations,
             min=1,
-            max=1000,
+            max=10000,
             description="Iterations:",
             disabled=False,
         )
 
         # Widget: Button for running the algorithm
         # =================================================================================================
         self.run_button = widgets.Button(
@@ -143,26 +147,26 @@
             button_style="",  # 'success', 'info', 'warning', 'danger' or ''
             tooltip="Run",
             icon="check",  # (FontAwesome names without the `fa-` prefix)
         )
         # Observer: Button for running the algorithm
         self.run_button.on_click(self.play_montecarlo)
 
-        self.pi_value = widgets.FloatText( # Widget: Pi value
+        self.pi_value = widgets.FloatText(  # Widget: Pi value
             value=0,
             description="$\pi$:",
             disabled=True,
         )
         # Widget: Grid
         # =================================================================================================
         self.grid = widgets.GridspecLayout(4, 4)
         self.grid[0:2, 0:2] = self.figure1
         self.grid[2:4, 0:4] = self.figure2
-        self.grid[0:1, 2:4] = widgets.VBox([self.iterations_widget,self.run_button])
-        
+        self.grid[0:1, 2:4] = widgets.VBox([self.iterations_widget, self.run_button])
+
         self.grid[1:2, 2:4] = self.pi_value
 
     def number_of_iterations(self):
         """
         Updates the number of iterations. This is called when the user plays the animation. It configures the x axis of the second figure. and the number of iterations of the algorithm.
         """
         self.iterations = self.iterations_widget.value
@@ -178,38 +182,56 @@
         self.generated_numbers = []
         self.current_value = 0
         self.inside_circle = 0
         self.points.x = []
         self.points.y = []
         self.current_value_line.x = []
         self.current_value_line.y = []
-
+        self.total_points = 0
         self.run_button.disabled = True
 
+        batch_coords = []
+        batch_current_value = []
+        batch_current_iteration = []
+        batch_size = int(self.iterations / 100) * (2 if self.iterations < 2000 else 5)
+
         for self.current_iteration in range(self.iterations):
             new_x = self.random_generator()
             new_y = self.random_generator()
-            self.generated_numbers.append([new_x, new_y])
-            with self.points.hold_sync():  # Animation for the points
-                self.points.x = [x[0] for x in self.generated_numbers]
-                self.points.y = [x[1] for x in self.generated_numbers]
+            self.total_points += 1
+
+            batch_coords.append([new_x, new_y])
             if ((new_x - 0.5) ** 2 + (new_y - 0.5) ** 2) <= 0.25:
                 self.inside_circle += 1
-            # sleep(0.0001)
-            self.current_value = 4 * self.inside_circle / len(self.generated_numbers)
+            batch_current_value.append(4 * self.inside_circle / self.total_points)
+
+            batch_current_iteration.append(self.current_iteration)
 
-            with self.current_value_line.hold_sync():  # Animation for the current value
-                self.current_value_line.x = [x for x in self.current_value_line.x] + [
-                    self.current_iteration
-                ]
-                self.current_value_line.y = [y for y in self.current_value_line.y] + [
-                    self.current_value
-                ]
-                self.pi_value.value = self.current_value
-            sleep(0.0001)
+            if (
+                len(batch_coords) >= batch_size
+                or self.current_iteration == self.iterations - 1
+            ):
+                aux = self.generated_numbers + batch_coords
+                with self.grid.hold_sync():
+                    with self.points.hold_sync():
+                        self.points.x = [x[0] for x in aux]
+                        self.points.y = [x[1] for x in aux]
+                    with self.current_value_line.hold_sync():
+                        self.current_value_line.x = (
+                            list(self.current_value_line.x) + batch_current_iteration
+                        )  # [x for x in self.current_value_line.x] + batch_current_iteration
+                        self.current_value_line.y = (
+                            list(self.current_value_line.y) + batch_current_value
+                        )  # [x for x in self.current_value_line.y] + batch_current_value
+                    self.pi_value.value = batch_current_value[-1]
+                    self.generated_numbers += batch_coords
+
+                batch_coords = []
+                batch_current_value = []
+                batch_current_iteration = []
 
         self.run_button.disabled = False
 
     def run(self):
         """
         Runs the visualizer.
         """
```

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet/module.py` & `BNumMet-1.0.0.dev9/src/BNumMet/module.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet.egg-info/PKG-INFO` & `BNumMet-1.0.0.dev9/src/BNumMet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BNumMet
-Version: 1.0.0.dev8
+Version: 1.0.0.dev9
 Summary: Basic Numerical Methods for Python 3
 Home-page: https://github.com/fbpazos/Trabajo-Fin-Master/tree/main/Python_BNumMet
 Author: Fernando Bellido Pazos
 Author-email: fbellidopazos@gmail.com
 License: AGPL-3.0
 Platform: unix
 Platform: linux
@@ -128,14 +128,59 @@
 
 ```bash
 python tests/__init__.py # Run tests
 
 # It will generate a coverage report in the Tests/coverage folder in different formats (html, xml, lcov). 
 # It will also format the code using the Black Library (I Might've forgottent to do so :) )
 ```
+## BNumMet Library Structure
+
+```
+BNumMet
+	* LinearSystems
+		- lu( matrix ) --> P,L,U matrices as np.array
+		- permute( matrix, row_1, row_2) --> Permuted Matrix as np.array
+		- forward_substitution( matrix_L, matrix_b ) --> Solution to Lx=b as np.array
+		- backward_substitution( matrix_U, matrix_b ) --> Solution to Ux=b as np.array
+		- lu_solve ( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using LU Decomposition
+		- qr_factorization ( matrix_A ) --> Q,R Matrices as np.array
+		- qr_solve( matrix_A, matrix_b ) --> Solution to Ax=b as np.array using QR decomposition
+ 		- interactive_lu( matrix_p, matrix_l, matrix_u, col, row, pivot_row) --> An iteration of LU Decomposition
+	* Interpolation
+		- polinomial(interpolation_x, interpolation_y, mesh) --> Polinomial-Interpolated values over mesh
+		- piecewise_linear(interpolation_x, interpolation_y, mesh) --> Piecewise Linear-Interpolated values over mesh
+		- pchip(interpolation_x, interpolation_y, mesh) --> Piecewise Cubic Hermite-Interpolated values over mesh
+		- splines(interpolation_x, interpolation_y, mesh) --> Piecewise Cubix-Interpolated values over mesh
+	* NonLinear
+		- bisect( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- secant( function, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- newton( function, derivative, interval:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- IQI( function, values_of_x:tuple, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken
+		- zBrentDekker( function, interval:tuple, tol, stop_iters:int, iters:bool, *args) --> x-value of where the zero is at and as optional the number of iterations taken	
+	* Random
+		- clear_lehmers_vars() --> Cleans the initiated values of the Lehmers random number generator
+		- lehmers_init(a, c, m, x) --> Initializes Lehmers R.N.G. with values given
+		- lehmers_rand(a, c, m, x) --> Initializes and produces a random number every time it is called
+		- clear_marsaglia_vars() --> Cleans the initiated values of the Marsaglia's random number generator
+		- marsaglia_init(base, lag_r, lag_s, carry, seed_tuple) --> Initializes Marsaglia's R.N.G. with values given
+		- marsaglia_rand(base, lag_r, lag_s, carry, seed_tuple) --> Initializes and produces a random number every time it is called
+		- clear_mt_vars() --> Cleans the initiated values of the Mersenne Twister random number generator
+		- sgenrand(seed:int) --> Initializes and produces a random number every time it is called
+	* Visualizers
+		- LUVisualizer
+			- LUVisualizer:Class 
+		- InterpolationVisualizer
+			- InterpolVisualizer:Class 
+		- NonLinearVisualizer
+			- NonLinearVisualizer:Class 
+		- LeastSquaresVisualizer
+			- LSPVisualizer:Class 
+		- RandomVisualizer
+			- RandomVisualizer:Class 
+```
 
 ## BNumMet - Structure
 ----
 ```bash
 .
 ├── Demos # Contains the Jupyter Notebooks with the demos
 │   ├── Interpolation.ipynb
```

### Comparing `BNumMet-1.0.0.dev8/src/BNumMet.egg-info/SOURCES.txt` & `BNumMet-1.0.0.dev9/src/BNumMet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_General.py` & `BNumMet-1.0.0.dev9/tests/test_General.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_Interpolation.py` & `BNumMet-1.0.0.dev9/tests/test_Interpolation.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_LeastSquares.py` & `BNumMet-1.0.0.dev9/tests/test_LeastSquares.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_LinealSystems.py` & `BNumMet-1.0.0.dev9/tests/test_LinealSystems.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_NonLinear.py` & `BNumMet-1.0.0.dev9/tests/test_NonLinear.py`

 * *Files identical despite different names*

### Comparing `BNumMet-1.0.0.dev8/tests/test_Random.py` & `BNumMet-1.0.0.dev9/tests/test_Random.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,14 +280,14 @@
         # Tests that the RandomVisualizer is initiated correctly without any arguments
         # No Exceptions should be raised
         rv = RandomVisualizer()
         rv.run()
 
         rv.iterations_widget.value = 10000
         self.assertEqual(
-            rv.iterations_widget.value, 1000
+            rv.iterations_widget.value, 10000
         )  # Should be 1000 because of the max value
 
         rv.iterations_widget.value = 0
         self.assertEqual(
             rv.iterations_widget.value, 1
         )  # Should be 1 because of the min value
```

### Comparing `BNumMet-1.0.0.dev8/tests/test_module.py` & `BNumMet-1.0.0.dev9/tests/test_module.py`

 * *Files identical despite different names*

