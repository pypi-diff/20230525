# Comparing `tmp/NanoPlot-1.9.2.tar.gz` & `tmp/NanoPlot-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NanoPlot-1.9.2.tar", last modified: Thu Jan 25 12:44:20 2018, max compression
+gzip compressed data, was "dist/NanoPlot-1.9.3.tar", last modified: Wed Feb  7 11:09:54 2018, max compression
```

## Comparing `NanoPlot-1.9.2.tar` & `NanoPlot-1.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/nanoplot/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)     2504 2017-11-20 16:07:10.000000 NanoPlot-1.9.2/nanoplot/utils.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       33 2017-08-22 08:56:42.000000 NanoPlot-1.9.2/nanoplot/__init__.py
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)       22 2018-01-25 12:21:05.000000 NanoPlot-1.9.2/nanoplot/version.py
--rwxrwxr-x   0 wdecoster  (1000) wdecoster  (1000)    23406 2018-01-25 12:26:24.000000 NanoPlot-1.9.2/nanoplot/NanoPlot.py
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       38 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/setup.cfg
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)    20832 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/PKG-INFO
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/scripts/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)      692 2017-12-05 09:25:17.000000 NanoPlot-1.9.2/scripts/test.sh
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       56 2017-11-06 07:59:30.000000 NanoPlot-1.9.2/MANIFEST.in
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/NanoPlot.egg-info/
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      120 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/NanoPlot.egg-info/requires.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       23 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/NanoPlot.egg-info/top_level.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)      345 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/NanoPlot.egg-info/SOURCES.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)    20832 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/NanoPlot.egg-info/PKG-INFO
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)       53 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/NanoPlot.egg-info/entry_points.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)        1 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/NanoPlot.egg-info/dependency_links.txt
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1775 2018-01-18 13:01:33.000000 NanoPlot-1.9.2/setup.py
-drwxr-xr-x   0 wdecoster  (1000) wdecoster  (1000)        0 2018-01-25 12:44:20.000000 NanoPlot-1.9.2/extra/
--rw-rw-r--   0 wdecoster  (1000) wdecoster  (1000)     1470 2017-09-28 12:26:08.000000 NanoPlot-1.9.2/extra/color_options.txt
--rw-r--r--   0 wdecoster  (1000) wdecoster  (1000)    17520 2018-01-25 12:44:19.000000 NanoPlot-1.9.2/README.rst
+drwxr-xr-x   0 wouter    (1000) wouter    (1000)        0 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/
+drwxr-xr-x   0 wouter    (1000) wouter    (1000)        0 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/nanoplot/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       33 2017-10-10 20:12:08.000000 NanoPlot-1.9.3/nanoplot/__init__.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       22 2018-02-07 11:09:30.000000 NanoPlot-1.9.3/nanoplot/version.py
+-rwxrwxr-x   0 wouter    (1000) wouter    (1000)    23399 2018-02-07 11:00:54.000000 NanoPlot-1.9.3/nanoplot/NanoPlot.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     2504 2017-11-22 22:15:09.000000 NanoPlot-1.9.3/nanoplot/utils.py
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1775 2018-02-06 14:31:14.000000 NanoPlot-1.9.3/setup.py
+drwxr-xr-x   0 wouter    (1000) wouter    (1000)        0 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/extra/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)     1470 2017-10-10 20:12:08.000000 NanoPlot-1.9.3/extra/color_options.txt
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)    17521 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/README.rst
+-rw-r--r--   0 wouter    (1000) wouter    (1000)    20833 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/PKG-INFO
+drwxr-xr-x   0 wouter    (1000) wouter    (1000)        0 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/
+-rw-r--r--   0 wouter    (1000) wouter    (1000)      120 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/requires.txt
+-rw-r--r--   0 wouter    (1000) wouter    (1000)        1 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter    (1000) wouter    (1000)    20833 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/PKG-INFO
+-rw-r--r--   0 wouter    (1000) wouter    (1000)      345 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter    (1000) wouter    (1000)       53 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/entry_points.txt
+-rw-r--r--   0 wouter    (1000) wouter    (1000)       23 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/NanoPlot.egg-info/top_level.txt
+-rw-r--r--   0 wouter    (1000) wouter    (1000)       38 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/setup.cfg
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)       56 2017-11-02 21:20:00.000000 NanoPlot-1.9.3/MANIFEST.in
+drwxr-xr-x   0 wouter    (1000) wouter    (1000)        0 2018-02-07 11:09:54.000000 NanoPlot-1.9.3/scripts/
+-rw-rw-r--   0 wouter    (1000) wouter    (1000)      692 2017-11-22 22:34:25.000000 NanoPlot-1.9.3/scripts/test.sh
```

### Comparing `NanoPlot-1.9.2/nanoplot/utils.py` & `NanoPlot-1.9.3/nanoplot/utils.py`

 * *Files identical despite different names*

### Comparing `NanoPlot-1.9.2/nanoplot/NanoPlot.py` & `NanoPlot-1.9.3/nanoplot/NanoPlot.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
                         help="Specify the output format of the plots.",
                         default="png",
                         type=str,
                         choices=['eps', 'jpeg', 'jpg', 'pdf', 'pgf', 'png', 'ps',
                                  'raw', 'rgba', 'svg', 'svgz', 'tif', 'tiff'])
     visual.add_argument("--plots",
                         help="Specify which bivariate plots have to be made.",
-                        default=['kde', 'hex', 'dot'],
+                        default=['kde', 'dot'],
                         type=str,
                         nargs='*',
                         choices=['kde', 'hex', 'dot', 'pauvre'])
     visual.add_argument("--listcolors",
                         help="List the colors which are available for plotting and exit.",
                         action=utils.Action_Print_Colors,
                         default=False)
