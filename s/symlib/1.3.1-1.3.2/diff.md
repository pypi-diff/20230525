# Comparing `tmp/symlib-1.3.1.tar.gz` & `tmp/symlib-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.1.tar", last modified: Thu May 11 04:10:28 2023, max compression
+gzip compressed data, was "symlib-1.3.2.tar", last modified: Thu May 25 11:21:37 2023, max compression
```

## Comparing `symlib-1.3.1.tar` & `symlib-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.610875 symlib-1.3.1/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-11 04:10:28.610760 symlib-1.3.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.1/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.1/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-11 04:10:28.610906 symlib-1.3.1/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-11 04:10:25.000000 symlib-1.3.1/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.609911 symlib-1.3.1/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1629 2023-04-18 17:25:19.000000 symlib-1.3.1/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.1/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    47959 2023-05-11 04:10:25.000000 symlib-1.3.1/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.1/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.1/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-11 04:10:28.610585 symlib-1.3.1/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-11 04:10:28.000000 symlib-1.3.1/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.328703 symlib-1.3.2/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.2/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-25 11:21:37.328568 symlib-1.3.2/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.2/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.2/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-05-25 11:21:37.328759 symlib-1.3.2/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-05-25 11:19:28.000000 symlib-1.3.2/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.327366 symlib-1.3.2/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.2/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.2/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    52489 2023-05-25 11:19:28.000000 symlib-1.3.2/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    35330 2023-04-11 22:48:38.000000 symlib-1.3.2/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.2/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-25 11:21:37.328357 symlib-1.3.2/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-05-25 11:21:37.000000 symlib-1.3.2/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.1/LICENSE` & `symlib-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.1/PKG-INFO` & `symlib-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.1
+Version: 1.3.2
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.1/setup.py` & `symlib-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.1"
+version = "1.3.2"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.1/symlib/__init__.py` & `symlib-1.3.2/symlib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Data types
 from .lib import SUBHALO_DTYPE, HISTORY_DTYPE, BRANCH_DTYPE, CORE_DTYPE, UM_DTYPE, PARTICLE_DTYPE
 # I/O function
 from .lib import read_subhalos, read_cores, read_branches, read_tree, read_particles, ParticleInfo
 from .lib import Particles
 # Utilities
-from .lib import simulation_parameters, parameter_table, scale_factors, pristine_merger_indices, merger_stats, propagate_parent_indices, colossus_parameters, suite_names, merger_lookup_table, find_merger_branch, find_all_merger_branches, is_real_confirmed, read_um
+from .lib import simulation_parameters, parameter_table, scale_factors, pristine_merger_indices, merger_stats, propagate_parent_indices, colossus_parameters, suite_names, merger_lookup_table, find_merger_branch, find_all_merger_branches, is_real_confirmed, read_um, read_symfind, read_rockstar
 # TODO: better names for pristine_merger_indices and propagate_parent_indices
 
 # Abstract models
 from .star_tagging import ProfileModel, RHalfModel, MStarModel, AbstractRanking
 # Profile models
 from .star_tagging import PlummerProfile
 # R_half models
```

### Comparing `symlib-1.3.1/symlib/file_management.py` & `symlib-1.3.2/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.1/symlib/lib.py` & `symlib-1.3.2/symlib/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,40 +6,68 @@
 import scipy.interpolate as interpolate
 import numpy.random as random
 import scipy.optimize as optimize
 import glob
 from . import util
 
 """ SUBHALO_DTYPE is the numpy datatype used by the main return value of
-read_subhalos(). Positions and distances are in comvoing Mpc/h, velocities are
-physical peculiar velocities, and masses are in Msun/h.
+read_subhalos().
 """
 SUBHALO_DTYPE = [("id", "i4"), ("mvir", "f4"), ("vmax", "f4"), ("rvmax", "f4"),
                  ("x", "f4", (3,)), ("v", "f4", (3,)), ("ok", "?"),
                  ("rvir", "f4"), ("cvir", "f4")]
 
