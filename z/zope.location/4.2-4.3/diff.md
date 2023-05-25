# Comparing `tmp/zope.location-4.2.tar.gz` & `tmp/zope.location-4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zope.location-4.2.tar", last modified: Tue Oct  9 13:43:18 2018, max compression
+gzip compressed data, was "zope.location-4.3.tar", last modified: Tue Nov 29 07:51:54 2022, max compression
```

## Comparing `zope.location-4.2.tar` & `zope.location-4.3.tar`

### file list

```diff
@@ -1,50 +1,45 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/
--rw-r--r--   0 mac        (501) staff       (20)     7458 2018-10-09 13:43:18.000000 zope.location-4.2/bootstrap.py
--rw-r--r--   0 mac        (501) staff       (20)    10745 2018-10-09 13:43:18.000000 zope.location-4.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      110 2018-10-09 13:43:18.000000 zope.location-4.2/rtd.txt
--rw-r--r--   0 mac        (501) staff       (20)       32 2018-10-09 13:43:18.000000 zope.location-4.2/COPYRIGHT.txt
--rw-r--r--   0 mac        (501) staff       (20)      385 2018-10-09 13:43:18.000000 zope.location-4.2/buildout.cfg
--rw-r--r--   0 mac        (501) staff       (20)      318 2018-10-09 13:43:18.000000 zope.location-4.2/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      190 2018-10-09 13:43:18.000000 zope.location-4.2/.coveragerc
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/docs/
--rw-r--r--   0 mac        (501) staff       (20)      204 2018-10-09 13:43:18.000000 zope.location-4.2/docs/index.rst
--rw-r--r--   0 mac        (501) staff       (20)     5588 2018-10-09 13:43:18.000000 zope.location-4.2/docs/Makefile
--rw-r--r--   0 mac        (501) staff       (20)     8006 2018-10-09 13:43:18.000000 zope.location-4.2/docs/conf.py
--rw-r--r--   0 mac        (501) staff       (20)     9132 2018-10-09 13:43:18.000000 zope.location-4.2/docs/hacking.rst
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/docs/_static/
--rw-r--r--   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/docs/_static/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)     5108 2018-10-09 13:43:18.000000 zope.location-4.2/docs/make.bat
--rw-r--r--   0 mac        (501) staff       (20)     4701 2018-10-09 13:43:18.000000 zope.location-4.2/docs/narr.rst
--rw-r--r--   0 mac        (501) staff       (20)    10844 2018-10-09 13:43:18.000000 zope.location-4.2/docs/api.rst
--rw-r--r--   0 mac        (501) staff       (20)     3400 2018-10-09 13:43:18.000000 zope.location-4.2/setup.py
--rw-r--r--   0 mac        (501) staff       (20)      135 2018-10-09 13:43:18.000000 zope.location-4.2/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)      967 2018-10-09 13:43:18.000000 zope.location-4.2/tox.ini
--rw-r--r--   0 mac        (501) staff       (20)      270 2018-10-09 13:43:18.000000 zope.location-4.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1228 2018-10-09 13:43:18.000000 zope.location-4.2/README.rst
--rw-r--r--   0 mac        (501) staff       (20)     2070 2018-10-09 13:43:18.000000 zope.location-4.2/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     6263 2018-10-09 13:43:18.000000 zope.location-4.2/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)      539 2018-10-09 13:43:18.000000 zope.location-4.2/.travis.yml
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    10745 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        1 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)        5 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)      985 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)      296 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        5 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope.location.egg-info/dependency_links.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/
--rw-r--r--   0 mac        (501) staff       (20)     4026 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)      679 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/configure.zcml
--rw-r--r--   0 mac        (501) staff       (20)     4511 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/traversing.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/
--rw-r--r--   0 mac        (501) staff       (20)        9 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1422 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/test_configure.py
--rw-r--r--   0 mac        (501) staff       (20)     2131 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/test_pickling.py
--rw-r--r--   0 mac        (501) staff       (20)    13850 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/test_location.py
--rw-r--r--   0 mac        (501) staff       (20)    10322 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/tests/test_traversing.py
--rw-r--r--   0 mac        (501) staff       (20)      868 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3731 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/location.py
--rw-r--r--   0 mac        (501) staff       (20)     1439 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/location/pickling.py
--rw-r--r--   0 mac        (501) staff       (20)       75 2018-10-09 13:43:18.000000 zope.location-4.2/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.912725 zope.location-4.3/
+-rw-r--r--   0 mac        (513) staff       (20)     6379 2022-11-29 07:51:51.000000 zope.location-4.3/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2022-11-29 07:51:51.000000 zope.location-4.3/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)       32 2022-11-29 07:51:51.000000 zope.location-4.3/COPYRIGHT.txt
+-rw-r--r--   0 mac        (513) staff       (20)     2070 2022-11-29 07:51:51.000000 zope.location-4.3/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)      373 2022-11-29 07:51:51.000000 zope.location-4.3/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     9099 2022-11-29 07:51:54.912955 zope.location-4.3/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     1271 2022-11-29 07:51:51.000000 zope.location-4.3/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      385 2022-11-29 07:51:51.000000 zope.location-4.3/buildout.cfg
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.901725 zope.location-4.3/docs/
+-rw-r--r--   0 mac        (513) staff       (20)     5588 2022-11-29 07:51:51.000000 zope.location-4.3/docs/Makefile
+-rw-r--r--   0 mac        (513) staff       (20)    10844 2022-11-29 07:51:51.000000 zope.location-4.3/docs/api.rst
+-rw-r--r--   0 mac        (513) staff       (20)     8006 2022-11-29 07:51:51.000000 zope.location-4.3/docs/conf.py
+-rw-r--r--   0 mac        (513) staff       (20)     9132 2022-11-29 07:51:51.000000 zope.location-4.3/docs/hacking.rst
+-rw-r--r--   0 mac        (513) staff       (20)      204 2022-11-29 07:51:51.000000 zope.location-4.3/docs/index.rst
+-rw-r--r--   0 mac        (513) staff       (20)     5108 2022-11-29 07:51:51.000000 zope.location-4.3/docs/make.bat
+-rw-r--r--   0 mac        (513) staff       (20)     4701 2022-11-29 07:51:51.000000 zope.location-4.3/docs/narr.rst
+-rw-r--r--   0 mac        (513) staff       (20)      110 2022-11-29 07:51:51.000000 zope.location-4.3/rtd.txt
+-rw-r--r--   0 mac        (513) staff       (20)      526 2022-11-29 07:51:54.914105 zope.location-4.3/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     3592 2022-11-29 07:51:51.000000 zope.location-4.3/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.890290 zope.location-4.3/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.902268 zope.location-4.3/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       76 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.909254 zope.location-4.3/src/zope/location/
+-rw-r--r--   0 mac        (513) staff       (20)      970 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)      679 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/configure.zcml
+-rw-r--r--   0 mac        (513) staff       (20)     4030 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/interfaces.py
+-rw-r--r--   0 mac        (513) staff       (20)     3730 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/location.py
+-rw-r--r--   0 mac        (513) staff       (20)     1479 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/pickling.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.912322 zope.location-4.3/src/zope/location/tests/
+-rw-r--r--   0 mac        (513) staff       (20)       10 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     1425 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/tests/test_configure.py
+-rw-r--r--   0 mac        (513) staff       (20)    13824 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/tests/test_location.py
+-rw-r--r--   0 mac        (513) staff       (20)     2113 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/tests/test_pickling.py
+-rw-r--r--   0 mac        (513) staff       (20)    10350 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/tests/test_traversing.py
+-rw-r--r--   0 mac        (513) staff       (20)     4518 2022-11-29 07:51:51.000000 zope.location-4.3/src/zope/location/traversing.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-11-29 07:51:54.906272 zope.location-4.3/src/zope.location.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     9099 2022-11-29 07:51:53.000000 zope.location-4.3/src/zope.location.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      929 2022-11-29 07:51:54.000000 zope.location-4.3/src/zope.location.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2022-11-29 07:51:53.000000 zope.location-4.3/src/zope.location.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2022-11-29 07:51:54.000000 zope.location-4.3/src/zope.location.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2022-11-29 07:51:53.000000 zope.location-4.3/src/zope.location.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)      296 2022-11-29 07:51:54.000000 zope.location-4.3/src/zope.location.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2022-11-29 07:51:54.000000 zope.location-4.3/src/zope.location.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1873 2022-11-29 07:51:51.000000 zope.location-4.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zope.location-4.2/docs/Makefile` & `zope.location-4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/docs/conf.py` & `zope.location-4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/docs/hacking.rst` & `zope.location-4.3/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/docs/make.bat` & `zope.location-4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/docs/narr.rst` & `zope.location-4.3/docs/narr.rst`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/docs/api.rst` & `zope.location-4.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/setup.py` & `zope.location-4.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,24 @@
 # http://docs.zope.org/zopetoolkit
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.location package
 """
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages
+from setuptools import setup
+
 
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
+
 ZCML_REQUIRES = [
     'zope.configuration',
 ]
 
 COMPONENT_REQUIRES = [
     'zope.component >= 4.0.1',
 ]
@@ -37,18 +41,18 @@
     'zope.copy >= 4.0',
     'zope.testrunner',
 ]
 
 DOCS_REQUIRE = [
     'Sphinx',
     'repoze.sphinx.autointerface',
-] + ZCML_REQUIRES + COMPONENT_REQUIRES # doctest snippets need these
+] + ZCML_REQUIRES + COMPONENT_REQUIRES  # doctest snippets need these
 
 setup(name='zope.location',
-      version='4.2',
+      version='4.3',
       author='Zope Corporation and Contributors',
       author_email='zope-dev@zope.org',
       description='Zope Location',
       long_description=(
           read('README.rst')
           + '\n\n' +
           read('CHANGES.rst')
@@ -60,29 +64,32 @@
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Programming Language :: Python',
           'Programming Language :: Python :: 2',
           'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.4',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Topic :: Internet :: WWW/HTTP',
-          'Framework :: Zope3',
+          'Framework :: Zope :: 3',
       ],
       url='http://github.com/zopefoundation/zope.location/',
       packages=find_packages('src'),
       package_dir={'': 'src'},
-      namespace_packages=['zope',],
+      namespace_packages=['zope', ],
       install_requires=[
           'setuptools',
           'zope.interface>=4.0.2',
           'zope.schema>=4.2.2',
           'zope.proxy>=4.0.1',
       ],
       extras_require={
@@ -90,8 +97,8 @@
           'component': COMPONENT_REQUIRES,
           'test': TESTS_REQUIRE,
           'docs': DOCS_REQUIRE,
       },
       test_suite='zope.location.tests',
       include_package_data=True,
       zip_safe=False,
-)
+      )
```

