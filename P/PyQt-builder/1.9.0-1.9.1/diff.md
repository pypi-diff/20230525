# Comparing `tmp/PyQt-builder-1.9.0.tar.gz` & `tmp/PyQt-builder-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "./PyQt-builder-1.9.0.tar", last modified: Mon Feb 22 17:52:30 2021, max compression
+gzip compressed data, was "./PyQt-builder-1.9.1.tar", last modified: Thu Mar  4 17:12:20 2021, max compression
```

## Comparing `PyQt-builder-1.9.0.tar` & `PyQt-builder-1.9.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/
--rw-r--r--   0 phil       (501) staff       (20)     2061 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/PKG-INFO
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)     2061 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     3726 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)      119 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/entry_points.txt
--rw-r--r--   0 phil       (501) staff       (20)       22 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       10 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/PyQt_builder.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)     2766 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)    32047 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)       57 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       65 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)     1327 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/README
--rw-r--r--   0 phil       (501) staff       (20)     2374 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/setup.py
--rw-r--r--   0 phil       (501) staff       (20)     2034 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/NEWS
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/
--rw-r--r--   0 phil       (501) staff       (20)      194 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/index.rst
--rw-r--r--   0 phil       (501) staff       (20)     4763 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/pyproject_toml.rst
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/riverbank/
--rw-r--r--   0 phil       (501) staff       (20)      128 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/riverbank/layout.html
--rw-r--r--   0 phil       (501) staff       (20)      372 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/riverbank/theme.conf
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/riverbank/static/
--rw-r--r--   0 phil       (501) staff       (20)      465 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/riverbank/static/logo_tn.png
--rw-r--r--   0 phil       (501) staff       (20)     3979 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/riverbank/static/logo.png
--rw-r--r--   0 phil       (501) staff       (20)      738 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/riverbank/static/riverbank.css
--rw-r--r--   0 phil       (501) staff       (20)     3702 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/conf.py
--rw-r--r--   0 phil       (501) staff       (20)      786 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/html/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/html/_downloads/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/
--rw-r--r--   0 phil       (501) staff       (20)      786 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)     6909 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/index.html
--rw-r--r--   0 phil       (501) staff       (20)     7865 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/searchindex.js
--rw-r--r--   0 phil       (501) staff       (20)    21063 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/pyqtbuild_api.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/html/_sources/
--rw-r--r--   0 phil       (501) staff       (20)     2185 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/command_line_tools.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     4763 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/pyproject_toml.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     5053 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/pyqtbundle.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     5266 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/pyqtbuild_api.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)      194 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/index.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     1913 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/introduction.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     3016 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_sources/example.rst.txt
--rw-r--r--   0 phil       (501) staff       (20)     3768 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/py-modindex.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/doc/html/_static/
--rw-r--r--   0 phil       (501) staff       (20)       90 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/plus.png
--rw-r--r--   0 phil       (501) staff       (20)    12140 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/underscore.js
--rw-r--r--   0 phil       (501) staff       (20)      465 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_static/logo_tn.png
--rw-r--r--   0 phil       (501) staff       (20)     4232 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/classic.css
--rw-r--r--   0 phil       (501) staff       (20)      355 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/documentation_options.js
--rw-r--r--   0 phil       (501) staff       (20)    16323 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/searchtools.js
--rw-r--r--   0 phil       (501) staff       (20)      286 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/file.png
--rw-r--r--   0 phil       (501) staff       (20)     4803 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/sidebar.js
--rw-r--r--   0 phil       (501) staff       (20)   287630 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/jquery-3.5.1.js
--rw-r--r--   0 phil       (501) staff       (20)    35168 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/underscore-1.3.1.js
--rw-r--r--   0 phil       (501) staff       (20)    10847 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/language_data.js
--rw-r--r--   0 phil       (501) staff       (20)       90 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/minus.png
--rw-r--r--   0 phil       (501) staff       (20)     3979 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_static/logo.png
--rw-r--r--   0 phil       (501) staff       (20)    13647 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/basic.css
--rw-r--r--   0 phil       (501) staff       (20)     4837 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/_static/pygments.css
--rw-r--r--   0 phil       (501) staff       (20)      738 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/html/_static/riverbank.css
--rw-r--r--   0 phil       (501) staff       (20)     9416 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/doctools.js
--rw-r--r--   0 phil       (501) staff       (20)    89476 2020-12-28 14:44:14.000000 PyQt-builder-1.9.0/doc/html/_static/jquery.js
--rw-r--r--   0 phil       (501) staff       (20)    13051 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/example.html
--rw-r--r--   0 phil       (501) staff       (20)    13960 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/pyqtbundle.html
--rw-r--r--   0 phil       (501) staff       (20)    11792 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/genindex.html
--rw-r--r--   0 phil       (501) staff       (20)     9437 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/command_line_tools.html
--rw-r--r--   0 phil       (501) staff       (20)     3530 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/search.html
--rw-r--r--   0 phil       (501) staff       (20)     7821 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/introduction.html
--rw-r--r--   0 phil       (501) staff       (20)      783 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/objects.inv
--rw-r--r--   0 phil       (501) staff       (20)    13007 2021-02-22 17:52:28.000000 PyQt-builder-1.9.0/doc/html/pyproject_toml.html
--rw-r--r--   0 phil       (501) staff       (20)     2185 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/command_line_tools.rst
--rw-r--r--   0 phil       (501) staff       (20)     5266 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/pyqtbuild_api.rst
--rw-r--r--   0 phil       (501) staff       (20)     5053 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/pyqtbundle.rst
--rw-r--r--   0 phil       (501) staff       (20)     1913 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/introduction.rst
--rw-r--r--   0 phil       (501) staff       (20)     3016 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/doc/example.rst
--rw-r--r--   0 phil       (501) staff       (20)      304 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)    35297 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/LICENSE-GPL3
--rw-r--r--   0 phil       (501) staff       (20)    18161 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/LICENSE-GPL2
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/pyqtbuild/
--rw-r--r--   0 phil       (501) staff       (20)     1683 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/installable.py
--rw-r--r--   0 phil       (501) staff       (20)       61 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/version.py
--rw-r--r--   0 phil       (501) staff       (20)     1466 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/
--rw-r--r--   0 phil       (501) staff       (20)     1612 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/verbose.py
--rw-r--r--   0 phil       (501) staff       (20)     5628 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/bundle.py
--rw-r--r--   0 phil       (501) staff       (20)     5231 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel.py
--rw-r--r--   0 phil       (501) staff       (20)    13560 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_metadata.py
--rw-r--r--   0 phil       (501) staff       (20)     3489 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/bundle_main.py
--rw-r--r--   0 phil       (501) staff       (20)     1233 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3314 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_main.py
--rw-r--r--   0 phil       (501) staff       (20)     8994 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/abstract_package.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/
--rwxr-xr-x   0 phil       (501) staff       (20)     2227 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6_3d.py
--rwxr-xr-x   0 phil       (501) staff       (20)     1729 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtnetworkauth.py
--rwxr-xr-x   0 phil       (501) staff       (20)     1741 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtchart.py
--rwxr-xr-x   0 phil       (501) staff       (20)     2582 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtwebengine.py
--rw-r--r--   0 phil       (501) staff       (20)     4774 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6.py
--rw-r--r--   0 phil       (501) staff       (20)     1631 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/__init__.py
--rwxr-xr-x   0 phil       (501) staff       (20)     1701 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6_networkauth.py
--rwxr-xr-x   0 phil       (501) staff       (20)     1756 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtdatavisualization.py
--rwxr-xr-x   0 phil       (501) staff       (20)     1723 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtpurchasing.py
--rw-r--r--   0 phil       (501) staff       (20)     5833 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt5.py
--rw-r--r--   0 phil       (501) staff       (20)     2659 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt.py
--rwxr-xr-x   0 phil       (501) staff       (20)     2593 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt3d.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/
--rw-r--r--   0 phil       (501) staff       (20)   101872 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/vcruntime140.dll
--rw-r--r--   0 phil       (501) staff       (20)   317208 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/concrt140.dll
--rw-r--r--   0 phil       (501) staff       (20)    31728 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140_1.dll
--rw-r--r--   0 phil       (501) staff       (20)   193520 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140_2.dll
--rw-r--r--   0 phil       (501) staff       (20)    44528 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/vcruntime140_1.dll
--rw-r--r--   0 phil       (501) staff       (20)   590112 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140.dll
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/
--rw-r--r--   0 phil       (501) staff       (20)  1297408 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libeay32.dll
--rw-r--r--   0 phil       (501) staff       (20)   530432 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libssl-1_1.dll
--rw-r--r--   0 phil       (501) staff       (20)  2499072 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libcrypto-1_1.dll
--rw-r--r--   0 phil       (501) staff       (20)   281600 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/ssleay32.dll
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:29.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/
--rw-r--r--   0 phil       (501) staff       (20)    83952 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/vcruntime140.dll
--rw-r--r--   0 phil       (501) staff       (20)   250352 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/concrt140.dll
--rw-r--r--   0 phil       (501) staff       (20)    29168 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140_1.dll
--rw-r--r--   0 phil       (501) staff       (20)   174064 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140_2.dll
--rw-r--r--   0 phil       (501) staff       (20)   454128 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140.dll
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/
--rw-r--r--   0 phil       (501) staff       (20)  1988608 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libeay32.dll
--rw-r--r--   0 phil       (501) staff       (20)  3205632 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libcrypto-1_1-x64.dll
--rw-r--r--   0 phil       (501) staff       (20)   681472 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libssl-1_1-x64.dll
--rw-r--r--   0 phil       (501) staff       (20)   361984 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/ssleay32.dll
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-02-22 17:52:30.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/
--rw-r--r--   0 phil       (501) staff       (20)    44738 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)       67 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/WHEEL
--rw-r--r--   0 phil       (501) staff       (20)      578 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/METADATA
--rw-r--r--   0 phil       (501) staff       (20)     3251 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/bundle/wheel.py
--rw-r--r--   0 phil       (501) staff       (20)    25391 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/builder.py
--rw-r--r--   0 phil       (501) staff       (20)     8737 2021-02-22 17:52:26.000000 PyQt-builder-1.9.0/pyqtbuild/bindings.py
--rw-r--r--   0 phil       (501) staff       (20)     6934 2021-02-22 17:52:27.000000 PyQt-builder-1.9.0/pyqtbuild/project.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/
+-rw-r--r--   0 phil       (501) staff       (20)     2061 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PKG-INFO
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)     2061 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     3726 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)      119 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/entry_points.txt
+-rw-r--r--   0 phil       (501) staff       (20)       22 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       10 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/PyQt_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)     2766 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)    32646 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)       57 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       65 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)     1327 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/README
+-rw-r--r--   0 phil       (501) staff       (20)     2374 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/setup.py
+-rw-r--r--   0 phil       (501) staff       (20)     2171 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/NEWS
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/
+-rw-r--r--   0 phil       (501) staff       (20)      194 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/index.rst
+-rw-r--r--   0 phil       (501) staff       (20)     4763 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/pyproject_toml.rst
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/riverbank/
+-rw-r--r--   0 phil       (501) staff       (20)      128 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/riverbank/layout.html
+-rw-r--r--   0 phil       (501) staff       (20)      372 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/riverbank/theme.conf
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/riverbank/static/
+-rw-r--r--   0 phil       (501) staff       (20)      465 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/riverbank/static/logo_tn.png
+-rw-r--r--   0 phil       (501) staff       (20)     3979 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/riverbank/static/logo.png
+-rw-r--r--   0 phil       (501) staff       (20)      738 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/riverbank/static/riverbank.css
+-rw-r--r--   0 phil       (501) staff       (20)     3702 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/conf.py
+-rw-r--r--   0 phil       (501) staff       (20)      786 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/html/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/html/_downloads/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/
+-rw-r--r--   0 phil       (501) staff       (20)      786 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)     6909 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/index.html
+-rw-r--r--   0 phil       (501) staff       (20)     7865 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/searchindex.js
+-rw-r--r--   0 phil       (501) staff       (20)    21063 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/pyqtbuild_api.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/html/_sources/
+-rw-r--r--   0 phil       (501) staff       (20)     2185 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/command_line_tools.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     4763 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/pyproject_toml.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     5053 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/pyqtbundle.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     5266 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/pyqtbuild_api.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)      194 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/index.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     1913 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/introduction.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_sources/example.rst.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3768 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/py-modindex.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/doc/html/_static/
+-rw-r--r--   0 phil       (501) staff       (20)       90 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/plus.png
+-rw-r--r--   0 phil       (501) staff       (20)    12140 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/underscore.js
+-rw-r--r--   0 phil       (501) staff       (20)      465 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_static/logo_tn.png
+-rw-r--r--   0 phil       (501) staff       (20)     4232 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/classic.css
+-rw-r--r--   0 phil       (501) staff       (20)      355 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/documentation_options.js
+-rw-r--r--   0 phil       (501) staff       (20)    16323 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/searchtools.js
+-rw-r--r--   0 phil       (501) staff       (20)      286 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/file.png
+-rw-r--r--   0 phil       (501) staff       (20)     4803 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/sidebar.js
+-rw-r--r--   0 phil       (501) staff       (20)   287630 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 phil       (501) staff       (20)    35168 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 phil       (501) staff       (20)    10847 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/language_data.js
+-rw-r--r--   0 phil       (501) staff       (20)       90 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/minus.png
+-rw-r--r--   0 phil       (501) staff       (20)     3979 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_static/logo.png
+-rw-r--r--   0 phil       (501) staff       (20)    13647 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/basic.css
+-rw-r--r--   0 phil       (501) staff       (20)     4837 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/_static/pygments.css
+-rw-r--r--   0 phil       (501) staff       (20)      738 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/html/_static/riverbank.css
+-rw-r--r--   0 phil       (501) staff       (20)     9416 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/doctools.js
+-rw-r--r--   0 phil       (501) staff       (20)    89476 2020-12-28 14:44:14.000000 PyQt-builder-1.9.1/doc/html/_static/jquery.js
+-rw-r--r--   0 phil       (501) staff       (20)    13051 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/example.html
+-rw-r--r--   0 phil       (501) staff       (20)    13960 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/pyqtbundle.html
+-rw-r--r--   0 phil       (501) staff       (20)    11792 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/genindex.html
+-rw-r--r--   0 phil       (501) staff       (20)     9437 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/command_line_tools.html
+-rw-r--r--   0 phil       (501) staff       (20)     3530 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/search.html
+-rw-r--r--   0 phil       (501) staff       (20)     7821 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/introduction.html
+-rw-r--r--   0 phil       (501) staff       (20)      783 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/objects.inv
+-rw-r--r--   0 phil       (501) staff       (20)    13007 2021-03-04 17:12:19.000000 PyQt-builder-1.9.1/doc/html/pyproject_toml.html
+-rw-r--r--   0 phil       (501) staff       (20)     2185 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/command_line_tools.rst
+-rw-r--r--   0 phil       (501) staff       (20)     5266 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/pyqtbuild_api.rst
+-rw-r--r--   0 phil       (501) staff       (20)     5053 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/pyqtbundle.rst
+-rw-r--r--   0 phil       (501) staff       (20)     1913 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/introduction.rst
+-rw-r--r--   0 phil       (501) staff       (20)     3016 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/doc/example.rst
+-rw-r--r--   0 phil       (501) staff       (20)      304 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)    35297 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/LICENSE-GPL3
+-rw-r--r--   0 phil       (501) staff       (20)    18161 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/LICENSE-GPL2
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/
+-rw-r--r--   0 phil       (501) staff       (20)     1683 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/installable.py
+-rw-r--r--   0 phil       (501) staff       (20)       61 2021-03-04 17:12:18.000000 PyQt-builder-1.9.1/pyqtbuild/version.py
+-rw-r--r--   0 phil       (501) staff       (20)     1466 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/
+-rw-r--r--   0 phil       (501) staff       (20)     1612 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/verbose.py
+-rw-r--r--   0 phil       (501) staff       (20)     5628 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/bundle.py
+-rw-r--r--   0 phil       (501) staff       (20)     5368 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel.py
+-rw-r--r--   0 phil       (501) staff       (20)    13560 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_metadata.py
+-rw-r--r--   0 phil       (501) staff       (20)     3489 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/bundle_main.py
+-rw-r--r--   0 phil       (501) staff       (20)     1233 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3314 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_main.py
+-rw-r--r--   0 phil       (501) staff       (20)     9470 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/abstract_package.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/
+-rwxr-xr-x   0 phil       (501) staff       (20)     2227 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6_3d.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     1729 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtnetworkauth.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     1741 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtchart.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     2582 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtwebengine.py
+-rw-r--r--   0 phil       (501) staff       (20)     4774 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6.py
+-rw-r--r--   0 phil       (501) staff       (20)     1631 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/__init__.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     1701 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6_networkauth.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     1756 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtdatavisualization.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     1723 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtpurchasing.py
+-rw-r--r--   0 phil       (501) staff       (20)     5833 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt5.py
+-rw-r--r--   0 phil       (501) staff       (20)     2659 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt.py
+-rwxr-xr-x   0 phil       (501) staff       (20)     2593 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt3d.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/
+-rw-r--r--   0 phil       (501) staff       (20)   101872 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/vcruntime140.dll
+-rw-r--r--   0 phil       (501) staff       (20)   317208 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/concrt140.dll
+-rw-r--r--   0 phil       (501) staff       (20)    31728 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140_1.dll
+-rw-r--r--   0 phil       (501) staff       (20)   193520 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140_2.dll
+-rw-r--r--   0 phil       (501) staff       (20)    44528 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/vcruntime140_1.dll
+-rw-r--r--   0 phil       (501) staff       (20)   590112 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140.dll
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/
+-rw-r--r--   0 phil       (501) staff       (20)  1297408 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libeay32.dll
+-rw-r--r--   0 phil       (501) staff       (20)   530432 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libssl-1_1.dll
+-rw-r--r--   0 phil       (501) staff       (20)  2499072 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libcrypto-1_1.dll
+-rw-r--r--   0 phil       (501) staff       (20)   281600 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/ssleay32.dll
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/
+-rw-r--r--   0 phil       (501) staff       (20)    83952 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/vcruntime140.dll
+-rw-r--r--   0 phil       (501) staff       (20)   250352 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/concrt140.dll
+-rw-r--r--   0 phil       (501) staff       (20)    29168 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140_1.dll
+-rw-r--r--   0 phil       (501) staff       (20)   174064 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140_2.dll
+-rw-r--r--   0 phil       (501) staff       (20)   454128 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140.dll
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/
+-rw-r--r--   0 phil       (501) staff       (20)  1988608 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libeay32.dll
+-rw-r--r--   0 phil       (501) staff       (20)  3205632 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libcrypto-1_1-x64.dll
+-rw-r--r--   0 phil       (501) staff       (20)   681472 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libssl-1_1-x64.dll
+-rw-r--r--   0 phil       (501) staff       (20)   361984 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/ssleay32.dll
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2021-03-04 17:12:20.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/
+-rw-r--r--   0 phil       (501) staff       (20)    44738 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)       67 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/WHEEL
+-rw-r--r--   0 phil       (501) staff       (20)      596 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/METADATA
+-rw-r--r--   0 phil       (501) staff       (20)     3251 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bundle/wheel.py
+-rw-r--r--   0 phil       (501) staff       (20)    25391 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/builder.py
+-rw-r--r--   0 phil       (501) staff       (20)     8737 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/bindings.py
+-rw-r--r--   0 phil       (501) staff       (20)     6934 2021-03-04 17:12:17.000000 PyQt-builder-1.9.1/pyqtbuild/project.py
```

### Comparing `PyQt-builder-1.9.0/PKG-INFO` & `PyQt-builder-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyQt-builder
-Version: 1.9.0
+Version: 1.9.1
 Summary: The PEP 517 compliant PyQt build system
 Home-page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-email: info@riverbankcomputing.com
 License: SIP
 Description: PyQt-builder - The PEP 517 Compliant PyQt Build System
         ======================================================
