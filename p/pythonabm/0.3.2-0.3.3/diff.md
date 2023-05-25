# Comparing `tmp/pythonabm-0.3.2.tar.gz` & `tmp/pythonabm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonabm-0.3.2.tar", last modified: Thu Apr 27 18:26:36 2023, max compression
+gzip compressed data, was "pythonabm-0.3.3.tar", last modified: Thu May 25 20:46:50 2023, max compression
```

## Comparing `pythonabm-0.3.2.tar` & `pythonabm-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-04-27 18:26:36.579666 pythonabm-0.3.2/
--rw-r--r--   0 jacktoppen   (501) staff       (20)      565 2021-12-30 02:18:00.000000 pythonabm-0.3.2/LICENSE.txt
--rw-r--r--   0 jacktoppen   (501) staff       (20)     2861 2023-04-27 18:26:36.579539 pythonabm-0.3.2/PKG-INFO
--rw-r--r--   0 jacktoppen   (501) staff       (20)     2663 2022-04-08 00:11:33.000000 pythonabm-0.3.2/README.md
-drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-04-27 18:26:36.578442 pythonabm-0.3.2/pythonabm/
--rw-r--r--   0 jacktoppen   (501) staff       (20)       51 2021-06-10 03:45:56.000000 pythonabm-0.3.2/pythonabm/__init__.py
--rw-r--r--   0 jacktoppen   (501) staff       (20)    18406 2022-03-21 23:51:39.000000 pythonabm-0.3.2/pythonabm/backend.py
--rw-r--r--   0 jacktoppen   (501) staff       (20)    34433 2023-04-27 18:02:18.000000 pythonabm-0.3.2/pythonabm/simulation.py
-drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-04-27 18:26:36.579295 pythonabm-0.3.2/pythonabm.egg-info/
--rw-r--r--   0 jacktoppen   (501) staff       (20)     2861 2023-04-27 18:26:36.000000 pythonabm-0.3.2/pythonabm.egg-info/PKG-INFO
--rw-r--r--   0 jacktoppen   (501) staff       (20)      261 2023-04-27 18:26:36.000000 pythonabm-0.3.2/pythonabm.egg-info/SOURCES.txt
--rw-r--r--   0 jacktoppen   (501) staff       (20)        1 2023-04-27 18:26:36.000000 pythonabm-0.3.2/pythonabm.egg-info/dependency_links.txt
--rw-r--r--   0 jacktoppen   (501) staff       (20)       77 2023-04-27 18:26:36.000000 pythonabm-0.3.2/pythonabm.egg-info/requires.txt
--rw-r--r--   0 jacktoppen   (501) staff       (20)       10 2023-04-27 18:26:36.000000 pythonabm-0.3.2/pythonabm.egg-info/top_level.txt
--rw-r--r--   0 jacktoppen   (501) staff       (20)       38 2023-04-27 18:26:36.579712 pythonabm-0.3.2/setup.cfg
--rw-r--r--   0 jacktoppen   (501) staff       (20)      656 2023-04-27 18:24:19.000000 pythonabm-0.3.2/setup.py
+drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-05-25 20:46:50.910255 pythonabm-0.3.3/
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)      565 2021-12-30 02:18:00.000000 pythonabm-0.3.3/LICENSE.txt
+-rw-r--r--   0 jacktoppen   (501) staff       (20)     2864 2023-05-25 20:46:50.910050 pythonabm-0.3.3/PKG-INFO
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)     2668 2023-05-25 20:05:09.000000 pythonabm-0.3.3/README.md
+drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-05-25 20:46:50.908715 pythonabm-0.3.3/pythonabm/
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)       51 2021-06-10 03:45:56.000000 pythonabm-0.3.3/pythonabm/__init__.py
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)    18406 2022-03-21 23:51:39.000000 pythonabm-0.3.3/pythonabm/backend.py
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)    35587 2023-05-25 20:38:35.000000 pythonabm-0.3.3/pythonabm/simulation.py
+drwxr-xr-x   0 jacktoppen   (501) staff       (20)        0 2023-05-25 20:46:50.909805 pythonabm-0.3.3/pythonabm.egg-info/
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)     2864 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/PKG-INFO
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)      293 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)        1 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/dependency_links.txt
+-rw-r--r--   0 jacktoppen   (501) staff       (20)        1 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/not-zip-safe
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)       77 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/requires.txt
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)       10 2023-05-25 20:46:50.000000 pythonabm-0.3.3/pythonabm.egg-info/top_level.txt
+-rw-r--r--   0 jacktoppen   (501) staff       (20)       38 2023-05-25 20:46:50.910330 pythonabm-0.3.3/setup.cfg
+-rwxrwxrwx   0 jacktoppen   (501) staff       (20)      677 2023-05-25 20:44:02.000000 pythonabm-0.3.3/setup.py
```

### Comparing `pythonabm-0.3.2/LICENSE.txt` & `pythonabm-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pythonabm-0.3.2/PKG-INFO` & `pythonabm-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonabm
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework for building Agent-Based Models (ABMs) in Python
 Author: Jack Toppen
 Author-email: jtoppen3@gatech.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -32,15 +32,15 @@
 Assuming you have Python 3.7-3.10, the latest version of the PythonABM library can be installed using the following command.
 ```
 pip install pythonabm
 ```
 
 PythonABM can also be built from [source](https://github.com/kemplab/pythonabm) once downloaded from GitHub.
 ```
-pip setup.py install
+python setup.py install
 ```
 
 ##
 
 ### Running a simulation
 Calling the start() method in the Simulation class will launch the ABM platform and run it as follows.
 (See the ***example.py*** script as a template for building a simulation.) A
```

### Comparing `pythonabm-0.3.2/README.md` & `pythonabm-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Assuming you have Python 3.7-3.10, the latest version of the PythonABM library can be installed using the following command.
 ```
 pip install pythonabm
 ```
 
 PythonABM can also be built from [source](https://github.com/kemplab/pythonabm) once downloaded from GitHub.
 ```
-pip setup.py install
+python setup.py install
 ```
 
 ##
 
 ### Running a simulation
 Calling the start() method in the Simulation class will launch the ABM platform and run it as follows.
 (See the ***example.py*** script as a template for building a simulation.) A
@@ -62,8 +62,8 @@
 [here](https://developer.nvidia.com/cuda-downloads) or with [Anaconda's](https://www.anaconda.com/) conda
 command show below.
 
 ```
 conda install cudatoolkit
 ```
 
-##
+##
```

### Comparing `pythonabm-0.3.2/pythonabm/backend.py` & `pythonabm-0.3.3/pythonabm/backend.py`

 * *Files identical despite different names*

### Comparing `pythonabm-0.3.2/pythonabm/simulation.py` & `pythonabm-0.3.3/pythonabm/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -799,7 +799,37 @@
                 cls.simulation_mode_1(name, output_dir)    # continuation
             elif mode == 2:
                 cls.simulation_mode_2(name, output_dir)    # images to video
             elif mode == 3:
                 cls.simulation_mode_3(name, output_dir)    # archive simulation
             else:
                 raise Exception("Mode does not exist!")
+
+
+    @classmethod
+    def make(cls, name, output_dir):
+        """ Creates a new brand new simulation and sets it up for
+            running within a separate script. Would need to call
+            run_simulation() on Simulation instance.
+
+            :param name: The name of the simulation.
+            :param output_dir: Path to simulation output directory.
+            :type name: str
+            :type output_dir: str
+        """
+        # get absolute path and check that the output directory exists
+        output_dir = os.path.abspath(os.path.expanduser(output_dir))
+        output_dir = check_output_dir(output_dir)
+        
+        # make simulation instance, update name, and add paths
+        sim = cls()
+        sim.name = name
+        sim.set_paths(output_dir)
+
+        # copy model files to simulation directory, ignoring __pycache__ files
+        direc_path = sim.main_path + name + "_copy"
+        shutil.copytree(os.getcwd(), direc_path, ignore=shutil.ignore_patterns("__pycache__", os.path.basename(output_dir[:-1])))
+
+        # set up the simulation agents 
+        sim.full_setup()
+
+        return sim
```

### Comparing `pythonabm-0.3.2/pythonabm.egg-info/PKG-INFO` & `pythonabm-0.3.3/pythonabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonabm
-Version: 0.3.2
+Version: 0.3.3
 Summary: Framework for building Agent-Based Models (ABMs) in Python
 Author: Jack Toppen
 Author-email: jtoppen3@gatech.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -32,15 +32,15 @@
 Assuming you have Python 3.7-3.10, the latest version of the PythonABM library can be installed using the following command.
 ```
 pip install pythonabm
 ```
 
 PythonABM can also be built from [source](https://github.com/kemplab/pythonabm) once downloaded from GitHub.
 ```
-pip setup.py install
+python setup.py install
 ```
 
 ##
 
 ### Running a simulation
 Calling the start() method in the Simulation class will launch the ABM platform and run it as follows.
 (See the ***example.py*** script as a template for building a simulation.) A
```

### Comparing `pythonabm-0.3.2/setup.py` & `pythonabm-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open('README.md') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pythonabm",
-    version="0.3.2",
+    version="0.3.3",
     author="Jack Toppen",
     author_email="jtoppen3@gatech.edu",
     description="Framework for building Agent-Based Models (ABMs) in Python",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=["pythonabm"],
     python_requires=">=3.7",
+    zip_safe=False,
     install_requires=[
         "matplotlib",
         "numpy>=1.11",
         "numba",
         "opencv-python",
         "psutil",
         "python-igraph",
```