### Comparing `zope.location-4.2/README.rst` & `zope.location-4.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -6,24 +6,24 @@
         :target: https://pypi.python.org/pypi/zope.location/
         :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/zope.location.svg
         :target: https://pypi.org/project/zope.location/
         :alt: Supported Python versions
 
-.. image:: https://travis-ci.org/zopefoundation/zope.location.svg?branch=master
-        :target: https://travis-ci.org/zopefoundation/zope.location
+.. image:: https://github.com/zopefoundation/zope.location/actions/workflows/tests.yml/badge.svg
+        :target: https://github.com/zopefoundation/zope.location/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/zope.location/badge.svg?branch=master
         :target: https://coveralls.io/github/zopefoundation/zope.location?branch=master
 
 .. image:: https://readthedocs.org/projects/zopelocation/badge/?version=latest
         :target: http://zopelocation.readthedocs.org/en/latest/
         :alt: Documentation Status
 
-In Zope3, "locations" are special objects that have a structural
+In Zope 3, "locations" are special objects that have a structural
 location, indicated with ``__name__`` and ``__parent__`` attributes.
 
 See `zope.container <https://zopecontainer.readthedocs.io/en/latest>`_
 for a useful extension of this concept to "containers."
 
 Documentation is hosted at https://zopelocation.readthedocs.io/en/latest/
