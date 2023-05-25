# Comparing `tmp/control-vegas-1.1.0.tar.gz` & `tmp/control-vegas-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-vegas-1.1.0.tar", last modified: Wed Apr 19 20:38:06 2023, max compression
+gzip compressed data, was "control-vegas-1.2.0.tar", last modified: Thu May 25 16:31:08 2023, max compression
```

## Comparing `control-vegas-1.1.0.tar` & `control-vegas-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-04-19 20:38:06.154738 control-vegas-1.1.0/
--rw-r--r--   0 person    (1000) person    (1000)       66 2023-03-31 14:30:55.000000 control-vegas-1.1.0/.gitattributes
--rw-r--r--   0 person    (1000) person    (1000)      114 2023-03-31 14:30:55.000000 control-vegas-1.1.0/.gitignore
--rw-r--r--   0 person    (1000) person    (1000)    35149 2023-03-31 14:30:55.000000 control-vegas-1.1.0/LICENSE
--rw-r--r--   0 person    (1000) person    (1000)    48242 2023-04-19 20:38:06.154738 control-vegas-1.1.0/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)     6760 2023-04-12 21:22:36.000000 control-vegas-1.1.0/README.md
--rw-r--r--   0 person    (1000) person    (1000)     1275 2023-04-19 20:36:14.000000 control-vegas-1.1.0/pyproject.toml
--rw-r--r--   0 person    (1000) person    (1000)       38 2023-04-19 20:38:06.154738 control-vegas-1.1.0/setup.cfg
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-04-19 20:38:06.151404 control-vegas-1.1.0/src/
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-04-19 20:38:06.154738 control-vegas-1.1.0/src/control_vegas/
--rw-r--r--   0 person    (1000) person    (1000)      256 2023-04-19 19:57:46.000000 control-vegas-1.1.0/src/control_vegas/__init__.py
--rw-r--r--   0 person    (1000) person    (1000)       76 2023-04-12 21:33:59.000000 control-vegas-1.1.0/src/control_vegas/_exceptions.py
--rw-r--r--   0 person    (1000) person    (1000)      340 2023-04-19 18:46:05.000000 control-vegas-1.1.0/src/control_vegas/_types.py
--rw-r--r--   0 person    (1000) person    (1000)    10282 2023-04-19 20:29:39.000000 control-vegas-1.1.0/src/control_vegas/functions.py
--rw-r--r--   0 person    (1000) person    (1000)    20026 2023-04-19 20:29:16.000000 control-vegas-1.1.0/src/control_vegas/mccv.py
--rw-r--r--   0 person    (1000) person    (1000)     4444 2023-04-19 18:39:01.000000 control-vegas-1.1.0/src/control_vegas/utilities.py
-drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-04-19 20:38:06.154738 control-vegas-1.1.0/src/control_vegas.egg-info/
--rw-r--r--   0 person    (1000) person    (1000)    48242 2023-04-19 20:38:06.000000 control-vegas-1.1.0/src/control_vegas.egg-info/PKG-INFO
--rw-r--r--   0 person    (1000) person    (1000)      441 2023-04-19 20:38:06.000000 control-vegas-1.1.0/src/control_vegas.egg-info/SOURCES.txt
--rw-r--r--   0 person    (1000) person    (1000)        1 2023-04-19 20:38:06.000000 control-vegas-1.1.0/src/control_vegas.egg-info/dependency_links.txt
--rw-r--r--   0 person    (1000) person    (1000)      105 2023-04-19 20:38:06.000000 control-vegas-1.1.0/src/control_vegas.egg-info/requires.txt
--rw-r--r--   0 person    (1000) person    (1000)       14 2023-04-19 20:38:06.000000 control-vegas-1.1.0/src/control_vegas.egg-info/top_level.txt
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.809237 control-vegas-1.2.0/
+-rw-r--r--   0 person    (1000) person    (1000)       66 2023-03-31 14:30:55.000000 control-vegas-1.2.0/.gitattributes
+-rw-r--r--   0 person    (1000) person    (1000)      114 2023-03-31 14:30:55.000000 control-vegas-1.2.0/.gitignore
+-rw-r--r--   0 person    (1000) person    (1000)      634 2023-05-25 16:27:17.000000 control-vegas-1.2.0/CITATION.cff
+-rw-r--r--   0 person    (1000) person    (1000)    35149 2023-03-31 14:30:55.000000 control-vegas-1.2.0/LICENSE
+-rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-25 16:31:08.805904 control-vegas-1.2.0/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)     8318 2023-05-25 16:14:49.000000 control-vegas-1.2.0/README.md
+-rw-r--r--   0 person    (1000) person    (1000)     1282 2023-05-25 16:29:32.000000 control-vegas-1.2.0/pyproject.toml
+-rw-r--r--   0 person    (1000) person    (1000)       38 2023-05-25 16:31:08.809237 control-vegas-1.2.0/setup.cfg
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/control_vegas/
+-rw-r--r--   0 person    (1000) person    (1000)      264 2023-05-13 08:27:23.000000 control-vegas-1.2.0/src/control_vegas/__init__.py
+-rw-r--r--   0 person    (1000) person    (1000)       76 2023-04-12 21:33:59.000000 control-vegas-1.2.0/src/control_vegas/_exceptions.py
+-rw-r--r--   0 person    (1000) person    (1000)      340 2023-05-13 08:25:27.000000 control-vegas-1.2.0/src/control_vegas/_types.py
+-rw-r--r--   0 person    (1000) person    (1000)    22721 2023-05-13 08:25:08.000000 control-vegas-1.2.0/src/control_vegas/cvintegrator.py
+-rw-r--r--   0 person    (1000) person    (1000)    10282 2023-05-13 08:23:18.000000 control-vegas-1.2.0/src/control_vegas/functions.py
+-rw-r--r--   0 person    (1000) person    (1000)     4789 2023-05-13 07:34:13.000000 control-vegas-1.2.0/src/control_vegas/utilities.py
+drwxr-xr-x   0 person    (1000) person    (1000)        0 2023-05-25 16:31:08.805904 control-vegas-1.2.0/src/control_vegas.egg-info/
+-rw-r--r--   0 person    (1000) person    (1000)    49800 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/PKG-INFO
+-rw-r--r--   0 person    (1000) person    (1000)      462 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/SOURCES.txt
+-rw-r--r--   0 person    (1000) person    (1000)        1 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/dependency_links.txt
+-rw-r--r--   0 person    (1000) person    (1000)      111 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/requires.txt
+-rw-r--r--   0 person    (1000) person    (1000)       14 2023-05-25 16:31:08.000000 control-vegas-1.2.0/src/control_vegas.egg-info/top_level.txt
```

### Comparing `control-vegas-1.1.0/LICENSE` & `control-vegas-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `control-vegas-1.1.0/PKG-INFO` & `control-vegas-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-vegas
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Control Variate wrapper over the vegas python package.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,17 +717,17 @@
 where the $*$ represents the optimal value. Plugging in $c^\*$ gives us a final variance of
 $$\text{Var}(f_c^\*)=\text{Var}(f)-\frac{\text{Cov}^2(f,g)}{\text{Var}(g)}=\left(1-\rho^2(f,g)\right)\text{Var}(f)\qquad\text{where}\qquad\rho(f,g)=\frac{\text{Cov}(f,g)}{\sqrt{\text{Var}(f)\text{Var}(g)}}$$
 is the correlation coefficient between $f$ and $g$. Since $|\rho(f,g)|\le1$, then this choice of $c$ will always decrease the variance. The same prescription can be applied for $n$ control variates, rather than just one, which is used in this package.
 
 A control variate is applied by using `vegas`'s importance sampling adaptation. Since $\rho$ is larger when the functions have a linear relationship, we use these previously adapted maps as the control variates. One can specify using the $i$th iteration of `vegas` as the control variate when initializing the `CVIntegrator` class or specify a list of iterations to use for multiple control variates.
 
 ## Installation
-To install, `numpy` and `cython` must be installed beforehand due to the `gvar` package. Therefore, for `pip`:
+It can just be installed via `pip`:
 ```
