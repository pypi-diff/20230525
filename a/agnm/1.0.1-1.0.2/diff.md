# Comparing `tmp/agnm-1.0.1.tar.gz` & `tmp/agnm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agnm-1.0.1.tar", last modified: Sun Apr 23 18:54:23 2023, max compression
+gzip compressed data, was "agnm-1.0.2.tar", last modified: Thu May 25 14:21:11 2023, max compression
```

## Comparing `agnm-1.0.1.tar` & `agnm-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.083951 agnm-1.0.1/
--rw-rw-rw-   0        0        0     1080 2023-04-17 16:38:53.000000 agnm-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2062 2023-04-23 18:54:23.081920 agnm-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1662 2023-04-23 18:53:52.000000 agnm-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.067635 agnm-1.0.1/agnm/
--rw-rw-rw-   0        0        0        0 2023-04-23 18:51:59.000000 agnm-1.0.1/agnm/__init__.py
--rw-rw-rw-   0        0        0     2603 2023-04-23 18:51:59.000000 agnm-1.0.1/agnm/motion.py
-drwxrwxrwx   0        0        0        0 2023-04-23 18:54:23.079957 agnm-1.0.1/agnm.egg-info/
--rw-rw-rw-   0        0        0     2062 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-23 18:54:23.000000 agnm-1.0.1/agnm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2023-04-23 18:53:52.000000 agnm-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 18:54:23.084922 agnm-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:21:11.479442 agnm-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-25 14:21:00.000000 agnm-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:21:11.479442 agnm-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-25 14:21:00.000000 agnm-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:21:11.479442 agnm-1.0.2/agnm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:21:00.000000 agnm-1.0.2/agnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-05-25 14:21:00.000000 agnm-1.0.2/agnm/motion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:21:11.479442 agnm-1.0.2/agnm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-25 14:21:11.000000 agnm-1.0.2/agnm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-25 14:21:11.000000 agnm-1.0.2/agnm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:21:11.000000 agnm-1.0.2/agnm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-25 14:21:11.000000 agnm-1.0.2/agnm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-25 14:21:00.000000 agnm-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:21:11.479442 agnm-1.0.2/setup.cfg
```

### Comparing `agnm-1.0.1/PKG-INFO` & `agnm-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: agnm
-Version: 1.0.1
-Summary: A package for physics motion calculations
-Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Physics equations of motion solver
-This is a package for physics motion calculations.
-
-# Installation
-```pip install agnm```
-
-# Usage
-### Displacement
-Displacement is calculated using formula: 
-```math
-x = (vi-vf)/2*t 
-```
-
-```python
-from agnm.motion import displacement
-
-displacement(1, 2.3, 3)  # output: 2.65
-# or use named variables
-displacement(vf=2.3, t=1, vi=3)  # output: 2.65
-```
-
-### Change in position
-Change in position is calculated using formula: 
-```math
-x = vi*t+1/2*a*t^2
-```
-
-```python
-from agnm.motion import change_in_position
-
-change_in_position(1, 3, 2)  # output: 12.0
-# or use named variables
-change_in_position(a=2, t=3, vi=1)  # output: 12.0
-```
-
-### Final velocity
-Final velocity is calculated using one of formulas: 
-```math
-vf = (vi^2+2a*x)^1/2
-vf = vi+a*t
-```
-
-```python
-from agnm.motion import v_final
-
-# using first equation
-v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
-# using second equation
-v_final(vi=1, a=2.3, t=2)  # output: 5.6
-```
-
-### Average velocity
-Average velocity is calculated using one of formulas: 
-```math
-va = x/t
-va = (vi+vf)/2
-```
-
-```python
-from agnm.motion import v_average
-
-# using first equation
-v_average(x_delta=1, t=3)  #output: 0.3333333333333333
-# using second equation
-v_average(vi=1, vf=2.6)  #output: 0.8
-```
-
-### Acceleration
-Acceleration velocity is calculated using one of formulas: 
-```math
-a = v/t
-a = (vf+vi)/t
-```
-
-```python
-from agnm.motion import acceleration
-
-# using first equation
-acceleration(v_delta=5, t=2.5)
-#output: 2.0
-# using second equation
-acceleration(vi=1, vf=6, t=2.5)
-#output: 2.0
-```
+Metadata-Version: 2.1
+Name: agnm
+Version: 1.0.2
+Summary: A package for physics motion calculations
+Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Physics equations of motion solver
+This is a package for physics motion calculations.
+
+# Installation
+```pip install agnm```
+
+# Usage
+### Displacement
+Displacement is calculated using formula: 
+```math
+x = (vi-vf)/2*t 
+```
+
+```python
+from agnm.motion import displacement
+
+displacement(1, 2.3, 3)  # output: 2.65
+# or use named variables
+displacement(vf=2.3, t=1, vi=3)  # output: 2.65
+```
+
+### Change in position
+Change in position is calculated using formula: 
+```math
+x = vi*t+1/2*a*t^2
+```
+
+```python
+from agnm.motion import change_in_position
+
+change_in_position(1, 3, 2)  # output: 12.0
+# or use named variables
+change_in_position(a=2, t=3, vi=1)  # output: 12.0
+```
+
+### Final velocity
+Final velocity is calculated using one of formulas: 
+```math
+vf = (vi^2+2a*x)^1/2
+vf = vi+a*t
+```
+
+```python
+from agnm.motion import v_final
+
+# using first equation
+v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
+# using second equation
+v_final(vi=1, a=2.3, t=2)  # output: 5.6
+```
+
+### Average velocity
+Average velocity is calculated using one of formulas: 
+```math
+va = x/t
+va = (vi+vf)/2
+```
+
+```python
+from agnm.motion import v_average
+
+# using first equation
+v_average(x_delta=1, t=3)  #output: 0.3333333333333333
+# using second equation
+v_average(vi=1, vf=2.6)  #output: 0.8
+```
+
+### Acceleration
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+
+```python
+from agnm.motion import acceleration
+
+# using first equation
+acceleration(v_delta=5, t=2.5)
+#output: 2.0
+# using second equation
+acceleration(vi=1, vf=6, t=2.5)
+#output: 2.0
+```
```

### Comparing `agnm-1.0.1/README.md` & `agnm-1.0.2/README.md`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# Physics equations of motion solver
-This is a package for physics motion calculations.
-
-# Installation
-```pip install agnm```
-
-# Usage
-### Displacement
-Displacement is calculated using formula: 
-```math
-x = (vi-vf)/2*t 
-```
-
-```python
-from agnm.motion import displacement
-
-displacement(1, 2.3, 3)  # output: 2.65
-# or use named variables
-displacement(vf=2.3, t=1, vi=3)  # output: 2.65
-```
-
-### Change in position
-Change in position is calculated using formula: 
-```math
-x = vi*t+1/2*a*t^2
-```
-
-```python
-from agnm.motion import change_in_position
-
-change_in_position(1, 3, 2)  # output: 12.0
-# or use named variables
-change_in_position(a=2, t=3, vi=1)  # output: 12.0
-```
-
-### Final velocity
-Final velocity is calculated using one of formulas: 
-```math
-vf = (vi^2+2a*x)^1/2
-vf = vi+a*t
-```
-
-```python
-from agnm.motion import v_final
-
-# using first equation
-v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
-# using second equation
-v_final(vi=1, a=2.3, t=2)  # output: 5.6
-```
-
-### Average velocity
-Average velocity is calculated using one of formulas: 
-```math
-va = x/t
-va = (vi+vf)/2
-```
-
-```python
-from agnm.motion import v_average
-
-# using first equation
-v_average(x_delta=1, t=3)  #output: 0.3333333333333333
-# using second equation
-v_average(vi=1, vf=2.6)  #output: 0.8
-```
-
-### Acceleration
-Acceleration velocity is calculated using one of formulas: 
-```math
-a = v/t
-a = (vf+vi)/t
-```
-
-```python
-from agnm.motion import acceleration
-
-# using first equation
-acceleration(v_delta=5, t=2.5)
-#output: 2.0
-# using second equation
-acceleration(vi=1, vf=6, t=2.5)
-#output: 2.0
+# Physics equations of motion solver
+This is a package for physics motion calculations.
+
+# Installation
+```pip install agnm```
+
+# Usage
+### Displacement
+Displacement is calculated using formula: 
+```math
+x = (vi-vf)/2*t 
+```
+
+```python
+from agnm.motion import displacement
+
+displacement(1, 2.3, 3)  # output: 2.65
+# or use named variables
+displacement(vf=2.3, t=1, vi=3)  # output: 2.65
+```
+
+### Change in position
+Change in position is calculated using formula: 
+```math
+x = vi*t+1/2*a*t^2
+```
+
+```python
+from agnm.motion import change_in_position
+
+change_in_position(1, 3, 2)  # output: 12.0
+# or use named variables
+change_in_position(a=2, t=3, vi=1)  # output: 12.0
+```
+
+### Final velocity
+Final velocity is calculated using one of formulas: 
+```math
+vf = (vi^2+2a*x)^1/2
+vf = vi+a*t
+```
+
+```python
+from agnm.motion import v_final
+
+# using first equation
+v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
+# using second equation
+v_final(vi=1, a=2.3, t=2)  # output: 5.6
+```
+
+### Average velocity
+Average velocity is calculated using one of formulas: 
+```math
+va = x/t
+va = (vi+vf)/2
+```
+
+```python
+from agnm.motion import v_average
+
+# using first equation
+v_average(x_delta=1, t=3)  #output: 0.3333333333333333
+# using second equation
+v_average(vi=1, vf=2.6)  #output: 0.8
+```
+
+### Acceleration
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+
+```python
+from agnm.motion import acceleration
+
+# using first equation
+acceleration(v_delta=5, t=2.5)
+#output: 2.0
+# using second equation
+acceleration(vi=1, vf=6, t=2.5)
+#output: 2.0
 ```