```

### Comparing `zope.location-4.2/LICENSE.txt` & `zope.location-4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/CHANGES.rst` & `zope.location-4.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+4.3 (2022-11-29)
+================
+
+- Add support for Python 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for Python 3.4.
+
+
 4.2 (2018-10-09)
 ================
 
 - Add support for Python 3.7.
 
 
 4.1.0 (2017-08-03)
```

### Comparing `zope.location-4.2/src/zope.location.egg-info/SOURCES.txt` & `zope.location-4.3/src/zope.location.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-.coveragerc
-.gitignore
-.travis.yml
 CHANGES.rst
+CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-bootstrap.py
 buildout.cfg
 rtd.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/hacking.rst
 docs/index.rst
 docs/make.bat
 docs/narr.rst
-docs/_static/.gitignore
 src/zope/__init__.py
 src/zope.location.egg-info/PKG-INFO
 src/zope.location.egg-info/SOURCES.txt
 src/zope.location.egg-info/dependency_links.txt
 src/zope.location.egg-info/namespace_packages.txt
 src/zope.location.egg-info/not-zip-safe
 src/zope.location.egg-info/requires.txt
```

### Comparing `zope.location-4.2/src/zope/location/interfaces.py` & `zope.location-4.3/src/zope/location/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Location framework interfaces
 """
 __docformat__ = 'restructuredtext'
 
-from zope.interface import Interface
 from zope.interface import Attribute
+from zope.interface import Interface
 from zope.schema import TextLine
 
 
 class ILocation(Interface):
     """Objects that can be located in a hierachy.
 
     Given a parent and a name an object can be located within that parent. The
