# Comparing `tmp/space_rocks-1.7.7.tar.gz` & `tmp/space_rocks-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.7.7.tar", max compression
+gzip compressed data, was "space_rocks-1.8.0.tar", max compression
```

## Comparing `space_rocks-1.7.7.tar` & `space_rocks-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.7.7/LICENSE
--rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.7.7/README.md
--rw-r--r--   0        0        0     1419 2023-04-24 10:12:17.117344 space_rocks-1.7.7/pyproject.toml
--rw-r--r--   0        0        0      450 2023-04-24 08:24:01.013287 space_rocks-1.7.7/rocks/__init__.py
--rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/cache.py
--rw-r--r--   0        0        0    11492 2023-04-24 14:38:10.881484 space_rocks-1.7.7/rocks/cli.py
--rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/config.py
--rw-r--r--   0        0        0    39130 2023-04-24 14:46:13.273488 space_rocks-1.7.7/rocks/core.py
--rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/datacloud.py
--rw-r--r--   0        0        0    13082 2023-04-25 07:26:58.446013 space_rocks-1.7.7/rocks/index.py
--rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/logging.py
--rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/metadata.py
--rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.7.7/rocks/plots.py
--rw-r--r--   0        0        0    12799 2023-04-24 08:24:01.017288 space_rocks-1.7.7/rocks/resolve.py
--rw-r--r--   0        0        0    12231 2023-04-21 07:53:47.215006 space_rocks-1.7.7/rocks/ssodnet.py
--rw-r--r--   0        0        0     3026 1970-01-01 00:00:00.000000 space_rocks-1.7.7/setup.py
--rw-r--r--   0        0        0     3148 1970-01-01 00:00:00.000000 space_rocks-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.8.0/LICENSE
+-rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.8.0/README.md
+-rw-r--r--   0        0        0     1430 2023-05-25 08:33:11.343667 space_rocks-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-05-25 08:32:54.311667 space_rocks-1.8.0/rocks/__init__.py
+-rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.8.0/rocks/cache.py
+-rw-r--r--   0        0        0    11492 2023-05-10 09:34:41.049861 space_rocks-1.8.0/rocks/cli.py
+-rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.8.0/rocks/config.py
+-rw-r--r--   0        0        0    39666 2023-05-06 14:21:15.505975 space_rocks-1.8.0/rocks/core.py
+-rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.8.0/rocks/datacloud.py
+-rw-r--r--   0        0        0    13082 2023-04-25 11:37:04.378144 space_rocks-1.8.0/rocks/index.py
+-rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.8.0/rocks/logging.py
+-rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.8.0/rocks/metadata.py
+-rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.8.0/rocks/plots.py
+-rw-r--r--   0        0        0    12799 2023-04-24 08:24:01.017288 space_rocks-1.8.0/rocks/resolve.py
+-rw-r--r--   0        0        0    12222 2023-05-04 09:06:04.136860 space_rocks-1.8.0/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 space_rocks-1.8.0/setup.py
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 space_rocks-1.8.0/PKG-INFO
```

### Comparing `space_rocks-1.7.7/LICENSE` & `space_rocks-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/README.md` & `space_rocks-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/pyproject.toml` & `space_rocks-1.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.7.7"
+version = "1.8.0"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
 packages = [{'include' = 'rocks'}]
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.11"
+python = ">=3.7.1,<3.12"
 numpy = ">=1.21"
 matplotlib = ">=3.4.3"
-aiohttp = "^3.7.4"
-cchardet = "^2.1.7"
+aiohttp = ">=3.8.2"
+faust-cchardet = ">=2.1.7"
 aiodns = "^3.0.0"
 pandas = ">=1.3.5"
 pydantic = "^1.8.2"
 rich = ">=12.2.0"
 click = ">=8.1.2"
 nest-asyncio = "^1.5.1"
 requests = "^2.26.0"
-Levenshtein = "^0.16.0"
+Levenshtein = ">=0.16.0"
 furo = "^2022.9.15"
 sphinx-copybutton = "^0.5.0"
 sphinx_design = "^0.3.0"
-bs4 = "^0.0.1"
 beautifulsoup4 = "^4.11.1"
 platformdirs = "^2.6.2"
+rapidfuzz = "^3"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-redactor-theme", "sphinx-hoverxref"]
 
 [tool.poetry.scripts]
 rocks = "rocks.cli:cli_rocks"