-python -m pip install numpy Cython && python -m pip install control-vegas
+python -m pip install control-vegas
 ```
 
 ## Usage
 The workflow involes creating a `Function` class and then passing that to the `CVIntegrator`. The `Function` class contains the function to be integrated but also other information such as its name, the true value of the integration (if available) and parameters of the function. The `CVIntegrator` class does the integration and stores the results like mean and variance.
 
 ### Using a Built-In Function
 For example,
@@ -770,38 +770,72 @@
     return self.a * x[:, 0]**2 + self.b * x[:, 1]
 
 # Creating class with name 'WeightedPoly' and assigning values to the parameters in the function
 wpoly = make_func('WeightedPoly', dimension=2, function=f, name='Weighted Polynomial', a=0.3, b=0.6)
 # Print out parameters of class (note `true_value` isn't shown)
 print(wpoly, '\n')
 
-# Create integrator class and use the 20th iteration as the control  variate
-cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=20)
+# Create integrator class and use multiple control variates
+cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=[10, 15, 20, 25, 30, 35])
 # Run the integration
 cvi.integrate()
 
 # Print info
 cvi.compare(rounding=5)
 ```
 which outputs
 ```
-WeightedPoly(dimension=2, name=WeightedPoly, a=0.3, b=0.6) 
+WeightedPoly(dimension=2, name=Weighted Polynomial, a=0.3, b=0.6) 
 
-         |     No CVs     |    With CVs    
----------+----------------+----------------
-Mean     |     0.39996303 |     0.39993278
-Variance | 5.27324871e-09 | 4.86145624e-09
-St Dev   | 7.26171379e-05 | 6.97241439e-05
-VPR      |                |    7.80908493%
+         |   No CVs    |  With CVs   
+---------+-------------+-------------
+Mean     |     0.39984 |     0.40004
+Variance | 5.83781e-08 | 4.90241e-08
+St Dev   | 2.41616e-04 | 2.21414e-04
+VPR      |             |   16.02309%
 ```
 The reason the function is vectorized is because, on the backend, `vegas`'s `batchintegrand` is used which can greatly speed up the computation.
 