@@ -48,17 +48,19 @@
         default=None)
 
 # The IContained interface was moved from zope.container to here in
 # zope.container 3.8.2 to break dependency cycles.  It is not actually
 # used within this package, but is depended upon by external
 # consumers.
 
+
 class IContained(ILocation):
     """Objects contained in containers."""
 
+
 class ILocationInfo(Interface):
     """Provides supplemental information for located objects.
 
     Requires that the object has been given a location in a hierarchy.
 
     """
 
@@ -117,16 +119,17 @@
     """Marker interface to designate root objects within a location hierarchy.
     """
 
 
 class LocationError(KeyError, LookupError):
     """There is no object for a given location."""
 
+
 # Soft dependency on zope.component.
 #
 # Also, these interfaces used to be defined here directly, so this provides
 # backward-compatibility
 try:
     from zope.component.interfaces import ISite
-except ImportError: # pragma: no cover
+except ImportError:  # pragma: no cover
     class ISite(Interface):
         pass
```

### Comparing `zope.location-4.2/src/zope/location/configure.zcml` & `zope.location-4.3/src/zope/location/configure.zcml`

 * *Files identical despite different names*

### Comparing `zope.location-4.2/src/zope/location/traversing.py` & `zope.location-4.3/src/zope/location/traversing.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 """
 __docformat__ = 'restructuredtext'
 
 from zope.interface import implementer
 
 from zope.location.interfaces import ILocationInfo
 from zope.location.interfaces import IRoot
-from zope.location.interfaces import ISite # zope.component, if present
+from zope.location.interfaces import ISite  # zope.component, if present
 
 
 @implementer(ILocationInfo)
 class LocationPhysicallyLocatable(object):
     """Provide location information for location objects
     """
+
     def __init__(self, context):
         self.context = context
 
     def getRoot(self):
         """See ILocationInfo.
         """
         context = self.context
@@ -80,15 +81,15 @@
     def getParents(self):
         """See ILocationInfo.
         """
         # XXX Merge this implementation with getPath. This was refactored
         # from zope.traversing.
         parents = []
         w = self.context
-        while 1:
+        while True:
             w = getattr(w, '__parent__', None)
             if w is None:
                 break
             parents.append(w)
 
         if parents and IRoot.providedBy(parents[-1]):
             return parents
@@ -106,22 +107,24 @@
         if ISite.providedBy(self.context):
             return self.context
         for parent in self.getParents():
             if ISite.providedBy(parent):
                 return parent
         return self.getRoot()
 
+
 @implementer(ILocationInfo)
 class RootPhysicallyLocatable(object):
     """Provide location information for the root object
 
     This adapter is very simple, because there's no places to search
     for parents and nearest sites, so we are only working with context
     object, knowing that its the root object already.
     """
+
     def __init__(self, context):
         self.context = context
 
     def getRoot(self):
         """See ILocationInfo
         """
         return self.context
```

### Comparing `zope.location-4.2/src/zope/location/tests/test_configure.py` & `zope.location-4.3/src/zope/location/tests/test_configure.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 """Test ZCML loading
 """
 import unittest
 
+
 class Test_ZCML_loads(unittest.TestCase):
 
     def test_it(self):
-        import zope.component # no registrations made if not present
+        import zope.component  # no registrations made if not present
         ADAPTERS_REGISTERED = 4
+        from zope.configuration.xmlconfig import XMLConfig
         from zope.configuration.xmlconfig import _clearContext
         from zope.configuration.xmlconfig import _getContext
-        from zope.configuration.xmlconfig import XMLConfig
+
         import zope.location
 
         _clearContext()
         context = _getContext()
         XMLConfig('configure.zcml', zope.location)
         adapters = ([x for x in context.actions
                      if x['discriminator'] is not None])
```

### Comparing `zope.location-4.2/src/zope/location/tests/test_pickling.py` & `zope.location-4.3/src/zope/location/tests/test_pickling.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,39 +10,38 @@
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 import unittest
 
 
-import zope.copy
-
 class LocationCopyHookTests(unittest.TestCase):
 
     def _getTargetClass(self):
         from zope.location.pickling import LocationCopyHook
         return LocationCopyHook
 
     def _makeOne(self, obj=None):
         if obj is None:
             obj = object()
         return self._getTargetClass()(obj)
 
     def test_class_conforms_to_ICopyHook(self):
-        from zope.interface.verify import verifyClass
         from zope.copy.interfaces import ICopyHook
+        from zope.interface.verify import verifyClass
         verifyClass(ICopyHook, self._getTargetClass())
 
     def test_instance_conforms_to_ICopyHook(self):
-        from zope.interface.verify import verifyObject
         from zope.copy.interfaces import ICopyHook
+        from zope.interface.verify import verifyObject
         verifyObject(ICopyHook, self._makeOne())
 
     def test___call___w_context_inside_toplevel(self):
         from zope.copy.interfaces import ResumeCopy
+
         class Dummy(object):
             __parent__ = __name__ = None
         top_level = Dummy()
         context = Dummy()
         context.__parent__ = top_level
         hook = self._makeOne(context)
         self.assertRaises(ResumeCopy, hook, top_level, object())
@@ -52,10 +51,9 @@
             __parent__ = __name__ = None
         top_level = Dummy()
         context = Dummy()
         hook = self._makeOne(context)
         self.assertTrue(hook(top_level, object()) is context)
 
 
-
 def test_suite():
     return unittest.defaultTestLoader.loadTestsFromName(__name__)
```

### Comparing `zope.location-4.2/src/zope/location/tests/test_location.py` & `zope.location-4.3/src/zope/location/tests/test_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 import unittest
 
 
 class ConformsToILocation(object):
 
     def test_class_conforms_to_ILocation(self):
         from zope.interface.verify import verifyClass
+
         from zope.location.interfaces import ILocation
         verifyClass(ILocation, self._getTargetClass())
 
     def test_instance_conforms_to_ILocation(self):
         from zope.interface.verify import verifyObject
+
         from zope.location.interfaces import ILocation
         verifyObject(ILocation, self._makeOne())
 
 
 class LocationTests(unittest.TestCase, ConformsToILocation):
 
     def _getTargetClass(self):
@@ -71,32 +73,37 @@
 
     def _callFUT(self, obj, *args, **kw):
         from zope.location.location import located
         return located(obj, *args, **kw)
 
     def test_wo_name_obj_implements_ILocation(self):
         from zope.interface import implementer
+
         from zope.location.interfaces import ILocation
+
         @implementer(ILocation)
         class Dummy(object):
             __parent__ = None
             __name__ = object()
         parent = Dummy()
         dummy = Dummy()
         self._callFUT(dummy, parent)
         self.assertTrue(dummy.__parent__ is parent)
         self.assertEqual(dummy.__name__, None)
 
     def test_w_name_adaptable_to_ILocation(self):
         from zope.interface.interface import adapter_hooks
+
         from zope.location.interfaces import ILocation
         _hooked = []
+
         def _hook(iface, obj):
             _hooked.append((iface, obj))
             return obj
+
         class Dummy(object):
             pass
         parent = Dummy()
         dummy = Dummy()
         before = adapter_hooks[:]
         adapter_hooks.insert(0, _hook)
         try:
@@ -202,37 +209,40 @@
         return ClassAndInstanceDescr
 
     def _makeOne(self, _inst, _class):
         return self._getTargetClass()(_inst, _class)
 
     def _makeScaffold(self):
         _inst_called = []
+
         def _inst(*args, **kw):
             _inst_called.append((args, kw))
             return 'INST'
         _class_called = []
+
         def _class(*args, **kw):
             _class_called.append((args, kw))
             return 'CLASS'
+
         class Foo(object):
             descr = self._makeOne(_inst, _class)
         return Foo, _class_called, _inst_called
 
     def test_fetched_from_class(self):
         Foo, _class_called, _inst_called = self._makeScaffold()
         self.assertEqual(Foo.descr, 'CLASS')
-        self.assertEqual(_class_called, [((Foo,),{})])
+        self.assertEqual(_class_called, [((Foo,), {})])
         self.assertEqual(_inst_called, [])
 
     def test_fetched_from_instance(self):
         Foo, _class_called, _inst_called = self._makeScaffold()
         foo = Foo()
         self.assertEqual(foo.descr, 'INST')
         self.assertEqual(_class_called, [])
-        self.assertEqual(_inst_called, [((foo,),{})])
+        self.assertEqual(_inst_called, [((foo,), {})])
 
 
 _MARKER = object()
 
 
 class LocationProxyTests(unittest.TestCase, ConformsToILocation):
 
@@ -246,21 +256,21 @@
         if container is _MARKER:
             self.assertIs(name, _MARKER)
             return self._getTargetClass()(obj)
         self.assertIsNot(name, _MARKER)
         return self._getTargetClass()(obj, container, name)
 
     def test_ctor_defaults(self):
-        dummy = object() # can't setattr
+        dummy = object()  # can't setattr
         proxy = self._makeOne(dummy)
         self.assertEqual(proxy.__parent__, None)
         self.assertEqual(proxy.__name__, None)
 
     def test_ctor_explicit(self):
-        dummy = object() # can't setattr
+        dummy = object()  # can't setattr
         parent = object()
         proxy = self._makeOne(dummy, parent, 'name')
         self.assertTrue(proxy.__parent__ is parent)
         self.assertEqual(proxy.__name__, 'name')
 
     def test___getattribute___wrapped(self):
         class Context(object):
@@ -275,27 +285,26 @@
         context = Context()
         proxy = self._makeOne(context)
         proxy.attr = 'AFTER'
         self.assertEqual(context.attr, 'AFTER')
 
     def test___doc___from_derived_class(self):
         klass = self._getTargetClass()
+
         class Derived(klass):
             """DERIVED"""
         self.assertEqual(Derived.__doc__, 'DERIVED')
 
     def test___doc___from_target_class(self):
-        klass = self._getTargetClass()
         class Context(object):
             """CONTEXT"""
         proxy = self._makeOne(Context())
         self.assertEqual(proxy.__doc__, 'CONTEXT')
 
     def test___doc___from_target_instance(self):
-        klass = self._getTargetClass()
         class Context(object):
             """CONTEXT"""
         context = Context()
         context.__doc__ = 'INSTANCE'
         proxy = self._makeOne(context)
         self.assertEqual(proxy.__doc__, 'INSTANCE')
 
@@ -305,74 +314,86 @@
 
     def test___reduce_ex__(self):
         proxy = self._makeOne()
         self.assertRaises(TypeError, proxy.__reduce_ex__, 1)
 
     def test___reduce___via_pickling(self):
         import pickle
+
         class Context(object):
             def __reduce__(self):
                 raise AssertionError("This is not called")
         proxy = self._makeOne(Context())
         # XXX: this TypeError is not due to LocationProxy.__reduce__:
         #      it's descriptor (under pure Python) isn't begin triggered
         #      properly
         self.assertRaises(TypeError, pickle.dumps, proxy)
 
     def test__providedBy___class(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import providedBy
         from zope.interface import provider
+
         class IProxyFactory(Interface):
             pass
+
         class IProxy(Interface):
             pass
+
         @provider(IProxyFactory)
         @implementer(IProxy)
         class Foo(self._getTargetClass()):
             pass
         self.assertEqual(list(providedBy(Foo)), [IProxyFactory])
 
     def test__providedBy___instance(self):
         from zope.interface import Interface
         from zope.interface import implementer
         from zope.interface import providedBy
         from zope.interface import provider
+
         from zope.location.interfaces import ILocation
+
         class IProxyFactory(Interface):
             pass
+
         class IProxy(Interface):
             pass
+
         class IContextFactory(Interface):
             pass
+
         class IContext(Interface):
             pass
+
         @provider(IProxyFactory)
         @implementer(IProxy)
         class Proxy(self._getTargetClass()):
             pass
+
         @provider(IContextFactory)
         @implementer(IContext)
         class Context(object):
             pass
         context = Context()
         proxy = Proxy(context)
-        self.assertEqual(list(providedBy(proxy)), [IContext, IProxy, ILocation])
+        self.assertEqual(list(providedBy(proxy)), [
+                         IContext, IProxy, ILocation])
 
 
 class LocationPyProxyTests(LocationProxyTests):
 
     def setUp(self):
         import sys
         for mod in ('zope.location.location',
                     'zope.proxy.decorator'):
             try:
                 del sys.modules[mod]
-            except KeyError: # pragma: no cover
+            except KeyError:  # pragma: no cover
                 pass
         import zope.proxy
         self.orig = (zope.proxy.ProxyBase,
                      zope.proxy.getProxiedObject,
                      zope.proxy.setProxiedObject,
                      zope.proxy.isProxy,
                      zope.proxy.sameProxiedObjects,
@@ -386,15 +407,14 @@
         zope.proxy.isProxy = zope.proxy.py_isProxy
         zope.proxy.sameProxiedObjects = zope.proxy.py_sameProxiedObjects
         zope.proxy.queryProxy = zope.proxy.py_queryProxy
         zope.proxy.queryInnerProxy = zope.proxy.py_queryInnerProxy
         zope.proxy.removeAllProxies = zope.proxy.py_removeAllProxies
         zope.proxy.non_overridable = zope.proxy.PyNonOverridable
 
-
     def tearDown(self):
         import zope.proxy
         (zope.proxy.ProxyBase,
          zope.proxy.getProxiedObject,
          zope.proxy.setProxiedObject,
          zope.proxy.isProxy,
          zope.proxy.sameProxiedObjects,
```

### Comparing `zope.location-4.2/src/zope/location/tests/test_traversing.py` & `zope.location-4.3/src/zope/location/tests/test_traversing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import unittest
 
 
 class ConformsToILocationInfo(object):
 
     def test_class_conforms_to_ILocationInfo(self):
         from zope.interface.verify import verifyClass
+
         from zope.location.interfaces import ILocationInfo
         verifyClass(ILocationInfo, self._getTargetClass())
 
     def test_instance_conforms_to_ILocationInfo(self):
         from zope.interface.verify import verifyObject
+
         from zope.location.interfaces import ILocationInfo
         verifyObject(ILocationInfo, self._makeOne())
 
 
 class LocationPhysicallyLocatableTests(
-                    unittest.TestCase, ConformsToILocationInfo):
+        unittest.TestCase, ConformsToILocationInfo):
 
     def _getTargetClass(self):
         from zope.location.traversing import LocationPhysicallyLocatable
         return LocationPhysicallyLocatable
 
     def _makeOne(self, obj=None):
         if obj is None:
@@ -47,15 +49,17 @@
         class Dummy(object):
             __parent__ = None
         proxy = self._makeOne(Dummy())
         self.assertRaises(TypeError, proxy.getRoot)
 
     def test_getRoot_wo_cycle(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         two = Dummy()
         two.__parent__ = one
         three = Dummy()
@@ -83,25 +87,29 @@
         class Dummy(object):
             __parent__ = __name__ = None
         proxy = self._makeOne(Dummy())
         self.assertRaises(TypeError, proxy.getPath)
 
     def test_getPath_at_root(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         proxy = self._makeOne(one)
         self.assertEqual(proxy.getPath(), '/')
 
     def test_getPath_wo_cycle(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         two = Dummy()
         two.__parent__ = one
         two.__name__ = 'two'
@@ -133,25 +141,29 @@
         class Dummy(object):
             __parent__ = __name__ = None
         proxy = self._makeOne(Dummy())
         self.assertRaises(TypeError, proxy.getParent)
 
     def test_getParent_at_root(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         proxy = self._makeOne(one)
         self.assertRaises(TypeError, proxy.getParent)
 
     def test_getParent_wo_cycle(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         two = Dummy()
         two.__parent__ = one
         two.__name__ = 'two'
@@ -169,25 +181,29 @@
         class Dummy(object):
             __parent__ = __name__ = None
         proxy = self._makeOne(Dummy())
         self.assertRaises(TypeError, proxy.getParents)
 
     def test_getParents_at_root(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         proxy = self._makeOne(one)
         self.assertRaises(TypeError, proxy.getParents)
 
     def test_getParents_wo_cycle(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         two = Dummy()
         two.__parent__ = one
         two.__name__ = 'two'
@@ -210,27 +226,33 @@
     def test_getName_location_w_name(self):
         class Dummy(object):
             __name__ = 'name'
         proxy = self._makeOne(Dummy())
         self.assertEqual(proxy.getName(), 'name')
 
     def test_getNearestSite_context_is_site(self):
-        from zope.location.interfaces import ISite # zope.component, if present
         from zope.interface import directlyProvides
+
+        from zope.location.interfaces import \
+            ISite  # zope.component, if present
+
         class Dummy(object):
             pass
         context = Dummy()
         directlyProvides(context, ISite)
         proxy = self._makeOne(context)
         self.assertTrue(proxy.getNearestSite() is context)
 
     def test_getNearestSite_ancestor_is_site(self):
-        from zope.location.interfaces import ISite # zope.component, if present
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+        from zope.location.interfaces import \
+            ISite  # zope.component, if present
+
         class Dummy(object):
             pass
         one = Dummy()
         directlyProvides(one, (ISite, IRoot))
         two = Dummy()
         two.__parent__ = one
         two.__name__ = 'two'
@@ -238,15 +260,17 @@
         three.__parent__ = two
         three.__name__ = 'three'
         proxy = self._makeOne(three)
         self.assertTrue(proxy.getNearestSite() is one)
 
     def test_getNearestSite_no_site(self):
         from zope.interface import directlyProvides
+
         from zope.location.interfaces import IRoot
+
         class Dummy(object):
             __parent__ = __name__ = None
         one = Dummy()
         directlyProvides(one, IRoot)
         two = Dummy()
         two.__parent__ = one
         two.__name__ = 'two'
@@ -254,15 +278,15 @@
         three.__parent__ = two
         three.__name__ = 'three'
         proxy = self._makeOne(three)
         self.assertTrue(proxy.getNearestSite() is one)
 
 
 class RootPhysicallyLocatableTests(
-                    unittest.TestCase, ConformsToILocationInfo):
+        unittest.TestCase, ConformsToILocationInfo):
 
     def _getTargetClass(self):
         from zope.location.traversing import RootPhysicallyLocatable
         return RootPhysicallyLocatable
 
     def _makeOne(self, obj=None):
         if obj is None:
```

### Comparing `zope.location-4.2/src/zope/location/location.py` & `zope.location-4.3/src/zope/location/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from zope.proxy import ProxyBase
 from zope.proxy import getProxiedObject
 from zope.proxy import non_overridable
 from zope.proxy.decorator import DecoratorSpecificationDescriptor
 
 from zope.location.interfaces import ILocation
 
+
 @implementer(ILocation)
 class Location(object):
     """Mix-in that implements ILocation.
 
     It provides the `__parent__` and `__name__` attributes.
     """
 
@@ -66,14 +67,15 @@
     """
     while l1 is not None:
         if l1 is l2:
             return True
         l1 = getattr(l1, '__parent__', None)
     return False
 
