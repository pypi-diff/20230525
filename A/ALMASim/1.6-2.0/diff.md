# Comparing `tmp/ALMASim-1.6.tar.gz` & `tmp/ALMASim-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALMASim-1.6.tar", last modified: Thu May 25 11:11:26 2023, max compression
+gzip compressed data, was "ALMASim-2.0.tar", last modified: Thu May 25 13:32:04 2023, max compression
```

## Comparing `ALMASim-1.6.tar` & `ALMASim-2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/ALMASim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 11:11:26.000000 ALMASim-1.6/ALMASim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 11:11:26.000000 ALMASim-1.6/ALMASim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:11:26.000000 ALMASim-1.6/ALMASim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 11:11:26.000000 ALMASim-1.6/ALMASim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 11:11:26.000000 ALMASim-1.6/ALMASim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 11:09:46.000000 ALMASim-1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 11:09:46.000000 ALMASim-1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 11:11:26.617604 ALMASim-1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-25 11:09:46.000000 ALMASim-1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 11:09:46.000000 ALMASim-1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:11:26.617604 ALMASim-1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 11:09:46.000000 ALMASim-1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.613604 ALMASim-1.6/submodules/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.613604 ALMASim-1.6/submodules/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/submodules/build/lib/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/sublink.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/build/lib/illustris_python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/submodules/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/sublink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/submodules/illustris_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/tests/groupcat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/tests/sublink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/illustris_python/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 11:09:58.000000 ALMASim-1.6/submodules/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:11:26.617604 ALMASim-1.6/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 11:09:46.000000 ALMASim-1.6/utility/generate_gaussian_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 11:09:46.000000 ALMASim-1.6/utility/split_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 11:09:46.000000 ALMASim-1.6/utility/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.996890 ALMASim-2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.988890 ALMASim-2.0/ALMASim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-25 13:32:03.000000 ALMASim-2.0/ALMASim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 13:32:03.000000 ALMASim-2.0/ALMASim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:32:03.000000 ALMASim-2.0/ALMASim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 13:32:03.000000 ALMASim-2.0/ALMASim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 13:32:03.000000 ALMASim-2.0/ALMASim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 13:30:31.000000 ALMASim-2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 13:30:31.000000 ALMASim-2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-25 13:32:03.992890 ALMASim-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-25 13:30:31.000000 ALMASim-2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-25 13:30:31.000000 ALMASim-2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:32:03.996890 ALMASim-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-25 13:30:31.000000 ALMASim-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.988890 ALMASim-2.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.988890 ALMASim-2.0/submodules/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.988890 ALMASim-2.0/submodules/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.992890 ALMASim-2.0/submodules/build/lib/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/sublink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/build/lib/illustris_python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.992890 ALMASim-2.0/submodules/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/sublink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.992890 ALMASim-2.0/submodules/illustris_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/tests/groupcat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/tests/sublink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/illustris_python/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 13:30:47.000000 ALMASim-2.0/submodules/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:03.992890 ALMASim-2.0/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 13:30:31.000000 ALMASim-2.0/utility/generate_gaussian_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 13:30:31.000000 ALMASim-2.0/utility/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 13:30:31.000000 ALMASim-2.0/utility/test.py
```

### Comparing `ALMASim-1.6/ALMASim.egg-info/SOURCES.txt` & `ALMASim-2.0/ALMASim.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE.md
 MANIFEST.in
-README.md
+README.rst
 pyproject.toml
 setup.py
 ALMASim.egg-info/PKG-INFO
 ALMASim.egg-info/SOURCES.txt
 ALMASim.egg-info/dependency_links.txt
 ALMASim.egg-info/requires.txt
 ALMASim.egg-info/top_level.txt
