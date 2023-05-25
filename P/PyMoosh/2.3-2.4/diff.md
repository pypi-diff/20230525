# Comparing `tmp/PyMoosh-2.3.tar.gz` & `tmp/PyMoosh-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMoosh-2.3.tar", last modified: Wed Feb 15 08:19:19 2023, max compression
+gzip compressed data, was "dist/PyMoosh-2.4.tar", last modified: Thu May 25 09:14:35 2023, max compression
```

## Comparing `PyMoosh-2.3.tar` & `PyMoosh-2.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/
--rw-rw-r--   0 moi       (1000) moi       (1000)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.3/LICENSE.txt
--rw-rw-r--   0 moi       (1000) moi       (1000)       34 2023-02-15 07:39:17.000000 PyMoosh-2.3/MANIFEST.in
--rw-rw-r--   0 moi       (1000) moi       (1000)     3349 2023-02-15 08:19:19.371868 PyMoosh-2.3/PKG-INFO
-drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.367868 PyMoosh-2.3/PyMoosh/
--rw-rw-r--   0 moi       (1000) moi       (1000)     1240 2023-02-15 08:15:49.000000 PyMoosh-2.3/PyMoosh/__init__.py
--rw-rw-r--   0 moi       (1000) moi       (1000)   162285 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/core.py
-drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/PyMoosh/data/
--rw-rw-r--   0 moi       (1000) moi       (1000)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/data/material_data.json
--rw-rw-r--   0 moi       (1000) moi       (1000)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/data/solar.json
--rw-rw-r--   0 moi       (1000) moi       (1000)     3616 2023-02-15 07:39:17.000000 PyMoosh-2.3/PyMoosh/materials.py
-drwxrwxr-x   0 moi       (1000) moi       (1000)        0 2023-02-15 08:19:19.371868 PyMoosh-2.3/PyMoosh.egg-info/
--rw-rw-r--   0 moi       (1000) moi       (1000)     3349 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/PKG-INFO
--rw-rw-r--   0 moi       (1000) moi       (1000)      319 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/SOURCES.txt
--rw-rw-r--   0 moi       (1000) moi       (1000)        1 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/dependency_links.txt
--rw-rw-r--   0 moi       (1000) moi       (1000)       23 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/requires.txt
--rw-rw-r--   0 moi       (1000) moi       (1000)        8 2023-02-15 08:19:19.000000 PyMoosh-2.3/PyMoosh.egg-info/top_level.txt
--rw-rw-r--   0 moi       (1000) moi       (1000)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.3/README.md
--rw-rw-r--   0 moi       (1000) moi       (1000)      107 2023-02-15 08:19:19.371868 PyMoosh-2.3/setup.cfg
--rw-rw-r--   0 moi       (1000) moi       (1000)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.3/setup.py
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-05-25 09:14:35.000000 PyMoosh-2.4/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3349 2023-05-25 09:14:35.000000 PyMoosh-2.4/PKG-INFO
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh/
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh/data/
+-rw-rw-r--   0 moi       (1001) moi       (1001)    80345 2023-02-15 07:39:17.000000 PyMoosh-2.4/PyMoosh/data/solar.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)    11075 2023-02-15 07:39:17.000000 PyMoosh-2.4/PyMoosh/data/material_data.json
+-rw-rw-r--   0 moi       (1001) moi       (1001)     1240 2023-05-25 09:14:24.000000 PyMoosh-2.4/PyMoosh/__init__.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)   185623 2023-05-22 22:43:43.000000 PyMoosh-2.4/PyMoosh/core.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     4373 2023-04-06 22:06:11.000000 PyMoosh-2.4/PyMoosh/materials.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2661 2023-05-25 09:10:49.000000 PyMoosh-2.4/PyMoosh/optim.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)    34502 2022-09-23 09:03:42.000000 PyMoosh-2.4/LICENSE.txt
+drwxrwxr-x   0 moi       (1001) moi       (1001)        0 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/
+-rw-rw-r--   0 moi       (1001) moi       (1001)     3349 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/PKG-INFO
+-rw-rw-r--   0 moi       (1001) moi       (1001)      336 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/SOURCES.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        8 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/top_level.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)       23 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/requires.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)        1 2023-05-25 09:14:35.000000 PyMoosh-2.4/PyMoosh.egg-info/dependency_links.txt
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2282 2023-02-15 07:39:17.000000 PyMoosh-2.4/setup.py
+-rw-rw-r--   0 moi       (1001) moi       (1001)       34 2023-02-15 07:39:17.000000 PyMoosh-2.4/MANIFEST.in
+-rw-rw-r--   0 moi       (1001) moi       (1001)      107 2023-05-25 09:14:35.000000 PyMoosh-2.4/setup.cfg
+-rw-rw-r--   0 moi       (1001) moi       (1001)     2565 2023-02-15 07:39:17.000000 PyMoosh-2.4/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `PyMoosh-2.3/LICENSE.txt` & `PyMoosh-2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.3/PKG-INFO` & `PyMoosh-2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.3
+Version: 2.4
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.3/PyMoosh/__init__.py` & `PyMoosh-2.4/PyMoosh/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,14 @@
     in a multilayered structure. This makes PyMoosh unconditionally stable,
     allowing to explore even advanced properties of such multilayers,
     find poles and zeros of the scattering matrix (and thus guided modes),
     and many other things...
 
 """
 __name__ = 'PyMoosh'
-__version__ = '2.3'
-__date__ = "02/15/2023"   # MM/DD/YYY
+__version__ = '2.4'
+__date__ = "05/25/2023"   # MM/DD/YYY
 __author__ = 'Antoine Moreau'
 
 
 ## make accessible everything from `core` directly from the PyMoosh base package
 from PyMoosh.core import *
```

### Comparing `PyMoosh-2.3/PyMoosh/core.py` & `PyMoosh-2.4/PyMoosh/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
 import scipy.optimize as optim
 from math import *
 import sys
 import copy
