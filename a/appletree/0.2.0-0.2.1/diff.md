# Comparing `tmp/appletree-0.2.0.tar.gz` & `tmp/appletree-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appletree-0.2.0.tar", last modified: Wed Mar 15 17:24:53 2023, max compression
+gzip compressed data, was "appletree-0.2.1.tar", last modified: Mon May 22 06:06:22 2023, max compression
```

## Comparing `appletree-0.2.0.tar` & `appletree-0.2.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:50.000000 appletree-0.2.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-15 17:24:50.000000 appletree-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-15 17:24:50.000000 appletree-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-15 17:24:53.536148 appletree-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-15 17:24:50.000000 appletree-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/appletree/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20431 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/appletree/components/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/components/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/components/er.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/components/nr.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/components/yields.py
--rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13117 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/appletree/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/contexts/er_only.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/appletree/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/er_microphys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/lyqy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/nestv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/plugins/reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/randgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/share.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-03-15 17:24:50.000000 appletree-0.2.0/appletree/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 17:24:53.536148 appletree-0.2.0/appletree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 17:24:53.000000 appletree-0.2.0/appletree.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-15 17:24:50.000000 appletree-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-15 17:24:53.536148 appletree-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-15 17:24:50.000000 appletree-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-22 06:06:13.000000 appletree-0.2.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 06:06:13.000000 appletree-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 06:06:13.000000 appletree-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-22 06:06:22.093899 appletree-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 06:06:13.000000 appletree-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/appletree/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20163 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/appletree/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/components/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/components/er.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/components/nr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/components/yields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14310 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/appletree/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/contexts/er_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/appletree/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/er_microphys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/lyqy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/nestv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/plugins/reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/randgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-05-22 06:06:13.000000 appletree-0.2.1/appletree/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:22.093899 appletree-0.2.1/appletree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-22 06:06:21.000000 appletree-0.2.1/appletree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 06:06:22.000000 appletree-0.2.1/appletree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:06:21.000000 appletree-0.2.1/appletree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:06:21.000000 appletree-0.2.1/appletree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 06:06:21.000000 appletree-0.2.1/appletree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 06:06:21.000000 appletree-0.2.1/appletree.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-22 06:06:13.000000 appletree-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-22 06:06:22.097899 appletree-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 06:06:13.000000 appletree-0.2.1/setup.py
```

### Comparing `appletree-0.2.0/LICENSE` & `appletree-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/README.md` & `appletree-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 # Appletree
 A high-Performance Program simuLatEs and fiTs REsponse of xEnon.
 
