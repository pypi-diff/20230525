# Comparing `tmp/PyMoosh-2.2.tar.gz` & `tmp/PyMoosh-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMoosh-2.2.tar", last modified: Mon Jan 23 10:08:13 2023, max compression
+gzip compressed data, was "PyMoosh-2.3.tar", last modified: Wed Feb 15 08:19:19 2023, max compression
```

## Comparing `PyMoosh-2.2.tar` & `PyMoosh-2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-01-23 10:08:13.000000 PyMoosh-2.2/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3312 2023-01-23 10:08:13.000000 PyMoosh-2.2/PKG-INFO
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh/
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh/data/
--rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-01-23 09:22:24.000000 PyMoosh-2.2/PyMoosh/data/solar.json
--rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-01-23 09:22:24.000000 PyMoosh-2.2/PyMoosh/data/material_data.json
--rw-rw-r--   0 moi       (1001) moi       (1001)     1242 2023-01-23 10:08:03.000000 PyMoosh-2.2/PyMoosh/__init__.py
--rw-rw-r--   0 moi       (1001) moi       (1001)   127595 2023-01-23 09:22:24.000000 PyMoosh-2.2/PyMoosh/core.py
--rw-rw-r--   0 moi       (1001) moi       (1001)     3554 2023-01-23 09:22:24.000000 PyMoosh-2.2/PyMoosh/materials.py
--rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-30 09:31:04.000000 PyMoosh-2.2/LICENSE.txt
-drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/
--rw-rw-r--   0 moi       (1001) moi       (1001)     3312 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/PKG-INFO
--rw-rw-r--   0 moi       (1001) moi       (1001)      319 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/SOURCES.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/top_level.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/requires.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-01-23 10:08:13.000000 PyMoosh-2.2/PyMoosh.egg-info/dependency_links.txt
--rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-01-23 09:49:54.000000 PyMoosh-2.2/setup.py
--rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-01-23 09:49:38.000000 PyMoosh-2.2/MANIFEST.in
--rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-01-23 10:08:13.000000 PyMoosh-2.2/setup.cfg
--rw-rw-r--   0 moi       (1001) moi       (1001)     2536 2023-01-23 10:03:54.000000 PyMoosh-2.2/README.md
+drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/
+-rw-rw-r--   0 moi       (1000) moi       (1000)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.3/LICENSE.txt
+-rw-rw-r--   0 moi       (1000) moi       (1000)       34 2023-02-15 07:39:17.000000 PyMoosh-2.3/MANIFEST.in
+-rw-rw-r--   0 moi       (1000) moi       (1000)     3349 2023-02-15 08:19:19.371868 PyMoosh-2.3/PKG-INFO
+drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.367868 PyMoosh-2.3/PyMoosh/
+-rw-rw-r--   0 moi       (1000) moi       (1000)     1240 2023-02-15 08:15:49.000000 PyMoosh-2.3/PyMoosh/__init__.py
+-rw-rw-r--   0 moi       (1000) moi       (1000)   162285 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/core.py
+drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/PyMoosh/data/
+-rw-rw-r--   0 moi       (1000) moi       (1000)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/data/material_data.json
+-rw-rw-r--   0 moi       (1000) moi       (1000)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/data/solar.json
+-rw-rw-r--   0 moi       (1000) moi       (1000)     3616 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/materials.py
+drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/PyMoosh.egg-info/
+-rw-rw-r--   0 moi       (1000) moi       (1000)     3349 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/PKG-INFO
+-rw-rw-r--   0 moi       (1000) moi       (1000)      319 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/SOURCES.txt
+-rw-rw-r--   0 moi       (1000) moi       (1000)        1 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/dependency_links.txt
+-rw-rw-r--   0 moi       (1000) moi       (1000)       23 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/requires.txt
+-rw-rw-r--   0 moi       (1000) moi       (1000)        8 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/top_level.txt
+-rw-rw-r--   0 moi       (1000) moi       (1000)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.3/README.md
+-rw-rw-r--   0 moi       (1000) moi       (1000)      107 2023-02-15 08:19:19.371868 PyMoosh-2.3/setup.cfg
+-rw-rw-r--   0 moi       (1000) moi       (1000)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyMoosh-2.2/PKG-INFO` & `PyMoosh-2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.2
+Version: 2.3
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
         
@@ -49,14 +49,15 @@
         
         ## Contributors
         
         Here is a list of contributors to PyMoosh (one way or another) so far:
         
         * Pauline Bennet (@Ellawin)
         * Peter Wiecha
+        * Denis Langevin (@Milloupe)
         * Demetrio Macias
         * Anorld Capo-Chichi
         
         and the contributors to the original Moosh program should not be forgotten : Josselin Defrance, Rémi Pollès, Fabien Krayzel, Paul-Henri Tichit, Jessica Benedicto mainly. Special thanks to Gérard Granet and Jean-Pierre Plumey.
         
 Keywords: Moosh,Maxwell,Optics,Multilayers,Plasmonics,Photovoltaics
 Platform: UNKNOWN