+import matplotlib.pyplot as plt
+import itertools
 
 from PyMoosh.materials import *
 
 class Structure:
     """Each instance of Structure describes a multilayer completely.
     This includes the materials the multilayer is made of and the
     thickness of each layer.
@@ -57,74 +59,75 @@
         if verbose :
             print("List of materials:")
         for mat in materials:
             if issubclass(mat.__class__,Material):
                 materials_final.append(mat)
                 if verbose :
                     print("Object:",mat.__class__.__name__)
-            elif isinstance(mat,float) or isinstance(mat,complex):
-                new_mat = Material(mat)
+            elif mat.__class__.__name__ == 'function':
+                newmat = CustomFunction(mat)
                 materials_final.append(new_mat)
                 if verbose :
-                    print("Simple, non dispersive: epsilon=",mat)
-            elif isinstance(mat,int):
-                new_mat = Material(float(mat))
+                    print("Custom dispersive material. Epsilon=",mat.__name__,"(wavelength in nm)")
+            # no func / not iterable --> single value, convert to complex by default
+            elif not hasattr(mat, '__iter__'):
+                new_mat = Material(complex(mat))
                 materials_final.append(new_mat)
                 if verbose :
                     print("Simple, non dispersive: epsilon=",mat)
-            elif isinstance(mat,list):
+            # iterable: if list or similar --> magnetic
+            elif isinstance(mat,list) or isinstance(mat,tuple) or isinstance(mat,np.ndarray):
                 newmat = MagneticND(mat[0],mat[1])
                 materials_final.append(new_mat)
                 if verbose :
                     print("Magnetic, non dispersive: epsilon=", mat[0]," mu=",mat[1])
-            elif mat.__class__.__name__ == 'function':
-                newmat = CustomFunction(mat)
-                materials_final.append(new_mat)
-                if verbose :
-                    print("Custom dispersive material. Epsilon=",mat.__name__,"(wavelength in nm)")
+                if len(mat)>2:
+                    print(f'Warning: Magnetic material should have 2 values (epsilon / mu), but {len(mat)} were given.')
+            # iterable: string --> database material
             elif isinstance(mat,str):
                 # from file in shipped database
                 import pkgutil
                 f = pkgutil.get_data(__name__, "data/material_data.json")
                 f_str = f.decode(encoding='utf8')
                 database = json.loads(f_str)
                 if mat in database:
-                    if verbose :
-                        print("Database material:",mat)
                     material_data = database[mat]
                     model = material_data["model"]
 #                    match model:
 #                    case "ExpData":
                     if model == "ExpData":
                         wl=np.array(material_data["wavelength_list"])
                         epsilon = np.array(material_data["permittivities"])
                         if "permittivities_imag" in material_data:
                             epsilon = epsilon + 1j*np.array(material_data["permittivities_imag"])
-                        new_mat= ExpData(wl,epsilon)
+                        new_mat= ExpData(wl,epsilon, name=mat)
                         materials_final.append(new_mat)
 #                    case "BrendelBormann"
                     elif model == "BrendelBormann":
                         f0 = material_data["f0"]
                         Gamma0 = material_data["Gamma0"]
                         omega_p = material_data["omega_p"]
                         ff = material_data["f"]
                         gamma = material_data["Gamma"]
                         omega = material_data["omega"]
                         sigma = material_data["sigma"]
-                        new_mat = BrendelBormann(f0,Gamma0,omega_p,ff,gamma,omega,sigma)
+                        new_mat = BrendelBormann(f0,Gamma0,omega_p,ff,gamma,omega,sigma, name=mat)
                         materials_final.append(new_mat)
 #                    case "CustomFunction":
                     elif model == "CustomFunction":
                         permittivity = material_data["function"]
-                        new_mat = CustomFunction(authorized[permittivity])
+                        new_mat = CustomFunction(authorized[permittivity], name=mat)
                         materials_final.append(new_mat)
 #                    case _:
                     else:
                         print(model," not an existing model.")
                         #sys.exit()
+
+                    if verbose :
+                        print("Database material:",new_mat)
                 else:
                     print(mat,"Unknown material")
                     print("Known materials:\n", existing_materials())
                     #sys.exit()
             else:
                 print("Whhaaaaat ? That has nothing to do here :",mat)
 #                sys.exit( )
@@ -154,14 +157,81 @@
             material = self.materials[k]
             epsilon[k] = material.get_permittivity(wavelength)
             mu[k] = material.get_permeability(wavelength)
 
         return epsilon, mu
 
 
+    def plot_stack(struct, wavelength=None, lim_eps_colors=[1.5, 4]):
+        """plot layerstack
+
+        evaluate materials at given wavelength for labels
+        """
+        if wavelength is None:
+            wavelength=500.0
+
+        _mats = []
+        _mats_names = []
+        _index_diff = []
+        for i, mat in enumerate(np.array(struct.materials)[struct.layer_type]):
+            if hasattr(mat, 'name') and len(mat.name)>0:
+                # Named materials
+                _mats_names.append(mat.name)
+                _index_diff.append(i)
+            # Simply using the permittivity at a given wavelength (default is 500 nm)
+            _mats.append(mat.get_permittivity(wavelength))
+        _index_diff = np.array(_index_diff)
+
+        _thick = struct.thickness
+
+        ## give sub- and superstrate a finite thickness
+        if _thick[0] == 0: _thick[0] = 50
+        if _thick[-1] == 0: _thick[-1] = 50
+
+        ## reverse order so that top layer is on top in plot
+        _thick = _thick[::-1]
+        _mats = _mats[::-1]
+
+        ## define colors for layers of different ref.indices
+        if any(isinstance(x, str) for x in _mats):
+            colors = ['.3'] + [f'C{i}'for i in range(len(_thick)-2)] + ['.3']
+        else:
+            cmap = plt.cm.jet
+            colors = ['.3'] + [cmap((n.real-lim_eps_colors[0])/lim_eps_colors[1])
+                                       for n in _mats[1:-1]] + ['.3']
+
+        for i, di in enumerate(_thick):
+            d0 = np.sum(_thick[:i])
+            n = _mats[i]
+
+            if type(n) is not str:
+                n = str(np.round(n, 2))
+
+            if i < len(_thick)-1:
+                plt.axhline(d0+di, color='k', lw=1)
+            plt.axhspan(d0, d0+di, color=colors[i], alpha=0.5)
+
+            if i not in _index_diff:
+                text = f'eps={n}'
+            else:
+                text = f'mat={_mats_names[np.where(_index_diff==i)[0][0]]}'
+
+            if len(_thick)-1 > i >= 1:
+                plt.text(0.05, d0+di/2, text, ha='left', va='center',fontsize=8)
+                plt.text(0.95, d0+di/2, f'd={int(np.round(di))}nm', ha='right', va='center',fontsize=8)
+            else:
+                plt.text(0.1, d0+di/2, text, ha='left', va='center',fontsize=8)
+        plt.title(f'permittivities at wavelength = {wavelength}nm')
+        plt.ylabel('D (nm)')
+        plt.xticks([])
+        plt.show()
+
+
+
+
 class Beam:
     """ An object of the class contains all the parameters defining an incident
     beam. At initialization, a few messages will be displayed to inform the
     user.
 
     Args:
         wavelength (float): Wavelength in vacuum in nanometers
@@ -186,15 +256,15 @@
 
 class Window:
     """An object containing all the parameters defining the spatial domain
     which is represented.
 
     Args:
         width (float): width of the spatial domain (in nm)
-        beam_relative_position (float): relative position of the beam center
+        beam_relative_position (float): relative position of the source
         horizontal_pixel_size (float): size in nm of a pixel, horizontally
         vertical_pixel_size (float): size in nm of a pixel, vertically
 
     The number of pixel for each layer will be computed later, but the number of
     pixel horizontally is computed and stored in nx.
 
     The position of the center of the beam is automatically deduced from
@@ -256,15 +326,15 @@
     S[1, 1] = B[1, 1] + B[1, 0] * B[0, 1]  * t
     return (S)
 
 def absorption(struct, wavelength, incidence, polarization):
     """
     This function computes the percentage of the incoming energy
     that is absorbed in each layer when the structure is illuminated
-    by a plane wave.
+    by a plane wave.For now, uses the S matrix formalism
 
     Args:
         struct (Structure): belongs to the Structure class
         wavelength (float): wavelength of the incidence light (in nm)
         incidence (float): incidence angle in radians
         polarization (float): 0 for TE, 1 (or anything) for TM
 