```

### Comparing `PyQt-builder-1.9.0/PyQt_builder.egg-info/PKG-INFO` & `PyQt-builder-1.9.1/PyQt_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PyQt-builder
-Version: 1.9.0
+Version: 1.9.1
 Summary: The PEP 517 compliant PyQt build system
 Home-page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-email: info@riverbankcomputing.com
 License: SIP
 Description: PyQt-builder - The PEP 517 Compliant PyQt Build System
         ======================================================
```

### Comparing `PyQt-builder-1.9.0/PyQt_builder.egg-info/SOURCES.txt` & `PyQt-builder-1.9.1/PyQt_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/LICENSE` & `PyQt-builder-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/ChangeLog` & `PyQt-builder-1.9.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,33 @@
+2021-03-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Released as v1.9.1.
+	[99dbf7f8c33c] [1.9.1] <1.9-maint>
+
+	* pyqtbuild/bundle/qt_wheel.py,
+	pyqtbuild/bundle/qt_wheel_distinfo/METADATA:
+	Fixed the name in the meta-data of a Qt wheel.
+	[5ce175b51818] <1.9-maint>
+
+	* pyqtbuild/bundle/qt_wheel.py:
+	Fixed the name of a Qt wheel.
+	[b4be05cac0d6] <1.9-maint>
+
+	* NEWS, pyqtbuild/bundle/abstract_package.py:
+	Handle the changed Qt installation directory used in newer PyQt
+	releases.
+	[ef7fa24f4c28] <1.9-maint>
+
 2021-02-22  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 1.9.0 for changeset de8775a53a87