+
+""" ROCKSTAR_DTYPE is the main numpy datatype returned by read_rockstar().
+ - id: unique identifier for the halo.
+ - m (Msun): mass of the subhalo.
+ - vmax (km/s): maximum value of the subhalo's rotation curve.
+ - rvmax (physical kpc): radius of vmax.
+ - x (physical kpc): displacement from the host's centre to the subhalo's
+   centre.
+ - v (km/s) velocity of the subhalo relative to the host's centre.
+ - rvir (physical kpc): radius of the subhalo according to Bryan & Norman 1998.
+   This is rarely a meaningful quantity for subhaloes as their tidal radii are
+   usually smaller than rvir.
+ - cvir: the NFW concentration parameter, r_-2/rvir for the subhalo, as
+   estimated from vmax/vvir. This is rarely a meaninfiul quantity for
+   subhaloes, because their profiles are very different from NFW..
+ - ok: True if the subhalo exists and False otherwise. Note that if Rockstar
+   has any errors but still believes this subhalo is real, this will be true.
+   This can only be calculated for haloes which symfind has been run on
+   You must use the HISTORY_DTYPE or SYMFIND_DTYPE to identify
+"""
+ROCKSTAR_DTYPE = [("id", "i4"), ("m", "f4"), ("vmax", "f4"), ("rvmax", "f4"),
+                 ("x", "f4", (3,)), ("v", "f4", (3,)), ("ok", "?"),
+                 ("rvir", "f4"), ("cvir", "f4")]
+
 """ HISTORY_DTYPE is a numpy datatype representing data about a subhalo which 
 is indepdent of time, such as the maximum mass that it takes on, its merger
-snapshot, and its locaiton in the full merger tree file.
+snapshot, and its location in the full merger tree file.
 
  - The main branch of a given halo within the depth-first merger tree can be 
    found with x[start:end].
- - is_real: false if a halo is definitely a numerical artefact (e.g. if it's
-   already a subhalo in its first snapshot).
- - is_disappear: true if the subhalo disappears without merging. This is also
-   bad and probably means the thing is a numerical artefact.
- - is_main_sub: true is the halo was ever a subhalo of the zoom-in box's main 
-   halo (includes splashback subhaloes).
- - preprocess: the index of the branch of the largest halo that hosted this 
-   halo before it became a subhalo of the main halo. If the halo was never a
-   subhalo of the main halo, this is just the index of largest halo to have
-   every hosted this halo. If no other halo every hosted this halo before
-   it entered Rvir of the main halo, this is -1. Includes splashback subhaloes
-   and doesn't include collisions between subhaloes once they've already been
-   accreted.
+ - mpeak: (Msun) the peak value of Mvir across the entire branch
+ - mpeak_pre: (Msun) the peak value of Mvir before becoming a subhalo
+ - vpeak: (km/s) the peak value of vmax across the entire branch
+ - merger_snap: the snapshot that the subhalo first became a subhalo of the
+   main host halo.
+ - first_infall_snap: the snapshot that the subhalo first became a subhalo of
+   any other object, excluding glitches during major mergers.
+ - conv_snap_*: the snaphot at which the subhalo is predicted to be
+   unconverged, according to various criteria. See mansfield et al. 2023 for
+   discussion
+ - disrupt_snap: the snapshot at which the subhalo disrupts in the symfind
+   catalogue
+ - disrupt_snap_rs: the snapshot at which the subhalo disrupts in Rockstar + 
+   consistent-trees. If the Rockstar has erroneous subhalo
+   identifications at the end of its branch, this flags the last non-error
+   snapshot.
+ - several other non-informative fields are included for consistency with
+   BRANCH_DTYPE.
 """
 HISTORY_DTYPE = [("mpeak", "f4"), ("vpeak", "f4"), ("merger_snap", "i4"),
                  ("merger_ratio", "f4"),
                  ("start", "i4"), ("end", "i4"), ("is_real", "?"),
                  ("is_disappear", "?"), ("is_main_sub", "?"),
                  ("preprocess", "i4"), ("first_infall_snap", "i4"),
                  ("branch_idx", "i4"), ("false_selection", "?"),
@@ -100,14 +128,61 @@
 CORE_DTYPE = [("x", "f4", (3,)), ("v", "f4", (3,)), ("r_tidal", "f4"),
               ("r50_bound", "f4"), ("r50_bound_rs", "f4"), ("m_tidal", "f4"),
               ("m_tidal_bound", "f4"), ("m_bound", "f4"), ("vmax", "f4"),
               ("f_core", "f4"), ("f_core_rs", "f4"), ("d_core_mbp", "f4"),
               ("ok", "?"), ("ok_rs", "?"), ("is_err", "?"), ("is_err_rs", "?"),
               ("interp", "?")]
 
+""" SYMFIND_DTYPE is the main numpy datatype returned by read_symfind().
+ - x (physical kpc): displacement from the host halo to the subhalo.
+ - v (km/s): velocity relative to the host.
+ - m (Msun): bound mass of the subhalo.
+ - r_half (physical kpc) half-mass radius of the subhalo.
+ - r_tidal (physical kpc): tidal radius of the subhalo. Accounts for angular
+   momentum and the mass profile of the central halo. Tidal radii can be
+   poor approximations if the size of the subhalo is comparable to the
+   distance to the host centre or if the subhalo is at pericentre. There is no
+   strict criteria for identifying this.
+ - m_tidal (Msun): total mass within tidal radius.
+ - m_tidal_bound (Msun): total bound mass within tidal radius, using only
+   particles within the tidal radius. This value can be a bit fragile at
+   pericentre.
+ - ok: true if the subhalo exists and is not an error, and false otherwise.
+   Interpolated subhaloes will be marked as true.
+ - interp: true if the subhalo in this snapshot is interpolated betwen two
+   nearby snapshots.
+
+Some values for Rockstar haloes are also calculated here:
+ - r_half_rs (physical kpc): half-mass radius of tracked particles using
+   Rockstar's position and velocity. This is the r_half used for error
+   detection, not the r_half in the Rockstar catalogues.
+ - ok_rs: true if a rockstar halo exists and at least one core particle is
+   still inside Rockstar's r_half. A slightly more conservative way to
+   identify Rockstar errors would be to check if ok_rs & (~is_err_rs).
+
+Some diagnostic values are included that will not be useful for a typical user:
+ - is_err: Rockstar and symfind disagree, but more core particles are
+   assoicated with Rockstar. If this is true, the subhalo is either
+   interpolated or flagged as disrupted.
+ - is_err_rs: Rockstar and symfind disagree, but more core particles are
+   associated with symfind.
+ - f_core: the fraction of core particles associated with Rockstar
+ - f_core_rs: the fraction of core particles associated with symfind.
+ - d_core_mbp (physical kpc): the distance between the subhalo and the
+   most-bound particle. Sometimes the most-bound particle can numerically
+   diffuse out of the subhalo.
+"""
+SYMFIND_DTYPE = [("x", "f4", (3,)), ("v", "f4", (3,)), ("r_tidal", "f4"),
+                 ("r_half", "f4"), ("m_tidal", "f4"),
+                 ("m_tidal_bound", "f4"), ("m", "f4"), ("vmax", "f4"),
+                 ("ok", "?"), ("interp", "?"),
+                 ("f_core", "f4"), ("f_core_rs", "f4"), ("d_core_mbp", "f4"),
+                 ("r_half_rs", "f4"), ("ok_rs", "?"),
+                 ("is_err", "?"), ("is_err_rs", "?")]
+
 """ UM_DTYPE is a numpy datatype representing UniverseMachine predictions for
 galaxy properties.
 - m_star: the stellar mass of the galaxy in Msun
 - m_in_situ: the stellar mass of a galaxy that formed inside the galaxy (as
              opposed to coming in via mergers) in Msun
 - m_icl: the stellar mass of the galaxy's stellar halo
 - sfr: the starformaiton rate in Msun/yr
@@ -399,14 +474,26 @@
         m_snap_sub = np.searchsorted(snap_i[::-1], m_snap_i)
         mpeak[j] = np.max(mvir_i)
         m_snap[j] = m_snap_i
         ratio[j] = mvir_i[::-1][m_snap_sub]/mw["mvir"][m_snap_i]
 
     return mpeak, m_snap, ratio, sub_idx
 
+ROCKSTAR_DTYPE = [("id", "i4"), ("m", "f4"), ("vmax", "f4"), ("rvmax", "f4"),
+                 ("x", "f4", (3,)), ("v", "f4", (3,)), ("ok", "?"),
+                 ("rvir", "f4"), ("cvir", "f4")]
+
+def read_rockstar(dir_name):
+    h, hist = read_subhalos(dir_name)
+    r = np.zeros(h.shape, dtype=ROCKSTAR_DTYPE)
+    r["id"], r["m"], r["vmax"] = h["id"], h["mvir"], h["vmax"]
+    r["rvmax"], r["x"], r["v"] = h["rvmax"], h["x"], h["v"]
+    r["ok"], r["rvir"], r["cvir"] = h["ok"], h["rvir"], h["cvir"]
+    return r, hist
+
 def read_subhalos(dir_name, comoving=False, include_false_selections=False):
     """ read_subhalos reads major merger data from the halo directory dir_name.
     It returns two arrays. The first, m_idx, is the indices of the major
     mergers within the branches arrays. Index 0 is the main halo, index 1 is the
     biggest merger (by Mpeak), index 2 is the second biggest, etc. As a
     convenience, data from the main branches of those haloes are returned as
     the second argument, m. m[halo_idx, snap] gives the  properties of the
@@ -522,20 +609,21 @@
         h["mpeak_pre"][i] = mpeak_infall
         h["false_selection"][i] = mpeak_infall < 300*param["mp"]
 
     (snap_discrete, snap_eps,
      snap_relax, snap_relax_hydro,
      disrupt_snap, disrupt_snap_rs) = read_convergence_limits(dir_name)
     if snap_discrete is not None:
-        h["conv_snap_discrete"] = snap_discrete
-        h["conv_snap_eps"] = snap_eps
-        h["conv_snap_relax"] = snap_relax
-        h["conv_snap_relax_hydro"] = snap_relax_hydro
-        h["disrupt_snap"] = disrupt_snap
-        h["disrupt_snap_rs"] = disrupt_snap_rs
+        ok = ~h["false_selection"]
+        h["conv_snap_discrete"][ok] = snap_discrete
+        h["conv_snap_eps"][ok] = snap_eps
+        h["conv_snap_relax"][ok] = snap_relax
+        h["conv_snap_relax_hydro"][ok] = snap_relax_hydro
+        h["disrupt_snap"][ok] = disrupt_snap
+        h["disrupt_snap_rs"][ok] = disrupt_snap_rs
 
     return h
 
 def read_convergence_limits(sim_dir):
     file_name = path.join(sim_dir, "convergence_limits.dat")
     if not path.exists(file_name): return None, None, None, None, None, None
 
@@ -549,14 +637,41 @@
             disrupt_snap = np.fromfile(fp, np.int32, n_halo)
             disrupt_snap_rs = np.fromfile(fp, np.int32, n_halo)
 
             return snap_discrete, snap_eps, snap_relax, snap_relax_hydro, disrupt_snap, disrupt_snap_rs
     except:
         return None, None, None, None, None, None
 
+def read_symfind(dir_name, suffix="fid3"):
+    """ read_symfind returns a pair of arrays representing each symfind
+    subhalo. dir_name is the simulation's directory. The first is a 2D array
+    of type SYMFIND_DTYPE where halos[i,j] is subhalo i at snapshot j.
+    Symfind only tracks subhaloes, so there are no entries prioer to first
+    infall. The second return value is an array of type HISTORY_DTYPE with
+    one element for each subhalo. Subhaloes are ordered by decreasing
+    pre-infall Mpeak, and the first element corresponds to the host halo.
+    (Because the host is not a subhalo by definition, symfind does not have
+    entries for this object).
+    """
+    h, hist = read_subhalos(dir_name)
+    c = read_cores(dir_name)
+
+    s = np.zeros(c.shape, dtype=SYMFIND_DTYPE)
+    s["x"], s["v"] = c["x"], c["v"]
+    s["r_tidal"], s["r_half"] = c["r_tidal"], c["r50_bound"] 
+    s["m_tidal_bound"], s["m"] = c["m_tidal_bound"], c["m_bound"]
+    s["vmax"], s["ok"], s["interp"] = c["vmax"], c["ok"], c["interp"]
+    s["f_core"], s["f_core_rs"] = c["f_core"], c["f_core"]
+    s["d_core_mbp"] = c["d_core_mbp"]
+    s["r_half_rs"], s["ok_rs"] = c["r50_bound_rs"], c["ok_rs"]
+    s["is_err"], s["is_err_rs"] = c["is_err"], c["is_err_rs"]
+
+    return s, hist
+
+
 def read_cores(dir_name, include_false_selections=False, suffix="fid3"):
     """ read_cores read the particle-tracked halo cores of the halo in the
     given directory. The returned array is a structured array of type
     CORE_DTYPE with shape (n_halos, n_snaps).
     """
     if suffix == "":
         file_name = path.join(dir_name, "halos", "cores.dat")
@@ -591,46 +706,14 @@
         out["is_err"] = np.fromfile(fp, np.bool, n)
         out["is_err_rs"] = np.fromfile(fp, np.bool, n)
         out["interp"] = np.fromfile(fp, np.bool, n)
        
 
     out = out.reshape((n_halo, n_snap))
 
-    """
-    r_core = np.sqrt(np.sum(out["x"]**2, axis=2))
-    r_rs = np.sqrt(np.sum(h["x"]**2, axis=2))
-    r_core_rs = np.sqrt(np.sum((h["x"] - out["x"])**2, axis=2))
-
-    out["is_err"] = (out["f_core"] == 0) | (out["r50_bound"] > r_core)
-    out["is_err_rs"] = (out["f_core_rs"] == 0)|(out["r50_bound_rs"] > r_rs)
-
-    both_ok = ((out["ok"] & (~out["is_err"])) &
-               (h["ok"] & (~out["is_err_rs"])))
-    disagree = (both_ok & (r_core_rs > out["r50_bound"]) &
-                (r_core_rs > out["r50_bound_rs"]))
-
-    disagree_rs_wins = disagree & (out["f_core_rs"] > out["f_core"])
-    disagree_core_wins = disagree & (~disagree_rs_wins)
-    out["is_err"] = (out["is_err"] | disagree_rs_wins) & out["ok"]
-    out["is_err_rs"] = (out["is_err_rs"] | disagree_core_wins) & h["ok"]
-
-    out["ok"] = out["ok"] & (~out["is_err"])
-    out["ok_rs"] = h["ok"] & (~out["is_err_rs"])
-
-    has_neighbor = np.zeros(out.shape, dtype=bool)
-    has_neighbor[:,:-1] = out["ok"][:,1:]
-    has_neighbor[:,1:] = has_neighbor[:,1:] | out["ok"][:,:-1]
-    out["ok"] = out["ok"] & has_neighbor
-    recent_infall = hist["first_infall_snap"] == out.shape[1]-1
-    out["ok"][recent_infall, -1] = True
-
-    scale = scale_factors(dir_name)
-    interpolate_cores(scale, out, h, hist, mp)
-    """
-
     if not include_false_selections:
         h, hist = read_subhalos(dir_name, include_false_selections=True)
         out = out[~hist["false_selection"]]
 
     return out
 
 def read_um(dir_name):
```

### Comparing `symlib-1.3.1/symlib/star_tagging.py` & `symlib-1.3.2/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.1/symlib/util.py` & `symlib-1.3.2/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.1/symlib.egg-info/PKG-INFO` & `symlib-1.3.2/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.1
+Version: 1.3.2
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