```

### Comparing `PyMoosh-2.2/PyMoosh/data/solar.json` & `PyMoosh-2.3/PyMoosh/data/solar.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.2/PyMoosh/data/material_data.json` & `PyMoosh-2.3/PyMoosh/data/material_data.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.2/PyMoosh/__init__.py` & `PyMoosh-2.3/PyMoosh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
     in a multilayered structure. This makes PyMoosh unconditionally stable,
     allowing to explore even advanced properties of such multilayers,
     find poles and zeros of the scattering matrix (and thus guided modes),
     and many other things...
 
 """
 __name__ = 'PyMoosh'
-__version__ = '2.2'
-__date__ = "01/20/2023"   # MM/DD/YYY
+__version__ = '2.3'
+__date__ = "02/15/2023"   # MM/DD/YYY
 __author__ = 'Antoine Moreau'
 
 
-
-
 ## make accessible everything from `core` directly from the PyMoosh base package
 from PyMoosh.core import *
```

### Comparing `PyMoosh-2.2/PyMoosh/core.py` & `PyMoosh-2.3/PyMoosh/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -62,14 +62,19 @@
                 if verbose :
                     print("Object:",mat.__class__.__name__)
             elif isinstance(mat,float) or isinstance(mat,complex):
                 new_mat = Material(mat)
                 materials_final.append(new_mat)
                 if verbose :
                     print("Simple, non dispersive: epsilon=",mat)
+            elif isinstance(mat,int):
+                new_mat = Material(float(mat))
+                materials_final.append(new_mat)
+                if verbose :
+                    print("Simple, non dispersive: epsilon=",mat)
             elif isinstance(mat,list):
                 newmat = MagneticND(mat[0],mat[1])
                 materials_final.append(new_mat)
                 if verbose :
                     print("Magnetic, non dispersive: epsilon=", mat[0]," mu=",mat[1])
             elif mat.__class__.__name__ == 'function':
                 newmat = CustomFunction(mat)
@@ -123,14 +128,19 @@
             else:
                 print("Whhaaaaat ? That has nothing to do here :",mat)
 #                sys.exit( )
         self.materials = materials_final
         self.layer_type = layer_type
         self.thickness = thickness
 
+    def __str__(self):
+        materials = [str(self.materials[i]) for i in range(len(self.materials))]
+        s = f"materials: {materials}\nlayers: {self.layer_type}\nthicknesses: {self.thickness}"
+        return s
+
     def polarizability(self, wavelength):
         """ Computes the actual permittivity of each material considered in
         the structure. This method is called before each calculation.
 
         Args:
             wavelength (float): the working wavelength (in nanometers)
         """
@@ -222,117 +232,33 @@
     S[0, 0] = A[0, 0] + A[0, 1] * B[0, 0] * A[1, 0] * t
     S[0, 1] = A[0, 1] * B[0, 1] * t
     S[1, 0] = B[1, 0] * A[1, 0] * t
     S[1, 1] = B[1, 1] + A[1, 1] * B[0, 1] * B[1, 0] * t
     return (S)
 
 
-def coefficient(struct, wavelength, incidence, polarization):
+
+def cascade_DirtoNeu(A, B):
     """
-    This function computes the reflection and transmission coefficients
-    of the structure.
+    This function takes two 2x2 matrixes A and B, that are assumed to be Dirichlet to Neumann
+    and combines them assuming A is the "upper" one, and B the "lower" one, physically.
+    The result is a 2x2 scattering matrix.
 
     Args:
-        struct (Structure): belongs to the Structure class
-        wavelength (float): wavelength of the incidence light (in nm)
-        incidence (float): incidence angle in radians
-        polarization (float): 0 for TE, 1 (or anything) for TM
-
-    returns:
-        r (complex): reflection coefficient, phase origin at first interface
-        t (complex): transmission coefficient
-        R (float): Reflectance (energy reflection)
-        T (float): Transmittance (energie transmission)
-
-
-    R and T are the energy coefficients (real quantities)
+        A (2x2 numpy array):
+        B (2x2 numpy array):
 
-    .. warning: The transmission coefficients have a meaning only if the lower medium
-    is lossless, or they have no true meaning.
     """
-    # In order to get a phase that corresponds to the expected reflected coefficient,
-    # we make the height of the upper (lossless) medium vanish. It changes only the
-    # phase of the reflection coefficient.
-
-    # The medium may be dispersive. The permittivity and permability of each
-    # layer has to be computed each time.
-    Epsilon, Mu = struct.polarizability(wavelength)
-    thickness = copy.deepcopy(struct.thickness)
-    # In order to ensure that the phase reference is at the beginning
-    # of the first layer.
-    thickness[0] = 0
-    Type = struct.layer_type
-    # The boundary conditions will change when the polarization changes.
-    if polarization == 0:
-        f = Mu
-    else:
-        f = Epsilon
-    # Wavevector in vacuum.
-    k0 = 2 * np.pi / wavelength
-    # Number of layers
-    g = len(struct.layer_type)
-    # Wavevector k_x, horizontal
-    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
-    # Computation of the vertical wavevectors k_z
-    gamma = np.sqrt(
-        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
-    # Be cautious if the upper medium is a negative index one.
-    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
-        gamma[0] = -gamma[0]
-
-    # Changing the determination of the square root to achieve perfect stability
-    if g > 2:
-        gamma[1:g - 2] = gamma[1:g - 2] * (
-                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
-    # Outgoing wave condition for the last medium
-    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
-            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
-        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
-        gamma[g - 1] = -np.sqrt(
-            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
-    else:
-        gamma[g - 1] = np.sqrt(
-            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
-    T = np.zeros(((2 * g, 2, 2)), dtype=complex)
-
-    # first S matrix
-    T[0] = [[0, 1], [1, 0]]
-    for k in range(g - 1):
-        # Layer scattering matrix
-        t = np.exp((1j) * gamma[k] * thickness[k])
-        T[2 * k + 1] = [[0, t], [t, 0]]
-        # Interface scattering matrix
-        b1 = gamma[k] / f[Type[k]]
-        b2 = gamma[k + 1] / f[Type[k + 1]]
-        T[2 * k + 2] = [[(b1 - b2) / (b1 + b2), 2 * b2 / (b1 + b2)],
-                        [2 * b1 / (b1 + b2), (b2 - b1) / (b1 + b2)]]
-    t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
-    T[2 * g - 1] = [[0, t], [t, 0]]
-    # Once the scattering matrixes have been prepared, now let us combine them
-    A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
-    A[0] = T[0]
-
-    for j in range(len(T) - 2):
-        A[j + 1] = cascade(A[j], T[j + 1])
-    # reflection coefficient of the whole structure
-    r = A[len(A) - 1][0, 0]
-    # transmission coefficient of the whole structure
-    t = A[len(A) - 1][1, 0]
-    # Energy reflexion coefficient;
-    R = np.real(abs(r) ** 2)
-    # Energy transmission coefficient;
-    T = np.real(
-        abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
-
-    return r, t, R, T
-
-
-# def fcoefficient(struct,wavelength)
-#    '''Computation of the reflection coefficient of the structure using
-#    the formalism of impedances...
+    t = 1 / (A[1, 1] - B[0, 0])
+    S = np.zeros((2, 2), dtype=complex)
+    S[0, 0] = A[0, 0] - A[0, 1] * A[1, 0] * t
+    S[0, 1] = A[0, 1] * B[0, 1] * t
+    S[1, 0] = - B[1, 0] * A[1, 0] * t
+    S[1, 1] = B[1, 1] + B[1, 0] * B[0, 1]  * t
+    return (S)
 
 def absorption(struct, wavelength, incidence, polarization):
     """
     This function computes the percentage of the incoming energy
     that is absorbed in each layer when the structure is illuminated
     by a plane wave.
 