@@ -276,142 +346,171 @@
         T (float): Transmittance (energie transmission)
     R and T are the energy coefficients (real quantities)
 
     .. warning: The transmission coefficients have a meaning only if the lower medium
     is lossless, or they have no true meaning.
 
     """
-    # The medium may be dispersive. The permittivity and permability of each
-    # layer has to be computed each time.
-    Epsilon, Mu = struct.polarizability(wavelength)
+    return absorption_S(struct, wavelength, incidence, polarization)
 
-    thickness = copy.deepcopy(struct.thickness)
-    # In order to ensure that the phase reference is at the beginning
-    # of the first layer.
-    thickness[0] = 0
+
+def field(struct, beam, window):
+    """Computes the electric (TE polarization) or magnetic (TM) field inside
+    a multilayered structure illuminated by a gaussian beam.
+
+    Args:
+        struct (Structure): description (materials,thicknesses)of the multilayer
+        beam (Beam): description of the incidence beam
+        window (Window): description of the simulation domain
+
+    Returns:
+        En (np.array): a matrix with the complex amplitude of the field
+
+    Afterwards the matrix may be used to represent either the modulus or the
+    real part of the field.
+    """
+
+    # Wavelength in vacuum.
+    lam = beam.wavelength
+    # Computation of all the permittivities/permeabilities
+    Epsilon, Mu = struct.polarizability(lam)
+    thickness = np.array(struct.thickness)
+    w = beam.waist
+    pol = beam.polarization
+    d = window.width
+    theta = beam.incidence
+    C = window.C
+    ny = np.floor(thickness / window.py)
+    nx = window.nx
     Type = struct.layer_type
-    # The boundary conditions will change when the polarization changes.
-    if polarization == 0:
+    print("Pixels vertically:", int(sum(ny)))
+
+    # Number of modes retained for the description of the field
+    # so that the last mode has an amplitude < 1e-3 - you may want
+    # to change it if the structure present reflexion coefficients
+    # that are subject to very swift changes with the angle of incidence.
+
+    nmod = int(np.floor(0.83660 * d / w))
+
+    # ----------- Do not touch this part ---------------
+    l = lam / d
+    w = w / d
+    thickness = thickness / d
+
+    if pol == 0:
         f = Mu
     else:
         f = Epsilon
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
-                1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
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
+    # Wavevector in vacuum, no dimension
+    k0 = 2 * pi / l
+    # Initialization of the field component
+    En = np.zeros((int(sum(ny)), int(nx)))
+    # Total number of layers
+    # g=Type.size-1
+    g = len(struct.layer_type) - 1
+    # Amplitude of the different modes
+    nmodvect = np.arange(-nmod, nmod + 1)
+    # First factor makes the gaussian beam, the second one the shift
+    # a constant phase is missing, it's just a change in the time origin.
+    X = np.exp(-w ** 2 * pi ** 2 * nmodvect ** 2) * np.exp(
+        -2 * 1j * pi * nmodvect * C)
 
-    # first S matrix
+    # Scattering matrix corresponding to no interface.
+    T = np.zeros((2 * g + 2, 2, 2), dtype=complex)
     T[0] = [[0, 1], [1, 0]]
-    gf = gamma / f[Type]
-    for k in range(g - 1):
-        # Layer scattering matrix
-        t = np.exp((1j) * gamma[k] * thickness[k])
-        T[2 * k + 1] = [[0, t], [t, 0]]
-        # Interface scattering matrix
-        b1 = gf[k]
-        b2 = gf[k + 1]
-        T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
-                                [2 * b1, b2 - b1]] / (b1 + b2))
-    t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
-    T[2 * g - 1] = [[0, t], [t, 0]]
-    # Once the scattering matrixes have been prepared, now let us combine them
-    H = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
-    A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
-    H[0] = T[2 * g - 1]
-    A[0] = T[0]
-    for k in range(len(T) - 2):
-        A[k + 1] = cascade(A[k], T[k + 1])
-        H[k + 1] = cascade(T[2 * g - 2 - k], H[k])
+    for nm in np.arange(2 * nmod + 1):
 
-    I = np.zeros(((2 * g, 2, 2)), dtype=complex)
-    for k in range(len(T) - 1):
-        I[k] = np.array(
-            [[A[k][1, 0], A[k][1, 1] * H[len(T) - k - 2][0, 1]],
-             [A[k][1, 0] * H[len(T) - k - 2][0, 0],
-              H[len(T) - k - 2][0, 1]]] / (
-                    1 - A[k][1, 1] * H[len(T) - k - 2][0, 0]))
-#        I[k][0, 0] = A[k][1, 0] / (1 - A[k][1, 1] * H[len(T) - 2 - k][0, 0])
-#        I[k][0, 1] = A[k][1, 1] * H[len(T) - 2 - k][0, 1] / (
-#                1 - A[k][1, 1] * H[len(T) - 2 - k][0, 0])
-#        I[k][1, 0] = A[k][1, 0] * H[len(T) - 2 - k][0, 0] / (
-#                1 - A[k][1, 1] * H[len(T) - 2 - k][0, 0])
-#        I[k][1, 1] = H[len(T) - 2 - k][0, 1] / (
-#                1 - A[k][1, 1] * H[len(T) - 2 - k][0, 0])
-    I[2 * g - 1][0, 0] = I[2 * g - 2][0, 0] * np.exp(
-        1j * gamma[g - 1] * thickness[g - 1])
-    I[2 * g - 1][0, 1] = I[2 * g - 2][0, 1] * np.exp(
-        1j * gamma[g - 1] * thickness[g - 1])
-    I[2 * g - 1][1, 0] = 0
-    I[2 * g - 1][1, 1] = 0
+        alpha = np.sqrt(Epsilon[Type[0]] * Mu[Type[0]]) * k0 * sin(
+            theta) + 2 * pi * (nm - nmod)
+        gamma = np.sqrt(
+            Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g + 1) * alpha ** 2)
 
-    w = 0
-    poynting = np.zeros(2 * g, dtype=complex)
-    if polarization == 0:  # TE
-        for k in range(2 * g):
-            poynting[k] = np.real((I[k][0, 0] + I[k][1, 0]) * np.conj(
-                (I[k][0, 0] - I[k][1, 0]) * gamma[w] / Mu[Type[w]])) * Mu[
-                              Type[0]] / (gamma[0])
-            w = w + 1 - np.mod(k + 1, 2)
-    else:  # TM
-        for k in range(2 * g):
-            poynting[k] = np.real((I[k][0, 0] - I[k][1, 0]) * np.conj(
-                (I[k][0, 0] + I[k][1, 0]) * gamma[w] / Epsilon[Type[w]]) *
-                                  Epsilon[Type[0]] / (gamma[0]))
-            w = w + 1 - np.mod(k + 1, 2)
-    # Absorption in each layer
-    tmp = abs(-np.diff(poynting))
-    # absorb=np.zeros(g,dtype=complex)
-    absorb = tmp[np.arange(0, 2 * g, 2)]
-    # reflection coefficient of the whole structure
-    r = A[len(A) - 1][0, 0]
-    # transmission coefficient of the whole structure
-    t = A[len(A) - 1][1, 0]
-    # Energy reflexion coefficient;
-    R = np.real(abs(r) ** 2)
-    # Energy transmission coefficient;
-    T = np.real(
-        abs(t) ** 2 * gamma[g - 1] * f[Type[0]] / (gamma[0] * f[Type[g - 1]]))
+        if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
+            gamma[0] = -gamma[0]
 
-    return absorb, r, t, R, T
+        if g > 2:
+            gamma[1:g - 1] = gamma[1:g - 1] * (
+                    1 - 2 * (np.imag(gamma[1:g - 1]) < 0))
+        if np.real(Epsilon[Type[g]]) < 0 and np.real(
+                Mu[Type[g]]) < 0 and np.real(
+            np.sqrt(Epsilon[Type[g]] * k0 ** 2 - alpha ** 2)) != 0:
+            gamma[g] = -np.sqrt(
+                Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
+        else:
+            gamma[g] = np.sqrt(
+                Epsilon[Type[g]] * Mu[Type[g]] * k0 ** 2 - alpha ** 2)
 
+        gf = gamma / f[Type]
+        for k in range(g):
+            t = np.exp(1j * gamma[k] * thickness[k])
+            T[2 * k + 1] = np.array([[0, t], [t, 0]])
+            b1 = gf[k]
+            b2 = gf[k + 1]
+            T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
+                                    [2 * b1, b2 - b1]]) / (b1 + b2)
+        t = np.exp(1j * gamma[g] * thickness[g])
+        T[2 * g + 1] = np.array([[0, t], [t, 0]])
 
-def field(struct, beam, window):
+        H = np.zeros((len(T) - 1, 2, 2), dtype=complex)
+        A = np.zeros((len(T) - 1, 2, 2), dtype=complex)
+
+        H[0] = T[2 * g + 1]
+        A[0] = T[0]
+
+        for k in range(len(T) - 2):
+            A[k + 1] = cascade(A[k], T[k + 1])
+            H[k + 1] = cascade(T[len(T) - k - 2], H[k])
+
+        I = np.zeros((len(T), 2, 2), dtype=complex)
+        for k in range(len(T) - 1):
+            I[k] = np.array(
+                [[A[k][1, 0], A[k][1, 1] * H[len(T) - k - 2][0, 1]],
+                 [A[k][1, 0] * H[len(T) - k - 2][0, 0],
+                  H[len(T) - k - 2][0, 1]]] / (
+                        1 - A[k][1, 1] * H[len(T) - k - 2][0, 0]))
+
+        h = 0
+        t = 0
+
+
+
+        E = np.zeros((int(np.sum(ny)), 1), dtype=complex)
+        for k in range(g + 1):
+            for m in range(int(ny[k])):
+                h = h + float(thickness[k]) / ny[k]
+                #The expression for the field used here is based on the assumption
+                # that the structure is illuminated from above only, with an Amplitude
+                # of 1 for the incident wave. If you want only the reflected
+                # field, take off the second term.
+                E[t, 0] = I[2 * k][0, 0] * np.exp(1j * gamma[k] * h) + \
+                          I[2 * k + 1][1, 0] * np.exp(
+                    1j * gamma[k] * (thickness[k] - h))
+                t += 1
+            h = 0
+        E = E * np.exp(1j * alpha * np.arange(0, nx) / nx)
+        En = En + X[int(nm)] * E
+
+    return En
+
+def fields(struct, beam, window):
     """Computes the electric (TE polarization) or magnetic (TM) field inside