+### Be lazy!
+If you're rushed or lazy, you can use the `quick_integrate` function that does the steps above for you and returns the `CVIntegrator` object. So to run the previous code block, you would use
+```python
+cvi = quick_integrate(
+         function=f,
+         evals=1000,
+         tot_iters=50,
+         bounds=[(0, 1), (0, 1)],
+         cv_iters=20,
+         cname="WeightPoly",
+         name="Weighted Polynomial",
+         a=0.3, b=0.6
+)
+cvi.compare()
+```
+which outputs
+```
+         |  No CVs   | With CVs  
+---------+-----------+-----------
+Mean     |     0.400 |     0.400
+Variance | 5.826e-08 | 5.025e-08
+St Dev   | 2.414e-04 | 2.242e-04
+VPR      |           |   13.746%
+```
+Note that the arguments are `cname` and `name` are optional but `bounds` is not. The dimension of the integral is implied from `bounds` when using `quick_integrate` whereas it's taken from the `Function` class for the previous code blocks.
+
+### Specifying Control Variate Iterations
+There are multiple valid arguments that can be passed to `cv_iters` for both the `CVIntegrator` class and `quick_integrate` which we'll lay out here.
+- For using one control variate, pass a integer representing the iteration to use.
+- For multiple control variates, pass a list of integers representing the iterations to use.
+- The string 'all' will use every iteration.
+- The string `all%n` will use every iteration mod $n$. So if you specify `tot_iters=15` and `cv_iters='all%3'`, then then the iterations used will be `[3, 6, 9, 12]`
+- This can be shifted by instead using `all%n+b` where $b$ is the shift. So for `tot_iters=15` and `cv_iters='all%3+2'`, you'll get `[2, 5, 8, 11, 14]`.
+
 ### Manual Use of `Function` Class
 To access the function call, use `function` or `f`. So, using the second example, I can run
 ```python
 wpoly.f([1.2, 1.5]) # returns 1.3319999999999999
 wpoly.f([0.2, 1], [0.8, 0.8], [1, 2]) # returns array([0.612, 0.672, 1.5  ])
 ```
 This wraps around the private, vectorized `_function`/`_f` used by `vegas` so you don't have to worry about the proper `numpy` array shape
 
 ## Notes
-- By default, functions are integrated from 0 to 1.
+- By default, functions are integrated from 0 to 1 unless `quick_integrate` is used.
```

### Comparing `control-vegas-1.1.0/README.md` & `control-vegas-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 where the $*$ represents the optimal value. Plugging in $c^\*$ gives us a final variance of
 $$\text{Var}(f_c^\*)=\text{Var}(f)-\frac{\text{Cov}^2(f,g)}{\text{Var}(g)}=\left(1-\rho^2(f,g)\right)\text{Var}(f)\qquad\text{where}\qquad\rho(f,g)=\frac{\text{Cov}(f,g)}{\sqrt{\text{Var}(f)\text{Var}(g)}}$$
 is the correlation coefficient between $f$ and $g$. Since $|\rho(f,g)|\le1$, then this choice of $c$ will always decrease the variance. The same prescription can be applied for $n$ control variates, rather than just one, which is used in this package.
 
 A control variate is applied by using `vegas`'s importance sampling adaptation. Since $\rho$ is larger when the functions have a linear relationship, we use these previously adapted maps as the control variates. One can specify using the $i$th iteration of `vegas` as the control variate when initializing the `CVIntegrator` class or specify a list of iterations to use for multiple control variates.
 
 ## Installation
-To install, `numpy` and `cython` must be installed beforehand due to the `gvar` package. Therefore, for `pip`:
+It can just be installed via `pip`:
 ```
-python -m pip install numpy Cython && python -m pip install control-vegas
+python -m pip install control-vegas
 ```
 
 ## Usage
 The workflow involes creating a `Function` class and then passing that to the `CVIntegrator`. The `Function` class contains the function to be integrated but also other information such as its name, the true value of the integration (if available) and parameters of the function. The `CVIntegrator` class does the integration and stores the results like mean and variance.
 
 ### Using a Built-In Function
 For example,