@@ -394,23 +320,24 @@
     else:
         gamma[g - 1] = np.sqrt(
             Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
     T = np.zeros(((2 * g, 2, 2)), dtype=complex)
 
     # first S matrix
     T[0] = [[0, 1], [1, 0]]
+    gf = gamma / f[Type]
     for k in range(g - 1):
         # Layer scattering matrix
         t = np.exp((1j) * gamma[k] * thickness[k])
         T[2 * k + 1] = [[0, t], [t, 0]]
         # Interface scattering matrix
-        b1 = gamma[k] / f[Type[k]]
-        b2 = gamma[k + 1] / f[Type[k + 1]]
-        T[2 * k + 2] = np.array(
-            [[b1 - b2, 2 * b2], [2 * b1, b2 - b1]] / (b1 + b2))
+        b1 = gf[k]
+        b2 = gf[k + 1]
+        T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                [2 * b1, b2 - b1]] / (b1 + b2))
     t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
     T[2 * g - 1] = [[0, t], [t, 0]]
     # Once the scattering matrixes have been prepared, now let us combine them
     H = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
     A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
     H[0] = T[2 * g - 1]
     A[0] = T[0]
@@ -552,21 +479,22 @@
             np.sqrt(Epsilon[Type[g]] * k0 ** 2 - alpha ** 2)) != 0:
             gamma[g] = -np.sqrt(
                 Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
         else:
             gamma[g] = np.sqrt(
                 Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
 
+        gf = gamma / f[Type]
         for k in range(g):
             t = np.exp(1j * gamma[k] * thickness[k])
             T[2 * k + 1] = np.array([[0, t], [t, 0]])
-            b1 = gamma[k] / f[Type[k]]
-            b2 = gamma[k + 1] / f[Type[k + 1]]
-            T[2 * k + 2] = np.array([[b1 - b2, 2 * b2], [2 * b1, b2 - b1]]) / (
-                    b1 + b2)
+            b1 = gf[k]
+            b2 = gf[k + 1]
+            T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                    [2 * b1, b2 - b1]]) / (b1 + b2)
         t = np.exp(1j * gamma[g] * thickness[g])
         T[2 * g + 1] = np.array([[0, t], [t, 0]])
 
         H = np.zeros((len(T) - 1, 2, 2), dtype=complex)
         A = np.zeros((len(T) - 1, 2, 2), dtype=complex)
 
         H[0] = T[2 * g + 1]
@@ -803,23 +731,24 @@
     gamma[g-1] = gamma[g-1] * (
                 1 - 2 * (np.angle(gamma[g-1])<-np.pi/5)  )
 
     T = np.zeros(((2 * g, 2, 2)), dtype=complex)
 
     # first S matrix
     T[0] = [[0, 1], [1, 0]]
+    gf = gamma / f[Type]
     for k in range(g - 1):
         # Layer scattering matrix
         t = np.exp((1j) * gamma[k] * thickness[k])
         T[2 * k + 1] = [[0, t], [t, 0]]
         # Interface scattering matrix
-        b1 = gamma[k] / f[Type[k]]
-        b2 = gamma[k + 1] / f[Type[k + 1]]
-        T[2 * k + 2] = [[(b1 - b2) / (b1 + b2), 2 * b2 / (b1 + b2)],
-                        [2 * b1 / (b1 + b2), (b2 - b1) / (b1 + b2)]]
+        b1 = gf[k]
+        b2 = gf[k + 1]
+        T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                 [2 * b1, b2 - b1]]) / (b1 + b2)
     t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
     T[2 * g - 1] = [[0, t], [t, 0]]
     # Once the scattering matrixes have been prepared, now let us combine them
     A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
     A[0] = T[0]
 
     for j in range(len(T) - 2):
@@ -1029,21 +958,22 @@
     gamma[0] = gamma[0] * (
                     1 - 2 * (np.angle(gamma[0])<-np.pi/5)  )
     gamma[g] = gamma[g] * (
                 1 - 2 * (np.angle(gamma[g])<-np.pi/5)  )
     # We compute all the scattering matrixes starting with the second layer
     T = np.zeros((2 * g, 2, 2), dtype=complex)
     T[0] = [[0, 1], [1, 0]]