-    a multilayered structure illuminated by a gaussian beam.
+    a multilayered structure illuminated by a gaussian beam, and uses them
+    to compute the rest of the fields (Hx,Hz in TE polarization/Ex,Ez in TM).
+    To be precise, the derived fields need to be divided by omega*µ0 in TE
+    and omega*epsilon_0 in TM. There a missing - sign in TM, too.
 
     Args:
         struct (Structure): description (materials,thicknesses)of the multilayer
         beam (Beam): description of the incidence beam
         window (Window): description of the simulation domain
 
     Returns:
         En (np.array): a matrix with the complex amplitude of the field
+        Hxn (np.array): a matrix with the complex amplitude of Hx/Ex
+        Hzn (np.array): a matrix with the complex amplitude of Hz/Ez
 
     Afterwards the matrix may be used to represent either the modulus or the
     real part of the field.
     """
 
     # Wavelength in vacuum.
     lam = beam.wavelength
@@ -444,14 +543,16 @@
         f = Mu
     else:
         f = Epsilon
     # Wavevector in vacuum, no dimension
     k0 = 2 * pi / l
     # Initialization of the field component
     En = np.zeros((int(sum(ny)), int(nx)))
+    Hxn = np.zeros((int(sum(ny)), int(nx)))
+    Hzn = np.zeros((int(sum(ny)), int(nx)))
     # Total number of layers
     # g=Type.size-1
     g = len(struct.layer_type) - 1
     # Amplitude of the different modes
     nmodvect = np.arange(-nmod, nmod + 1)
     # First factor makes the gaussian beam, the second one the shift
     # a constant phase is missing, it's just a change in the time origin.
@@ -511,33 +612,43 @@
                  [A[k][1, 0] * H[len(T) - k - 2][0, 0],
                   H[len(T) - k - 2][0, 1]]] / (
                         1 - A[k][1, 1] * H[len(T) - k - 2][0, 0]))
 
         h = 0
         t = 0
 
-
-
         E = np.zeros((int(np.sum(ny)), 1), dtype=complex)
+        Hx = np.zeros((int(np.sum(ny)), 1), dtype=complex)
+        Hz = np.zeros((int(np.sum(ny)), 1), dtype=complex)
         for k in range(g + 1):
             for m in range(int(ny[k])):
                 h = h + float(thickness[k]) / ny[k]
                 #The expression for the field used here is based on the assumption
                 # that the structure is illuminated from above only, with an Amplitude
                 # of 1 for the incident wave. If you want only the reflected
                 # field, take off the second term.
                 E[t, 0] = I[2 * k][0, 0] * np.exp(1j * gamma[k] * h) + \
-                          I[2 * k + 1][1, 0] * np.exp(
+                          I[2 * k + 1][1, 0] * np.exp(\
                     1j * gamma[k] * (thickness[k] - h))
+                Hx[t, 0] = - gf[k] *(I[2 * k][0, 0] * np.exp(1j * gamma[k] * h) - \
+                        I[2 * k + 1][1, 0] * np.exp(\
+                        1j * gamma[k] * (thickness[k] - h)))
+                Hz[t,0] = alpha * E[t,0] / f[Type[k]]
                 t += 1
+
             h = 0
         E = E * np.exp(1j * alpha * np.arange(0, nx) / nx)
+        Hx = Hx * np.exp(1j * alpha * np.arange(0, nx) / nx)
+        Hz = Hz * np.exp(1j * alpha * np.arange(0, nx) / nx)
+
         En = En + X[int(nm)] * E
+        Hxn = Hxn + X[int(nm)] * Hx
+        Hzn = Hzn + X[int(nm)] * Hz
 
-    return En
+    return En,Hxn,Hzn
 
 
 def Angular(structure, wavelength, polarization, theta_min, theta_max,
             n_points):
     """Represents the reflexion coefficient (reflectance and phase) for a
     multilayered structure. This is an automated call to the :coefficient:
     function making the angle of incidence vary.
@@ -832,42 +943,156 @@
         if (len(modes)==0):
             modes.append(solution)
         elif (min(abs(modes-solution))>1e-5*k_0):
             modes.append(solution)
 
     return modes
 
-def muller(starting_points,tol,step_max,struct,wl,pol):
+def follow_guided_modes(struct, wavelength_list, polarization,
+                        neff_min, neff_max, format="n", initial_points=40, plot=True):
 