@@ -73,38 +73,72 @@
     return self.a * x[:, 0]**2 + self.b * x[:, 1]
 
 # Creating class with name 'WeightedPoly' and assigning values to the parameters in the function
 wpoly = make_func('WeightedPoly', dimension=2, function=f, name='Weighted Polynomial', a=0.3, b=0.6)
 # Print out parameters of class (note `true_value` isn't shown)
 print(wpoly, '\n')
 
-# Create integrator class and use the 20th iteration as the control  variate
-cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=20)
+# Create integrator class and use multiple control variates
+cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=[10, 15, 20, 25, 30, 35])
 # Run the integration
 cvi.integrate()
 
 # Print info
 cvi.compare(rounding=5)
 ```
 which outputs
 ```
-WeightedPoly(dimension=2, name=WeightedPoly, a=0.3, b=0.6) 
+WeightedPoly(dimension=2, name=Weighted Polynomial, a=0.3, b=0.6) 
 
-         |     No CVs     |    With CVs    
----------+----------------+----------------
-Mean     |     0.39996303 |     0.39993278
-Variance | 5.27324871e-09 | 4.86145624e-09
-St Dev   | 7.26171379e-05 | 6.97241439e-05
-VPR      |                |    7.80908493%
+         |   No CVs    |  With CVs   
+---------+-------------+-------------
+Mean     |     0.39984 |     0.40004
+Variance | 5.83781e-08 | 4.90241e-08
+St Dev   | 2.41616e-04 | 2.21414e-04
+VPR      |             |   16.02309%
 ```
 The reason the function is vectorized is because, on the backend, `vegas`'s `batchintegrand` is used which can greatly speed up the computation.
 
+### Be lazy!
+If you're rushed or lazy, you can use the `quick_integrate` function that does the steps above for you and returns the `CVIntegrator` object. So to run the previous code block, you would use
+```python
+cvi = quick_integrate(
+         function=f,
+         evals=1000,
+         tot_iters=50,
+         bounds=[(0, 1), (0, 1)],
+         cv_iters=20,
+         cname="WeightPoly",
+         name="Weighted Polynomial",
+         a=0.3, b=0.6
+)
+cvi.compare()
+```
+which outputs
+```
+         |  No CVs   | With CVs  
+---------+-----------+-----------
+Mean     |     0.400 |     0.400
+Variance | 5.826e-08 | 5.025e-08
+St Dev   | 2.414e-04 | 2.242e-04
+VPR      |           |   13.746%
+```
+Note that the arguments are `cname` and `name` are optional but `bounds` is not. The dimension of the integral is implied from `bounds` when using `quick_integrate` whereas it's taken from the `Function` class for the previous code blocks.
+
+### Specifying Control Variate Iterations
+There are multiple valid arguments that can be passed to `cv_iters` for both the `CVIntegrator` class and `quick_integrate` which we'll lay out here.
+- For using one control variate, pass a integer representing the iteration to use.
+- For multiple control variates, pass a list of integers representing the iterations to use.
+- The string 'all' will use every iteration.
+- The string `all%n` will use every iteration mod $n$. So if you specify `tot_iters=15` and `cv_iters='all%3'`, then then the iterations used will be `[3, 6, 9, 12]`
+- This can be shifted by instead using `all%n+b` where $b$ is the shift. So for `tot_iters=15` and `cv_iters='all%3+2'`, you'll get `[2, 5, 8, 11, 14]`.
+
 ### Manual Use of `Function` Class
 To access the function call, use `function` or `f`. So, using the second example, I can run
 ```python
 wpoly.f([1.2, 1.5]) # returns 1.3319999999999999
 wpoly.f([0.2, 1], [0.8, 0.8], [1, 2]) # returns array([0.612, 0.672, 1.5  ])
 ```
 This wraps around the private, vectorized `_function`/`_f` used by `vegas` so you don't have to worry about the proper `numpy` array shape
 
 ## Notes
-- By default, functions are integrated from 0 to 1.
+- By default, functions are integrated from 0 to 1 unless `quick_integrate` is used.
```