+
 class ClassAndInstanceDescr(object):
 
     def __init__(self, *args):
         self.funcs = args
 
     def __get__(self, inst, cls):
         if inst is None:
@@ -89,16 +91,16 @@
     don't implement `ILocation`.
     """
     __slots__ = ('__parent__', '__name__')
     __safe_for_unpickling__ = True
 
     __doc__ = ClassAndInstanceDescr(
         lambda inst: getProxiedObject(inst).__doc__,
-        lambda cls, __doc__ = __doc__: __doc__,
-        )
+        lambda cls, __doc__=__doc__: __doc__,
+    )
 
     def __new__(self, ob, container=None, name=None):
         return ProxyBase.__new__(self, ob)
 
     def __init__(self, ob, container=None, name=None):
         ProxyBase.__init__(self, ob)
         self.__parent__ = container
@@ -107,18 +109,18 @@
     def __getattribute__(self, name):
         if name in LocationProxy.__dict__:
             return object.__getattribute__(self, name)
         return ProxyBase.__getattribute__(self, name)
 
     def __setattr__(self, name, value):
         if name in self.__slots__ + getattr(ProxyBase, '__slots__', ()):
-            #('_wrapped', '__parent__', '__name__'):
+            # ('_wrapped', '__parent__', '__name__'):
             try:
                 return object.__setattr__(self, name, value)
-            except TypeError: #pragma NO COVER C Optimization
+            except TypeError:  # pragma NO COVER C Optimization
                 return ProxyBase.__setattr__(self, name, value)
         return ProxyBase.__setattr__(self, name, value)
 
     @non_overridable
     def __reduce__(self, proto=None):
         raise TypeError("Not picklable")
     __reduce_ex__ = __reduce__
```

### Comparing `zope.location-4.2/src/zope/location/pickling.py` & `zope.location-4.3/src/zope/location/pickling.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 #
 ##############################################################################
 """Location copying/pickling support
 """
 __docformat__ = 'restructuredtext'
 
 from zope.interface import implementer
+
 from zope.location.location import inside
 
+
 try:
-    from zope.copy.interfaces import ICopyHook, ResumeCopy
-except ImportError: # pragma: no cover
+    from zope.copy.interfaces import ICopyHook
+    from zope.copy.interfaces import ResumeCopy
+except ImportError:  # pragma: no cover
     raise NotImplementedError("zope.location.pickling is not supported "
                               "because zope.copy is not available")
 
 
 @implementer(ICopyHook)
 class LocationCopyHook(object):
     """Copy hook to preserve copying referenced objects that are not
     located inside object that's being copied.
     """
+
     def __init__(self, context):
         self.context = context
 
     def __call__(self, toplevel, register):
         if not inside(self.context, toplevel):
             return self.context
         raise ResumeCopy
```