+    gf = gamma / f[Type]
     for k in range(1,g):
         t = np.exp(1j * gamma[k] * thickness[k])
         T[2 * k -1 ] = np.array([[0, t], [t, 0]])
-        b1 = gamma[k] / f[Type[k]]
-        b2 = gamma[k + 1] / f[Type[k + 1]]
-        T[2 * k ] = np.array([[b1 - b2, 2 * b2], [2 * b1, b2 - b1]]) / (
-                    b1 + b2)
+        b1 = gf[k]
+        b2 = gf[k + 1]
+        T[2 * k ] = np.array([[b1 - b2, 2 * b2],
+                              [2 * b1, b2 - b1]]) / (b1 + b2)
     t = np.exp(1j * gamma[g] * thickness[g])
     T[2 * g - 1] = np.array([[0, t], [t, 0]])
 
     H = np.zeros((len(T) - 1, 2, 2), dtype=complex)
     A = np.zeros((len(T) - 1, 2, 2), dtype=complex)
     H[0] = T[2 * g - 1]
     A[0] = T[0]
@@ -1175,21 +1105,22 @@
             np.sqrt(Epsilon[Type[g]] * k0 ** 2 - alpha ** 2)) != 0:
             gamma[g] = -np.sqrt(
                 Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
         else:
             gamma[g] = np.sqrt(
                 Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
 
+        gf = gamma / f[Type]
         for k in range(g):
             t = np.exp(1j * gamma[k] * thickness[k])
             T[2 * k + 1] = np.array([[0, t], [t, 0]])
-            b1 = gamma[k] / f[Type[k]]
-            b2 = gamma[k + 1] / f[Type[k + 1]]
-            T[2 * k + 2] = np.array([[b1 - b2, 2 * b2], [2 * b1, b2 - b1]]) / (
-                    b1 + b2)
+            b1 = gf[k]
+            b2 = gf[k + 1]
+            T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                     [2 * b1, b2 - b1]]) / (b1 + b2)
         t = np.exp(1j * gamma[g] * thickness[g])
         T[2 * g + 1] = np.array([[0, t], [t, 0]])
 
         H_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
         A_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
 
         H_up[0] = T[0]
@@ -1225,7 +1156,971 @@
                     1j * gamma[k] * (thickness[k] - h))
                 t += 1
             h = 0
         E = E * np.exp(1j * alpha * np.arange(0, nx) / nx)
         En = En + E
 
     return En