### Comparing `control-vegas-1.1.0/pyproject.toml` & `control-vegas-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools", "setuptools.scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "control-vegas"
-version = "1.1.0"
+version = "1.2.0"
 description = "A Control Variate wrapper over the vegas python package."
 authors = [
     {name = "Jacob Scott", email = "jscott137@pm.me"}
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dependencies = [
-    "numpy>=1.24",
+    "numpy<1.24, >=1.22",
     "vegas>=5.4",
     "nptyping>=2.5"
 ]
 keywords = ["Monte Carlo", "vegas", "control variates", "integration"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.9",
```

### Comparing `control-vegas-1.1.0/src/control_vegas/functions.py` & `control-vegas-1.2.0/src/control_vegas/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 
 @dataclass(repr=False)
 class ScalarTopLoop(Function):
     """
     A one-loop scalar box integral.
 
     Parameters:
-    s12, s23, s1, s2, s3, s4 (defaults 130**2, -130**2/, 0, 0, 0, 125**) =
+    s12, s23, s1, s2, s3, s4 (defaults 130**2, -130**2, 0, 0, 0, 125**2) =
         Parameters of function
     mtsq (default 173.9**2) - Square of top quark mass
     """
 
     s12: float = 130**2
     s23: float = -(130**2) / 2
     s1: float = 0
```

### Comparing `control-vegas-1.1.0/src/control_vegas/mccv.py` & `control-vegas-1.2.0/src/control_vegas/cvintegrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 File that holds the CVIntegrator class
 """
 
 from copy import deepcopy
 from itertools import product
 from numbers import Number
 from re import findall
+from sys import getsizeof
 from typing import Optional, Sequence, Union
 
 import numpy as np
 from nptyping import Float, NDArray, Shape
 from numpy.random import RandomState
 from vegas import Integrator
 
 from ._types import _ftype
 from .functions import Function, make_func
-from .utilities import check_value, timing
-
-# Should you print out the time it takes for the main 3 functions to run?
-TIMING = False
+from .utilities import check_attrs, timing
 
 
 def quick_integrate(
     function: _ftype,
     evals: int,
     tot_iters: int,
     bounds: Union[Sequence[tuple[float, float]], tuple[float, float]],
@@ -108,23 +106,29 @@
             map. Defaults to neval.
         jac_neval - The size of the Jacobian arrays, i.e. how finely split up the
             integration region is. Defaults to neval*nitn
         tot_neval - The total number of evaluations done when creating the fully adapted
             map.
     """
 
+    # Should you print out the time it takes for the main 3 functions to run?
+    TIMING = False
+    # Memory threshold for when `memory="tiny"`
+    TINY_THRESHOLD = 100
+
     def __init__(
         self,
         function: Function,
         evals: int,
         tot_iters: int,
         bounds: Optional[Sequence[tuple[float, float]]] = None,
         cv_iters: Optional[Union[list[int], int, str]] = None,
         cv_means: Union[float, Sequence[float]] = 1,
         rng: Optional[RandomState] = None,
+        memory: str = "medium",
     ):
         """
         Takes in a Function class object from functions.py. One can make their own using
         the make_func function found in that file.
 
         Parameters:
         f - Function class with f to integrate.
@@ -143,15 +147,23 @@
                 - 'all%n+b': Use every iteration (shifted by b) mod n. For example, if
                     tot_iters=10 and cv_iters='all%2+1', then use [1, 3, 5, 7, 9]
         cv_means (default 1) - The value of E[g_i] but by the scheme laid out in
             `get_is_cv_values` to obtain the control variate, E[g_i] should be
             approximately one.
         rng (default None) - The Numpy Randomstate to use. If None, will create a new
             one.
+        memory (default 'medium') - Either 'low', 'medium', 'large' or `max. Determines
+            what is saved. If `max`, save everything. If `large, don't save self.xs
+            and self.is_jac. If 'medium', additionally don't save self.weight_value and
+            self.weight_prime. If 'tiny', remove everything below the threshold
+            TINY_TRESHOLD.
         """
+        # Initialize private attributes for the properties
+        self._init_results()
+
         self.function = function
         self.bounds = self.function.dim * [[0, 1]] if bounds is None else bounds
         self.neval = evals
         self.nitn = tot_iters
 
         self.cv_nitn = cv_iters
         # Create empty list if not specified, i.e. no control variates
@@ -180,14 +192,21 @@
         self.num_cvs = len(self.cv_nitn)
         self.cv_means = cv_means
         # A number implies a constant mean value
         if isinstance(self.cv_means, Number):
             self.cv_means = self.num_cvs * [cv_means]
 
         self.rng = RandomState() if rng is None else rng
+        self.memory = memory
+
+    def _init_results(self):
+        """Initializes the private attributes for the listed properties."""
+        for name, obj in self.__class__.__dict__.items():
+            if isinstance(obj, property):
+                self.__setattr__(f"_{name}", np.nan)
 
     @timing(active=TIMING)
     def create_maps(self, map_neval: Optional[int] = None) -> None:
         """
         Creates the maps corresponding to the adapted function, f, and the
         control variates, g_i.
 
@@ -241,30 +260,34 @@
         """
         self.jac_neval = self.neval * self.nitn if jac_neval is None else jac_neval
 
         # Uniformly distributed unit hypercube
         ys = self.rng.uniform(0, 1, (self.jac_neval, self.function.dim))
         # Find the Jacobian. If by importance sampling we transform f -> f/p, then
         # the Jacobian is 1/p
-        self.xs = np.empty(ys.shape, float)
+        xs = np.empty(ys.shape, float)
         is_jac = np.empty(ys.shape[0], float)
-        self._is_map.map(ys, self.xs, is_jac)
-
+        self._is_map.map(ys, xs, is_jac)
         # The IS values
-        self.weight_value = is_jac * self.function._f(self.xs)
+        self.weight_value = is_jac * self.function._f(xs)
 
         # Find the Jacobian(s) for the CV(s)
-        self.cv_values = []
+        self.cv_values, self.cv_jacs = [], []
         for cv_map in self._cv_maps:
             # Use inverse map for control variate to find CV Jacobian
-            t_inv = np.empty(self.xs.shape, float)
-            cv_jac = np.empty(self.xs.shape[0], float)
-            cv_map.invmap(self.xs, t_inv, cv_jac)
+            t_inv = np.empty(xs.shape, float)
+            cv_jac = np.empty(xs.shape[0], float)
+            cv_map.invmap(xs, t_inv, cv_jac)
 
             self.cv_values.append(is_jac / cv_jac)
+            self.cv_jacs.append(cv_jac)
+
+        if self.memory == "max":
+            self.xs = xs
+            self.is_jac = is_jac
 
     @timing(active=TIMING)
     def get_weight_prime(self, constant: bool = True) -> None:
         """
         Calculates the final CV function by finding the optimal coefficients
         for the control variates.
 
@@ -353,15 +376,15 @@
         ) / (self.jac_neval - 1) ** 2
         return cov
 
     def integrate(
         self,
         map_neval: Optional[int] = None,
         jac_neval: Optional[int] = None,
-        constant: bool = False,
+        constant: bool = True,
     ) -> None:
         """
         Runs the necessary functions to integrate the function in the order:
             1) self.create_maps
             2) self.get_is_cv_values
             3) self.get_weight_primes
         Check out the docstrings of these functions for more info on them.