```

### Comparing `ALMASim-1.6/LICENSE.md` & `ALMASim-2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/README.md` & `ALMASim-2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,70 @@
-# ALMASim
-[![arXiv](https://img.shields.io/badge/arXiv-2211.11462-00ff00.svg)](https://arxiv.org/abs/2211.11462) 
-![build](https://github.com/MicheleDelliVeneri/ALMASim/actions/workflows/python-package.yml/badge.svg)
+.. image:: images/extended_sim_0.png
 
-![](images/extended_sim_0.png)
+Overview
+========
+
+.. INTRO_START_LABEL
 
 ALMASim is a package to generate mock observations of HI line galaxies as observed by the Atacama Large Millimetre/Submillimetre Array (ALMA). ALMASim primary goal is to allow users to generate simulated datasets on which to test deconvolution and source detection models. ALMASim is intended to leverage MPI parallel computing on modern HPC clusters to generate thousands of ALMA data cubes. Users are free to set both source and observational parameters such as antenna configuration, bandwidth, integration time and so on, or completely generate data using random configuration and sources.
 ALMASim is built upon the CASA PiP Wheels (https://casadocs.readthedocs.io/en/latest/index.html), the MARTINI Package (https://github.com/kyleaoman/martini), and the Illustris Python Package (https://github.com/illustristng/illustris_python) to be able to generate observations of both high redshift point-like sources and close extendend sources in all possible ALMA configurations. 
 For every observed target ALMASim generates:
 - A Sky model .fits cube containing the source without any source of noise or instrumental effects;
 - A Dirty .fits cube, i.e. the Fourier inversion of the observed visibilities 
 - A Measurements set .npy file containing the measured visibilities as a numpy array 
 - A parameters.csv containing the observational and source parameters
 
+.. INTRO_END_LABEL
 
-## Installation
-<pre><code> pip install ALMASim </code></pre>
+Citing ALMASim
+--------------
 
+.. CITING_START_LABEL
+   
+If you use ALMASim in your research, please cite the following paper:
+.. code-block:: bibtex
+@ARTICLE{10.1093/mnras/stac3314,
+author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
+title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
+journal = {Monthly Notices of the Royal Astronomical Society},
+year = {2022},
+month = {11},
+issn = {0035-8711},
+doi = {10.1093/mnras/stac3314},
+url = {https://doi.org/10.1093/mnras/stac3314},
+note = {stac3314},
+eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf}
+}
 
-If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
+.. _ALMASim entry: https://doi.org/10.1093/mnras/stac3314
 
-![](images/TNGStructure.PNG)
+.. CITING_END_LABEL
 
-The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/
+Installation Notes
+==================
+.. INSTALLATION_NOTES_START_LABEL
 
-## Usage
-To run the simulation, just navigate to the ALMASim folder and execute 
-<pre><code> python main.py --option value --option1 value1 value2  </code></pre>
-to check the available option run 
-<pre><code> python main.py -h </code></pre>
+ALMASim works with ``python3`` (version ``3.8``), and does not support ``python2``.
 
+Stable releases are available via PyPI_ (``pip install ALMASim``) or GitHub .
+The github main branch is actively developed: things will change, bugs will happen. Any feedback is greatly appreciated via github or micheledelliveneri@gmail.com.
 
-**Happy Simulations**
+.. _PyPI: https://pypi.org/
+.. _micheledelliveneri@gmail.com: mailto:micheledelliveneri@gmail.com
 
+.. INSTALLATION_NOTES_END_LABEL
 
-### Cite us
+Getting started
+===============
 
-Michele Delli Veneri, Łukasz Tychoniec, Fabrizia Guglielmetti, Giuseppe Longo, Eric Villard, 3D Detection and Characterisation of ALMA Sources through Deep Learning, Monthly Notices of the Royal Astronomical Society, 2022;, stac3314, https://doi.org/10.1093/mnras/stac3314
+.. QUICKSTART_START_LABEL
+
+To run the simulation, just navigate to the ALMASim folder and execute 
+``python main.py --option value --option1 value1 value2``
+to check the available option run 
+``python main.py -h``
+If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
+.. image:: images/TNGStructure.PNG
+The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/  
+
+.. QUICKSTART_END_LABEL
 
-@article{10.1093/mnras/stac3314,
-    author = {Delli Veneri, Michele and Tychoniec, Łukasz and Guglielmetti, Fabrizia and Longo, Giuseppe and Villard, Eric},
-    title = "{3D Detection and Characterisation of ALMA Sources through Deep Learning}",
-    journal = {Monthly Notices of the Royal Astronomical Society},
-    year = {2022},
-    month = {11},
-    issn = {0035-8711},
-    doi = {10.1093/mnras/stac3314},
-    url = {https://doi.org/10.1093/mnras/stac3314},
-    note = {stac3314},
-    eprint = {https://academic.oup.com/mnras/advance-article-pdf/doi/10.1093/mnras/stac3314/47014718/stac3314.pdf},
-}
```

### Comparing `ALMASim-1.6/pyproject.toml` & `ALMASim-2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ALMASim"
-version = "1.6"
+version = "2.0"
 authors = [
     {name="M. Delli Veneri", email="micheledelliveneri@gmail.com"},
     {name="L. Tychoniec", email="lukasz.tychoniec@eso.org"},
     {name="F. Guglielmetti", email="fgugliel@eso.org"},
     {name="I. Baronchelli", email="ivano.baronchelli@inaf.it"},
     {name="E. Villard", email="evillard@eso.org"},
     {name="G. Longo", email="giuseppe.longo@unina.it"}
```

### Comparing `ALMASim-1.6/setup.py` & `ALMASim-2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name='ALMASim',
-    version='1.4',
+    version='2.0',
     description='ALMA Simulator for synthetic observations of galaxies. To know more about the code, please visit https://github.com/MicheleDelliVeneri/ALMASim',
+    long_description="fobar",
     packages=find_namespace_packages(),
     install_requires=["numpy", "h5py", "six", 
                       "astropy==5.1.1", "scipy", "matplotlib", "pandas", "tqdm",
                       "h5py", "hdecompose", "spectral-cube", "astromartini", 
                       "dask", "dask[distributed]", "natsort", "distributed", "casatools==6.5.5.21", 
                       "casatasks==6.5.5.21", "casadata==2023.4.10",
```

### Comparing `ALMASim-1.6/submodules/build/lib/illustris_python/groupcat.py` & `ALMASim-2.0/submodules/build/lib/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/build/lib/illustris_python/lhalotree.py` & `ALMASim-2.0/submodules/build/lib/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/build/lib/illustris_python/snapshot.py` & `ALMASim-2.0/submodules/build/lib/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/build/lib/illustris_python/sublink.py` & `ALMASim-2.0/submodules/build/lib/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/build/lib/illustris_python/util.py` & `ALMASim-2.0/submodules/build/lib/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/groupcat.py` & `ALMASim-2.0/submodules/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/lhalotree.py` & `ALMASim-2.0/submodules/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/snapshot.py` & `ALMASim-2.0/submodules/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/sublink.py` & `ALMASim-2.0/submodules/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/tests/groupcat_test.py` & `ALMASim-2.0/submodules/illustris_python/tests/groupcat_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/tests/snapshot_test.py` & `ALMASim-2.0/submodules/illustris_python/tests/snapshot_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/tests/sublink_test.py` & `ALMASim-2.0/submodules/illustris_python/tests/sublink_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/submodules/illustris_python/util.py` & `ALMASim-2.0/submodules/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/utility/generate_gaussian_params.py` & `ALMASim-2.0/utility/generate_gaussian_params.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.6/utility/split_data.py` & `ALMASim-2.0/utility/split_data.py`

 * *Files identical despite different names*

