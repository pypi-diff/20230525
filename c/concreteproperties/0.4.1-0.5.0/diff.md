# Comparing `tmp/concreteproperties-0.4.1.tar.gz` & `tmp/concreteproperties-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concreteproperties-0.4.1.tar", last modified: Mon Nov 28 02:43:44 2022, max compression
+gzip compressed data, was "concreteproperties-0.5.0.tar", last modified: Tue Dec 20 09:18:04 2022, max compression
```

## Comparing `concreteproperties-0.4.1.tar` & `concreteproperties-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     5741 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4575 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/concreteproperties/
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22829 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/analysis_section.py
--rw-r--r--   0 runner    (1001) docker     (122)    80111 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/concrete_section.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/concreteproperties/design_codes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/design_codes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21419 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/design_codes/as3600.py
--rw-r--r--   0 runner    (1001) docker     (122)     6633 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/design_codes/design_code.py
--rw-r--r--   0 runner    (1001) docker     (122)     3351 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/material.py
--rw-r--r--   0 runner    (1001) docker     (122)     3048 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/post.py
--rw-r--r--   0 runner    (1001) docker     (122)    14713 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/pre.py
--rw-r--r--   0 runner    (1001) docker     (122)    49893 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/results.py
--rw-r--r--   0 runner    (1001) docker     (122)    22820 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/stress_strain_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/concreteproperties/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_gross_properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     8411 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_moment_interaction.py
--rw-r--r--   0 runner    (1001) docker     (122)    12982 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_reinforced_concrete_basics.py
--rw-r--r--   0 runner    (1001) docker     (122)     7633 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_rotation.py
--rw-r--r--   0 runner    (1001) docker     (122)     5737 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_stress_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/tests/test_stress_strain_profile.py
--rw-r--r--   0 runner    (1001) docker     (122)    13991 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/concreteproperties/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/concreteproperties.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5741 2022-11-28 02:43:44.000000 concreteproperties-0.4.1/concreteproperties.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2022-11-28 02:43:44.000000 concreteproperties-0.4.1/concreteproperties.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 02:43:44.000000 concreteproperties-0.4.1/concreteproperties.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      206 2022-11-28 02:43:44.000000 concreteproperties-0.4.1/concreteproperties.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-28 02:43:44.000000 concreteproperties-0.4.1/concreteproperties.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1584 2022-11-28 02:43:44.133462 concreteproperties-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       69 2022-11-28 02:43:33.000000 concreteproperties-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/concreteproperties/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22984 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/analysis_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81092 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/concrete_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/concreteproperties/design_codes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/design_codes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21688 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/design_codes/as3600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/design_codes/design_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78603 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/design_codes/nzs3101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/pre.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35225 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/prestressed_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53361 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46777 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/stress_strain_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/concreteproperties/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_gross_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_moment_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44219 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_nzs3101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_prestress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_prestress_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12984 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_reinforced_concrete_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_stress_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/tests/test_stress_strain_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15930 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/concreteproperties/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/concreteproperties.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2022-12-20 09:18:04.000000 concreteproperties-0.5.0/concreteproperties.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2022-12-20 09:18:04.000000 concreteproperties-0.5.0/concreteproperties.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 09:18:04.000000 concreteproperties-0.5.0/concreteproperties.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-20 09:18:04.000000 concreteproperties-0.5.0/concreteproperties.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 09:18:04.000000 concreteproperties-0.5.0/concreteproperties.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2022-12-20 09:18:04.112963 concreteproperties-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-20 09:17:48.000000 concreteproperties-0.5.0/setup.py
```

### Comparing `concreteproperties-0.4.1/LICENSE.md` & `concreteproperties-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/PKG-INFO` & `concreteproperties-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concreteproperties
-Version: 0.4.1
+Version: 0.5.0
 Summary: A python package to determine cross-section propreties of reinforced concrete sections
 Home-page: https://github.com/robbievanleeuwen/concrete-properties
 Author: Robbie van Leeuwen
 Author-email: robbie.vanleeuwen@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/robbievanleeuwen/concrete-properties
 Project-URL: Tracker, https://github.com/robbievanleeuwen/concrete-properties/issues
@@ -39,89 +39,108 @@
 
 Here's an example of some of the non-linear output *concreteproperties* can generate:
 
 <p align="center">
   <img src="docs/source/_static/anim/anim_compress.gif" width="500"/>
 </p>
 