```

### Comparing `NanoPlot-1.9.2/PKG-INFO` & `NanoPlot-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: NanoPlot
-Version: 1.9.2
+Version: 1.9.3
 Summary: Plotting suite for Oxford Nanopore sequencing data and alignments
 Home-page: https://github.com/wdecoster/NanoPlot
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: NanoPlot
@@ -98,15 +98,15 @@
               --barcoded            Use if you want to split the summary file by barcode
         
             Options for customizing the plots created:
               -c, --color COLOR     Specify a color for the plots, must be a valid matplotlib color
               -f, --format          Specify the output format of the plots.
                                     One of png [default], eps,jpeg,jpg,pdf,pgf,ps,raw,rgba,svg,svgz,tif,tiff
               --plots               Specify which bivariate plots have to be made.
-                                    One or more of kde (default), hex (default), dot (default), pauvre
+                                    One or more of 'dot' (default), 'kde' (default), 'hex' and 'pauvre'
               --listcolors          List the colors which are available for plotting and exit.
               --no-N50              Hide the N50 mark in the read length histogram
               --N50                 Show the N50 mark in the read length histogram
               --title TITLE         Add a title to all plots, requires quoting if using spaces
         
             Input data sources, one of these is required.:
               --fastq file [file ...]
```

### Comparing `NanoPlot-1.9.2/scripts/test.sh` & `NanoPlot-1.9.3/scripts/test.sh`

 * *Files identical despite different names*

### Comparing `NanoPlot-1.9.2/NanoPlot.egg-info/PKG-INFO` & `NanoPlot-1.9.3/NanoPlot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: NanoPlot
-Version: 1.9.2
+Version: 1.9.3
 Summary: Plotting suite for Oxford Nanopore sequencing data and alignments
 Home-page: https://github.com/wdecoster/NanoPlot
 Author: Wouter De Coster
 Author-email: decosterwouter@gmail.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: NanoPlot
@@ -98,15 +98,15 @@
               --barcoded            Use if you want to split the summary file by barcode
         
             Options for customizing the plots created:
               -c, --color COLOR     Specify a color for the plots, must be a valid matplotlib color
               -f, --format          Specify the output format of the plots.
                                     One of png [default], eps,jpeg,jpg,pdf,pgf,ps,raw,rgba,svg,svgz,tif,tiff
               --plots               Specify which bivariate plots have to be made.
-                                    One or more of kde (default), hex (default), dot (default), pauvre
+                                    One or more of 'dot' (default), 'kde' (default), 'hex' and 'pauvre'
               --listcolors          List the colors which are available for plotting and exit.
               --no-N50              Hide the N50 mark in the read length histogram
               --N50                 Show the N50 mark in the read length histogram
               --title TITLE         Add a title to all plots, requires quoting if using spaces
         
             Input data sources, one of these is required.:
               --fastq file [file ...]
```

### Comparing `NanoPlot-1.9.2/setup.py` & `NanoPlot-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `NanoPlot-1.9.2/extra/color_options.txt` & `NanoPlot-1.9.3/extra/color_options.txt`

 * *Files identical despite different names*

### Comparing `NanoPlot-1.9.2/README.rst` & `NanoPlot-1.9.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
       --barcoded            Use if you want to split the summary file by barcode
 
     Options for customizing the plots created:
       -c, --color COLOR     Specify a color for the plots, must be a valid matplotlib color
       -f, --format          Specify the output format of the plots.
                             One of png [default], eps,jpeg,jpg,pdf,pgf,ps,raw,rgba,svg,svgz,tif,tiff
       --plots               Specify which bivariate plots have to be made.
-                            One or more of kde (default), hex (default), dot (default), pauvre
+                            One or more of 'dot' (default), 'kde' (default), 'hex' and 'pauvre'
       --listcolors          List the colors which are available for plotting and exit.
       --no-N50              Hide the N50 mark in the read length histogram
       --N50                 Show the N50 mark in the read length histogram
       --title TITLE         Add a title to all plots, requires quoting if using spaces
 
     Input data sources, one of these is required.:
       --fastq file [file ...]
```