+	[82511d30da8f]
+
 	* NEWS:
 	Released as v1.9.0.
 	[de8775a53a87] [1.9.0]
 
 	* NEWS:
 	Updated the NEWS file.
 	[a3908330c638]
```

### Comparing `PyQt-builder-1.9.0/README` & `PyQt-builder-1.9.1/README`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/setup.py` & `PyQt-builder-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/NEWS` & `PyQt-builder-1.9.1/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v1.9.1 2nd March 2021
+  - Handle the changed Qt installation directory used by PyQt5 v5.15.4 and
+    later, and PyQt6 v6.0.3 and later.
+
 v1.9.0 23rd February 2021
   - Added support for PyQtNetworkAuth.
   - Added support for creating Qt5 wheels.
   - The default minimum glibc version for Qt6 is now v2.28.
   - The default minimum macOS version for Qt6 is now v10.14.
 
 v1.8.0 5th February 2021
```

### Comparing `PyQt-builder-1.9.0/doc/pyproject_toml.rst` & `PyQt-builder-1.9.1/doc/pyproject_toml.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/riverbank/static/logo.png` & `PyQt-builder-1.9.1/doc/riverbank/static/logo.png`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/riverbank/static/riverbank.css` & `PyQt-builder-1.9.1/doc/riverbank/static/riverbank.css`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/conf.py` & `PyQt-builder-1.9.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/pyproject.toml` & `PyQt-builder-1.9.1/doc/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/pyproject.toml` & `PyQt-builder-1.9.1/doc/html/_downloads/522adf759addbd3b193c74ca85243f7d/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/index.html` & `PyQt-builder-1.9.1/doc/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>PyQt-builder Reference Guide &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>PyQt-builder Reference Guide &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -27,15 +27,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="introduction.html" title="Introduction"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyQt-builder Reference Guide</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -109,15 +109,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="introduction.html" title="Introduction"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">PyQt-builder Reference Guide</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * PyQt-builder Reference Guide
 ****** PyQt-builder Reference GuideÂ¶ ******
     * Introduction
           o Installation
     * Command_Line_Tools
     * pyproject.toml_Reference
           o [tool.sip.builder]_Section