-    k_0 = 2* np.pi / wl
-    x=np.array(starting_points) * k_0
-    f=np.array([dispersion(x[0],struct,wl,pol),dispersion(x[1],struct,wl,pol),dispersion(x[2],struct,wl,pol)])
-    step=0
-    print(x,"\n step :",step,"\n",f)
-
-    while (f[2]>tol) and (step<step_max):
-        #print(x,"\n step :",step,"\n valeur de f", f[2] )
-        q=(x[2]-x[1])/(x[1]-x[0])
-        A = q * f[2] - q*(1+ q) * f[1] + q * q * f[0]
-        B = (2*q+1) * f[2] - (1+q)**2 * f[1] + q*q * f[0]
-        C = (1+q) * f[2]
-        temp = np.sqrt(B*B-4*A*C)
-        D = max([abs(B+temp),abs(B-temp)])
-        new_x = x[2]-(x[2]-x[1]) * 2 * C / D
-        #new_x= x[2] - 2*C/D
-        x[0]=x[1]
-        x[1]=x[2]
-        x[2]=new_x
-        f[0]=f[1]
-        f[1]=f[2]
-        f[2]=dispersion(new_x,struct,wl,pol)
-        print("New values:",step,new_x/k_0,f[2])
-        step += 1
+    """ This function explores the complex plane, looking for zeros of the
+    dispersion relation. It does so by launching a steepest descent for a number
+    `initial_points` of points on the real axis between neff_min and neff_max.
 
-    return x[2]/k_0
+
+    Args:
+        struct (Structure): object describing the multilayer
+        wavelength_list (float): wavelengths in nm
+        polarization: 0 for TE, 1 for TM
+        neff_min: minimum value of the effective index expected
+        neff_max: maximum value of the effective index expected
+        format: index output format, n for effective index, wav for wavelength, k for wavevector
+
+    Returns:
+        modes (list of list, complex): complex effective indices identified as
+                            solutions of the dispersion relation for all wavelengths.
+
+    """
+
+    if not format in ["n", "k", "wav"]:
+        print("Unknown index format: accepted values or n, k and wav")
+
+    tolerance = 1e-10
+#    initial_points = 40
+    wavelength = wavelength_list[0]
+    k_0 = 2*np.pi/wavelength
+    neff_start = np.linspace(neff_min, neff_max, initial_points, dtype=complex)
+
+    # Finding the first modes, that we will then follow
+    first_modes = []
+    for neff in neff_start:
+        solution = steepest(neff, tolerance, 1000, struct, wavelength, polarization)
+#        print(solution)
+        if (len(first_modes) == 0):
+            first_modes.append(solution)
+        elif (min(abs(first_modes-solution))>1e-5*k_0):
+            first_modes.append(solution)
+    modes = [first_modes]
+
+    # Following these modes for all the wavelength range
+    for i in range(1, len(wavelength_list)):
+        wavelength = wavelength_list[i]
+        k_0 = 2*np.pi/wavelength
+        neff_start = np.array(modes[-1]).flatten()
+        new_modes = []
+        if (len(neff_start)>1):
+            for neff in neff_start:
+                solution = steepest(neff, tolerance, 1000, struct, wavelength, polarization)
+                if (len(new_modes) == 0):
+                    new_modes.append(solution)
+                elif (min(abs(new_modes-solution))>1e-5*k_0):
+                    new_modes.append(solution)
+        else:
+            neff = neff_start
+            solution = steepest(neff, tolerance, 1000, struct, wavelength, polarization)
+            if (len(new_modes) == 0):
+                new_modes.append(solution)
+            elif (min(abs(new_modes-solution))>1e-5*k_0):
+                new_modes.append(solution)
+
+        modes.append(np.array(new_modes).flatten())
+
+    if (format == "k"):
+        for i in range(len(modes)):
+            modes[i] = np.array(modes[i]) * 2*np.pi/wavelength_list[i]
+    elif (format == "wav"):
+        for i in range(len(modes)):
+            modes[i] = wavelength_list[i] / np.array(modes[i])
+
+    mode_filled = np.array(list(itertools.zip_longest(*modes, fillvalue=0)))
+    mode_filled = mode_filled.T
+
+    # The following bit links modes together, for ease of use
+    # However, it only follows the modes that exist at the smallest wavelength
+    follow_modes = []
+    nb_mode = np.shape(mode_filled)[1]
+    for shift in range(nb_mode // 2):
+        index = nb_mode // 2 + shift # starting with the middle mode because it's the usually the most stable one
+        mode = [mode_filled[0, index]]
+        i = 1
+        while (i < len(mode_filled) and index >= 0 and index < nb_mode):
+            res = np.abs(mode[-1] - mode_filled[i, index-1:index+2])
+            if (len(res) == 3):
+                a, b, c = res
+                if (a < b and a < c):
+                    index = index - 1
+                elif (c < a and c < b):
+                    index = index + 1
+                mode.append(mode_filled[i, index])
+            else:
+                break
+            i += 1
+        follow_modes.append(mode)
+
+        if shift > 0:
+            index = nb_mode // 2 - shift
+            mode = [mode_filled[0, index]]
+            i = 1
+            while (i < len(mode_filled) and index >= 0 and index < nb_mode):
+                res = np.abs(mode[-1] - mode_filled[i, index-1:index+2])
+                if (len(res) == 3):
+                    a, b, c = res
+                    if (a < b and a < c):
+                        index = index - 1
+                    elif (c < a and c < b):
+                        index = index + 1
+                    mode.append(mode_filled[i, index])
+                else:
+                    break
+                i += 1
+            follow_modes.append(mode)
+
+    follow_modes = np.array(list(itertools.zip_longest(*follow_modes, fillvalue=0)))
+    # Because we are following modes, we add 0 when the modes disappear
+
+    if (plot):
+        modes_no_zero = []
+        for i in range(np.shape(follow_modes)[1]):
+            j = 0
+            while(j < np.shape(follow_modes)[0] and follow_modes[j, i] != 0):
+                j += 1
+            modes_no_zero.append(follow_modes[:j-1, i])
+
+        for i in range(len(modes_no_zero)):
+            if (format == "n"):
+                plt.plot(wavelength_list[:len(modes_no_zero[i])], wavelength_list[:len(modes_no_zero[i])]/modes_no_zero[i])
+                plt.xlabel("Wavelength in vacuum (nm)")
+                plt.ylabel("Mode index (nm)")
+            elif (format == "wav"):
+                plt.plot(wavelength_list[:len(modes_no_zero[i])], modes_no_zero[i])
+                plt.xlabel("Wavelength in vacuum (nm)")
+                plt.ylabel("Mode index (nm)")
+            elif (format == "k"):
+                plt.plot(2*np.pi/wavelength_list[:len(modes_no_zero[i])], modes_no_zero[i])
+                plt.xlabel("Wavevector in vacuum (nm-1)")
+                plt.ylabel("Mode index (nm-1)")
+        plt.show()
+
+    return modes, follow_modes
 
 def steepest(start,tol,step_max,struct,wl,pol):
     """ Steepest descent to find a zero of the `dispersion`
     function. The advantage of looking for a zero is that you
     know when the algorithm can stop (when the value of the function
     is smaller than `tol`).
 
@@ -884,15 +1109,15 @@
 
         (float) : last effective index reached at the end of the descent
 
     """
 
 
     k_0 = 2 * np.pi / wl
-    z=start*k_0
+    z = start*k_0
     delta = abs(z) * 0.001
     dz= 0.01 * delta
     step = 0
     current = dispersion(z,struct,wl,pol)
 
     while (current > tol) and (step < step_max):
 
@@ -904,16 +1129,18 @@
 #        -dispersion(z-1j*dz,struct,wl,pol))
         -current)
         )/(dz)
 
         if abs(grad)!=0 :
             z_new = z - delta * grad / abs(grad)
         else:
-            print("Time to get out of here ! Gradient is null")
-            step = step_max
+            # We have a finishing condition not linked to the gradient
+            # So if we meet a gradient of 0, we just divide the step by two
+            delta = delta/2.
+            z_new = z
 
         value_new = dispersion(z_new,struct,wl,pol)
         if (value_new > current):
             # The path not taken
             delta = delta / 2.
             dz = dz / 2.
         else:
@@ -1020,23 +1247,24 @@
         h=0
 
     x = np.linspace(0,sum(thickness),len(E))
     return x,E
 
 def Green(struct,window,lam,source_interface):
 
-    """Computes the electric (TE polarization) or magnetic (TM) field inside
+    """Computes the electric (TE polarization) field inside
     a multilayered structure illuminated by punctual source placed inside
     the structure.
 
     Args:
         struct (Structure): description (materials,thicknesses)of the multilayer
         window (Window): description of the simulation domain
         lam (float): wavelength in vacuum
-        source_interface (int):
+        source_interface (int): # of the interface where the source is located.
+                                The medium should be the same on both sides.
     Returns:
         En (np.array): a matrix with the complex amplitude of the field
 
     Afterwards the matrix may be used to represent either the modulus or the
     real part of the field.
     """
 
@@ -1062,19 +1290,19 @@
         return 0
 
     # Number of modes retained for the description of the field
     # so that the last mode has an amplitude < 1e-3 - you may want
     # to change it if the structure present reflexion coefficients
     # that are subject to very swift changes with the angle of incidence.
 
-    nmod = int(np.floor(0.83660 * d / w))
+    #nmod = int(np.floor(0.83660 * d / w))
+    nmod = 100
 
     # ----------- Do not touch this part ---------------
     l = lam / d
-    w = w / d
     thickness = thickness / d
 
     if pol == 0:
         f = Mu
     else:
         f = Epsilon
     # Wavevector in vacuum, no dimension
@@ -1085,15 +1313,15 @@
     # g=Type.size-1
     g = len(struct.layer_type) - 1
 
     # Scattering matrix corresponding to no interface.
     T = np.zeros((2 * g + 2, 2, 2), dtype=complex)
     T[0] = [[0, 1], [1, 0]]
     for nm in np.arange(2 * nmod + 1):
-
+        # horizontal wavevector
         alpha = 2 * pi * (nm - nmod)
         gamma = np.sqrt(
             Epsilon[Type] * Mu[Type] * k0 ** 2 - np.ones(g + 1) * alpha ** 2)
 
         if np.real(Epsilon[Type[0]]) < 0 and np.real(Mu[Type[0]]) < 0:
             gamma[0] = -gamma[0]
 
@@ -1116,55 +1344,104 @@
             b1 = gf[k]
             b2 = gf[k + 1]
             T[2 * k + 2] = np.array([[b1 - b2, 2 * b2],
                                      [2 * b1, b2 - b1]]) / (b1 + b2)
         t = np.exp(1j * gamma[g] * thickness[g])
         T[2 * g + 1] = np.array([[0, t], [t, 0]])
 
+        Ampl = np.zeros((2 * g + 2, 2), dtype=complex)
+
+# -----------------------------> Above the source
+# calculation of the scattering matrices above the source (*_up)
         H_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
         A_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
 
-        H_up[0] = T[0]
+        # T[2*source_interface] should be a neutral matrix for cascading
+        # if the two media are the same on each side of the source.
+
+        H_up[0] = T[2*source_interface]
         A_up[0] = T[0]
 
         for k in range(2*source_interface-1):
-            A_up[k + 1] = cascade(A[k], T[k + 1])
-            H_up[k + 1] = cascade(T[2*source_interface-1-k], H[k])
+            A_up[k + 1] = cascade(A_up[k], T[k + 1])
+            H_up[k + 1] = cascade(T[2*source_interface-1-k], H_up[k])
 
-        I_up = np.zeros((len(T), 2, 2), dtype=complex)
+        I_up = np.zeros((2*source_interface, 2, 2), dtype=complex)
         for k in range(2*source_interface-1):
             I_up[k] = np.array(
-                [[A[k][1, 0], A[k][1, 1] * H[len(T) - k - 2][0, 1]],
-                 [A[k][1, 0] * H[len(T) - k - 2][0, 0],
-                  H[len(T) - k - 2][0, 1]]] / (
-                        1 - A[k][1, 1] * H[len(T) - k - 2][0, 0]))
+                [[A_up[k][1, 0], A_up[k][1, 1] * H_up[2*source_interface-1-k][0, 1]],
+                 [A_up[k][1, 0] * H_up[2*source_interface-1-k][0, 0],
+                  H_up[2*source_interface-1-k][0, 1]]] / (
+                        1 - A_up[k][1, 1] * H_up[2*source_interface-1-k][0, 0]))
+
+# ----------------------------> Below the source
+# Calculation of the scattering matrices below the source (*_d)
+
+        H_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
+        A_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
+
+        H_d[0] = T[0]
+        A_d[0] = T[0]
+
+        for k in range(2*g+1-2*source_interface):
+            A_d[k + 1] = cascade(A_d[k], T[k + 1])
+            H_d[k + 1] = cascade(T[2*g+1-k], H_d[k])
+
+        I_d = np.zeros((-2*source_interface+2*g+2, 2, 2), dtype=complex)
+        for k in range(2*g+1-2*source_interface):
+            I_d[k] = np.array(
+                [[A_d[k][1, 0], A_d[k][1, 1] * H_d[2*(g-source_interface)+1-k][0, 1]],
+                 [A_d[k][1, 0] * H_d[2*(g-source_interface)+1-k][0, 0],
+                  H_d[2*(g-source_interface)+1-k][0, 1]]] / (
+                        1 - A_d[k][1, 1] * H_d[2*(g-source_interface)+1-k][0, 0]))
+
+# >>> Inside the layer containing the source <<<
+
+        r_up = A_up[2*source_interface-1][1,1]
+        r_d  = H_d[2*g+1-2*source_interface][0,0]
+        ex=np.exp(1j*alpha*window.C); # Multiply by -omega µ_0
+        M = ex / (1 - r_up + (1 + r_up) * (1- r_d) / (1 + r_d)) \
+        / gamma[source_interface]
+        D = ex / (1 - r_d + (1-r_up)/(1-r_up)*(1+r_d)) \
+        / gamma[source_interface]
+
+# Starting with the intermediary matrices, compute the right coefficients
+
+        Ampl = np.zeros(2*g+2, dtype=complex)
+        #Ampl[2*source_interface-1] = M
+        #Ampl[2*source_interface] = D
+
+        for k in range(source_interface):
+            Ampl[2*k] = I_up[2*k][1,1] * M
+            Ampl[2*k+1] = I_up[2*k+1][0,1] * M
+
+        for k in range(source_interface,g+1):
+            Ampl[2*k] = I_d[2*(k-source_interface)][1,0] * D
+            Ampl[2*k+1] = I_d[2*(k-source_interface)+1][0,0] * D
+
+# >>> Calculation of the fields <<<
 
         h = 0
         t = 0
-
-
         E = np.zeros((int(np.sum(ny)), 1), dtype=complex)
 
         for k in range(g + 1):
             for m in range(int(ny[k])):
-                h = h + float(thickness[k]) / ny[k]
-                #The expression for the field used here is based on the assumption
-                # that the structure is illuminated from above only, with an Amplitude
-                # of 1 for the incident wave. If you want only the reflected
-                # field, take off the second term.
-                E[t, 0] = I[2 * k][0, 0] * np.exp(1j * gamma[k] * h) + \
-                          I[2 * k + 1][1, 0] * np.exp(
-                    1j * gamma[k] * (thickness[k] - h))
-                t += 1
+                 h = h + float(thickness[k]) / ny[k]
+
+                 E[t, 0] = Ampl[2 * k + 1] * np.exp(1j * gamma[k] * h) + \
+                           Ampl[2 * k] * np.exp( \
+                     1j * gamma[k] * (thickness[k] - h))
+                 t += 1
             h = 0
         E = E * np.exp(1j * alpha * np.arange(0, nx) / nx)
         En = En + E
 
     return En
-
+#    return r_up,r_d
 
 def coefficient(struct, wavelength, incidence, polarization):
     """
         Wrapper function to comput reflection and transmission coefficients
         with various methods.
         (and retrocompatibility)
     """
@@ -2120,7 +2397,314 @@
         r_pas, t_pas, R_pas, T_pas = function(struct, wavelength, incidence, polarization)
         dr[i+len(base_thickness)-2] = (r_pas - r)/pas
         dR[i+len(base_thickness)-2] = (R_pas - R)/pas
         dt[i+len(base_thickness)-2] = (t_pas - t)/pas
         dT[i+len(base_thickness)-2] = (T_pas - T)/pas
 
     return dr, dt, dR, dT
+
+
+
+def absorption_S(struct, wavelength, incidence, polarization, layers=[]):
+    """
+    This function computes the percentage of the incoming energy
+    that is absorbed in each layer when the structure is illuminated
+    by a plane wave.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+        layers (list of int): which layers we must compute absorption in
+
+    returns:
+        absorb (numpy array): absorption in each layer
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+
+    """
+    # The medium may be dispersive. The permittivity and permability of each
+    # layer has to be computed each time.
+    Epsilon, Mu = struct.polarizability(wavelength)
+
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
+                1 - 2 * (np.imag(gamma[1:g - 2]) < 0))
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
+                                [2 * b1, b2 - b1]] / (b1 + b2))
+    t = np.exp((1j) * gamma[g - 1] * thickness[g - 1])
+    T[2 * g - 1] = [[0, t], [t, 0]]
+    # Once the scattering matrixes have been prepared, now let us combine them
+    H = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
+    A = np.zeros(((2 * g - 1, 2, 2)), dtype=complex)
+    H[0] = T[2 * g - 1]
+    A[0] = T[0]
+    for k in range(len(T) - 2):
+        A[k + 1] = cascade(A[k], T[k + 1])
+        H[k + 1] = cascade(T[2 * g - 2 - k], H[k])
+
+
+    if len(layers) == 0:
+        I = np.zeros(((2 * g, 2, 2)), dtype=complex)
+        for k in range(len(T) - 1):
+            I[k] = np.array(
+                [[A[k][1, 0], A[k][1, 1] * H[len(T) - k - 2][0, 1]],
+                 [A[k][1, 0] * H[len(T) - k - 2][0, 0],
+                  H[len(T) - k - 2][0, 1]]] / (
+                        1 - A[k][1, 1] * H[len(T) - k - 2][0, 0]))
+
+        I[2 * g - 1][0, 0] = I[2 * g - 2][0, 0] * np.exp(
+            1j * gamma[g - 1] * thickness[g - 1])
+        I[2 * g - 1][0, 1] = I[2 * g - 2][0, 1] * np.exp(
+            1j * gamma[g - 1] * thickness[g - 1])
+        I[2 * g - 1][1, 0] = 0
+        I[2 * g - 1][1, 1] = 0
+
+        poynting = np.zeros(2 * g, dtype=complex)
+        if polarization == 0:  # TE
+            for k in range(2 * g):
+                poynting[k] = np.real((I[k][0, 0] + I[k][1, 0]) * np.conj(
+                    (I[k][0, 0] - I[k][1, 0]) * gf[k//2] / gf[0]))
+        else:  # TM
+            for k in range(2 * g):
+                poynting[k] = np.real((I[k][0, 0] - I[k][1, 0]) * np.conj(
+                    (I[k][0, 0] + I[k][1, 0])) * gf[k//2] / gf[0])
+        # Absorption in each layer
+
+        tmp = abs(-np.diff(poynting))
+        # absorb=np.zeros(g,dtype=complex)
+        absorb = tmp[np.arange(0, 2 * g, 2)]
+
+    else:
+        # Specific layers are given for the absorption
+
+        nb_lay = len(layers)
+        layers = np.sort(layers)
+        I = np.zeros(((2 * nb_lay, 2, 2)), dtype=complex)
+        i = 0
+        for k in layers:
+            if (k != g-1):
+                I[2*i] = np.array(
+                    [[A[2*k][1, 0], A[2*k][1, 1] * H[len(T) - 2*k - 2][0, 1]],
+                     [A[2*k][1, 0] * H[len(T) - 2*k - 2][0, 0], H[len(T) - 2*k - 2][0, 1]]]
+                     / (1 - A[2*k][1, 1] * H[len(T) - 2*k - 2][0, 0]))
+                I[2*i+1] = np.array(
+                    [[A[2*k+1][1, 0], A[2*k+1][1, 1] * H[len(T) - 2*k - 3][0, 1]],
+                     [A[2*k+1][1, 0] * H[len(T) - 2*k - 3][0, 0],H[len(T) - 2*k - 3][0, 1]]]
+                     / (1 - A[2*k+1][1, 1] * H[len(T) - 2*k - 3][0, 0]))
+                i += 1
+        if g-1 in layers:
+            I[-2] = np.array(
+                [[A[2*g-2][1, 0], A[2*g-2][1, 1] * H[len(T) - 2*g][0, 1]],
+                 [A[2*g-2][1, 0] * H[len(T) - 2*g][0, 0],
+                  H[len(T) - 2*g][0, 1]]] / (
+                        1 - A[2*g-2][1, 1] * H[len(T) - 2*g][0, 0]))
+            I[-1][0, 0] = I[-2][0, 0] * np.exp(1j * gamma[g-1] * thickness[g-1])
+            I[-1][0, 1] = I[-2][0, 1] * np.exp(1j * gamma[g-1] * thickness[g-1])
+            I[-1][1, 0] = 0
+            I[-1][1, 1] = 0
+
+        poynting = np.zeros(2 * nb_lay, dtype=complex)
+        if polarization == 0:  # TE
+            for k in range(2*nb_lay):
+                poynting[k] = np.real((I[k][0, 0] + I[k][1, 0]) * np.conj(
+                    (I[k][0, 0] - I[k][1, 0]) * gf[layers[k//2]] / gf[0]))
+        else:  # TM
+            for k in range(2*nb_lay):
+                poynting[k] = np.real((I[k][0, 0] + I[k][1, 0]) * np.conj(
+                    (I[k][0, 0] - I[k][1, 0]) * gf[layers[k//2]]) / gf[0])
+        # Absorption in each layer
+
+        tmp = abs(-np.diff(poynting))
+        # absorb = abs(poynting[1::]-poynting[::-1])[::2]
+        # absorb=np.zeros(g,dtype=complex)
+        absorb = tmp[np.arange(0, 2 * nb_lay, 2)]
+
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
+    return absorb, r, t, R, T
+
+
+def absorption_A(struct, wavelength, incidence, polarization):
+    """
+    This function computes the percentage of the incoming energy
+    that is absorbed in each layer when the structure is illuminated
+    by a plane wave.
+
+    Args:
+        struct (Structure): belongs to the Structure class
+        wavelength (float): wavelength of the incidence light (in nm)
+        incidence (float): incidence angle in radians
+        polarization (float): 0 for TE, 1 (or anything) for TM
+
+    returns:
+        absorb (numpy array): absorption in each layer
+        r (complex): reflection coefficient, phase origin at first interface
+        t (complex): transmission coefficient
+        R (float): Reflectance (energy reflection)
+        T (float): Transmittance (energie transmission)
+    R and T are the energy coefficients (real quantities)
+
+    .. warning: The transmission coefficients have a meaning only if the lower medium
+    is lossless, or they have no true meaning.
+
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
+    A = np.empty((T.shape[0], 2,2), dtype=complex)
+    A[0] = T[0]
+    for i in range(1, T.shape[0]):
+        A[i] = T[i] @ A[i-1]
+
+    a = A[-1][0, 0]
+    b = A[-1][0, 1]
+    c = A[-1][1, 0]
+    d = A[-1][1, 1]
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
+    I = np.zeros(((A.shape[0]+1, 2)), dtype=complex)
+
+    for k in range(A.shape[0]):
+        I[k,0] = A[k][0, 0] * (r+1) + A[k][0, 1]*(1.j*gf[0]*(r-1))
+        I[k,1] = A[k][1, 0] * (r+1) + A[k][1, 1]*(1.j*gf[0]*(r-1))
+             # Contains Ey and dzEy in layer k
+    I[-1] = [t, -1.j*gf[-1]*t]
+
+    w = 0
+    poynting = np.zeros(A.shape[0]+1, dtype=complex)
+    if polarization == 0:  # TE
+        for k in range(A.shape[0]+1):
+            poynting[k] = np.real(-1.j * I[k, 0] * np.conj(I[k, 1]) / gf[0])
+    else:  # TM
+        for k in range(A.shape[0]+1):
+            poynting[k] = np.real(1.j * np.conj(I[k, 0]) * I[k, 1] / gf[0])
+    # Absorption in each layer
+    absorb = np.concatenate(([0],abs(-np.diff(poynting))))
+    # First layer is always supposed non absorbing
+
+    return absorb, r, t, R, T
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PyMoosh-2.3/PyMoosh/data/material_data.json` & `PyMoosh-2.4/PyMoosh/data/material_data.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.3/PyMoosh/data/solar.json` & `PyMoosh-2.4/PyMoosh/data/solar.json`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.3/PyMoosh/materials.py` & `PyMoosh-2.4/PyMoosh/materials.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,48 +2,63 @@
 import numpy as np
 from scipy.special import wofz
 import json
 #from enum import Enum
 
 class Material:
 
-    def __init__(self,permittivity):
+    def __init__(self,permittivity, name=""):
         self.permittivity = permittivity
+        self.name = name
 
     def __str__(self):
+        if (len(self.name) > 1):
+            return f"{self.name}, perm: {self.permittivity}"
         return str(self.permittivity)
 
     def get_permittivity(self,wavelength):
         return self.permittivity
 
     def get_permeability(self,wavelength):
         return 1.0
 
 class CustomFunction(Material):
 
-    def __init__(self,permittivity_function):
+    def __init__(self,permittivity_function, name=""):
         self.permittivity_function = permittivity_function
+        self.name = name
+
+    def __str__(self):
+        if (len(self.name) > 1):
+            return f"{self.name}, model: custom function, see material_data.json"
+        return "Custom function for permittivity"
 
     def get_permittivity(self,wavelength):
         return self.permittivity_function(wavelength)
 
 class ExpData(Material):
     """
     Class of materials defined by their permittivity measured for
     well defined values of the wavelength in vacuum. We make asin
     interpolation to get the most accurate value of the permittivity.
     Two lists are thus expected:
     - wavelength_list
     - permittivities (potentially complex)
     """
 
-    def __init__(self, wavelength_list,permittivities):
+    def __init__(self, wavelength_list,permittivities, name=""):
 
-        self.wavelength_list = np.array(wavelength_list, dtype = float)
-        self.permittivities  = np.array(permittivities, dtype = complex)
+        self.wavelength_list = np.array(wavelength_list, dtype=float)
+        self.permittivities  = np.array(permittivities, dtype=complex)
+        self.name = name
+
+    def __str__(self):
+        if (len(self.name) > 1):
+            return f"{self.name}, model: Exp Data"
+        return "Experimental Data for database material"
 
     def get_permittivity(self, wavelength):
         return np.interp(wavelength, self.wavelength_list, self.permittivities)
 
 class MagneticND(Material):
 
     """
@@ -60,22 +75,29 @@
 
 
 class BrendelBormann(Material):
     """
     Material described using a Brendel Bormann model for a metal.
     """
 
-    def __init__(self, f0,gamma0,omega_p,f,gamma,omega,sigma) -> None:
+    def __init__(self, f0,gamma0,omega_p,f,gamma,omega,sigma, name="") -> None:
         self.f0 = f0
         self.Gamma0 = gamma0
         self.omega_p = omega_p
         self.f = np.array(f)
         self.gamma = np.array(gamma)
         self.omega = np.array(omega)
         self.sigma = np.array(sigma)
+        self.name = name
+
+
+    def __str__(self):
+        if (len(self.name) > 1):
+            return f"{self.name}, model: Brendel Bormann"
+        return "Brendel Bormann model for Database material"
 
     def get_permittivity(self, wavelength):
         w = 6.62606957e-25 * 299792458 / 1.602176565e-19 / wavelength
         a = np.sqrt(w * (w + 1j * self.gamma))
         x = (a - self.omega) / (np.sqrt(2) * self.sigma)
         y = (a + self.omega) / (np.sqrt(2) * self.sigma)
         # Polarizability due to bound electrons
```

### Comparing `PyMoosh-2.3/PyMoosh.egg-info/PKG-INFO` & `PyMoosh-2.4/PyMoosh.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: PyMoosh
-Version: 2.3
+Version: 2.4
 Summary: A scattering matrix formalism to solve Maxwell's equations in a multilayered structure.
 Home-page: https://github.com/AnMoreau/PyMoosh
 Author: Antoine Moreau
 Author-email: antoine.moreau@uca.fr
 License: GPLv3+
 Description: # PyMoosh
```

### Comparing `PyMoosh-2.3/README.md` & `PyMoosh-2.4/README.md`

 * *Files identical despite different names*

### Comparing `PyMoosh-2.3/setup.py` & `PyMoosh-2.4/setup.py`

 * *Files identical despite different names*

