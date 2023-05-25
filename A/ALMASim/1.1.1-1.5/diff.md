# Comparing `tmp/ALMASim-1.1.1.tar.gz` & `tmp/ALMASim-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALMASim-1.1.1.tar", last modified: Fri May 12 16:25:00 2023, max compression
+gzip compressed data, was "ALMASim-1.5.tar", last modified: Thu May 25 10:42:51 2023, max compression
```

## Comparing `ALMASim-1.1.1.tar` & `ALMASim-1.5.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.753047 ALMASim-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/ALMASim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 16:25:00.000000 ALMASim-1.1.1/ALMASim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-12 16:25:00.000000 ALMASim-1.1.1/ALMASim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 16:25:00.000000 ALMASim-1.1.1/ALMASim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 16:25:00.000000 ALMASim-1.1.1/ALMASim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 16:25:00.000000 ALMASim-1.1.1/ALMASim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-12 16:23:35.000000 ALMASim-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 16:25:00.753047 ALMASim-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-12 16:23:35.000000 ALMASim-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 16:25:00.753047 ALMASim-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-12 16:23:35.000000 ALMASim-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/submodules/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/submodules/build/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/submodules/build/lib/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/sublink.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/build/lib/illustris_python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.749047 ALMASim-1.1.1/submodules/illustris_python/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/groupcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/lhalotree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/sublink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.753047 ALMASim-1.1.1/submodules/illustris_python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/tests/groupcat_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/tests/snapshot_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/tests/sublink_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/illustris_python/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-12 16:23:42.000000 ALMASim-1.1.1/submodules/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 16:25:00.753047 ALMASim-1.1.1/utility/
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-12 16:23:35.000000 ALMASim-1.1.1/utility/generate_gaussian_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-12 16:23:35.000000 ALMASim-1.1.1/utility/split_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-12 16:23:35.000000 ALMASim-1.1.1/utility/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.805582 ALMASim-1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.801582 ALMASim-1.5/ALMASim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 10:42:51.000000 ALMASim-1.5/ALMASim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 10:42:51.000000 ALMASim-1.5/ALMASim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:42:51.000000 ALMASim-1.5/ALMASim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 10:42:51.000000 ALMASim-1.5/ALMASim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-25 10:42:51.000000 ALMASim-1.5/ALMASim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-25 10:40:33.000000 ALMASim-1.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 10:40:33.000000 ALMASim-1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 10:42:51.805582 ALMASim-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-25 10:40:33.000000 ALMASim-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 10:40:33.000000 ALMASim-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:42:51.805582 ALMASim-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-25 10:40:33.000000 ALMASim-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.801582 ALMASim-1.5/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.801582 ALMASim-1.5/submodules/build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.801582 ALMASim-1.5/submodules/build/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.805582 ALMASim-1.5/submodules/build/lib/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/sublink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/build/lib/illustris_python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.805582 ALMASim-1.5/submodules/illustris_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/groupcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/lhalotree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/sublink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.805582 ALMASim-1.5/submodules/illustris_python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/tests/groupcat_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/tests/snapshot_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/tests/sublink_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/illustris_python/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 10:40:48.000000 ALMASim-1.5/submodules/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:42:51.805582 ALMASim-1.5/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-05-25 10:40:33.000000 ALMASim-1.5/utility/generate_gaussian_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-25 10:40:33.000000 ALMASim-1.5/utility/split_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 10:40:33.000000 ALMASim-1.5/utility/test.py
```

### Comparing `ALMASim-1.1.1/ALMASim.egg-info/SOURCES.txt` & `ALMASim-1.5/ALMASim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-LICENSE
+LICENSE.md
+MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 ALMASim.egg-info/PKG-INFO
 ALMASim.egg-info/SOURCES.txt
 ALMASim.egg-info/dependency_links.txt
 ALMASim.egg-info/requires.txt
 ALMASim.egg-info/top_level.txt
 submodules/setup.py
```

### Comparing `ALMASim-1.1.1/README.md` & `ALMASim-1.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,36 +10,23 @@
 - A Sky model .fits cube containing the source without any source of noise or instrumental effects;
 - A Dirty .fits cube, i.e. the Fourier inversion of the observed visibilities 
 - A Measurements set .npy file containing the measured visibilities as a numpy array 
 - A parameters.csv containing the observational and source parameters
 
 
 ## Installation
-1 Clone the GitHub repository and move into it:
-<pre><code>git clone https://github.com/MicheleDelliVeneri/ALMASim.git</code></pre>
-<pre><code>cd ALMASim</code></pre>
-
-2 Create a conda environment from the provided requirements and activate it:
-<pre><code>conda create --name casa6.5 --file requirements.txt </code></pre>
-<pre><code>conda activate casa6.5 </code></pre>
-
-3 Install the illustris_python package:
-<pre><code> git clone git@github.com:illustristng/illustris_python.git </code></pre>
-<pre><code> cd illustris_python </code></pre>
-<pre><code> pip install . </code></pre>
+<pre><code> pip install ALMASim </code></pre>
 
-4 If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
+
+If you are interested in simulating Extended sources, you need to download and configure the Illustris TNG100-1 simulation folder.
 
 ![](images/TNGStructure.PNG)
 
 The picture shows an example for Snapshot-99, reproduce this for every Snapshot you are interested i. You can check more at the Illustris TNG official website: https://www.tng-project.org/data/
 
-6. Install the required packages 
-<pre><code> pip install -r requirements.txt  </code></pre>
-
 ## Usage
 To run the simulation, just navigate to the ALMASim folder and execute 
 <pre><code> python main.py --option value --option1 value1 value2  </code></pre>
 to check the available option run 
 <pre><code> python main.py -h </code></pre>
```

### Comparing `ALMASim-1.1.1/submodules/build/lib/illustris_python/groupcat.py` & `ALMASim-1.5/submodules/build/lib/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/build/lib/illustris_python/lhalotree.py` & `ALMASim-1.5/submodules/build/lib/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/build/lib/illustris_python/snapshot.py` & `ALMASim-1.5/submodules/build/lib/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/build/lib/illustris_python/sublink.py` & `ALMASim-1.5/submodules/build/lib/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/build/lib/illustris_python/util.py` & `ALMASim-1.5/submodules/build/lib/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/groupcat.py` & `ALMASim-1.5/submodules/illustris_python/groupcat.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/lhalotree.py` & `ALMASim-1.5/submodules/illustris_python/lhalotree.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/snapshot.py` & `ALMASim-1.5/submodules/illustris_python/snapshot.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/sublink.py` & `ALMASim-1.5/submodules/illustris_python/sublink.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/tests/groupcat_test.py` & `ALMASim-1.5/submodules/illustris_python/tests/groupcat_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/tests/snapshot_test.py` & `ALMASim-1.5/submodules/illustris_python/tests/snapshot_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/tests/sublink_test.py` & `ALMASim-1.5/submodules/illustris_python/tests/sublink_test.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/submodules/illustris_python/util.py` & `ALMASim-1.5/submodules/illustris_python/util.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/utility/generate_gaussian_params.py` & `ALMASim-1.5/utility/generate_gaussian_params.py`

 * *Files identical despite different names*

### Comparing `ALMASim-1.1.1/utility/split_data.py` & `ALMASim-1.5/utility/split_data.py`

 * *Files identical despite different names*