@@ -34,10 +34,10 @@
 Introduction
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * PyQt-builder Reference Guide
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/searchindex.js` & `PyQt-builder-1.9.1/doc/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/pyqtbuild_api.html` & `PyQt-builder-1.9.1/doc/html/pyqtbuild_api.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyqtbuild Module Reference &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>pyqtbuild Module Reference &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="An Example"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="pyproject_toml.html" title="pyproject.toml Reference"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href=""><code class="xref py py-mod docutils literal notranslate"><span class="pre">pyqtbuild</span></code> Module Reference</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -271,15 +271,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="An Example"
              >next</a> |</li>
         <li class="right" >
           <a href="pyproject_toml.html" title="pyproject.toml Reference"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href=""><code class="xref py py-mod docutils literal notranslate"><span class="pre">pyqtbuild</span></code> Module Reference</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * pyqtbuild Module Reference
 ****** pyqtbuild Module ReferenceÂ¶ ******
 The pyqtbuild module provides a number of API elements that can be used by a
 projectâs project.py file.
 ***** PYQTBUILD_VERSIONÂ¶ *****
   pyqtbuild.PYQTBUILD_VERSIONÂ¶
       This is a Python integer object that represents the version number of the
@@ -118,10 +118,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * pyqtbuild Module Reference
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/command_line_tools.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/command_line_tools.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/pyproject_toml.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/pyproject_toml.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/pyqtbundle.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/pyqtbundle.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/pyqtbuild_api.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/pyqtbuild_api.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/introduction.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_sources/example.rst.txt` & `PyQt-builder-1.9.1/doc/html/_sources/example.rst.txt`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/py-modindex.html` & `PyQt-builder-1.9.1/doc/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Python Module Index &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -30,15 +30,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -91,15 +91,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -3,23 +3,23 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Python Module Index
 ****** Python Module Index ******
 p
   
  p
  pyqtbuild The PyQt build system.
 [Logo]
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Python Module Index
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/_static/underscore.js` & `PyQt-builder-1.9.1/doc/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/classic.css` & `PyQt-builder-1.9.1/doc/html/_static/classic.css`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/searchtools.js` & `PyQt-builder-1.9.1/doc/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/sidebar.js` & `PyQt-builder-1.9.1/doc/html/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/jquery-3.5.1.js` & `PyQt-builder-1.9.1/doc/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/underscore-1.3.1.js` & `PyQt-builder-1.9.1/doc/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/language_data.js` & `PyQt-builder-1.9.1/doc/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/logo.png` & `PyQt-builder-1.9.1/doc/html/_static/logo.png`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/basic.css` & `PyQt-builder-1.9.1/doc/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/pygments.css` & `PyQt-builder-1.9.1/doc/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/riverbank.css` & `PyQt-builder-1.9.1/doc/html/_static/riverbank.css`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/doctools.js` & `PyQt-builder-1.9.1/doc/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/_static/jquery.js` & `PyQt-builder-1.9.1/doc/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/html/example.html` & `PyQt-builder-1.9.1/doc/html/example.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>An Example &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>An Example &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyqtbundle.html" title="Bundling Qt Using pyqt-bundle"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="pyqtbuild_api.html" title="pyqtbuild Module Reference"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">An Example</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -166,15 +166,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyqtbundle.html" title="Bundling Qt Using pyqt-bundle"
              >next</a> |</li>
         <li class="right" >
           <a href="pyqtbuild_api.html" title="pyqtbuild Module Reference"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">An Example</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * An Example
 ****** An ExampleÂ¶ ******
 In this section we walk through the pyproject.toml file for the PyQtChart
 project. PyQtChart is the set of bindings for the QtCharts v5 library and is
 built on top of PyQt5. It comprises a single extension module. The simplicitly
 of PyQtChart means that there is no need to provide any additional code in a
 project.py file.
