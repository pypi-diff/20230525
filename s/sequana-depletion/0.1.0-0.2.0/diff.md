# Comparing `tmp/sequana_depletion-0.1.0.tar.gz` & `tmp/sequana_depletion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_depletion-0.1.0.tar", last modified: Fri Apr  1 13:34:36 2022, max compression
+gzip compressed data, was "sequana_depletion-0.2.0.tar", last modified: Thu May 25 10:51:05 2023, max compression
```

## Comparing `sequana_depletion-0.1.0.tar` & `sequana_depletion-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       66 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/.coveragerc
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/.github/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/.github/workflows/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1402 2022-04-01 12:55:42.000000 sequana_depletion-0.1.0/.github/workflows/main.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1036 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/.github/workflows/pypi.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1172 2022-04-01 12:42:00.000000 sequana_depletion-0.1.0/.gitignore
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      320 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/.workflow-index.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4152 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2867 2022-04-01 13:33:19.000000 sequana_depletion-0.1.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/conda.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       22 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/environment.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       50 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4152 2022-04-01 13:34:35.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      768 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-04-01 13:34:35.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       76 2022-04-01 13:34:35.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-03-30 16:00:31.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       50 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_depletion.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      784 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3156 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/depletion.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3801 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       22 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      672 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/sequana_pipelines/depletion/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      255 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3347 2022-04-01 13:34:25.000000 sequana_depletion-0.1.0/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-04-01 13:34:36.000000 sequana_depletion-0.1.0/singularity/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       58 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/singularity/Makefile
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      450 2022-04-01 12:41:44.000000 sequana_depletion-0.1.0/singularity/Singularity
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-25 10:51:05.871407 sequana_depletion-0.2.0/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-08-09 13:06:53.000000 sequana_depletion-0.2.0/LICENSE
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      149 2022-08-09 13:06:53.000000 sequana_depletion-0.2.0/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4203 2023-05-25 10:51:05.871407 sequana_depletion-0.2.0/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2947 2023-05-25 10:45:19.000000 sequana_depletion-0.2.0/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       36 2023-05-25 10:01:36.000000 sequana_depletion-0.2.0/requirements.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-25 10:51:05.871407 sequana_depletion-0.2.0/sequana_depletion.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4203 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      599 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       76 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-05-23 15:01:30.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       36 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2023-05-25 10:51:05.000000 sequana_depletion-0.2.0/sequana_depletion.egg-info/top_level.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-25 10:51:05.870407 sequana_depletion-0.2.0/sequana_pipelines/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-25 10:51:05.871407 sequana_depletion-0.2.0/sequana_pipelines/depletion/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      127 2022-08-09 13:06:53.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1295 2023-05-25 10:36:58.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/config.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4050 2023-05-25 10:22:38.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/depletion.rules
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3740 2023-05-25 10:06:30.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/main.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       22 2022-08-09 13:06:53.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      760 2023-05-25 09:04:20.000000 sequana_depletion-0.2.0/sequana_pipelines/depletion/schema.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      255 2023-05-25 10:51:05.872407 sequana_depletion-0.2.0/setup.cfg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3370 2023-05-25 10:46:38.000000 sequana_depletion-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sequana_depletion-0.1.0/LICENSE` & `sequana_depletion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sequana_depletion-0.1.0/PKG-INFO` & `sequana_depletion-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: sequana_depletion
-Version: 0.1.0
-Summary: Deplete or select reads from Fastq files
+Version: 0.2.0
+Summary: A short description
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
-Keywords: sequana,NGS,workflows,depletion
+Keywords: A list of keywords separated by commas
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -88,15 +88,14 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
 
 - bwa
-- bioconvert
 - samtools
 - bamtools
 
 #.. image:: https://raw.githubusercontent.com/sequana/depletion/master/sequana_pipelines/depletion/dag.png
 
 
 Details
@@ -114,13 +113,13 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+0.2.0     * handle paired/unpaired data
+          * refactorise to use containers/apptainers
 0.1.0     **First release.**
 ========= ====================================================================
 
 
-
-
```

### Comparing `sequana_depletion-0.1.0/README.rst` & `sequana_depletion-0.2.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
 
 - bwa
-- bioconvert
 - samtools
 - bamtools
 
 #.. image:: https://raw.githubusercontent.com/sequana/depletion/master/sequana_pipelines/depletion/dag.png
 
 
 Details
@@ -81,11 +80,13 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+0.2.0     * handle paired/unpaired data
+          * refactorise to use containers/apptainers
 0.1.0     **First release.**
 ========= ====================================================================
```

### Comparing `sequana_depletion-0.1.0/sequana_depletion.egg-info/PKG-INFO` & `sequana_depletion-0.2.0/sequana_depletion.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: sequana-depletion
-Version: 0.1.0
-Summary: Deplete or select reads from Fastq files
+Version: 0.2.0
+Summary: A short description
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
-Keywords: sequana,NGS,workflows,depletion
+Keywords: A list of keywords separated by commas
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
 License-File: LICENSE