+
+
+def coefficient(struct, wavelength, incidence, polarization):
+    """
+        Wrapper function to comput reflection and transmission coefficients
+        with various methods.
+        (and retrocompatibility)
+    """
+    return coefficient_S(struct, wavelength, incidence, polarization)
+
+
+def coefficient_S(struct, wavelength, incidence, polarization):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    T = np.zeros(((2 * g, 2, 2)), dtype=complex)
+
+    # first S matrix
+    T[0] = [[0, 1], [1, 0]]
+    gf = gamma / f[Type]
+    for k in range(g - 1):
+        # Layer scattering matrix
+        t = np.exp((1j) * gamma[k] * thickness[k])
+        T[2 * k + 1] = [[0, t], [t, 0]]
+        # Interface scattering matrix
+        b1 = gf[k]
+        b2 = gf[k + 1]
+        T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                 [2 * b1, b2 - b1]]) / (b1 + b2)
+    t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
+    T[2 * g - 1] = [[0, t], [t, 0]]
+    # Once the scattering matrixes have been prepared, now let us combine them
+    A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
+    A[0] = T[0]
+
+    for j in range(len(T) - 2):
+        A[j + 1] = cascade(A[j], T[j + 1])
+    # reflection coefficient of the whole structure
+    r = A[len(A) - 1][0, 0]
+    # transmission coefficient of the whole structure
+    t = A[len(A) - 1][1, 0]
+    # Energy reflexion coefficient;
+    R = np.real(abs(r) ** 2)
+    # Energy transmission coefficient;
+    T = np.real(
+        abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+
+    return r, t, R, T
+
+
+
+def coefficient_A(struct, wavelength, incidence, polarization):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the (true) Abeles matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+
+    T = np.zeros(((g-1, 2, 2)), dtype=complex)
+    c = np.cos(gamma * thickness)
+    s = np.sin(gamma * thickness)
+    gf = gamma/f[Type]
+    for k in range(g-1):
+        # Layer scattering matrix
+
+        T[k] = [[c[k], -s[k] / gf[k]],
+                [gf[k] * s[k], c[k]]]
+    # Once the scattering matrixes have been prepared, now let us combine them
+
+    A = np.empty((2,2), dtype=complex)
+    A = T[0]
+    for i in range(1, T.shape[0]):
+        A = T[i] @ A
+
+    a = A[0, 0]
+    b = A[0, 1]
+    c = A[1, 0]
+    d = A[1, 1]
+
+    amb = a - 1.j * gf[0] * b
+    apb = a + 1.j * gf[0] * b
+    cmd = c - 1.j * gf[0] * d
+    cpd = c + 1.j * gf[0] * d
+    # reflection coefficient of the whole structure
+
+    r = -(cmd + 1.j * gf[-1] * amb)/(cpd + 1.j * gf[-1] * apb)
+    # transmission coefficient of the whole structure
+    t = a * (r+1) + 1.j * gf[0] * b * (r-1)
+    # Energy reflexion coefficient;
+    R = np.real(abs(r) ** 2)
+    # Energy transmission coefficient;
+    T = np.real(abs(t) ** 2 * gf[g - 1] / gf[0])
+
+    return r, t, R, T
+
+
+def coefficient_T(struct, wavelength, incidence, polarization):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the Transfer matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+    T = np.zeros(((2*g-2, 2, 2)), dtype=complex)
+    gf = gamma/f[Type]
+    sum = (gf[1:] + gf[:-1]) / (2*gf[1:])
+    dif = (gf[1:] - gf[:-1]) / (2*gf[1:])
+    phases = np.exp(1.j* gamma[1:] * thickness[1:])
+    for k in range(g-1):
+        # Layer transfer matrix
+        T[2*k] = [[sum[k], dif[k]],
+                  [dif[k], sum[k]]]
+
+        # Layer propagation matrix
+        T[2*k+1] = [[1/phases[k], 0],
+                    [0, phases[k]]]
+    # Once the scattering matrixes have been prepared, now let us combine them
+
+    A = np.empty((2,2), dtype=complex)
+    A = T[0]
+    for i in range(1, T.shape[0]):
+        A =  A @ T[i]
+    # reflection coefficient of the whole structure
+    r = -A[1,0] / A[0,0]
+    # transmission coefficient of the whole structure
+    t = A[1,1] - (A[1,0] * A[0,1])/A[0,0]
+    # Energy reflexion coefficient;
+    R = np.real(abs(r) ** 2)
+    # Energy transmission coefficient;
+    T = np.real(abs(t) ** 2 * gf[g - 1] / gf[0])
+
+    return r, t, R, T
+
+
+def coefficient_DN(struct, wavelength, incidence, polarization):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the Dirichlet to Neumann matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+
+    T = np.zeros(((g-2, 2, 2)), dtype=complex)
+    gf = gamma/f[Type]
+    t = np.tan(gamma * thickness) / gf
+    s = np.sin(gamma * thickness) / gf
+    for k in range(1,g-1):
+        # Layer scattering matrix
+        T[k-1] = np.array([[1 / t[k], -1 / s[k]],
+                           [1 / s[k], -1 / t[k]]])
+    # Once the scattering matrixes have been prepared, now let us combine them
+
+    A = np.empty(T.shape, dtype=complex)
+    A[0] = T[0]
+    for j in range(1, T.shape[0]):
+        A[j] = cascade_DirtoNeu(A[j-1], T[j])
+
+    a = A[-1][0, 0]
+    b = A[-1][0, 1]
+    c = A[-1][1, 0]
+    d = A[-1][1, 1]
+
+    # reflection coefficient of the whole structure
+
+    gamma_eps = 1.j*gf[0]
+
+    r = ((a + gamma_eps)*(d + gamma_eps) - b*c)/((gamma_eps - a)*(d + gamma_eps) + b*c)
+    # transmission coefficient of the whole structure
+    t = - c * (r+1) / (d + gamma_eps)
+    # Energy reflexion coefficient;
+    R = np.real(abs(r) ** 2)
+    # Energy transmission coefficient;
+    T = np.real(abs(t) ** 2 * gf[g - 1] / gf[0])
+
+    return r, t, R, T
+
+def coefficient_I(struct, wavelength, incidence, polarization):
+    #n,d,lam,theta0):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the fast impedance formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+    cos_theta = np.zeros(g,dtype=complex)
+    sin_theta = np.zeros(g,dtype=complex)
+    n_s = np.zeros(g,dtype=complex)
+
+    sin_theta[0] = sin(incidence)
+
+    n = np.sqrt(Epsilon*Mu)
+
+    n_s[0] = n[Type[0]] * np.cos(incidence)
+    n_s[1:] = np.sqrt(n[Type[1:]]**2 - n[Type[0]]**2 * sin_theta[0]**2)
+    opp = np.imag(n_s) > 0
+    n_s = n_s - 2* n_s * (opp)
+
+    n_p = n[Type]**2 / n_s
+    delta = 2*np.pi*thickness*n_s/wavelength
+    #cos_theta = np.cos(np.arcsin(sin_theta))
+    temp = -1.j*np.tan(delta)
+    #print(sin_theta)
+    #print(cos_theta)
+    #print(temp)
+
+    if polarization == 0:
+        admittance = n_s
+    else:
+        admittance = n_p
+
+    Y = admittance[-1]
+
+    for m in np.arange(g-2,-1,-1):
+        Y = (Y + admittance[m]*temp[m])/(1 + Y*temp[m]/admittance[m])
+
+    r = (admittance[0]-Y) / (admittance[0]+Y)
+    if (polarization == 1):
+        r = -r
+    R = abs(r)**2
+
+    return(r,R)
+
+def coefficient_with_grad_A(struct, wavelength, incidence, polarization, mode="value", i_change=-1, saved_mat=None):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the (true) Abeles matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+        mode (string): "value" to compute r, t, R, T, "grad" to compute them with a small parameter shift
+        i_change (int): the layer where there is a modification
+        saved_mat (arrays): the matrices used to compute the coefficients
+
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+
+    if (mode == "grad" and saved_mat is None):
+        print("Not giving the abeles matrices to compute the gradient leads to regular computation")
+        return coefficient_A(struct, wavelength, incidence, polarization)
+
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+    if (mode == "value"):
+        T = np.zeros(((g-1, 2, 2)), dtype=complex)
+        for k in range(g-1):
+            # Layer scattering matrix
+            c = np.cos(gamma[k] * thickness[k])
+            s = np.sin(gamma[k] * thickness[k])
+
+            T[k] = [[c, -f[Type[k]]/gamma[k] * s],
+                    [gamma[k]/f[Type[k]] * s, c]]
+        # Once the scattering matrixes have been prepared, now let us combine them
+
+        A = np.empty((len(T)+1, 2, 2), dtype=complex)
+        B = np.empty((len(T)+1, 2, 2), dtype=complex)
+        A[0] = np.array([[1, 0],
+                         [0, 1]])
+        B[0] = np.array([[1, 0],
+                         [0, 1]])
+        for i in range(1, T.shape[0]+1):
+            A[i] = T[i-1] @ A[i-1]
+            B[i] = B[i-1] @ T[-i]
+
+        a = A[-1][0, 0]
+        b = A[-1][0, 1]
+        c = A[-1][1, 0]
+        d = A[-1][1, 1]
+
+        amb = a - 1.j * gamma[0]/f[Type[0]] * b
+        apb = a + 1.j * gamma[0]/f[Type[0]] * b
+        cmd = c - 1.j * gamma[0]/f[Type[0]] * d
+        cpd = c + 1.j * gamma[0]/f[Type[0]] * d
+        # reflection coefficient of the whole structure
+
+        r = -(cmd + 1.j * gamma[-1]/f[Type[-1]] * amb)/(cpd + 1.j * gamma[-1]/f[Type[-1]] * apb)
+        # transmission coefficient of the whole structure
+        t = a * (r+1) + 1.j * gamma[0]/f[Type[0]] * b * (r-1)
+        # Energy reflexion coefficient;
+        R = np.real(abs(r) ** 2)
+        # Energy transmission coefficient;
+        T = np.real(
+            abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+
+        return r, t, R, T, A, B
+
+    if (mode == "grad" and len(saved_mat) == 2):
+        A, B = saved_mat
+        T = np.zeros((2, 2), dtype=complex)
+        # Layer scattering matrix
+        c = np.cos(gamma[i_change] * thickness[i_change])
+        s = np.sin(gamma[i_change] * thickness[i_change])
+
+        T = [[c, -f[Type[i_change]]/gamma[i_change] * s],
+              [gamma[i_change]/f[Type[i_change]] * s, c]]
+
+        res = B[-i_change-2] @ T @ A[i_change]
+
+
+        a = res[0, 0]
+        b = res[0, 1]
+        c = res[1, 0]
+        d = res[1, 1]
+
+        amb = a - 1.j * gamma[0]/f[Type[0]] * b
+        apb = a + 1.j * gamma[0]/f[Type[0]] * b
+        cmd = c - 1.j * gamma[0]/f[Type[0]] * d
+        cpd = c + 1.j * gamma[0]/f[Type[0]] * d
+        # reflection coefficient of the whole structure
+
+        r = -(cmd + 1.j * gamma[-1]/f[Type[-1]] * amb)/(cpd + 1.j * gamma[-1]/f[Type[-1]] * apb)
+        # transmission coefficient of the whole structure
+        t = a * (r+1) + 1.j * gamma[0]/f[Type[0]] * b * (r-1)
+        # Energy reflexion coefficient;
+        R = np.real(abs(r) ** 2)
+        # Energy transmission coefficient;
+        T = np.real(
+            abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+
+        return r, t, R, T
+
+    else:
+        print("I do not understand what you are trying to do.")
+
+
+def coefficient_with_grad_T(struct, wavelength, incidence, polarization, mode="value", i_change=-1, saved_mat=None):
+    """
+    This function computes the reflection and transmission coefficients
+    of the structure using the Transfer matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+        mode (string): "value" to compute r, t, R, T, "grad" to compute them with a small parameter shift
+        i_change (int): the layer where there is a modification
+        saved_mat (arrays): the matrices used to compute the coefficients
+
+    returns:
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+
+    if (mode == "grad" and saved_mat is None):
+        print("Not giving the T matrices to compute the gradient leads to regular computation")
+        return coefficient_T(struct, wavelength, incidence, polarization)
+
+    # In order to get a phase that corresponds to the expected reflected coefficient,
+    # we make the height of the upper (lossless) medium vanish. It changes only the
+    # phase of the reflection coefficient.
+
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+    thickness = copy.deepcopy(struct.thickness)
+    # In order to ensure that the phase reference is at the beginning
+    # of the first layer.
+    thickness[0] = 0
+    Type = struct.layer_type
+    # The boundary conditions will change when the polarization changes.
+    if polarization == 0:
+        f = Mu
+    else:
+        f = Epsilon
+    # Wavevector in vacuum.
+    k0 = 2 * np.pi / wavelength
+    # Number of layers
+    g = len(struct.layer_type)
+    # Wavevector k_x, horizontal
+    alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * np.sin(incidence)
+    # Computation of the vertical wavevectors k_z
+    gamma = np.sqrt(
+        Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g) * alpha ** 2)
+    # Be cautious if the upper medium is a negative index one.
+    if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+        gamma[0] = -gamma[0]
+
+    # Changing the determination of the square root to achieve perfect stability
+    if g > 2:
+        gamma[1:g - 2] = gamma[1:g - 2] * (
+                    1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
+    # Outgoing wave condition for the last medium
+    if np.real(Epsilon[Type[g - 1]]) < 0 and np.real(
+            Mu[Type[g - 1]]) < 0 and np.real(np.sqrt(Epsilon[Type[g - 1]] * Mu[
+        Type[g - 1]] * k0 ** 2 - alpha ** 2)) != 0:
+        gamma[g - 1] = -np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+    else:
+        gamma[g - 1] = np.sqrt(
+            Epsilon[Type[g - 1]] * Mu[Type[g - 1]] * k0 ** 2 - alpha ** 2)
+
+    if (mode == "value"):
+        T = np.zeros(((2*g-2, 2, 2)), dtype=complex)
+        for k in range(g-1):
+            sum = gamma[k]/f[Type[k]] + gamma[k+1]/f[Type[k+1]]
+            dif = gamma[k]/f[Type[k]] - gamma[k+1]/f[Type[k+1]]
+            # print("pop", gamma[k], gamma[k+1])
+            # print(sum, dif)
+            # Layer transfer matrix
+            T[2*k] = f[Type[k+1]]/(2*gamma[k+1]) * np.array([[sum, -dif],
+                                                              [-dif, sum]])
+
+            phase = 1.j* gamma[k+1] * thickness[k+1]
+            # Layer propagation matrix
+            T[2*k+1] = [[np.exp(-phase), 0],
+                        [0, np.exp(phase)]]
+        # Once the scattering matrixes have been prepared, now let us combine them
+
+        A = np.empty((len(T)+1, 2, 2), dtype=complex)
+        B = np.empty((len(T)+1, 2, 2), dtype=complex)
+        A[0] = np.array([[1, 0],
+                         [0, 1]])
+        B[0] = np.array([[1, 0],
+                         [0, 1]])
+        for i in range(1, T.shape[0]+1):
+            A[i] =  A[i - 1] @ T[i-1]
+            B[i] = T[-i] @ B[i-1]
+        #print(T)
+        #print(A)
+        # reflection coefficient of the whole structure
+        r = -A[-1][1,0]/A[-1][0,0]
+        # transmission coefficient of the whole structure
+        t = A[-1][1,1] - (A[-1][1,0] * A[-1][0,1])/A[-1][0,0]
+        # Energy reflexion coefficient;
+        R = np.real(abs(r) ** 2)
+        # Energy transmission coefficient;
+        T = np.real(
+            abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+
+        return r, t, R, T, A, B
+
+    if (mode == "grad" and len(saved_mat) == 2):
+        A, B = saved_mat
+
+        if (0 < i_change):
+            T = np.zeros(((3, 2, 2)), dtype=complex)
+
+            sum = gamma[i_change-1]/f[Type[i_change-1]] + gamma[i_change]/f[Type[i_change]]
+            dif = gamma[i_change-1]/f[Type[i_change-1]] - gamma[i_change]/f[Type[i_change]]
+            # print("pop", gamma[k], gamma[k+1])
+            # print(sum, dif)
+            # Layer transfer matrix
+            T[0] = f[Type[i_change]]/(2*gamma[i_change]) * np.array([[sum, -dif],
+                                                                     [-dif, sum]])
+
+            phase = 1.j* gamma[i_change] * thickness[i_change]
+            # Layer propagation matrix
+            T[1] = [[np.exp(-phase), 0],
+                    [0, np.exp(phase)]]
+
+
+            sum = gamma[i_change]/f[Type[i_change]] + gamma[i_change+1]/f[Type[i_change+1]]
+            dif = gamma[i_change]/f[Type[i_change]] - gamma[i_change+1]/f[Type[i_change+1]]
+            # print("pop", gamma[k], gamma[k+1])
+            # print(sum, dif)
+            # Layer transfer matrix
+            T[2] = f[Type[i_change+1]]/(2*gamma[i_change+1]) * np.array([[sum, -dif],
+                                                                        [-dif, sum]])
+            # Once the scattering matrixes have been prepared, now let us combine them
+
+            res = A[i_change*2-2] @ T[0] @ T[1] @ T[2] @ B[-(i_change)*2-2]
+
+        else:
+            T = np.zeros(((2, 2, 2)), dtype=complex)
+
+            phase = 1.j* gamma[i_change] * thickness[i_change]
+            # Layer propagation matrix
+            T[0] = [[np.exp(-phase), 0],
+                    [0, np.exp(phase)]]
+
+
+            sum = gamma[i_change]/f[Type[i_change]] + gamma[i_change+1]/f[Type[i_change+1]]
+            dif = gamma[i_change]/f[Type[i_change]] - gamma[i_change+1]/f[Type[i_change+1]]
+            # print("pop", gamma[k], gamma[k+1])
+            # print(sum, dif)
+            # Layer transfer matrix
+            T[1] = f[Type[i_change+1]]/(2*gamma[i_change+1]) * np.array([[sum, -dif],
+                                                                        [-dif, sum]])
+            # Once the scattering matrixes have been prepared, now let us combine them
+            res = A[i_change*2] @ T[0] @ T[1] @ B[-(i_change)*2-2]
+
+        #print(T)
+        #print(A)
+        # reflection coefficient of the whole structure
+        r = -res[1,0]/res[0,0]
+        # transmission coefficient of the whole structure
+        t = res[1,1] - (res[1,0] * res[0,1])/res[0,0]
+        # Energy reflexion coefficient;
+        R = np.real(abs(r) ** 2)
+        # Energy transmission coefficient;
+        T = np.real(
+            abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+
+        return r, t, R, T
+
+def diff_coefficient(struct, wavelength, incidence, polarization, method="S", pas=0.01):
+    """
+    This function computes the reflection and transmission coefficients derivative
+    of the structure using the Transfer matrix formalism.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+        method (string): T for T matrix, A for abeles matrix
+
+    returns:
+        dr (complex): deriv. of reflection coefficient, phase origin at first interface
+        dt (complex): deriv. of transmission coefficient
+        dR (float): deriv. of Reflectance (energy reflection)
+        dT (float): deriv. of Transmittance (energie transmission)
+
+
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+    """
+
+    nb_var = len(struct.thickness)-2 + len(struct.layer_type)-2
+    base_thickness = struct.thickness
+    base_mat = np.array(struct.materials)
+    base_lay = struct.layer_type
+
+    dr = np.zeros(nb_var, dtype=complex)
+    dt = np.zeros(nb_var, dtype=complex)
+    dR = np.zeros(nb_var, dtype=float)
+    dT = np.zeros(nb_var, dtype=float)
+
+    function = None
+
+    if (method == "T"):
+        function = coefficient_with_grad_T
+    elif (method =="A"):
+        function = coefficient_with_grad_A
+
+    if not function is None:
+        # Using one of the fast differentiation methods
+        r, t, R, T, A, B = function(struct, wavelength, incidence, polarization, mode="value")
+
+        for i in range(len(base_thickness) - 2):
+            thickness = base_thickness.copy()
+            thickness[i+1] += pas
+            struct = Structure(base_mat, base_lay, thickness, verbose=False)
+            r_pas, t_pas, R_pas, T_pas = function(struct, wavelength, incidence, polarization,
+                                                  mode="grad", i_change=i+1, saved_mat=[A,B])
+            dr[i] = (r_pas - r)/pas
+            dt[i] = (t_pas - t)/pas
+            dR[i] = (R_pas - R)/pas
+            dT[i] = (T_pas - T)/pas
+
+        for i in range(len(base_mat)-2):
+            mat = list(base_mat.copy())
+            layer_type = base_lay.copy()
+
+            mat.append(mat[base_lay[i+1]].permittivity+pas)
+            # Creating a new permittivity and referencing it
+            layer_type[i+1] = len(mat)-1
+
+            struct = Structure(mat, layer_type, base_thickness, verbose=False)
+            r_pas, t_pas, R_pas, T_pas = function(struct, wavelength, incidence, polarization,
+                                                  mode="grad", i_change=i+1, saved_mat=[A,B])
+            dr[i+len(base_thickness)-2] = (r_pas - r)/pas
+            dt[i+len(base_thickness)-2] = (t_pas - t)/pas
+            dR[i+len(base_thickness)-2] = (R_pas - R)/pas
+            dT[i+len(base_thickness)-2] = (T_pas - T)/pas
+
+        return dr, dt, dR, dT
+
+    # Not using the fast computation -> using S matrix formalism
+    function = coefficient_S
+    r, t, R, T, = function(struct, wavelength, incidence, polarization)
+
+    for i in range(len(base_thickness)-2):
+        thickness = base_thickness.copy()
+        thickness[i+1] += pas
+        struct = Structure(base_mat, base_lay, thickness, verbose=False)
+        r_pas, t_pas, R_pas, T_pas = function(struct, wavelength, incidence, polarization)
+        dr[i] = (r_pas - r)/pas
+        dt[i] = (t_pas - t)/pas
+        dR[i] = (R_pas - R)/pas
+        dT[i] = (T_pas - T)/pas
+
+    for i in range(len(base_mat)-2):
+        mat = list(base_mat.copy())
+        layer_type = base_lay.copy()
+
+        mat.append(mat[base_lay[i+1]].permittivity+pas)
+        # Creating a new permittivity and referencing it
+        layer_type[i+1] = len(mat)-1
+
+        struct = Structure(mat, layer_type, base_thickness, verbose=False)
+        r_pas, t_pas, R_pas, T_pas = function(struct, wavelength, incidence, polarization)
+        dr[i+len(base_thickness)-2] = (r_pas - r)/pas
+        dR[i+len(base_thickness)-2] = (R_pas - R)/pas
+        dt[i+len(base_thickness)-2] = (t_pas - t)/pas
+        dT[i+len(base_thickness)-2] = (T_pas - T)/pas
+
+    return dr, dt, dR, dT
```

### Comparing `PyMoosh-2.2/PyMoosh/materials.py` & `PyMoosh-2.3/PyMoosh/materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 #from enum import Enum
 
 class Material:
 
     def __init__(self,permittivity):
         self.permittivity = permittivity
 
+    def __str__(self):
+        return str(self.permittivity)
+
     def get_permittivity(self,wavelength):
         return self.permittivity
 
     def get_permeability(self,wavelength):
         return 1.0
 
 class CustomFunction(Material):
```

### Comparing `PyMoosh-2.2/LICENSE.txt` & `PyMoosh-2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.2/PyMoosh.egg-info/PKG-INFO` & `PyMoosh-2.3/PyMoosh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.2
+Version: 2.3
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
         
@@ -49,14 +49,15 @@
         
         ## Contributors
         
         Here is a list of contributors to PyMoosh (one way or another) so far:
         
         * Pauline Bennet (@Ellawin)
         * Peter Wiecha
+        * Denis Langevin (@Milloupe)
         * Demetrio Macias
         * Anorld Capo-Chichi
         
         and the contributors to the original Moosh program should not be forgotten : Josselin Defrance, Rémi Pollès, Fabien Krayzel, Paul-Henri Tichit, Jessica Benedicto mainly. Special thanks to Gérard Granet and Jean-Pierre Plumey.
         
 Keywords: Moosh,Maxwell,Optics,Multilayers,Plasmonics,Photovoltaics
 Platform: UNKNOWN
```

### Comparing `PyMoosh-2.2/setup.py` & `PyMoosh-2.3/setup.py`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.2/README.md` & `PyMoosh-2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,11 +41,12 @@
 
 ## Contributors
 
 Here is a list of contributors to PyMoosh (one way or another) so far:
 
 * Pauline Bennet (@Ellawin)
 * Peter Wiecha
+* Denis Langevin (@Milloupe)
 * Demetrio Macias
 * Anorld Capo-Chichi
 
 and the contributors to the original Moosh program should not be forgotten : Josselin Defrance, Rémi Pollès, Fabien Krayzel, Paul-Henri Tichit, Jessica Benedicto mainly. Special thanks to Gérard Granet and Jean-Pierre Plumey.
```