@@ -90,10 +90,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * An Example
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/pyqtbundle.html` & `PyQt-builder-1.9.1/doc/html/pyqtbundle.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Bundling Qt Using pyqt-bundle &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Bundling Qt Using pyqt-bundle &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -27,15 +27,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="An Example"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Bundling Qt Using <strong class="program">pyqt-bundle</strong></a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -220,15 +220,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="example.html" title="An Example"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Bundling Qt Using <strong class="program">pyqt-bundle</strong></a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Bundling Qt Using pyqt-bundle
 ****** Bundling Qt Using pyqt-bundleÂ¶ ******
 PyQt wheels can contain a bundled copy of the relavent parts of Qt. The main
 reason for doing this is so that users can install a complete PyQt environment
 with a single pip install.
 A bundled copy may also be replaced by a newer release of Qt. Given the ABI
 guarantees made by Qt (i.e. that a later version or Qt should be able to
@@ -103,10 +103,10 @@
 An_Example
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Bundling Qt Using pyqt-bundle
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/genindex.html` & `PyQt-builder-1.9.1/doc/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Index &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -359,15 +359,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Index
 ****** Index ******
 Symbols | C | E | H | M | P | Q
 ***** Symbols *****
     * --android-abi ABI                  * --openssl-dir DIR
           o command_line_option                o pyqt-bundle_command_line
     * --build-tag-suffix SUFFIX                  option
@@ -79,10 +79,10 @@
                                               attribute)
 [Logo]
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Index
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/command_line_tools.html` & `PyQt-builder-1.9.1/doc/html/command_line_tools.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Command Line Tools &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Command Line Tools &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyproject_toml.html" title="pyproject.toml Reference"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="introduction.html" title="Introduction"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Command Line Tools</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -166,15 +166,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyproject_toml.html" title="pyproject.toml Reference"
              >next</a> |</li>
         <li class="right" >
           <a href="introduction.html" title="Introduction"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Command Line Tools</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Command Line Tools
 ****** Command Line ToolsÂ¶ ******
 PyQt-builder adds the following command line options to SIPâs_build_tools.
 Unless stated otherwise, each option is added to all of the build tools.
 Note
 Individual projects may also add their own project-specific command line
 options.