```

### Comparing `agnm-1.0.1/agnm/motion.py` & `agnm-1.0.2/agnm/motion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import math
-
-
-def acceleration(v_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
-    """
-    Method, that calculates acceleration, using function, based on passed parameters
-    a = v/t
-    a = (vf+vi)/t
-
-    :param v_delta: change in velocity (m/s)
-    :param t: time (s)
-    :param vf: final velocity (m/s)
-    :param vi: initial velocity (m/s)
-    :return: acceleration value or infinity if none of the passed arguments combinations match described functions
-    """
-    if v_delta != math.inf and t != math.inf:
-        return v_delta / t
-    elif vi != math.inf and vf != math.inf and t != math.inf:
-        return (vf - vi) / t
-    else:
-        return math.inf
-
-
-def v_average(x_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
-    """
-    Method, that calculates average velocity, using function, based on passed parameters
-    va = x/t
-    va = (vi+vf)/2
-
-    :param x_delta: change in position (m)
-    :param t: time (s)
-    :param vf: final velocity (m/s)
-    :param vi: initial velocity (m/s)
-    :return: average velocity value or infinity if none of the passed arguments combinations match described functions
-    """
-    if x_delta != math.inf and t != math.inf:
-        return x_delta / t
-    elif vi != math.inf and vf != math.inf:
-        return (vf - vi) / 2
-    else:
-        return math.inf
-
-
-def v_final(vi, a, t=math.inf, x_delta=math.inf):
-    """
-    Method, that calculates final velocity, using function, based on passed parameters
-    vf = (vi^2+2a*x)^1/2
-    vf = vi+a*t
-
-    :param vi: initial velocity (m/s)
-    :param a: acceleration (m/s^2)
-    :param t: time (s)
-    :param x_delta: change in position (m)
-    :return: final velocity value or infinity if none of the passed arguments combinations match described functions
-    """
-    if not vi or not a:
-        return math.inf
-
-    if t != math.inf:
-        return vi + a * t
-
-    if x_delta != math.inf:
-        return vi ** 2 + 2 * a * x_delta
-
-    return math.inf
-
-
-def change_in_position(vi, t, a):
-    """
-    Method, that calculates change in position
-    x = vi*t+1/2*a*t^2
-
-    :param vi: initial velocity (m/s)
-    :param t: time (s)
-    :param a: acceleration (m/s^2)
-    :return: change in position value
-    """
-    return vi * t + 0.5 * a * (t ** 2)
-
-
-def displacement(t, vf, vi):
-    """
-    Method, that calculates displacement
-    x = (vi-vf)/2*t
-
-    :param t: time (s)
-    :param vf: final velocity (m/s)
-    :param vi: initial velocity (m/s)
-    :return:
-    """
-    return 0.5 * (vi + vf) * t
+import math
+
+
+def acceleration(v_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
+    """
+    Method, that calculates acceleration, using function, based on passed parameters
+    a = v/t
+    a = (vf+vi)/t
+
+    :param v_delta: change in velocity (m/s)
+    :param t: time (s)
+    :param vf: final velocity (m/s)
+    :param vi: initial velocity (m/s)
+    :return: acceleration value or infinity if none of the passed arguments combinations match described functions
+    """
+    if v_delta != math.inf and t != math.inf:
+        return v_delta / t
+    elif vi != math.inf and vf != math.inf and t != math.inf:
+        return (vf - vi) / t
+    else:
+        return math.inf
+
+
+def v_average(x_delta=math.inf, t=math.inf, vf=math.inf, vi=math.inf):
+    """
+    Method, that calculates average velocity, using function, based on passed parameters
+    va = x/t
+    va = (vi+vf)/2
+
+    :param x_delta: change in position (m)
+    :param t: time (s)
+    :param vf: final velocity (m/s)
+    :param vi: initial velocity (m/s)
+    :return: average velocity value or infinity if none of the passed arguments combinations match described functions
+    """
+    if x_delta != math.inf and t != math.inf:
+        return x_delta / t
+    elif vi != math.inf and vf != math.inf:
+        return (vf - vi) / 2
+    else:
+        return math.inf
+
+
+def v_final(vi, a, t=math.inf, x_delta=math.inf):
+    """
+    Method, that calculates final velocity, using function, based on passed parameters
+    vf = (vi^2+2a*x)^1/2
+    vf = vi+a*t
+
+    :param vi: initial velocity (m/s)
+    :param a: acceleration (m/s^2)
+    :param t: time (s)
+    :param x_delta: change in position (m)
+    :return: final velocity value or infinity if none of the passed arguments combinations match described functions
+    """
+    if not vi or not a:
+        return math.inf
+
+    if t != math.inf:
+        return vi + a * t
+
+    if x_delta != math.inf:
+        return vi ** 2 + 2 * a * x_delta
+
+    return math.inf
+
+
+def change_in_position(vi, t, a):
+    """
+    Method, that calculates change in position
+    x = vi*t+1/2*a*t^2
+
+    :param vi: initial velocity (m/s)
+    :param t: time (s)
+    :param a: acceleration (m/s^2)
+    :return: change in position value
+    """
+    return vi * t + 0.5 * a * (t ** 2)
+
+
+def displacement(t, vf, vi):
+    """
+    Method, that calculates displacement
+    x = (vi-vf)/2*t
+
+    :param t: time (s)
+    :param vf: final velocity (m/s)
+    :param vi: initial velocity (m/s)
+    :return: displacement value
+    """
+    return 0.5 * (vi + vf) * t
```

### Comparing `agnm-1.0.1/agnm.egg-info/PKG-INFO` & `agnm-1.0.2/agnm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-Metadata-Version: 2.1
-Name: agnm
-Version: 1.0.1
-Summary: A package for physics motion calculations
-Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# Physics equations of motion solver
-This is a package for physics motion calculations.
-
-# Installation
-```pip install agnm```
-
-# Usage
-### Displacement
-Displacement is calculated using formula: 
-```math
-x = (vi-vf)/2*t 
-```
-
-```python
-from agnm.motion import displacement
-
-displacement(1, 2.3, 3)  # output: 2.65
-# or use named variables
-displacement(vf=2.3, t=1, vi=3)  # output: 2.65
-```
-
-### Change in position
-Change in position is calculated using formula: 
-```math
-x = vi*t+1/2*a*t^2
-```
-
-```python
-from agnm.motion import change_in_position
-
-change_in_position(1, 3, 2)  # output: 12.0
-# or use named variables
-change_in_position(a=2, t=3, vi=1)  # output: 12.0
-```
-
-### Final velocity
-Final velocity is calculated using one of formulas: 
-```math
-vf = (vi^2+2a*x)^1/2
-vf = vi+a*t
-```
-
-```python
-from agnm.motion import v_final
-
-# using first equation
-v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
-# using second equation
-v_final(vi=1, a=2.3, t=2)  # output: 5.6
-```
-
-### Average velocity
-Average velocity is calculated using one of formulas: 
-```math
-va = x/t
-va = (vi+vf)/2
-```
-
-```python
-from agnm.motion import v_average
-
-# using first equation
-v_average(x_delta=1, t=3)  #output: 0.3333333333333333
-# using second equation
-v_average(vi=1, vf=2.6)  #output: 0.8
-```
-
-### Acceleration
-Acceleration velocity is calculated using one of formulas: 
-```math
-a = v/t
-a = (vf+vi)/t
-```
-
-```python
-from agnm.motion import acceleration
-
-# using first equation
-acceleration(v_delta=5, t=2.5)
-#output: 2.0
-# using second equation
-acceleration(vi=1, vf=6, t=2.5)
-#output: 2.0
-```
+Metadata-Version: 2.1
+Name: agnm
+Version: 1.0.2
+Summary: A package for physics motion calculations
+Author-email: Agnė Moleikaitytė <agnmol@ktu.lt>
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Physics equations of motion solver
+This is a package for physics motion calculations.
+
+# Installation
+```pip install agnm```
+
+# Usage
+### Displacement
+Displacement is calculated using formula: 
+```math
+x = (vi-vf)/2*t 
+```
+
+```python
+from agnm.motion import displacement
+
+displacement(1, 2.3, 3)  # output: 2.65
+# or use named variables
+displacement(vf=2.3, t=1, vi=3)  # output: 2.65
+```
+
+### Change in position
+Change in position is calculated using formula: 
+```math
+x = vi*t+1/2*a*t^2
+```
+
+```python
+from agnm.motion import change_in_position
+
+change_in_position(1, 3, 2)  # output: 12.0
+# or use named variables
+change_in_position(a=2, t=3, vi=1)  # output: 12.0
+```
+
+### Final velocity
+Final velocity is calculated using one of formulas: 
+```math
+vf = (vi^2+2a*x)^1/2
+vf = vi+a*t
+```
+
+```python
+from agnm.motion import v_final
+
+# using first equation
+v_final(vi=1, a=3, x_delta=1.5)  # output: 10.0
+# using second equation
+v_final(vi=1, a=2.3, t=2)  # output: 5.6
+```
+
+### Average velocity
+Average velocity is calculated using one of formulas: 
+```math
+va = x/t
+va = (vi+vf)/2
+```
+
+```python
+from agnm.motion import v_average
+
+# using first equation
+v_average(x_delta=1, t=3)  #output: 0.3333333333333333
+# using second equation
+v_average(vi=1, vf=2.6)  #output: 0.8
+```
+
+### Acceleration
+Acceleration velocity is calculated using one of formulas: 
+```math
+a = v/t
+a = (vf+vi)/t
+```
+
+```python
+from agnm.motion import acceleration
+
+# using first equation
+acceleration(v_delta=5, t=2.5)
+#output: 2.0
+# using second equation
+acceleration(vi=1, vf=6, t=2.5)
+#output: 2.0
+```
```