-## Installation:
+## Installation
 
 For more detailed installation instructions, refer to the [documentation](https://robbievanleeuwen.github.io/concrete-properties/rst/installation.html).
 
 ```shell
 pip install concreteproperties
 ```
 
-## Documentation:
+## Documentation
 
 *concreteproperties* is fully documented including examples and a fully documented API.
 The documentation can found at [https://robbievanleeuwen.github.io/concrete-properties](https://robbievanleeuwen.github.io/concrete-properties).
 
 ## Contributing
 
 We welcome anyone interested in contributing to *concreteproperties*, whether it be
 through submitting bug reports, feature requests or pull requests. Please read the
 [contributing guide](.github/CONTRIBUTING.md) prior to contributing.
 
-## Current Capabilities:
+## Current Capabilities
+
+### Analysis Types
+
+- [x] Reinforced Concrete
+- [x] Steel-Concrete Composite
+- [x] Prestressed Concrete
 
 ### Material Properties
+
 - [x] Concrete material
   - [x] Service stress-strain profiles
     - [x] Linear profile
     - [x] Linear profile (no tension)
     - [x] Eurocode non-linear
+    - [x] Modified Mander non-linear profile (confined & unconfined concrete)
   - [x] Ultimate stress-strain profiles
     - [x] Rectangular stress block
     - [x] Bilinear stress-strain profile
     - [x] Eurocode parabolic
   - [x] Flexural tensile strength
 - [x] Steel material
   - [x] Stress-strain profiles
     - [x] Elastic-plastic
     - [x] Elastic-plastic (with hardening)
+- [x] Strand material
+  - [x] Stress-strain profiles
+    - [x] Elastic-plastic (with hardening)
+    - [x] PCI journal (1992) non-linear
 
 ### Gross Section Properties
-- [x] Cross-sectional areas (total, concrete, steel)
+
+- [x] Cross-sectional areas (total, concrete, steel, strand)
 - [x] Axial rigidity
 - [x] Cross-section mass
 - [x] Cross-section perimeter
 - [x] First moments of area
 - [x] Elastic centroid
 - [x] Global second moments of area
 - [x] Centroidal second moments of area
 - [x] Principal axis angle
 - [x] Principal second moments of area
 - [x] Centroidal section moduli
 - [x] Principal section moduli
+- [x] Prestressed Aations
 
 ### Service Analysis
+
 - [x] Cracking moment
-- [x] Cracked second moment of area
+- [x] Cracked area properties
 - [x] Moment-curvature diagram
 
 ### Ultimate Analysis
+
 - [x] Ultimate bending capacity
 - [x] Squash load
 - [x] Tensile load
 - [x] Moment interaction diagrams
   - [x] M-N curves
   - [x] Biaxial bending curve
 
 ### Stress Analysis
+
 - [x] Uncracked stresses
 - [x] Cracked stresses
 - [x] Service stresses
 - [x] Ultimate stresses
 
 ### Design Codes
+
 - [x] Design code modules
   - [x] AS3600
   - [ ] AS5100
+  - [x] NZS3101 & NZSEE C5 Assessment Guidelines
 
-## Disclaimer:
+## Disclaimer
 
 *concreteproperties* is an open source engineering tool that continues to benefit from
 the collaboration of many contributors. Although efforts have been made to ensure the
 that relevant engineering theories have been correctly implemented, it remains the
 user's responsibility to confirm and accept the output. Refer to the
 [license](LICENSE.md) for clarification of the conditions of use.
```

### Comparing `concreteproperties-0.4.1/README.md` & `concreteproperties-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -11,89 +11,108 @@
 
 Here's an example of some of the non-linear output *concreteproperties* can generate:
 
 <p align="center">
   <img src="docs/source/_static/anim/anim_compress.gif" width="500"/>
 </p>
 
-## Installation:
+## Installation
 
 For more detailed installation instructions, refer to the [documentation](https://robbievanleeuwen.github.io/concrete-properties/rst/installation.html).
 
 ```shell
 pip install concreteproperties
 ```
 
-## Documentation:
+## Documentation
 
 *concreteproperties* is fully documented including examples and a fully documented API.
 The documentation can found at [https://robbievanleeuwen.github.io/concrete-properties](https://robbievanleeuwen.github.io/concrete-properties).
 
 ## Contributing
 
 We welcome anyone interested in contributing to *concreteproperties*, whether it be
 through submitting bug reports, feature requests or pull requests. Please read the
 [contributing guide](.github/CONTRIBUTING.md) prior to contributing.
 
-## Current Capabilities:
+## Current Capabilities
+
+### Analysis Types
+
+- [x] Reinforced Concrete
+- [x] Steel-Concrete Composite
+- [x] Prestressed Concrete
 
 ### Material Properties
+
 - [x] Concrete material
   - [x] Service stress-strain profiles
     - [x] Linear profile
     - [x] Linear profile (no tension)
     - [x] Eurocode non-linear
+    - [x] Modified Mander non-linear profile (confined & unconfined concrete)
   - [x] Ultimate stress-strain profiles
     - [x] Rectangular stress block
     - [x] Bilinear stress-strain profile
     - [x] Eurocode parabolic
   - [x] Flexural tensile strength
 - [x] Steel material
   - [x] Stress-strain profiles
     - [x] Elastic-plastic
     - [x] Elastic-plastic (with hardening)
+- [x] Strand material
+  - [x] Stress-strain profiles
+    - [x] Elastic-plastic (with hardening)
+    - [x] PCI journal (1992) non-linear
 
 ### Gross Section Properties
-- [x] Cross-sectional areas (total, concrete, steel)
+
+- [x] Cross-sectional areas (total, concrete, steel, strand)
 - [x] Axial rigidity
 - [x] Cross-section mass
 - [x] Cross-section perimeter
 - [x] First moments of area
 - [x] Elastic centroid
 - [x] Global second moments of area
 - [x] Centroidal second moments of area
 - [x] Principal axis angle
 - [x] Principal second moments of area
 - [x] Centroidal section moduli
 - [x] Principal section moduli
+- [x] Prestressed Aations
 
 ### Service Analysis
+
 - [x] Cracking moment
-- [x] Cracked second moment of area
+- [x] Cracked area properties
 - [x] Moment-curvature diagram
 
 ### Ultimate Analysis
+
 - [x] Ultimate bending capacity
 - [x] Squash load
 - [x] Tensile load
 - [x] Moment interaction diagrams
   - [x] M-N curves
   - [x] Biaxial bending curve
 
 ### Stress Analysis
+
 - [x] Uncracked stresses
 - [x] Cracked stresses
 - [x] Service stresses
 - [x] Ultimate stresses
 
 ### Design Codes
+
 - [x] Design code modules
   - [x] AS3600
   - [ ] AS5100
+  - [x] NZS3101 & NZSEE C5 Assessment Guidelines
 
-## Disclaimer:
+## Disclaimer
 
 *concreteproperties* is an open source engineering tool that continues to benefit from
 the collaboration of many contributors. Although efforts have been made to ensure the
 that relevant engineering theories have been correctly implemented, it remains the
 user's responsibility to confirm and accept the output. Refer to the
 [license](LICENSE.md) for clarification of the conditions of use.
```

### Comparing `concreteproperties-0.4.1/concreteproperties/analysis_section.py` & `concreteproperties-0.5.0/concreteproperties/analysis_section.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,23 +168,24 @@
             d_x = m_y_sec / n_sec
             d_y = m_x_sec / n_sec
 
         return sig, n_sec, d_x, d_y
 
     def service_analysis(
         self,
-        point_na: Tuple[float, float],
+        ecf: Tuple[float, float],
+        eps0: float,
         theta: float,
         kappa: float,
         centroid: Tuple[float, float],
     ) -> Tuple[float, float, float, float, float]:
         r"""Performs a service stress analysis on the section.
 
-        :param point_na: Point on the neutral axis
-        :param d_n: Depth of the neutral axis from the extreme compression fibre
+        :param ecf: Global coordinate of the extreme compressive fibre
+        :param eps0: Strain at top fibre
         :param theta: Angle (in radians) the neutral axis makes with the
             horizontal axis (:math:`-\pi \leq \theta \leq \pi`)
         :param kappa: Curvature
         :param centroid: Centroid about which to take moments
 
         :return: Axial force, section moments and min/max strain
         """
@@ -200,15 +201,16 @@
             (
                 el_n,
                 el_m_x,
                 el_m_y,
                 el_min_strain,
                 el_max_strain,
             ) = el.calculate_service_actions(
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=theta,
                 kappa=kappa,
                 centroid=centroid,
             )
             min_strain = min(min_strain, el_min_strain)
             max_strain = max(max_strain, el_max_strain)
 
@@ -216,26 +218,26 @@
             m_x_sec += el_m_x
             m_y_sec += el_m_y
 
         return n_sec, m_x_sec, m_y_sec, min_strain, max_strain
 
     def get_service_stress(
         self,
-        d_n: float,
         kappa: float,
-        point_na: Tuple[float, float],
+        ecf: Tuple[float, float],
+        eps0: float,
         theta: float,
         centroid: Tuple[float, float],
     ) -> Tuple[np.ndarray, float, float, float]:
         r"""Given the neutral axis depth `d_n` and curvature `kappa` determines the
         service stresses within the section.
 
-        :param d_n: Neutral axis depth
         :param kappa: Curvature
-        :param point_na: Point on the neutral axis
+        :param ecf: Global coordinate of the extreme compressive fibre
+        :param eps0: Strain at top fibre
         :param theta: Angle (in radians) the neutral axis makes with the
             horizontal axis (:math:`-\pi \leq \theta \leq \pi`)
         :param centroid: Centroid about which to take moments
 
         :return: Service stresses, net force and distance from centroid to point of
             force action
         """
@@ -244,25 +246,27 @@
         sig = np.zeros(len(self.mesh_nodes))
 
         # loop through nodes and calculate stress at nodes
         for idx, node in enumerate(self.mesh_nodes):
             # get strain at node
             strain = utils.get_service_strain(
                 point=(node[0], node[1]),
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=theta,
                 kappa=kappa,
             )
 
             # get stress at node
             sig[idx] = self.material.stress_strain_profile.get_stress(strain=strain)
 
         # calculate total force
         n_sec, m_x_sec, m_y_sec, _, _ = self.service_analysis(
-            point_na=point_na,
+            ecf=ecf,
+            eps0=eps0,
             theta=theta,
             kappa=kappa,
             centroid=centroid,
         )
 
         # calculate point of action
         if n_sec == 0:
@@ -603,22 +607,24 @@
             m_x_e += force_gp * y
             m_y_e += force_gp * x
 
         return force_e, m_x_e, m_y_e
 
     def calculate_service_actions(
         self,
-        point_na: Tuple[float, float],
+        ecf: Tuple[float, float],
+        eps0: float,
         theta: float,
         kappa: float,
         centroid: Tuple[float, float],
     ) -> Tuple[float, float, float, float, float]:
         r"""Calculates service actions for the current finite element.
 
-        :param point_na: Point on the neutral axis
+        :param ecf: Global coordinate of the extreme compressive fibre
+        :param eps0: Strain at top fibre
         :param theta: Angle (in radians) the neutral axis makes with the
             horizontal axis (:math:`-\pi \leq \theta \leq \pi`)
         :param kappa: Curvature
         :param centroid: Centroid about which to take moments
 
         :return: Axial force, moments and min/max strain
         """
@@ -641,15 +647,16 @@
             # get coordinates of the gauss point
             x = np.dot(N, np.transpose(self.coords[0, :]))
             y = np.dot(N, np.transpose(self.coords[1, :]))
 
             # get strain at gauss point
             strain = utils.get_service_strain(
                 point=(x, y),
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=theta,
                 kappa=kappa,
             )
             min_strain_e = min(min_strain_e, strain)
             max_strain_e = max(max_strain_e, strain)
 
             # get stress at gauss point
```

### Comparing `concreteproperties-0.4.1/concreteproperties/concrete_section.py` & `concreteproperties-0.5.0/concreteproperties/concrete_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from rich.live import Live
 from scipy.interpolate import interp1d
 from scipy.optimize import brentq
 
 import concreteproperties.results as res
 import concreteproperties.utils as utils
 from concreteproperties.analysis_section import AnalysisSection
-from concreteproperties.material import Concrete
+from concreteproperties.material import Concrete, SteelStrand
 from concreteproperties.post import plotting_context
 from concreteproperties.pre import CPGeom, CPGeomConcrete
 
 if TYPE_CHECKING:
     import matplotlib
 
 
@@ -26,15 +26,15 @@
     """Class for a reinforced concrete section."""
 
     def __init__(
         self,
         geometry: sp_geom.CompoundGeometry,
         moment_centroid: Optional[Tuple[float, float]] = None,
         geometric_centroid_override: bool = False,
-    ):
+    ) -> None:
         """Inits the ConcreteSection class.
 
         :param geometry: *sectionproperties* CompoundGeometry object describing the
             reinforced concrete section
         :param moment_centroid: If specified, all moments for service and ultimate
             analyses are calculated about this point. If not specified, all moments are
             calculated about the gross cross-section centroid, i.e. no material
@@ -50,42 +50,50 @@
         polygons = [sec_geom.geom for sec_geom in self.compound_geometry.geoms]
         overlapped_regions = sp_geom.check_geometry_overlaps(polygons)
         if overlapped_regions:
             warnings.warn(
                 "The provided geometry contains overlapping regions, results may be incorrect."
             )
 
-        # sort into concrete and reinforcement (meshed and lumped) geometries
+        # sort into concrete, reinforcement (meshed and lumped) and strand geometries
         self.all_geometries: List[Union[CPGeomConcrete, CPGeom]] = []
         self.meshed_geometries: List[Union[CPGeomConcrete, CPGeom]] = []
         self.concrete_geometries: List[CPGeomConcrete] = []
         self.reinf_geometries_meshed: List[CPGeom] = []
         self.reinf_geometries_lumped: List[CPGeom] = []
+        self.strand_geometries: List[CPGeom] = []
 
         # sort geometry into appropriate list
         for geom in self.compound_geometry.geoms:
             if isinstance(geom.material, Concrete):
                 cp_geom = CPGeomConcrete(geom=geom.geom, material=geom.material)
                 self.concrete_geometries.append(cp_geom)
                 self.meshed_geometries.append(cp_geom)
+            elif isinstance(geom.material, SteelStrand):
+                # SteelStrand materials can only be in PrestressedSection
+                if type(self) == ConcreteSection:
+                    raise ValueError(
+                        "SteelStrand material detected. Use PrestressedSection instead."
+                    )
+                else:
+                    cp_geom = CPGeom(geom=geom.geom, material=geom.material)
+                    self.strand_geometries.append(cp_geom)
             else:
                 cp_geom = CPGeom(geom=geom.geom, material=geom.material)  # type: ignore
 
                 if cp_geom.material.meshed:
                     self.reinf_geometries_meshed.append(cp_geom)
                     self.meshed_geometries.append(cp_geom)
                 elif not cp_geom.material.meshed:
                     self.reinf_geometries_lumped.append(cp_geom)
 
             self.all_geometries.append(cp_geom)
 
-        # initialise gross properties results class
+        # calculate gross properties
         self.gross_properties = res.GrossProperties()
-
-        # calculate gross area properties
         self.calculate_gross_area_properties()
 
         # set moment centroid
         if moment_centroid:
             self.moment_centroid = moment_centroid
         else:
             self.moment_centroid = (
@@ -93,17 +101,15 @@
                 self.gross_properties.cy_gross,
             )
 
         # if moment centroid overriden
         if geometric_centroid_override:
             self.moment_centroid = self.gross_properties.cx, self.gross_properties.cy
 
-    def calculate_gross_area_properties(
-        self,
-    ):
+    def calculate_gross_area_properties(self) -> None:
         """Calculates and stores gross section area properties."""
 
         # loop through all geometries
         for geom in self.all_geometries:
             # area and centroid of geometry
             area = geom.calculate_area()
             centroid = geom.calculate_centroid()
@@ -157,15 +163,15 @@
             for el in sec.elements:
                 el_e_ixx_g, el_e_iyy_g, el_e_ixy_g = el.second_moments_of_area()
                 self.gross_properties.e_ixx_g += el_e_ixx_g
                 self.gross_properties.e_iyy_g += el_e_iyy_g
                 self.gross_properties.e_ixy_g += el_e_ixy_g
 
         # lumped geometries - treat as lumped circles
-        for geom in self.reinf_geometries_lumped:
+        for geom in self.reinf_geometries_lumped + self.strand_geometries:
             # area, diameter and centroid of geometry
             area = geom.calculate_area()
             diam = np.sqrt(4 * area / np.pi)
             centroid = geom.calculate_centroid()
 
             self.gross_properties.e_ixx_g += geom.material.elastic_modulus * (
                 np.pi * pow(diam, 4) / 64 + area * centroid[1] * centroid[1]
@@ -322,101 +328,15 @@
             )
         except ValueError:
             msg = "Analysis failed. Please raise an issue at "
             msg += "https://github.com/robbievanleeuwen/concrete-properties/issues"
             raise utils.AnalysisError(msg)
 
         # calculate cracked section properties
-        # axial rigidity & first moments of area
-        for geom in cracked_results.cracked_geometries:
-            area = geom.calculate_area()
-            centroid = geom.calculate_centroid()
-
-            cracked_results.e_a_cr += area * geom.material.elastic_modulus
-            cracked_results.e_qx_cr += (
-                area * geom.material.elastic_modulus * centroid[1]
-            )
-            cracked_results.e_qy_cr += (
-                area * geom.material.elastic_modulus * centroid[0]
-            )
-
-        # centroids
-        cracked_results.cx = cracked_results.e_qy_cr / cracked_results.e_a_cr
-        cracked_results.cy = cracked_results.e_qx_cr / cracked_results.e_a_cr
-
-        # global second moments of area
-        for geom in cracked_results.cracked_geometries:
-            # if meshed
-            if geom.material.meshed:
-                sec = AnalysisSection(geometry=geom)
-
-                for el in sec.elements:
-                    el_e_ixx_g, el_e_iyy_g, el_e_ixy_g = el.second_moments_of_area()
-                    cracked_results.e_ixx_g_cr += el_e_ixx_g
-                    cracked_results.e_iyy_g_cr += el_e_iyy_g
-                    cracked_results.e_ixy_g_cr += el_e_ixy_g
-            # if lumped
-            else:
-                # area, diameter and centroid of geometry
-                area = geom.calculate_area()
-                diam = np.sqrt(4 * area / np.pi)
-                centroid = geom.calculate_centroid()
-
-                cracked_results.e_ixx_g_cr += geom.material.elastic_modulus * (
-                    np.pi * pow(diam, 4) / 64 + area * centroid[1] * centroid[1]
-                )
-                cracked_results.e_iyy_g_cr += geom.material.elastic_modulus * (
-                    np.pi * pow(diam, 4) / 64 + area * centroid[0] * centroid[0]
-                )
-                cracked_results.e_ixy_g_cr += geom.material.elastic_modulus * (
-                    area * centroid[0] * centroid[1]
-                )
-
-        # centroidal second moments of area
-        cracked_results.e_ixx_c_cr = (
-            cracked_results.e_ixx_g_cr
-            - cracked_results.e_qx_cr**2 / cracked_results.e_a_cr
-        )
-        cracked_results.e_iyy_c_cr = (
-            cracked_results.e_iyy_g_cr
-            - cracked_results.e_qy_cr**2 / cracked_results.e_a_cr
-        )
-        cracked_results.e_ixy_c_cr = (
-            cracked_results.e_ixy_g_cr
-            - cracked_results.e_qx_cr * cracked_results.e_qy_cr / cracked_results.e_a_cr
-        )
-        cracked_results.e_iuu_cr = (
-            cracked_results.e_iyy_c_cr * (np.sin(theta)) ** 2
-            + cracked_results.e_ixx_c_cr * (np.cos(theta)) ** 2
-            - 2 * cracked_results.e_ixy_c_cr * np.sin(theta) * np.cos(theta)
-        )
-
-        # principal 2nd moments of area about the centroidal xy axis
-        Delta = (
-            ((cracked_results.e_ixx_c_cr - cracked_results.e_iyy_c_cr) / 2) ** 2
-            + cracked_results.e_ixy_c_cr**2
-        ) ** 0.5
-        cracked_results.e_i11_cr = (
-            cracked_results.e_ixx_c_cr + cracked_results.e_iyy_c_cr
-        ) / 2 + Delta
-        cracked_results.e_i22_cr = (
-            cracked_results.e_ixx_c_cr + cracked_results.e_iyy_c_cr
-        ) / 2 - Delta
-
-        # principal axis angle
-        if (
-            abs(cracked_results.e_ixx_c_cr - cracked_results.e_i11_cr)
-            < 1e-12 * cracked_results.e_i11_cr
-        ):
-            cracked_results.phi_cr = 0
-        else:
-            cracked_results.phi_cr = np.arctan2(
-                cracked_results.e_ixx_c_cr - cracked_results.e_i11_cr,
-                cracked_results.e_ixy_c_cr,
-            )
+        self.cracked_section_properties(cracked_results=cracked_results)
 
         return cracked_results
 
     def calculate_cracking_moment(
         self,
         theta: float,
     ) -> float:
@@ -535,30 +455,139 @@
             # calculate first moment of area
             e_qu += ea * (c_v - na_local[1])
 
         cracked_results.cracked_geometries = cracked_geoms
 
         return e_qu
 
+    def cracked_section_properties(
+        self,
+        cracked_results: res.CrackedResults,
+    ) -> None:
+        """Given a list of cracked geometries (stored in ``cracked_results``),
+        determines the cracked section properties and stores in ``cracked_results``.
+
+        :param cracked_results: Cracked results object with stored cracked geometries
+        """
+
+        # reset results
+        cracked_results.reset_results()
+
+        # axial rigidity & first moments of area
+        for geom in cracked_results.cracked_geometries:
+            area = geom.calculate_area()
+            centroid = geom.calculate_centroid()
+
+            cracked_results.e_a_cr += area * geom.material.elastic_modulus
+            cracked_results.e_qx_cr += (
+                area * geom.material.elastic_modulus * centroid[1]
+            )
+            cracked_results.e_qy_cr += (
+                area * geom.material.elastic_modulus * centroid[0]
+            )
+
+        # centroids
+        cracked_results.cx = cracked_results.e_qy_cr / cracked_results.e_a_cr
+        cracked_results.cy = cracked_results.e_qx_cr / cracked_results.e_a_cr
+
+        # global second moments of area
+        for geom in cracked_results.cracked_geometries:
+            # if meshed
+            if geom.material.meshed:
+                sec = AnalysisSection(geometry=geom)
+
+                for el in sec.elements:
+                    el_e_ixx_g, el_e_iyy_g, el_e_ixy_g = el.second_moments_of_area()
+                    cracked_results.e_ixx_g_cr += el_e_ixx_g
+                    cracked_results.e_iyy_g_cr += el_e_iyy_g
+                    cracked_results.e_ixy_g_cr += el_e_ixy_g
+            # if lumped
+            else:
+                # area, diameter and centroid of geometry
+                area = geom.calculate_area()
+                diam = np.sqrt(4 * area / np.pi)
+                centroid = geom.calculate_centroid()
+
+                cracked_results.e_ixx_g_cr += geom.material.elastic_modulus * (
+                    np.pi * pow(diam, 4) / 64 + area * centroid[1] * centroid[1]
+                )
+                cracked_results.e_iyy_g_cr += geom.material.elastic_modulus * (
+                    np.pi * pow(diam, 4) / 64 + area * centroid[0] * centroid[0]
+                )
+                cracked_results.e_ixy_g_cr += geom.material.elastic_modulus * (
+                    area * centroid[0] * centroid[1]
+                )
+
+        # centroidal second moments of area
+        cracked_results.e_ixx_c_cr = (
+            cracked_results.e_ixx_g_cr
+            - cracked_results.e_qx_cr**2 / cracked_results.e_a_cr
+        )
+        cracked_results.e_iyy_c_cr = (
+            cracked_results.e_iyy_g_cr
+            - cracked_results.e_qy_cr**2 / cracked_results.e_a_cr
+        )
+        cracked_results.e_ixy_c_cr = (
+            cracked_results.e_ixy_g_cr
+            - cracked_results.e_qx_cr * cracked_results.e_qy_cr / cracked_results.e_a_cr
+        )
+        cracked_results.e_iuu_cr = (
+            cracked_results.e_iyy_c_cr * (np.sin(cracked_results.theta)) ** 2
+            + cracked_results.e_ixx_c_cr * (np.cos(cracked_results.theta)) ** 2
+            - 2
+            * cracked_results.e_ixy_c_cr
+            * np.sin(cracked_results.theta)
+            * np.cos(cracked_results.theta)
+        )
+
+        # principal 2nd moments of area about the centroidal xy axis
+        Delta = (
+            ((cracked_results.e_ixx_c_cr - cracked_results.e_iyy_c_cr) / 2) ** 2
+            + cracked_results.e_ixy_c_cr**2
+        ) ** 0.5
+        cracked_results.e_i11_cr = (
+            cracked_results.e_ixx_c_cr + cracked_results.e_iyy_c_cr
+        ) / 2 + Delta
+        cracked_results.e_i22_cr = (
+            cracked_results.e_ixx_c_cr + cracked_results.e_iyy_c_cr
+        ) / 2 - Delta
+
+        # principal axis angle
+        if (
+            abs(cracked_results.e_ixx_c_cr - cracked_results.e_i11_cr)
+            < 1e-12 * cracked_results.e_i11_cr
+        ):
+            cracked_results.phi_cr = 0
+        else:
+            cracked_results.phi_cr = np.arctan2(
+                cracked_results.e_ixx_c_cr - cracked_results.e_i11_cr,
+                cracked_results.e_ixy_c_cr,
+            )
+
     def moment_curvature_analysis(
         self,
         theta: float = 0,
+        n: float = 0,
+        kappa0: float = 0,
         kappa_inc: float = 1e-7,
         kappa_mult: float = 2,
         kappa_inc_max: float = 5e-6,
         delta_m_min: float = 0.15,
         delta_m_max: float = 0.3,
         progress_bar: bool = True,
     ) -> res.MomentCurvatureResults:
-        r"""Performs a moment curvature analysis given a bending angle ``theta``.
+        r"""Performs a moment curvature analysis given a bending angle ``theta`` and
+        applied axial force ``n``.
 
         Analysis continues until a material reaches its ultimate strain.
 
         :param theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
+        :param n: Axial force
+        :param kappa0: Initial curvature
         :param kappa_inc: Initial curvature increment
         :param kappa_mult: Multiplier to apply to the curvature increment ``kappa_inc``
             when ``delta_m_max`` is satisfied. When ``delta_m_min`` is satisfied, the
             inverse of this multipler is applied to ``kappa_inc``.
         :param kappa_inc_max: Maximum curvature increment
         :param delta_m_min: Relative change in moment at which to reduce the curvature
             increment
@@ -566,28 +595,20 @@
             increment
         :param progress_bar: If set to True, displays the progress bar
 
         :return: Moment curvature results object
         """
 
         # initialise variables
-        moment_curvature = res.MomentCurvatureResults(theta=theta)
-
-        # set neutral axis depth limits
-        # depth of neutral axis at extreme tensile fibre
-        _, d_t = utils.calculate_extreme_fibre(
-            points=self.compound_geometry.points, theta=theta
-        )
-        a = 1e-6 * d_t  # sufficiently small depth of compressive zone
-        b = d_t  # neutral axis at extreme tensile fibre
+        moment_curvature = res.MomentCurvatureResults(theta=theta, n_target=n)
 
         # function that performs moment curvature analysis
         def mcurve(kappa_inc=kappa_inc, progress=None):
             iter = 0
-            kappa = 0
+            kappa = kappa0
 
             while not moment_curvature._failure:
                 # calculate adaptive step size for curvature
                 if iter > 2:
                     moment_diff = (
                         abs(moment_curvature.kappa[-1] - moment_curvature.kappa[-2])
                         / moment_curvature.kappa[-1]
@@ -598,25 +619,23 @@
                         kappa_inc *= 1 / kappa_mult
 
                     # enforce maximum curvature increment
                     if kappa_inc > kappa_inc_max:
                         kappa_inc = kappa_inc_max
 
                 # update curvature
-                kappa = 0 if iter == 0 else moment_curvature.kappa[-1] + kappa_inc
+                kappa = kappa0 if iter == 0 else moment_curvature.kappa[-1] + kappa_inc
 
                 # find neutral axis that gives convergence of the axial force
                 try:
-                    (d_n, r) = brentq(
+                    brentq(
                         f=self.service_normal_force_convergence,
-                        a=a,
-                        b=b,
+                        a=-0.1,
+                        b=0.1,
                         args=(kappa, moment_curvature),
-                        xtol=1e-3,
-                        rtol=1e-6,  # type: ignore
                         full_output=True,
                         disp=False,
                     )
                 except ValueError:
                     if not moment_curvature._failure:
                         msg = "Analysis failed. Please raise an issue at "
                         msg += "https://github.com/robbievanleeuwen/concrete-properties/issues"
@@ -650,19 +669,17 @@
 
             # this method (given a kappa) outputs the failure convergence
             # (normalised to zero)
             def failure_kappa(kappa_fail):
                 # given kappa find equilibrium
                 brentq(
                     f=self.service_normal_force_convergence,
-                    a=a,
-                    b=b,
+                    a=-0.1,
+                    b=0.1,
                     args=(kappa_fail, moment_curvature),
-                    xtol=1e-3,
-                    rtol=1e-6,  # type: ignore
                     full_output=True,
                     disp=False,
                 )
 
                 return moment_curvature._failure_convergence - 1
 
             if progress:
@@ -707,56 +724,45 @@
         else:
             mcurve()
 
         return moment_curvature
 
     def service_normal_force_convergence(
         self,
-        d_n: float,
+        eps0: float,
         kappa: float,
         moment_curvature: res.MomentCurvatureResults,
     ) -> float:
         """Given a neutral axis depth ``d_n`` and curvature ``kappa``, returns the the
         net axial force.
 
-        :param d_n: Trial neutral axis
+        :param eps0: Strain at top fibre
         :param kappa: Curvature
         :param moment_curvature: Moment curvature results object
 
         :return: Net axial force
         """
 
         # reset failure
         moment_curvature._failure = False
 
-        # calculate extreme fibre in global coordinates
-        extreme_fibre, d_t = utils.calculate_extreme_fibre(
+        # get global coordinates of extreme compressive fibre
+        ecf, _ = utils.calculate_extreme_fibre(
             points=self.compound_geometry.points, theta=moment_curvature.theta
         )
 
-        # validate d_n input
-        if d_n <= 0:
-            raise ValueError("d_n must be positive.")
-        elif d_n > d_t:
-            raise ValueError("d_n must lie within the section, i.e. d_n <= d_t")
-
-        # find point on neutral axis by shifting by d_n
-        point_na = utils.point_on_neutral_axis(
-            extreme_fibre=extreme_fibre, d_n=d_n, theta=moment_curvature.theta
-        )
-
         # create splits in meshed geometries at points in stress-strain profiles
         meshed_split_geoms: List[Union[CPGeom, CPGeomConcrete]] = []
 
         for meshed_geom in self.meshed_geometries:
-            split_geoms = utils.split_geom_at_strains(
+            split_geoms = utils.split_geom_at_strains_service(
                 geom=meshed_geom,
                 theta=moment_curvature.theta,
-                point_na=point_na,
-                ultimate=False,
+                ecf=ecf,
+                eps0=eps0,
                 kappa=kappa,
             )
 
             meshed_split_geoms.extend(split_geoms)
 
         # initialise results
         n = 0
@@ -765,15 +771,16 @@
         failure_convergence = 0
 
         # calculate meshed geometry actions
         for meshed_geom in meshed_split_geoms:
             sec = AnalysisSection(geometry=meshed_geom)
 
             n_sec, m_x_sec, m_y_sec, min_strain, max_strain = sec.service_analysis(
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=moment_curvature.theta,
                 kappa=kappa,
                 centroid=self.moment_centroid,
             )
 
             n += n_sec
             m_x += m_x_sec
@@ -801,27 +808,33 @@
             # tensile failure (ignore concrete)
             if not isinstance(meshed_geom, CPGeomConcrete):
                 failure_convergence = max(
                     min_strain / ult_tens_strain, failure_convergence
                 )
 
         # calculate lumped geometry actions
-        for lumped_geom in self.reinf_geometries_lumped:
+        for lumped_geom in self.reinf_geometries_lumped + self.strand_geometries:
             # calculate area and centroid
             area = lumped_geom.calculate_area()
             centroid = lumped_geom.calculate_centroid()
 
             # get strain at centroid of lump
             strain = utils.get_service_strain(
                 point=(centroid[0], centroid[1]),
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=moment_curvature.theta,
                 kappa=kappa,
             )
 
+            # add initial prestress strain
+            if isinstance(lumped_geom.material, SteelStrand):
+                eps_pe = -lumped_geom.material.get_prestress_strain(area=area)
+                strain += eps_pe
+
             # check for failure
             ult_comp_strain = (
                 lumped_geom.material.stress_strain_profile.get_ultimate_compressive_strain()
             )
             ult_tens_strain = (
                 lumped_geom.material.stress_strain_profile.get_ultimate_tensile_strain()
             )
@@ -837,42 +850,50 @@
             failure_convergence = max(strain / ult_tens_strain, failure_convergence)
 
             # calculate stress and force
             stress = lumped_geom.material.stress_strain_profile.get_stress(
                 strain=strain
             )
             force = stress * area
+
             n += force
 
             # calculate moment
             m_x += force * (centroid[1] - self.moment_centroid[1])
             m_y += force * (centroid[0] - self.moment_centroid[0])
 
         moment_curvature._kappa = kappa
         moment_curvature._n_i = n
         moment_curvature._m_x_i = m_x
         moment_curvature._m_y_i = m_y
         moment_curvature._failure_convergence = failure_convergence
 
         # return normal force convergence
-        return n
+        return n - moment_curvature.n_target
 
     def ultimate_bending_capacity(
         self,
         theta: float = 0,
         n: float = 0,
     ) -> res.UltimateBendingResults:
         r"""Given a neutral axis angle ``theta`` and an axial force ``n``, calculates
         the ultimate bending capacity.
 
+        .. note::
+
+            This calculation is code agnostic and no capacity reduction factors are
+            applied. If design capacities are required, use the applicable
+            ``design_code`` module or consult your local design code on how to treat
+            nominal axial loads in ultimate bending calculations.
+
         Note that ``k_u`` is calculated only for lumped (non-meshed) geometries.
 
         :param theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
-        :param n: Net axial force
+        :param n: Net axial force (nominal axial load)
 
         :return: Ultimate bending results object
         """
 
         # set neutral axis depth limits
         # depth of neutral axis at extreme tensile fibre
         _, d_t = utils.calculate_extreme_fibre(
@@ -974,19 +995,18 @@
         # create splits in meshed geometries at points in stress-strain profiles
         meshed_split_geoms: List[Union[CPGeom, CPGeomConcrete]] = []
 
         if isinf(d_n):
             meshed_split_geoms = self.meshed_geometries
         else:
             for meshed_geom in self.meshed_geometries:
-                split_geoms = utils.split_geom_at_strains(
+                split_geoms = utils.split_geom_at_strains_ultimate(
                     geom=meshed_geom,
                     theta=ultimate_results.theta,
                     point_na=point_na,
-                    ultimate=True,
                     ultimate_strain=self.gross_properties.conc_ultimate_strain,
                     d_n=d_n,
                 )
 
                 meshed_split_geoms.extend(split_geoms)
 
         # initialise results
@@ -1007,15 +1027,15 @@
             )
 
             n += n_sec
             m_x += m_x_sec
             m_y += m_y_sec
 
         # calculate lumped actions
-        for lumped_geom in self.reinf_geometries_lumped:
+        for lumped_geom in self.reinf_geometries_lumped + self.strand_geometries:
             # calculate area and centroid
             area = lumped_geom.calculate_area()
             centroid = lumped_geom.calculate_centroid()
 
             # get strain at centroid of lump
             if isinf(d_n):
                 strain = self.gross_properties.conc_ultimate_strain
@@ -1024,14 +1044,19 @@
                     point=(centroid[0], centroid[1]),
                     point_na=point_na,
                     d_n=d_n,
                     theta=ultimate_results.theta,
                     ultimate_strain=self.gross_properties.conc_ultimate_strain,
                 )
 
+                # add initial prestress strain (N.B. ignore eps_ce)
+                if isinstance(lumped_geom.material, SteelStrand):
+                    eps_pe = -lumped_geom.material.get_prestress_strain(area=area)
+                    strain += eps_pe
+
             # calculate stress and force
             stress = lumped_geom.material.stress_strain_profile.get_stress(
                 strain=strain
             )
             force = stress * area
             n += force
 
@@ -1090,15 +1115,15 @@
         Types of control points are detailed below:
 
         .. admonition:: Control points
 
           - ``"D"`` - ratio of neutral axis depth to section depth
           - ``"d_n"`` - neutral axis depth
           - ``"fy"`` - yield ratio of the most extreme tensile bar
-          - ``"N"`` - axial force
+          - ``"N"`` - net (nominal) axial force
           - ``"kappa0"`` - zero curvature compression (N.B second item in tuple is not
             used)
 
         :param theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
         :param limits: List of control points that define the start and end of the
             interaction diagram. List length must equal two. The default limits range
@@ -1505,19 +1530,19 @@
                 -(e_ixy * m_x) / (e_ixx * e_iyy - e_ixy**2) * x
                 + (e_iyy * m_x) / (e_ixx * e_iyy - e_ixy**2) * y
             )
             sig += lumped_geom.material.elastic_modulus * (
                 +(e_ixx * m_y) / (e_ixx * e_iyy - e_ixy**2) * x
                 - (e_ixy * m_y) / (e_ixx * e_iyy - e_ixy**2) * y
             )
+
             strain = sig / lumped_geom.material.elastic_modulus
 
             # net force and point of action
             n_lumped = sig * lumped_geom.calculate_area()
-
             lumped_reinf_sigs.append(sig)
             lumped_reinf_strains.append(strain)
             lumped_reinf_forces.append((n_lumped, x, y))
             lumped_reinf_geoms.append(lumped_geom)
 
         return res.StressResult(
             concrete_section=self,
@@ -1698,33 +1723,25 @@
             # get curvature
             kappa = moment_curvature_results.get_curvature(moment=m)
 
         # get theta
         theta = moment_curvature_results.theta
 
         # initialise variables
-        mk = res.MomentCurvatureResults(theta=theta)
-
-        # set neutral axis depth limits
-        # depth of neutral axis at extreme tensile fibre
-        extreme_fibre, d_t = utils.calculate_extreme_fibre(
-            points=self.compound_geometry.points, theta=theta
+        mk = res.MomentCurvatureResults(
+            theta=theta, n_target=moment_curvature_results.n_target
         )
-        a = 1e-6 * d_t  # sufficiently small depth of compressive zone
-        b = d_t  # neutral axis at extreme tensile fibre
 
         # find neutral axis that gives convergence of the axial force
         try:
-            (d_n, r) = brentq(
+            eps0, r = brentq(
                 f=self.service_normal_force_convergence,
-                a=a,
-                b=b,
+                a=-0.1,
+                b=0.1,
                 args=(kappa, mk),
-                xtol=1e-3,
-                rtol=1e-6,  # type: ignore
                 full_output=True,
                 disp=False,
             )
         except ValueError:
             msg = "Analysis failed. Confirm that the supplied moment/curvature is "
             msg += "within the range of the moment-curvature analysis."
             raise utils.AnalysisError(msg)
@@ -1737,42 +1754,42 @@
         meshed_reinf_sigs = []
         meshed_reinf_forces = []
         lumped_reinf_geoms = []
         lumped_reinf_sigs = []
         lumped_reinf_strains = []
         lumped_reinf_forces = []
 
-        # find point on neutral axis by shifting by d_n
-        point_na = utils.point_on_neutral_axis(
-            extreme_fibre=extreme_fibre, d_n=d_n, theta=theta
+        # get global coordinates of extreme compressive fibre
+        ecf, _ = utils.calculate_extreme_fibre(
+            points=self.compound_geometry.points, theta=theta
         )
 
         # create splits in meshed geometries at points in stress-strain profiles
         meshed_split_geoms: List[Union[CPGeom, CPGeomConcrete]] = []
 
         for meshed_geom in self.meshed_geometries:
-            split_geoms = utils.split_geom_at_strains(
+            split_geoms = utils.split_geom_at_strains_service(
                 geom=meshed_geom,
                 theta=theta,
-                point_na=point_na,
-                ultimate=False,
+                ecf=ecf,
+                eps0=eps0,
                 kappa=kappa,
             )
 
             meshed_split_geoms.extend(split_geoms)
 
         # loop through all meshed geometries and calculate stress
         for meshed_geom in meshed_split_geoms:
             analysis_section = AnalysisSection(geometry=meshed_geom)
 
             # calculate stress, force and point of action
             sig, n_sec, d_x, d_y = analysis_section.get_service_stress(
-                d_n=d_n,
                 kappa=kappa,
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=theta,
                 centroid=self.moment_centroid,
             )
 
             # save results
             if isinstance(meshed_geom, CPGeomConcrete):
                 conc_sigs.append(sig)
@@ -1787,15 +1804,16 @@
         for lumped_geom in self.reinf_geometries_lumped:
             # get position of geometry
             centroid = lumped_geom.calculate_centroid()
 
             # get strain at centroid of lump
             strain = utils.get_service_strain(
                 point=(centroid[0], centroid[1]),
-                point_na=point_na,
+                ecf=ecf,
+                eps0=eps0,
                 theta=theta,
                 kappa=kappa,
             )
 
             # calculate stress, force and point of action
             sig = lumped_geom.material.stress_strain_profile.get_stress(strain=strain)
             n_lumped = sig * lumped_geom.calculate_area()
@@ -1866,19 +1884,18 @@
         # create splits in meshed geometries at points in stress-strain profiles
         meshed_split_geoms: List[Union[CPGeom, CPGeomConcrete]] = []
 
         if isinf(ultimate_results.d_n):
             meshed_split_geoms = self.meshed_geometries
         else:
             for meshed_geom in self.meshed_geometries:
-                split_geoms = utils.split_geom_at_strains(
+                split_geoms = utils.split_geom_at_strains_ultimate(
                     geom=meshed_geom,
                     theta=ultimate_results.theta,
                     point_na=point_na,
-                    ultimate=True,
                     ultimate_strain=self.gross_properties.conc_ultimate_strain,
                     d_n=ultimate_results.d_n,
                 )
 
                 meshed_split_geoms.extend(split_geoms)
 
         # loop through all concrete geometries and calculate stress
@@ -2106,16 +2123,16 @@
                         [meshed_geom.points[f[0]][0], meshed_geom.points[f[1]][0]],
                         [meshed_geom.points[f[0]][1], meshed_geom.points[f[1]][1]],
                         fmt,
                         markersize=2,
                         linewidth=1.5,
                     )
 
-            # plot lumped geometries
-            for lumped_geom in self.reinf_geometries_lumped:
+            # plot lumped geometries and strands
+            for lumped_geom in self.reinf_geometries_lumped + self.strand_geometries:
                 if lumped_geom.material not in plotted_materials:
                     patch = mpatches.Patch(
                         color=lumped_geom.material.colour,
                         label=lumped_geom.material.name,
                     )
                     legend_labels.append(patch)
                     plotted_materials.append(lumped_geom.material)
```

### Comparing `concreteproperties-0.4.1/concreteproperties/design_codes/as3600.py` & `concreteproperties-0.5.0/concreteproperties/design_codes/as3600.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from math import inf
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
+import numpy as np
+from rich.live import Live
+from scipy.interpolate import interp1d
+from scipy.optimize import brentq
+
 import concreteproperties.results as res
 import concreteproperties.stress_strain_profile as ssp
 import concreteproperties.utils as utils
-import numpy as np
 from concreteproperties.design_codes.design_code import DesignCode
 from concreteproperties.material import Concrete, SteelBar
-from rich.live import Live
-from scipy.interpolate import interp1d
-from scipy.optimize import brentq
 
 if TYPE_CHECKING:
     from concreteproperties.concrete_section import ConcreteSection
 
 
 class AS3600(DesignCode):
     """Design code class for Australian standard AS 3600:2018.
 
-    Note that this design code only supports :class:`~concreteproperties.pre.Concrete`
-    and :class:`~concreteproperties.pre.SteelBar` material objects. Meshed
-    :class:`~concreteproperties.pre.Steel` material objects are **not** supported
-    as this falls under the composite structures design code.
+    .. note::
+        Note that this design code only supports
+        :class:`~concreteproperties.material.Concrete` and
+        :class:`~concreteproperties.material.SteelBar` material objects. Meshed
+        :class:`~concreteproperties.material.Steel` material objects are **not**
+        supported as this falls under the composite structures design code.
     """
 
-    def __init__(
-        self,
-    ):
+    def __init__(self):
         """Inits the AS3600 class."""
 
         super().__init__()
 
     def assign_concrete_section(
         self,
         concrete_section: ConcreteSection,
@@ -71,23 +72,29 @@
     def create_concrete_material(
         self,
         compressive_strength: float,
         colour: str = "lightgrey",
     ) -> Concrete:
         r"""Returns a concrete material object to AS 3600:2018.
 
-        | **Material assumptions:**
-        | - *Density*: 2400 kg/m\ :sup:`3`
-        | - *Elastic modulus*: Interpolated from Table 3.1.2
-        | - *Service stress-strain profile*: Linear with no tension, compressive strength
-          at 0.9 * f'c
-        | - *Ultimate stress-strain profile*: Rectangular stress block, parameters from
-          Cl. 8.1.3
-        | - *Alpha squash*: From Cl. 10.6.2.2
-        | - *Flexural tensile strength*: From Cl. 3.1.1.3
+        .. admonition:: Material assumptions
+
+          - *Density*: 2400 kg/m\ :sup:`3`
+
+          - *Elastic modulus*: Interpolated from Table 3.1.2
+
+          - *Service stress-strain profile*: Linear with no tension, compressive
+            strength at :math:`0.9f'_c`
+
+          - *Ultimate stress-strain profile*: Rectangular stress block, parameters from
+            Cl. 8.1.3
+
+          - *Alpha squash*: From Cl. 10.6.2.2
+
+          - *Flexural tensile strength*: From Cl. 3.1.1.3
 
         :param compressive_strength: Characteristic compressive strength of
             concrete at 28 days in megapascals (MPa)
         :param colour: Colour of the concrete for rendering
 
         :raises ValueError: If ``compressive_strength`` is not between 20 MPa and
             100 MPa.
@@ -138,18 +145,21 @@
         self,
         yield_strength: float = 500,
         ductility_class: str = "N",
         colour: str = "grey",
     ) -> SteelBar:
         r"""Returns a steel bar material object.
 
-        | **Material assumptions:**
-        | - *Density*: 7850 kg/m\ :sup:`3`
-        | - *Elastic modulus*: 200,000 MPa
-        | - *Stress-strain profile:* Elastic-plastic, fracture strain from Table 3.2.1
+        .. admonition:: Material assumptions
+
+          - *Density*: 7850 kg/m\ :sup:`3`
+
+          - *Elastic modulus*: 200000 MPa
+
+          - *Stress-strain profile*: Elastic-plastic, fracture strain from Table 3.2.1
 
         :param yield_strength: Steel yield strength
         :param ductility_class: Steel ductility class ("N" or "L")
         :param colour: Colour of the steel for rendering
 
         :raises ValueError: If ``ductility_class`` is not "N" or "L"
 
@@ -170,17 +180,15 @@
                 yield_strength=yield_strength,
                 elastic_modulus=200e3,
                 fracture_strain=fracture_strain,
             ),
             colour=colour,
         )
 
-    def squash_tensile_load(
-        self,
-    ) -> Tuple[float, float]:
+    def squash_tensile_load(self) -> Tuple[float, float]:
         """Calculates the squash and tensile load of the reinforced concrete section.
 
         :return: Squash and tensile load
         """
 
         # initialise the squash load, tensile load and squash moment variables
         squash_load = 0
@@ -319,47 +327,47 @@
         )
 
         return balanced_res.n
 
     def ultimate_bending_capacity(
         self,
         theta: float = 0,
-        n: float = 0,
+        n_design: float = 0,
         phi_0: float = 0.6,
     ) -> Tuple[res.UltimateBendingResults, res.UltimateBendingResults, float]:
         r"""Calculates the ultimate bending capacity with capacity factors to
         AS 3600:2018.
 
         :param theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
-        :param n: Net axial force
+        :param n_design: Design axial force, N*
         :param phi_0: Compression dominant capacity reduction factor, see Table 2.2.2(d)
 
         :return: Factored and unfactored ultimate bending results objects, and capacity
             reduction factor *(factored_results, unfactored_results, phi)*
         """
 
         # get parameters to determine phi
         n_uot = self.tensile_load
         k_uo = self.get_k_uo(theta=theta)
         n_ub = self.get_n_ub(theta=theta)
 
         # non-linear calculation of phi
         def non_linear_phi(phi_guess):
             phi = self.capacity_reduction_factor(
-                n_u=n / phi_guess,
+                n_u=n_design / phi_guess,
                 n_ub=n_ub,
                 n_uot=n_uot,
                 k_uo=k_uo,
                 phi_0=phi_0,
             )
 
             return phi - phi_guess
 
-        (phi, r) = brentq(
+        phi, _ = brentq(
             f=non_linear_phi,
             a=phi_0,
             b=0.85,
             xtol=1e-3,
             rtol=1e-6,  # type: ignore
             full_output=True,
             disp=False,
@@ -379,63 +387,63 @@
         # get significant axial loads
         n_squash = f_mi_res.results[0].n
         n_decomp = f_mi_res.results[1].n
         n_tensile = f_mi_res.results[-1].n
 
         # DETERMINE where we are on interaction diagram
         # if we are above the squash load or tensile load
-        if n > n_squash:
+        if n_design > n_squash:
             raise utils.AnalysisError(
-                f"N = {n} is greater than the squash load, phiNc = {n_squash}."
+                f"N = {n_design} is greater than the squash load, phiNc = {n_squash}."
             )
-        elif n < n_tensile:
+        elif n_design < n_tensile:
             raise utils.AnalysisError(
-                f"N = {n} is greater than the tensile load, phiNt = {n_tensile}"
+                f"N = {n_design} is greater than the tensile load, phiNt = {n_tensile}"
             )
         # compression linear interpolation
-        elif n > n_decomp:
-            factor = (n - n_decomp) / (n_squash - n_decomp)
+        elif n_design > n_decomp:
+            factor = (n_design - n_decomp) / (n_squash - n_decomp)
             squash = f_mi_res.results[0]
             decomp = f_mi_res.results[1]
             ult_res = res.UltimateBendingResults(
                 theta=theta,
                 d_n=inf,
                 k_u=0,
-                n=n,
+                n=n_design / phi,
                 m_x=(decomp.m_x + factor * (squash.m_x - decomp.m_x)) / phi,
                 m_y=(decomp.m_y + factor * (squash.m_y - decomp.m_y)) / phi,
                 m_xy=(decomp.m_xy + factor * (squash.m_xy - decomp.m_xy)) / phi,
             )
         # regular calculation
-        elif n > 0:
+        elif n_design > 0:
             ult_res = self.concrete_section.ultimate_bending_capacity(
-                theta=theta, n=n / phi
+                theta=theta, n=n_design / phi
             )
         # tensile linear interpolation
         else:
-            factor = n / n_tensile
+            factor = n_design / n_tensile
             pure = f_mi_res.results[-2]
             ult_res = res.UltimateBendingResults(
                 theta=theta,
                 d_n=inf,
                 k_u=0,
-                n=n,
+                n=n_design / phi,
                 m_x=(1 - factor) * pure.m_x / phi,
                 m_y=(1 - factor) * pure.m_y / phi,
                 m_xy=(1 - factor) * pure.m_xy / phi,
             )
 
         # factor ultimate results
-        factored_ult_res = deepcopy(ult_res)
-        factored_ult_res.n *= phi
-        factored_ult_res.m_x *= phi
-        factored_ult_res.m_y *= phi
-        factored_ult_res.m_xy *= phi
+        f_ult_res = deepcopy(ult_res)
+        f_ult_res.n *= phi
+        f_ult_res.m_x *= phi
+        f_ult_res.m_y *= phi
+        f_ult_res.m_xy *= phi
 
-        return factored_ult_res, ult_res, phi
+        return f_ult_res, ult_res, phi
 
     def moment_interaction_diagram(
         self,
         theta: float = 0,
         limits: List[Tuple[str, float]] = [
             ("D", 1.0),
             ("N", 0.0),
@@ -448,27 +456,31 @@
         n_spacing: Optional[int] = None,
         phi_0: float = 0.6,
         progress_bar: bool = True,
     ) -> Tuple[res.MomentInteractionResults, res.MomentInteractionResults, List[float]]:
         r"""Generates a moment interaction diagram with capacity factors to
         AS 3600:2018.
 
-        See :meth:`concreteproperties.concrete_section.moment_interaction_diagram` for
-        allowable control points.
+        See :meth:`concreteproperties.concrete_section.ConcreteSection.moment_interaction_diagram`
+        for allowable control points.
+
+        .. note::
+
+            When providing ``"N"`` to ``limits`` or ``control_points``, ``"N"`` is taken
+            to be the unfactored net (nominal) axial load :math:`N^{*} / \phi`.
 
         :param theta: Angle (in radians) the neutral axis makes with the horizontal axis
             (:math:`-\pi \leq \theta \leq \pi`)
         :param limits: List of control points that define the start and end of the
             interaction diagram. List length must equal two. The default limits range
-            from concrete decompression strain to zero curvature tension.
+            from concrete decompression strain to the pure bending point.
         :param control_points: List of additional control points to add to the moment
-            interaction diagram. The default control points include the pure
-            compression point (``kappa0``), the balanced point (``fy=1``) and the pure
-            bending point (``N=0``). Control points may lie outside the limits of the
-            moment interaction diagram as long as equilibrium can be found.
+            interaction diagram. The default control points include the balanced point
+            (``fy=1``). Control points may lie outside the limits of the moment
+            interaction diagram as long as equilibrium can be found.
         :param labels: List of labels to apply to the ``limits`` and ``control_points``
             for plotting purposes. The first two values in ``labels`` apply labels to
             the ``limits``, the remaining values apply labels to the ``control_points``.
             If a single value is provided, this value will be applied to both ``limits``
             and all ``control_points``. The length of ``labels`` must equal ``1`` or
             ``2 + len(control_points)``.
         :param n_points: Number of points to compute including and between the
@@ -523,72 +535,72 @@
                 m_x=0,
                 m_y=0,
                 m_xy=0,
             )
         )
 
         # make a copy of the results to factor
-        factored_mi_res = deepcopy(mi_res)
+        f_mi_res = deepcopy(mi_res)
 
         # list to store phis
         phis = []
 
         # get required constants for phi
         n_uot = self.tensile_load
         k_uo = self.get_k_uo(theta=theta)
         n_ub = self.get_n_ub(theta=theta)
 
         # factor results
-        for ult_res in factored_mi_res.results:
+        for ult_res in f_mi_res.results:
             phi = self.capacity_reduction_factor(
                 n_u=ult_res.n, n_ub=n_ub, n_uot=n_uot, k_uo=k_uo, phi_0=phi_0
             )
             ult_res.n *= phi
             ult_res.m_x *= phi
             ult_res.m_y *= phi
             ult_res.m_xy *= phi
             phis.append(phi)
 
-        return factored_mi_res, mi_res, phis
+        return f_mi_res, mi_res, phis
 
     def biaxial_bending_diagram(
         self,
-        n: float = 0,
+        n_design: float = 0,
         n_points: int = 48,
         phi_0: float = 0.6,
         progress_bar: bool = True,
     ) -> Tuple[res.BiaxialBendingResults, List[float]]:
         """Generates a biaxial bending with capacity factors to AS 3600:2018.
 
-        :param n: Net axial force
+        :param n_design: Design axial force, N*
         :param n_points: Number of calculation points
         :param phi_0: Compression dominant capacity reduction factor, see Table 2.2.2(d)
         :param progress_bar: If set to True, displays the progress bar
 
         :return: Factored biaxial bending results object and list of capacity reduction
             factors *(factored_results, phis)*
         """
 
         # initialise results
-        f_bb_res = res.BiaxialBendingResults(n=n)
+        f_bb_res = res.BiaxialBendingResults(n=n_design)
         phis = []
 
         # calculate d_theta
         d_theta = 2 * np.pi / n_points
 
         # generate list of thetas
         theta_list = np.linspace(start=-np.pi, stop=np.pi - d_theta, num=n_points)
 
         # function that performs biaxial bending analysis
         def bbcurve(progress=None):
             # loop through thetas
             for theta in theta_list:
                 # factored capacity
                 f_ult_res, _, phi = self.ultimate_bending_capacity(
-                    theta=theta, n=n, phi_0=phi_0
+                    theta=theta, n_design=n_design, phi_0=phi_0
                 )
                 f_bb_res.results.append(f_ult_res)
                 phis.append(phi)
 
                 if progress:
                     progress.update(task, advance=1)
```

### Comparing `concreteproperties-0.4.1/concreteproperties/design_codes/design_code.py` & `concreteproperties-0.5.0/concreteproperties/design_codes/design_code.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/material.py` & `concreteproperties-0.5.0/concreteproperties/material.py`

 * *Files 17% similar despite different names*

```diff
@@ -97,11 +97,57 @@
     name: str
     density: float
     stress_strain_profile: ssp.StressStrainProfile
     colour: str
     meshed: bool = field(default=False, init=False)
 
 
-# @dataclass
-# class SteelStrand(Steel):
-#     # placeholder
-#     pass
+@dataclass
+class SteelStrand(Steel):
+    """Class for a steel strand material, treated as a lumped circular mass with a
+    constant strain.
+
+    .. note::
+
+      A :class:`~concreteproperties.stress_strain_profile.StrandProfile` must be used
+      if using a :class:`~concreteproperties.material.SteelStrand` object.
+
+    .. note::
+
+      The strand is assumed to be bonded to the concrete.
+
+    :param name: Steel strand material name
+    :param density: Steel strand density (mass per unit volume)
+    :param stress_strain_profile: Steel strand stress-strain profile
+    :param colour: Colour of the material for rendering
+    :param prestress_stress: Prestressing stress applied to the strand
+    """
+
+    name: str
+    density: float
+    stress_strain_profile: ssp.StrandProfile
+    colour: str
+    prestress_stress: float = 0
+    meshed: bool = field(default=False, init=False)
+
+    def get_prestress_stress(self) -> float:
+        """Returns the prestress stress.
+
+        :return: Prestress stress
+        """
+
+        return self.prestress_stress
+
+    def get_prestress_strain(
+        self,
+        area: float,
+    ) -> float:
+        """Given the strand cross-sectional area, returns the prestress strain.
+
+        :param area: Strand cross-sectional area
+
+        :return: Prestress strain
+        """
+
+        stress = self.get_prestress_stress()
+
+        return self.stress_strain_profile.get_strain(stress=stress)
```

### Comparing `concreteproperties-0.4.1/concreteproperties/post.py` & `concreteproperties-0.5.0/concreteproperties/post.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/pre.py` & `concreteproperties-0.5.0/concreteproperties/pre.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from concreteproperties.material import Concrete
 
 if TYPE_CHECKING:
     import matplotlib
     from sectionproperties.pre.geometry import CompoundGeometry
 
-    from concreteproperties.material import Material, SteelBar
+    from concreteproperties.material import Material, SteelBar, SteelStrand
 
 
 class CPGeom:
     """Watered down implementation of the *sectionproperties* Geometry object, optimised
     for *concreteproperties*.
     """
 
@@ -350,15 +350,15 @@
         # ensure material is a Concrete object
         self.material = material
 
 
 def add_bar(
     geometry: Union[Geometry, CompoundGeometry],
     area: float,
-    material: SteelBar,
+    material: Union[SteelBar, SteelStrand],
     x: float,
     y: float,
     n: int = 4,
 ) -> CompoundGeometry:
     """Adds a reinforcing bar to a *sectionproperties* geometry.
 
     Bars are discretised by four points by default.
@@ -379,15 +379,15 @@
 
     return (geometry - bar) + bar  # type: ignore
 
 
 def add_bar_rectangular_array(
     geometry: Union[Geometry, CompoundGeometry],
     area: float,
-    material: SteelBar,
+    material: Union[SteelBar, SteelStrand],
     n_x: int,
     x_s: float,
     n_y: int = 1,
     y_s: float = 0,
     anchor: Tuple[float, float] = (0, 0),
     exterior_only: bool = False,
     n: int = 4,
@@ -430,15 +430,15 @@
 
     return geometry  # type: ignore
 
 
 def add_bar_circular_array(
     geometry: Union[Geometry, CompoundGeometry],
     area: float,
-    material: SteelBar,
+    material: Union[SteelBar, SteelStrand],
     n_bar: int,
     r_array: float,
     theta_0: float = 0,
     ctr: Tuple[float, float] = (0, 0),
     n: int = 4,
 ) -> CompoundGeometry:
     """Adds a circular array of reinforcing bars to a *sectionproperties* geometry.
```

### Comparing `concreteproperties-0.4.1/concreteproperties/results.py` & `concreteproperties-0.5.0/concreteproperties/results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, List, Optional, Tuple
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 import matplotlib.cm as cm
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import matplotlib.tri as tri
 import numpy as np
 from matplotlib.collections import PatchCollection
 from matplotlib.colors import CenteredNorm  # type: ignore
-from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 from rich.console import Console
 from rich.table import Table
 from scipy.interpolate import interp1d
 from sectionproperties.pre.geometry import CompoundGeometry
 from shapely.geometry import Point
 from shapely.geometry.polygon import Polygon
 
@@ -40,14 +39,15 @@
     """
 
     # section areas
     total_area: float = 0
     concrete_area: float = 0
     reinf_meshed_area: float = 0
     reinf_lumped_area: float = 0
+    strand_area: float = 0
     e_a: float = 0
 
     # section mass
     mass: float = 0
 
     # section perimeter
     perimeter: float = 0
@@ -85,14 +85,16 @@
     e_z11_plus: float = 0
     e_z11_minus: float = 0
     e_z22_plus: float = 0
     e_z22_minus: float = 0
 
     # other properties
     conc_ultimate_strain: float = 0
+    n_prestress: float = 0
+    m_prestress: float = 0
 
     def print_results(
         self,
         fmt: str = "8.6e",
     ):
         """Prints the gross concrete section properties to the terminal.
 
@@ -101,22 +103,29 @@
 
         table = Table(title="Gross Concrete Section Properties")
         table.add_column("Property", justify="left", style="cyan", no_wrap=True)
         table.add_column("Value", justify="right", style="green")
 
         table.add_row("Total Area", "{:>{fmt}}".format(self.total_area, fmt=fmt))
         table.add_row("Concrete Area", "{:>{fmt}}".format(self.concrete_area, fmt=fmt))
-        table.add_row(
-            "Meshed Reinforcement Area",
-            "{:>{fmt}}".format(self.reinf_meshed_area, fmt=fmt),
-        )
+
+        if self.reinf_meshed_area:
+            table.add_row(
+                "Meshed Reinforcement Area",
+                "{:>{fmt}}".format(self.reinf_meshed_area, fmt=fmt),
+            )
+
         table.add_row(
             "Lumped Reinforcement Area",
             "{:>{fmt}}".format(self.reinf_lumped_area, fmt=fmt),
         )
+
+        if self.strand_area:
+            table.add_row("Strand Area", "{:>{fmt}}".format(self.strand_area, fmt=fmt))
+
         table.add_row("Axial Rigidity (EA)", "{:>{fmt}}".format(self.e_a, fmt=fmt))
         table.add_row("Mass (per unit length)", "{:>{fmt}}".format(self.mass, fmt=fmt))
         table.add_row("Perimeter", "{:>{fmt}}".format(self.perimeter, fmt=fmt))
         table.add_row("E.Qx", "{:>{fmt}}".format(self.e_qx, fmt=fmt))
         table.add_row("E.Qy", "{:>{fmt}}".format(self.e_qy, fmt=fmt))
         table.add_row("x-Centroid", "{:>{fmt}}".format(self.cx, fmt=fmt))
         table.add_row("y-Centroid", "{:>{fmt}}".format(self.cy, fmt=fmt))
@@ -140,14 +149,19 @@
         table.add_row("E.Z22+", "{:>{fmt}}".format(self.e_z22_plus, fmt=fmt))
         table.add_row("E.Z22-", "{:>{fmt}}".format(self.e_z22_minus, fmt=fmt))
         table.add_row(
             "Ultimate Concrete Strain",
             "{:>{fmt}}".format(self.conc_ultimate_strain, fmt=fmt),
         )
 
+        # add prestressed results if they exist
+        if self.n_prestress:
+            table.add_row("n_prestress", "{:>{fmt}}".format(self.n_prestress, fmt=fmt))
+            table.add_row("m_prestress", "{:>{fmt}}".format(self.m_prestress, fmt=fmt))
+
         console = Console()
         console.print(table)
 
 
 @dataclass
 class TransformedGrossProperties:
     """Class for storing transformed gross concrete section properties.
@@ -257,15 +271,17 @@
     method.
 
     :param theta: Angle (in radians) the neutral axis makes with the horizontal
         axis (:math:`-\pi \leq \theta \leq \pi`)
     """
 
     theta: float
-    m_cr: float = 0
+    n: float = 0
+    m: float = 0
+    m_cr: Union[float, Tuple[float, float]] = 0
     d_nc: float = 0
     cracked_geometries: List[CPGeom] = field(default_factory=list, repr=False)
     e_a_cr: float = 0
     e_qx_cr: float = 0
     e_qy_cr: float = 0
     cx: float = 0
     cy: float = 0
@@ -291,14 +307,33 @@
     ixx_c_cr: Optional[float] = None
     iyy_c_cr: Optional[float] = None
     ixy_c_cr: Optional[float] = None
     iuu_cr: Optional[float] = None
     i11_cr: Optional[float] = None
     i22_cr: Optional[float] = None
 
+    def reset_results(self) -> None:
+        """Resets the analysis results."""
+
+        self.e_a_cr = 0
+        self.e_qx_cr = 0
+        self.e_qy_cr = 0
+        self.cx = 0
+        self.cy = 0
+        self.e_ixx_g_cr = 0
+        self.e_iyy_g_cr = 0
+        self.e_ixy_g_cr = 0
+        self.e_ixx_c_cr = 0
+        self.e_iyy_c_cr = 0
+        self.e_ixy_c_cr = 0
+        self.e_iuu_cr = 0
+        self.e_i11_cr = 0
+        self.e_i22_cr = 0
+        self.phi_cr = 0
+
     def calculate_transformed_properties(
         self,
         elastic_modulus: float,
     ):
         """Calculates and stores transformed cracked properties using a reference
         elastic modulus.
 
@@ -348,21 +383,28 @@
         """
 
         table = Table(title="Cracked Concrete Section Properties")
         table.add_column("Property", justify="left", style="cyan", no_wrap=True)
         table.add_column("Value", justify="right", style="green")
 
         table.add_row("theta", "{:>{fmt}}".format(self.theta, fmt=fmt))
+        table.add_row("n", "{:>{fmt}}".format(self.n, fmt=fmt))
+        table.add_row("m", "{:>{fmt}}".format(self.m, fmt=fmt))
 
         if self.elastic_modulus_ref:
             table.add_row(
                 "E_ref", "{:>{fmt}}".format(self.elastic_modulus_ref, fmt=fmt)
             )
 
-        table.add_row("M_cr", "{:>{fmt}}".format(self.m_cr, fmt=fmt))
+        if isinstance(self.m_cr, tuple):
+            table.add_row("m_cr_pos", "{:>{fmt}}".format(self.m_cr[0], fmt=fmt))
+            table.add_row("m_cr_neg", "{:>{fmt}}".format(self.m_cr[1], fmt=fmt))
+        else:
+            table.add_row("m_cr", "{:>{fmt}}".format(self.m_cr, fmt=fmt))
+
         table.add_row("d_nc", "{:>{fmt}}".format(self.d_nc, fmt=fmt))
 
         if self.a_cr:
             table.add_row("A_cr", "{:>{fmt}}".format(self.a_cr, fmt=fmt))
 
         table.add_row("E.A_cr", "{:>{fmt}}".format(self.e_a_cr, fmt=fmt))
 
@@ -402,14 +444,15 @@
 
 
 @dataclass
 class MomentCurvatureResults:
     r"""Class for storing moment curvature results.
 
     :param theta: Angle (in radians) the neutral axis makes with the horizontal
+    :param n_target: Target axial force
         axis (:math:`-\pi \leq \theta \leq \pi`)
     :param kappa: List of curvatures
     :param n: List of axial forces
     :param m_x: List of bending moments about the x-axis
     :param m_y: List of bending moments about the y-axis
     :param m_xy: List of resultant bending moments
     :param failure_geometry: Geometry object of the region of the cross-section that
@@ -417,20 +460,21 @@
     :param convergence: The critical ratio between the strain and the failure strain
         within the cross-section for each curvature step in the analysis. A value of one
         indicates failure.
     """
 
     # results
     theta: float
+    n_target: float
     kappa: List[float] = field(default_factory=list)
     n: List[float] = field(default_factory=list)
     m_x: List[float] = field(default_factory=list)
     m_y: List[float] = field(default_factory=list)
     m_xy: List[float] = field(default_factory=list)
-    failure_geometry: CPGeom = field(init=False)
+    failure_geometry: CPGeom = field(init=False, repr=False)
     convergence: List[float] = field(default_factory=list)
 
     # for analysis
     _kappa: float = field(default=0, repr=False)
     _n_i: float = field(default=0, repr=False)
     _m_x_i: float = field(default=0, repr=False)
     _m_y_i: float = field(default=0, repr=False)
@@ -1053,28 +1097,39 @@
     :param lumped_reinforcement_geometries: List of lumped reinforcement geometry
         objects present in the stress analysis
     :param lumped_reinforcement_stresses: List of lumped reinforcement stresses for
         each lumped geometry
     :param lumped_reinforcement_strains: List of lumped reinforcement strains for each
         lumped geometry
     :param lumped_reinforcement_forces: List of net forces for each lumped reinforcement
-         geometry and its lever arm (``force``, ``d_x``, ``d_y``)
+        geometry and its lever arm (``force``, ``d_x``, ``d_y``)
+    :param strand_geometries: List of strand geometry objects present in the stress
+        analysis
+    :param strand_stresses: List of strand stresses for each strand
+    :param strand_strains: List of strand strains for each strand
+    :param strand_forces: List of net forces for each strand geometry and its lever arm
+        (``force``, ``d_x``, ``d_y``)
     """
 
     concrete_section: ConcreteSection
     concrete_analysis_sections: List[AnalysisSection]
     concrete_stresses: List[np.ndarray]
     concrete_forces: List[Tuple[float, float, float]]
     meshed_reinforcement_sections: List[AnalysisSection]
     meshed_reinforcement_stresses: List[np.ndarray]
     meshed_reinforcement_forces: List[Tuple[float, float, float]]
     lumped_reinforcement_geometries: List[CPGeom]
     lumped_reinforcement_stresses: List[float]
     lumped_reinforcement_strains: List[float]
     lumped_reinforcement_forces: List[Tuple[float, float, float]]
+    strand_geometries: List[CPGeom] = field(default_factory=list)
+    strand_stresses: List[float] = field(default_factory=list)
+    strand_strains: List[float] = field(default_factory=list)
+    strand_forces: List[Tuple[float, float, float]] = field(default_factory=list)
+    _m_net: Optional[float] = field(default=None, repr=False)
 
     def plot_stress(
         self,
         title: str = "Stress",
         conc_cmap: str = "RdGy",
         reinf_cmap: str = "bwr",
         **kwargs,
@@ -1119,17 +1174,21 @@
                     max([max(x) for x in self.meshed_reinforcement_stresses]) + 1e-12
                 )
             else:
                 meshed_reinf_sig_min = None
                 meshed_reinf_sig_max = None
 
             # if there is lumped reinforcement, calculate min and max
-            if self.lumped_reinforcement_stresses:
-                lumped_reinf_sig_min = min(self.lumped_reinforcement_stresses)
-                lumped_reinf_sig_max = max(self.lumped_reinforcement_stresses)
+            if self.lumped_reinforcement_stresses or self.strand_stresses:
+                lumped_reinf_sig_min = min(
+                    self.lumped_reinforcement_stresses + self.strand_stresses
+                )
+                lumped_reinf_sig_max = max(
+                    self.lumped_reinforcement_stresses + self.strand_stresses
+                )
             else:
                 lumped_reinf_sig_min = None
                 lumped_reinf_sig_max = None
 
             # determine min and max reinforcement stresess
             if (
                 meshed_reinf_sig_min
@@ -1272,14 +1331,22 @@
                 lumped_reinf_patches.append(
                     mpatches.Polygon(
                         xy=list(self.lumped_reinforcement_geometries[idx].geom.exterior.coords)  # type: ignore
                     )
                 )
                 colours.append(sig)
 
+            for idx, sig in enumerate(self.strand_stresses):
+                lumped_reinf_patches.append(
+                    mpatches.Polygon(
+                        xy=list(self.strand_geometries[idx].geom.exterior.coords)  # type: ignore
+                    )
+                )
+                colours.append(sig)
+
             patch = PatchCollection(lumped_reinf_patches, cmap=cmap_reinf)
             patch.set_array(colours)
             if reinf_tick_same:
                 patch.set_clim(vmin=0.99 * v_reinf[0], vmax=1.01 * v_reinf[-1])
             else:
                 patch.set_clim(vmin=v_reinf[0], vmax=v_reinf[-1])
             fig.axes[0].add_collection(patch)  # type: ignore
@@ -1304,61 +1371,85 @@
                 format="%.2e",
                 ticks=ticks_reinf,
                 cax=fig.axes[2],
             )
 
         return ax
 
-    def sum_forces(
-        self,
-    ) -> float:
+    def sum_forces(self) -> float:
         """Returns the sum of the internal forces.
 
         :return: Sum of internal forces
         """
 
         force_sum = 0
 
         # sum concrete forces
         for conc_force in self.concrete_forces:
             force_sum += conc_force[0]
 
-        # sum meshed reinf stresses
+        # sum meshed reinf forces
         for meshed_reinf_force in self.meshed_reinforcement_forces:
             force_sum += meshed_reinf_force[0]
 
         # sum lumped reinf forces
         for lumped_reinf_force in self.lumped_reinforcement_forces:
             force_sum += lumped_reinf_force[0]
 
+        # sum strand forces
+        for strand_force in self.strand_forces:
+            force_sum += strand_force[0]
+
         return force_sum
 
-    def sum_moments(
-        self,
-    ) -> Tuple[float, float, float]:
+    def sum_moments(self) -> Tuple[float, float, float]:
         """Returns the sum of the internal moments.
 
         :return: Sum of internal moments about each axis and resultant moment
             (``m_x``, ``m_y``, ``m``)
         """
 
         moment_sum_x = 0
         moment_sum_y = 0
 
-        # sum concrete forces
+        # sum concrete moments
         for conc_force in self.concrete_forces:
             moment_sum_x += conc_force[0] * conc_force[2]
             moment_sum_y += conc_force[0] * conc_force[1]
 
-        # sum meshed reinf stresses
+        # sum meshed reinf moments
         for meshed_reinf_force in self.meshed_reinforcement_forces:
             moment_sum_x += meshed_reinf_force[0] * meshed_reinf_force[2]
             moment_sum_y += meshed_reinf_force[0] * meshed_reinf_force[1]
 
-        # sum lumped reinf forces
+        # sum lumped reinf moments
         for lumped_reinf_force in self.lumped_reinforcement_forces:
             moment_sum_x += lumped_reinf_force[0] * lumped_reinf_force[2]
             moment_sum_y += lumped_reinf_force[0] * lumped_reinf_force[1]
 
+        # sum strand moments
+        for strand_force in self.strand_forces:
+            moment_sum_x += strand_force[0] * strand_force[2]
+            moment_sum_y += strand_force[0] * strand_force[1]
+
         moment_sum = np.sqrt(moment_sum_x * moment_sum_x + moment_sum_y * moment_sum_y)
 
         return moment_sum_x, moment_sum_y, moment_sum
+
+    def get_concrete_stress_limits(self) -> Tuple[float, float]:
+        """Returns the minimum and maximum concrete stress.
+
+        :return: Minimum concrete stress, maximum concrete stress
+        """
+
+        min_stress = 0
+        max_stress = 0
+
+        for idx, stress_list in enumerate(self.concrete_stresses):
+            if idx == 0:
+                min_stress = stress_list.min()
+                max_stress = stress_list.max()
+            else:
+                min_stress = min(min_stress, stress_list.min())
+                max_stress = max(max_stress, stress_list.max())
+
+        return min_stress, max_stress
```

### Comparing `concreteproperties-0.4.1/concreteproperties/tests/test_gross_properties.py` & `concreteproperties-0.5.0/concreteproperties/tests/test_gross_properties.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/tests/test_moment_interaction.py` & `concreteproperties-0.5.0/concreteproperties/tests/test_moment_interaction.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/tests/test_reinforced_concrete_basics.py` & `concreteproperties-0.5.0/concreteproperties/tests/test_reinforced_concrete_basics.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     ConcreteLinear,
     RectangularStressBlock,
     SteelElasticPlastic,
 )
 from sectionproperties.pre.library.concrete_sections import concrete_rectangular_section
 
 # All examples come from:
-# Warner, R. F., Foster, S. J., & Kilpatrick, A. E. (2007). Reinforced Concrete Basics (1st ed.). Pearson Australia.
+# Warner, R. F., Foster, S. J., & Kilpatrick, A. E. (2007). Reinforced Concrete Basics
+# (1st ed.). Pearson Australia.
 
 
 def test_example_3_1():
     concrete = Concrete(
         name="32 MPa Concrete",
         density=2.4e-6,
         stress_strain_profile=ConcreteLinear(elastic_modulus=30.1e3),
```

### Comparing `concreteproperties-0.4.1/concreteproperties/tests/test_rotation.py` & `concreteproperties-0.5.0/concreteproperties/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/tests/test_stress_equilibrium.py` & `concreteproperties-0.5.0/concreteproperties/tests/test_stress_equilibrium.py`

 * *Files identical despite different names*

### Comparing `concreteproperties-0.4.1/concreteproperties/utils.py` & `concreteproperties-0.5.0/concreteproperties/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,40 +13,42 @@
     from sectionproperties.pre.geometry import CompoundGeometry
 
     from concreteproperties.pre import CPGeom
 
 
 def get_service_strain(
     point: Tuple[float, float],
-    point_na: Tuple[float, float],
+    ecf: Tuple[float, float],
+    eps0: float,
     theta: float,
     kappa: float,
 ) -> float:
     r"""Determines the strain at point `point` given curvature `kappa` and neutral axis
     angle `theta`. Positive strain is compression.
 
     :param point: Point at which to evaluate the strain
-    :param point_na: Point on the neutral axis
+    :param ecf: Global coordinate of the extreme compressive fibre
+    :param eps0: Strain at top fibre
     :param theta: Angle (in radians) the neutral axis makes with the horizontal
         axis (:math:`-\pi \leq \theta \leq \pi`)
     :param kappa: Curvature
 
     :return: Strain
     """
 
     # convert point to local coordinates
     _, v = global_to_local(theta=theta, x=point[0], y=point[1])
 
-    # convert point_na to local coordinates
-    _, v_na = global_to_local(theta=theta, x=point_na[0], y=point_na[1])
+    # convert ecf to local coordinates
+    _, v_ecf = global_to_local(theta=theta, x=ecf[0], y=ecf[1])
 
-    # calculate distance between NA and point in `v` direction
-    d = v - v_na
+    # calculate distance between ecf and point in `v` direction
+    d = v_ecf - v
 
-    return kappa * d
+    return eps0 - kappa * d
 
 
 def get_ultimate_strain(
     point: Tuple[float, float],
     point_na: Tuple[float, float],
     d_n: float,
     theta: float,
@@ -99,70 +101,133 @@
     # subtract the neutral axis depth
     v -= d_n
 
     # convert point back to global coordinates
     return local_to_global(theta=theta, u=u, v=v)
 
 
-def split_geom_at_strains(
+def split_geom_at_strains_service(
+    geom: Union[CPGeom, CPGeomConcrete],
+    theta: float,
+    ecf: Tuple[float, float],
+    eps0: float,
+    kappa: float,
+) -> Union[List[CPGeom], List[CPGeomConcrete]]:
+    r"""Splits geometries at discontinuities in its stress-strain profile.
+
+    :param geom: Geometry to split
+    :param theta: Angle (in radians) the neutral axis makes with the horizontal
+        axis (:math:`-\pi \leq \theta \leq \pi`)
+    :param ecf: Global coordinate of the extreme compressive fibre
+    :param eps0: Strain at top fibre
+    :param kappa: Curvature
+
+    :return: List of split geometries
+    """
+
+    # handle zero curvature
+    if kappa == 0:
+        return [geom]
+
+    # create splits in concrete geometries at points in stress-strain profiles
+    split_geoms: Union[List[CPGeom], List[CPGeomConcrete]] = []
+
+    strains = geom.material.stress_strain_profile.get_unique_strains()
+
+    # make geom a list of geometries
+    geom_list = [geom]
+
+    # initialise top_geoms in case of two unique strains
+    top_geoms = geom_list
+    continuing_geoms = []
+
+    # loop through intermediate points on stress-strain profile
+    for strain in strains[1:-1]:
+        # depth to points of *strain* from ecf
+        d = (eps0 - strain) / kappa
+
+        # convert depth to global coordinates
+        dx, dy = local_to_global(theta=theta, u=0, v=d)
+
+        # calculate location of point
+        pt = ecf[0] - dx, ecf[1] - dy
+
+        # make list of geometries that will need to continue to be split after the
+        # split operation, i.e. those above the split
+        continuing_geoms = []
+
+        # split concrete geometries
+        for g in geom_list:
+            top_geoms, bot_geoms = g.split_section(
+                point=pt,
+                theta=theta,
+            )
+
+            if kappa < 0:
+                # save top geoms
+                split_geoms.extend(top_geoms)
+
+                # save continuing geoms
+                continuing_geoms.extend(bot_geoms)
+            else:
+                # save bot geoms
+                split_geoms.extend(bot_geoms)
+
+                # save continuing geoms
+                continuing_geoms.extend(top_geoms)
+
+        # update geom_list for next strain
+        geom_list = continuing_geoms
+
+    # save final top geoms
+    split_geoms.extend(continuing_geoms)
+
+    return split_geoms
+
+
+def split_geom_at_strains_ultimate(
     geom: Union[CPGeom, CPGeomConcrete],
     theta: float,
     point_na: Tuple[float, float],
-    ultimate: bool,
-    ultimate_strain: Optional[float] = None,
-    d_n: Optional[float] = None,
-    kappa: Optional[float] = None,
+    ultimate_strain: float,
+    d_n: float,
 ) -> Union[List[CPGeom], List[CPGeomConcrete]]:
     r"""Splits geometries at discontinuities in its stress-strain profile.
 
     :param geom: Geometry to split
     :param theta: Angle (in radians) the neutral axis makes with the horizontal
         axis (:math:`-\pi \leq \theta \leq \pi`)
     :param point_na: Point on the neutral axis
-    :param ultimate: If set to True, uses ultimate stress-strain profile for concrete
-        geometries
     :param ultimate_strain: Concrete strain at failure (required for ``ultimate=True``
         only)
     :param d_n: Depth of the neutral axis from the extreme compression fibre (required
         for ``ultimate=True`` only)
-    :param kappa: Curvature
 
     :return: List of split geometries
     """
 
-    # handle zero curvature
-    if kappa == 0:
-        return [geom]
-
     # create splits in concrete geometries at points in stress-strain profiles
     split_geoms: Union[List[CPGeom], List[CPGeomConcrete]] = []
 
-    if ultimate and isinstance(geom, CPGeomConcrete):
+    if isinstance(geom, CPGeomConcrete):
         strains = geom.material.ultimate_stress_strain_profile.get_unique_strains()
     else:
         strains = geom.material.stress_strain_profile.get_unique_strains()
 
     # make geom a list of geometries
     geom_list = [geom]
 
     # initialise top_geoms in case of two unique strains
     top_geoms = geom_list
     continuing_geoms = []
 
     # loop through intermediate points on stress-strain profile
     for strain in strains[1:-1]:
         # depth to points of *strain* from NA
-        # ultimate case
-        if ultimate and ultimate_strain and d_n:
-            d = strain / ultimate_strain * d_n
-        # service case
-        elif kappa:
-            d = strain / kappa
-        else:
-            raise ValueError("Not enough arguments provided.")
+        d = strain / ultimate_strain * d_n
 
         # convert depth to global coordinates
         dx, dy = local_to_global(theta=theta, u=0, v=d)
 
         # calculate location of point
         pt = point_na[0] + dx, point_na[1] + dy
 
@@ -241,15 +306,15 @@
     bending about an axis `theta`.
 
     :param points: Points over which to search for a bending depth
     :param c_local_v: Centroid coordinate in the local v-direction
     :param theta: Angle (in radians) the bending axis makes with the horizontal
         axis (:math:`-\pi \leq \theta \leq \pi`)
 
-    :return: Maximum bending depth
+    :return: Maximum bending depth, returns zero if distance is negative
     """
 
     max_bending_depth = 0
 
     # loop through all points
     for idx, point in enumerate(points):
         # determine the coordinate of the point wrt the local axis
```

### Comparing `concreteproperties-0.4.1/concreteproperties.egg-info/PKG-INFO` & `concreteproperties-0.5.0/concreteproperties.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concreteproperties
-Version: 0.4.1
+Version: 0.5.0
 Summary: A python package to determine cross-section propreties of reinforced concrete sections
 Home-page: https://github.com/robbievanleeuwen/concrete-properties
 Author: Robbie van Leeuwen
 Author-email: robbie.vanleeuwen@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/robbievanleeuwen/concrete-properties
 Project-URL: Tracker, https://github.com/robbievanleeuwen/concrete-properties/issues
@@ -39,89 +39,108 @@
 
 Here's an example of some of the non-linear output *concreteproperties* can generate:
 
 <p align="center">
   <img src="docs/source/_static/anim/anim_compress.gif" width="500"/>
 </p>
 
-## Installation:
+## Installation
 
 For more detailed installation instructions, refer to the [documentation](https://robbievanleeuwen.github.io/concrete-properties/rst/installation.html).
 
 ```shell
 pip install concreteproperties
 ```
 
-## Documentation:
+## Documentation
 
 *concreteproperties* is fully documented including examples and a fully documented API.
 The documentation can found at [https://robbievanleeuwen.github.io/concrete-properties](https://robbievanleeuwen.github.io/concrete-properties).
 
 ## Contributing
 
 We welcome anyone interested in contributing to *concreteproperties*, whether it be
 through submitting bug reports, feature requests or pull requests. Please read the
 [contributing guide](.github/CONTRIBUTING.md) prior to contributing.
 
-## Current Capabilities:
+## Current Capabilities
+
+### Analysis Types
+
+- [x] Reinforced Concrete
+- [x] Steel-Concrete Composite
+- [x] Prestressed Concrete
 
 ### Material Properties
+
 - [x] Concrete material
   - [x] Service stress-strain profiles
     - [x] Linear profile
     - [x] Linear profile (no tension)
     - [x] Eurocode non-linear
+    - [x] Modified Mander non-linear profile (confined & unconfined concrete)
   - [x] Ultimate stress-strain profiles
     - [x] Rectangular stress block
     - [x] Bilinear stress-strain profile
     - [x] Eurocode parabolic
   - [x] Flexural tensile strength
 - [x] Steel material
   - [x] Stress-strain profiles
     - [x] Elastic-plastic
     - [x] Elastic-plastic (with hardening)
+- [x] Strand material
+  - [x] Stress-strain profiles
+    - [x] Elastic-plastic (with hardening)
+    - [x] PCI journal (1992) non-linear
 
 ### Gross Section Properties
-- [x] Cross-sectional areas (total, concrete, steel)
+
+- [x] Cross-sectional areas (total, concrete, steel, strand)
 - [x] Axial rigidity
 - [x] Cross-section mass
 - [x] Cross-section perimeter
 - [x] First moments of area
 - [x] Elastic centroid
 - [x] Global second moments of area
 - [x] Centroidal second moments of area
 - [x] Principal axis angle
 - [x] Principal second moments of area
 - [x] Centroidal section moduli
 - [x] Principal section moduli
+- [x] Prestressed Aations
 
 ### Service Analysis
+
 - [x] Cracking moment
-- [x] Cracked second moment of area
+- [x] Cracked area properties
 - [x] Moment-curvature diagram
 
 ### Ultimate Analysis
+
 - [x] Ultimate bending capacity
 - [x] Squash load
 - [x] Tensile load
 - [x] Moment interaction diagrams
   - [x] M-N curves
   - [x] Biaxial bending curve
 
 ### Stress Analysis
+
 - [x] Uncracked stresses
 - [x] Cracked stresses
 - [x] Service stresses
 - [x] Ultimate stresses
 
 ### Design Codes
+
 - [x] Design code modules
   - [x] AS3600
   - [ ] AS5100
+  - [x] NZS3101 & NZSEE C5 Assessment Guidelines
 
-## Disclaimer:
+## Disclaimer
 
 *concreteproperties* is an open source engineering tool that continues to benefit from
 the collaboration of many contributors. Although efforts have been made to ensure the
 that relevant engineering theories have been correctly implemented, it remains the
 user's responsibility to confirm and accept the output. Refer to the
 [license](LICENSE.md) for clarification of the conditions of use.
```

### Comparing `concreteproperties-0.4.1/concreteproperties.egg-info/SOURCES.txt` & `concreteproperties-0.5.0/concreteproperties.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 setup.py
 concreteproperties/__init__.py
 concreteproperties/analysis_section.py
 concreteproperties/concrete_section.py
 concreteproperties/material.py
 concreteproperties/post.py
 concreteproperties/pre.py
+concreteproperties/prestressed_section.py
 concreteproperties/results.py
 concreteproperties/stress_strain_profile.py
 concreteproperties/utils.py
 concreteproperties.egg-info/PKG-INFO
 concreteproperties.egg-info/SOURCES.txt
 concreteproperties.egg-info/dependency_links.txt
 concreteproperties.egg-info/requires.txt
 concreteproperties.egg-info/top_level.txt
 concreteproperties/design_codes/__init__.py
 concreteproperties/design_codes/as3600.py
 concreteproperties/design_codes/design_code.py
+concreteproperties/design_codes/nzs3101.py
 concreteproperties/tests/__init__.py
 concreteproperties/tests/test_gross_properties.py
 concreteproperties/tests/test_moment_interaction.py
+concreteproperties/tests/test_nzs3101.py
+concreteproperties/tests/test_prestress.py
+concreteproperties/tests/test_prestress_validation.py
 concreteproperties/tests/test_reinforced_concrete_basics.py
 concreteproperties/tests/test_rotation.py
 concreteproperties/tests/test_stress_equilibrium.py
 concreteproperties/tests/test_stress_strain_profile.py
```

### Comparing `concreteproperties-0.4.1/setup.cfg` & `concreteproperties-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 	setuptools
 install_requires = 
 	numpy
 	scipy
 	matplotlib>=3.4
 	triangle
 	sectionproperties
+	shapely<2.0
 	rich
 
 [options.extras_require]
 test = 
 	pytest
 dev = 
 	pytest
```