@@ -57,10 +57,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Command Line Tools
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/search.html` & `PyQt-builder-1.9.1/doc/html/search.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Search &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
@@ -29,15 +29,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -83,15 +83,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -3,20 +3,20 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 [Logo]
 **** Navigation ****
     * index
     * modules |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Search
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/introduction.html` & `PyQt-builder-1.9.1/doc/html/introduction.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Introduction &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>Introduction &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="command_line_tools.html" title="Command Line Tools"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="PyQt-builder Reference Guide"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Introduction</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -129,15 +129,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="command_line_tools.html" title="Command Line Tools"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="PyQt-builder Reference Guide"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Introduction</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Introduction
 ****** IntroductionÂ¶ ******
 PyQt-builder is a tool for generating Python bindings for C++ libraries that
 use the Qt application framework. The bindings are built on top of the PyQt
 bindings for Qt. PyQt-builder is used to build PyQt itself.
 PyQt-builder also includes the pyqt-bundle command line tool used to bundle a
 copy of Qt with a PyQt wheel. This is separate from the build system and
@@ -49,10 +49,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * Introduction
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/html/objects.inv` & `PyQt-builder-1.9.1/doc/html/objects.inv`

 * *Files 16% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: PyQt-builder
-# Version: 1.9.0
+# Version: 1.9.1
 # The remainder of this file is compressed using zlib.
 
 pyqtbuild py:module 0 pyqtbuild_api.html#module-$ -
 pyqtbuild.PYQTBUILD_VERSION py:data 1 pyqtbuild_api.html#$ -
 pyqtbuild.PYQTBUILD_VERSION_STR py:data 1 pyqtbuild_api.html#$ -
 pyqtbuild.PyQtBindings py:class 1 pyqtbuild_api.html#$ -
 pyqtbuild.PyQtBindings.handle_test_output py:method 1 pyqtbuild_api.html#$ -
```