@@ -369,71 +392,113 @@
         Parameters:
         map_neval (default None) - From self.create_maps docstring: The number of
             evaluations per iteration as the maps are being created. Defaults to
             `self.neval`.
         jac_neval (default None) - From self.get_is_cv_values docstring: The number of
             steps to split up `ys`, the unit hypercube, into. Defaults to
             `self.tot_neval`, the total number of iterations used when adapting the map.
-        constant (default False) - From self.get_weight_primes: Since the ith value of a
+        constant (default True) - From self.get_weight_primes: Since the ith value of a
             control variate can be slightly correlated to its coefficient, we can remove
             said value to calculate the variance/covariance (and therefore the
             coefficient). Thus we can have different values (albeit similar ones) for
             each value. This is so if `constant=True`. If `constant=False`, just do a
             single coefficient per CV.
         """
         self.create_maps(map_neval=map_neval)
         self.get_is_cv_values(jac_neval=jac_neval)
         if self.cv_values:
             # only run if we are using control variates
             self.get_weight_prime(constant=constant)
+        self.garbage_collect()
+
+    def garbage_collect(self, memory: Optional[str] = None) -> None:
+        """
+        Deletes attributes depending on choices of self.memory to clear up memory.
+
+        Parameters:
+        memory (default None) - A measure of how many attributes to delete to clear up
+            memory. Can be 'max', 'large', 'medium' or 'tiny'. More info in the class
+            __init__ docstring.
+        """
+        memory = memory or self.memory
+
+        # Initialize properties so result is saved before deleting arrays they need
+        self.stdev
+        self.mean
+        self.w_stdev
+        self.w_mean
+
+        # Large arrays not used in anything
+        if memory in {"large", "medium", "tiny"}:
+            self._delete("xs", "is_jac")
+        # Large arrays but used in properties below
+        if memory in {"medium", "tiny"}:
+            self._delete("weight_prime", "weight_value")
+        # All bigger than a certain threshold
+        if memory == "tiny":
+            attr_items = list(self.__dict__.items())
+            for attr, attr_val in attr_items:
+                if getsizeof(attr_val) > self.TINY_THRESHOLD:
+                    self.__delattr__(attr)
+
+    def _delete(self, *attrs):
+        """Delete attribute if it still exists as one."""
+        for attr in attrs:
+            if attr in self.__dir__():
+                self.__delattr__(attr)
 
     @property
-    @check_value
+    @check_attrs("weight_prime", "jac_neval")
     def stdev(self) -> float:
         """Standard deviation of CV function"""
-        return np.std(self.weight_prime) / np.sqrt(self.jac_neval)
+        self._stdev = np.std(self.weight_prime) / np.sqrt(self.jac_neval)
+        return self._stdev
 
     @property
-    @check_value
+    @check_attrs("weight_value", "jac_neval")
     def w_stdev(self) -> float:
         """Standard deviation of IS function"""
-        return np.std(self.weight_value) / np.sqrt(self.jac_neval)
+        self._w_stdev = np.std(self.weight_value) / np.sqrt(self.jac_neval)
+        return self._w_stdev
 
     @property
-    @check_value
+    @check_attrs("stdev")
     def var(self) -> float:
         """Variance of CV function"""
-        return self.stdev**2
+        self._var = self.stdev**2
+        return self._var
 
     @property
-    @check_value
     def w_var(self) -> float:
         """Variance of IS function"""
-        return self.w_stdev**2
+        self._w_var = self.w_stdev**2
+        return self._w_var
 
     @property
-    @check_value
+    @check_attrs("weight_prime")
     def mean(self) -> float:
         """Mean of CV function"""
-        return np.mean(self.weight_prime)
+        self._mean = np.mean(self.weight_prime)
+        return self._mean
 
     @property
-    @check_value
+    @check_attrs("weight_value")
     def w_mean(self) -> float:
         """Mean of IS function"""
-        return np.mean(self.weight_value)
+        self._w_mean = np.mean(self.weight_value)
+        return self._w_mean
 
     @property
-    @check_value
     def vpr(self) -> float:
         """
         Variance percentage reduction, i.e. by what percent was the variance
         reduced due to the CVs.
         """
-        return 1 - self.var / self.w_var
+        self._vpr = 1 - self.var / self.w_var
+        return self._vpr
 
     def compare(
         self, rounding: int = 3, cutoff: Union[int, tuple[int, int]] = 3
     ) -> None:
         """
         Print out mean, variance and standard deviation for without and with the CVs.