@@ -88,15 +88,14 @@
 
 Requirements
 ~~~~~~~~~~~~
 
 This pipelines requires the following executable(s):
 
 - bwa
-- bioconvert
 - samtools
 - bamtools
 
 #.. image:: https://raw.githubusercontent.com/sequana/depletion/master/sequana_pipelines/depletion/dag.png
 
 
 Details
@@ -114,13 +113,13 @@
 
 Changelog
 ~~~~~~~~~
 
 ========= ====================================================================
 Version   Description
 ========= ====================================================================
+0.2.0     * handle paired/unpaired data
+          * refactorise to use containers/apptainers
 0.1.0     **First release.**
 ========= ====================================================================
 
 
-
-
```

### Comparing `sequana_depletion-0.1.0/sequana_pipelines/depletion/main.py` & `sequana_depletion-0.2.0/sequana_pipelines/depletion/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sys
 import os
 import argparse
 import shutil
 import subprocess
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
 from sequana_pipetools import SequanaManager
 
 col = Colors()
 
 NAME = "depletion"
@@ -32,15 +33,14 @@
         super(Options, self).__init__(
             usage=usage,
             prog=prog,
             description="",
             epilog=epilog,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
-
         # add a new group of options to the parser
         so = SlurmOptions()
         so.add_options(self)
 
         # add a snakemake group of options to the parser
         so = SnakemakeOptions(working_directory=NAME)
         so.add_options(self)
@@ -53,14 +53,16 @@
 
         pipeline_group = self.add_argument_group("pipeline")
 
         pipeline_group.add_argument("--mode", dest="mode", required=True, choices=["selection", "depletion"])
         pipeline_group.add_argument("--reference", dest="reference", required=True, 
             help="reference from which to select or deplete reads")
 
+        self.add_argument("--run", default=False, action="store_true", help="execute the pipeline directly")
+
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
             if len(args_list) > 2:
                 msg = (
                     "WARNING [sequana]: With --from-project option, "
                     + "pipeline and data-related options will be ignored."
@@ -75,43 +77,37 @@
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
     # whatever needs to be called by all pipeline before the options parsing
-    from sequana_pipetools.options import before_pipeline
-
     before_pipeline(NAME)
 
     # option parsing including common epilog
     options = Options(NAME, epilog=sequana_epilog).parse_args(args[1:])
 
     # the real stuff is here
     manager = SequanaManager(options, NAME)
 
     # create the beginning of the command and the working directory
     manager.setup()
-    from sequana import logger
-
-    logger.setLevel(options.level)
-    logger.name = "sequana_depletion"
-    logger.info(f"#Welcome to sequana_depletion pipeline.")
 
     # fill the config file with input parameters
     if options.from_project is None:
-        # fill the config file with input parameters
         cfg = manager.config.config
-        # EXAMPLE TOREPLACE WITH YOUR NEEDS
         cfg.input_directory = os.path.abspath(options.input_directory)
         cfg.input_pattern = options.input_pattern
         manager.exists(cfg.input_directory)
         cfg.general.mode = options.mode
         cfg.general.reference = os.path.abspath(options.reference)
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
+    if options.run:
+        subprocess.Popen(["sh", "{}.sh".format(NAME)], cwd=options.workdir)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_depletion-0.1.0/sequana_pipelines/depletion/schema.yaml` & `sequana_depletion-0.2.0/sequana_pipelines/depletion/schema.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -8,24 +8,32 @@
         required: False
     "input_readtag":
         type: str
         required: False
     "input_pattern":
         type: str
         required: False
+
     "general":
         type: map
         mapping:
             "reference":
                type: str
                required: True
             "mode":
                type: str
                required: True
                enum: [selection, depletion]
-    "depletion_selection":
-        type: map
-        mapping:
+
+    "apptainers":
+        type: any
+
+    "mapping":
+      type: map
+      mapping:
           "threads":
-                type: int
-                range: { min: 1}
+             type: int
+             range: { min: 1}
+          "options":
+            type: str
+            required: False
```

### Comparing `sequana_depletion-0.1.0/setup.py` & `sequana_depletion-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,40 @@
 
 # handle sequana git link
 with open("requirements.txt") as fh:
     requirements = [req.rstrip() if not req.startswith("git+") else req.rstrip().split("egg=")[-1] for req in fh]
 
 
 _MAJOR               = 0
-_MINOR               = 1
+_MINOR               = 2
 _MICRO               = 0
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
     'url' : "https://github.com/sequana/",
-    'description': "Deplete or select reads from Fastq files" ,
+    'description': "A short description" ,
     'platforms' : ['Linux', 'Unix', 'MacOsX', 'Windows'],
-    'keywords' : ["sequana", "NGS", "workflows","depletion"],
+    'keywords' : ['A list of keywords separated by commas'],
     'classifiers' : [
-          'Development Status :: 5 - Production/Stable',
+          'Development Status :: 4 - Beta',
+          #'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
+          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
```