### Comparing `PyQt-builder-1.9.0/doc/html/pyproject_toml.html` & `PyQt-builder-1.9.1/doc/html/pyproject_toml.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>pyproject.toml Reference &#8212; PyQt-builder v1.9.0 Reference Guide</title>
+    <title>pyproject.toml Reference &#8212; PyQt-builder v1.9.1 Reference Guide</title>
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <link rel="stylesheet" href="_static/riverbank.css" type="text/css" />
     
     <script id="documentation_options" data-url_root="./" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
@@ -31,15 +31,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyqtbuild_api.html" title="pyqtbuild Module Reference"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="command_line_tools.html" title="Command Line Tools"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href=""><code class="file docutils literal notranslate"><span class="pre">pyproject.toml</span></code> Reference</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -199,15 +199,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="pyqtbuild_api.html" title="pyqtbuild Module Reference"
              >next</a> |</li>
         <li class="right" >
           <a href="command_line_tools.html" title="Command Line Tools"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.0 Reference Guide</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">PyQt-builder v1.9.1 Reference Guide</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href=""><code class="file docutils literal notranslate"><span class="pre">pyproject.toml</span></code> Reference</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2021 Riverbank Computing Limited.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 3.4.1.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * pyproject.toml Reference
 ****** pyproject.toml ReferenceÂ¶ ******
 PyQt-builder adds the following keys to those implemented_by_SIP.
 Note
 Individual projects may also add their own project-specific keys.
 ***** [tool.sip.builder] SectionÂ¶ *****
 Unless stated otherwise, all values are strings. Unless stated otherwise, the
@@ -110,10 +110,10 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * PyQt-builder_v1.9.0_Reference_Guide »
+    * PyQt-builder_v1.9.1_Reference_Guide »
     * pyproject.toml Reference
 © Copyright 2021 Riverbank Computing Limited. Created using Sphinx 3.4.1.
```

### Comparing `PyQt-builder-1.9.0/doc/command_line_tools.rst` & `PyQt-builder-1.9.1/doc/command_line_tools.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/pyqtbuild_api.rst` & `PyQt-builder-1.9.1/doc/pyqtbuild_api.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/pyqtbundle.rst` & `PyQt-builder-1.9.1/doc/pyqtbundle.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/introduction.rst` & `PyQt-builder-1.9.1/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/doc/example.rst` & `PyQt-builder-1.9.1/doc/example.rst`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/LICENSE-GPL3` & `PyQt-builder-1.9.1/LICENSE-GPL3`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/LICENSE-GPL2` & `PyQt-builder-1.9.1/LICENSE-GPL2`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/installable.py` & `PyQt-builder-1.9.1/pyqtbuild/installable.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/__init__.py` & `PyQt-builder-1.9.1/pyqtbuild/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/verbose.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/verbose.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/bundle.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         raise UserException(
                 "Qt architecture '{0}' is unsupported".format(qt_arch))
 
     tag_parts = ['py3', 'none', arch]
     tag = '-'.join(tag_parts)
 
     # Construct the name of the wheel.
-    name_parts = [package_name + '_Qt']
+    name_parts = [package_name + '_Qt' + package.qt_version_str[0]]
     name_parts.append(package.qt_version_str)
 
     distinfo_dir = '-'.join(name_parts) + '.dist-info'
 
     if build_tag:
         name_parts.append(build_tag)
 
@@ -115,14 +115,16 @@
         dst = os.path.join(distinfo_dir, proto)
 
         if proto == 'METADATA':
             with open(src) as s:
                 metadata = s.read()
 
             metadata = metadata.replace('@RB_PACKAGE@', package_title)
+            metadata = metadata.replace('@RB_MAJOR_VERSION@',
+                    package.qt_version_str[0])
             metadata = metadata.replace('@RB_VERSION@', package.qt_version_str)
             metadata = metadata.replace('@RB_LICENSE@',
                     "LGPL v3" if lgpl else "GPL v3")
 
             with open(dst, 'w') as d:
                 d.write(metadata)
         elif proto == 'WHEEL':
```

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/qt_metadata.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/qt_metadata.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/bundle_main.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/bundle_main.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/__init__.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_main.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_main.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/abstract_package.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/abstract_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,26 +43,28 @@
 
         # Get the Qt version.
         self.qt_version = self._parse_version(
                 os.path.basename(os.path.dirname(self._qt_dir)))
 
         # Parse any package version string.
         if version_str:
-            version = self._parse_version(version_str)
+            self._version = self._parse_version(version_str)
 
             # If we set the maintenance number to 0 then this will be the
             # version of Qt the wheel was built against.  (This is not a valid
             # assumption on Windows because of the QAxContainer problem but
             # this is handled elsewhere.)
-            min_qt_version = (version[0], version[1], 0)
+            min_qt_version = (self._version[0], self._version[1], 0)
 
             # Check the versions are compatible.
             if self.qt_version < min_qt_version:
                 raise UserException(
                         "The version of Qt being bundled is too old")
+        else:
+            self._version = None
 
     def bundle_msvc_runtime(self, target_qt_dir, arch):
         """ Bundle the MSVC runtime. """
 
         # This default implementation does nothing.
 
     def bundle_openssl(self, target_qt_dir, openssl_dir, arch):
@@ -150,15 +152,26 @@
         """
 
     def get_target_qt_dir(self):
         """ Return the directory, relative to the wheel root, containing the
         bundled Qt directory.
         """
 
-        return os.path.join('PyQt{}'.format(self.qt_version[0]), 'Qt')
+        # Assume the current naming of the bundled Qt directory.
+        qt_major_version = self.qt_version[0]
+
+        # See if it is an older version.
+        if self._version is not None:
+            if (6, 0, 0) <= self._version <= (6, 0, 2):
+                qt_major_version = ''
+            elif self._version <= (5, 15, 3):
+                qt_major_version = ''
+
+        return os.path.join('PyQt{}'.format(qt_major_version),
+                'Qt{}'.format(qt_major_version))
 
     @property
     def qt_version_str(self):
         """ The version number of the Qt installation as a string. """
 
         return '.'.join([str(v) for v in self.qt_version])
```

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6_3d.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6_3d.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtnetworkauth.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtnetworkauth.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtchart.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtchart.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtwebengine.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtwebengine.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/__init__.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt6_networkauth.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt6_networkauth.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtdatavisualization.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtdatavisualization.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqtpurchasing.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqtpurchasing.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt5.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt5.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/packages/pyqt3d.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/packages/pyqt3d.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/vcruntime140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/concrt140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/concrt140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140_1.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140_1.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140_2.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140_2.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/vcruntime140_1.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/vcruntime140_1.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-64/msvcp140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-64/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libeay32.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libeay32.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libssl-1_1.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libssl-1_1.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/libcrypto-1_1.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/libcrypto-1_1.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-32/ssleay32.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-32/ssleay32.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/vcruntime140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/vcruntime140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/concrt140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/concrt140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140_1.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140_1.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140_2.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140_2.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/msvc-32/msvcp140.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/msvc-32/msvcp140.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libeay32.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libeay32.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libcrypto-1_1-x64.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libcrypto-1_1-x64.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/libssl-1_1-x64.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/libssl-1_1-x64.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/dlls/openssl-64/ssleay32.dll` & `PyQt-builder-1.9.1/pyqtbuild/bundle/dlls/openssl-64/ssleay32.dll`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/LICENSE` & `PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/qt_wheel_distinfo/METADATA` & `PyQt-builder-1.9.1/pyqtbuild/bundle/qt_wheel_distinfo/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1
-Name: @RB_PACKAGE@-Qt
+Name: @RB_PACKAGE@-Qt@RB_MAJOR_VERSION@
 Version: @RB_VERSION@
 Summary: The subset of a Qt installation needed by @RB_PACKAGE@.
 Home-page: https://www.riverbankcomputing.com/software/pyqt/
 Author: Riverbank Computing Limited
 Author-email: info@riverbankcomputing.com
 License: @RB_LICENSE@
 Platform: Linux
```

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bundle/wheel.py` & `PyQt-builder-1.9.1/pyqtbuild/bundle/wheel.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/builder.py` & `PyQt-builder-1.9.1/pyqtbuild/builder.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/bindings.py` & `PyQt-builder-1.9.1/pyqtbuild/bindings.py`

 * *Files identical despite different names*

### Comparing `PyQt-builder-1.9.0/pyqtbuild/project.py` & `PyQt-builder-1.9.1/pyqtbuild/project.py`

 * *Files identical despite different names*