```

### Comparing `control-vegas-1.1.0/src/control_vegas/utilities.py` & `control-vegas-1.2.0/src/control_vegas/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,45 +9,50 @@
 
 from ._exceptions import ParameterBoundError
 
 
 def timing(active: bool = True):
     """Decorator for timing with option to turn it off"""
 
-    def decorator(f):
-        def wrapper(*args, **kwargs):
+    def decorator(func):
+        def wrapper(inst, *args, **kwargs):
             if active:
                 dt0 = dt.now()
-                output = f(*args, **kwargs)
+                output = func(*args, **kwargs)
                 dt1 = dt.now()
                 tot_time = (dt1 - dt0).total_seconds()
-                print(f"{f.__name__}: {tot_time:>{30 - len(f.__name__)}.3f}s")
+                print(f"{func.__name__}: {tot_time:>{30 - len(func.__name__)}.3f}s")
             else:
-                output = f(*args, **kwargs)
+                output = func(inst, *args, **kwargs)
 
             return output
 
         return wrapper
 
     return decorator
 
 
-def check_value(f):
+def check_attrs(*attrs):
     """
-    Decorator to return nan if there is no value otherwise. Used for the properties
-    of CVIntegrator being passed as numbers, e.g. in self.compare.
+    Decorator that checks if the class instance has the attributes in `attrs`.
+    If it doesn't, return the value as is rather than calculate it. So properties
+    can "cache" their values if the largest arrays they rely on are deleted.
     """
 
-    def wrapper(*args, **kwargs):
-        try:
-            return f(*args, **kwargs)
-        except AttributeError:
-            return np.nan
+    def decorator(func):
+        def wrapper(inst, *args, **kwargs):
+            for attr in attrs:
+                if not hasattr(inst, attr):
+                    # get hidden attribute name (has an underscore in the front)
+                    return inst.__getattribute__(f"_{func.__name__}")
+            return func(inst, *args, **kwargs)
 
