# Comparing `tmp/ALMASim-2.3.tar.gz` & `tmp/ALMASim-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALMASim-2.3.tar", last modified: Thu May 25 14:29:33 2023, max compression
+gzip compressed data, was "ALMASim-2.5.tar", last modified: Thu May 25 15:13:59 2023, max compression
```

## Comparing `ALMASim-2.3.tar` & `ALMASim-2.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.181018 ALMASim-2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.177018 ALMASim-2.3/ALMASim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 14:29:33.000000 ALMASim-2.3/ALMASim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 14:29:33.000000 ALMASim-2.3/ALMASim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:29:33.000000 ALMASim-2.3/ALMASim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 14:29:33.000000 ALMASim-2.3/ALMASim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 14:29:33.000000 ALMASim-2.3/ALMASim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 14:28:00.000000 ALMASim-2.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 14:28:00.000000 ALMASim-2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-25 14:29:33.181018 ALMASim-2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-25 14:28:00.000000 ALMASim-2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.173018 ALMASim-2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.177018 ALMASim-2.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-25 14:28:00.000000 ALMASim-2.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 14:28:00.000000 ALMASim-2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:29:33.181018 ALMASim-2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 14:28:00.000000 ALMASim-2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.177018 ALMASim-2.3/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.173018 ALMASim-2.3/submodules/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.173018 ALMASim-2.3/submodules/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.177018 ALMASim-2.3/submodules/build/lib/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/sublink.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/build/lib/illustris_python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.181018 ALMASim-2.3/submodules/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/sublink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.181018 ALMASim-2.3/submodules/illustris_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/tests/groupcat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/tests/sublink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/illustris_python/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 14:28:17.000000 ALMASim-2.3/submodules/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:29:33.181018 ALMASim-2.3/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 14:28:00.000000 ALMASim-2.3/utility/generate_gaussian_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 14:28:00.000000 ALMASim-2.3/utility/split_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 14:28:00.000000 ALMASim-2.3/utility/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.923838 ALMASim-2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.919838 ALMASim-2.5/ALMASim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-25 15:13:59.000000 ALMASim-2.5/ALMASim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-25 15:13:59.000000 ALMASim-2.5/ALMASim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:13:59.000000 ALMASim-2.5/ALMASim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 15:13:59.000000 ALMASim-2.5/ALMASim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 15:13:59.000000 ALMASim-2.5/ALMASim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 15:12:40.000000 ALMASim-2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 15:12:40.000000 ALMASim-2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-25 15:13:59.923838 ALMASim-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-25 15:12:40.000000 ALMASim-2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.915837 ALMASim-2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.919838 ALMASim-2.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-25 15:12:40.000000 ALMASim-2.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 15:12:40.000000 ALMASim-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:13:59.923838 ALMASim-2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 15:12:40.000000 ALMASim-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.919838 ALMASim-2.5/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.915837 ALMASim-2.5/submodules/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.915837 ALMASim-2.5/submodules/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.919838 ALMASim-2.5/submodules/build/lib/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/sublink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/build/lib/illustris_python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.923838 ALMASim-2.5/submodules/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/sublink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.923838 ALMASim-2.5/submodules/illustris_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/tests/groupcat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/tests/sublink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/illustris_python/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 15:12:54.000000 ALMASim-2.5/submodules/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:13:59.923838 ALMASim-2.5/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 15:12:40.000000 ALMASim-2.5/utility/generate_gaussian_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 15:12:40.000000 ALMASim-2.5/utility/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 15:12:40.000000 ALMASim-2.5/utility/test.py
```

### Comparing `ALMASim-2.3/ALMASim.egg-info/PKG-INFO` & `ALMASim-2.5/ALMASim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMASim
-Version: 2.3
+Version: 2.5
 Summary: Simulation code for ALMA observations of both high redshift and local galaxies.
 Author-email: "M. Delli Veneri" <micheledelliveneri@gmail.com>, "L. Tychoniec" <lukasz.tychoniec@eso.org>, "F. Guglielmetti" <fgugliel@eso.org>, "I. Baronchelli" <ivano.baronchelli@inaf.it>, "E. Villard" <evillard@eso.org>, "G. Longo" <giuseppe.longo@unina.it>
 Project-URL: Homepage, https://github.com/MicheleDelliVeneri/ALMASim
 Project-URL: Documentation, https://almasim.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MicheleDelliVeneri/ALMASim/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,27 +39,29 @@
 
 Citing ALMASim
 --------------
 
 .. CITING_START_LABEL
    
 If you use ALMASim in your research, please cite the following paper:
+
 .. code-block:: bibtex
-@ARTICLE{10.1093/mnras/stac3314,
-author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
-title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
-journal = {Monthly Notices of the Royal Astronomical Society},
-year = {2022},
-month = {11},
-issn = {0035-8711},
-doi = {10.1093/mnras/stac3314},
-url = {https://doi.org/10.1093/mnras/stac3314},
-note = {stac3314},
-eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
-}
+
+    @ARTICLE{10.1093/mnras/stac3314,
+    author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
+    title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2022},
+    month = {11},
+    issn = {0035-8711}, 
+    doi = {10.1093/mnras/stac3314},
+    url = {https://doi.org/10.1093/mnras/stac3314},
+    note = {stac3314},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
+    }
 
 .. _ALMASim entry: https://doi.org/10.1093/mnras/stac3314
 
 .. CITING_END_LABEL
 
 Installation Notes
 ==================
@@ -81,12 +83,10 @@
 .. QUICKSTART_START_LABEL
 
 To run the simulation, just navigate to the ALMASim folder and execute 
 ``python main.py --option value --option1 value1 value2``
 to check the available option run 
 ``python main.py -h``
 If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
-.. image:: TNGStructure.PNG
-The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
+TNGStructure.PNG shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
 
 .. QUICKSTART_END_LABEL
-
```

### Comparing `ALMASim-2.3/ALMASim.egg-info/SOURCES.txt` & `ALMASim-2.5/ALMASim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/LICENSE.md` & `ALMASim-2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/PKG-INFO` & `ALMASim-2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALMASim
-Version: 2.3
+Version: 2.5
 Summary: Simulation code for ALMA observations of both high redshift and local galaxies.
 Author-email: "M. Delli Veneri" <micheledelliveneri@gmail.com>, "L. Tychoniec" <lukasz.tychoniec@eso.org>, "F. Guglielmetti" <fgugliel@eso.org>, "I. Baronchelli" <ivano.baronchelli@inaf.it>, "E. Villard" <evillard@eso.org>, "G. Longo" <giuseppe.longo@unina.it>
 Project-URL: Homepage, https://github.com/MicheleDelliVeneri/ALMASim
 Project-URL: Documentation, https://almasim.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MicheleDelliVeneri/ALMASim/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -39,27 +39,29 @@
 
 Citing ALMASim
 --------------
 
 .. CITING_START_LABEL
    
 If you use ALMASim in your research, please cite the following paper:
+
 .. code-block:: bibtex
-@ARTICLE{10.1093/mnras/stac3314,
-author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
-title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
-journal = {Monthly Notices of the Royal Astronomical Society},
-year = {2022},
-month = {11},
-issn = {0035-8711},
-doi = {10.1093/mnras/stac3314},
-url = {https://doi.org/10.1093/mnras/stac3314},
-note = {stac3314},
-eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
-}
+
+    @ARTICLE{10.1093/mnras/stac3314,
+    author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
+    title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2022},
+    month = {11},
+    issn = {0035-8711}, 
+    doi = {10.1093/mnras/stac3314},
+    url = {https://doi.org/10.1093/mnras/stac3314},
+    note = {stac3314},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
+    }
 
 .. _ALMASim entry: https://doi.org/10.1093/mnras/stac3314
 
 .. CITING_END_LABEL
 
 Installation Notes
 ==================
@@ -81,12 +83,10 @@
 .. QUICKSTART_START_LABEL
 
 To run the simulation, just navigate to the ALMASim folder and execute 
 ``python main.py --option value --option1 value1 value2``
 to check the available option run 
 ``python main.py -h``
 If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
-.. image:: TNGStructure.PNG
-The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
+TNGStructure.PNG shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
 
 .. QUICKSTART_END_LABEL
-
```

### Comparing `ALMASim-2.3/README.rst` & `ALMASim-2.5/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -17,27 +17,29 @@
 
 Citing ALMASim
 --------------
 
 .. CITING_START_LABEL
    
 If you use ALMASim in your research, please cite the following paper:
+
 .. code-block:: bibtex
-@ARTICLE{10.1093/mnras/stac3314,
-author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
-title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
-journal = {Monthly Notices of the Royal Astronomical Society},
-year = {2022},
-month = {11},
-issn = {0035-8711},
-doi = {10.1093/mnras/stac3314},
-url = {https://doi.org/10.1093/mnras/stac3314},
-note = {stac3314},
-eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
-}
+
+    @ARTICLE{10.1093/mnras/stac3314,
+    author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
+    title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
+    journal = {Monthly Notices of the Royal Astronomical Society},
+    year = {2022},
+    month = {11},
+    issn = {0035-8711}, 
+    doi = {10.1093/mnras/stac3314},
+    url = {https://doi.org/10.1093/mnras/stac3314},
+    note = {stac3314},
+    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
+    }
 
 .. _ALMASim entry: https://doi.org/10.1093/mnras/stac3314
 
 .. CITING_END_LABEL
 
 Installation Notes
 ==================
@@ -59,12 +61,10 @@
 .. QUICKSTART_START_LABEL
 
 To run the simulation, just navigate to the ALMASim folder and execute 
 ``python main.py --option value --option1 value1 value2``
 to check the available option run 
 ``python main.py -h``
 If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
-.. image:: TNGStructure.PNG
-The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
+TNGStructure.PNG shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
 
 .. QUICKSTART_END_LABEL
-
```

### Comparing `ALMASim-2.3/docs/source/conf.py` & `ALMASim-2.5/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ALMASim"
 copyright = "2023, Michele Delli Veneri"
 author = "Michele Delli Veneri"
 
 # The full version, including alpha/beta/rc tags
-release = "2.3"
+release = "2.5"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `ALMASim-2.3/pyproject.toml` & `ALMASim-2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ALMASim"
-version = "2.3"
+version = "2.5"
 authors = [
     {name="M. Delli Veneri", email="micheledelliveneri@gmail.com"},
     {name="L. Tychoniec", email="lukasz.tychoniec@eso.org"},
     {name="F. Guglielmetti", email="fgugliel@eso.org"},
     {name="I. Baronchelli", email="ivano.baronchelli@inaf.it"},
     {name="E. Villard", email="evillard@eso.org"},
     {name="G. Longo", email="giuseppe.longo@unina.it"}
```

### Comparing `ALMASim-2.3/setup.py` & `ALMASim-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='ALMASim',
-    version='2.3',
+    version='2.5',
     description='ALMA Simulator for synthetic observations of galaxies. To know more about the code, please visit https://github.com/MicheleDelliVeneri/ALMASim',
     long_description="fobar",
     packages=find_namespace_packages(),
     install_requires=["numpy", "h5py", "six", 
                       "astropy==5.1.1", "scipy", "matplotlib", "pandas", "tqdm",
                       "h5py", "hdecompose", "spectral-cube", "astromartini", 
                       "dask", "dask[distributed]", "natsort", "distributed", "casatools==6.5.5.21",
```

### Comparing `ALMASim-2.3/submodules/build/lib/illustris_python/groupcat.py` & `ALMASim-2.5/submodules/build/lib/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/build/lib/illustris_python/lhalotree.py` & `ALMASim-2.5/submodules/build/lib/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/build/lib/illustris_python/snapshot.py` & `ALMASim-2.5/submodules/build/lib/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/build/lib/illustris_python/sublink.py` & `ALMASim-2.5/submodules/build/lib/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/build/lib/illustris_python/util.py` & `ALMASim-2.5/submodules/build/lib/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/groupcat.py` & `ALMASim-2.5/submodules/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/lhalotree.py` & `ALMASim-2.5/submodules/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/snapshot.py` & `ALMASim-2.5/submodules/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/sublink.py` & `ALMASim-2.5/submodules/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/tests/groupcat_test.py` & `ALMASim-2.5/submodules/illustris_python/tests/groupcat_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/tests/snapshot_test.py` & `ALMASim-2.5/submodules/illustris_python/tests/snapshot_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/tests/sublink_test.py` & `ALMASim-2.5/submodules/illustris_python/tests/sublink_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/submodules/illustris_python/util.py` & `ALMASim-2.5/submodules/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/utility/generate_gaussian_params.py` & `ALMASim-2.5/utility/generate_gaussian_params.py`

 * *Files identical despite different names*

### Comparing `ALMASim-2.3/utility/split_data.py` & `ALMASim-2.5/utility/split_data.py`

 * *Files identical despite different names*