+[![DOI](https://zenodo.org/badge/534803881.svg)](https://zenodo.org/badge/latestdoi/534803881)
 [![Test package](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml/badge.svg?branch=master)](https://github.com/XENONnT/appletree/actions/workflows/pytest.yml)
 [![Coverage Status](https://coveralls.io/repos/github/XENONnT/appletree/badge.svg)](https://coveralls.io/github/XENONnT/appletree)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/appletree.svg)](https://pypi.python.org/pypi/appletree/)
 [![Readthedocs Badge](https://readthedocs.org/projects/appletree/badge/?version=latest)](https://appletree.readthedocs.io/en/latest/?badge=latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/xenonnt/appletree/badge)](https://www.codefactor.io/repository/github/xenonnt/appletree)
 
 ## Installation and Set-Up
 
 ### Regular installation:
 ```
-pip install appletree
+pip install appletree -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ### Developer setup:
 Clone the repository:
 
 ```
 git clone https://github.com/XENONnT/appletree
 cd appletree
 ```
-Install the requirements in your environment:
+
+Install the package and requirements in your environment:
+
 ```
 pip install -r requirements.txt
+python setup.py install --user
 ```
 
-Then install the package:
+If you wanna install appletree in editable mode, replace the last line with
+
 ```
-python setup.py install --user
+pip install -e ./ --user
 ```
+
 You are now good to go!
 
 ## Usage
 The best way to start with the `appletree` package is to have a look at the tutorial `notebooks`. 
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `appletree-0.2.0/appletree/__init__.py` & `appletree-0.2.1/appletree/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 from . import utils
 from .utils import *
 
 from . import hist
 from .hist import *
 
@@ -36,7 +36,15 @@
 from .likelihood import *
 
 from . import contexts
 from .contexts import *
 
 from . import context
 from .context import *
+
+try:
+    import aptext
+    HAVE_APTEXT = True
+    print('Using aptext package from https://github.com/XENONnT/applefiles')
+except ImportError:
+    HAVE_APTEXT = False
+    print('Can not find aptext')
```

### Comparing `appletree-0.2.0/appletree/component.py` & `appletree-0.2.1/appletree/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from warnings import warn
 from functools import partial
 
 import numpy as np
 import pandas as pd
 from jax import numpy as jnp
-import pandas as pd
 
 import appletree
 from appletree import utils
 from appletree.plugin import Plugin
 from appletree.share import _cached_configs, _cached_functions, set_global_config
 from appletree.utils import exporter, load_data
 from appletree.hist import make_hist_mesh_grid, make_hist_irreg_bin_2d
@@ -166,19 +165,14 @@
         """Register a plugin to the component."""
         if isinstance(plugin_class, (tuple, list)):
             # Shortcut for multiple registration
             for x in plugin_class:
                 self.register(x)
             return
 
-        if not hasattr(plugin_class, 'provides'):
-            # No output name specified: construct one from the class name
-            snake_name = appletree.camel_to_snake(plugin_class.__name__)
-            plugin_class.provides = (snake_name,)
-
         # Ensure plugin_class.provides is a tuple
         if isinstance(plugin_class.provides, str):
             plugin_class.provides = tuple([plugin_class.provides])
 
         for p in plugin_class.provides:
             self._plugin_class_registry[p] = plugin_class
```

### Comparing `appletree-0.2.0/appletree/components/er.py` & `appletree-0.2.1/appletree/components/er.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/components/nr.py` & `appletree-0.2.1/appletree/components/nr.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/components/yields.py` & `appletree-0.2.1/appletree/components/yields.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/config.py` & `appletree-0.2.1/appletree/config.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/context.py` & `appletree-0.2.1/appletree/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from warnings import warn
 import os
 import copy
 import json
 import importlib
 from datetime import datetime
 import numpy as np
 import emcee
@@ -121,14 +122,29 @@
 
         print('\n'+'='*40)
         for key, likelihood in self.likelihoods.items():
             print(f'LIKELIHOOD {key}')
             likelihood.print_likelihood_summary(short=short)
             print('\n'+'='*40)
 
+    def get_num_events_accepted(self, parameters, batch_size=1_000_000):
+        """Get number of events in the histogram under given parameters.
+
+        :param batch_size: int of number of simulated events
+        :param parameters: dict of parameters used in simulation
+        """
+        n_events = 0
+        for likelihood in self.likelihoods.values():
+            if hasattr(likelihood, 'data_hist'):
+                n_events += likelihood.get_num_events_accepted(batch_size, parameters)
+            else:
+                warning = f'{likelihood.name} will be omitted.'
+                warn(warning)
+        return n_events
+
     def log_posterior(self, parameters, batch_size=1_000_000):
         """Get log likelihood of given parameters
 
         :param batch_size: int of number of simulated events
         :param parameters: dict of parameters used in simulation
         """
         self.par_manager.set_parameter(parameters)
```

### Comparing `appletree-0.2.0/appletree/contexts/er_only.py` & `appletree-0.2.1/appletree/contexts/er_only.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/hist.py` & `appletree-0.2.1/appletree/hist.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/interpolation.py` & `appletree-0.2.1/appletree/interpolation.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/likelihood.py` & `appletree-0.2.1/appletree/likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from warnings import warn
 
 import numpy as np
 from jax import numpy as jnp
 
 from scipy.stats import norm
 
+from appletree import randgen
 from appletree.hist import make_hist_mesh_grid, make_hist_irreg_bin_2d
 from appletree.utils import load_data, get_equiprob_bins_2d
 from appletree.component import Component, ComponentSim, ComponentFixed
 from appletree.randgen import TwoHalfNorm, BandTwoHalfNorm
 
 
 class Likelihood:
@@ -188,14 +189,24 @@
         # Poisson likelihood
         llh = jnp.sum(self.data_hist * jnp.log(model_hist) - model_hist)
         llh = float(llh)
         if np.isnan(llh):
             llh = -np.inf
         return key, llh
 
+    def get_num_events_accepted(self, batch_size, parameters):
+        """Get number of events in the histogram under given parameters.
+
+        :param batch_size: int of number of simulated events
+        :param parameters: dict of parameters used in simulation
+        """
+        key = randgen.get_key()
+        _, model_hist = self._simulate_model_hist(key, batch_size, parameters)
+        return model_hist.sum()
+
     def print_likelihood_summary(self,
                                  indent: str = ' '*4,
                                  short: bool = True):
         """Print likelihood summary: components, bins, file names.
 
         :param indent: str of indent
         :param short: bool, whether only print short summary
```

### Comparing `appletree-0.2.0/appletree/parameter.py` & `appletree-0.2.1/appletree/parameter.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/plugin.py` & `appletree-0.2.1/appletree/plugin.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/plugins/common.py` & `appletree-0.2.1/appletree/plugins/common.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/plugins/detector.py` & `appletree-0.2.1/appletree/plugins/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 export, __all__ = exporter(export_self=False)
 
 
 @export
 @appletree.takes_config(
     Map(name='s1_lce',
-        default='s1_correction_map.json',
+        default='s1_correction_map_regbin.json',
         help='S1 light collection efficiency correction'),
 )
 class S1Correction(Plugin):
     depends_on = ['rec_x', 'rec_y', 'rec_z']
     provides = ['s1_correction']
 
     @partial(jit, static_argnums=(0, ))
@@ -27,15 +27,15 @@
         s1_correction = self.s1_lce.apply(pos)
         return key, s1_correction
 
 
 @export
 @appletree.takes_config(
     Map(name='s2_lce',
-        default='s2_correction_map.json',
+        default='s2_correction_map_regbin.json',
         help='S2 light collection efficiency correction'),
 )
 class S2Correction(Plugin):
     depends_on = ['rec_x', 'rec_y']
     provides = ['s2_correction']
 
     @partial(jit, static_argnums=(0, ))
```

### Comparing `appletree-0.2.0/appletree/plugins/efficiency.py` & `appletree-0.2.1/appletree/plugins/efficiency.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from appletree.utils import exporter
 
 export, __all__ = exporter(export_self=False)
 
 
 @export
 class S2Threshold(Plugin):
-    depends_on = ['s2']
+    depends_on = ['s2_area']
     provides = ['acc_s2_threshold']
     parameters = ('s2_threshold',)
 
     @partial(jit, static_argnums=(0, ))
-    def simulate(self, key, parameters, s2):
-        return key, jnp.where(s2 > parameters['s2_threshold'], 1., 0)
+    def simulate(self, key, parameters, s2_area):
+        return key, jnp.where(s2_area > parameters['s2_threshold'], 1., 0)
 
 
 @export
 @appletree.takes_config(
     SigmaMap(name='s1_eff_3f',
         default=[
             '3fold_recon_eff.json',
@@ -49,42 +49,42 @@
         default=[
             's1_cut_acc.json',
             's1_cut_acc.json',
             's1_cut_acc.json'],
         help='S1 cut acceptance'),
 )
 class S1CutAccept(Plugin):
-    depends_on = ['s1']
+    depends_on = ['s1_area']
     provides = ['cut_acc_s1']
     parameters = ('s1_cut_acc_sigma',)
 
     @partial(jit, static_argnums=(0, ))
-    def simulate(self, key, parameters, s1):
-        cut_acc_s1 = self.s1_cut_acc.apply(s1, parameters)
+    def simulate(self, key, parameters, s1_area):
+        cut_acc_s1 = self.s1_cut_acc.apply(s1_area, parameters)
         cut_acc_s1 = jnp.clip(cut_acc_s1, 0., 1.)
         return key, cut_acc_s1
 
 
 @export
 @appletree.takes_config(
     SigmaMap(name='s2_cut_acc',
         default=[
             's2_cut_acc.json',
             's2_cut_acc.json',
             's2_cut_acc.json'],
         help='S2 cut acceptance'),
 )
 class S2CutAccept(Plugin):
-    depends_on = ['s2']
+    depends_on = ['s2_area']
     provides = ['cut_acc_s2']
     parameters = ('s2_cut_acc_sigma',)
 
     @partial(jit, static_argnums=(0, ))
-    def simulate(self, key, parameters, s2):
-        cut_acc_s2 = self.s2_cut_acc.apply(s2, parameters)
+    def simulate(self, key, parameters, s2_area):
+        cut_acc_s2 = self.s2_cut_acc.apply(s2_area, parameters)
         cut_acc_s2 = jnp.clip(cut_acc_s2, 0., 1.)
         return key, cut_acc_s2
 
 
 @export
 class Eff(Plugin):
     depends_on = ['acc_s2_threshold', 'acc_s1_recon_eff', 'cut_acc_s1', 'cut_acc_s2']
```

### Comparing `appletree-0.2.0/appletree/plugins/er_microphys.py` & `appletree-0.2.1/appletree/plugins/er_microphys.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/plugins/lyqy.py` & `appletree-0.2.1/appletree/plugins/lyqy.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/plugins/nestv2.py` & `appletree-0.2.1/appletree/plugins/nestv2.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/randgen.py` & `appletree-0.2.1/appletree/randgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 
 from appletree.utils import exporter
 
 export, __all__ = exporter(export_self=False)
 
 INT = np.int32
 FLOAT = np.float32
-ALWAYS_USE_NORMAL_APPROX_IN_BINOM = bool(
-    os.environ.get('ALWAYS_USE_NORMAL_APPROX_IN_BINOM', True))
+
+if os.environ.get('DO_NOT_USE_APPROX_IN_BINOM') is None:
+    ALWAYS_USE_NORMAL_APPROX_IN_BINOM = True
+    print('Using Normal as an approximation of Binomial')
+else:
+    ALWAYS_USE_NORMAL_APPROX_IN_BINOM = False
+    print('Using accurate Binomial, not Normal approximation')
 
 
 @export
 def get_key(seed=None):
     """Generate a key for jax.random."""
     if seed is None:
         seed = int(time()*1e6)
@@ -189,28 +194,28 @@
             (seed, p, n), lambda x: _binomial_normal_approx_dispatch(*x),
             (seed, p, n), lambda x: _binomial_dispatch_numpyro(*x),
         )
 
     key, seed = random.split(key)
 
     shape = shape or lax.broadcast_shapes(jnp.shape(p), jnp.shape(n))
-    p = jnp.reshape(jnp.broadcast_to(p, shape), -1).astype(FLOAT)
-    n = jnp.reshape(jnp.broadcast_to(n, shape), -1).astype(INT)
+    p = jnp.reshape(jnp.broadcast_to(p, shape), -1)
+    n = jnp.reshape(jnp.broadcast_to(n, shape), -1)
     seed = random.split(seed, jnp.size(p))
 
     if always_use_normal:
         dispatch = _binomial_normal_approx_dispatch
     else:
         dispatch = _binomial_dispatch
 
     if jax.default_backend() == "cpu":
         ret = lax.map(lambda x: dispatch(*x), (seed, p, n))
     else:
         ret = vmap(lambda *x: dispatch(*x))(seed, p, n)
-    return key, jnp.reshape(ret, shape).astype(INT)
+    return key, jnp.reshape(ret, shape)
 
 
 @export
 @jit
 def uniform_key_vectorized(key):
     """Uniform(0,1) distribution sampler, vectorized by key.
     Note: key won't be updated!
```

### Comparing `appletree-0.2.0/appletree/share.py` & `appletree-0.2.1/appletree/share.py`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/appletree/utils.py` & `appletree-0.2.1/appletree/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import re
 import json
 from warnings import warn
 import pkg_resources
 from time import time
 
+from jax.lib import xla_bridge
 import numpy as np
 import pandas as pd
 import matplotlib as mpl
 from matplotlib.patches import Rectangle
 from matplotlib import pyplot as plt
 
 import GOFevaluation
@@ -87,23 +88,14 @@
     """Load data from json file."""
     with open(get_file_path(file_name), 'r') as file:
         data = json.load(file)
     return data
 
 
 @export
-def camel_to_snake(x):
-    """Convert x from CamelCase to snake_case,
-    from https://stackoverflow.com/questions/1175208
-    """
-    x = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', x)
-    return re.sub('([a-z0-9])([A-Z])', r'\1_\2', x).lower()
-
-
-@export
 def _get_abspath(file_name):
     """Get the abspath of the file. Raise FileNotFoundError when not found in any subfolder"""
     for sub_dir in ('maps', 'data', 'parameters', 'instructs'):
         p = os.path.join(_package_path(sub_dir), file_name)
         if os.path.exists(p):
             return p
     raise FileNotFoundError(f'Cannot find {file_name}')
@@ -197,14 +189,20 @@
     if isinstance(indent, str):
         return lambda func: _timeit(func, indent)
     else:
         return _timeit(indent, "")
 
 
 @export
+def get_platform():
+    """Show the platform we are using, either cpu ot gpu"""
+    return xla_bridge.get_backend().platform
+
+
+@export
 def set_gpu_memory_usage(fraction=0.3):
     """Set GPU memory usage.
     See more on https://jax.readthedocs.io/en/latest/gpu_memory_allocation.html
     """
     if fraction > 1:
         fraction = 1
     if fraction <= 0:
```

### Comparing `appletree-0.2.0/appletree.egg-info/SOURCES.txt` & `appletree-0.2.1/appletree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/setup.cfg` & `appletree-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `appletree-0.2.0/setup.py` & `appletree-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import setuptools
 
 
 def open_requirements(path):
     with open(path) as f:
         requires = [
             r.split('/')[-1] if r.startswith('git+') else r
-            for r in f.read().splitlines()]
+            for r in f.read().splitlines() if not r.startswith('-')]
     return requires
 
 
 requires = open_requirements('requirements.txt')
 
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(
     name='appletree',
-    version='0.2.0',
+    version='0.2.1',
     description='A high-Performance Program simuLatEs and fiTs REsponse of xEnon.',
     author='Appletree contributors, the XENON collaboration',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/markdown',
     setup_requires=['pytest-runner'],
     install_requires=requires,
     python_requires='>=3.8',
@@ -33,15 +33,15 @@
             'pytest',
             'flake8',
         ],
     },
     packages=setuptools.find_packages(),
     url="https://github.com/XENONnT/appletree",
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering :: Physics',
```