-    return wrapper
+        return wrapper
+
+    return decorator
 
 
 def save(
     name: str,
     savedir: str = "",
     savepath: str = "",
     stype: str = "npz",
```

### Comparing `control-vegas-1.1.0/src/control_vegas.egg-info/PKG-INFO` & `control-vegas-1.2.0/src/control_vegas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-vegas
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Control Variate wrapper over the vegas python package.
 Author-email: Jacob Scott <jscott137@pm.me>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -717,17 +717,17 @@
 where the $*$ represents the optimal value. Plugging in $c^\*$ gives us a final variance of
 $$\text{Var}(f_c^\*)=\text{Var}(f)-\frac{\text{Cov}^2(f,g)}{\text{Var}(g)}=\left(1-\rho^2(f,g)\right)\text{Var}(f)\qquad\text{where}\qquad\rho(f,g)=\frac{\text{Cov}(f,g)}{\sqrt{\text{Var}(f)\text{Var}(g)}}$$
 is the correlation coefficient between $f$ and $g$. Since $|\rho(f,g)|\le1$, then this choice of $c$ will always decrease the variance. The same prescription can be applied for $n$ control variates, rather than just one, which is used in this package.
 
 A control variate is applied by using `vegas`'s importance sampling adaptation. Since $\rho$ is larger when the functions have a linear relationship, we use these previously adapted maps as the control variates. One can specify using the $i$th iteration of `vegas` as the control variate when initializing the `CVIntegrator` class or specify a list of iterations to use for multiple control variates.
 
 ## Installation
-To install, `numpy` and `cython` must be installed beforehand due to the `gvar` package. Therefore, for `pip`:
+It can just be installed via `pip`:
 ```
-python -m pip install numpy Cython && python -m pip install control-vegas
+python -m pip install control-vegas
 ```
 
 ## Usage
 The workflow involes creating a `Function` class and then passing that to the `CVIntegrator`. The `Function` class contains the function to be integrated but also other information such as its name, the true value of the integration (if available) and parameters of the function. The `CVIntegrator` class does the integration and stores the results like mean and variance.
 
 ### Using a Built-In Function
 For example,
@@ -770,38 +770,72 @@
     return self.a * x[:, 0]**2 + self.b * x[:, 1]
 
 # Creating class with name 'WeightedPoly' and assigning values to the parameters in the function
 wpoly = make_func('WeightedPoly', dimension=2, function=f, name='Weighted Polynomial', a=0.3, b=0.6)
 # Print out parameters of class (note `true_value` isn't shown)
 print(wpoly, '\n')
 
-# Create integrator class and use the 20th iteration as the control  variate
-cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=20)
+# Create integrator class and use multiple control variates
+cvi = CVIntegrator(wpoly, evals=1000, tot_iters=50, cv_iters=[10, 15, 20, 25, 30, 35])
 # Run the integration
 cvi.integrate()
 
 # Print info
 cvi.compare(rounding=5)
 ```
 which outputs
 ```
-WeightedPoly(dimension=2, name=WeightedPoly, a=0.3, b=0.6) 
+WeightedPoly(dimension=2, name=Weighted Polynomial, a=0.3, b=0.6) 
 
-         |     No CVs     |    With CVs    
----------+----------------+----------------
-Mean     |     0.39996303 |     0.39993278
-Variance | 5.27324871e-09 | 4.86145624e-09
-St Dev   | 7.26171379e-05 | 6.97241439e-05
-VPR      |                |    7.80908493%
+         |   No CVs    |  With CVs   
+---------+-------------+-------------
+Mean     |     0.39984 |     0.40004
+Variance | 5.83781e-08 | 4.90241e-08
+St Dev   | 2.41616e-04 | 2.21414e-04
+VPR      |             |   16.02309%
 ```
 The reason the function is vectorized is because, on the backend, `vegas`'s `batchintegrand` is used which can greatly speed up the computation.
 
+### Be lazy!
+If you're rushed or lazy, you can use the `quick_integrate` function that does the steps above for you and returns the `CVIntegrator` object. So to run the previous code block, you would use
+```python
+cvi = quick_integrate(
+         function=f,
+         evals=1000,
+         tot_iters=50,
+         bounds=[(0, 1), (0, 1)],
+         cv_iters=20,
+         cname="WeightPoly",
+         name="Weighted Polynomial",
+         a=0.3, b=0.6
+)
+cvi.compare()
+```
+which outputs
+```
+         |  No CVs   | With CVs  
+---------+-----------+-----------
+Mean     |     0.400 |     0.400
+Variance | 5.826e-08 | 5.025e-08
+St Dev   | 2.414e-04 | 2.242e-04
+VPR      |           |   13.746%
+```
+Note that the arguments are `cname` and `name` are optional but `bounds` is not. The dimension of the integral is implied from `bounds` when using `quick_integrate` whereas it's taken from the `Function` class for the previous code blocks.
+
+### Specifying Control Variate Iterations
+There are multiple valid arguments that can be passed to `cv_iters` for both the `CVIntegrator` class and `quick_integrate` which we'll lay out here.
+- For using one control variate, pass a integer representing the iteration to use.
+- For multiple control variates, pass a list of integers representing the iterations to use.
+- The string 'all' will use every iteration.
+- The string `all%n` will use every iteration mod $n$. So if you specify `tot_iters=15` and `cv_iters='all%3'`, then then the iterations used will be `[3, 6, 9, 12]`
+- This can be shifted by instead using `all%n+b` where $b$ is the shift. So for `tot_iters=15` and `cv_iters='all%3+2'`, you'll get `[2, 5, 8, 11, 14]`.
+
 ### Manual Use of `Function` Class
 To access the function call, use `function` or `f`. So, using the second example, I can run
 ```python
 wpoly.f([1.2, 1.5]) # returns 1.3319999999999999
 wpoly.f([0.2, 1], [0.8, 0.8], [1, 2]) # returns array([0.612, 0.672, 1.5  ])
 ```
 This wraps around the private, vectorized `_function`/`_f` used by `vegas` so you don't have to worry about the proper `numpy` array shape
 
 ## Notes
-- By default, functions are integrated from 0 to 1.
+- By default, functions are integrated from 0 to 1 unless `quick_integrate` is used.
```