```

### Comparing `space_rocks-1.7.7/rocks/cache.py` & `space_rocks-1.8.0/rocks/cache.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/cli.py` & `space_rocks-1.8.0/rocks/cli.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/config.py` & `space_rocks-1.8.0/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/core.py` & `space_rocks-1.8.0/rocks/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,17 @@
 class Bibref(Parameter):
     doi: str = ""
     year: int = None
     title: str = ""
     bibcode: str = ""
     shortbib: str = ""
 
+    def __bool__(self):
+        return bool(self.shortbib)
+
 
 class LinksParameter(Parameter):
     datacloud: str = ""
     selection: str = ""
 
 
 # And a special class for the Spin list
@@ -243,15 +246,15 @@
 # Dynamical parameters
 class OrbitalElements(Parameter):
     """parameters.dynamical.oribtal_elements"""
 
     ceu: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
     author: StringValue = StringValue(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     ceu_rate: FloatValue = FloatValue(**{})
     ref_epoch: FloatValue = FloatValue(**{})
     inclination: FloatValue = FloatValue(**{})
     mean_motion: FloatValue = FloatValue(**{})
     orbital_arc: IntegerValue = IntegerValue(**{})
     eccentricity: FloatValue = FloatValue(**{})
     mean_anomaly: FloatValue = FloatValue(**{})
@@ -270,15 +273,15 @@
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class ProperElements(Parameter):
     links: LinksParameter = LinksParameter(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     lyapunov_time: FloatValue = FloatValue(**{})
     integration_time: FloatValue = FloatValue(**{})
     proper_eccentricity: FloatValue = FloatValue(**{})
     proper_inclination: FloatValue = FloatValue(**{})
     proper_semi_major_axis: FloatValue = FloatValue(**{})
     proper_sine_inclination: FloatValue = FloatValue(**{})
     proper_frequency_mean_motion: FloatValue = FloatValue(**{})
@@ -356,27 +359,27 @@
 
 class TisserandParameter(Parameter):
     jupiter: FloatValue = pydantic.Field(FloatValue(**{}), alias="Jupiter")
     saturn: FloatValue = pydantic.Field(FloatValue(**{}), alias="Saturn")
     uranus: FloatValue = pydantic.Field(FloatValue(**{}), alias="Uranus")
     neptune: FloatValue = pydantic.Field(FloatValue(**{}), alias="Neptune")
     method: List[Method] = [Method(**{})]
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.dynamical.tisserand_parameter")
 
 
 class Yarkovsky(Parameter):
     S: FloatValue = FloatValue(**{})
     A2: FloatValue = FloatValue(**{})
     snr: FloatValue = FloatValue(**{})
     dadt: FloatValue = FloatValue(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
 
     def __str__(self):
         return "\n".join([self.A2.__str__(), self.dadt.__str__()])
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
@@ -397,30 +400,30 @@
         return self.json()
 
 
 # ------
 # Physical Value
 class Albedo(FloatValue):
     links: LinksParameter = LinksParameter(**{})
-    bibref: ListWithAttributes = []
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = []
 
     path = "parameters.physical.albedo.albedo"
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class ColorEntry(Parameter):
     color: FloatValue = FloatValue(**{})
     epoch: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
     method: List[Method] = []
-    bibref: ListWithAttributes = []
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     facility: StringValue = StringValue(**{})
     observer: StringValue = StringValue(**{})
     phot_sys: StringValue = StringValue(**{})
     technique: StringValue = StringValue(**{})
     delta_time: FloatValue = FloatValue(**{})
     id_filter_1: StringValue = StringValue(**{})
     id_filter_2: StringValue = StringValue(**{})
@@ -511,42 +514,42 @@
         if observed:
             return "\n".join(observed)
         return "No color on record."
 
 
 class Density(FloatValue):
     method: List[Method] = []
-    bibref: ListWithAttributes = []
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.physical.density.density")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class Diameter(FloatValue):
     links: LinksParameter = LinksParameter(**{})
     method: List[Method] = [Method(**{})]
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.physical.diameter.diameter")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class Mass(FloatValue):
     links: LinksParameter = LinksParameter(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(cls, values, "parameters.physical.mass.mass")
 
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
@@ -558,15 +561,15 @@
     H: FloatValue = FloatValue(**{})
     N: FloatValue = FloatValue(**{})
     G1: FloatValue = FloatValue(**{})
     G2: FloatValue = FloatValue(**{})
     rms: FloatValue = FloatValue(**{})
     phase: Error = Error(**{})
     links: LinksParameter = LinksParameter(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     facility: StringValue = StringValue(**{})
     technique: StringValue = StringValue(**{})
     name_filter: StringValue = StringValue(**{})
 
     def __bool__(self):
         return bool(np.isfinite(self.H.value))
 
@@ -579,16 +582,17 @@
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class PhaseFunction(Parameter):
     # Generic
     generic_johnson_V: Phase = pydantic.Field(Phase(**{}), alias="Generic/Johnson.V")
+    generic_johnson_R: Phase = pydantic.Field(Phase(**{}), alias="Generic/Johnson.R")
     # Gaia
-    gaia_gaia3_g: Phase = pydantic.Field(Phase(**{}), alias="GAIA/GAIA3.G")
+    gaia_gaia3_G: Phase = pydantic.Field(Phase(**{}), alias="GAIA/GAIA3.G")
     # ATLAS
     misc_atlas_cyan: Phase = pydantic.Field(Phase(**{}), alias="Misc/Atlas.cyan")
     misc_atlas_orange: Phase = pydantic.Field(Phase(**{}), alias="Misc/Atlas.orange")
 
     def __getattr__(self, name):
         """Implement attribute shortcuts. Gets called if __getattribute__ fails."""
 
@@ -597,27 +601,29 @@
         raise AttributeError
 
     def __bool__(self):
         return any(
             [
                 np.isfinite(getattr(self, filter_).H.value)
                 for filter_ in [
-                    "gaia_gaia3_g",
+                    "gaia_gaia3_G",
+                    "generic_johnson_R",
                     "generic_johnson_V",
                     "misc_atlas_cyan",
                     "misc_atlas_orange",
                 ]
             ]
         )
 
     def __str__(self):
         observed = []
 
         for filter_ in [
-            "gaia_gaia3_g",
+            "gaia_gaia3_G",
+            "generic_johnson_R",
             "generic_johnson_V",
             "misc_atlas_cyan",
             "misc_atlas_orange",
         ]:
             entry = getattr(self, filter_)
             if not np.isnan(entry.H.value):
                 observed.append(
@@ -637,15 +643,15 @@
     Wp: FloatValue = FloatValue(**{})
     id_: IntegerValue = IntegerValue(**{})
     lat: FloatValue = FloatValue(**{})
     RA0: FloatValue = FloatValue(**{})
     DEC0: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
     long_: FloatValue = pydantic.Field(FloatValue(**{}), alias="long")
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
     period: FloatValue = FloatValue(**{})
     obliquity: FloatValue = FloatValue(**{})
     technique: StringValue = StringValue(**{})
     technique: StringValue = StringValue(**{})
     period_type: StringValue = StringValue(**{})
 
@@ -657,15 +663,15 @@
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class Taxonomy(Parameter):
     links: LinksParameter = LinksParameter(**{})
     class_: StringValue = pydantic.Field(StringValue(**{}), alias="class")
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
     scheme: StringValue = StringValue(**{})
     complex: StringValue = StringValue(**{})
     technique: StringValue = StringValue(**{})
     waverange: StringValue = StringValue(**{})
 
     def __bool__(self):
@@ -684,15 +690,15 @@
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class ThermalInertia(FloatValue):
     dsun: FloatValue = FloatValue(**{})
     links: LinksParameter = LinksParameter(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
     method: List[Method] = [Method(**{})]
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(
             cls, values, "parameters.physical.thermal_inertia.thermal_inertia"
         )
@@ -700,15 +706,15 @@
     _convert_list_to_parameterlist: classmethod = pydantic.validator(
         "bibref", allow_reuse=True, pre=True
     )(lambda list_: ListWithAttributes([Bibref(**element) for element in list_]))
 
 
 class AbsoluteMagnitude(FloatValue):
     G: FloatValue = FloatValue(**{})
-    bibref: ListWithAttributes = [Bibref(**{})]
+    bibref: ListWithAttributes = ListWithAttributes([Bibref(**{})])
 
     @pydantic.root_validator()
     def _add_paths(cls, values):
         return add_paths(
             cls, values, "parameters.physical.absolute_magnitude.absolute_magnitude"
         )
```

### Comparing `space_rocks-1.7.7/rocks/datacloud.py` & `space_rocks-1.8.0/rocks/datacloud.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/index.py` & `space_rocks-1.8.0/rocks/index.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/logging.py` & `space_rocks-1.8.0/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/metadata.py` & `space_rocks-1.8.0/rocks/metadata.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/plots.py` & `space_rocks-1.8.0/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/resolve.py` & `space_rocks-1.8.0/rocks/resolve.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.7.7/rocks/ssodnet.py` & `space_rocks-1.8.0/rocks/ssodnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,16 @@
         try:
             cat = cat[0]["datacloud"]
         except (IndexError, KeyError):
             logger.error(
                 f"Catalogue '{catalogue}' for '{id_ssodnet}' got an invalid response from datacloud."
             )
             cat = {}
+            _update_progress(progress_bar, progress)
+            return cat
         if catalogue in cat:
             cat = cat[catalogue]
         else:
             cat = {}
     else:
         cat = {}
 
@@ -381,12 +383,11 @@
         f"{URL_SSODNET}/webservices/ssodnet/api/datacloud.php?-name=id:{id_ssodnet}"
         f"&-resource={catalogue}&-mime=json&-from=rocks"
     )
 
     response = await session.request(method="GET", url=URL)
 
     if not response.ok:
-        logger.warning(f"Catalogue query failed for ID: {id_ssodnet} - {catalogue}")
         return {"data": {id_ssodnet: {"datacloud": None}}}
 
     response_json = await response.json()
     return response_json
```

### Comparing `space_rocks-1.7.7/setup.py` & `space_rocks-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 packages = \
 ['rocks']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Levenshtein>=0.16.0,<0.17.0',
+['Levenshtein>=0.16.0',
  'aiodns>=3.0.0,<4.0.0',
- 'aiohttp>=3.7.4,<4.0.0',
+ 'aiohttp>=3.8.2',
  'beautifulsoup4>=4.11.1,<5.0.0',
- 'bs4>=0.0.1,<0.0.2',
- 'cchardet>=2.1.7,<3.0.0',
  'click>=8.1.2',
+ 'faust-cchardet>=2.1.7',
  'furo>=2022.9.15,<2023.0.0',
  'matplotlib>=3.4.3',
  'nest-asyncio>=1.5.1,<2.0.0',
  'numpy>=1.21',
  'pandas>=1.3.5',
  'platformdirs>=2.6.2,<3.0.0',
  'pydantic>=1.8.2,<2.0.0',
+ 'rapidfuzz>=3,<4',
  'requests>=2.26.0,<3.0.0',
  'rich>=12.2.0',
  'sphinx-copybutton>=0.5.0,<0.6.0',
  'sphinx_design>=0.3.0,<0.4.0']
 
 entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
 
 setup_kwargs = {
     'name': 'space-rocks',
-    'version': '1.7.7',
+    'version': '1.8.0',
     'description': 'Python client for SsODNet data access.',
     'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://rocks.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<3.11',
+    'python_requires': '>=3.7.1,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['rocks']
-package_data = \ {'': ['*']} install_requires = \
-['Levenshtein>=0.16.0,<0.17.0', 'aiodns>=3.0.0,<4.0.0',
-'aiohttp>=3.7.4,<4.0.0', 'beautifulsoup4>=4.11.1,<5.0.0', 'bs4>=0.0.1,<0.0.2',
-'cchardet>=2.1.7,<3.0.0', 'click>=8.1.2', 'furo>=2022.9.15,<2023.0.0',
+package_data = \ {'': ['*']} install_requires = \ ['Levenshtein>=0.16.0',
+'aiodns>=3.0.0,<4.0.0', 'aiohttp>=3.8.2', 'beautifulsoup4>=4.11.1,<5.0.0',
+'click>=8.1.2', 'faust-cchardet>=2.1.7', 'furo>=2022.9.15,<2023.0.0',
 'matplotlib>=3.4.3', 'nest-asyncio>=1.5.1,<2.0.0', 'numpy>=1.21',
 'pandas>=1.3.5', 'platformdirs>=2.6.2,<3.0.0', 'pydantic>=1.8.2,<2.0.0',
-'requests>=2.26.0,<3.0.0', 'rich>=12.2.0', 'sphinx-copybutton>=0.5.0,<0.6.0',
-'sphinx_design>=0.3.0,<0.4.0'] entry_points = \ {'console_scripts': ['rocks =
-rocks.cli:cli_rocks']} setup_kwargs = { 'name': 'space-rocks', 'version':
-'1.7.7', 'description': 'Python client for SsODNet data access.',
-'long_description': '
+'rapidfuzz>=3,<4', 'requests>=2.26.0,<3.0.0', 'rich>=12.2.0', 'sphinx-
+copybutton>=0.5.0,<0.6.0', 'sphinx_design>=0.3.0,<0.4.0'] entry_points = \
+{'console_scripts': ['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name':
+'space-rocks', 'version': '1.8.0', 'description': 'Python client for SsODNet
+data access.', 'long_description': '
   \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                logo_rocks.svg]\n
 \n\n
                     \n Features - Install - Documentation\n
 \n\n
 \n\n
   \n \n_[https://img.shields.io/pypi/pyversions/space-rocks]\n\n \n_[https://
@@ -32,9 +31,9 @@
 Install\n\nInstall from PyPi using `pip`:\n\n $ pip install space-rocks\n\nThe
 minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out
 the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/
 latest/) or run\n\n $ rocks docs\n', 'author': 'Max Mahlke', 'author_email':
 'max.mahlke@oca.eu', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
 'https://rocks.readthedocs.io/en/latest/', 'packages': packages,
 'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.11', } setup
+'entry_points': entry_points, 'python_requires': '>=3.7.1,<3.12', } setup
 (**setup_kwargs)
```

### Comparing `space_rocks-1.7.7/PKG-INFO` & `space_rocks-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: space-rocks
-Version: 1.7.7
+Version: 1.8.0
 Summary: Python client for SsODNet data access.
 Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
-Requires-Python: >=3.7.1,<3.11
+Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
-Requires-Dist: Levenshtein (>=0.16.0,<0.17.0)
+Requires-Dist: Levenshtein (>=0.16.0)
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
-Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.2)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
-Requires-Dist: cchardet (>=2.1.7,<3.0.0)
 Requires-Dist: click (>=8.1.2)
+Requires-Dist: faust-cchardet (>=2.1.7)
 Requires-Dist: furo (>=2022.9.15,<2023.0.0)
 Requires-Dist: matplotlib (>=3.4.3)
 Requires-Dist: nest-asyncio (>=1.5.1,<2.0.0)
 Requires-Dist: numpy (>=1.21)
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: platformdirs (>=2.6.2,<3.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: rapidfuzz (>=3,<4)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: rich (>=12.2.0)
 Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
 Requires-Dist: sphinx_design (>=0.3.0,<0.4.0)
 Project-URL: Documentation, https://rocks.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/maxmahlke/rocks.git
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: space-rocks Version: 1.7.7 Summary: Python client
+Metadata-Version: 2.1 Name: space-rocks Version: 1.8.0 Summary: Python client
 for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
-Python: >=3.7.1,<3.11 Classifier: License :: OSI Approved :: MIT License
+Python: >=3.7.1,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Provides-Extra: docs
-Requires-Dist: Levenshtein (>=0.16.0,<0.17.0) Requires-Dist: aiodns
-(>=3.0.0,<4.0.0) Requires-Dist: aiohttp (>=3.7.4,<4.0.0) Requires-Dist:
-beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-
-Dist: cchardet (>=2.1.7,<3.0.0) Requires-Dist: click (>=8.1.2) Requires-Dist:
-furo (>=2022.9.15,<2023.0.0) Requires-Dist: matplotlib (>=3.4.3) Requires-Dist:
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist: Levenshtein
+(>=0.16.0) Requires-Dist: aiodns (>=3.0.0,<4.0.0) Requires-Dist: aiohttp
+(>=3.8.2) Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0) Requires-Dist: click
+(>=8.1.2) Requires-Dist: faust-cchardet (>=2.1.7) Requires-Dist: furo
+(>=2022.9.15,<2023.0.0) Requires-Dist: matplotlib (>=3.4.3) Requires-Dist:
 nest-asyncio (>=1.5.1,<2.0.0) Requires-Dist: numpy (>=1.21) Requires-Dist:
 pandas (>=1.3.5) Requires-Dist: platformdirs (>=2.6.2,<3.0.0) Requires-Dist:
-pydantic (>=1.8.2,<2.0.0) Requires-Dist: requests (>=2.26.0,<3.0.0) Requires-
-Dist: rich (>=12.2.0) Requires-Dist: sphinx-copybutton (>=0.5.0,<0.6.0)
-Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) Project-URL: Documentation,
-https://rocks.readthedocs.io/en/latest/ Project-URL: Repository, https://
-github.com/maxmahlke/rocks.git Description-Content-Type: text/markdown
+pydantic (>=1.8.2,<2.0.0) Requires-Dist: rapidfuzz (>=3,<4) Requires-Dist:
+requests (>=2.26.0,<3.0.0) Requires-Dist: rich (>=12.2.0) Requires-Dist:
+sphinx-copybutton (>=0.5.0,<0.6.0) Requires-Dist: sphinx_design
+(>=0.3.0,<0.4.0) Project-URL: Documentation, https://rocks.readthedocs.io/en/
+latest/ Project-URL: Repository, https://github.com/maxmahlke/rocks.git
+Description-Content-Type: text/markdown
     [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                 logo_rocks.svg]
                       Features - Install - Documentation
 
  [https://img.shields.io/pypi/pyversions/space-rocks] [https://img.shields.io/
       pypi/v/space-rocks] [https://readthedocs.org/projects/rocks/badge/
   ?version=latest] [https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg]
```

