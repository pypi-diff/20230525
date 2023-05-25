# Comparing `tmp/libonvif-2.0.10.tar.gz` & `tmp/libonvif-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libonvif-2.0.10.tar", last modified: Thu May 25 17:35:39 2023, max compression
+gzip compressed data, was "libonvif-2.0.9.tar", last modified: Wed Apr 26 00:47:34 2023, max compression
```

## Comparing `libonvif-2.0.10.tar` & `libonvif-2.0.9.tar`

### file list

```diff
@@ -1,316 +1,305 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.454977 libonvif-2.0.10/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2235 2023-05-25 17:26:34.000000 libonvif-2.0.10/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    27028 2023-05-25 17:26:34.000000 libonvif-2.0.10/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      124 2023-05-25 17:26:34.000000 libonvif-2.0.10/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2088 2023-05-25 17:35:39.454977 libonvif-2.0.10/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1557 2023-05-25 17:26:34.000000 libonvif-2.0.10/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.426977 libonvif-2.0.10/include/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2644 2023-05-25 17:26:34.000000 libonvif-2.0.10/include/cencode.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19149 2023-05-25 17:26:34.000000 libonvif-2.0.10/include/getopt-win.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9815 2023-05-25 17:26:34.000000 libonvif-2.0.10/include/onvif.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9785 2023-05-25 17:26:34.000000 libonvif-2.0.10/include/onvifboss.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2564 2023-05-25 17:26:34.000000 libonvif-2.0.10/include/sha1.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.426977 libonvif-2.0.10/libonvif/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      564 2023-05-25 17:26:34.000000 libonvif-2.0.10/libonvif/__init__.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.426977 libonvif-2.0.10/libonvif.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2088 2023-05-25 17:35:39.000000 libonvif-2.0.10/libonvif.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9766 2023-05-25 17:35:39.000000 libonvif-2.0.10/libonvif.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-25 17:35:39.000000 libonvif-2.0.10/libonvif.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-25 17:29:04.000000 libonvif-2.0.10/libonvif.egg-info/not-zip-safe
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        9 2023-05-25 17:35:39.000000 libonvif-2.0.10/libonvif.egg-info/top_level.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1271 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.appveyor.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      996 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.clang-format
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2605 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.clang-tidy
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2196 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.cmake-format.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1308 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.codespell-ignore-lines
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       45 2023-05-25 17:26:47.000000 libonvif-2.0.10/pybind11/.git
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       18 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.gitattributes
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/.github/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/CODEOWNERS
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15284 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/CONTRIBUTING.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2561 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      328 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/dependabot.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      116 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       50 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/labeler_merged.yml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/.github/matchers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      668 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/matchers/pylint.json
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/pull_request_template.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/.github/workflows/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    33993 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/ci.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2158 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/configure.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1491 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/format.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      641 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2589 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/pip.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2784 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.github/workflows/upstream.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      502 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.gitignore
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3600 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       62 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/.readthedocs.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12031 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1684 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7686 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/README.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/docs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      607 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/Doxyfile
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7417 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/Makefile
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.426977 libonvif-2.0.10/pybind11/docs/_static/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.430977 libonvif-2.0.10/pybind11/docs/_static/css/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/_static/css/custom.css
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/docs/advanced/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/docs/advanced/cast/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3937 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3429 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/custom.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3889 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/functional.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1556 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12371 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/overview.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9586 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/stl.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9119 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/cast/strings.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    47796 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/classes.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8453 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/embedding.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17796 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/exceptions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26729 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/functions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15651 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/misc.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/docs/advanced/pycpp/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      278 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17161 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6377 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9240 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/basics.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2856 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/benchmark.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   117582 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/changelog.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16880 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/classes.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/docs/cmake/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      273 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/cmake/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25777 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/compiling.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11574 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/conf.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13177 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/faq.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      613 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3277 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/installing.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3079 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/limitations.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    61034 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/pybind11-logo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    44653 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    87708 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    41121 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    85853 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2647 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/reference.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4414 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/release.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23489 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/docs/upgrade.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.426977 libonvif-2.0.10/pybind11/include/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/include/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24334 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7069 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    67312 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8458 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      120 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2096 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.434978 libonvif-2.0.10/pybind11/include/pybind11/detail/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28518 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    53462 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5962 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17859 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28221 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    48364 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1625 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.438978 libonvif-2.0.10/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    31450 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18140 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13459 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4731 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5002 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8262 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8862 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    79416 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9103 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2734 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/options.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   126708 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    94641 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.438978 libonvif-2.0.10/pybind11/include/pybind11/stl/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4185 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15399 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    29897 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1929 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/include/pybind11/type_caster_pyobject_ptr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2765 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/noxfile.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.438978 libonvif-2.0.10/pybind11/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1544 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/__main__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      233 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/_version.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1207 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/commands.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/py.typed
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17462 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pybind11/setup_helpers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2360 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1452 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4877 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21801 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5619 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/conftest.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11736 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/constructor_stats.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3578 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1776 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      396 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      926 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/env.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/extra_python_package/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8345 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/extra_python_package/test_files.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/extra_setuptools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4153 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2847 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/local_bindings.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/object.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4517 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/pybind11_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2685 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/pybind11_tests.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      600 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      855 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_async.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_async.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8567 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_buffers.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4848 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_buffers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16025 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_builtin_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17243 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_builtin_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4118 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_call_policies.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6549 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_call_policies.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10858 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_callbacks.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6796 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_callbacks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3370 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_chrono.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5691 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_chrono.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24874 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_class.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14757 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_class.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2639 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1171 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1293 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      152 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1353 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1163 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1368 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      198 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_cmake_build/test.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3831 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_const_name.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      593 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_const_name.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1551 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_constants_and_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26064 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_copy_move.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_copy_move.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7280 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3992 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_custom_type_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1259 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_custom_type_setup.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1091 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_custom_type_setup.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4557 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_docstring_options.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2423 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_docstring_options.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19350 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eigen_matrix.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    29028 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eigen_matrix.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      473 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eigen_tensor.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10590 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eigen_tensor.inl
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9414 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eigen_tensor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.446977 libonvif-2.0.10/pybind11/tests/test_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1798 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1315 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/catch.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      543 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/external_module.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17396 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      237 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      275 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_embed/test_trampoline.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5722 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_enum.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8939 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_enum.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eval.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1143 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eval.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      119 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_eval_call.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12082 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_exceptions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      399 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_exceptions.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13176 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_exceptions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18155 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_factory_constructors.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16491 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_factory_constructors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5311 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_gil_scoped.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8507 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_gil_scoped.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3960 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_iostream.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7144 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_iostream.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9444 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13600 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4401 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_local_bindings.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8054 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_local_bindings.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22211 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18346 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_methods_and_attributes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4121 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_modules.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3963 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_modules.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12305 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11874 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_multiple_inheritance.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19861 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20414 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_array.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21114 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14272 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_dtypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4487 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9658 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_numpy_vectorize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2777 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_opaque_types.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1847 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_opaque_types.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9132 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_operator_overloading.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4332 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_operator_overloading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6719 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_pickling.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2720 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_pickling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30750 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_pytypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23629 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_pytypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21153 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8039 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18898 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_smart_ptr.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9530 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_smart_ptr.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21587 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_stl.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12239 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_stl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6205 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_stl_binders.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9804 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_stl_binders.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4617 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      741 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1855 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_thread.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      826 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_thread.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4501 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_type_caster_pyobject_ptr.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3260 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_type_caster_pyobject_ptr.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      603 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_union.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      148 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_union.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      845 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_unnamed_namespace_a.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1141 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_unnamed_namespace_a.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      341 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_unnamed_namespace_b.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      143 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_unnamed_namespace_b.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1471 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_vector_unique_ptr_member.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      329 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_vector_unique_ptr_member.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22991 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_virtual_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12913 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/test_virtual_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3226 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2657 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tests/valgrind-python.supp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.454977 libonvif-2.0.10/pybind11/tools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2449 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3105 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11190 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      817 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/JoinPaths.cmake
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1423 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/check-style.sh
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      952 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1117 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1031 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/libsize.py
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1311 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/make_changelog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14179 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6930 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8960 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8361 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       94 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2104 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1234 2023-05-25 17:26:50.000000 libonvif-2.0.10/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1601 2023-05-25 17:26:34.000000 libonvif-2.0.10/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-25 17:35:39.454977 libonvif-2.0.10/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2164 2023-05-25 17:26:34.000000 libonvif-2.0.10/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:39.454977 libonvif-2.0.10/src/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4518 2023-05-25 17:26:34.000000 libonvif-2.0.10/src/cencode.c
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   142373 2023-05-25 17:26:34.000000 libonvif-2.0.10/src/onvif.c
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6201 2023-05-25 17:26:34.000000 libonvif-2.0.10/src/onvif.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7079 2023-05-25 17:26:34.000000 libonvif-2.0.10/src/onvifboss.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9752 2023-05-25 17:26:34.000000 libonvif-2.0.10/src/sha1.c
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.322404 libonvif-2.0.9/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2200 2023-04-25 23:50:48.000000 libonvif-2.0.9/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26526 2023-04-25 23:50:48.000000 libonvif-2.0.9/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      121 2023-04-25 23:50:48.000000 libonvif-2.0.9/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2077 2023-04-26 00:47:34.322404 libonvif-2.0.9/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1497 2023-04-25 23:50:48.000000 libonvif-2.0.9/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.298404 libonvif-2.0.9/include/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2580 2023-04-25 23:50:48.000000 libonvif-2.0.9/include/cencode.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18497 2023-04-25 23:50:48.000000 libonvif-2.0.9/include/getopt-win.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9568 2023-04-25 23:50:48.000000 libonvif-2.0.9/include/onvif.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9447 2023-04-25 23:50:48.000000 libonvif-2.0.9/include/onvifboss.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2487 2023-04-25 23:50:48.000000 libonvif-2.0.9/include/sha1.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.298404 libonvif-2.0.9/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1271 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.appveyor.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      996 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.clang-format
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2605 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.clang-tidy
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2196 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1308 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.codespell-ignore-lines
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       45 2023-04-25 23:51:01.000000 libonvif-2.0.9/pybind11/.git
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       18 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.gitattributes
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/.github/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/CODEOWNERS
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15284 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/CONTRIBUTING.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2561 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      328 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/dependabot.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      116 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/labeler.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       50 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/labeler_merged.yml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/.github/matchers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      668 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/matchers/pylint.json
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/pull_request_template.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/.github/workflows/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    32023 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/ci.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2127 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/configure.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1460 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/format.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      559 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/labeler.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2558 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/pip.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2865 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.github/workflows/upstream.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      502 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.gitignore
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3588 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       62 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/.readthedocs.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11983 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1684 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      235 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7686 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/README.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/docs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      607 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/Doxyfile
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7417 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/Makefile
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.294404 libonvif-2.0.9/pybind11/docs/_static/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/docs/_static/css/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/_static/css/custom.css
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.302404 libonvif-2.0.9/pybind11/docs/advanced/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/docs/advanced/cast/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3937 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3429 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3889 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1556 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12371 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9586 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8863 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    47796 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/classes.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8453 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/embedding.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17796 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/exceptions.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26729 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/functions.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15651 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/misc.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/docs/advanced/pycpp/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      278 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17161 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6377 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9240 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/basics.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2856 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/benchmark.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   114174 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/changelog.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16380 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/classes.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/docs/cmake/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      273 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/cmake/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25777 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/compiling.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11574 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/conf.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13177 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/faq.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      613 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3277 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/installing.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3079 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/limitations.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    61034 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/pybind11-logo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    44653 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    87708 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    41121 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    85853 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2647 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/reference.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4414 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/release.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/requirements.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23489 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/docs/upgrade.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.298404 libonvif-2.0.9/pybind11/include/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/include/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23959 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7069 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    65952 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8458 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      120 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2096 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    28518 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    52990 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5491 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17869 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26498 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    42613 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1625 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    31450 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18140 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13475 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4731 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5002 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8262 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8862 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    79416 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9103 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2734 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   126420 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    94641 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.306404 libonvif-2.0.9/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4185 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15399 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29824 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/include/pybind11/stl_bind.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2765 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/noxfile.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.310404 libonvif-2.0.9/pybind11/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      429 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1544 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      233 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/_version.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1207 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/commands.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/py.typed
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17631 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pybind11/setup_helpers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2316 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1452 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4877 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21675 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5625 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/conftest.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11736 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/constructor_stats.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3578 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1776 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      396 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      926 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/env.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/extra_python_package/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8294 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/extra_python_package/test_files.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/extra_setuptools/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4153 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2847 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/local_bindings.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/object.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4517 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/pybind11_tests.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2685 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/pybind11_tests.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      600 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/requirements.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      855 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_async.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      536 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_async.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8567 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_buffers.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4848 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_buffers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16025 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17243 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_builtin_casters.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4118 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_call_policies.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6549 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_call_policies.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10858 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_callbacks.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6796 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_callbacks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3370 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_chrono.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5691 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_chrono.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24874 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_class.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14757 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_class.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2639 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1171 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1293 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      152 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1353 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1163 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1368 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      198 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_cmake_build/test.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3831 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_const_name.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      593 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_const_name.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5615 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1498 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_constants_and_functions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10886 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_copy_move.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_copy_move.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7280 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3992 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_custom_type_casters.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1259 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_custom_type_setup.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1091 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_custom_type_setup.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4557 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_docstring_options.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2423 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_docstring_options.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19350 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eigen_matrix.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29028 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eigen_matrix.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      473 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eigen_tensor.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10590 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eigen_tensor.inl
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9414 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eigen_tensor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.318404 libonvif-2.0.9/pybind11/tests/test_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1798 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1315 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/catch.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      543 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17410 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      237 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      275 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_embed/test_trampoline.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5722 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_enum.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8939 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_enum.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eval.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1143 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eval.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      119 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_eval_call.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12082 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_exceptions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      399 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_exceptions.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13001 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_exceptions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18155 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16491 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_factory_constructors.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5311 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8507 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_gil_scoped.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3960 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_iostream.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7202 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_iostream.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9444 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13600 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4401 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_local_bindings.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8054 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_local_bindings.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21388 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18105 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4121 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_modules.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4043 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_modules.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12305 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11874 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19861 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_array.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20414 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_array.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21114 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14272 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4487 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9658 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2777 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_opaque_types.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1847 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_opaque_types.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9132 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4332 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_operator_overloading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6719 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_pickling.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2720 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_pickling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    30750 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_pytypes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23629 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_pytypes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21153 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8039 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18898 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9530 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_smart_ptr.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21587 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_stl.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12232 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_stl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4622 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_stl_binders.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9138 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_stl_binders.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4617 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      741 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1855 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_thread.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      826 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_thread.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      603 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_union.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      148 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_union.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22991 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12913 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/test_virtual_functions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3226 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2657 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tests/valgrind-python.supp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.322404 libonvif-2.0.9/pybind11/tools/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2449 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3105 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11190 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      817 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/JoinPaths.cmake
+-rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1423 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/check-style.sh
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      952 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1117 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1031 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/libsize.py
+-rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1311 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14033 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6930 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8960 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8361 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       94 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2104 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1234 2023-04-25 23:51:08.000000 libonvif-2.0.9/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1558 2023-04-26 00:39:35.000000 libonvif-2.0.9/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-04-26 00:47:34.322404 libonvif-2.0.9/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4000 2023-04-26 00:39:45.000000 libonvif-2.0.9/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.322404 libonvif-2.0.9/src/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4383 2023-04-25 23:50:48.000000 libonvif-2.0.9/src/cencode.c
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-04-26 00:47:34.322404 libonvif-2.0.9/src/libonvif.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2077 2023-04-26 00:47:34.000000 libonvif-2.0.9/src/libonvif.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9344 2023-04-26 00:47:34.000000 libonvif-2.0.9/src/libonvif.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-26 00:47:34.000000 libonvif-2.0.9/src/libonvif.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-04-26 00:22:11.000000 libonvif-2.0.9/src/libonvif.egg-info/not-zip-safe
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        9 2023-04-26 00:47:34.000000 libonvif-2.0.9/src/libonvif.egg-info/top_level.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   139248 2023-04-25 23:50:48.000000 libonvif-2.0.9/src/onvif.c
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6062 2023-04-26 00:39:23.000000 libonvif-2.0.9/src/onvif.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6810 2023-04-25 23:50:48.000000 libonvif-2.0.9/src/onvifboss.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9431 2023-04-25 23:50:48.000000 libonvif-2.0.9/src/sha1.c
```

### Comparing `libonvif-2.0.10/CMakeLists.txt` & `libonvif-2.0.9/CMakeLists.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,91 @@
-#*******************************************************************************
-# libonvif/libonvif/CMakeLists.txt
-#
-# Copyright (c) 2023 Stephen Rhodes 
-#
-# This program is free software; you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation; either version 2 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-#
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
-#
-#******************************************************************************/
-
-cmake_minimum_required(VERSION 3.17)
-
-project(libonvif VERSION 2.0.7)
-
-set(CMAKE_CXX_STANDARD 17)
-set(CMAKE_CXX_STANDARD_REQUIRED True)
-
-add_definitions(-w)
-
-find_package(LibXml2 REQUIRED)
-
-if (NOT WITHOUT_LIBS)
-
-    add_library(libonvif SHARED
-        src/onvif.c
-        src/cencode.c
-        src/sha1.c
-        src/onvifboss.cpp
-    )
-
-    target_link_libraries(libonvif PRIVATE
-        ${LIBXML2_LIBRARIES}
-    )
-
-    if (UNIX)
-        set_target_properties(libonvif PROPERTIES
-            OUTPUT_NAME onvif
-            SOVERSION 1
-        )
-    endif()
-
-    target_include_directories(libonvif PUBLIC
-        include
-        ${Iconv_INCLUDE_DIRS}
-        ${LIBXML2_INCLUDE_DIRS}
-    )
-
-endif()
-
-IF (NOT WITHOUT_PYTHON)
-
-    add_subdirectory(pybind11)
-
-    pybind11_add_module(pyonvif
-        src/onvif.cpp
-        src/onvif.c
-        src/cencode.c
-        src/sha1.c
-        src/onvifboss.cpp
-    )
-
-    set_target_properties(pyonvif PROPERTIES
-        OUTPUT_NAME libonvif
-    )
-
-    target_link_libraries(pyonvif PRIVATE
-        ${LIBXML2_LIBRARIES}
-    )
-
-    target_include_directories(pyonvif PUBLIC
-        include
-        ${Iconv_INCLUDE_DIRS}
-        ${LIBXML2_INCLUDE_DIRS}
-    )
-
-endif()
+#*******************************************************************************
+# libonvif/libonvif/CMakeLists.txt
+#
+# Copyright (c) 2023 Stephen Rhodes 
+#
+# This program is free software; you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation; either version 2 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+#
+# You should have received a copy of the GNU General Public License along
+# with this program; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+#
+#******************************************************************************/
+
+cmake_minimum_required(VERSION 3.17)
+
+project(libonvif VERSION 2.0.7)
+
+set(CMAKE_CXX_STANDARD 17)
+set(CMAKE_CXX_STANDARD_REQUIRED True)
+
+if(WIN32)
+    find_package(Iconv REQUIRED)
+endif()
+
+add_definitions(-w)
+
+find_package(LibXml2 REQUIRED)
+
+if (NOT WITHOUT_LIBS)
+
+    add_library(libonvif SHARED
+        src/onvif.c
+        src/cencode.c
+        src/sha1.c
+        src/onvifboss.cpp
+    )
+
+    target_link_libraries(libonvif PRIVATE
+        ${LIBXML2_LIBRARIES}
+    )
+
+    if (UNIX)
+        set_target_properties(libonvif PROPERTIES
+            OUTPUT_NAME onvif
+            SOVERSION 1
+        )
+    endif()
+
+    target_include_directories(libonvif PUBLIC
+        include
+        ${Iconv_INCLUDE_DIRS}
+        ${LIBXML2_INCLUDE_DIRS}
+    )
+
+endif()
+
+IF (NOT WITHOUT_PYTHON)
+
+    add_subdirectory(pybind11)
+
+    pybind11_add_module(pyonvif
+        src/onvif.cpp
+        src/onvif.c
+        src/cencode.c
+        src/sha1.c
+        src/onvifboss.cpp
+    )
+
+    set_target_properties(pyonvif PROPERTIES
+        OUTPUT_NAME libonvif
+    )
+
+    target_link_libraries(pyonvif PRIVATE
+        ${LIBXML2_LIBRARIES}
+    )
+
+    target_include_directories(pyonvif PUBLIC
+        include
+        ${Iconv_INCLUDE_DIRS}
+        ${LIBXML2_INCLUDE_DIRS}
+    )
+
+endif()
```

### Comparing `libonvif-2.0.10/LICENSE` & `libonvif-2.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,502 +1,502 @@
-                  GNU LESSER GENERAL PUBLIC LICENSE
-                       Version 2.1, February 1999
-
- Copyright (C) 1991, 1999 Free Software Foundation, Inc.
- 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-[This is the first released version of the Lesser GPL.  It also counts
- as the successor of the GNU Library Public License, version 2, hence
- the version number 2.1.]
-
-                            Preamble
-
-  The licenses for most software are designed to take away your
-freedom to share and change it.  By contrast, the GNU General Public
-Licenses are intended to guarantee your freedom to share and change
-free software--to make sure the software is free for all its users.
-
-  This license, the Lesser General Public License, applies to some
-specially designated software packages--typically libraries--of the
-Free Software Foundation and other authors who decide to use it.  You
-can use it too, but we suggest you first think carefully about whether
-this license or the ordinary General Public License is the better
-strategy to use in any particular case, based on the explanations below.
-
-  When we speak of free software, we are referring to freedom of use,
-not price.  Our General Public Licenses are designed to make sure that
-you have the freedom to distribute copies of free software (and charge
-for this service if you wish); that you receive source code or can get
-it if you want it; that you can change the software and use pieces of
-it in new free programs; and that you are informed that you can do
-these things.
-
-  To protect your rights, we need to make restrictions that forbid
-distributors to deny you these rights or to ask you to surrender these
-rights.  These restrictions translate to certain responsibilities for
-you if you distribute copies of the library or if you modify it.
-
-  For example, if you distribute copies of the library, whether gratis
-or for a fee, you must give the recipients all the rights that we gave
-you.  You must make sure that they, too, receive or can get the source
-code.  If you link other code with the library, you must provide
-complete object files to the recipients, so that they can relink them
-with the library after making changes to the library and recompiling
-it.  And you must show them these terms so they know their rights.
-
-  We protect your rights with a two-step method: (1) we copyright the
-library, and (2) we offer you this license, which gives you legal
-permission to copy, distribute and/or modify the library.
-
-  To protect each distributor, we want to make it very clear that
-there is no warranty for the free library.  Also, if the library is
-modified by someone else and passed on, the recipients should know
-that what they have is not the original version, so that the original
-author's reputation will not be affected by problems that might be
-introduced by others.
-
-  Finally, software patents pose a constant threat to the existence of
-any free program.  We wish to make sure that a company cannot
-effectively restrict the users of a free program by obtaining a
-restrictive license from a patent holder.  Therefore, we insist that
-any patent license obtained for a version of the library must be
-consistent with the full freedom of use specified in this license.
-
-  Most GNU software, including some libraries, is covered by the
-ordinary GNU General Public License.  This license, the GNU Lesser
-General Public License, applies to certain designated libraries, and
-is quite different from the ordinary General Public License.  We use
-this license for certain libraries in order to permit linking those
-libraries into non-free programs.
-
-  When a program is linked with a library, whether statically or using
-a shared library, the combination of the two is legally speaking a
-combined work, a derivative of the original library.  The ordinary
-General Public License therefore permits such linking only if the
-entire combination fits its criteria of freedom.  The Lesser General
-Public License permits more lax criteria for linking other code with
-the library.
-
-  We call this license the "Lesser" General Public License because it
-does Less to protect the user's freedom than the ordinary General
-Public License.  It also provides other free software developers Less
-of an advantage over competing non-free programs.  These disadvantages
-are the reason we use the ordinary General Public License for many
-libraries.  However, the Lesser license provides advantages in certain
-special circumstances.
-
-  For example, on rare occasions, there may be a special need to
-encourage the widest possible use of a certain library, so that it becomes
-a de-facto standard.  To achieve this, non-free programs must be
-allowed to use the library.  A more frequent case is that a free
-library does the same job as widely used non-free libraries.  In this
-case, there is little to gain by limiting the free library to free
-software only, so we use the Lesser General Public License.
-
-  In other cases, permission to use a particular library in non-free
-programs enables a greater number of people to use a large body of
-free software.  For example, permission to use the GNU C Library in
-non-free programs enables many more people to use the whole GNU
-operating system, as well as its variant, the GNU/Linux operating
-system.
-
-  Although the Lesser General Public License is Less protective of the
-users' freedom, it does ensure that the user of a program that is
-linked with the Library has the freedom and the wherewithal to run
-that program using a modified version of the Library.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.  Pay close attention to the difference between a
-"work based on the library" and a "work that uses the library".  The
-former contains code derived from the library, whereas the latter must
-be combined with the library in order to run.
-
-                  GNU LESSER GENERAL PUBLIC LICENSE
-   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
-
-  0. This License Agreement applies to any software library or other
-program which contains a notice placed by the copyright holder or
-other authorized party saying it may be distributed under the terms of
-this Lesser General Public License (also called "this License").
-Each licensee is addressed as "you".
-
-  A "library" means a collection of software functions and/or data
-prepared so as to be conveniently linked with application programs
-(which use some of those functions and data) to form executables.
-
-  The "Library", below, refers to any such software library or work
-which has been distributed under these terms.  A "work based on the
-Library" means either the Library or any derivative work under
-copyright law: that is to say, a work containing the Library or a
-portion of it, either verbatim or with modifications and/or translated
-straightforwardly into another language.  (Hereinafter, translation is
-included without limitation in the term "modification".)
-
-  "Source code" for a work means the preferred form of the work for
-making modifications to it.  For a library, complete source code means
-all the source code for all modules it contains, plus any associated
-interface definition files, plus the scripts used to control compilation
-and installation of the library.
-
-  Activities other than copying, distribution and modification are not
-covered by this License; they are outside its scope.  The act of
-running a program using the Library is not restricted, and output from
-such a program is covered only if its contents constitute a work based
-on the Library (independent of the use of the Library in a tool for
-writing it).  Whether that is true depends on what the Library does
-and what the program that uses the Library does.
-
-  1. You may copy and distribute verbatim copies of the Library's
-complete source code as you receive it, in any medium, provided that
-you conspicuously and appropriately publish on each copy an
-appropriate copyright notice and disclaimer of warranty; keep intact
-all the notices that refer to this License and to the absence of any
-warranty; and distribute a copy of this License along with the
-Library.
-
-  You may charge a fee for the physical act of transferring a copy,
-and you may at your option offer warranty protection in exchange for a
-fee.
-
-  2. You may modify your copy or copies of the Library or any portion
-of it, thus forming a work based on the Library, and copy and
-distribute such modifications or work under the terms of Section 1
-above, provided that you also meet all of these conditions:
-
-    a) The modified work must itself be a software library.
-
-    b) You must cause the files modified to carry prominent notices
-    stating that you changed the files and the date of any change.
-
-    c) You must cause the whole of the work to be licensed at no
-    charge to all third parties under the terms of this License.
-
-    d) If a facility in the modified Library refers to a function or a
-    table of data to be supplied by an application program that uses
-    the facility, other than as an argument passed when the facility
-    is invoked, then you must make a good faith effort to ensure that,
-    in the event an application does not supply such function or
-    table, the facility still operates, and performs whatever part of
-    its purpose remains meaningful.
-
-    (For example, a function in a library to compute square roots has
-    a purpose that is entirely well-defined independent of the
-    application.  Therefore, Subsection 2d requires that any
-    application-supplied function or table used by this function must
-    be optional: if the application does not supply it, the square
-    root function must still compute square roots.)
-
-These requirements apply to the modified work as a whole.  If
-identifiable sections of that work are not derived from the Library,
-and can be reasonably considered independent and separate works in
-themselves, then this License, and its terms, do not apply to those
-sections when you distribute them as separate works.  But when you
-distribute the same sections as part of a whole which is a work based
-on the Library, the distribution of the whole must be on the terms of
-this License, whose permissions for other licensees extend to the
-entire whole, and thus to each and every part regardless of who wrote
-it.
-
-Thus, it is not the intent of this section to claim rights or contest
-your rights to work written entirely by you; rather, the intent is to
-exercise the right to control the distribution of derivative or
-collective works based on the Library.
-
-In addition, mere aggregation of another work not based on the Library
-with the Library (or with a work based on the Library) on a volume of
-a storage or distribution medium does not bring the other work under
-the scope of this License.
-
-  3. You may opt to apply the terms of the ordinary GNU General Public
-License instead of this License to a given copy of the Library.  To do
-this, you must alter all the notices that refer to this License, so
-that they refer to the ordinary GNU General Public License, version 2,
-instead of to this License.  (If a newer version than version 2 of the
-ordinary GNU General Public License has appeared, then you can specify
-that version instead if you wish.)  Do not make any other change in
-these notices.
-
-  Once this change is made in a given copy, it is irreversible for
-that copy, so the ordinary GNU General Public License applies to all
-subsequent copies and derivative works made from that copy.
-
-  This option is useful when you wish to copy part of the code of
-the Library into a program that is not a library.
-
-  4. You may copy and distribute the Library (or a portion or
-derivative of it, under Section 2) in object code or executable form
-under the terms of Sections 1 and 2 above provided that you accompany
-it with the complete corresponding machine-readable source code, which
-must be distributed under the terms of Sections 1 and 2 above on a
-medium customarily used for software interchange.
-
-  If distribution of object code is made by offering access to copy
-from a designated place, then offering equivalent access to copy the
-source code from the same place satisfies the requirement to
-distribute the source code, even though third parties are not
-compelled to copy the source along with the object code.
-
-  5. A program that contains no derivative of any portion of the
-Library, but is designed to work with the Library by being compiled or
-linked with it, is called a "work that uses the Library".  Such a
-work, in isolation, is not a derivative work of the Library, and
-therefore falls outside the scope of this License.
-
-  However, linking a "work that uses the Library" with the Library
-creates an executable that is a derivative of the Library (because it
-contains portions of the Library), rather than a "work that uses the
-library".  The executable is therefore covered by this License.
-Section 6 states terms for distribution of such executables.
-
-  When a "work that uses the Library" uses material from a header file
-that is part of the Library, the object code for the work may be a
-derivative work of the Library even though the source code is not.
-Whether this is true is especially significant if the work can be
-linked without the Library, or if the work is itself a library.  The
-threshold for this to be true is not precisely defined by law.
-
-  If such an object file uses only numerical parameters, data
-structure layouts and accessors, and small macros and small inline
-functions (ten lines or less in length), then the use of the object
-file is unrestricted, regardless of whether it is legally a derivative
-work.  (Executables containing this object code plus portions of the
-Library will still fall under Section 6.)
-
-  Otherwise, if the work is a derivative of the Library, you may
-distribute the object code for the work under the terms of Section 6.
-Any executables containing that work also fall under Section 6,
-whether or not they are linked directly with the Library itself.
-
-  6. As an exception to the Sections above, you may also combine or
-link a "work that uses the Library" with the Library to produce a
-work containing portions of the Library, and distribute that work
-under terms of your choice, provided that the terms permit
-modification of the work for the customer's own use and reverse
-engineering for debugging such modifications.
-
-  You must give prominent notice with each copy of the work that the
-Library is used in it and that the Library and its use are covered by
-this License.  You must supply a copy of this License.  If the work
-during execution displays copyright notices, you must include the
-copyright notice for the Library among them, as well as a reference
-directing the user to the copy of this License.  Also, you must do one
-of these things:
-
-    a) Accompany the work with the complete corresponding
-    machine-readable source code for the Library including whatever
-    changes were used in the work (which must be distributed under
-    Sections 1 and 2 above); and, if the work is an executable linked
-    with the Library, with the complete machine-readable "work that
-    uses the Library", as object code and/or source code, so that the
-    user can modify the Library and then relink to produce a modified
-    executable containing the modified Library.  (It is understood
-    that the user who changes the contents of definitions files in the
-    Library will not necessarily be able to recompile the application
-    to use the modified definitions.)
-
-    b) Use a suitable shared library mechanism for linking with the
-    Library.  A suitable mechanism is one that (1) uses at run time a
-    copy of the library already present on the user's computer system,
-    rather than copying library functions into the executable, and (2)
-    will operate properly with a modified version of the library, if
-    the user installs one, as long as the modified version is
-    interface-compatible with the version that the work was made with.
-
-    c) Accompany the work with a written offer, valid for at
-    least three years, to give the same user the materials
-    specified in Subsection 6a, above, for a charge no more
-    than the cost of performing this distribution.
-
-    d) If distribution of the work is made by offering access to copy
-    from a designated place, offer equivalent access to copy the above
-    specified materials from the same place.
-
-    e) Verify that the user has already received a copy of these
-    materials or that you have already sent this user a copy.
-
-  For an executable, the required form of the "work that uses the
-Library" must include any data and utility programs needed for
-reproducing the executable from it.  However, as a special exception,
-the materials to be distributed need not include anything that is
-normally distributed (in either source or binary form) with the major
-components (compiler, kernel, and so on) of the operating system on
-which the executable runs, unless that component itself accompanies
-the executable.
-
-  It may happen that this requirement contradicts the license
-restrictions of other proprietary libraries that do not normally
-accompany the operating system.  Such a contradiction means you cannot
-use both them and the Library together in an executable that you
-distribute.
-
-  7. You may place library facilities that are a work based on the
-Library side-by-side in a single library together with other library
-facilities not covered by this License, and distribute such a combined
-library, provided that the separate distribution of the work based on
-the Library and of the other library facilities is otherwise
-permitted, and provided that you do these two things:
-
-    a) Accompany the combined library with a copy of the same work
-    based on the Library, uncombined with any other library
-    facilities.  This must be distributed under the terms of the
-    Sections above.
-
-    b) Give prominent notice with the combined library of the fact
-    that part of it is a work based on the Library, and explaining
-    where to find the accompanying uncombined form of the same work.
-
-  8. You may not copy, modify, sublicense, link with, or distribute
-the Library except as expressly provided under this License.  Any
-attempt otherwise to copy, modify, sublicense, link with, or
-distribute the Library is void, and will automatically terminate your
-rights under this License.  However, parties who have received copies,
-or rights, from you under this License will not have their licenses
-terminated so long as such parties remain in full compliance.
-
-  9. You are not required to accept this License, since you have not
-signed it.  However, nothing else grants you permission to modify or
-distribute the Library or its derivative works.  These actions are
-prohibited by law if you do not accept this License.  Therefore, by
-modifying or distributing the Library (or any work based on the
-Library), you indicate your acceptance of this License to do so, and
-all its terms and conditions for copying, distributing or modifying
-the Library or works based on it.
-
-  10. Each time you redistribute the Library (or any work based on the
-Library), the recipient automatically receives a license from the
-original licensor to copy, distribute, link with or modify the Library
-subject to these terms and conditions.  You may not impose any further
-restrictions on the recipients' exercise of the rights granted herein.
-You are not responsible for enforcing compliance by third parties with
-this License.
-
-  11. If, as a consequence of a court judgment or allegation of patent
-infringement or for any other reason (not limited to patent issues),
-conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot
-distribute so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you
-may not distribute the Library at all.  For example, if a patent
-license would not permit royalty-free redistribution of the Library by
-all those who receive copies directly or indirectly through you, then
-the only way you could satisfy both it and this License would be to
-refrain entirely from distribution of the Library.
-
-If any portion of this section is held invalid or unenforceable under any
-particular circumstance, the balance of the section is intended to apply,
-and the section as a whole is intended to apply in other circumstances.
-
-It is not the purpose of this section to induce you to infringe any
-patents or other property right claims or to contest validity of any
-such claims; this section has the sole purpose of protecting the
-integrity of the free software distribution system which is
-implemented by public license practices.  Many people have made
-generous contributions to the wide range of software distributed
-through that system in reliance on consistent application of that
-system; it is up to the author/donor to decide if he or she is willing
-to distribute software through any other system and a licensee cannot
-impose that choice.
-
-This section is intended to make thoroughly clear what is believed to
-be a consequence of the rest of this License.
-
-  12. If the distribution and/or use of the Library is restricted in
-certain countries either by patents or by copyrighted interfaces, the
-original copyright holder who places the Library under this License may add
-an explicit geographical distribution limitation excluding those countries,
-so that distribution is permitted only in or among countries not thus
-excluded.  In such case, this License incorporates the limitation as if
-written in the body of this License.
-
-  13. The Free Software Foundation may publish revised and/or new
-versions of the Lesser General Public License from time to time.
-Such new versions will be similar in spirit to the present version,
-but may differ in detail to address new problems or concerns.
-
-Each version is given a distinguishing version number.  If the Library
-specifies a version number of this License which applies to it and
-"any later version", you have the option of following the terms and
-conditions either of that version or of any later version published by
-the Free Software Foundation.  If the Library does not specify a
-license version number, you may choose any version ever published by
-the Free Software Foundation.
-
-  14. If you wish to incorporate parts of the Library into other free
-programs whose distribution conditions are incompatible with these,
-write to the author to ask for permission.  For software which is
-copyrighted by the Free Software Foundation, write to the Free
-Software Foundation; we sometimes make exceptions for this.  Our
-decision will be guided by the two goals of preserving the free status
-of all derivatives of our free software and of promoting the sharing
-and reuse of software generally.
-
-                            NO WARRANTY
-
-  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
-WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
-EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
-OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
-KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
-LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
-THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
-WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
-AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
-FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
-CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
-LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
-RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
-FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
-SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
-DAMAGES.
-
-                     END OF TERMS AND CONDITIONS
-
-           How to Apply These Terms to Your New Libraries
-
-  If you develop a new library, and you want it to be of the greatest
-possible use to the public, we recommend making it free software that
-everyone can redistribute and change.  You can do so by permitting
-redistribution under these terms (or, alternatively, under the terms of the
-ordinary General Public License).
-
-  To apply these terms, attach the following notices to the library.  It is
-safest to attach them to the start of each source file to most effectively
-convey the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the library's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Lesser General Public
-    License as published by the Free Software Foundation; either
-    version 2.1 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public
-    License along with this library; if not, write to the Free Software
-    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-
-Also add information on how to contact you by electronic and paper mail.
-
-You should also get your employer (if you work as a programmer) or your
-school, if any, to sign a "copyright disclaimer" for the library, if
-necessary.  Here is a sample; alter the names:
-
-  Yoyodyne, Inc., hereby disclaims all copyright interest in the
-  library `Frob' (a library for tweaking knobs) written by James Random Hacker.
-
-  <signature of Ty Coon>, 1 April 1990
-  Ty Coon, President of Vice
-
-That's all there is to it!
+                  GNU LESSER GENERAL PUBLIC LICENSE
+                       Version 2.1, February 1999
+
+ Copyright (C) 1991, 1999 Free Software Foundation, Inc.
+ 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+[This is the first released version of the Lesser GPL.  It also counts
+ as the successor of the GNU Library Public License, version 2, hence
+ the version number 2.1.]
+
+                            Preamble
+
+  The licenses for most software are designed to take away your
+freedom to share and change it.  By contrast, the GNU General Public
+Licenses are intended to guarantee your freedom to share and change
+free software--to make sure the software is free for all its users.
+
+  This license, the Lesser General Public License, applies to some
+specially designated software packages--typically libraries--of the
+Free Software Foundation and other authors who decide to use it.  You
+can use it too, but we suggest you first think carefully about whether
+this license or the ordinary General Public License is the better
+strategy to use in any particular case, based on the explanations below.
+
+  When we speak of free software, we are referring to freedom of use,
+not price.  Our General Public Licenses are designed to make sure that
+you have the freedom to distribute copies of free software (and charge
+for this service if you wish); that you receive source code or can get
+it if you want it; that you can change the software and use pieces of
+it in new free programs; and that you are informed that you can do
+these things.
+
+  To protect your rights, we need to make restrictions that forbid
+distributors to deny you these rights or to ask you to surrender these
+rights.  These restrictions translate to certain responsibilities for
+you if you distribute copies of the library or if you modify it.
+
+  For example, if you distribute copies of the library, whether gratis
+or for a fee, you must give the recipients all the rights that we gave
+you.  You must make sure that they, too, receive or can get the source
+code.  If you link other code with the library, you must provide
+complete object files to the recipients, so that they can relink them
+with the library after making changes to the library and recompiling
+it.  And you must show them these terms so they know their rights.
+
+  We protect your rights with a two-step method: (1) we copyright the
+library, and (2) we offer you this license, which gives you legal
+permission to copy, distribute and/or modify the library.
+
+  To protect each distributor, we want to make it very clear that
+there is no warranty for the free library.  Also, if the library is
+modified by someone else and passed on, the recipients should know
+that what they have is not the original version, so that the original
+author's reputation will not be affected by problems that might be
+introduced by others.
+
+  Finally, software patents pose a constant threat to the existence of
+any free program.  We wish to make sure that a company cannot
+effectively restrict the users of a free program by obtaining a
+restrictive license from a patent holder.  Therefore, we insist that
+any patent license obtained for a version of the library must be
+consistent with the full freedom of use specified in this license.
+
+  Most GNU software, including some libraries, is covered by the
+ordinary GNU General Public License.  This license, the GNU Lesser
+General Public License, applies to certain designated libraries, and
+is quite different from the ordinary General Public License.  We use
+this license for certain libraries in order to permit linking those
+libraries into non-free programs.
+
+  When a program is linked with a library, whether statically or using
+a shared library, the combination of the two is legally speaking a
+combined work, a derivative of the original library.  The ordinary
+General Public License therefore permits such linking only if the
+entire combination fits its criteria of freedom.  The Lesser General
+Public License permits more lax criteria for linking other code with
+the library.
+
+  We call this license the "Lesser" General Public License because it
+does Less to protect the user's freedom than the ordinary General
+Public License.  It also provides other free software developers Less
+of an advantage over competing non-free programs.  These disadvantages
+are the reason we use the ordinary General Public License for many
+libraries.  However, the Lesser license provides advantages in certain
+special circumstances.
+
+  For example, on rare occasions, there may be a special need to
+encourage the widest possible use of a certain library, so that it becomes
+a de-facto standard.  To achieve this, non-free programs must be
+allowed to use the library.  A more frequent case is that a free
+library does the same job as widely used non-free libraries.  In this
+case, there is little to gain by limiting the free library to free
+software only, so we use the Lesser General Public License.
+
+  In other cases, permission to use a particular library in non-free
+programs enables a greater number of people to use a large body of
+free software.  For example, permission to use the GNU C Library in
+non-free programs enables many more people to use the whole GNU
+operating system, as well as its variant, the GNU/Linux operating
+system.
+
+  Although the Lesser General Public License is Less protective of the
+users' freedom, it does ensure that the user of a program that is
+linked with the Library has the freedom and the wherewithal to run
+that program using a modified version of the Library.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.  Pay close attention to the difference between a
+"work based on the library" and a "work that uses the library".  The
+former contains code derived from the library, whereas the latter must
+be combined with the library in order to run.
+
+                  GNU LESSER GENERAL PUBLIC LICENSE
+   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
+
+  0. This License Agreement applies to any software library or other
+program which contains a notice placed by the copyright holder or
+other authorized party saying it may be distributed under the terms of
+this Lesser General Public License (also called "this License").
+Each licensee is addressed as "you".
+
+  A "library" means a collection of software functions and/or data
+prepared so as to be conveniently linked with application programs
+(which use some of those functions and data) to form executables.
+
+  The "Library", below, refers to any such software library or work
+which has been distributed under these terms.  A "work based on the
+Library" means either the Library or any derivative work under
+copyright law: that is to say, a work containing the Library or a
+portion of it, either verbatim or with modifications and/or translated
+straightforwardly into another language.  (Hereinafter, translation is
+included without limitation in the term "modification".)
+
+  "Source code" for a work means the preferred form of the work for
+making modifications to it.  For a library, complete source code means
+all the source code for all modules it contains, plus any associated
+interface definition files, plus the scripts used to control compilation
+and installation of the library.
+
+  Activities other than copying, distribution and modification are not
+covered by this License; they are outside its scope.  The act of
+running a program using the Library is not restricted, and output from
+such a program is covered only if its contents constitute a work based
+on the Library (independent of the use of the Library in a tool for
+writing it).  Whether that is true depends on what the Library does
+and what the program that uses the Library does.
+
+  1. You may copy and distribute verbatim copies of the Library's
+complete source code as you receive it, in any medium, provided that
+you conspicuously and appropriately publish on each copy an
+appropriate copyright notice and disclaimer of warranty; keep intact
+all the notices that refer to this License and to the absence of any
+warranty; and distribute a copy of this License along with the
+Library.
+
+  You may charge a fee for the physical act of transferring a copy,
+and you may at your option offer warranty protection in exchange for a
+fee.
+
+  2. You may modify your copy or copies of the Library or any portion
+of it, thus forming a work based on the Library, and copy and
+distribute such modifications or work under the terms of Section 1
+above, provided that you also meet all of these conditions:
+
+    a) The modified work must itself be a software library.
+
+    b) You must cause the files modified to carry prominent notices
+    stating that you changed the files and the date of any change.
+
+    c) You must cause the whole of the work to be licensed at no
+    charge to all third parties under the terms of this License.
+
+    d) If a facility in the modified Library refers to a function or a
+    table of data to be supplied by an application program that uses
+    the facility, other than as an argument passed when the facility
+    is invoked, then you must make a good faith effort to ensure that,
+    in the event an application does not supply such function or
+    table, the facility still operates, and performs whatever part of
+    its purpose remains meaningful.
+
+    (For example, a function in a library to compute square roots has
+    a purpose that is entirely well-defined independent of the
+    application.  Therefore, Subsection 2d requires that any
+    application-supplied function or table used by this function must
+    be optional: if the application does not supply it, the square
+    root function must still compute square roots.)
+
+These requirements apply to the modified work as a whole.  If
+identifiable sections of that work are not derived from the Library,
+and can be reasonably considered independent and separate works in
+themselves, then this License, and its terms, do not apply to those
+sections when you distribute them as separate works.  But when you
+distribute the same sections as part of a whole which is a work based
+on the Library, the distribution of the whole must be on the terms of
+this License, whose permissions for other licensees extend to the
+entire whole, and thus to each and every part regardless of who wrote
+it.
+
+Thus, it is not the intent of this section to claim rights or contest
+your rights to work written entirely by you; rather, the intent is to
+exercise the right to control the distribution of derivative or
+collective works based on the Library.
+
+In addition, mere aggregation of another work not based on the Library
+with the Library (or with a work based on the Library) on a volume of
+a storage or distribution medium does not bring the other work under
+the scope of this License.
+
+  3. You may opt to apply the terms of the ordinary GNU General Public
+License instead of this License to a given copy of the Library.  To do
+this, you must alter all the notices that refer to this License, so
+that they refer to the ordinary GNU General Public License, version 2,
+instead of to this License.  (If a newer version than version 2 of the
+ordinary GNU General Public License has appeared, then you can specify
+that version instead if you wish.)  Do not make any other change in
+these notices.
+
+  Once this change is made in a given copy, it is irreversible for
+that copy, so the ordinary GNU General Public License applies to all
+subsequent copies and derivative works made from that copy.
+
+  This option is useful when you wish to copy part of the code of
+the Library into a program that is not a library.
+
+  4. You may copy and distribute the Library (or a portion or
+derivative of it, under Section 2) in object code or executable form
+under the terms of Sections 1 and 2 above provided that you accompany
+it with the complete corresponding machine-readable source code, which
+must be distributed under the terms of Sections 1 and 2 above on a
+medium customarily used for software interchange.
+
+  If distribution of object code is made by offering access to copy
+from a designated place, then offering equivalent access to copy the
+source code from the same place satisfies the requirement to
+distribute the source code, even though third parties are not
+compelled to copy the source along with the object code.
+
+  5. A program that contains no derivative of any portion of the
+Library, but is designed to work with the Library by being compiled or
+linked with it, is called a "work that uses the Library".  Such a
+work, in isolation, is not a derivative work of the Library, and
+therefore falls outside the scope of this License.
+
+  However, linking a "work that uses the Library" with the Library
+creates an executable that is a derivative of the Library (because it
+contains portions of the Library), rather than a "work that uses the
+library".  The executable is therefore covered by this License.
+Section 6 states terms for distribution of such executables.
+
+  When a "work that uses the Library" uses material from a header file
+that is part of the Library, the object code for the work may be a
+derivative work of the Library even though the source code is not.
+Whether this is true is especially significant if the work can be
+linked without the Library, or if the work is itself a library.  The
+threshold for this to be true is not precisely defined by law.
+
+  If such an object file uses only numerical parameters, data
+structure layouts and accessors, and small macros and small inline
+functions (ten lines or less in length), then the use of the object
+file is unrestricted, regardless of whether it is legally a derivative
+work.  (Executables containing this object code plus portions of the
+Library will still fall under Section 6.)
+
+  Otherwise, if the work is a derivative of the Library, you may
+distribute the object code for the work under the terms of Section 6.
+Any executables containing that work also fall under Section 6,
+whether or not they are linked directly with the Library itself.
+
+  6. As an exception to the Sections above, you may also combine or
+link a "work that uses the Library" with the Library to produce a
+work containing portions of the Library, and distribute that work
+under terms of your choice, provided that the terms permit
+modification of the work for the customer's own use and reverse
+engineering for debugging such modifications.
+
+  You must give prominent notice with each copy of the work that the
+Library is used in it and that the Library and its use are covered by
+this License.  You must supply a copy of this License.  If the work
+during execution displays copyright notices, you must include the
+copyright notice for the Library among them, as well as a reference
+directing the user to the copy of this License.  Also, you must do one
+of these things:
+
+    a) Accompany the work with the complete corresponding
+    machine-readable source code for the Library including whatever
+    changes were used in the work (which must be distributed under
+    Sections 1 and 2 above); and, if the work is an executable linked
+    with the Library, with the complete machine-readable "work that
+    uses the Library", as object code and/or source code, so that the
+    user can modify the Library and then relink to produce a modified
+    executable containing the modified Library.  (It is understood
+    that the user who changes the contents of definitions files in the
+    Library will not necessarily be able to recompile the application
+    to use the modified definitions.)
+
+    b) Use a suitable shared library mechanism for linking with the
+    Library.  A suitable mechanism is one that (1) uses at run time a
+    copy of the library already present on the user's computer system,
+    rather than copying library functions into the executable, and (2)
+    will operate properly with a modified version of the library, if
+    the user installs one, as long as the modified version is
+    interface-compatible with the version that the work was made with.
+
+    c) Accompany the work with a written offer, valid for at
+    least three years, to give the same user the materials
+    specified in Subsection 6a, above, for a charge no more
+    than the cost of performing this distribution.
+
+    d) If distribution of the work is made by offering access to copy
+    from a designated place, offer equivalent access to copy the above
+    specified materials from the same place.
+
+    e) Verify that the user has already received a copy of these
+    materials or that you have already sent this user a copy.
+
+  For an executable, the required form of the "work that uses the
+Library" must include any data and utility programs needed for
+reproducing the executable from it.  However, as a special exception,
+the materials to be distributed need not include anything that is
+normally distributed (in either source or binary form) with the major
+components (compiler, kernel, and so on) of the operating system on
+which the executable runs, unless that component itself accompanies
+the executable.
+
+  It may happen that this requirement contradicts the license
+restrictions of other proprietary libraries that do not normally
+accompany the operating system.  Such a contradiction means you cannot
+use both them and the Library together in an executable that you
+distribute.
+
+  7. You may place library facilities that are a work based on the
+Library side-by-side in a single library together with other library
+facilities not covered by this License, and distribute such a combined
+library, provided that the separate distribution of the work based on
+the Library and of the other library facilities is otherwise
+permitted, and provided that you do these two things:
+
+    a) Accompany the combined library with a copy of the same work
+    based on the Library, uncombined with any other library
+    facilities.  This must be distributed under the terms of the
+    Sections above.
+
+    b) Give prominent notice with the combined library of the fact
+    that part of it is a work based on the Library, and explaining
+    where to find the accompanying uncombined form of the same work.
+
+  8. You may not copy, modify, sublicense, link with, or distribute
+the Library except as expressly provided under this License.  Any
+attempt otherwise to copy, modify, sublicense, link with, or
+distribute the Library is void, and will automatically terminate your
+rights under this License.  However, parties who have received copies,
+or rights, from you under this License will not have their licenses
+terminated so long as such parties remain in full compliance.
+
+  9. You are not required to accept this License, since you have not
+signed it.  However, nothing else grants you permission to modify or
+distribute the Library or its derivative works.  These actions are
+prohibited by law if you do not accept this License.  Therefore, by
+modifying or distributing the Library (or any work based on the
+Library), you indicate your acceptance of this License to do so, and
+all its terms and conditions for copying, distributing or modifying
+the Library or works based on it.
+
+  10. Each time you redistribute the Library (or any work based on the
+Library), the recipient automatically receives a license from the
+original licensor to copy, distribute, link with or modify the Library
+subject to these terms and conditions.  You may not impose any further
+restrictions on the recipients' exercise of the rights granted herein.
+You are not responsible for enforcing compliance by third parties with
+this License.
+
+  11. If, as a consequence of a court judgment or allegation of patent
+infringement or for any other reason (not limited to patent issues),
+conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot
+distribute so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you
+may not distribute the Library at all.  For example, if a patent
+license would not permit royalty-free redistribution of the Library by
+all those who receive copies directly or indirectly through you, then
+the only way you could satisfy both it and this License would be to
+refrain entirely from distribution of the Library.
+
+If any portion of this section is held invalid or unenforceable under any
+particular circumstance, the balance of the section is intended to apply,
+and the section as a whole is intended to apply in other circumstances.
+
+It is not the purpose of this section to induce you to infringe any
+patents or other property right claims or to contest validity of any
+such claims; this section has the sole purpose of protecting the
+integrity of the free software distribution system which is
+implemented by public license practices.  Many people have made
+generous contributions to the wide range of software distributed
+through that system in reliance on consistent application of that
+system; it is up to the author/donor to decide if he or she is willing
+to distribute software through any other system and a licensee cannot
+impose that choice.
+
+This section is intended to make thoroughly clear what is believed to
+be a consequence of the rest of this License.
+
+  12. If the distribution and/or use of the Library is restricted in
+certain countries either by patents or by copyrighted interfaces, the
+original copyright holder who places the Library under this License may add
+an explicit geographical distribution limitation excluding those countries,
+so that distribution is permitted only in or among countries not thus
+excluded.  In such case, this License incorporates the limitation as if
+written in the body of this License.
+
+  13. The Free Software Foundation may publish revised and/or new
+versions of the Lesser General Public License from time to time.
+Such new versions will be similar in spirit to the present version,
+but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number.  If the Library
+specifies a version number of this License which applies to it and
+"any later version", you have the option of following the terms and
+conditions either of that version or of any later version published by
+the Free Software Foundation.  If the Library does not specify a
+license version number, you may choose any version ever published by
+the Free Software Foundation.
+
+  14. If you wish to incorporate parts of the Library into other free
+programs whose distribution conditions are incompatible with these,
+write to the author to ask for permission.  For software which is
+copyrighted by the Free Software Foundation, write to the Free
+Software Foundation; we sometimes make exceptions for this.  Our
+decision will be guided by the two goals of preserving the free status
+of all derivatives of our free software and of promoting the sharing
+and reuse of software generally.
+
+                            NO WARRANTY
+
+  15. BECAUSE THE LIBRARY IS LICENSED FREE OF CHARGE, THERE IS NO
+WARRANTY FOR THE LIBRARY, TO THE EXTENT PERMITTED BY APPLICABLE LAW.
+EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR
+OTHER PARTIES PROVIDE THE LIBRARY "AS IS" WITHOUT WARRANTY OF ANY
+KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE
+LIBRARY IS WITH YOU.  SHOULD THE LIBRARY PROVE DEFECTIVE, YOU ASSUME
+THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN
+WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MAY MODIFY
+AND/OR REDISTRIBUTE THE LIBRARY AS PERMITTED ABOVE, BE LIABLE TO YOU
+FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR
+CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE
+LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
+RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
+FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
+SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
+DAMAGES.
+
+                     END OF TERMS AND CONDITIONS
+
+           How to Apply These Terms to Your New Libraries
+
+  If you develop a new library, and you want it to be of the greatest
+possible use to the public, we recommend making it free software that
+everyone can redistribute and change.  You can do so by permitting
+redistribution under these terms (or, alternatively, under the terms of the
+ordinary General Public License).
+
+  To apply these terms, attach the following notices to the library.  It is
+safest to attach them to the start of each source file to most effectively
+convey the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the library's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This library is free software; you can redistribute it and/or
+    modify it under the terms of the GNU Lesser General Public
+    License as published by the Free Software Foundation; either
+    version 2.1 of the License, or (at your option) any later version.
+
+    This library is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+    Lesser General Public License for more details.
+
+    You should have received a copy of the GNU Lesser General Public
+    License along with this library; if not, write to the Free Software
+    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+
+Also add information on how to contact you by electronic and paper mail.
+
+You should also get your employer (if you work as a programmer) or your
+school, if any, to sign a "copyright disclaimer" for the library, if
+necessary.  Here is a sample; alter the names:
+
+  Yoyodyne, Inc., hereby disclaims all copyright interest in the
+  library `Frob' (a library for tweaking knobs) written by James Random Hacker.
+
+  <signature of Ty Coon>, 1 April 1990
+  Ty Coon, President of Vice
+
+That's all there is to it!
```

### Comparing `libonvif-2.0.10/PKG-INFO` & `libonvif-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: libonvif
-Version: 2.0.10
+Version: 2.0.9
 Summary: A python module for communicating with onvif cameras
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Tracker, https://github.com/sr99622/libonvif/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libonvif
 
 Python enabled library for communicating with onvif devices.
 
@@ -27,19 +27,19 @@
 to install the dependencies.
 
 ```
 sudo apt install cmake libxml2-dev
 ```
 
 **Windows**, please use Anaconda.  The dependencies may
-be installed using the following command under a conda prompt. 
+be installed using the following command under a conda prompt.  The 
 Visual Studio C++ compiler must be installed as well.
 
 ```
-conda install cmake libxml2 -c conda-forge
+conda install cmake libxml2
 ```
 
 If successful, install libonvif python module
 
 ```
 pip install libonvif
 ```
```

### Comparing `libonvif-2.0.10/README.md` & `libonvif-2.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# libonvif
-
-Python enabled library for communicating with onvif devices.
-
-*Please Note*
-
-This python module has dependencies on development libraries which
-must be installed prior to installing.  This module is released as 
-a source distribution and is compiled on the host.
-
-**Debian or Ubuntu linux**, use the following command
-to install the dependencies.
-
-```
-sudo apt install cmake libxml2-dev
-```
-
-**Windows**, please use Anaconda.  The dependencies may
-be installed using the following command under a conda prompt. 
-Visual Studio C++ compiler must be installed as well.
-
-```
-conda install cmake libxml2 -c conda-forge
-```
-
-If successful, install libonvif python module
-
-```
-pip install libonvif
-```
-To uninstall
-```
-pip uninstall libonvif
-```
-
-Copyright (c) 2020, 2023 Stephen Rhodes 
-
- This library is free software; you can redistribute it and/or
- modify it under the terms of the GNU Lesser General Public
- License as published by the Free Software Foundation; either
- version 2.1 of the License, or (at your option) any later version.
-
- This library is distributed in the hope that it will be useful,
- but WITHOUT ANY WARRANTY; without even the implied warranty of
- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
- Lesser General Public License for more details.
-
- You should have received a copy of the GNU Lesser General Public
- License along with this library; if not, write to the Free Software
- Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+# libonvif
+
+Python enabled library for communicating with onvif devices.
+
+*Please Note*
+
+This python module has dependencies on development libraries which
+must be installed prior to installing.  This module is released as 
+a source distribution and is compiled on the host.
+
+**Debian or Ubuntu linux**, use the following command
+to install the dependencies.
+
+```
+sudo apt install cmake libxml2-dev
+```
+
+**Windows**, please use Anaconda.  The dependencies may
+be installed using the following command under a conda prompt.  The 
+Visual Studio C++ compiler must be installed as well.
+
+```
+conda install cmake libxml2
+```
+
+If successful, install libonvif python module
+
+```
+pip install libonvif
+```
+To uninstall
+```
+pip uninstall libonvif
+```
+
+Copyright (c) 2020, 2023 Stephen Rhodes 
+
+ This library is free software; you can redistribute it and/or
+ modify it under the terms of the GNU Lesser General Public
+ License as published by the Free Software Foundation; either
+ version 2.1 of the License, or (at your option) any later version.
+
+ This library is distributed in the hope that it will be useful,
+ but WITHOUT ANY WARRANTY; without even the implied warranty of
+ MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+ Lesser General Public License for more details.
+
+ You should have received a copy of the GNU Lesser General Public
+ License along with this library; if not, write to the Free Software
+ Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `libonvif-2.0.10/include/cencode.h` & `libonvif-2.0.9/include/cencode.h`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-/*
-cencode.h - c header for a base64 encoding algorithm
-
-This is part of the libb64 project, and has been placed in the public domain.
-For details, see http://sourceforge.net/projects/libb64
-
-The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
-hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
-is in the public domain of the country from which the work is published, or (b) hereby dedicates 
-whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
-the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
-associated work, and for these purposes, is described as a "dedicator" below.
-
-A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
-recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
-is not in the public domain.
-
-Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
-Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
-in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
-Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
-rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
-
-Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
-transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
-non-commercial, and in any way, including by methods that have not yet been invented or conceived.
-
-CC0 for Public Domain Dedication
-This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
-to the public domain, we recommend CC0.
-*/
-
-#ifndef BASE64_CENCODE_H
-#define BASE64_CENCODE_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-typedef enum
-{
-	step_A, step_B, step_C
-} base64_encodestep;
-
-typedef struct
-{
-	base64_encodestep step;
-	char result;
-	int stepcount;
-} base64_encodestate;
-
-void base64_init_encodestate(base64_encodestate* state_in);
-
-char base64_encode_value(char value_in);
-
-int base64_encode_block(const char* plaintext_in, int length_in, char* code_out, base64_encodestate* state_in);
-
-int base64_encode_blockend(char* code_out, base64_encodestate* state_in);
-
-#ifdef __cplusplus
-}
-#endif
-
-#endif /* BASE64_CENCODE_H */
+/*
+cencode.h - c header for a base64 encoding algorithm
+
+This is part of the libb64 project, and has been placed in the public domain.
+For details, see http://sourceforge.net/projects/libb64
+
+The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
+hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
+is in the public domain of the country from which the work is published, or (b) hereby dedicates 
+whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
+the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
+associated work, and for these purposes, is described as a "dedicator" below.
+
+A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
+recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
+is not in the public domain.
+
+Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
+Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
+in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
+Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
+rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
+
+Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
+transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
+non-commercial, and in any way, including by methods that have not yet been invented or conceived.
+
+CC0 for Public Domain Dedication
+This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
+to the public domain, we recommend CC0.
+*/
+
+#ifndef BASE64_CENCODE_H
+#define BASE64_CENCODE_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+typedef enum
+{
+	step_A, step_B, step_C
+} base64_encodestep;
+
+typedef struct
+{
+	base64_encodestep step;
+	char result;
+	int stepcount;
+} base64_encodestate;
+
+void base64_init_encodestate(base64_encodestate* state_in);
+
+char base64_encode_value(char value_in);
+
+int base64_encode_block(const char* plaintext_in, int length_in, char* code_out, base64_encodestate* state_in);
+
+int base64_encode_blockend(char* code_out, base64_encodestate* state_in);
+
+#ifdef __cplusplus
+}
+#endif
+
+#endif /* BASE64_CENCODE_H */
```

### Comparing `libonvif-2.0.10/include/getopt-win.h` & `libonvif-2.0.9/include/getopt-win.h`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,653 +1,653 @@
-/**
- * DISCLAIMER
- * This file is part of the mingw-w64 runtime package.
- *
- * The mingw-w64 runtime package and its code is distributed in the hope that it 
- * will be useful but WITHOUT ANY WARRANTY.  ALL WARRANTIES, EXPRESSED OR 
- * IMPLIED ARE HEREBY DISCLAIMED.  This includes but is not limited to 
- * warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
- */
- /*
- * Copyright (c) 2002 Todd C. Miller <Todd.Miller@courtesan.com>
- *
- * Permission to use, copy, modify, and distribute this software for any
- * purpose with or without fee is hereby granted, provided that the above
- * copyright notice and this permission notice appear in all copies.
- *
- * THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
- * WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
- * MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
- * ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
- * WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
- * ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
- * OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
- *
- * Sponsored in part by the Defense Advanced Research Projects
- * Agency (DARPA) and Air Force Research Laboratory, Air Force
- * Materiel Command, USAF, under agreement number F39502-99-1-0512.
- */
-/*-
- * Copyright (c) 2000 The NetBSD Foundation, Inc.
- * All rights reserved.
- *
- * This code is derived from software contributed to The NetBSD Foundation
- * by Dieter Baron and Thomas Klausner.
- *
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions
- * are met:
- * 1. Redistributions of source code must retain the above copyright
- *    notice, this list of conditions and the following disclaimer.
- * 2. Redistributions in binary form must reproduce the above copyright
- *    notice, this list of conditions and the following disclaimer in the
- *    documentation and/or other materials provided with the distribution.
- *
- * THIS SOFTWARE IS PROVIDED BY THE NETBSD FOUNDATION, INC. AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE FOUNDATION OR CONTRIBUTORS
- * BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
- * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
- * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
- * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
- * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
- * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
- * POSSIBILITY OF SUCH DAMAGE.
- */
-
-#ifndef __GETOPT_H__
-#define __GETOPT_H__
-
-#pragma warning(disable:4996)
-
-/* All the headers include this file. */
-#include <crtdefs.h>
-#include <errno.h>
-#include <stdlib.h>
-#include <string.h>
-#include <stdarg.h>
-#include <stdio.h>
-#include <windows.h>
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#define	REPLACE_GETOPT		/* use this getopt as the system getopt(3) */
-
-#ifdef REPLACE_GETOPT
-int	opterr = 1;		/* if error message should be printed */
-int	optind = 1;		/* index into parent argv vector */
-int	optopt = '?';		/* character checked for validity */
-#undef	optreset		/* see getopt.h */
-#define	optreset		__mingw_optreset
-int	optreset;		/* reset getopt */
-char    *optarg;		/* argument associated with option */
-#endif
-
-//extern int optind;		/* index of first non-option in argv      */
-//extern int optopt;		/* single option character, as parsed     */
-//extern int opterr;		/* flag to enable built-in diagnostics... */
-//				/* (user may set to zero, to suppress)    */
-//
-//extern char *optarg;		/* pointer to argument of current option  */
-
-#define PRINT_ERROR	((opterr) && (*options != ':'))
-
-#define FLAG_PERMUTE	0x01	/* permute non-options to the end of argv */
-#define FLAG_ALLARGS	0x02	/* treat non-options as args to option "-1" */
-#define FLAG_LONGONLY	0x04	/* operate as getopt_long_only */
-
-/* return values */
-#define	BADCH		(int)'?'
-#define	BADARG		((*options == ':') ? (int)':' : (int)'?')
-#define	INORDER 	(int)1
-
-#ifndef __CYGWIN__
-#define __progname __argv[0]
-#else
-extern char __declspec(dllimport) *__progname;
-#endif
-
-#ifdef __CYGWIN__
-static char EMSG[] = "";
-#else
-#define	EMSG		""
-#endif
-
-static int getopt_internal(int, char * const *, const char *,
-			   const struct option *, int *, int);
-static int parse_long_options(char * const *, const char *,
-			      const struct option *, int *, int);
-static int gcd(int, int);
-static void permute_args(int, int, int, char * const *);
-
-static char *place = EMSG; /* option letter processing */
-
-/* XXX: set optreset to 1 rather than these two */
-static int nonopt_start = -1; /* first non option argument (for permute) */
-static int nonopt_end = -1;   /* first option after non options (for permute) */
-
-/* Error messages */
-static const char recargchar[] = "option requires an argument -- %c";
-static const char recargstring[] = "option requires an argument -- %s";
-static const char ambig[] = "ambiguous option -- %.*s";
-static const char noarg[] = "option doesn't take an argument -- %.*s";
-static const char illoptchar[] = "unknown option -- %c";
-static const char illoptstring[] = "unknown option -- %s";
-
-static void
-_vwarnx(const char *fmt,va_list ap)
-{
-  (void)fprintf(stderr,"%s: ",__progname);
-  if (fmt != NULL)
-    (void)vfprintf(stderr,fmt,ap);
-  (void)fprintf(stderr,"\n");
-}
-
-static void
-warnx(const char *fmt,...)
-{
-  va_list ap;
-  va_start(ap,fmt);
-  _vwarnx(fmt,ap);
-  va_end(ap);
-}
-
-/*
- * Compute the greatest common divisor of a and b.
- */
-static int
-gcd(int a, int b)
-{
-	int c;
-
-	c = a % b;
-	while (c != 0) {
-		a = b;
-		b = c;
-		c = a % b;
-	}
-
-	return (b);
-}
-
-/*
- * Exchange the block from nonopt_start to nonopt_end with the block
- * from nonopt_end to opt_end (keeping the same order of arguments
- * in each block).
- */
-static void
-permute_args(int panonopt_start, int panonopt_end, int opt_end,
-	char * const *nargv)
-{
-	int cstart, cyclelen, i, j, ncycle, nnonopts, nopts, pos;
-	char *swap;
-
-	/*
-	 * compute lengths of blocks and number and size of cycles
-	 */
-	nnonopts = panonopt_end - panonopt_start;
-	nopts = opt_end - panonopt_end;
-	ncycle = gcd(nnonopts, nopts);
-	cyclelen = (opt_end - panonopt_start) / ncycle;
-
-	for (i = 0; i < ncycle; i++) {
-		cstart = panonopt_end+i;
-		pos = cstart;
-		for (j = 0; j < cyclelen; j++) {
-			if (pos >= panonopt_end)
-				pos -= nnonopts;
-			else
-				pos += nopts;
-			swap = nargv[pos];
-			/* LINTED const cast */
-			((char **) nargv)[pos] = nargv[cstart];
-			/* LINTED const cast */
-			((char **)nargv)[cstart] = swap;
-		}
-	}
-}
-
-#ifdef REPLACE_GETOPT
-/*
- * getopt --
- *	Parse argc/argv argument vector.
- *
- * [eventually this will replace the BSD getopt]
- */
-int
-getopt(int nargc, char * const *nargv, const char *options)
-{
-
-	/*
-	 * We don't pass FLAG_PERMUTE to getopt_internal() since
-	 * the BSD getopt(3) (unlike GNU) has never done this.
-	 *
-	 * Furthermore, since many privileged programs call getopt()
-	 * before dropping privileges it makes sense to keep things
-	 * as simple (and bug-free) as possible.
-	 */
-	return (getopt_internal(nargc, nargv, options, NULL, NULL, 0));
-}
-#endif /* REPLACE_GETOPT */
-
-//extern int getopt(int nargc, char * const *nargv, const char *options);
-
-#ifdef _BSD_SOURCE
-/*
- * BSD adds the non-standard `optreset' feature, for reinitialisation
- * of `getopt' parsing.  We support this feature, for applications which
- * proclaim their BSD heritage, before including this header; however,
- * to maintain portability, developers are advised to avoid it.
- */
-# define optreset  __mingw_optreset
-extern int optreset;
-#endif
-#ifdef __cplusplus
-}
-#endif
-/*
- * POSIX requires the `getopt' API to be specified in `unistd.h';
- * thus, `unistd.h' includes this header.  However, we do not want
- * to expose the `getopt_long' or `getopt_long_only' APIs, when
- * included in this manner.  Thus, close the standard __GETOPT_H__
- * declarations block, and open an additional __GETOPT_LONG_H__
- * specific block, only when *not* __UNISTD_H_SOURCED__, in which
- * to declare the extended API.
- */
-#endif /* !defined(__GETOPT_H__) */
-
-#if !defined(__UNISTD_H_SOURCED__) && !defined(__GETOPT_LONG_H__)
-#define __GETOPT_LONG_H__
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-struct option		/* specification for a long form option...	*/
-{
-  const char *name;		/* option name, without leading hyphens */
-  int         has_arg;		/* does it take an argument?		*/
-  int        *flag;		/* where to save its status, or NULL	*/
-  int         val;		/* its associated status value		*/
-};
-
-enum    		/* permitted values for its `has_arg' field...	*/
-{
-  no_argument = 0,      	/* option never takes an argument	*/
-  required_argument,		/* option always requires an argument	*/
-  optional_argument		/* option may take an argument		*/
-};
-
-/*
- * parse_long_options --
- *	Parse long options in argc/argv argument vector.
- * Returns -1 if short_too is set and the option does not match long_options.
- */
-static int
-parse_long_options(char * const *nargv, const char *options,
-	const struct option *long_options, int *idx, int short_too)
-{
-	char *current_argv, *has_equal;
-	size_t current_argv_len;
-	int i, ambiguous, match;
-
-#define IDENTICAL_INTERPRETATION(_x, _y)                                \
-	(long_options[(_x)].has_arg == long_options[(_y)].has_arg &&    \
-	 long_options[(_x)].flag == long_options[(_y)].flag &&          \
-	 long_options[(_x)].val == long_options[(_y)].val)
-
-	current_argv = place;
-	match = -1;
-	ambiguous = 0;
-
-	optind++;
-
-	if ((has_equal = strchr(current_argv, '=')) != NULL) {
-		/* argument found (--option=arg) */
-		current_argv_len = has_equal - current_argv;
-		has_equal++;
-	} else
-		current_argv_len = strlen(current_argv);
-
-	for (i = 0; long_options[i].name; i++) {
-		/* find matching long option */
-		if (strncmp(current_argv, long_options[i].name,
-		    current_argv_len))
-			continue;
-
-		if (strlen(long_options[i].name) == current_argv_len) {
-			/* exact match */
-			match = i;
-			ambiguous = 0;
-			break;
-		}
-		/*
-		 * If this is a known short option, don't allow
-		 * a partial match of a single character.
-		 */
-		if (short_too && current_argv_len == 1)
-			continue;
-
-		if (match == -1)	/* partial match */
-			match = i;
-		else if (!IDENTICAL_INTERPRETATION(i, match))
-			ambiguous = 1;
-	}
-	if (ambiguous) {
-		/* ambiguous abbreviation */
-		if (PRINT_ERROR)
-			warnx(ambig, (int)current_argv_len,
-			     current_argv);
-		optopt = 0;
-		return (BADCH);
-	}
-	if (match != -1) {		/* option found */
-		if (long_options[match].has_arg == no_argument
-		    && has_equal) {
-			if (PRINT_ERROR)
-				warnx(noarg, (int)current_argv_len,
-				     current_argv);
-			/*
-			 * XXX: GNU sets optopt to val regardless of flag
-			 */
-			if (long_options[match].flag == NULL)
-				optopt = long_options[match].val;
-			else
-				optopt = 0;
-			return (BADARG);
-		}
-		if (long_options[match].has_arg == required_argument ||
-		    long_options[match].has_arg == optional_argument) {
-			if (has_equal)
-				optarg = has_equal;
-			else if (long_options[match].has_arg ==
-			    required_argument) {
-				/*
-				 * optional argument doesn't use next nargv
-				 */
-				optarg = nargv[optind++];
-			}
-		}
-		if ((long_options[match].has_arg == required_argument)
-		    && (optarg == NULL)) {
-			/*
-			 * Missing argument; leading ':' indicates no error
-			 * should be generated.
-			 */
-			if (PRINT_ERROR)
-				warnx(recargstring,
-				    current_argv);
-			/*
-			 * XXX: GNU sets optopt to val regardless of flag
-			 */
-			if (long_options[match].flag == NULL)
-				optopt = long_options[match].val;
-			else
-				optopt = 0;
-			--optind;
-			return (BADARG);
-		}
-	} else {			/* unknown option */
-		if (short_too) {
-			--optind;
-			return (-1);
-		}
-		if (PRINT_ERROR)
-			warnx(illoptstring, current_argv);
-		optopt = 0;
-		return (BADCH);
-	}
-	if (idx)
-		*idx = match;
-	if (long_options[match].flag) {
-		*long_options[match].flag = long_options[match].val;
-		return (0);
-	} else
-		return (long_options[match].val);
-#undef IDENTICAL_INTERPRETATION
-}
-
-/*
- * getopt_internal --
- *	Parse argc/argv argument vector.  Called by user level routines.
- */
-static int
-getopt_internal(int nargc, char * const *nargv, const char *options,
-	const struct option *long_options, int *idx, int flags)
-{
-	char *oli;				/* option letter list index */
-	int optchar, short_too;
-	static int posixly_correct = -1;
-
-	if (options == NULL)
-		return (-1);
-
-	/*
-	 * XXX Some GNU programs (like cvs) set optind to 0 instead of
-	 * XXX using optreset.  Work around this braindamage.
-	 */
-	if (optind == 0)
-		optind = optreset = 1;
-
-	/*
-	 * Disable GNU extensions if POSIXLY_CORRECT is set or options
-	 * string begins with a '+'.
-	 *
-	 * CV, 2009-12-14: Check POSIXLY_CORRECT anew if optind == 0 or
-	 *                 optreset != 0 for GNU compatibility.
-	 */
-	if (posixly_correct == -1 || optreset != 0)
-		posixly_correct = (getenv("POSIXLY_CORRECT") != NULL);
-	if (*options == '-')
-		flags |= FLAG_ALLARGS;
-	else if (posixly_correct || *options == '+')
-		flags &= ~FLAG_PERMUTE;
-	if (*options == '+' || *options == '-')
-		options++;
-
-	optarg = NULL;
-	if (optreset)
-		nonopt_start = nonopt_end = -1;
-start:
-	if (optreset || !*place) {		/* update scanning pointer */
-		optreset = 0;
-		if (optind >= nargc) {          /* end of argument vector */
-			place = EMSG;
-			if (nonopt_end != -1) {
-				/* do permutation, if we have to */
-				permute_args(nonopt_start, nonopt_end,
-				    optind, nargv);
-				optind -= nonopt_end - nonopt_start;
-			}
-			else if (nonopt_start != -1) {
-				/*
-				 * If we skipped non-options, set optind
-				 * to the first of them.
-				 */
-				optind = nonopt_start;
-			}
-			nonopt_start = nonopt_end = -1;
-			return (-1);
-		}
-		if (*(place = nargv[optind]) != '-' ||
-		    (place[1] == '\0' && strchr(options, '-') == NULL)) {
-			place = EMSG;		/* found non-option */
-			if (flags & FLAG_ALLARGS) {
-				/*
-				 * GNU extension:
-				 * return non-option as argument to option 1
-				 */
-				optarg = nargv[optind++];
-				return (INORDER);
-			}
-			if (!(flags & FLAG_PERMUTE)) {
-				/*
-				 * If no permutation wanted, stop parsing
-				 * at first non-option.
-				 */
-				return (-1);
-			}
-			/* do permutation */
-			if (nonopt_start == -1)
-				nonopt_start = optind;
-			else if (nonopt_end != -1) {
-				permute_args(nonopt_start, nonopt_end,
-				    optind, nargv);
-				nonopt_start = optind -
-				    (nonopt_end - nonopt_start);
-				nonopt_end = -1;
-			}
-			optind++;
-			/* process next argument */
-			goto start;
-		}
-		if (nonopt_start != -1 && nonopt_end == -1)
-			nonopt_end = optind;
-
-		/*
-		 * If we have "-" do nothing, if "--" we are done.
-		 */
-		if (place[1] != '\0' && *++place == '-' && place[1] == '\0') {
-			optind++;
-			place = EMSG;
-			/*
-			 * We found an option (--), so if we skipped
-			 * non-options, we have to permute.
-			 */
-			if (nonopt_end != -1) {
-				permute_args(nonopt_start, nonopt_end,
-				    optind, nargv);
-				optind -= nonopt_end - nonopt_start;
-			}
-			nonopt_start = nonopt_end = -1;
-			return (-1);
-		}
-	}
-
-	/*
-	 * Check long options if:
-	 *  1) we were passed some
-	 *  2) the arg is not just "-"
-	 *  3) either the arg starts with -- we are getopt_long_only()
-	 */
-	if (long_options != NULL && place != nargv[optind] &&
-	    (*place == '-' || (flags & FLAG_LONGONLY))) {
-		short_too = 0;
-		if (*place == '-')
-			place++;		/* --foo long option */
-		else if (*place != ':' && strchr(options, *place) != NULL)
-			short_too = 1;		/* could be short option too */
-
-		optchar = parse_long_options(nargv, options, long_options,
-		    idx, short_too);
-		if (optchar != -1) {
-			place = EMSG;
-			return (optchar);
-		}
-	}
-
-	if ((optchar = (int)*place++) == (int)':' ||
-	    (optchar == (int)'-' && *place != '\0') ||
-	    (oli = (char*)strchr(options, optchar)) == NULL) {
-		/*
-		 * If the user specified "-" and  '-' isn't listed in
-		 * options, return -1 (non-option) as per POSIX.
-		 * Otherwise, it is an unknown option character (or ':').
-		 */
-		if (optchar == (int)'-' && *place == '\0')
-			return (-1);
-		if (!*place)
-			++optind;
-		if (PRINT_ERROR)
-			warnx(illoptchar, optchar);
-		optopt = optchar;
-		return (BADCH);
-	}
-	if (long_options != NULL && optchar == 'W' && oli[1] == ';') {
-		/* -W long-option */
-		if (*place)			/* no space */
-			/* NOTHING */;
-		else if (++optind >= nargc) {	/* no arg */
-			place = EMSG;
-			if (PRINT_ERROR)
-				warnx(recargchar, optchar);
-			optopt = optchar;
-			return (BADARG);
-		} else				/* white space */
-			place = nargv[optind];
-		optchar = parse_long_options(nargv, options, long_options,
-		    idx, 0);
-		place = EMSG;
-		return (optchar);
-	}
-	if (*++oli != ':') {			/* doesn't take argument */
-		if (!*place)
-			++optind;
-	} else {				/* takes (optional) argument */
-		optarg = NULL;
-		if (*place)			/* no white space */
-			optarg = place;
-		else if (oli[1] != ':') {	/* arg not optional */
-			if (++optind >= nargc) {	/* no arg */
-				place = EMSG;
-				if (PRINT_ERROR)
-					warnx(recargchar, optchar);
-				optopt = optchar;
-				return (BADARG);
-			} else
-				optarg = nargv[optind];
-		}
-		place = EMSG;
-		++optind;
-	}
-	/* dump back option letter */
-	return (optchar);
-}
-
-/*
- * getopt_long --
- *	Parse argc/argv argument vector.
- */
-int
-getopt_long(int nargc, char * const *nargv, const char *options,
-    const struct option *long_options, int *idx)
-{
-
-	return (getopt_internal(nargc, nargv, options, long_options, idx,
-	    FLAG_PERMUTE));
-}
-
-/*
- * getopt_long_only --
- *	Parse argc/argv argument vector.
- */
-int
-getopt_long_only(int nargc, char * const *nargv, const char *options,
-    const struct option *long_options, int *idx)
-{
-
-	return (getopt_internal(nargc, nargv, options, long_options, idx,
-	    FLAG_PERMUTE|FLAG_LONGONLY));
-}
-
-//extern int getopt_long(int nargc, char * const *nargv, const char *options,
-//    const struct option *long_options, int *idx);
-//extern int getopt_long_only(int nargc, char * const *nargv, const char *options,
-//    const struct option *long_options, int *idx);
-/*
- * Previous MinGW implementation had...
- */
-#ifndef HAVE_DECL_GETOPT
-/*
- * ...for the long form API only; keep this for compatibility.
- */
-# define HAVE_DECL_GETOPT	1
-#endif
-
-#ifdef __cplusplus
-}
-#endif
-
+/**
+ * DISCLAIMER
+ * This file is part of the mingw-w64 runtime package.
+ *
+ * The mingw-w64 runtime package and its code is distributed in the hope that it 
+ * will be useful but WITHOUT ANY WARRANTY.  ALL WARRANTIES, EXPRESSED OR 
+ * IMPLIED ARE HEREBY DISCLAIMED.  This includes but is not limited to 
+ * warranties of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+ */
+ /*
+ * Copyright (c) 2002 Todd C. Miller <Todd.Miller@courtesan.com>
+ *
+ * Permission to use, copy, modify, and distribute this software for any
+ * purpose with or without fee is hereby granted, provided that the above
+ * copyright notice and this permission notice appear in all copies.
+ *
+ * THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
+ * WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
+ * MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
+ * ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+ * WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+ * ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
+ * OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+ *
+ * Sponsored in part by the Defense Advanced Research Projects
+ * Agency (DARPA) and Air Force Research Laboratory, Air Force
+ * Materiel Command, USAF, under agreement number F39502-99-1-0512.
+ */
+/*-
+ * Copyright (c) 2000 The NetBSD Foundation, Inc.
+ * All rights reserved.
+ *
+ * This code is derived from software contributed to The NetBSD Foundation
+ * by Dieter Baron and Thomas Klausner.
+ *
+ * Redistribution and use in source and binary forms, with or without
+ * modification, are permitted provided that the following conditions
+ * are met:
+ * 1. Redistributions of source code must retain the above copyright
+ *    notice, this list of conditions and the following disclaimer.
+ * 2. Redistributions in binary form must reproduce the above copyright
+ *    notice, this list of conditions and the following disclaimer in the
+ *    documentation and/or other materials provided with the distribution.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE NETBSD FOUNDATION, INC. AND CONTRIBUTORS
+ * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
+ * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+ * PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE FOUNDATION OR CONTRIBUTORS
+ * BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
+ */
+
+#ifndef __GETOPT_H__
+#define __GETOPT_H__
+
+#pragma warning(disable:4996)
+
+/* All the headers include this file. */
+#include <crtdefs.h>
+#include <errno.h>
+#include <stdlib.h>
+#include <string.h>
+#include <stdarg.h>
+#include <stdio.h>
+#include <windows.h>
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#define	REPLACE_GETOPT		/* use this getopt as the system getopt(3) */
+
+#ifdef REPLACE_GETOPT
+int	opterr = 1;		/* if error message should be printed */
+int	optind = 1;		/* index into parent argv vector */
+int	optopt = '?';		/* character checked for validity */
+#undef	optreset		/* see getopt.h */
+#define	optreset		__mingw_optreset
+int	optreset;		/* reset getopt */
+char    *optarg;		/* argument associated with option */
+#endif
+
+//extern int optind;		/* index of first non-option in argv      */
+//extern int optopt;		/* single option character, as parsed     */
+//extern int opterr;		/* flag to enable built-in diagnostics... */
+//				/* (user may set to zero, to suppress)    */
+//
+//extern char *optarg;		/* pointer to argument of current option  */
+
+#define PRINT_ERROR	((opterr) && (*options != ':'))
+
+#define FLAG_PERMUTE	0x01	/* permute non-options to the end of argv */
+#define FLAG_ALLARGS	0x02	/* treat non-options as args to option "-1" */
+#define FLAG_LONGONLY	0x04	/* operate as getopt_long_only */
+
+/* return values */
+#define	BADCH		(int)'?'
+#define	BADARG		((*options == ':') ? (int)':' : (int)'?')
+#define	INORDER 	(int)1
+
+#ifndef __CYGWIN__
+#define __progname __argv[0]
+#else
+extern char __declspec(dllimport) *__progname;
+#endif
+
+#ifdef __CYGWIN__
+static char EMSG[] = "";
+#else
+#define	EMSG		""
+#endif
+
+static int getopt_internal(int, char * const *, const char *,
+			   const struct option *, int *, int);
+static int parse_long_options(char * const *, const char *,
+			      const struct option *, int *, int);
+static int gcd(int, int);
+static void permute_args(int, int, int, char * const *);
+
+static char *place = EMSG; /* option letter processing */
+
+/* XXX: set optreset to 1 rather than these two */
+static int nonopt_start = -1; /* first non option argument (for permute) */
+static int nonopt_end = -1;   /* first option after non options (for permute) */
+
+/* Error messages */
+static const char recargchar[] = "option requires an argument -- %c";
+static const char recargstring[] = "option requires an argument -- %s";
+static const char ambig[] = "ambiguous option -- %.*s";
+static const char noarg[] = "option doesn't take an argument -- %.*s";
+static const char illoptchar[] = "unknown option -- %c";
+static const char illoptstring[] = "unknown option -- %s";
+
+static void
+_vwarnx(const char *fmt,va_list ap)
+{
+  (void)fprintf(stderr,"%s: ",__progname);
+  if (fmt != NULL)
+    (void)vfprintf(stderr,fmt,ap);
+  (void)fprintf(stderr,"\n");
+}
+
+static void
+warnx(const char *fmt,...)
+{
+  va_list ap;
+  va_start(ap,fmt);
+  _vwarnx(fmt,ap);
+  va_end(ap);
+}
+
+/*
+ * Compute the greatest common divisor of a and b.
+ */
+static int
+gcd(int a, int b)
+{
+	int c;
+
+	c = a % b;
+	while (c != 0) {
+		a = b;
+		b = c;
+		c = a % b;
+	}
+
+	return (b);
+}
+
+/*
+ * Exchange the block from nonopt_start to nonopt_end with the block
+ * from nonopt_end to opt_end (keeping the same order of arguments
+ * in each block).
+ */
+static void
+permute_args(int panonopt_start, int panonopt_end, int opt_end,
+	char * const *nargv)
+{
+	int cstart, cyclelen, i, j, ncycle, nnonopts, nopts, pos;
+	char *swap;
+
+	/*
+	 * compute lengths of blocks and number and size of cycles
+	 */
+	nnonopts = panonopt_end - panonopt_start;
+	nopts = opt_end - panonopt_end;
+	ncycle = gcd(nnonopts, nopts);
+	cyclelen = (opt_end - panonopt_start) / ncycle;
+
+	for (i = 0; i < ncycle; i++) {
+		cstart = panonopt_end+i;
+		pos = cstart;
+		for (j = 0; j < cyclelen; j++) {
+			if (pos >= panonopt_end)
+				pos -= nnonopts;
+			else
+				pos += nopts;
+			swap = nargv[pos];
+			/* LINTED const cast */
+			((char **) nargv)[pos] = nargv[cstart];
+			/* LINTED const cast */
+			((char **)nargv)[cstart] = swap;
+		}
+	}
+}
+
+#ifdef REPLACE_GETOPT
+/*
+ * getopt --
+ *	Parse argc/argv argument vector.
+ *
+ * [eventually this will replace the BSD getopt]
+ */
+int
+getopt(int nargc, char * const *nargv, const char *options)
+{
+
+	/*
+	 * We don't pass FLAG_PERMUTE to getopt_internal() since
+	 * the BSD getopt(3) (unlike GNU) has never done this.
+	 *
+	 * Furthermore, since many privileged programs call getopt()
+	 * before dropping privileges it makes sense to keep things
+	 * as simple (and bug-free) as possible.
+	 */
+	return (getopt_internal(nargc, nargv, options, NULL, NULL, 0));
+}
+#endif /* REPLACE_GETOPT */
+
+//extern int getopt(int nargc, char * const *nargv, const char *options);
+
+#ifdef _BSD_SOURCE
+/*
+ * BSD adds the non-standard `optreset' feature, for reinitialisation
+ * of `getopt' parsing.  We support this feature, for applications which
+ * proclaim their BSD heritage, before including this header; however,
+ * to maintain portability, developers are advised to avoid it.
+ */
+# define optreset  __mingw_optreset
+extern int optreset;
+#endif
+#ifdef __cplusplus
+}
+#endif
+/*
+ * POSIX requires the `getopt' API to be specified in `unistd.h';
+ * thus, `unistd.h' includes this header.  However, we do not want
+ * to expose the `getopt_long' or `getopt_long_only' APIs, when
+ * included in this manner.  Thus, close the standard __GETOPT_H__
+ * declarations block, and open an additional __GETOPT_LONG_H__
+ * specific block, only when *not* __UNISTD_H_SOURCED__, in which
+ * to declare the extended API.
+ */
+#endif /* !defined(__GETOPT_H__) */
+
+#if !defined(__UNISTD_H_SOURCED__) && !defined(__GETOPT_LONG_H__)
+#define __GETOPT_LONG_H__
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+struct option		/* specification for a long form option...	*/
+{
+  const char *name;		/* option name, without leading hyphens */
+  int         has_arg;		/* does it take an argument?		*/
+  int        *flag;		/* where to save its status, or NULL	*/
+  int         val;		/* its associated status value		*/
+};
+
+enum    		/* permitted values for its `has_arg' field...	*/
+{
+  no_argument = 0,      	/* option never takes an argument	*/
+  required_argument,		/* option always requires an argument	*/
+  optional_argument		/* option may take an argument		*/
+};
+
+/*
+ * parse_long_options --
+ *	Parse long options in argc/argv argument vector.
+ * Returns -1 if short_too is set and the option does not match long_options.
+ */
+static int
+parse_long_options(char * const *nargv, const char *options,
+	const struct option *long_options, int *idx, int short_too)
+{
+	char *current_argv, *has_equal;
+	size_t current_argv_len;
+	int i, ambiguous, match;
+
+#define IDENTICAL_INTERPRETATION(_x, _y)                                \
+	(long_options[(_x)].has_arg == long_options[(_y)].has_arg &&    \
+	 long_options[(_x)].flag == long_options[(_y)].flag &&          \
+	 long_options[(_x)].val == long_options[(_y)].val)
+
+	current_argv = place;
+	match = -1;
+	ambiguous = 0;
+
+	optind++;
+
+	if ((has_equal = strchr(current_argv, '=')) != NULL) {
+		/* argument found (--option=arg) */
+		current_argv_len = has_equal - current_argv;
+		has_equal++;
+	} else
+		current_argv_len = strlen(current_argv);
+
+	for (i = 0; long_options[i].name; i++) {
+		/* find matching long option */
+		if (strncmp(current_argv, long_options[i].name,
+		    current_argv_len))
+			continue;
+
+		if (strlen(long_options[i].name) == current_argv_len) {
+			/* exact match */
+			match = i;
+			ambiguous = 0;
+			break;
+		}
+		/*
+		 * If this is a known short option, don't allow
+		 * a partial match of a single character.
+		 */
+		if (short_too && current_argv_len == 1)
+			continue;
+
+		if (match == -1)	/* partial match */
+			match = i;
+		else if (!IDENTICAL_INTERPRETATION(i, match))
+			ambiguous = 1;
+	}
+	if (ambiguous) {
+		/* ambiguous abbreviation */
+		if (PRINT_ERROR)
+			warnx(ambig, (int)current_argv_len,
+			     current_argv);
+		optopt = 0;
+		return (BADCH);
+	}
+	if (match != -1) {		/* option found */
+		if (long_options[match].has_arg == no_argument
+		    && has_equal) {
+			if (PRINT_ERROR)
+				warnx(noarg, (int)current_argv_len,
+				     current_argv);
+			/*
+			 * XXX: GNU sets optopt to val regardless of flag
+			 */
+			if (long_options[match].flag == NULL)
+				optopt = long_options[match].val;
+			else
+				optopt = 0;
+			return (BADARG);
+		}
+		if (long_options[match].has_arg == required_argument ||
+		    long_options[match].has_arg == optional_argument) {
+			if (has_equal)
+				optarg = has_equal;
+			else if (long_options[match].has_arg ==
+			    required_argument) {
+				/*
+				 * optional argument doesn't use next nargv
+				 */
+				optarg = nargv[optind++];
+			}
+		}
+		if ((long_options[match].has_arg == required_argument)
+		    && (optarg == NULL)) {
+			/*
+			 * Missing argument; leading ':' indicates no error
+			 * should be generated.
+			 */
+			if (PRINT_ERROR)
+				warnx(recargstring,
+				    current_argv);
+			/*
+			 * XXX: GNU sets optopt to val regardless of flag
+			 */
+			if (long_options[match].flag == NULL)
+				optopt = long_options[match].val;
+			else
+				optopt = 0;
+			--optind;
+			return (BADARG);
+		}
+	} else {			/* unknown option */
+		if (short_too) {
+			--optind;
+			return (-1);
+		}
+		if (PRINT_ERROR)
+			warnx(illoptstring, current_argv);
+		optopt = 0;
+		return (BADCH);
+	}
+	if (idx)
+		*idx = match;
+	if (long_options[match].flag) {
+		*long_options[match].flag = long_options[match].val;
+		return (0);
+	} else
+		return (long_options[match].val);
+#undef IDENTICAL_INTERPRETATION
+}
+
+/*
+ * getopt_internal --
+ *	Parse argc/argv argument vector.  Called by user level routines.
+ */
+static int
+getopt_internal(int nargc, char * const *nargv, const char *options,
+	const struct option *long_options, int *idx, int flags)
+{
+	char *oli;				/* option letter list index */
+	int optchar, short_too;
+	static int posixly_correct = -1;
+
+	if (options == NULL)
+		return (-1);
+
+	/*
+	 * XXX Some GNU programs (like cvs) set optind to 0 instead of
+	 * XXX using optreset.  Work around this braindamage.
+	 */
+	if (optind == 0)
+		optind = optreset = 1;
+
+	/*
+	 * Disable GNU extensions if POSIXLY_CORRECT is set or options
+	 * string begins with a '+'.
+	 *
+	 * CV, 2009-12-14: Check POSIXLY_CORRECT anew if optind == 0 or
+	 *                 optreset != 0 for GNU compatibility.
+	 */
+	if (posixly_correct == -1 || optreset != 0)
+		posixly_correct = (getenv("POSIXLY_CORRECT") != NULL);
+	if (*options == '-')
+		flags |= FLAG_ALLARGS;
+	else if (posixly_correct || *options == '+')
+		flags &= ~FLAG_PERMUTE;
+	if (*options == '+' || *options == '-')
+		options++;
+
+	optarg = NULL;
+	if (optreset)
+		nonopt_start = nonopt_end = -1;
+start:
+	if (optreset || !*place) {		/* update scanning pointer */
+		optreset = 0;
+		if (optind >= nargc) {          /* end of argument vector */
+			place = EMSG;
+			if (nonopt_end != -1) {
+				/* do permutation, if we have to */
+				permute_args(nonopt_start, nonopt_end,
+				    optind, nargv);
+				optind -= nonopt_end - nonopt_start;
+			}
+			else if (nonopt_start != -1) {
+				/*
+				 * If we skipped non-options, set optind
+				 * to the first of them.
+				 */
+				optind = nonopt_start;
+			}
+			nonopt_start = nonopt_end = -1;
+			return (-1);
+		}
+		if (*(place = nargv[optind]) != '-' ||
+		    (place[1] == '\0' && strchr(options, '-') == NULL)) {
+			place = EMSG;		/* found non-option */
+			if (flags & FLAG_ALLARGS) {
+				/*
+				 * GNU extension:
+				 * return non-option as argument to option 1
+				 */
+				optarg = nargv[optind++];
+				return (INORDER);
+			}
+			if (!(flags & FLAG_PERMUTE)) {
+				/*
+				 * If no permutation wanted, stop parsing
+				 * at first non-option.
+				 */
+				return (-1);
+			}
+			/* do permutation */
+			if (nonopt_start == -1)
+				nonopt_start = optind;
+			else if (nonopt_end != -1) {
+				permute_args(nonopt_start, nonopt_end,
+				    optind, nargv);
+				nonopt_start = optind -
+				    (nonopt_end - nonopt_start);
+				nonopt_end = -1;
+			}
+			optind++;
+			/* process next argument */
+			goto start;
+		}
+		if (nonopt_start != -1 && nonopt_end == -1)
+			nonopt_end = optind;
+
+		/*
+		 * If we have "-" do nothing, if "--" we are done.
+		 */
+		if (place[1] != '\0' && *++place == '-' && place[1] == '\0') {
+			optind++;
+			place = EMSG;
+			/*
+			 * We found an option (--), so if we skipped
+			 * non-options, we have to permute.
+			 */
+			if (nonopt_end != -1) {
+				permute_args(nonopt_start, nonopt_end,
+				    optind, nargv);
+				optind -= nonopt_end - nonopt_start;
+			}
+			nonopt_start = nonopt_end = -1;
+			return (-1);
+		}
+	}
+
+	/*
+	 * Check long options if:
+	 *  1) we were passed some
+	 *  2) the arg is not just "-"
+	 *  3) either the arg starts with -- we are getopt_long_only()
+	 */
+	if (long_options != NULL && place != nargv[optind] &&
+	    (*place == '-' || (flags & FLAG_LONGONLY))) {
+		short_too = 0;
+		if (*place == '-')
+			place++;		/* --foo long option */
+		else if (*place != ':' && strchr(options, *place) != NULL)
+			short_too = 1;		/* could be short option too */
+
+		optchar = parse_long_options(nargv, options, long_options,
+		    idx, short_too);
+		if (optchar != -1) {
+			place = EMSG;
+			return (optchar);
+		}
+	}
+
+	if ((optchar = (int)*place++) == (int)':' ||
+	    (optchar == (int)'-' && *place != '\0') ||
+	    (oli = (char*)strchr(options, optchar)) == NULL) {
+		/*
+		 * If the user specified "-" and  '-' isn't listed in
+		 * options, return -1 (non-option) as per POSIX.
+		 * Otherwise, it is an unknown option character (or ':').
+		 */
+		if (optchar == (int)'-' && *place == '\0')
+			return (-1);
+		if (!*place)
+			++optind;
+		if (PRINT_ERROR)
+			warnx(illoptchar, optchar);
+		optopt = optchar;
+		return (BADCH);
+	}
+	if (long_options != NULL && optchar == 'W' && oli[1] == ';') {
+		/* -W long-option */
+		if (*place)			/* no space */
+			/* NOTHING */;
+		else if (++optind >= nargc) {	/* no arg */
+			place = EMSG;
+			if (PRINT_ERROR)
+				warnx(recargchar, optchar);
+			optopt = optchar;
+			return (BADARG);
+		} else				/* white space */
+			place = nargv[optind];
+		optchar = parse_long_options(nargv, options, long_options,
+		    idx, 0);
+		place = EMSG;
+		return (optchar);
+	}
+	if (*++oli != ':') {			/* doesn't take argument */
+		if (!*place)
+			++optind;
+	} else {				/* takes (optional) argument */
+		optarg = NULL;
+		if (*place)			/* no white space */
+			optarg = place;
+		else if (oli[1] != ':') {	/* arg not optional */
+			if (++optind >= nargc) {	/* no arg */
+				place = EMSG;
+				if (PRINT_ERROR)
+					warnx(recargchar, optchar);
+				optopt = optchar;
+				return (BADARG);
+			} else
+				optarg = nargv[optind];
+		}
+		place = EMSG;
+		++optind;
+	}
+	/* dump back option letter */
+	return (optchar);
+}
+
+/*
+ * getopt_long --
+ *	Parse argc/argv argument vector.
+ */
+int
+getopt_long(int nargc, char * const *nargv, const char *options,
+    const struct option *long_options, int *idx)
+{
+
+	return (getopt_internal(nargc, nargv, options, long_options, idx,
+	    FLAG_PERMUTE));
+}
+
+/*
+ * getopt_long_only --
+ *	Parse argc/argv argument vector.
+ */
+int
+getopt_long_only(int nargc, char * const *nargv, const char *options,
+    const struct option *long_options, int *idx)
+{
+
+	return (getopt_internal(nargc, nargv, options, long_options, idx,
+	    FLAG_PERMUTE|FLAG_LONGONLY));
+}
+
+//extern int getopt_long(int nargc, char * const *nargv, const char *options,
+//    const struct option *long_options, int *idx);
+//extern int getopt_long_only(int nargc, char * const *nargv, const char *options,
+//    const struct option *long_options, int *idx);
+/*
+ * Previous MinGW implementation had...
+ */
+#ifndef HAVE_DECL_GETOPT
+/*
+ * ...for the long form API only; keep this for compatibility.
+ */
+# define HAVE_DECL_GETOPT	1
+#endif
+
+#ifdef __cplusplus
+}
+#endif
+
 #endif /* !defined(__UNISTD_H_SOURCED__) && !defined(__GETOPT_LONG_H__) */
```

### Comparing `libonvif-2.0.10/include/onvif.h` & `libonvif-2.0.9/include/onvif.h`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,247 +1,247 @@
-
-/*******************************************************************************
-* onvif.h
-*
-* copyright 2018, 2023 Stephen Rhodes
-*
-* This library is free software; you can redistribute it and/or
-* modify it under the terms of the GNU Lesser General Public
-* License as published by the Free Software Foundation; either
-* version 2.1 of the License, or (at your option) any later version.
-*
-* This library is distributed in the hope that it will be useful,
-* but WITHOUT ANY WARRANTY; without even the implied warranty of
-* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-* Lesser General Public License for more details.
-*
-* You should have received a copy of the GNU Lesser General Public
-* License along with this library; if not, write to the Free Software
-* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-*
-*******************************************************************************/
-
-#ifndef ONVIF_H
-#define ONVIF_H
-
-#include <stdbool.h>
-#include <time.h> 
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#ifndef _WIN32
-    #include <time.h>
-#endif
-
-#ifdef __MINGW32__
-    #include <ws2tcpip.h>
-#endif
-
-#ifdef LIBONVIFDLL_EXPORTS
-    #define LIBRARY_API __declspec(dllexport)
-#else
-    #define LIBRARY_API extern
-#endif
-
-static const int PAN_TILT_STOP = 0;
-static const int ZOOM_STOP = 1;
-
-struct OnvifData {
-    /*video*/
-    char videoEncoderConfigurationToken[128];
-    char resolutions_buf[16][128];
-    int gov_length_min;
-    int gov_length_max;
-    int frame_rate_min;
-    int frame_rate_max;
-    int bitrate_min;
-    int bitrate_max;
-    int width;
-    int height;
-    int gov_length;
-    int frame_rate;
-    int bitrate;
-    char video_encoder_name_buf[128];
-    int use_count;
-    float quality;
-    char h264_profile_buf[128];
-    char multicast_address_type_buf[128];
-    char multicast_address_buf[128];
-    int multicast_port;
-    int multicast_ttl;
-    bool autostart;
-    char session_time_out_buf[128];
-	bool guaranteed_frame_rate;
-    char encoding[128];
-    int conf_width;
-    int conf_height;
-    int conf_frame_rate_limit;
-    int conf_encoding_interval;
-    int conf_bitrate_limit;
-    /*network*/
-    char networkInterfaceToken[128];
-    char networkInterfaceName[128];
-    bool dhcp_enabled;
-    char ip_address_buf[128];
-    char default_gateway_buf[128];
-    char dns_buf[128];
-    int prefix_length;
-    char mask_buf[128];
-    /*image*/
-    char videoSourceConfigurationToken[128];
-    int brightness_min;
-    int brightness_max;
-    int saturation_min;
-    int saturation_max;
-    int contrast_min;
-    int contrast_max;
-    int sharpness_min;
-    int sharpness_max;
-    int brightness;
-    int saturation;
-    int contrast;
-    int sharpness;
-    /*service*/
-    char device_service[1024];
-    char media_service[1024];
-    char imaging_service[1024];
-    char ptz_service[1024];
-    char event_service[1024];
-    /*event*/
-    char subscription_reference[128];
-    int event_listen_port;
-    /*general*/
-    char xaddrs[1024];
-    char profileToken[128];
-    char username[128];
-    char password[128];
-    time_t time_offset;
-    char stream_uri[1024];
-    char camera_name[1024];
-    char serial_number[128];
-    char host_name[1024];
-    char host[128];
-    /*error*/
-    char last_error[1024];
-	/*date/time*/
-	char datetimetype;
-	bool dst;
-	char timezone[128];
-	bool ntp_dhcp;
-	char ntp_type[128];
-	char ntp_addr[128];
-};
-
-struct OnvifSession {
-    char buf[128][8192];
-    int len[128];
-    char uuid[47];
-    int discovery_msg_id;
-    char preferred_network_address[16];
-    char active_network_interfaces[16][1024];
-};
-
-LIBRARY_API void initializeSession(struct OnvifSession *onvif_session);
-LIBRARY_API void closeSession(struct OnvifSession *onvif_session);
-LIBRARY_API int broadcast(struct OnvifSession *onvif_session);
-LIBRARY_API bool prepareOnvifData(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
-LIBRARY_API int fillRTSPn(struct OnvifData *onvif_data, int profileIndex);
-#define fillRTSP(a) fillRTSPn(a,0)
-LIBRARY_API void clearData(struct OnvifData *onvif_data);
-
-LIBRARY_API int getCapabilities(struct OnvifData *onvif_data);
-LIBRARY_API int getProfile(struct OnvifData *onvif_data);
-
-LIBRARY_API int getNetworkInterfaces(struct OnvifData *onvif_data);
-LIBRARY_API int setNetworkInterfaces(struct OnvifData *onvif_data);
-LIBRARY_API int getNetworkDefaultGateway(struct OnvifData *onvif_data);
-LIBRARY_API int setNetworkDefaultGateway(struct OnvifData *onvif_data);
-LIBRARY_API int getDNS(struct OnvifData *onvif_data);
-LIBRARY_API int setDNS(struct OnvifData *onvif_data);
-LIBRARY_API int getNTP(struct OnvifData *onvif_data);
-LIBRARY_API int setNTP(struct OnvifData *onvif_data);
-LIBRARY_API int getHostname(struct OnvifData *onvif_data);
-LIBRARY_API int setHostname(struct OnvifData *onvif_data);
-
-LIBRARY_API int getVideoEncoderConfigurationOptions(struct OnvifData *onvif_data);
-LIBRARY_API int getVideoEncoderConfiguration(struct OnvifData *onvif_data);
-LIBRARY_API int setVideoEncoderConfiguration(struct OnvifData *onvif_data);
-
-LIBRARY_API int getOptions(struct OnvifData *onvif_data);
-LIBRARY_API int getImagingSettings(struct OnvifData *onvif_data);
-LIBRARY_API int setImagingSettings(struct OnvifData *onvif_data);
-
-LIBRARY_API int continuousMove(float x, float y, float z, struct OnvifData *onvif_data);
-LIBRARY_API int moveStop(int type, struct OnvifData *onvif_data);
-LIBRARY_API int setPreset(char * arg, struct OnvifData *onvif_data);
-LIBRARY_API int gotoPreset(char * arg, struct OnvifData *onvif_data);
-
-LIBRARY_API int setUser(char * new_password, struct OnvifData *onvif_data);
-LIBRARY_API int setSystemDateAndTime(struct OnvifData *onvif_data);
-LIBRARY_API int setSystemDateAndTimeUsingTimezone(struct OnvifData *onvif_data);
-LIBRARY_API int getTimeOffset(struct OnvifData *onvif_data);
-LIBRARY_API int getProfileToken(struct OnvifData *onvif_data, int profileIndex);
-#define getFirstProfileToken(a) getProfileToken(a,0)
-LIBRARY_API int getStreamUri(struct OnvifData *onvif_data);
-LIBRARY_API int getDeviceInformation(struct OnvifData *onvif_data);
-LIBRARY_API int rebootCamera(struct OnvifData *onvif_data);
-LIBRARY_API int hardReset(struct OnvifData *onvif_data);
-
-LIBRARY_API void saveSystemDateAndTime(char * filename, struct OnvifData *onvif_data);
-LIBRARY_API void saveScopes(char * filename, struct OnvifData *onvif_data);
-LIBRARY_API void saveDeviceInformation(char * filename, struct OnvifData *onvif_data);
-LIBRARY_API void saveCapabilities(char * filename, struct OnvifData *onvif_data);
-LIBRARY_API void saveProfiles(char * filename, struct OnvifData *onvif_data);
-LIBRARY_API void saveServiceCapabilities(char * filename, struct OnvifData *onvif_data);
-
-LIBRARY_API int eventSubscribe(struct OnvifData *onvif_data);
-LIBRARY_API int eventRenew(struct OnvifData *onvif_data);
-
-/*
-LIBRARY_API xmlDocPtr sendCommandToCamera(char * cmd, char * xaddrs);
-LIBRARY_API void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result);
-LIBRARY_API void getUUID(char uuid_buf[47]);
-LIBRARY_API void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char * user, char * password, time_t offset);
-LIBRARY_API void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char * xaddrs, char * post_type, char cmd[], int cmd_length);
-LIBRARY_API void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]);
-LIBRARY_API void getDiscoveryXml2(char buffer[], int buf_size);
-LIBRARY_API void getScopeField(char *, char *, char[1024]);
-LIBRARY_API void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
-LIBRARY_API void extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
-LIBRARY_API void extractOnvifService(char service[1024], bool post);
-LIBRARY_API void extractHost(char * xaddrs, char host[128]);
-LIBRARY_API int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]);
-LIBRARY_API int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length);
-LIBRARY_API int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex);
-#define getNodeAttribute(doc,xpath,attribute,buf,buf_length) getNodeAttributen(doc,xpath,attribute,buf,buf_length,0)
-LIBRARY_API xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath);
-*/
-
-LIBRARY_API void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]);
-LIBRARY_API void getDiscoveryXml2(char buffer[], int buf_size);
-LIBRARY_API void getScopeField(char *, char *, char[1024]);
-LIBRARY_API void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
-LIBRARY_API bool extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
-LIBRARY_API void extractOnvifService(char service[1024], bool post);
-LIBRARY_API void extractHost(char * xaddrs, char host[128]);
-
-LIBRARY_API int setSocketOptions(int socket);
-LIBRARY_API void prefix2mask(int prefix, char mask_buf[128]);
-LIBRARY_API int mask2prefix(char * mask_buf);
-LIBRARY_API void getIPAddress(char buf[128]);
-LIBRARY_API void copyData(struct OnvifData* dts, struct OnvifData* src);
-LIBRARY_API bool hasPTZ(struct OnvifData* onvif_data);
-LIBRARY_API void getActiveNetworkInterfaces(struct OnvifSession* onvif_session);
-LIBRARY_API void dumpConfigAll (struct OnvifData *onvif_data);
-
-#ifdef __MINGW32__
-    int inet_pton(int af, const char *src, void *dst);
-    const char *inet_ntop(int af, const void *src, char *dst, socklen_t size);
-#endif
-
-#ifdef __cplusplus
-}
-#endif
-
-#endif
+
+/*******************************************************************************
+* onvif.h
+*
+* copyright 2018, 2023 Stephen Rhodes
+*
+* This library is free software; you can redistribute it and/or
+* modify it under the terms of the GNU Lesser General Public
+* License as published by the Free Software Foundation; either
+* version 2.1 of the License, or (at your option) any later version.
+*
+* This library is distributed in the hope that it will be useful,
+* but WITHOUT ANY WARRANTY; without even the implied warranty of
+* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+* Lesser General Public License for more details.
+*
+* You should have received a copy of the GNU Lesser General Public
+* License along with this library; if not, write to the Free Software
+* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+*
+*******************************************************************************/
+
+#ifndef ONVIF_H
+#define ONVIF_H
+
+#include <stdbool.h>
+#include <time.h> 
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#ifndef _WIN32
+    #include <time.h>
+#endif
+
+#ifdef __MINGW32__
+    #include <ws2tcpip.h>
+#endif
+
+#ifdef LIBONVIFDLL_EXPORTS
+    #define LIBRARY_API __declspec(dllexport)
+#else
+    #define LIBRARY_API extern
+#endif
+
+static const int PAN_TILT_STOP = 0;
+static const int ZOOM_STOP = 1;
+
+struct OnvifData {
+    /*video*/
+    char videoEncoderConfigurationToken[128];
+    char resolutions_buf[16][128];
+    int gov_length_min;
+    int gov_length_max;
+    int frame_rate_min;
+    int frame_rate_max;
+    int bitrate_min;
+    int bitrate_max;
+    int width;
+    int height;
+    int gov_length;
+    int frame_rate;
+    int bitrate;
+    char video_encoder_name_buf[128];
+    int use_count;
+    float quality;
+    char h264_profile_buf[128];
+    char multicast_address_type_buf[128];
+    char multicast_address_buf[128];
+    int multicast_port;
+    int multicast_ttl;
+    bool autostart;
+    char session_time_out_buf[128];
+	bool guaranteed_frame_rate;
+    char encoding[128];
+    int conf_width;
+    int conf_height;
+    int conf_frame_rate_limit;
+    int conf_encoding_interval;
+    int conf_bitrate_limit;
+    /*network*/
+    char networkInterfaceToken[128];
+    char networkInterfaceName[128];
+    bool dhcp_enabled;
+    char ip_address_buf[128];
+    char default_gateway_buf[128];
+    char dns_buf[128];
+    int prefix_length;
+    char mask_buf[128];
+    /*image*/
+    char videoSourceConfigurationToken[128];
+    int brightness_min;
+    int brightness_max;
+    int saturation_min;
+    int saturation_max;
+    int contrast_min;
+    int contrast_max;
+    int sharpness_min;
+    int sharpness_max;
+    int brightness;
+    int saturation;
+    int contrast;
+    int sharpness;
+    /*service*/
+    char device_service[1024];
+    char media_service[1024];
+    char imaging_service[1024];
+    char ptz_service[1024];
+    char event_service[1024];
+    /*event*/
+    char subscription_reference[128];
+    int event_listen_port;
+    /*general*/
+    char xaddrs[1024];
+    char profileToken[128];
+    char username[128];
+    char password[128];
+    time_t time_offset;
+    char stream_uri[1024];
+    char camera_name[1024];
+    char serial_number[128];
+    char host_name[1024];
+    char host[128];
+    /*error*/
+    char last_error[1024];
+	/*date/time*/
+	char datetimetype;
+	bool dst;
+	char timezone[128];
+	bool ntp_dhcp;
+	char ntp_type[128];
+	char ntp_addr[128];
+};
+
+struct OnvifSession {
+    char buf[128][8192];
+    int len[128];
+    char uuid[47];
+    int discovery_msg_id;
+    char preferred_network_address[16];
+    char active_network_interfaces[16][1024];
+};
+
+LIBRARY_API void initializeSession(struct OnvifSession *onvif_session);
+LIBRARY_API void closeSession(struct OnvifSession *onvif_session);
+LIBRARY_API int broadcast(struct OnvifSession *onvif_session);
+LIBRARY_API bool prepareOnvifData(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
+LIBRARY_API int fillRTSPn(struct OnvifData *onvif_data, int profileIndex);
+#define fillRTSP(a) fillRTSPn(a,0)
+LIBRARY_API void clearData(struct OnvifData *onvif_data);
+
+LIBRARY_API int getCapabilities(struct OnvifData *onvif_data);
+LIBRARY_API int getProfile(struct OnvifData *onvif_data);
+
+LIBRARY_API int getNetworkInterfaces(struct OnvifData *onvif_data);
+LIBRARY_API int setNetworkInterfaces(struct OnvifData *onvif_data);
+LIBRARY_API int getNetworkDefaultGateway(struct OnvifData *onvif_data);
+LIBRARY_API int setNetworkDefaultGateway(struct OnvifData *onvif_data);
+LIBRARY_API int getDNS(struct OnvifData *onvif_data);
+LIBRARY_API int setDNS(struct OnvifData *onvif_data);
+LIBRARY_API int getNTP(struct OnvifData *onvif_data);
+LIBRARY_API int setNTP(struct OnvifData *onvif_data);
+LIBRARY_API int getHostname(struct OnvifData *onvif_data);
+LIBRARY_API int setHostname(struct OnvifData *onvif_data);
+
+LIBRARY_API int getVideoEncoderConfigurationOptions(struct OnvifData *onvif_data);
+LIBRARY_API int getVideoEncoderConfiguration(struct OnvifData *onvif_data);
+LIBRARY_API int setVideoEncoderConfiguration(struct OnvifData *onvif_data);
+
+LIBRARY_API int getOptions(struct OnvifData *onvif_data);
+LIBRARY_API int getImagingSettings(struct OnvifData *onvif_data);
+LIBRARY_API int setImagingSettings(struct OnvifData *onvif_data);
+
+LIBRARY_API int continuousMove(float x, float y, float z, struct OnvifData *onvif_data);
+LIBRARY_API int moveStop(int type, struct OnvifData *onvif_data);
+LIBRARY_API int setPreset(char * arg, struct OnvifData *onvif_data);
+LIBRARY_API int gotoPreset(char * arg, struct OnvifData *onvif_data);
+
+LIBRARY_API int setUser(char * new_password, struct OnvifData *onvif_data);
+LIBRARY_API int setSystemDateAndTime(struct OnvifData *onvif_data);
+LIBRARY_API int setSystemDateAndTimeUsingTimezone(struct OnvifData *onvif_data);
+LIBRARY_API int getTimeOffset(struct OnvifData *onvif_data);
+LIBRARY_API int getProfileToken(struct OnvifData *onvif_data, int profileIndex);
+#define getFirstProfileToken(a) getProfileToken(a,0)
+LIBRARY_API int getStreamUri(struct OnvifData *onvif_data);
+LIBRARY_API int getDeviceInformation(struct OnvifData *onvif_data);
+LIBRARY_API int rebootCamera(struct OnvifData *onvif_data);
+LIBRARY_API int hardReset(struct OnvifData *onvif_data);
+
+LIBRARY_API void saveSystemDateAndTime(char * filename, struct OnvifData *onvif_data);
+LIBRARY_API void saveScopes(char * filename, struct OnvifData *onvif_data);
+LIBRARY_API void saveDeviceInformation(char * filename, struct OnvifData *onvif_data);
+LIBRARY_API void saveCapabilities(char * filename, struct OnvifData *onvif_data);
+LIBRARY_API void saveProfiles(char * filename, struct OnvifData *onvif_data);
+LIBRARY_API void saveServiceCapabilities(char * filename, struct OnvifData *onvif_data);
+
+LIBRARY_API int eventSubscribe(struct OnvifData *onvif_data);
+LIBRARY_API int eventRenew(struct OnvifData *onvif_data);
+
+/*
+LIBRARY_API xmlDocPtr sendCommandToCamera(char * cmd, char * xaddrs);
+LIBRARY_API void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result);
+LIBRARY_API void getUUID(char uuid_buf[47]);
+LIBRARY_API void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char * user, char * password, time_t offset);
+LIBRARY_API void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char * xaddrs, char * post_type, char cmd[], int cmd_length);
+LIBRARY_API void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]);
+LIBRARY_API void getDiscoveryXml2(char buffer[], int buf_size);
+LIBRARY_API void getScopeField(char *, char *, char[1024]);
+LIBRARY_API void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
+LIBRARY_API void extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
+LIBRARY_API void extractOnvifService(char service[1024], bool post);
+LIBRARY_API void extractHost(char * xaddrs, char host[128]);
+LIBRARY_API int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]);
+LIBRARY_API int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length);
+LIBRARY_API int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex);
+#define getNodeAttribute(doc,xpath,attribute,buf,buf_length) getNodeAttributen(doc,xpath,attribute,buf,buf_length,0)
+LIBRARY_API xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath);
+*/
+
+LIBRARY_API void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]);
+LIBRARY_API void getDiscoveryXml2(char buffer[], int buf_size);
+LIBRARY_API void getScopeField(char *, char *, char[1024]);
+LIBRARY_API void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
+LIBRARY_API bool extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data);
+LIBRARY_API void extractOnvifService(char service[1024], bool post);
+LIBRARY_API void extractHost(char * xaddrs, char host[128]);
+
+LIBRARY_API int setSocketOptions(int socket);
+LIBRARY_API void prefix2mask(int prefix, char mask_buf[128]);
+LIBRARY_API int mask2prefix(char * mask_buf);
+LIBRARY_API void getIPAddress(char buf[128]);
+LIBRARY_API void copyData(struct OnvifData* dts, struct OnvifData* src);
+LIBRARY_API bool hasPTZ(struct OnvifData* onvif_data);
+LIBRARY_API void getActiveNetworkInterfaces(struct OnvifSession* onvif_session);
+LIBRARY_API void dumpConfigAll (struct OnvifData *onvif_data);
+
+#ifdef __MINGW32__
+    int inet_pton(int af, const char *src, void *dst);
+    const char *inet_ntop(int af, const void *src, char *dst, socklen_t size);
+#endif
+
+#ifdef __cplusplus
+}
+#endif
+
+#endif
```

### Comparing `libonvif-2.0.10/include/sha1.h` & `libonvif-2.0.9/include/sha1.h`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-/*
-   SHA-1 in C
-   By Steve Reid <steve@edmweb.com>
-   100% Public Domain
-
-The person or persons who have associated work with this document (the "Dedicator" or "Certifier")
-hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
-is in the public domain of the country from which the work is published, or (b) hereby dedicates 
-whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
-the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
-associated work, and for these purposes, is described as a "dedicator" below.
-
-A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
-recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
-is not in the public domain.
-
-Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
-Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
-in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
-Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
-rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
-
-Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
-transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
-non-commercial, and in any way, including by methods that have not yet been invented or conceived.
-
-CC0 for Public Domain Dedication
-This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
-to the public domain, we recommend CC0.
- */
-
-#ifndef SHA1_H
-#define SHA1_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include "stdint.h"
-
-typedef struct
-{
-    uint32_t state[5];
-    uint32_t count[2];
-    unsigned char buffer[64];
-} SHA1_CTX;
-
-void SHA1Transform(
-    uint32_t state[5],
-    const unsigned char buffer[64]
-    );
-
-void SHA1Init(
-    SHA1_CTX * context
-    );
-
-void SHA1Update(
-    SHA1_CTX * context,
-    const unsigned char *data,
-    uint32_t len
-    );
-
-void SHA1Final(
-    unsigned char digest[20],
-    SHA1_CTX * context
-    );
-
-void SHA1(
-    char *hash_out,
-    const char *str,
-    int len);
-
-#ifdef __cplusplus
-}
-#endif
-
-#endif /* SHA1_H */
+/*
+   SHA-1 in C
+   By Steve Reid <steve@edmweb.com>
+   100% Public Domain
+
+The person or persons who have associated work with this document (the "Dedicator" or "Certifier")
+hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
+is in the public domain of the country from which the work is published, or (b) hereby dedicates 
+whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
+the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
+associated work, and for these purposes, is described as a "dedicator" below.
+
+A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
+recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
+is not in the public domain.
+
+Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
+Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
+in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
+Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
+rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
+
+Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
+transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
+non-commercial, and in any way, including by methods that have not yet been invented or conceived.
+
+CC0 for Public Domain Dedication
+This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
+to the public domain, we recommend CC0.
+ */
+
+#ifndef SHA1_H
+#define SHA1_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "stdint.h"
+
+typedef struct
+{
+    uint32_t state[5];
+    uint32_t count[2];
+    unsigned char buffer[64];
+} SHA1_CTX;
+
+void SHA1Transform(
+    uint32_t state[5],
+    const unsigned char buffer[64]
+    );
+
+void SHA1Init(
+    SHA1_CTX * context
+    );
+
+void SHA1Update(
+    SHA1_CTX * context,
+    const unsigned char *data,
+    uint32_t len
+    );
+
+void SHA1Final(
+    unsigned char digest[20],
+    SHA1_CTX * context
+    );
+
+void SHA1(
+    char *hash_out,
+    const char *str,
+    int len);
+
+#ifdef __cplusplus
+}
+#endif
+
+#endif /* SHA1_H */
```

### Comparing `libonvif-2.0.10/libonvif.egg-info/PKG-INFO` & `libonvif-2.0.9/src/libonvif.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: libonvif
-Version: 2.0.10
+Version: 2.0.9
 Summary: A python module for communicating with onvif cameras
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Tracker, https://github.com/sr99622/libonvif/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libonvif
 
 Python enabled library for communicating with onvif devices.
 
@@ -27,19 +27,19 @@
 to install the dependencies.
 
 ```
 sudo apt install cmake libxml2-dev
 ```
 
 **Windows**, please use Anaconda.  The dependencies may
-be installed using the following command under a conda prompt. 
+be installed using the following command under a conda prompt.  The 
 Visual Studio C++ compiler must be installed as well.
 
 ```
-conda install cmake libxml2 -c conda-forge
+conda install cmake libxml2
 ```
 
 If successful, install libonvif python module
 
 ```
 pip install libonvif
 ```
```

### Comparing `libonvif-2.0.10/libonvif.egg-info/SOURCES.txt` & `libonvif-2.0.9/src/libonvif.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,14 @@
 pyproject.toml
 setup.py
 include/cencode.h
 include/getopt-win.h
 include/onvif.h
 include/onvifboss.h
 include/sha1.h
-libonvif/__init__.py
-libonvif.egg-info/PKG-INFO
-libonvif.egg-info/SOURCES.txt
-libonvif.egg-info/dependency_links.txt
-libonvif.egg-info/not-zip-safe
-libonvif.egg-info/top_level.txt
 pybind11/.appveyor.yml
 pybind11/.clang-format
 pybind11/.clang-tidy
 pybind11/.cmake-format.yaml
 pybind11/.codespell-ignore-lines
 pybind11/.git
 pybind11/.gitattributes
@@ -105,15 +99,14 @@
 pybind11/include/pybind11/numpy.h
 pybind11/include/pybind11/operators.h
 pybind11/include/pybind11/options.h
 pybind11/include/pybind11/pybind11.h
 pybind11/include/pybind11/pytypes.h
 pybind11/include/pybind11/stl.h
 pybind11/include/pybind11/stl_bind.h
-pybind11/include/pybind11/type_caster_pyobject_ptr.h
 pybind11/include/pybind11/detail/class.h
 pybind11/include/pybind11/detail/common.h
 pybind11/include/pybind11/detail/descr.h
 pybind11/include/pybind11/detail/init.h
 pybind11/include/pybind11/detail/internals.h
 pybind11/include/pybind11/detail/type_caster_base.h
 pybind11/include/pybind11/detail/typeid.h
@@ -217,24 +210,16 @@
 pybind11/tests/test_stl.py
 pybind11/tests/test_stl_binders.cpp
 pybind11/tests/test_stl_binders.py
 pybind11/tests/test_tagbased_polymorphic.cpp
 pybind11/tests/test_tagbased_polymorphic.py
 pybind11/tests/test_thread.cpp
 pybind11/tests/test_thread.py
-pybind11/tests/test_type_caster_pyobject_ptr.cpp
-pybind11/tests/test_type_caster_pyobject_ptr.py
 pybind11/tests/test_union.cpp
 pybind11/tests/test_union.py
-pybind11/tests/test_unnamed_namespace_a.cpp
-pybind11/tests/test_unnamed_namespace_a.py
-pybind11/tests/test_unnamed_namespace_b.cpp
-pybind11/tests/test_unnamed_namespace_b.py
-pybind11/tests/test_vector_unique_ptr_member.cpp
-pybind11/tests/test_vector_unique_ptr_member.py
 pybind11/tests/test_virtual_functions.cpp
 pybind11/tests/test_virtual_functions.py
 pybind11/tests/valgrind-numpy-scipy.supp
 pybind11/tests/valgrind-python.supp
 pybind11/tests/extra_python_package/pytest.ini
 pybind11/tests/extra_python_package/test_files.py
 pybind11/tests/extra_setuptools/pytest.ini
@@ -272,8 +257,13 @@
 pybind11/tools/pyproject.toml
 pybind11/tools/setup_global.py.in
 pybind11/tools/setup_main.py.in
 src/cencode.c
 src/onvif.c
 src/onvif.cpp
 src/onvifboss.cpp
-src/sha1.c
+src/sha1.c
+src/libonvif.egg-info/PKG-INFO
+src/libonvif.egg-info/SOURCES.txt
+src/libonvif.egg-info/dependency_links.txt
+src/libonvif.egg-info/not-zip-safe
+src/libonvif.egg-info/top_level.txt
```

### Comparing `libonvif-2.0.10/pybind11/.appveyor.yml` & `libonvif-2.0.9/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.clang-format` & `libonvif-2.0.9/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.clang-tidy` & `libonvif-2.0.9/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.cmake-format.yaml` & `libonvif-2.0.9/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.codespell-ignore-lines` & `libonvif-2.0.9/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.github/CONTRIBUTING.md` & `libonvif-2.0.9/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `libonvif-2.0.9/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.github/matchers/pylint.json` & `libonvif-2.0.9/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.github/pull_request_template.md` & `libonvif-2.0.9/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/ci.yml` & `libonvif-2.0.9/pybind11/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
   pull_request:
   push:
     branches:
       - master
       - stable
       - v*
 
-permissions: read-all
-
 concurrency:
   group: test-${{ github.ref }}
   cancel-in-progress: true
 
 env:
   PIP_ONLY_BINARY: numpy
   FORCE_COLOR: 3
@@ -80,15 +78,15 @@
       run: sudo apt-get install libboost-dev
 
     - name: Setup Boost (macOS)
       if: runner.os == 'macOS'
       run: brew install boost
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Cache wheels
       if: runner.os == 'macOS'
       uses: actions/cache@v3
       with:
         # This path is specific to macOS - we really only need it for PyPy NumPy wheels
         # See https://github.com/actions/cache/blob/master/examples.md#python---pip
@@ -162,14 +160,15 @@
       run: >
         cmake -S . -B build3
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
         -DDOWNLOAD_EIGEN=ON
         -DCMAKE_CXX_STANDARD=17
         -DPYBIND11_INTERNALS_VERSION=10000000
+        "-DPYBIND11_TEST_OVERRIDE=test_call_policies.cpp;test_gil_scoped.cpp;test_thread.cpp"
         ${{ matrix.args }}
 
     - name: Build (unstable ABI)
       run: cmake --build build3 -j 2
 
     - name: Python tests (unstable ABI)
       run: cmake --build build3 --target pytest
@@ -205,15 +204,15 @@
     - name: Setup Python ${{ matrix.python-version }} (deadsnakes)
       uses: deadsnakes/action@v3.0.0
       with:
         python-version: ${{ matrix.python-version }}
         debug: ${{ matrix.python-debug }}
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Valgrind cache
       if: matrix.valgrind
       uses: actions/cache@v3
       id: cache-valgrind
       with:
         path: valgrind
@@ -471,15 +470,15 @@
     - name: Add Python 3
       run: apt-get update; apt-get install -y python3-dev python3-numpy python3-pytest python3-pip libeigen3-dev
 
     - name: Update pip
       run: python3 -m pip install --upgrade pip
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Configure
       shell: bash
       run: >
         cmake -S . -B build
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
@@ -494,32 +493,14 @@
 
     - name: C++ tests
       run: cmake --build build --target cpptest
 
     - name: Interface test
       run: cmake --build build --target test_cmake_build
 
-    - name: Configure - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      if: matrix.gcc == '12'
-      shell: bash
-      run: >
-        cmake -S . -B build_partial
-        -DPYBIND11_WERROR=ON
-        -DDOWNLOAD_CATCH=ON
-        -DCMAKE_CXX_STANDARD=${{ matrix.std }}
-        -DPYTHON_EXECUTABLE=$(python3 -c "import sys; print(sys.executable)")
-        "-DPYBIND11_TEST_OVERRIDE=test_call_policies.cpp;test_gil_scoped.cpp;test_thread.cpp"
-
-    - name: Build - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      if: matrix.gcc == '12'
-      run: cmake --build build_partial -j 2
-
-    - name: Python tests - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      if: matrix.gcc == '12'
-      run: cmake --build build_partial --target pytest
 
   # Testing on ICC using the oneAPI apt repo
   icc:
     runs-on: ubuntu-20.04
     strategy:
       fail-fast: false
 
@@ -778,15 +759,15 @@
     - name: Setup Python ${{ matrix.python }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
         architecture: x86
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Prepare MSVC
       uses: ilammy/msvc-dev-cmd@v1.12.1
       with:
         arch: x86
 
     - name: Prepare env
@@ -831,15 +812,15 @@
     - name: Setup Python ${{ matrix.python }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python }}
         architecture: x86
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Prepare MSVC
       uses: ilammy/msvc-dev-cmd@v1.12.1
       with:
         arch: x86
 
     - name: Prepare env
@@ -882,15 +863,15 @@
         python-version: ${{ matrix.python }}
 
     - name: Prepare env
       run: |
         python3 -m pip install -r tests/requirements.txt
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
     - name: Configure C++20
       run: >
         cmake -S . -B build
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
         -DDOWNLOAD_EIGEN=ON
@@ -904,29 +885,14 @@
 
     - name: C++20 tests
       run: cmake --build build --target cpptest -j 2
 
     - name: Interface test C++20
       run: cmake --build build --target test_cmake_build
 
-    - name: Configure C++20 - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      run: >
-        cmake -S . -B build_partial
-        -DPYBIND11_WERROR=ON
-        -DDOWNLOAD_CATCH=ON
-        -DDOWNLOAD_EIGEN=ON
-        -DCMAKE_CXX_STANDARD=20
-        "-DPYBIND11_TEST_OVERRIDE=test_call_policies.cpp;test_gil_scoped.cpp;test_thread.cpp"
-
-    - name: Build C++20 - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      run: cmake --build build_partial -j 2
-
-    - name: Python tests - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-      run: cmake --build build_partial --target pytest
-
   mingw:
     name: "🐍 3 • windows-latest • ${{ matrix.sys }}"
     runs-on: windows-latest
     defaults:
       run:
         shell: msys2 {0}
     strategy:
@@ -1030,15 +996,15 @@
 
       - name: Setup Python ${{ matrix.python }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
       - name: Update CMake
-        uses: jwlawson/actions-setup-cmake@v1.14
+        uses: jwlawson/actions-setup-cmake@v1.13
 
       - name: Install ninja-build tool
         uses: seanmiddleditch/gha-setup-ninja@v3
 
       - name: Run pip installs
         run: |
           python -m pip install --upgrade pip
@@ -1100,15 +1066,15 @@
       - name: brew install llvm
         run: brew install llvm
 
       - name: Show Clang++ version after brew install llvm
         run: clang++ --version
 
       - name: Update CMake
-        uses: jwlawson/actions-setup-cmake@v1.14
+        uses: jwlawson/actions-setup-cmake@v1.13
 
       - name: Run pip installs
         run: |
           python3 -m pip install --upgrade pip
           python3 -m pip install -r tests/requirements.txt
           python3 -m pip install numpy
           python3 -m pip install scipy
@@ -1135,27 +1101,9 @@
 
       - name: C++ tests
         run: cmake --build . --target cpptest -j 2
 
       - name: Interface test
         run: cmake --build . --target test_cmake_build -j 2
 
-      - name: CMake Configure - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-        run: >
-          cmake -S . -B build_partial
-          -DPYBIND11_WERROR=ON
-          -DPYBIND11_SIMPLE_GIL_MANAGEMENT=OFF
-          -DDOWNLOAD_CATCH=ON
-          -DDOWNLOAD_EIGEN=ON
-          -DCMAKE_CXX_COMPILER=clang++
-          -DCMAKE_CXX_STANDARD=17
-          -DPYTHON_EXECUTABLE=$(python3 -c "import sys; print(sys.executable)")
-          "-DPYBIND11_TEST_OVERRIDE=test_call_policies.cpp;test_gil_scoped.cpp;test_thread.cpp"
-
-      - name: Build - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-        run: cmake --build build_partial -j 2
-
-      - name: Python tests - Exercise cmake -DPYBIND11_TEST_OVERRIDE
-        run: cmake --build build_partial --target pytest -j 2
-
       - name: Clean directory
         run: git clean -fdx
```

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/configure.yml` & `libonvif-2.0.9/pybind11/.github/workflows/configure.yml`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,14 @@
   pull_request:
   push:
     branches:
       - master
       - stable
       - v*
 
-permissions:
-  contents: read
-
 env:
   # For cmake:
   VERBOSE: 1
 
 jobs:
   # This tests various versions of CMake in various combinations, to make sure
   # the configure step passes.
@@ -54,15 +51,15 @@
 
     - name: Prepare env
       run: python -m pip install -r tests/requirements.txt
 
     # An action for adding a specific version of CMake:
     #   https://github.com/jwlawson/actions-setup-cmake
     - name: Setup CMake ${{ matrix.cmake }}
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
       with:
         cmake-version: ${{ matrix.cmake }}
 
     # These steps use a directory with a space in it intentionally
     - name: Make build directories
       run: mkdir "build dir"
```

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/format.yml` & `libonvif-2.0.9/pybind11/.github/workflows/format.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,14 @@
   pull_request:
   push:
     branches:
     - master
     - stable
     - "v*"
 
-permissions:
-  contents: read
-
 env:
   FORCE_COLOR: 3
   # For cmake:
   VERBOSE: 1
 
 jobs:
   pre-commit:
```

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/labeler.yml` & `libonvif-2.0.9/pybind11/.github/workflows/labeler.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 name: Labeler
 on:
   pull_request_target:
     types: [closed]
 
-permissions: {}
-
 jobs:
   label:
     name: Labeler
     runs-on: ubuntu-latest
-    permissions:
-      contents: read
-      pull-requests: write
     steps:
 
     - uses: actions/labeler@main
       if: >
         github.event.pull_request.merged == true &&
         !startsWith(github.event.pull_request.title, 'chore(deps):') &&
         !startsWith(github.event.pull_request.title, 'ci(fix):') &&
```

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/pip.yml` & `libonvif-2.0.9/pybind11/.github/workflows/pip.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,14 @@
     - master
     - stable
     - v*
   release:
     types:
     - published
 
-permissions:
-  contents: read
-
 env:
   PIP_ONLY_BINARY: numpy
 
 jobs:
   # This builds the sdists and wheels and makes sure the files are exactly as
   # expected. Using Windows and Python 3.6, since that is often the most
   # challenging matrix element.
@@ -97,17 +94,17 @@
       with:
         python-version: "3.x"
 
     # Downloads all to directories matching the artifact names
     - uses: actions/download-artifact@v3
 
     - name: Publish standard package
-      uses: pypa/gh-action-pypi-publish@v1.8.6
+      uses: pypa/gh-action-pypi-publish@v1.6.4
       with:
         password: ${{ secrets.pypi_password }}
-        packages-dir: standard/
+        packages_dir: standard/
 
     - name: Publish global package
-      uses: pypa/gh-action-pypi-publish@v1.8.6
+      uses: pypa/gh-action-pypi-publish@v1.6.4
       with:
         password: ${{ secrets.pypi_password_global }}
-        packages-dir: global/
+        packages_dir: global/
```

### Comparing `libonvif-2.0.10/pybind11/.github/workflows/upstream.yml` & `libonvif-2.0.9/pybind11/.github/workflows/upstream.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,114 +1,114 @@
 
 name: Upstream
 
 on:
   workflow_dispatch:
   pull_request:
 
-permissions:
-  contents: read
-
 concurrency:
   group: upstream-${{ github.ref }}
   cancel-in-progress: true
 
 env:
-  PIP_ONLY_BINARY: ":all:"
+  PIP_ONLY_BINARY: numpy
   # For cmake:
   VERBOSE: 1
 
 jobs:
   standard:
-    name: "🐍 3.12 latest • ubuntu-latest • x64"
+    name: "🐍 3.11 latest internals • ubuntu-latest • x64"
     runs-on: ubuntu-latest
-    # Only runs when the  'python dev' label is selected
     if: "contains(github.event.pull_request.labels.*.name, 'python dev')"
 
     steps:
     - uses: actions/checkout@v3
 
-    - name: Setup Python 3.12
+    - name: Setup Python 3.11
       uses: actions/setup-python@v4
       with:
-        python-version: "3.12-dev"
+        python-version: "3.11-dev"
 
-    - name: Setup Boost
+    - name: Setup Boost (Linux)
+      if: runner.os == 'Linux'
       run: sudo apt-get install libboost-dev
 
     - name: Update CMake
-      uses: jwlawson/actions-setup-cmake@v1.14
+      uses: jwlawson/actions-setup-cmake@v1.13
 
-    - name: Run pip installs
+    - name: Prepare env
       run: |
-        python -m pip install --upgrade pip
         python -m pip install -r tests/requirements.txt
 
-    - name: Show platform info
-      run: |
-        python -m platform
-        cmake --version
-        pip list
+    - name: Setup annotations on Linux
+      if: runner.os == 'Linux'
+      run: python -m pip install pytest-github-actions-annotate-failures
 
     # First build - C++11 mode and inplace
     - name: Configure C++11
       run: >
-        cmake -S . -B build11
+        cmake -S . -B .
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
         -DDOWNLOAD_EIGEN=ON
         -DCMAKE_CXX_STANDARD=11
-        -DCMAKE_BUILD_TYPE=Debug
 
     - name: Build C++11
-      run: cmake --build build11 -j 2
+      run: cmake --build . -j 2
 
     - name: Python tests C++11
-      run: cmake --build build11 --target pytest -j 2
+      run: cmake --build . --target pytest -j 2
 
-    # - name: C++11 tests
-    #   run: cmake --build build11  --target cpptest -j 2
+    - name: C++11 tests
+      run: cmake --build .  --target cpptest -j 2
 
     - name: Interface test C++11
-      run: cmake --build build11 --target test_cmake_build
+      run: cmake --build . --target test_cmake_build
+
+    - name: Clean directory
+      run: git clean -fdx
 
     # Second build - C++17 mode and in a build directory
     - name: Configure C++17
       run: >
-        cmake -S . -B build17
+        cmake -S . -B build2
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
         -DDOWNLOAD_EIGEN=ON
         -DCMAKE_CXX_STANDARD=17
+        ${{ matrix.args }}
+        ${{ matrix.args2 }}
 
     - name: Build
-      run: cmake --build build17 -j 2
+      run: cmake --build build2 -j 2
 
     - name: Python tests
-      run: cmake --build build17 --target pytest
+      run: cmake --build build2 --target pytest
 
-    # - name: C++ tests
-    #   run: cmake --build build17 --target cpptest
+    - name: C++ tests
+      run: cmake --build build2 --target cpptest
 
     # Third build - C++17 mode with unstable ABI
     - name: Configure (unstable ABI)
       run: >
-        cmake -S . -B build17max
+        cmake -S . -B build3
         -DPYBIND11_WERROR=ON
         -DDOWNLOAD_CATCH=ON
         -DDOWNLOAD_EIGEN=ON
         -DCMAKE_CXX_STANDARD=17
         -DPYBIND11_INTERNALS_VERSION=10000000
+        "-DPYBIND11_TEST_OVERRIDE=test_call_policies.cpp;test_gil_scoped.cpp;test_thread.cpp"
+        ${{ matrix.args }}
 
     - name: Build (unstable ABI)
-      run: cmake --build build17max -j 2
+      run: cmake --build build3 -j 2
 
     - name: Python tests (unstable ABI)
-      run: cmake --build build17max --target pytest
+      run: cmake --build build3 --target pytest
 
     - name: Interface test
-      run: cmake --build build17max --target test_cmake_build
+      run: cmake --build build3 --target test_cmake_build
 
     # This makes sure the setup_helpers module can build packages using
     # setuptools
     - name: Setuptools helpers test
       run: pytest tests/extra_setuptools
```

### Comparing `libonvif-2.0.10/pybind11/.pre-commit-config.yaml` & `libonvif-2.0.9/pybind11/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -37,42 +37,42 @@
   - id: end-of-file-fixer
   - id: mixed-line-ending
   - id: requirements-txt-fixer
   - id: trailing-whitespace
 
 # Black, the code formatter, natively supports pre-commit
 - repo: https://github.com/psf/black
-  rev: "23.3.0" # Keep in sync with blacken-docs
+  rev: "23.1.0" # Keep in sync with blacken-docs
   hooks:
   - id: black
 
 # Also code format the docs
 - repo: https://github.com/asottile/blacken-docs
   rev: "1.13.0"
   hooks:
   - id: blacken-docs
     additional_dependencies:
-    - black==23.3.0 # keep in sync with black hook
+    - black==23.1.0 # keep in sync with black hook
 
 # Changes tabs to spaces
 - repo: https://github.com/Lucas-C/pre-commit-hooks
-  rev: "v1.5.1"
+  rev: "v1.4.2"
   hooks:
   - id: remove-tabs
 
 # Avoid directional quotes
 - repo: https://github.com/sirosen/texthooks
   rev: "0.5.0"
   hooks:
   - id: fix-ligatures
   - id: fix-smartquotes
 
 # Ruff, the Python auto-correcting linter written in Rust
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.263
+  rev: v0.0.251
   hooks:
   - id: ruff
     args: ["--fix", "--show-fixes"]
 
 # Checking for common mistakes
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: "v1.10.0"
@@ -80,15 +80,15 @@
   - id: rst-backticks
   - id: rst-directive-colons
   - id: rst-inline-touching-normal
 
 
 # PyLint has native support - not always usable, but works for us
 - repo: https://github.com/PyCQA/pylint
-  rev: "v3.0.0a6"
+  rev: "v2.16.1"
   hooks:
   - id: pylint
     files: ^pybind11
 
 # CMake formatting
 - repo: https://github.com/cheshirekow/cmake-format-precommit
   rev: "v0.6.13"
@@ -96,15 +96,15 @@
   - id: cmake-format
     additional_dependencies: [pyyaml]
     types: [file]
     files: (\.cmake|CMakeLists.txt)(.in)?$
 
 # Check static types with mypy
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: "v1.2.0"
+  rev: "v0.991"
   hooks:
   - id: mypy
     args: []
     exclude: ^(tests|docs)/
     additional_dependencies: [nox, rich]
 
 # Checks the manifest for missing files (native support)
@@ -116,19 +116,19 @@
     stages: [manual]
     additional_dependencies: [cmake, ninja]
 
 # Check for spelling
 # Use tools/codespell_ignore_lines_from_errors.py
 # to rebuild .codespell-ignore-lines
 - repo: https://github.com/codespell-project/codespell
-  rev: "v2.2.4"
+  rev: "v2.2.2"
   hooks:
   - id: codespell
     exclude: ".supp$"
-    args: ["-x.codespell-ignore-lines", "-Lccompiler"]
+    args: ["-x", ".codespell-ignore-lines"]
 
 # Check for common shell mistakes
 - repo: https://github.com/shellcheck-py/shellcheck-py
   rev: "v0.9.0.2"
   hooks:
   - id: shellcheck
 
@@ -139,11 +139,11 @@
     name: Disallow improper capitalization
     language: pygrep
     entry: PyBind|Numpy|Cmake|CCache|PyTest
     exclude: ^\.pre-commit-config.yaml$
 
 # Clang format the codebase automatically
 - repo: https://github.com/pre-commit/mirrors-clang-format
-  rev: "v16.0.2"
+  rev: "v15.0.7"
   hooks:
   - id: clang-format
     types_or: [c++, c, cuda]
```

### Comparing `libonvif-2.0.10/pybind11/CMakeLists.txt` & `libonvif-2.0.9/pybind11/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,16 +135,15 @@
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
     include/pybind11/stl_bind.h
-    include/pybind11/stl/filesystem.h
-    include/pybind11/type_caster_pyobject_ptr.h)
+    include/pybind11/stl/filesystem.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
```

### Comparing `libonvif-2.0.10/pybind11/LICENSE` & `libonvif-2.0.9/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/README.rst` & `libonvif-2.0.9/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/Doxyfile` & `libonvif-2.0.9/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/Makefile` & `libonvif-2.0.9/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/chrono.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/custom.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/eigen.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/functional.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/index.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/overview.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/stl.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/cast/strings.rst` & `libonvif-2.0.9/pybind11/docs/advanced/cast/strings.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,31 +97,27 @@
 
 .. code-block:: c++
 
     // This uses the Python C API to convert Latin-1 to Unicode
     m.def("str_output",
         []() {
             std::string s = "Send your r\xe9sum\xe9 to Alice in HR"; // Latin-1
-            py::handle py_s = PyUnicode_DecodeLatin1(s.data(), s.length(), nullptr);
-            if (!py_s) {
-                throw py::error_already_set();
-            }
-            return py::reinterpret_steal<py::str>(py_s);
+            py::str py_s = PyUnicode_DecodeLatin1(s.data(), s.length());
+            return py_s;
         }
     );
 
 .. code-block:: pycon
 
     >>> str_output()
     'Send your résumé to Alice in HR'
 
 The `Python C API
 <https://docs.python.org/3/c-api/unicode.html#built-in-codecs>`_ provides
-several built-in codecs. Note that these all return *new* references, so
-use :cpp:func:`reinterpret_steal` when converting them to a :cpp:class:`str`.
+several built-in codecs.
 
 
 One could also use a third party encoding library such as libiconv to transcode
 to UTF-8.
 
 Return C++ strings without conversion
 -------------------------------------
```

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/classes.rst` & `libonvif-2.0.9/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/embedding.rst` & `libonvif-2.0.9/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/exceptions.rst` & `libonvif-2.0.9/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/functions.rst` & `libonvif-2.0.9/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/misc.rst` & `libonvif-2.0.9/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/pycpp/numpy.rst` & `libonvif-2.0.9/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/pycpp/object.rst` & `libonvif-2.0.9/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/pycpp/utilities.rst` & `libonvif-2.0.9/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/advanced/smart_ptrs.rst` & `libonvif-2.0.9/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/basics.rst` & `libonvif-2.0.9/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/benchmark.py` & `libonvif-2.0.9/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/benchmark.rst` & `libonvif-2.0.9/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/changelog.rst` & `libonvif-2.0.9/pybind11/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,112 +6,30 @@
 Starting with version 1.8.0, pybind11 releases use a `semantic versioning
 <http://semver.org>`_ policy.
 
 Changes will be added here periodically from the "Suggested changelog entry"
 block in pull request descriptions.
 
 
-Version 2.11.0 (June 2, 2023)
------------------------------
+IN DEVELOPMENT
+--------------
 
-New features:
-
-* ``pybind11::detail::is_move_constructible`` can now be specialized for cases
-   in which ``std::is_move_constructible`` does not work as needed. This is
-   very similar to the long-established
-   ``pybind11::detail::is_copy_constructible``.
-  `#4631 <https://github.com/pybind/pybind11/pull/4631>`_
-
-* Introduce ``recursive_container_traits``.
-  `#4623 <https://github.com/pybind/pybind11/pull/4623>`_
-
-* ``pybind11/type_caster_pyobject_ptr.h`` was added to support automatic
-  wrapping of APIs that make use of ``PyObject *``. This header needs to
-  included explicitly (i.e. it is not included implicitly
-  with ``pybind/pybind11.h``).
-  `#4601 <https://github.com/pybind/pybind11/pull/4601>`_
+Changes will be summarized here periodically.
 
 Changes:
 
 * ``PyGILState_Check()``'s in ``pybind11::handle``'s ``inc_ref()`` &
   ``dec_ref()`` are now enabled by default again.
   `#4246 <https://github.com/pybind/pybind11/pull/4246>`_
 
-* ``py::initialize_interpreter()`` using ``PyConfig_InitPythonConfig()``
-  instead of ``PyConfig_InitIsolatedConfig()``, to obtain complete
-  ``sys.path``.
-  `#4473 <https://github.com/pybind/pybind11/pull/4473>`_
-
-* Cast errors now always include Python type information, even if
-  ``PYBIND11_DETAILED_ERROR_MESSAGES`` is not defined. This increases binary
-  sizes slightly (~1.5%) but the error messages are much more informative.
-  `#4463 <https://github.com/pybind/pybind11/pull/4463>`_
-
-* Setter return values (which are inaccessible for all practical purposes) are
-  no longer converted to Python (only to be discarded).
-  `#4621 <https://github.com/pybind/pybind11/pull/4621>`_
-
-* Allow lambda specified to function definition to be ``noexcept(true)``
-  in C++17.
-  `#4593 <https://github.com/pybind/pybind11/pull/4593>`_
-
-* Get rid of recursive template instantiations for concatenating type
-  signatures on C++17 and higher.
-  `#4587 <https://github.com/pybind/pybind11/pull/4587>`_
-
-* Compatibility with Python 3.12 (alpha). Note that the minimum pybind11
-  ABI version for Python 3.12 is version 5. (The default ABI version
-  for Python versions up to and including 3.11 is still version 4.).
-  `#4570 <https://github.com/pybind/pybind11/pull/4570>`_
-
-* With ``PYBIND11_INTERNALS_VERSION 5`` (default for Python 3.12+), MSVC builds
-  use ``std::hash<std::type_index>`` and ``std::equal_to<std::type_index>``
-  instead of string-based type comparisons. This resolves issues when binding
-  types defined in the unnamed namespace.
-  `#4319 <https://github.com/pybind/pybind11/pull/4319>`_
-
 Build system improvements:
 
 * Update clang-tidy to 15 in CI.
   `#4387 <https://github.com/pybind/pybind11/pull/4387>`_
 
-* Moved the linting framework over to Ruff.
-  `#4483 <https://github.com/pybind/pybind11/pull/4483>`_
-
-* Skip lto checks and target generation when
-  ``CMAKE_INTERPROCEDURAL_OPTIMIZATION`` is defined.
-  `#4643 <https://github.com/pybind/pybind11/pull/4643>`_
-
-* No longer inject ``-stdlib=libc++``, not needed for modern Pythons
-  (macOS 10.9+).
-  `#4639 <https://github.com/pybind/pybind11/pull/4639>`_
-
-
-Version 2.10.4 (Mar 16, 2023)
------------------------------
-
-Changes:
-
-* ``python3 -m pybind11`` gained a ``--version`` option (prints the version and
-  exits).
-  `#4526 <https://github.com/pybind/pybind11/pull/4526>`_
-
-Bug Fixes:
-
-* Fix a warning when pydebug is enabled on Python 3.11.
-  `#4461 <https://github.com/pybind/pybind11/pull/4461>`_
-
-* Ensure ``gil_scoped_release`` RAII is non-copyable.
-  `#4490 <https://github.com/pybind/pybind11/pull/4490>`_
-
-* Ensure the tests dir does not show up with new versions of setuptools.
-  `#4510 <https://github.com/pybind/pybind11/pull/4510>`_
-
-* Better stacklevel for a warning in setuptools helpers.
-  `#4516 <https://github.com/pybind/pybind11/pull/4516>`_
 
 Version 2.10.3 (Jan 3, 2023)
 ----------------------------
 
 Changes:
 
 * Temporarily made our GIL status assertions (added in 2.10.2) disabled by
```

### Comparing `libonvif-2.0.10/pybind11/docs/classes.rst` & `libonvif-2.0.9/pybind11/docs/classes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,14 @@
     'Charly'
 
 .. seealso::
 
     Static member functions can be bound in the same way using
     :func:`class_::def_static`.
 
-.. note::
-
-    Binding C++ types in unnamed namespaces (also known as anonymous namespaces)
-    works reliably on many platforms, but not all. The `XFAIL_CONDITION` in
-    tests/test_unnamed_namespace_a.py encodes the currently known conditions.
-    For background see `#4319 <https://github.com/pybind/pybind11/pull/4319>`_.
-    If portability is a concern, it is therefore not recommended to bind C++
-    types in unnamed namespaces. It will be safest to manually pick unique
-    namespace names.
-
 Keyword and default arguments
 =============================
 It is possible to specify keyword and default arguments using the syntax
 discussed in the previous chapter. Refer to the sections :ref:`keyword_args`
 and :ref:`default_args` for details.
 
 Binding lambda functions
```

### Comparing `libonvif-2.0.10/pybind11/docs/compiling.rst` & `libonvif-2.0.9/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/conf.py` & `libonvif-2.0.9/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/faq.rst` & `libonvif-2.0.9/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/index.rst` & `libonvif-2.0.9/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/installing.rst` & `libonvif-2.0.9/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/limitations.rst` & `libonvif-2.0.9/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/pybind11-logo.png` & `libonvif-2.0.9/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python1.png` & `libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python1.svg` & `libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python2.png` & `libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/pybind11_vs_boost_python2.svg` & `libonvif-2.0.9/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/reference.rst` & `libonvif-2.0.9/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/release.rst` & `libonvif-2.0.9/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/docs/upgrade.rst` & `libonvif-2.0.9/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/attr.h` & `libonvif-2.0.9/pybind11/include/pybind11/attr.h`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 
 /// Annotation for methods
 struct is_method {
     handle class_;
     explicit is_method(const handle &c) : class_(c) {}
 };
 
-/// Annotation for setters
-struct is_setter {};
-
 /// Annotation for operators
 struct is_operator {};
 
 /// Annotation for classes that cannot be subclassed
 struct is_final {};
 
 /// Annotation for parent scope
@@ -187,16 +184,16 @@
 };
 
 /// Internal data structure which holds metadata about a bound function (signature, overloads,
 /// etc.)
 struct function_record {
     function_record()
         : is_constructor(false), is_new_style_constructor(false), is_stateless(false),
-          is_operator(false), is_method(false), is_setter(false), has_args(false),
-          has_kwargs(false), prepend(false) {}
+          is_operator(false), is_method(false), has_args(false), has_kwargs(false),
+          prepend(false) {}
 
     /// Function name
     char *name = nullptr; /* why no C++ strings? They generate heavier code.. */
 
     // User-specified documentation string
     char *doc = nullptr;
 
@@ -229,17 +226,14 @@
 
     /// True if this is an operator (__add__), etc.
     bool is_operator : 1;
 
     /// True if this is a method
     bool is_method : 1;
 
-    /// True if this is a setter
-    bool is_setter : 1;
-
     /// True if the function has a '*args' argument
     bool has_args : 1;
 
     /// True if the function has a '**kwargs' argument
     bool has_kwargs : 1;
 
     /// True if this function is to be inserted at the beginning of the overload resolution chain
@@ -428,20 +422,14 @@
 struct process_attribute<is_method> : process_attribute_default<is_method> {
     static void init(const is_method &s, function_record *r) {
         r->is_method = true;
         r->scope = s.class_;
     }
 };
 
-/// Process an attribute which indicates that this function is a setter
-template <>
-struct process_attribute<is_setter> : process_attribute_default<is_setter> {
-    static void init(const is_setter &, function_record *r) { r->is_setter = true; }
-};
-
 /// Process an attribute which indicates the parent scope of a method
 template <>
 struct process_attribute<scope> : process_attribute_default<scope> {
     static void init(const scope &s, function_record *r) { r->scope = s.value; }
 };
 
 /// Process an attribute which indicates that this function is an operator
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/buffer_info.h` & `libonvif-2.0.9/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/cast.h` & `libonvif-2.0.9/pybind11/include/pybind11/cast.h`

 * *Files 2% similar despite different names*

```diff
@@ -960,26 +960,26 @@
 struct move_always : std::false_type {};
 template <typename T>
 struct move_always<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<is_copy_constructible<T>>,
-               is_move_constructible<T>,
+               std::is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T, typename SFINAE = void>
 struct move_if_unreferenced : std::false_type {};
 template <typename T>
 struct move_if_unreferenced<
     T,
     enable_if_t<
         all_of<move_is_plain_type<T>,
                negation<move_always<T>>,
-               is_move_constructible<T>,
+               std::is_move_constructible<T>,
                std::is_same<decltype(std::declval<make_caster<T>>().operator T &()), T &>>::value>>
     : std::true_type {};
 template <typename T>
 using move_never = none_of<move_always<T>, move_if_unreferenced<T>>;
 
 // Detect whether returning a `type` from a cast on type's type_caster is going to result in a
 // reference or pointer to a local variable of the type_caster.  Basically, only
@@ -1037,60 +1037,28 @@
     load_type(conv, handle);
     return conv;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 // pytype -> C++ type
-template <typename T,
-          detail::enable_if_t<!detail::is_pyobject<T>::value
-                                  && !detail::is_same_ignoring_cvref<T, PyObject *>::value,
-                              int>
-          = 0>
+template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
 T cast(const handle &handle) {
     using namespace detail;
     static_assert(!cast_is_temporary_value_reference<T>::value,
                   "Unable to cast type to reference: value is local to type caster");
     return cast_op<T>(load_type<T>(handle));
 }
 
 // pytype -> pytype (calls converting constructor)
 template <typename T, detail::enable_if_t<detail::is_pyobject<T>::value, int> = 0>
 T cast(const handle &handle) {
     return T(reinterpret_borrow<object>(handle));
 }
 
-// Note that `cast<PyObject *>(obj)` increments the reference count of `obj`.
-// This is necessary for the case that `obj` is a temporary, and could
-// not possibly be different, given
-// 1. the established convention that the passed `handle` is borrowed, and
-// 2. we don't want to force all generic code using `cast<T>()` to special-case
-//    handling of `T` = `PyObject *` (to increment the reference count there).
-// It is the responsibility of the caller to ensure that the reference count
-// is decremented.
-template <typename T,
-          typename Handle,
-          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
-                                  && detail::is_same_ignoring_cvref<Handle, handle>::value,
-                              int>
-          = 0>
-T cast(Handle &&handle) {
-    return handle.inc_ref().ptr();
-}
-// To optimize way an inc_ref/dec_ref cycle:
-template <typename T,
-          typename Object,
-          detail::enable_if_t<detail::is_same_ignoring_cvref<T, PyObject *>::value
-                                  && detail::is_same_ignoring_cvref<Object, object>::value,
-                              int>
-          = 0>
-T cast(Object &&obj) {
-    return obj.release().ptr();
-}
-
 // C++ type -> py::object
 template <typename T, detail::enable_if_t<!detail::is_pyobject<T>::value, int> = 0>
 object cast(T &&value,
             return_value_policy policy = return_value_policy::automatic_reference,
             handle parent = handle()) {
     using no_ref_T = typename std::remove_reference<T>::type;
     if (policy == return_value_policy::automatic) {
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/chrono.h` & `libonvif-2.0.9/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/complex.h` & `libonvif-2.0.9/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/class.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/common.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/common.h`

 * *Files 0% similar despite different names*

```diff
@@ -657,18 +657,14 @@
 struct remove_cvref {
     using type = remove_cv_t<remove_reference_t<T>>;
 };
 template <class T>
 using remove_cvref_t = typename remove_cvref<T>::type;
 #endif
 
-/// Example usage: is_same_ignoring_cvref<T, PyObject *>::value
-template <typename T, typename U>
-using is_same_ignoring_cvref = std::is_same<detail::remove_cvref_t<T>, U>;
-
 /// Index sequences
 #if defined(PYBIND11_CPP14)
 using std::index_sequence;
 using std::make_index_sequence;
 #else
 template <size_t...>
 struct index_sequence {};
@@ -754,24 +750,15 @@
 struct remove_class<R (C::*)(A...)> {
     using type = R(A...);
 };
 template <typename C, typename R, typename... A>
 struct remove_class<R (C::*)(A...) const> {
     using type = R(A...);
 };
-#ifdef __cpp_noexcept_function_type
-template <typename C, typename R, typename... A>
-struct remove_class<R (C::*)(A...) noexcept> {
-    using type = R(A...);
-};
-template <typename C, typename R, typename... A>
-struct remove_class<R (C::*)(A...) const noexcept> {
-    using type = R(A...);
-};
-#endif
+
 /// Helper template to strip away type modifiers
 template <typename T>
 struct intrinsic_type {
     using type = T;
 };
 template <typename T>
 struct intrinsic_type<const T> {
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/descr.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/descr.h`

 * *Files 4% similar despite different names*

```diff
@@ -139,32 +139,19 @@
 constexpr descr<0> concat() { return {}; }
 
 template <size_t N, typename... Ts>
 constexpr descr<N, Ts...> concat(const descr<N, Ts...> &descr) {
     return descr;
 }
 
-#ifdef __cpp_fold_expressions
-template <size_t N1, size_t N2, typename... Ts1, typename... Ts2>
-constexpr descr<N1 + N2 + 2, Ts1..., Ts2...> operator,(const descr<N1, Ts1...> &a,
-                                                       const descr<N2, Ts2...> &b) {
-    return a + const_name(", ") + b;
-}
-
-template <size_t N, typename... Ts, typename... Args>
-constexpr auto concat(const descr<N, Ts...> &d, const Args &...args) {
-    return (d, ..., args);
-}
-#else
 template <size_t N, typename... Ts, typename... Args>
 constexpr auto concat(const descr<N, Ts...> &d, const Args &...args)
     -> decltype(std::declval<descr<N + 2, Ts...>>() + concat(args...)) {
     return d + const_name(", ") + concat(args...);
 }
-#endif
 
 template <size_t N, typename... Ts>
 constexpr descr<N + 2, Ts...> type_descr(const descr<N, Ts...> &descr) {
     return const_name("{") + descr + const_name("}");
 }
 
 PYBIND11_NAMESPACE_END(detail)
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/init.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/init.h`

 * *Files 0% similar despite different names*

```diff
@@ -171,30 +171,30 @@
 // return-by-value version 1: returning a cpp class by value.  If the class has an alias and an
 // alias is required the alias must have an `Alias(Cpp &&)` constructor so that we can construct
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
     PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
-    static_assert(is_move_constructible<Cpp<Class>>::value,
+    static_assert(std::is_move_constructible<Cpp<Class>>::value,
                   "pybind11::init() return-by-value factory function requires a movable class");
     if (Class::has_alias && need_alias) {
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
     } else {
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
     }
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
 // Alias instance (even if no the python-side inheritance is involved).  The is intended for
 // cases where Alias initialization is always desired.
 template <typename Class>
 void construct(value_and_holder &v_h, Alias<Class> &&result, bool) {
     static_assert(
-        is_move_constructible<Alias<Class>>::value,
+        std::is_move_constructible<Alias<Class>>::value,
         "pybind11::init() return-by-alias-value factory function requires a movable alias class");
     v_h.value_ptr() = new Alias<Class>(std::move(result));
 }
 
 // Implementing class for py::init<...>()
 template <typename... Args>
 struct constructor {
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/internals.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/internals.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,17 @@
 /// newer ABI.
 ///
 /// WARNING: If you choose to manually increase the ABI version, note that
 /// pybind11 may not be tested as thoroughly with a non-default ABI version, and
 /// further ABI-incompatible changes may be made before the ABI is officially
 /// changed to the new version.
 #ifndef PYBIND11_INTERNALS_VERSION
-#    if PY_VERSION_HEX >= 0x030C0000
-// Version bump for Python 3.12+, before first 3.12 beta release.
-#        define PYBIND11_INTERNALS_VERSION 5
-#    else
-#        define PYBIND11_INTERNALS_VERSION 4
-#    endif
+#    define PYBIND11_INTERNALS_VERSION 4
 #endif
 
-// This requirement is mainly to reduce the support burden (see PR #4570).
-static_assert(PY_VERSION_HEX < 0x030C0000 || PYBIND11_INTERNALS_VERSION >= 5,
-              "pybind11 ABI version 5 is the minimum for Python 3.12+");
-
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ExceptionTranslator = void (*)(std::exception_ptr);
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 constexpr const char *internals_function_record_capsule_name = "pybind11_function_record_capsule";
@@ -119,16 +110,15 @@
 
 // Python loads modules by default with dlopen with the RTLD_LOCAL flag; under libc++ and possibly
 // other STLs, this means `typeid(A)` from one module won't equal `typeid(A)` from another module
 // even when `A` is the same, non-hidden-visibility type (e.g. from a common include).  Under
 // libstdc++, this doesn't happen: equality and the type_index hash are based on the type name,
 // which works.  If not under a known-good stl, provide our own name-based hash and equality
 // functions that use the type name.
-#if (PYBIND11_INTERNALS_VERSION <= 4 && defined(__GLIBCXX__))                                     \
-    || (PYBIND11_INTERNALS_VERSION >= 5 && !defined(_LIBCPP_VERSION))
+#if defined(__GLIBCXX__)
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) { return lhs == rhs; }
 using type_hash = std::hash<std::type_index>;
 using type_equal_to = std::equal_to<std::type_index>;
 #else
 inline bool same_type(const std::type_info &lhs, const std::type_info &rhs) {
     return lhs.name() == rhs.name() || std::strcmp(lhs.name(), rhs.name()) == 0;
 }
@@ -427,46 +417,14 @@
     } catch (const builtin_exception &e) {
         e.set_error();
         return;
     }
 }
 #endif
 
-inline object get_python_state_dict() {
-    object state_dict;
-#if PYBIND11_INTERNALS_VERSION <= 4 || PY_VERSION_HEX < 0x03080000 || defined(PYPY_VERSION)
-    state_dict = reinterpret_borrow<object>(PyEval_GetBuiltins());
-#else
-#    if PY_VERSION_HEX < 0x03090000
-    PyInterpreterState *istate = _PyInterpreterState_Get();
-#    else
-    PyInterpreterState *istate = PyInterpreterState_Get();
-#    endif
-    if (istate) {
-        state_dict = reinterpret_borrow<object>(PyInterpreterState_GetDict(istate));
-    }
-#endif
-    if (!state_dict) {
-        raise_from(PyExc_SystemError, "pybind11::detail::get_python_state_dict() FAILED");
-    }
-    return state_dict;
-}
-
-inline object get_internals_obj_from_state_dict(handle state_dict) {
-    return reinterpret_borrow<object>(dict_getitemstring(state_dict.ptr(), PYBIND11_INTERNALS_ID));
-}
-
-inline internals **get_internals_pp_from_capsule(handle obj) {
-    void *raw_ptr = PyCapsule_GetPointer(obj.ptr(), /*name=*/nullptr);
-    if (raw_ptr == nullptr) {
-        raise_from(PyExc_SystemError, "pybind11::detail::get_internals_pp_from_capsule() FAILED");
-    }
-    return static_cast<internals **>(raw_ptr);
-}
-
 /// Return a reference to the current `internals` data
 PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
     if (internals_pp && *internals_pp) {
         return **internals_pp;
     }
 
@@ -483,20 +441,20 @@
         ~gil_scoped_acquire_local() { PyGILState_Release(state); }
         const PyGILState_STATE state;
     } gil;
 #    endif
 #endif
     error_scope err_scope;
 
-    dict state_dict = get_python_state_dict();
-    if (object internals_obj = get_internals_obj_from_state_dict(state_dict)) {
-        internals_pp = get_internals_pp_from_capsule(internals_obj);
-    }
-    if (internals_pp && *internals_pp) {
-        // We loaded the internals through `state_dict`, which means that our `error_already_set`
+    PYBIND11_STR_TYPE id(PYBIND11_INTERNALS_ID);
+    auto builtins = handle(PyEval_GetBuiltins());
+    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
+        internals_pp = static_cast<internals **>(capsule(builtins[id]));
+
+        // We loaded builtins through python's builtins, which means that our `error_already_set`
         // and `builtin_exception` may be different local classes than the ones set up in the
         // initial exception translator, below, so add another for our local exception classes.
         //
         // libstdc++ doesn't require this (types there are identified only by name)
         // libc++ with CPython doesn't require this (types are explicitly exported)
         // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
@@ -522,15 +480,15 @@
         if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->loader_life_support_tls_key)) {
             pybind11_fail("get_internals: could not successfully initialize the "
                           "loader_life_support TSS key!");
         }
 #    endif
         internals_ptr->istate = tstate->interp;
 #endif
-        state_dict[PYBIND11_INTERNALS_ID] = capsule(internals_pp);
+        builtins[id] = capsule(internals_pp);
         internals_ptr->registered_exception_translators.push_front(&translate_exception);
         internals_ptr->static_property_type = make_static_property_type();
         internals_ptr->default_metaclass = make_default_metaclass();
         internals_ptr->instance_base = make_object_base_type(internals_ptr->default_metaclass);
     }
     return **internals_pp;
 }
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/type_caster_base.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files 7% similar despite different names*

```diff
@@ -254,17 +254,17 @@
     instance *inst = nullptr;
     size_t index = 0u;
     const detail::type_info *type = nullptr;
     void **vh = nullptr;
 
     // Main constructor for a found value/holder:
     value_and_holder(instance *i, const detail::type_info *type, size_t vpos, size_t index)
-        : inst{i}, index{index}, type{type},
-          vh{inst->simple_layout ? inst->simple_value_holder
-                                 : &inst->nonsimple.values_and_holders[vpos]} {}
+        : inst{i}, index{index}, type{type}, vh{inst->simple_layout
+                                                    ? inst->simple_value_holder
+                                                    : &inst->nonsimple.values_and_holders[vpos]} {}
 
     // Default constructor (used to signal a value-and-holder not found by get_value_and_holder())
     value_and_holder() = default;
 
     // Used for past-the-end iterator
     explicit value_and_holder(size_t index) : index{index} {}
 
@@ -818,207 +818,49 @@
 using movable_cast_op_type
     = conditional_t<std::is_pointer<typename std::remove_reference<T>::type>::value,
                     typename std::add_pointer<intrinsic_t<T>>::type,
                     conditional_t<std::is_rvalue_reference<T>::value,
                                   typename std::add_rvalue_reference<intrinsic_t<T>>::type,
                                   typename std::add_lvalue_reference<intrinsic_t<T>>::type>>;
 
-// Does the container have a mapped type and is it recursive?
-// Implemented by specializations below.
-template <typename Container, typename SFINAE = void>
-struct container_mapped_type_traits {
-    static constexpr bool has_mapped_type = false;
-    static constexpr bool has_recursive_mapped_type = false;
-};
-
-template <typename Container>
-struct container_mapped_type_traits<
-    Container,
-    typename std::enable_if<
-        std::is_same<typename Container::mapped_type, Container>::value>::type> {
-    static constexpr bool has_mapped_type = true;
-    static constexpr bool has_recursive_mapped_type = true;
-};
-
-template <typename Container>
-struct container_mapped_type_traits<
-    Container,
-    typename std::enable_if<
-        negation<std::is_same<typename Container::mapped_type, Container>>::value>::type> {
-    static constexpr bool has_mapped_type = true;
-    static constexpr bool has_recursive_mapped_type = false;
-};
-
-// Does the container have a value type and is it recursive?
-// Implemented by specializations below.
-template <typename Container, typename SFINAE = void>
-struct container_value_type_traits : std::false_type {
-    static constexpr bool has_value_type = false;
-    static constexpr bool has_recursive_value_type = false;
-};
-
-template <typename Container>
-struct container_value_type_traits<
-    Container,
-    typename std::enable_if<
-        std::is_same<typename Container::value_type, Container>::value>::type> {
-    static constexpr bool has_value_type = true;
-    static constexpr bool has_recursive_value_type = true;
-};
-
-template <typename Container>
-struct container_value_type_traits<
-    Container,
-    typename std::enable_if<
-        negation<std::is_same<typename Container::value_type, Container>>::value>::type> {
-    static constexpr bool has_value_type = true;
-    static constexpr bool has_recursive_value_type = false;
-};
-
-/*
- * Tag to be used for representing the bottom of recursively defined types.
- * Define this tag so we don't have to use void.
- */
-struct recursive_bottom {};
-
-/*
- * Implementation detail of `recursive_container_traits` below.
- * `T` is the `value_type` of the container, which might need to be modified to
- * avoid recursive types and const types.
- */
-template <typename T, bool is_this_a_map>
-struct impl_type_to_check_recursively {
-    /*
-     * If the container is recursive, then no further recursion should be done.
-     */
-    using if_recursive = recursive_bottom;
-    /*
-     * Otherwise yield `T` unchanged.
-     */
-    using if_not_recursive = T;
-};
-
-/*
- * For pairs - only as value type of a map -, the first type should remove the `const`.
- * Also, if the map is recursive, then the recursive checking should consider
- * the first type only.
- */
-template <typename A, typename B>
-struct impl_type_to_check_recursively<std::pair<A, B>, /* is_this_a_map = */ true> {
-    using if_recursive = typename std::remove_const<A>::type;
-    using if_not_recursive = std::pair<typename std::remove_const<A>::type, B>;
-};
-
-/*
- * Implementation of `recursive_container_traits` below.
- */
-template <typename Container, typename SFINAE = void>
-struct impl_recursive_container_traits {
-    using type_to_check_recursively = recursive_bottom;
-};
-
-template <typename Container>
-struct impl_recursive_container_traits<
-    Container,
-    typename std::enable_if<container_value_type_traits<Container>::has_value_type>::type> {
-    static constexpr bool is_recursive
-        = container_mapped_type_traits<Container>::has_recursive_mapped_type
-          || container_value_type_traits<Container>::has_recursive_value_type;
-    /*
-     * This member dictates which type Pybind11 should check recursively in traits
-     * such as `is_move_constructible`, `is_copy_constructible`, `is_move_assignable`, ...
-     * Direct access to `value_type` should be avoided:
-     * 1. `value_type` might recursively contain the type again
-     * 2. `value_type` of STL map types is `std::pair<A const, B>`, the `const`
-     *    should be removed.
-     *
-     */
-    using type_to_check_recursively = typename std::conditional<
-        is_recursive,
-        typename impl_type_to_check_recursively<
-            typename Container::value_type,
-            container_mapped_type_traits<Container>::has_mapped_type>::if_recursive,
-        typename impl_type_to_check_recursively<
-            typename Container::value_type,
-            container_mapped_type_traits<Container>::has_mapped_type>::if_not_recursive>::type;
-};
-
-/*
- * This trait defines the `type_to_check_recursively` which is needed to properly
- * handle recursively defined traits such as `is_move_constructible` without going
- * into an infinite recursion.
- * Should be used instead of directly accessing the `value_type`.
- * It cancels the recursion by returning the `recursive_bottom` tag.
- *
- * The default definition of `type_to_check_recursively` is as follows:
- *
- * 1. By default, it is `recursive_bottom`, so that the recursion is canceled.
- * 2. If the type is non-recursive and defines a `value_type`, then the `value_type` is used.
- *    If the `value_type` is a pair and a `mapped_type` is defined,
- *    then the `const` is removed from the first type.
- * 3. If the type is recursive and `value_type` is not a pair, then `recursive_bottom` is returned.
- * 4. If the type is recursive and `value_type` is a pair and a `mapped_type` is defined,
- *    then `const` is removed from the first type and the first type is returned.
- *
- * This behavior can be extended by the user as seen in test_stl_binders.cpp.
- *
- * This struct is exactly the same as impl_recursive_container_traits.
- * The duplication achieves that user-defined specializations don't compete
- * with internal specializations, but take precedence.
- */
-template <typename Container, typename SFINAE = void>
-struct recursive_container_traits : impl_recursive_container_traits<Container> {};
-
-template <typename T>
-struct is_move_constructible
-    : all_of<std::is_move_constructible<T>,
-             is_move_constructible<
-                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
-
-template <>
-struct is_move_constructible<recursive_bottom> : std::true_type {};
-
-// Likewise for std::pair
-// (after C++17 it is mandatory that the move constructor not exist when the two types aren't
-// themselves move constructible, but this can not be relied upon when T1 or T2 are themselves
-// containers).
-template <typename T1, typename T2>
-struct is_move_constructible<std::pair<T1, T2>>
-    : all_of<is_move_constructible<T1>, is_move_constructible<T2>> {};
-
 // std::is_copy_constructible isn't quite enough: it lets std::vector<T> (and similar) through when
 // T is non-copyable, but code containing such a copy constructor fails to actually compile.
-template <typename T>
-struct is_copy_constructible
-    : all_of<std::is_copy_constructible<T>,
-             is_copy_constructible<
-                 typename recursive_container_traits<T>::type_to_check_recursively>> {};
+template <typename T, typename SFINAE = void>
+struct is_copy_constructible : std::is_copy_constructible<T> {};
 
-template <>
-struct is_copy_constructible<recursive_bottom> : std::true_type {};
+// Specialization for types that appear to be copy constructible but also look like stl containers
+// (we specifically check for: has `value_type` and `reference` with `reference = value_type&`): if
+// so, copy constructability depends on whether the value_type is copy constructible.
+template <typename Container>
+struct is_copy_constructible<
+    Container,
+    enable_if_t<
+        all_of<std::is_copy_constructible<Container>,
+               std::is_same<typename Container::value_type &, typename Container::reference>,
+               // Avoid infinite recursion
+               negation<std::is_same<Container, typename Container::value_type>>>::value>>
+    : is_copy_constructible<typename Container::value_type> {};
 
 // Likewise for std::pair
 // (after C++17 it is mandatory that the copy constructor not exist when the two types aren't
 // themselves copy constructible, but this can not be relied upon when T1 or T2 are themselves
 // containers).
 template <typename T1, typename T2>
 struct is_copy_constructible<std::pair<T1, T2>>
     : all_of<is_copy_constructible<T1>, is_copy_constructible<T2>> {};
 
 // The same problems arise with std::is_copy_assignable, so we use the same workaround.
-template <typename T>
-struct is_copy_assignable
-    : all_of<
-          std::is_copy_assignable<T>,
-          is_copy_assignable<typename recursive_container_traits<T>::type_to_check_recursively>> {
-};
-
-template <>
-struct is_copy_assignable<recursive_bottom> : std::true_type {};
-
+template <typename T, typename SFINAE = void>
+struct is_copy_assignable : std::is_copy_assignable<T> {};
+template <typename Container>
+struct is_copy_assignable<Container,
+                          enable_if_t<all_of<std::is_copy_assignable<Container>,
+                                             std::is_same<typename Container::value_type &,
+                                                          typename Container::reference>>::value>>
+    : is_copy_assignable<typename Container::value_type> {};
 template <typename T1, typename T2>
 struct is_copy_assignable<std::pair<T1, T2>>
     : all_of<is_copy_assignable<T1>, is_copy_assignable<T2>> {};
 
 PYBIND11_NAMESPACE_END(detail)
 
 // polymorphic_type_hook<itype>::get(src, tinfo) determines whether the object pointed
@@ -1148,15 +990,15 @@
        decltype argument to apply SFINAE to the public copy/move constructors.*/
     template <typename T, typename = enable_if_t<is_copy_constructible<T>::value>>
     static auto make_copy_constructor(const T *)
         -> decltype(new T(std::declval<const T>()), Constructor{}) {
         return [](const void *arg) -> void * { return new T(*reinterpret_cast<const T *>(arg)); };
     }
 
-    template <typename T, typename = enable_if_t<is_move_constructible<T>::value>>
+    template <typename T, typename = enable_if_t<std::is_move_constructible<T>::value>>
     static auto make_move_constructor(const T *)
         -> decltype(new T(std::declval<T &&>()), Constructor{}) {
         return [](const void *arg) -> void * {
             return new T(std::move(*const_cast<T *>(reinterpret_cast<const T *>(arg))));
         };
     }
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/detail/typeid.h` & `libonvif-2.0.9/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/eigen/matrix.h` & `libonvif-2.0.9/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/eigen/tensor.h` & `libonvif-2.0.9/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/embed.h` & `libonvif-2.0.9/pybind11/include/pybind11/embed.h`

 * *Files 2% similar despite different names*

```diff
@@ -239,22 +239,24 @@
         itself cannot completely unload binary extension modules and there are several
         caveats with regard to interpreter restarting. All the details can be found
         in the CPython documentation. In short, not all interpreter memory may be
         freed, either due to reference cycles or user-created global data.
 
  \endrst */
 inline void finalize_interpreter() {
+    handle builtins(PyEval_GetBuiltins());
+    const char *id = PYBIND11_INTERNALS_ID;
+
     // Get the internals pointer (without creating it if it doesn't exist).  It's possible for the
     // internals to be created during Py_Finalize() (e.g. if a py::capsule calls `get_internals()`
     // during destruction), so we get the pointer-pointer here and check it after Py_Finalize().
     detail::internals **internals_ptr_ptr = detail::get_internals_pp();
-    // It could also be stashed in state_dict, so look there too:
-    if (object internals_obj
-        = get_internals_obj_from_state_dict(detail::get_python_state_dict())) {
-        internals_ptr_ptr = detail::get_internals_pp_from_capsule(internals_obj);
+    // It could also be stashed in builtins, so look there too:
+    if (builtins.contains(id) && isinstance<capsule>(builtins[id])) {
+        internals_ptr_ptr = capsule(builtins[id]);
     }
     // Local internals contains data managed by the current interpreter, so we must clear them to
     // avoid undefined behaviors when initializing another interpreter
     detail::get_local_internals().registered_types_cpp.clear();
     detail::get_local_internals().registered_exception_translators.clear();
 
     Py_Finalize();
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/eval.h` & `libonvif-2.0.9/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/functional.h` & `libonvif-2.0.9/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/gil.h` & `libonvif-2.0.9/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/iostream.h` & `libonvif-2.0.9/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/numpy.h` & `libonvif-2.0.9/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/operators.h` & `libonvif-2.0.9/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/options.h` & `libonvif-2.0.9/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/pybind11.h` & `libonvif-2.0.9/pybind11/include/pybind11/pybind11.h`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(std::nullptr_t) {}
-    cpp_function(std::nullptr_t, const is_setter &) {}
 
     /// Construct a cpp_function from a vanilla function pointer
     template <typename Return, typename... Args, typename... Extra>
     // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (*f)(Args...), const Extra &...extra) {
         initialize(f, f, extra...);
     }
@@ -241,24 +240,18 @@
             return_value_policy policy
                 = return_value_policy_override<Return>::policy(call.func.policy);
 
             /* Function scope guard -- defaults to the compile-to-nothing `void_type` */
             using Guard = extract_guard_t<Extra...>;
 
             /* Perform the function call */
-            handle result;
-            if (call.func.is_setter) {
-                (void) std::move(args_converter).template call<Return, Guard>(cap->f);
-                result = none().release();
-            } else {
-                result = cast_out::cast(
-                    std::move(args_converter).template call<Return, Guard>(cap->f),
-                    policy,
-                    call.parent);
-            }
+            handle result
+                = cast_out::cast(std::move(args_converter).template call<Return, Guard>(cap->f),
+                                 policy,
+                                 call.parent);
 
             /* Invoke call policy post-call hook */
             process_attributes<Extra...>::postcall(call, result);
 
             return result;
         };
 
@@ -1732,16 +1725,15 @@
         return def_property_static(name, fget, nullptr, extra...);
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename Setter, typename... Extra>
     class_ &
     def_property(const char *name, const Getter &fget, const Setter &fset, const Extra &...extra) {
-        return def_property(
-            name, fget, cpp_function(method_adaptor<type>(fset), is_setter()), extra...);
+        return def_property(name, fget, cpp_function(method_adaptor<type>(fset)), extra...);
     }
     template <typename Getter, typename... Extra>
     class_ &def_property(const char *name,
                          const Getter &fget,
                          const cpp_function &fset,
                          const Extra &...extra) {
         return def_property(name,
```

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/pytypes.h` & `libonvif-2.0.9/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/stl/filesystem.h` & `libonvif-2.0.9/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/stl.h` & `libonvif-2.0.9/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/include/pybind11/stl_bind.h` & `libonvif-2.0.9/pybind11/include/pybind11/stl_bind.h`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,17 @@
     T,
     enable_if_t<container_traits<T>::is_element && container_traits<T>::is_comparable>>
     : std::true_type {};
 
 /* For a vector/map data structure, recursively check the value type
    (which is std::pair for maps) */
 template <typename T>
-struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>>
-    : is_comparable<typename recursive_container_traits<T>::type_to_check_recursively> {};
-
-template <>
-struct is_comparable<recursive_bottom> : std::true_type {};
+struct is_comparable<T, enable_if_t<container_traits<T>::is_vector>> {
+    static constexpr const bool value = is_comparable<typename T::value_type>::value;
+};
 
 /* For pairs, recursively check the two data types */
 template <typename T>
 struct is_comparable<T, enable_if_t<container_traits<T>::is_pair>> {
     static constexpr const bool value = is_comparable<typename T::first_type>::value
                                         && is_comparable<typename T::second_type>::value;
 };
```

### Comparing `libonvif-2.0.10/pybind11/noxfile.py` & `libonvif-2.0.9/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/pybind11/__main__.py` & `libonvif-2.0.9/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/pybind11/commands.py` & `libonvif-2.0.9/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/pybind11/setup_helpers.py` & `libonvif-2.0.9/pybind11/pybind11/setup_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,24 +140,29 @@
                     self.include_dirs.append(pyinc)
             except ModuleNotFoundError:
                 pass
 
         self.cxx_std = cxx_std
 
         cflags = []
+        ldflags = []
         if WIN:
             cflags += ["/EHsc", "/bigobj"]
         else:
             cflags += ["-fvisibility=hidden"]
             env_cflags = os.environ.get("CFLAGS", "")
             env_cppflags = os.environ.get("CPPFLAGS", "")
             c_cpp_flags = shlex.split(env_cflags) + shlex.split(env_cppflags)
             if not any(opt.startswith("-g") for opt in c_cpp_flags):
                 cflags += ["-g0"]
+            if MACOS:
+                cflags += ["-stdlib=libc++"]
+                ldflags += ["-stdlib=libc++"]
         self._add_cflags(cflags)
+        self._add_ldflags(ldflags)
 
     @property
     def cxx_std(self) -> int:
         """
         The CXX standard level. If set, will add the required flags. If left at
         0, it will trigger an automatic search when pybind11's build_ext is
         used. If None, will have no effect.  Besides just the flags, this may
```

### Comparing `libonvif-2.0.10/pybind11/pyproject.toml` & `libonvif-2.0.9/pybind11/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -89,8 +89,7 @@
 unfixable = ["T20"]
 exclude = []
 line-length = 120
 isort.known-first-party = ["env", "pybind11_cross_module_tests", "pybind11_tests"]
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["EM", "N"]
-"tests/test_call_policies.py" = ["PLC1901"]
```

### Comparing `libonvif-2.0.10/pybind11/setup.cfg` & `libonvif-2.0.9/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/setup.py` & `libonvif-2.0.9/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -150,19 +150,15 @@
     test_pytypes
     test_sequences_and_iterators
     test_smart_ptr
     test_stl
     test_stl_binders
     test_tagbased_polymorphic
     test_thread
-    test_type_caster_pyobject_ptr
     test_union
-    test_unnamed_namespace_a
-    test_unnamed_namespace_b
-    test_vector_unique_ptr_member
     test_virtual_functions)
 
 # Invoking cmake with something like:
 #     cmake -DPYBIND11_TEST_OVERRIDE="test_callbacks.cpp;test_pickling.cpp" ..
 # lets you override the tests that get compiled and run.  You can restore to all tests with:
 #     cmake -DPYBIND11_TEST_OVERRIDE= ..
 if(PYBIND11_TEST_OVERRIDE)
```

### Comparing `libonvif-2.0.10/pybind11/tests/conftest.py` & `libonvif-2.0.9/pybind11/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 Adds docstring and exceptions message sanitizers.
 """
 
 import contextlib
 import difflib
 import gc
 import multiprocessing
+import os
 import re
-import sys
 import textwrap
 import traceback
 
 import pytest
 
 # Early diagnostic for failed imports
 try:
@@ -21,24 +21,25 @@
 except Exception:
     # pytest does not show the traceback without this.
     traceback.print_exc()
     raise
 
 
 @pytest.fixture(scope="session", autouse=True)
-def use_multiprocessing_forkserver_on_linux():
-    if sys.platform != "linux":
-        # The default on Windows and macOS is "spawn": If it's not broken, don't fix it.
+def always_forkserver_on_unix():
+    if os.name == "nt":
         return
 
     # Full background: https://github.com/pybind/pybind11/issues/4105#issuecomment-1301004592
     # In a nutshell: fork() after starting threads == flakiness in the form of deadlocks.
     # It is actually a well-known pitfall, unfortunately without guard rails.
     # "forkserver" is more performant than "spawn" (~9s vs ~13s for tests/test_gil_scoped.py,
     # visit the issuecomment link above for details).
+    # Windows does not have fork() and the associated pitfall, therefore it is best left
+    # running with defaults.
     multiprocessing.set_start_method("forkserver")
 
 
 _long_marker = re.compile(r"([0-9])L")
 _hexadecimal = re.compile(r"0x[0-9a-fA-F]+")
 
 # Avoid collecting Python3 only files
```

### Comparing `libonvif-2.0.10/pybind11/tests/constructor_stats.h` & `libonvif-2.0.9/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/cross_module_gil_utils.cpp` & `libonvif-2.0.9/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `libonvif-2.0.9/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/env.py` & `libonvif-2.0.9/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/extra_python_package/test_files.py` & `libonvif-2.0.9/pybind11/tests/extra_python_package/test_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     "include/pybind11/numpy.h",
     "include/pybind11/operators.h",
     "include/pybind11/options.h",
     "include/pybind11/pybind11.h",
     "include/pybind11/pytypes.h",
     "include/pybind11/stl.h",
     "include/pybind11/stl_bind.h",
-    "include/pybind11/type_caster_pyobject_ptr.h",
 }
 
 detail_headers = {
     "include/pybind11/detail/class.h",
     "include/pybind11/detail/common.h",
     "include/pybind11/detail/descr.h",
     "include/pybind11/detail/init.h",
```

### Comparing `libonvif-2.0.10/pybind11/tests/extra_setuptools/test_setuphelper.py` & `libonvif-2.0.9/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/local_bindings.h` & `libonvif-2.0.9/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/object.h` & `libonvif-2.0.9/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/pybind11_cross_module_tests.cpp` & `libonvif-2.0.9/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/pybind11_tests.cpp` & `libonvif-2.0.9/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/pybind11_tests.h` & `libonvif-2.0.9/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/pytest.ini` & `libonvif-2.0.9/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/requirements.txt` & `libonvif-2.0.9/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_async.cpp` & `libonvif-2.0.9/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_async.py` & `libonvif-2.0.9/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_buffers.cpp` & `libonvif-2.0.9/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_buffers.py` & `libonvif-2.0.9/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_builtin_casters.cpp` & `libonvif-2.0.9/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_builtin_casters.py` & `libonvif-2.0.9/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_call_policies.cpp` & `libonvif-2.0.9/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_call_policies.py` & `libonvif-2.0.9/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_callbacks.cpp` & `libonvif-2.0.9/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_callbacks.py` & `libonvif-2.0.9/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_chrono.cpp` & `libonvif-2.0.9/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_chrono.py` & `libonvif-2.0.9/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_class.cpp` & `libonvif-2.0.9/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_class.py` & `libonvif-2.0.9/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/embed.cpp` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_const_name.cpp` & `libonvif-2.0.9/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_const_name.py` & `libonvif-2.0.9/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_constants_and_functions.cpp` & `libonvif-2.0.9/pybind11/tests/test_constants_and_functions.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -144,11 +144,8 @@
             "should_raise",
             [](int, int, const py::object &) { return 42; },
             "some docstring",
             py::arg_v("x", 42),
             py::arg_v("y", 42, "<the answer>"),
             py::arg_v("z", default_value));
     });
-
-    // test noexcept(true) lambda (#4565)
-    m.def("l1", []() noexcept(true) { return 0; });
 }
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_constants_and_functions.py` & `libonvif-2.0.9/pybind11/tests/test_constants_and_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,11 +46,7 @@
         def __repr__(self):
             raise RuntimeError("Surprise!")
 
     with pytest.raises(RuntimeError):
         m.register_large_capture_with_invalid_arguments(m)
     with pytest.raises(RuntimeError):
         m.register_with_raising_repr(m, RaisingRepr())
-
-
-def test_noexcept_lambda():
-    assert m.l1() == 0
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_copy_move.py` & `libonvif-2.0.9/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_custom_type_casters.cpp` & `libonvif-2.0.9/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_custom_type_casters.py` & `libonvif-2.0.9/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_custom_type_setup.cpp` & `libonvif-2.0.9/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_custom_type_setup.py` & `libonvif-2.0.9/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_docstring_options.cpp` & `libonvif-2.0.9/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_docstring_options.py` & `libonvif-2.0.9/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eigen_matrix.cpp` & `libonvif-2.0.9/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eigen_matrix.py` & `libonvif-2.0.9/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eigen_tensor.inl` & `libonvif-2.0.9/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eigen_tensor.py` & `libonvif-2.0.9/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_embed/CMakeLists.txt` & `libonvif-2.0.9/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_embed/catch.cpp` & `libonvif-2.0.9/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_embed/external_module.cpp` & `libonvif-2.0.9/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_embed/test_interpreter.cpp` & `libonvif-2.0.9/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -251,28 +251,28 @@
         py::scoped_interpreter scoped_interp{&config};
         REQUIRE(get_sys_path_size() == path_size_add_program_dir_to_path_false + 1);
     }
     py::initialize_interpreter();
 }
 #endif
 
-bool has_state_dict_internals_obj() {
-    return bool(
-        py::detail::get_internals_obj_from_state_dict(py::detail::get_python_state_dict()));
-}
+bool has_pybind11_internals_builtin() {
+    auto builtins = py::handle(PyEval_GetBuiltins());
+    return builtins.contains(PYBIND11_INTERNALS_ID);
+};
 
 bool has_pybind11_internals_static() {
     auto **&ipp = py::detail::get_internals_pp();
     return (ipp != nullptr) && (*ipp != nullptr);
 }
 
 TEST_CASE("Restart the interpreter") {
     // Verify pre-restart state.
     REQUIRE(py::module_::import("widget_module").attr("add")(1, 2).cast<int>() == 3);
-    REQUIRE(has_state_dict_internals_obj());
+    REQUIRE(has_pybind11_internals_builtin());
     REQUIRE(has_pybind11_internals_static());
     REQUIRE(py::module_::import("external_module").attr("A")(123).attr("value").cast<int>()
             == 123);
 
     // local and foreign module internals should point to the same internals:
     REQUIRE(reinterpret_cast<uintptr_t>(*py::detail::get_internals_pp())
             == py::module_::import("external_module").attr("internals_at")().cast<uintptr_t>());
@@ -281,39 +281,39 @@
     py::finalize_interpreter();
     REQUIRE(Py_IsInitialized() == 0);
 
     py::initialize_interpreter();
     REQUIRE(Py_IsInitialized() == 1);
 
     // Internals are deleted after a restart.
-    REQUIRE_FALSE(has_state_dict_internals_obj());
+    REQUIRE_FALSE(has_pybind11_internals_builtin());
     REQUIRE_FALSE(has_pybind11_internals_static());
     pybind11::detail::get_internals();
-    REQUIRE(has_state_dict_internals_obj());
+    REQUIRE(has_pybind11_internals_builtin());
     REQUIRE(has_pybind11_internals_static());
     REQUIRE(reinterpret_cast<uintptr_t>(*py::detail::get_internals_pp())
             == py::module_::import("external_module").attr("internals_at")().cast<uintptr_t>());
 
     // Make sure that an interpreter with no get_internals() created until finalize still gets the
     // internals destroyed
     py::finalize_interpreter();
     py::initialize_interpreter();
     bool ran = false;
     py::module_::import("__main__").attr("internals_destroy_test")
         = py::capsule(&ran, [](void *ran) {
               py::detail::get_internals();
               *static_cast<bool *>(ran) = true;
           });
-    REQUIRE_FALSE(has_state_dict_internals_obj());
+    REQUIRE_FALSE(has_pybind11_internals_builtin());
     REQUIRE_FALSE(has_pybind11_internals_static());
     REQUIRE_FALSE(ran);
     py::finalize_interpreter();
     REQUIRE(ran);
     py::initialize_interpreter();
-    REQUIRE_FALSE(has_state_dict_internals_obj());
+    REQUIRE_FALSE(has_pybind11_internals_builtin());
     REQUIRE_FALSE(has_pybind11_internals_static());
 
     // C++ modules can be reloaded.
     auto cpp_module = py::module_::import("widget_module");
     REQUIRE(cpp_module.attr("add")(1, 2).cast<int>() == 3);
 
     // C++ type information is reloaded and can be used in python modules.
@@ -327,25 +327,25 @@
     py::module_::import("__main__").attr("main_tag") = "main interpreter";
     {
         auto m = py::module_::import("widget_module");
         m.attr("extension_module_tag") = "added to module in main interpreter";
 
         REQUIRE(m.attr("add")(1, 2).cast<int>() == 3);
     }
-    REQUIRE(has_state_dict_internals_obj());
+    REQUIRE(has_pybind11_internals_builtin());
     REQUIRE(has_pybind11_internals_static());
 
     /// Create and switch to a subinterpreter.
     auto *main_tstate = PyThreadState_Get();
     auto *sub_tstate = Py_NewInterpreter();
 
     // Subinterpreters get their own copy of builtins. detail::get_internals() still
     // works by returning from the static variable, i.e. all interpreters share a single
     // global pybind11::internals;
-    REQUIRE_FALSE(has_state_dict_internals_obj());
+    REQUIRE_FALSE(has_pybind11_internals_builtin());
     REQUIRE(has_pybind11_internals_static());
 
     // Modules tags should be gone.
     REQUIRE_FALSE(py::hasattr(py::module_::import("__main__"), "tag"));
     {
         auto m = py::module_::import("widget_module");
         REQUIRE_FALSE(py::hasattr(m, "extension_module_tag"));
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_enum.cpp` & `libonvif-2.0.9/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_enum.py` & `libonvif-2.0.9/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eval.cpp` & `libonvif-2.0.9/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_eval.py` & `libonvif-2.0.9/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_exceptions.cpp` & `libonvif-2.0.9/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_exceptions.py` & `libonvif-2.0.9/pybind11/tests/test_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,19 +313,14 @@
     exc_type, exc_value, expected_what
 ):
     what, py_err_set_after_what = m.error_already_set_what(exc_type, exc_value)
     assert not py_err_set_after_what
     assert what == expected_what
 
 
-@pytest.mark.skipif(
-    # Intentionally very specific:
-    "sys.version_info == (3, 12, 0, 'alpha', 7)",
-    reason="WIP: https://github.com/python/cpython/issues/102594",
-)
 @pytest.mark.skipif("env.PYPY", reason="PyErr_NormalizeException Segmentation fault")
 def test_flaky_exception_failure_point_init():
     with pytest.raises(RuntimeError) as excinfo:
         m.error_already_set_what(FlakyException, ("failure_point_init",))
     lines = str(excinfo.value).splitlines()
     # PyErr_NormalizeException replaces the original FlakyException with ValueError:
     assert lines[:3] == [
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_factory_constructors.cpp` & `libonvif-2.0.9/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_factory_constructors.py` & `libonvif-2.0.9/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_gil_scoped.cpp` & `libonvif-2.0.9/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_gil_scoped.py` & `libonvif-2.0.9/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_iostream.cpp` & `libonvif-2.0.9/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_iostream.py` & `libonvif-2.0.9/pybind11/tests/test_iostream.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,134 +5,134 @@
 
 
 def test_captured(capsys):
     msg = "I've been redirected to Python, I hope!"
     m.captured_output(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
     m.captured_err(msg)
     stdout, stderr = capsys.readouterr()
-    assert not stdout
+    assert stdout == ""
     assert stderr == msg
 
 
 def test_captured_large_string(capsys):
     # Make this bigger than the buffer used on the C++ side: 1024 chars
     msg = "I've been redirected to Python, I hope!"
     msg = msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_2byte_offset0(capsys):
     msg = "\u07FF"
     msg = "" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_2byte_offset1(capsys):
     msg = "\u07FF"
     msg = "1" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_3byte_offset0(capsys):
     msg = "\uFFFF"
     msg = "" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_3byte_offset1(capsys):
     msg = "\uFFFF"
     msg = "1" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_3byte_offset2(capsys):
     msg = "\uFFFF"
     msg = "12" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_4byte_offset0(capsys):
     msg = "\U0010FFFF"
     msg = "" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_4byte_offset1(capsys):
     msg = "\U0010FFFF"
     msg = "1" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_4byte_offset2(capsys):
     msg = "\U0010FFFF"
     msg = "12" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_captured_utf8_4byte_offset3(capsys):
     msg = "\U0010FFFF"
     msg = "123" + msg * (1024 // len(msg) + 1)
 
     m.captured_output_default(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_guard_capture(capsys):
     msg = "I've been redirected to Python, I hope!"
     m.guard_output(msg)
     stdout, stderr = capsys.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
 
 
 def test_series_captured(capture):
     with capture:
         m.captured_output("a")
         m.captured_output("b")
     assert capture == "ab"
@@ -141,15 +141,15 @@
 def test_flush(capfd):
     msg = "(not flushed)"
     msg2 = "(flushed)"
 
     with m.ostream_redirect():
         m.noisy_function(msg, flush=False)
         stdout, stderr = capfd.readouterr()
-        assert not stdout
+        assert stdout == ""
 
         m.noisy_function(msg2, flush=True)
         stdout, stderr = capfd.readouterr()
         assert stdout == msg + msg2
 
         m.noisy_function(msg, flush=False)
 
@@ -160,42 +160,42 @@
 def test_not_captured(capfd):
     msg = "Something that should not show up in log"
     stream = StringIO()
     with redirect_stdout(stream):
         m.raw_output(msg)
     stdout, stderr = capfd.readouterr()
     assert stdout == msg
-    assert not stderr
-    assert not stream.getvalue()
+    assert stderr == ""
+    assert stream.getvalue() == ""
 
     stream = StringIO()
     with redirect_stdout(stream):
         m.captured_output(msg)
     stdout, stderr = capfd.readouterr()
-    assert not stdout
-    assert not stderr
+    assert stdout == ""
+    assert stderr == ""
     assert stream.getvalue() == msg
 
 
 def test_err(capfd):
     msg = "Something that should not show up in log"
     stream = StringIO()
     with redirect_stderr(stream):
         m.raw_err(msg)
     stdout, stderr = capfd.readouterr()
-    assert not stdout
+    assert stdout == ""
     assert stderr == msg
-    assert not stream.getvalue()
+    assert stream.getvalue() == ""
 
     stream = StringIO()
     with redirect_stderr(stream):
         m.captured_err(msg)
     stdout, stderr = capfd.readouterr()
-    assert not stdout
-    assert not stderr
+    assert stdout == ""
+    assert stderr == ""
     assert stream.getvalue() == msg
 
 
 def test_multi_captured(capfd):
     stream = StringIO()
     with redirect_stdout(stream):
         m.captured_output("a")
@@ -217,57 +217,57 @@
 def test_redirect(capfd):
     msg = "Should not be in log!"
     stream = StringIO()
     with redirect_stdout(stream):
         m.raw_output(msg)
     stdout, stderr = capfd.readouterr()
     assert stdout == msg
-    assert not stream.getvalue()
+    assert stream.getvalue() == ""
 
     stream = StringIO()
     with redirect_stdout(stream), m.ostream_redirect():
         m.raw_output(msg)
     stdout, stderr = capfd.readouterr()
-    assert not stdout
+    assert stdout == ""
     assert stream.getvalue() == msg
 
     stream = StringIO()
     with redirect_stdout(stream):
         m.raw_output(msg)
     stdout, stderr = capfd.readouterr()
     assert stdout == msg
-    assert not stream.getvalue()
+    assert stream.getvalue() == ""
 
 
 def test_redirect_err(capfd):
     msg = "StdOut"
     msg2 = "StdErr"
 
     stream = StringIO()
     with redirect_stderr(stream), m.ostream_redirect(stdout=False):
         m.raw_output(msg)
         m.raw_err(msg2)
     stdout, stderr = capfd.readouterr()
     assert stdout == msg
-    assert not stderr
+    assert stderr == ""
     assert stream.getvalue() == msg2
 
 
 def test_redirect_both(capfd):
     msg = "StdOut"
     msg2 = "StdErr"
 
     stream = StringIO()
     stream2 = StringIO()
     with redirect_stdout(stream), redirect_stderr(stream2), m.ostream_redirect():
         m.raw_output(msg)
         m.raw_err(msg2)
     stdout, stderr = capfd.readouterr()
-    assert not stdout
-    assert not stderr
+    assert stdout == ""
+    assert stderr == ""
     assert stream.getvalue() == msg
     assert stream2.getvalue() == msg2
 
 
 def test_threading():
     with m.ostream_redirect(stdout=True, stderr=False):
         # start some threads
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_kwargs_and_defaults.cpp` & `libonvif-2.0.9/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_kwargs_and_defaults.py` & `libonvif-2.0.9/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_local_bindings.cpp` & `libonvif-2.0.9/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_local_bindings.py` & `libonvif-2.0.9/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_methods_and_attributes.cpp` & `libonvif-2.0.9/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -173,46 +173,14 @@
 struct RValueRefParam {
     std::size_t func1(std::string &&s) { return s.size(); }
     std::size_t func2(std::string &&s) const { return s.size(); }
     std::size_t func3(std::string &&s) & { return s.size(); }
     std::size_t func4(std::string &&s) const & { return s.size(); }
 };
 
-namespace pybind11_tests {
-namespace exercise_is_setter {
-
-struct FieldBase {
-    int int_value() const { return int_value_; }
-
-    FieldBase &SetIntValue(int int_value) {
-        int_value_ = int_value;
-        return *this;
-    }
-
-private:
-    int int_value_ = -99;
-};
-
-struct Field : FieldBase {};
-
-void add_bindings(py::module &m) {
-    py::module sm = m.def_submodule("exercise_is_setter");
-    // NOTE: FieldBase is not wrapped, therefore ...
-    py::class_<Field>(sm, "Field")
-        .def(py::init<>())
-        .def_property(
-            "int_value",
-            &Field::int_value,
-            &Field::SetIntValue // ... the `FieldBase &` return value here cannot be converted.
-        );
-}
-
-} // namespace exercise_is_setter
-} // namespace pybind11_tests
-
 TEST_SUBMODULE(methods_and_attributes, m) {
     // test_methods_and_attributes
     py::class_<ExampleMandA> emna(m, "ExampleMandA");
     emna.def(py::init<>())
         .def(py::init<int>())
         .def(py::init<std::string &&>())
         .def(py::init<const ExampleMandA &>())
@@ -484,10 +452,8 @@
 
     py::class_<RValueRefParam>(m, "RValueRefParam")
         .def(py::init<>())
         .def("func1", &RValueRefParam::func1)
         .def("func2", &RValueRefParam::func2)
         .def("func3", &RValueRefParam::func3)
         .def("func4", &RValueRefParam::func4);
-
-    pybind11_tests::exercise_is_setter::add_bindings(m);
 }
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_methods_and_attributes.py` & `libonvif-2.0.9/pybind11/tests/test_methods_and_attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,16 +518,7 @@
 
 def test_rvalue_ref_param():
     r = m.RValueRefParam()
     assert r.func1("123") == 3
     assert r.func2("1234") == 4
     assert r.func3("12345") == 5
     assert r.func4("123456") == 6
-
-
-def test_is_setter():
-    fld = m.exercise_is_setter.Field()
-    assert fld.int_value == -99
-    setter_return = fld.int_value = 100
-    assert isinstance(setter_return, int)
-    assert setter_return == 100
-    assert fld.int_value == 100
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_modules.cpp` & `libonvif-2.0.9/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_modules.py` & `libonvif-2.0.9/pybind11/tests/test_modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 def test_importing():
     from collections import OrderedDict
 
     from pybind11_tests.modules import OD
 
     assert OD is OrderedDict
+    assert str(OD([(1, "a"), (2, "b")])) == "OrderedDict([(1, 'a'), (2, 'b')])"
 
 
 def test_pydoc():
     """Pydoc needs to be able to provide help() for everything inside a pybind11 module"""
     import pydoc
 
     import pybind11_tests
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_multiple_inheritance.cpp` & `libonvif-2.0.9/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_multiple_inheritance.py` & `libonvif-2.0.9/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_array.cpp` & `libonvif-2.0.9/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_array.py` & `libonvif-2.0.9/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_dtypes.cpp` & `libonvif-2.0.9/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_dtypes.py` & `libonvif-2.0.9/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_vectorize.cpp` & `libonvif-2.0.9/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_numpy_vectorize.py` & `libonvif-2.0.9/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_opaque_types.cpp` & `libonvif-2.0.9/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_opaque_types.py` & `libonvif-2.0.9/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_operator_overloading.cpp` & `libonvif-2.0.9/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_operator_overloading.py` & `libonvif-2.0.9/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_pickling.cpp` & `libonvif-2.0.9/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_pickling.py` & `libonvif-2.0.9/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_pytypes.cpp` & `libonvif-2.0.9/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_pytypes.py` & `libonvif-2.0.9/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_sequences_and_iterators.cpp` & `libonvif-2.0.9/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_sequences_and_iterators.py` & `libonvif-2.0.9/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_smart_ptr.cpp` & `libonvif-2.0.9/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_smart_ptr.py` & `libonvif-2.0.9/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_stl.cpp` & `libonvif-2.0.9/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_stl.py` & `libonvif-2.0.9/pybind11/tests/test_stl.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     assert m.array_cast_sequence((1, 2, 3)) == [1, 2, 3]
 
 
 def test_issue_1561():
     """check fix for issue #1561"""
     bar = m.Issue1561Outer()
     bar.list = [m.Issue1561Inner("bar")]
-    assert bar.list
+    bar.list
     assert bar.list[0].data == "bar"
 
 
 def test_return_vector_bool_raw_ptr():
     # Add `while True:` for manual leak checking.
     v = m.return_vector_bool_raw_ptr()
     assert isinstance(v, list)
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_stl_binders.cpp` & `libonvif-2.0.9/pybind11/tests/test_stl_binders.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -66,52 +66,14 @@
         for (int j = 1; j <= n; j++) {
             (*m)[i].emplace(int(j * 10), E_nc(100 * j));
         }
     }
     return m;
 }
 
-/*
- * Recursive data structures as test for issue #4623
- */
-struct RecursiveVector : std::vector<RecursiveVector> {
-    using Parent = std::vector<RecursiveVector>;
-    using Parent::Parent;
-};
-
-struct RecursiveMap : std::map<int, RecursiveMap> {
-    using Parent = std::map<int, RecursiveMap>;
-    using Parent::Parent;
-};
-
-/*
- * Pybind11 does not catch more complicated recursion schemes, such as mutual
- * recursion.
- * In that case custom recursive_container_traits specializations need to be added,
- * thus manually telling pybind11 about the recursion.
- */
-struct MutuallyRecursiveContainerPairMV;
-struct MutuallyRecursiveContainerPairVM;
-
-struct MutuallyRecursiveContainerPairMV : std::map<int, MutuallyRecursiveContainerPairVM> {};
-struct MutuallyRecursiveContainerPairVM : std::vector<MutuallyRecursiveContainerPairMV> {};
-
-namespace pybind11 {
-namespace detail {
-template <typename SFINAE>
-struct recursive_container_traits<MutuallyRecursiveContainerPairMV, SFINAE> {
-    using type_to_check_recursively = recursive_bottom;
-};
-template <typename SFINAE>
-struct recursive_container_traits<MutuallyRecursiveContainerPairVM, SFINAE> {
-    using type_to_check_recursively = recursive_bottom;
-};
-} // namespace detail
-} // namespace pybind11
-
 TEST_SUBMODULE(stl_binders, m) {
     // test_vector_int
     py::bind_vector<std::vector<unsigned int>>(m, "VectorInt", py::buffer_protocol());
 
     // test_vector_custom
     py::class_<El>(m, "El").def(py::init<int>());
     py::bind_vector<std::vector<El>>(m, "VectorEl");
@@ -163,20 +125,14 @@
         bool z;
     };
     m.def("create_undeclstruct", [m]() mutable {
         py::bind_vector<std::vector<VUndeclStruct>>(
             m, "VectorUndeclStruct", py::buffer_protocol());
     });
 
-    // Bind recursive container types
-    py::bind_vector<RecursiveVector>(m, "RecursiveVector");
-    py::bind_map<RecursiveMap>(m, "RecursiveMap");
-    py::bind_map<MutuallyRecursiveContainerPairMV>(m, "MutuallyRecursiveContainerPairMV");
-    py::bind_vector<MutuallyRecursiveContainerPairVM>(m, "MutuallyRecursiveContainerPairVM");
-
     // The rest depends on numpy:
     try {
         py::module_::import("numpy");
     } catch (...) {
         return;
     }
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_stl_binders.py` & `libonvif-2.0.9/pybind11/tests/test_stl_binders.py`

 * *Files 8% similar despite different names*

```diff
@@ -331,25 +331,7 @@
     assert type(map_string_double_const.values()) is values_type
     assert type(unordered_map_string_double_const.values()) is values_type
 
     items_type = type(map_string_double.items())
     assert type(unordered_map_string_double.items()) is items_type
     assert type(map_string_double_const.items()) is items_type
     assert type(unordered_map_string_double_const.items()) is items_type
-
-
-def test_recursive_vector():
-    recursive_vector = m.RecursiveVector()
-    recursive_vector.append(m.RecursiveVector())
-    recursive_vector[0].append(m.RecursiveVector())
-    recursive_vector[0].append(m.RecursiveVector())
-    # Can't use len() since test_stl_binders.cpp does not include stl.h,
-    # so the necessary conversion is missing
-    assert recursive_vector[0].count(m.RecursiveVector()) == 2
-
-
-def test_recursive_map():
-    recursive_map = m.RecursiveMap()
-    recursive_map[100] = m.RecursiveMap()
-    recursive_map[100][101] = m.RecursiveMap()
-    recursive_map[100][102] = m.RecursiveMap()
-    assert list(recursive_map[100].keys()) == [101, 102]
```

### Comparing `libonvif-2.0.10/pybind11/tests/test_tagbased_polymorphic.cpp` & `libonvif-2.0.9/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_tagbased_polymorphic.py` & `libonvif-2.0.9/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_thread.cpp` & `libonvif-2.0.9/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_thread.py` & `libonvif-2.0.9/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_union.cpp` & `libonvif-2.0.9/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_virtual_functions.cpp` & `libonvif-2.0.9/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/test_virtual_functions.py` & `libonvif-2.0.9/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/valgrind-numpy-scipy.supp` & `libonvif-2.0.9/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tests/valgrind-python.supp` & `libonvif-2.0.9/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/FindCatch.cmake` & `libonvif-2.0.9/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/FindEigen3.cmake` & `libonvif-2.0.9/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/FindPythonLibsNew.cmake` & `libonvif-2.0.9/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/JoinPaths.cmake` & `libonvif-2.0.9/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/check-style.sh` & `libonvif-2.0.9/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/cmake_uninstall.cmake.in` & `libonvif-2.0.9/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/codespell_ignore_lines_from_errors.py` & `libonvif-2.0.9/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/libsize.py` & `libonvif-2.0.9/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/make_changelog.py` & `libonvif-2.0.9/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/pybind11Common.cmake` & `libonvif-2.0.9/pybind11/tools/pybind11Common.cmake`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #[======================================================[.rst
 
 Adds the following targets::
 
     pybind11::pybind11 - link to headers and pybind11
     pybind11::module - Adds module links
     pybind11::embed - Adds embed links
-    pybind11::lto - Link time optimizations (only if CMAKE_INTERPROCEDURAL_OPTIMIZATION is not set)
-    pybind11::thin_lto - Link time optimizations (only if CMAKE_INTERPROCEDURAL_OPTIMIZATION is not set)
+    pybind11::lto - Link time optimizations (manual selection)
+    pybind11::thin_lto - Link time optimizations (manual selection)
     pybind11::python_link_helper - Adds link to Python libraries
     pybind11::windows_extras - MSVC bigobj and mp for building multithreaded
     pybind11::opt_size - avoid optimizations that increase code size
 
 Adds the following functions::
 
     pybind11_strip(target) - strip target after building on linux/macOS
     pybind11_find_import(module) - See if a module is installed.
 
 #]======================================================]
 
 # CMake 3.10 has an include_guard command, but we can't use that yet
 # include_guard(global) (pre-CMake 3.10)
-if(TARGET pybind11::pybind11)
+if(TARGET pybind11::lto)
   return()
 endif()
 
 # If we are in subdirectory mode, all IMPORTED targets must be GLOBAL. If we
 # are in CONFIG mode, they should be "normal" targets instead.
 # In CMake 3.11+ you can promote a target to global after you create it,
 # which might be simpler than this check.
@@ -368,21 +368,19 @@
         TARGET ${target}
         APPEND
         PROPERTY INTERFACE_LINK_OPTIONS "$<${not_debug}:${PYBIND11_LTO_LINKER_FLAGS}>")
     endif()
   endif()
 endfunction()
 
-if(NOT DEFINED CMAKE_INTERPROCEDURAL_OPTIMIZATION)
-  add_library(pybind11::lto IMPORTED INTERFACE ${optional_global})
-  _pybind11_generate_lto(pybind11::lto FALSE)
+add_library(pybind11::lto IMPORTED INTERFACE ${optional_global})
+_pybind11_generate_lto(pybind11::lto FALSE)
 
-  add_library(pybind11::thin_lto IMPORTED INTERFACE ${optional_global})
-  _pybind11_generate_lto(pybind11::thin_lto TRUE)
-endif()
+add_library(pybind11::thin_lto IMPORTED INTERFACE ${optional_global})
+_pybind11_generate_lto(pybind11::thin_lto TRUE)
 
 # ---------------------- pybind11_strip -----------------------------
 
 function(pybind11_strip target_name)
   # Strip unnecessary sections of the binary on Linux/macOS
   if(CMAKE_STRIP)
     if(APPLE)
```

### Comparing `libonvif-2.0.10/pybind11/tools/pybind11Config.cmake.in` & `libonvif-2.0.9/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/pybind11NewTools.cmake` & `libonvif-2.0.9/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/pybind11Tools.cmake` & `libonvif-2.0.9/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/setup_global.py.in` & `libonvif-2.0.9/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/pybind11/tools/setup_main.py.in` & `libonvif-2.0.9/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `libonvif-2.0.10/src/cencode.c` & `libonvif-2.0.9/src/cencode.c`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-/*
-cencoder.c - c source to a base64 encoding algorithm implementation
-
-This is part of the libb64 project, and has been placed in the public domain.
-For details, see http://sourceforge.net/projects/libb64
-
-**MODIFIED FOR LIBONVIF - remove trailing \n
-
-The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
-hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
-is in the public domain of the country from which the work is published, or (b) hereby dedicates 
-whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
-the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
-associated work, and for these purposes, is described as a "dedicator" below.
-
-A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
-recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
-is not in the public domain.
-
-Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
-Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
-in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
-Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
-rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
-
-Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
-transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
-non-commercial, and in any way, including by methods that have not yet been invented or conceived.
-
-CC0 for Public Domain Dedication
-This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
-to the public domain, we recommend CC0.
-*/
-
-#include "cencode.h"
-
-const int CHARS_PER_LINE = 72;
-
-void base64_init_encodestate(base64_encodestate* state_in)
-{
-	state_in->step = step_A;
-	state_in->result = 0;
-	state_in->stepcount = 0;
-}
-
-char base64_encode_value(char value_in)
-{
-	static const char* encoding = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/";
-	if (value_in > 63) return '=';
-	return encoding[(int)value_in];
-}
-
-int base64_encode_block(const char* plaintext_in, int length_in, char* code_out, base64_encodestate* state_in)
-{
-	const char* plainchar = plaintext_in;
-	const char* const plaintextend = plaintext_in + length_in;
-	char* codechar = code_out;
-	char result;
-	char fragment;
-
-	result = state_in->result;
-
-	switch (state_in->step)
-	{
-		while (1)
-		{
-	case step_A:
-			if (plainchar == plaintextend)
-			{
-				state_in->result = result;
-				state_in->step = step_A;
-				return codechar - code_out;
-			}
-			fragment = *plainchar++;
-			result = (fragment & 0x0fc) >> 2;
-			*codechar++ = base64_encode_value(result);
-			result = (fragment & 0x003) << 4;
-	case step_B:
-			if (plainchar == plaintextend)
-			{
-				state_in->result = result;
-				state_in->step = step_B;
-				return codechar - code_out;
-			}
-			fragment = *plainchar++;
-			result |= (fragment & 0x0f0) >> 4;
-			*codechar++ = base64_encode_value(result);
-			result = (fragment & 0x00f) << 2;
-	case step_C:
-			if (plainchar == plaintextend)
-			{
-				state_in->result = result;
-				state_in->step = step_C;
-				return codechar - code_out;
-			}
-			fragment = *plainchar++;
-			result |= (fragment & 0x0c0) >> 6;
-			*codechar++ = base64_encode_value(result);
-			result  = (fragment & 0x03f) >> 0;
-			*codechar++ = base64_encode_value(result);
-
-			++(state_in->stepcount);
-			if (state_in->stepcount == CHARS_PER_LINE/4)
-			{
-				//*codechar++ = '\n';
-				state_in->stepcount = 0;
-			}
-		}
-	}
-	/* control should not reach here */
-	return codechar - code_out;
-}
-
-int base64_encode_blockend(char* code_out, base64_encodestate* state_in)
-{
-	char* codechar = code_out;
-
-	switch (state_in->step)
-	{
-	case step_B:
-		*codechar++ = base64_encode_value(state_in->result);
-		*codechar++ = '=';
-		*codechar++ = '=';
-		break;
-	case step_C:
-		*codechar++ = base64_encode_value(state_in->result);
-		*codechar++ = '=';
-		break;
-	case step_A:
-		break;
-	}
-	//*codechar++ = '\n';
-
-	return codechar - code_out;
-}
+/*
+cencoder.c - c source to a base64 encoding algorithm implementation
+
+This is part of the libb64 project, and has been placed in the public domain.
+For details, see http://sourceforge.net/projects/libb64
+
+**MODIFIED FOR LIBONVIF - remove trailing \n
+
+The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
+hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
+is in the public domain of the country from which the work is published, or (b) hereby dedicates 
+whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
+the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
+associated work, and for these purposes, is described as a "dedicator" below.
+
+A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
+recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
+is not in the public domain.
+
+Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
+Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
+in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
+Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
+rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
+
+Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
+transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
+non-commercial, and in any way, including by methods that have not yet been invented or conceived.
+
+CC0 for Public Domain Dedication
+This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
+to the public domain, we recommend CC0.
+*/
+
+#include "cencode.h"
+
+const int CHARS_PER_LINE = 72;
+
+void base64_init_encodestate(base64_encodestate* state_in)
+{
+	state_in->step = step_A;
+	state_in->result = 0;
+	state_in->stepcount = 0;
+}
+
+char base64_encode_value(char value_in)
+{
+	static const char* encoding = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/";
+	if (value_in > 63) return '=';
+	return encoding[(int)value_in];
+}
+
+int base64_encode_block(const char* plaintext_in, int length_in, char* code_out, base64_encodestate* state_in)
+{
+	const char* plainchar = plaintext_in;
+	const char* const plaintextend = plaintext_in + length_in;
+	char* codechar = code_out;
+	char result;
+	char fragment;
+
+	result = state_in->result;
+
+	switch (state_in->step)
+	{
+		while (1)
+		{
+	case step_A:
+			if (plainchar == plaintextend)
+			{
+				state_in->result = result;
+				state_in->step = step_A;
+				return codechar - code_out;
+			}
+			fragment = *plainchar++;
+			result = (fragment & 0x0fc) >> 2;
+			*codechar++ = base64_encode_value(result);
+			result = (fragment & 0x003) << 4;
+	case step_B:
+			if (plainchar == plaintextend)
+			{
+				state_in->result = result;
+				state_in->step = step_B;
+				return codechar - code_out;
+			}
+			fragment = *plainchar++;
+			result |= (fragment & 0x0f0) >> 4;
+			*codechar++ = base64_encode_value(result);
+			result = (fragment & 0x00f) << 2;
+	case step_C:
+			if (plainchar == plaintextend)
+			{
+				state_in->result = result;
+				state_in->step = step_C;
+				return codechar - code_out;
+			}
+			fragment = *plainchar++;
+			result |= (fragment & 0x0c0) >> 6;
+			*codechar++ = base64_encode_value(result);
+			result  = (fragment & 0x03f) >> 0;
+			*codechar++ = base64_encode_value(result);
+
+			++(state_in->stepcount);
+			if (state_in->stepcount == CHARS_PER_LINE/4)
+			{
+				//*codechar++ = '\n';
+				state_in->stepcount = 0;
+			}
+		}
+	}
+	/* control should not reach here */
+	return codechar - code_out;
+}
+
+int base64_encode_blockend(char* code_out, base64_encodestate* state_in)
+{
+	char* codechar = code_out;
+
+	switch (state_in->step)
+	{
+	case step_B:
+		*codechar++ = base64_encode_value(state_in->result);
+		*codechar++ = '=';
+		*codechar++ = '=';
+		break;
+	case step_C:
+		*codechar++ = base64_encode_value(state_in->result);
+		*codechar++ = '=';
+		break;
+	case step_A:
+		break;
+	}
+	//*codechar++ = '\n';
+
+	return codechar - code_out;
+}
```

### Comparing `libonvif-2.0.10/src/onvif.c` & `libonvif-2.0.9/src/onvif.c`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,3125 +1,3125 @@
-/*******************************************************************************
-* onvif.c
-*
-* copyright 2018, 2023 Stephen Rhodes
-*
-* This library is free software; you can redistribute it and/or
-* modify it under the terms of the GNU Lesser General Public
-* License as published by the Free Software Foundation; either
-* version 2.1 of the License, or (at your option) any later version.
-*
-* This library is distributed in the hope that it will be useful,
-* but WITHOUT ANY WARRANTY; without even the implied warranty of
-* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-* Lesser General Public License for more details.
-*
-* You should have received a copy of the GNU Lesser General Public
-* License along with this library; if not, write to the Free Software
-* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-*
-*******************************************************************************/
-
-#include <string.h>
-#include <stdio.h>
-#include <stdlib.h>
-#include <math.h>
-#include <sys/stat.h>
-#include <libxml/parser.h>
-#include <libxml/xpath.h>
-#include "libxml/xpathInternals.h"
-
-#ifdef _WIN32
-    #include <ws2tcpip.h>
-    #include <winsock2.h>
-    #include <wincrypt.h>
-    #include <iphlpapi.h>
-    #include <fcntl.h>
-	#pragma comment(lib, "iphlpapi.lib")
-	#pragma comment(lib, "ws2_32.lib")
-#else
-    #include <sys/socket.h>
-    #include <arpa/inet.h>
-    #include <unistd.h>
-    #include <ifaddrs.h>
-    #include <sys/ioctl.h>
-    #include <sys/types.h>
-    #include <netdb.h>
-    #include <net/if.h>
-    #include <netinet/in.h>
-    #include <sys/time.h>
-#endif
-
-#include "onvif.h"
-#include "sha1.h"
-#include "cencode.h"
-#include <stdint.h>
-#include <errno.h>
-
-#define INT_TO_ADDR(_addr) \
-(_addr & 0xFF), \
-(_addr >> 8 & 0xFF), \
-(_addr >> 16 & 0xFF), \
-(_addr >> 24 & 0xFF)
-
-xmlDocPtr sendCommandToCamera(char * cmd, char * xaddrs);
-void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result);
-void getUUID(char uuid_buf[47]);
-void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char * user, char * password, time_t offset);
-void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char * xaddrs, char * post_type, char cmd[], int cmd_length);
-int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]);
-int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length);
-int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex);
-#define getNodeAttribute(doc,xpath,attribute,buf,buf_length) getNodeAttributen(doc,xpath,attribute,buf,buf_length,0)
-xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath);
-
-
-const int SHA1_DIGEST_SIZE = 20;
-char preferred_network_address[16];
-static bool dump_reply = false;
-static void dumpReply(xmlDocPtr reply);
-
-int getNetworkInterfaces(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNetworkInterfaces", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNetworkInterfacesResponse//tds:NetworkInterfaces";
-        xmlNodeSetPtr nodeset;
-        xmlChar *enabled = NULL;
-        xmlXPathObjectPtr xml_result = getNodeSet(reply, xpath);
-        if (xml_result) {
-            nodeset = xml_result->nodesetval;
-            for (int i=0; i<nodeset->nodeNr; i++) {
-                xmlNodePtr cur = nodeset->nodeTab[i];
-                xmlChar *token = xmlGetProp(cur, BAD_CAST "token");
-                xmlDocPtr temp_doc = xmlNewDoc(BAD_CAST "1.0");
-                xmlDocSetRootElement(temp_doc, cur);
-
-                bool dhcp = false;
-                char isDHCP[128];
-                xpath = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:DHCP";
-                if (getXmlValue(temp_doc, xpath, isDHCP, 128) == 0) {
-                    if (strcmp(isDHCP, "true") == 0) {
-                        dhcp = true;
-                    }
-                    onvif_data->dhcp_enabled = dhcp;
-                }
-
-                xmlChar *xpath_address;
-                xmlChar *xpath_prefix;
-                if (dhcp) {
-                    xpath_address = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:FromDHCP//tt:Address";
-                    xpath_prefix = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:FromDHCP//tt:PrefixLength";
-                } else {
-                    xpath_address = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:Manual//tt:Address";
-                    xpath_prefix = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:Manual//tt:PrefixLength";
-                }
-
-                char ip_address_buf[128];
-                if (getXmlValue(temp_doc, xpath_address, ip_address_buf, 128) == 0) {
-                    char host[128] = {0};
-                    extractHost(onvif_data->xaddrs, host);
-
-                    if (strcmp(ip_address_buf, host) == 0) {
-                        strcpy(onvif_data->ip_address_buf, ip_address_buf);
-                        strcpy(onvif_data->networkInterfaceToken, (char*) token);
-                        char prefix_length_buf[128];
-                        if (getXmlValue(temp_doc, xpath_prefix, prefix_length_buf, 128) ==  0) {
-                            onvif_data->prefix_length = atoi(prefix_length_buf);
-                        }
-                        xpath = BAD_CAST "//tds:NetworkInterfaces//tt:Info//tt:Name";
-                        getXmlValue(temp_doc, xpath, onvif_data->networkInterfaceName, 128);
-                        i = nodeset->nodeNr;
-                    }
-                }
-                xmlFreeDoc(temp_doc);
-            }
-        }
-        if (enabled != NULL) {
-            xmlFree(enabled);
-        }
-        xmlXPathFreeObject(xml_result);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getNetworkInterfaces");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getNetworkInterfaces - No XML reply");
-    }
-    return result;
-}
-
-int setNetworkInterfaces(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setNetworkInterfaces = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNetworkInterfaces", NULL);
-    xmlNewTextChild(setNetworkInterfaces, ns_tt, BAD_CAST "InterfaceToken", BAD_CAST onvif_data->networkInterfaceName);
-    xmlNodePtr networkInterface = xmlNewTextChild(setNetworkInterfaces, ns_tt, BAD_CAST "NetworkInterface", NULL);
-    xmlNodePtr ipv4 = xmlNewTextChild(networkInterface, ns_tt, BAD_CAST "IPv4", NULL);
-    if (onvif_data->dhcp_enabled) {
-        xmlNewTextChild(ipv4, ns_tt, BAD_CAST "DHCP", BAD_CAST "true");
-    } else {
-        xmlNewTextChild(ipv4, ns_tt, BAD_CAST "DHCP", BAD_CAST "false");
-        xmlNodePtr manual = xmlNewTextChild(ipv4, ns_tt, BAD_CAST "Manual", NULL);
-        xmlNewTextChild(manual, ns_tt, BAD_CAST "Address" , BAD_CAST onvif_data->ip_address_buf);
-        char prefix_length_buf[128];
-        sprintf(prefix_length_buf, "%d", onvif_data->prefix_length);
-        xmlNewTextChild(manual, ns_tt, BAD_CAST "PrefixLength", BAD_CAST prefix_length_buf);
-    }
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body//tds:SetNetworkInterfacesResponse//tds:RebootNeeded";
-        char rebootNeeded[128];
-        if (getXmlValue(reply, xpath, rebootNeeded, 128) == 0) {
-            if (strcmp(rebootNeeded, "true") == 0) {
-                rebootCamera(onvif_data);
-            }
-        }
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setNetworkInterfaces");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setNetworkInterfaces - No XML reply");
-    }
-    return result;
-}
-
-int getNetworkDefaultGateway(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNetworkDefaultGateway", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNetworkDefaultGatewayResponse//tds:NetworkGateway//tt:IPv4Address";
-        getXmlValue(reply, xpath, onvif_data->default_gateway_buf, 128);
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getNetworkDefaultGateway");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getNetworkDefaultGateway - No XML reply");
-    }
-    return result;
-}
-
-int setNetworkDefaultGateway(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setNetworkDefaultGateway = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNetworkDefaultGateway", NULL);
-    xmlNewTextChild(setNetworkDefaultGateway, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->default_gateway_buf);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setNetworkDefaultGateway");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setNetworkDefaultGateway - No XML reply");
-    }
-    return result;
-}
-
-int getDNS(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDNS", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:FromDHCP";
-        char fromDHCP[128];
-        if (getXmlValue(reply, xpath, fromDHCP, 128) == 0) {
-            if (strcmp(fromDHCP, "true") == 0) {
-                xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:DNSFromDHCP//tt:IPv4Address";
-                if (getXmlValue(reply, xpath, onvif_data->dns_buf, 128) == 0) {}
-            } else {
-                xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:DNSManual//tt:IPv4Address";
-                if (getXmlValue(reply, xpath, onvif_data->dns_buf, 128) == 0) {}
-            }
-        }
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getDNS");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getDNS - No XML reply");
-    }
-    return result;
-}
-
-int setDNS(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    char fromDHCP_buf[128];
-    if (onvif_data->dhcp_enabled) {
-        strcpy(fromDHCP_buf, "true");
-    } else {
-        strcpy(fromDHCP_buf, "false");
-    }
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);        if (result < 0)
-            strcat(onvif_data->last_error, " getVideoEncoderConfiguration");
-
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setDNS = xmlNewTextChild(body, ns_tds, BAD_CAST "SetDNS", NULL);
-    if (!onvif_data->dhcp_enabled) {
-        xmlNodePtr dnsManual = xmlNewTextChild(setDNS, ns_tds, BAD_CAST "DNSManual", NULL);
-        xmlNewTextChild(dnsManual, ns_tt, BAD_CAST "Type", BAD_CAST "IPv4");
-        xmlNewTextChild(dnsManual, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->dns_buf);
-    } else {
-        xmlNewTextChild(setDNS, ns_tds, BAD_CAST "FromDHCP", BAD_CAST fromDHCP_buf);
-    }
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setDNS");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setDNS - No XML reply");
-    }
-    return result;
-}
-
-int getNTP(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNTP", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-		xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:FromDHCP";
-		char ntp_buf[128];
-		getXmlValue(reply, xpath, ntp_buf, 128);
-		if (strcmp(ntp_buf,"true") == 0) {
-			onvif_data->ntp_dhcp = true;
-			xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:Type";
-			getXmlValue(reply, xpath, onvif_data->ntp_type, 128);
-			if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:IPv4Address";
-			else if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:IPv6Address";
-			else
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:DNSname";
-			getXmlValue(reply, xpath, onvif_data->ntp_addr, 128);
-		} else {
-			onvif_data->ntp_dhcp = false;
-			xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:Type";
-			getXmlValue(reply, xpath, onvif_data->ntp_type, 128);
-			if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:IPv4Address";
-			else if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:IPv6Address";
-			else
-				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:DNSname";
-			getXmlValue(reply, xpath, onvif_data->ntp_addr, 128);
-		}
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getNTP");
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getNTP - No XML reply");
-    }
-    return result;
-}
-
-int setNTP(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    char fromDHCP_buf[128];
-    if (onvif_data->ntp_dhcp) {
-        strcpy(fromDHCP_buf, "true");
-    } else {
-        strcpy(fromDHCP_buf, "false");
-    }
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setNTP = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNTP", NULL);
-
-    xmlNewTextChild(setNTP, ns_tds, BAD_CAST "FromDHCP", BAD_CAST fromDHCP_buf);
-    if (!onvif_data->ntp_dhcp) {
-        xmlNodePtr ntpManual = xmlNewTextChild(setNTP, ns_tds, BAD_CAST "NTPManual", NULL);
-        xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "Type", BAD_CAST onvif_data->ntp_type);
-		if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
-			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->ntp_addr);
-		else if (strcmp(onvif_data->ntp_type,"IPv6") == 0)
-			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "IPv6Address", BAD_CAST onvif_data->ntp_addr);
-		else
-			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "DNSName", BAD_CAST onvif_data->ntp_addr);
-    }
-
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setNTP");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setNTP - No XML reply");
-    }
-    return result;
-}
-
-int getHostname(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetHostname", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetHostnameResponse//tds:HostnameInformation//tt:FromDHCP";
-        xpath = BAD_CAST "//s:Body//tds:GetHostnameResponse//tds:HostnameInformation//tt:Name";
-        getXmlValue(reply, xpath, onvif_data->host_name, 128);
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getHostname");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getHostname - No XML reply");
-    }
-    return result;
-}
-
-int setHostname(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    if (onvif_data->host_name[0]) {
-        xmlNodePtr setHostname = xmlNewTextChild(body, ns_tds, BAD_CAST "SetHostname", NULL);
-        xmlNewTextChild(setHostname, ns_tds, BAD_CAST "Name", BAD_CAST onvif_data->host_name);
-        /* Do I also need to set FromDHCP to false ? */
-    } else {
-        xmlNodePtr setHostname = xmlNewTextChild(body, ns_tds, BAD_CAST "SetHostnameFromDHCP", NULL);
-        xmlNewTextChild(setHostname, ns_tds, BAD_CAST "FromDHCP", BAD_CAST "true");
-    }
-
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-		/* Should check for RebootNeeded=true from setHostnameFronDHCP */
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setHostname");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setHostname - No XML reply");
-    }
-    return result;
-}
-
-
-int getCapabilities(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr capabilities = xmlNewTextChild(body, ns_tds, BAD_CAST "GetCapabilities", NULL);
-    xmlNewTextChild(capabilities, ns_tds, BAD_CAST "Category", BAD_CAST "All");
-    char cmd[4096] = {0};
-
-
-    strcpy(onvif_data->device_service, onvif_data->xaddrs);
-    extractOnvifService(onvif_data->device_service, true);
-
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath;
-
-        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Events//tt:XAddr";
-        strcpy(onvif_data->event_service, "");
-        if (getXmlValue(reply, xpath, onvif_data->event_service, 128) == 0) {
-            extractOnvifService(onvif_data->event_service, true);
-        }
-
-        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Imaging//tt:XAddr";
-        strcpy(onvif_data->imaging_service, "");
-        if (getXmlValue(reply, xpath, onvif_data->imaging_service, 128) == 0)
-            extractOnvifService(onvif_data->imaging_service, true);
-
-        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Media//tt:XAddr";
-        strcpy(onvif_data->media_service, "");
-        if (getXmlValue(reply, xpath, onvif_data->media_service, 128) == 0)
-            extractOnvifService(onvif_data->media_service, true);
-
-        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:PTZ//tt:XAddr";
-        strcpy(onvif_data->ptz_service, "");
-        if (getXmlValue(reply, xpath, onvif_data->ptz_service, 128) == 0)
-            extractOnvifService(onvif_data->ptz_service, true);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getCapabilities");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getCapabilities - No XML reply");
-    }
-    return result;
-}
-
-int getVideoEncoderConfigurationOptions(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getVideoEncoderConfigurationOptions = xmlNewTextChild(body, ns_trt, BAD_CAST "GetVideoEncoderConfigurationOptions", NULL);
-    if (onvif_data->videoEncoderConfigurationToken[0])
-        xmlNewTextChild(getVideoEncoderConfigurationOptions, ns_trt, BAD_CAST "ConfigurationToken", BAD_CAST onvif_data->videoEncoderConfigurationToken);
-    if (onvif_data->profileToken[0])
-        xmlNewTextChild(getVideoEncoderConfigurationOptions, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *width = NULL;
-        xmlChar *height = NULL;
-        xmlChar *xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:ResolutionsAvailable";
-        xmlNodeSetPtr nodeset;
-        xmlXPathObjectPtr xml_result = getNodeSet(reply, xpath);
-        int k = 0;
-        if (xml_result) {
-            nodeset = xml_result->nodesetval;
-            for (int i=0; i<nodeset->nodeNr; i++) {
-                xmlNodePtr cur = nodeset->nodeTab[i]->children;
-                while(cur != NULL) {
-                    if ((!xmlStrcmp(cur->name, (const xmlChar *) "Width"))) {
-                        width = xmlNodeListGetString(reply, cur->xmlChildrenNode, 1);
-                    }
-                    else if ((!xmlStrcmp(cur->name, (const xmlChar *) "Height"))) {
-                        height = xmlNodeListGetString(reply, cur->xmlChildrenNode, 1);
-                    }
-                    cur = cur->next;
-                }
-                char tmp[128] = {0};
-                if ((strlen((char *)width) + strlen((char *)height)) > 124) {
-                  fprintf(stderr, "xmlNodeListString return buffer overflow %zu\n", strlen((char *)width) + strlen((char *)height));
-                } else {
-                  sprintf(tmp, "%s x %s", width, height);
-                }
-
-                int size = 0;
-                bool found_size = false;
-                while (!found_size) {
-                    if (strlen(onvif_data->resolutions_buf[size]) == 0) {
-                        found_size = true;
-                    } else {
-                        size++;
-                        if (size > 15)
-                            found_size = true;
-                    }
-                }
-                bool duplicate = false;
-                for (int n=0; n<size; n++) {
-                    if (strcmp(onvif_data->resolutions_buf[n], tmp) == 0) {
-                        duplicate = true;
-                    }
-                }
-                if (!duplicate) {
-                    strcpy(onvif_data->resolutions_buf[size], tmp);
-                    k++;
-                }
-
-                if (width != NULL)
-                    xmlFree(width);
-                if (height != NULL)
-                    xmlFree(height);
-            }
-            xmlXPathFreeObject(xml_result);
-        }
-
-        char temp_buf[128];
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:GovLengthRange//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->gov_length_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:GovLengthRange//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->gov_length_max = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:FrameRateRange//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->frame_rate_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:FrameRateRange//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->frame_rate_max = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:Extension//tt:H264//tt:BitrateRange//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->bitrate_min = atoi(temp_buf);
-        else
-            onvif_data->bitrate_min = 128;
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:Extension//tt:H264//tt:BitrateRange//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->bitrate_max = atoi(temp_buf);
-        else
-            onvif_data->bitrate_max = 16384;
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getVideoEncoderConfigurationOptions");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getVideoEncoderConfigurationOptions - No XML reply");
-    }
-    return result;
-}
-
-int getVideoEncoderConfiguration(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getVideoEncoderConfiguration = xmlNewTextChild(body, ns_trt, BAD_CAST "GetVideoEncoderConfiguration", NULL);
-    xmlNewTextChild(getVideoEncoderConfiguration, ns_trt, BAD_CAST "ConfigurationToken", BAD_CAST onvif_data->videoEncoderConfigurationToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath;
-        char temp_buf[128] = {0};
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Name";
-        getXmlValue(reply, xpath, onvif_data->video_encoder_name_buf, 128);
-
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:UseCount";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->use_count = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:GuaranteedFrameRate";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
-        if (strcmp(temp_buf, "true") == 0)
-            onvif_data->guaranteed_frame_rate = true;
-        else
-            onvif_data->guaranteed_frame_rate = false;
-        }
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Encoding";
-        getXmlValue(reply, xpath, onvif_data->encoding, 128);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Resolution//tt:Width";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->conf_width = atof(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Resolution//tt:Height";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->conf_height = atof(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Quality";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->quality = atof(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:FrameRateLimit";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->conf_frame_rate_limit = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:EncodingInterval";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->conf_encoding_interval = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:BitrateLimit";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->conf_bitrate_limit = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:H264//tt:H264Profile";
-        getXmlValue(reply, xpath, onvif_data->h264_profile_buf, 128);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:Type";
-        getXmlValue(reply, xpath, onvif_data->multicast_address_type_buf, 128);
-		if (strcmp(onvif_data->multicast_address_type_buf,"IPv6") == 0)
-            xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:IPv6Address";
-		else
-            xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:IPv4Address";
-        getXmlValue(reply, xpath, onvif_data->multicast_address_buf, 128);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Port";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->multicast_port = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:TTL";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->multicast_ttl = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:AutoStart";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
-        if (strcmp(temp_buf, "true") == 0)
-            onvif_data->autostart = true;
-        else
-            onvif_data->autostart = false;
-        }
-        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:SessionTimeout";
-        getXmlValue(reply, xpath, onvif_data->session_time_out_buf, 128);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getVideoEncoderConfiguration");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getVideoEncoderConfiguration - No XML reply");
-    }
-    return result;
-}
-
-int setVideoEncoderConfiguration(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    char frame_rate_buf[128] = {0};
-    char gov_length_buf[128] = {0};
-    char bitrate_buf[128] = {0};
-    char width_buf[128] = {0};
-    char height_buf[128] = {0};
-    char use_count_buf[128] = {0};
-    char quality_buf[128] = {0};
-    char multicast_port_buf[128] = {0};
-    char multicast_ttl_buf[128] = {0};
-    char autostart_buf[128] = {0};
-    char encoding_interval_buf[128] = {0};
-
-    sprintf(frame_rate_buf, "%d", onvif_data->frame_rate);
-    sprintf(gov_length_buf, "%d", onvif_data->gov_length);
-    sprintf(bitrate_buf, "%d", onvif_data->bitrate);
-    sprintf(use_count_buf, "%d", onvif_data->use_count);
-    sprintf(width_buf, "%d", onvif_data->width);
-    sprintf(height_buf, "%d", onvif_data->height);
-    sprintf(quality_buf, "%f", onvif_data->quality);
-    sprintf(multicast_port_buf, "%d", onvif_data->multicast_port);
-    sprintf(multicast_ttl_buf, "%d", onvif_data->multicast_ttl);
-    if (onvif_data->autostart)
-        strcpy(autostart_buf, "true");
-    else
-        strcpy(autostart_buf, "false");
-    sprintf(encoding_interval_buf, "%d", onvif_data->conf_encoding_interval);
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setVideoEncoderConfiguration = xmlNewTextChild(body, ns_trt, BAD_CAST "SetVideoEncoderConfiguration", NULL);
-    xmlNodePtr configuration = xmlNewTextChild(setVideoEncoderConfiguration, ns_trt, BAD_CAST "Configuration", NULL);
-    xmlNewProp(configuration, BAD_CAST "token", BAD_CAST onvif_data->videoEncoderConfigurationToken);
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Name", BAD_CAST onvif_data->video_encoder_name_buf);
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "UseCount", BAD_CAST use_count_buf);
-#ifdef ONVIF19060
-	/* Sad, but not supported until 19.06 release - crashes my older camera */
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "GuaranteedFrameRate", onvif_data->guaranteed_frame_rate?BAD_CAST "true":BAD_CAST "false");
-#endif
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Encoding", onvif_data->encoding[0]?BAD_CAST onvif_data->encoding:BAD_CAST "H264");
-    xmlNodePtr resolution = xmlNewTextChild(configuration, ns_tt, BAD_CAST "Resolution", NULL);
-    xmlNewTextChild(resolution, ns_tt, BAD_CAST "Width", BAD_CAST width_buf);
-    xmlNewTextChild(resolution, ns_tt, BAD_CAST "Height", BAD_CAST height_buf);
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Quality", BAD_CAST quality_buf);
-    xmlNodePtr rateControl = xmlNewTextChild(configuration, ns_tt, BAD_CAST "RateControl", NULL);
-    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "FrameRateLimit", BAD_CAST frame_rate_buf);
-    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "EncodingInterval", BAD_CAST encoding_interval_buf);
-    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "BitrateLimit", BAD_CAST bitrate_buf);
-    xmlNodePtr h264 = xmlNewTextChild(configuration, ns_tt, BAD_CAST "H264", NULL);
-    xmlNewTextChild(h264, ns_tt, BAD_CAST "GovLength", BAD_CAST gov_length_buf);
-    xmlNewTextChild(h264, ns_tt, BAD_CAST "H264Profile", BAD_CAST onvif_data->h264_profile_buf);
-    xmlNodePtr multicast = xmlNewTextChild(configuration, ns_tt, BAD_CAST "Multicast", NULL);
-    xmlNodePtr address = xmlNewTextChild(multicast, ns_tt, BAD_CAST "Address", NULL);
-    xmlNewTextChild(address, ns_tt, BAD_CAST "Type", BAD_CAST onvif_data->multicast_address_type_buf);
-    xmlNewTextChild(address, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->multicast_address_buf);
-    xmlNewTextChild(multicast, ns_tt, BAD_CAST "Port", BAD_CAST multicast_port_buf);
-    xmlNewTextChild(multicast, ns_tt, BAD_CAST "TTL", BAD_CAST multicast_ttl_buf);
-    xmlNewTextChild(multicast, ns_tt, BAD_CAST "AutoStart", BAD_CAST autostart_buf);
-    xmlNewTextChild(configuration, ns_tt, BAD_CAST "SessionTimeout", BAD_CAST onvif_data->session_time_out_buf);
-    xmlNewTextChild(setVideoEncoderConfiguration, ns_trt, BAD_CAST "ForcePersistence", BAD_CAST "true");
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setVideoEncoderConfiguration");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setVideoEncoderConfiguration - No XML reply");
-    }
-    return result;
-}
-
-int getProfile(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getProfile = xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfile", NULL);
-    xmlNewTextChild(getProfile, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        char temp_buf[128];
-
-        xmlChar *xpath;
-
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:Resolution//tt:Width";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->width = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:Resolution//tt:Height";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->height = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:RateControl//tt:FrameRateLimit";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
-            onvif_data->frame_rate = atoi(temp_buf);
-        }
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:RateControl//tt:BitrateLimit";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
-            onvif_data->bitrate = atoi(temp_buf);
-        } else {
-            onvif_data->bitrate = 0;
-        }
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:H264//tt:GovLength";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
-            onvif_data->gov_length = atoi(temp_buf);
-        }
-
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration";
-        getNodeAttribute(reply, xpath, BAD_CAST "token", onvif_data->videoEncoderConfigurationToken, 128);
-        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoSourceConfiguration//tt:SourceToken";
-        getXmlValue(reply, xpath, onvif_data->videoSourceConfigurationToken, 128);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getProfile");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getProfile - No XML reply");
-    }
-    return result;
-}
-
-int getOptions(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getOptions = xmlNewTextChild(body, ns_timg, BAD_CAST "GetOptions", NULL);
-    xmlNewTextChild(getOptions, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath;
-        char temp_buf[128];
-
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Brightness//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->brightness_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Brightness//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->brightness_max = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:ColorSaturation//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->saturation_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:ColorSaturation//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->saturation_max = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Contrast//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->contrast_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Contrast//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->contrast_max = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Sharpness//tt:Min";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->sharpness_min = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Sharpness//tt:Max";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->sharpness_max = atoi(temp_buf);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getOptions");
-        xmlFreeDoc(reply);
-     } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getOptions - No XML reply");
-    }
-    return result;
-}
-
-int getImagingSettings(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getImagingSettings = xmlNewTextChild(body, ns_timg, BAD_CAST "GetImagingSettings", NULL);
-    xmlNewTextChild(getImagingSettings, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlChar *xpath;
-        char temp_buf[128];
-
-        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Brightness";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->brightness = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:ColorSaturation";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->saturation = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Contrast";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->contrast = atoi(temp_buf);
-        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Sharpness";
-        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
-            onvif_data->sharpness = atoi(temp_buf);
-
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getImagingSettings");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getImagingSettings - No XML reply");
-    }
-    return result;
-}
-
-int setImagingSettings(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    char brightness_buf[128] = {0};
-    char saturation_buf[128] = {0};
-    char contrast_buf[128] = {0};
-    char sharpness_buf[128] = {0};
-    sprintf(brightness_buf, "%d", onvif_data->brightness);
-    sprintf(saturation_buf, "%d", onvif_data->saturation);
-    sprintf(contrast_buf, "%d", onvif_data->contrast);
-    sprintf(sharpness_buf, "%d", onvif_data->sharpness);
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setImagingSettings = xmlNewTextChild(body, ns_timg, BAD_CAST "SetImagingSettings", NULL);
-    xmlNewTextChild(setImagingSettings, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
-    xmlNodePtr imagingSettings = xmlNewTextChild(setImagingSettings, ns_timg, BAD_CAST "ImagingSettings", NULL);
-    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Brightness", BAD_CAST brightness_buf);
-    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "ColorSaturation", BAD_CAST saturation_buf);
-    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Contrast", BAD_CAST contrast_buf);
-    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Sharpness", BAD_CAST sharpness_buf);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setImagingSettings");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setImagingSettings - No XML reply");
-    }
-    return result;
-}
-
-int continuousMove(float x, float y, float z, struct OnvifData *onvif_data) {
-    int result = 0;
-    char pan_tilt_string[128] = {0};
-    char zoom_string[128] = {0};
-    sprintf(pan_tilt_string, "PanTilt x=\"%.*f\" y=\"%.*f\"", 2, x, 2, y);
-    sprintf(zoom_string, "Zoom x=\"%.*f\"", 2, z);
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr continuousMove = xmlNewTextChild(body, ns_ptz, BAD_CAST "ContinuousMove", NULL);
-    xmlNewTextChild(continuousMove, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    xmlNodePtr velocity = xmlNewTextChild(continuousMove, ns_ptz, BAD_CAST "Velocity", BAD_CAST NULL);
-    xmlNewTextChild(velocity, ns_tt, BAD_CAST pan_tilt_string, NULL);
-    xmlNewTextChild(velocity, ns_tt, BAD_CAST zoom_string, NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " continuousMove");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "continuousMove - No XML reply");
-    }
-    return result;
-}
-
-int moveStop(int type, struct OnvifData *onvif_data) {
-    int result = 0;
-    char pan_tilt_flag[128] = {0};
-    char zoom_flag[128] = {0};
-
-    if (type == PAN_TILT_STOP) {
-        strcpy(pan_tilt_flag, "true");
-        strcpy(zoom_flag, "false");
-    }
-    else if (type == ZOOM_STOP) {
-        strcpy(pan_tilt_flag, "false");
-        strcpy(zoom_flag, "true");
-    }
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr stop = xmlNewTextChild(body, ns_ptz, BAD_CAST "Stop", NULL);
-    xmlNewTextChild(stop, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    xmlNewTextChild(stop, ns_ptz, BAD_CAST "PanTilt", BAD_CAST pan_tilt_flag);
-    xmlNewTextChild(stop, ns_ptz, BAD_CAST "Zoom", BAD_CAST zoom_flag);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " moveStop");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "moveStop - No XML reply");
-    }
-    return result;
-}
-
-int setPreset(char *arg, struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setPreset = xmlNewTextChild(body, ns_ptz, BAD_CAST "SetPreset", NULL);
-    xmlNewTextChild(setPreset, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    xmlNewTextChild(setPreset, ns_ptz, BAD_CAST "PresetToken", BAD_CAST arg);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setPreset");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setPreset - No XML reply");
-    }
-    return result;
-}
-
-int gotoPreset(char *arg, struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr gotoPreset = xmlNewTextChild(body, ns_ptz, BAD_CAST "GotoPreset", NULL);
-    xmlNewTextChild(gotoPreset, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    xmlNewTextChild(gotoPreset, ns_ptz, BAD_CAST "PresetToken", BAD_CAST arg);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " gotoPreset");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "gotoPreset - No XML reply");
-    }
-    return result;
-}
-
-int setUser(char *new_password, struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setUser = xmlNewTextChild(body, ns_tds, BAD_CAST "SetUser", NULL);
-    xmlNodePtr user = xmlNewTextChild(setUser, ns_tds, BAD_CAST "User", NULL);
-    xmlNewTextChild(user, ns_tt, BAD_CAST "Username", BAD_CAST "admin");
-    xmlNewTextChild(user, ns_tt, BAD_CAST "Password", BAD_CAST new_password);
-    xmlNewTextChild(user, ns_tt, BAD_CAST "UserLevel", BAD_CAST "Administrator");
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setUser");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setUser - No XML reply");
-    }
-    return result;
-}
-
-int setSystemDateAndTime(struct OnvifData *onvif_data) {
-    int result = 0;
-    time_t rawtime;
-    time(&rawtime);
-    struct tm *UTCTime = localtime(&rawtime);
-    char dst_flag_buf[128];
-    if (UTCTime->tm_isdst == 1)
-        strcpy(dst_flag_buf, "true");
-    else
-        strcpy(dst_flag_buf, "false");
-    char hour_buf[128];
-    char minute_buf[128];
-    char second_buf[128];
-    char year_buf[128];
-    char month_buf[128];
-    char day_buf[128];
-    sprintf(hour_buf, "%d", UTCTime->tm_hour);
-    sprintf(minute_buf, "%d", UTCTime->tm_min);
-    sprintf(second_buf, "%d", UTCTime->tm_sec);
-    sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
-    sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
-    sprintf(day_buf, "%d", UTCTime->tm_mday);
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
-    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "Manual");
-    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
-    xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
-    xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST "UTC0");
-    xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
-    xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
-    xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " setSystemDatAndTime");
-        xmlFreeDoc(reply);
-    }
-    else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setSystemDateAndTime - No XML reply");
-    }
-    return result;
-}
-
-int setSystemDateAndTimeUsingTimezone(struct OnvifData *onvif_data) {
-    int result = 0;
-    time_t rawtime;
-    time(&rawtime);
-	bool special = false;
-    struct tm *UTCTime = localtime(&rawtime);
-    char dst_flag_buf[128];
-    if (UTCTime->tm_isdst == 1)
-        strcpy(dst_flag_buf, "true");
-    else
-        strcpy(dst_flag_buf, "false");
-    if (strcmp(onvif_data->timezone,"UTC0") == 0) {
-        special = true;
-    } else {
-        if (!onvif_data->timezone[0]) {
-#ifndef _WIN32
-            // work out a timezone to use on the camera 
-            int h = -(UTCTime->tm_gmtoff/3600);
-            int m = (UTCTime->tm_gmtoff + 3600 * h)/60;
-            if (m)
-                sprintf(onvif_data->timezone,"%s%d:%02d:00%s",tzname[0],h,m,tzname[1]);
-            else
-                sprintf(onvif_data->timezone,"%s%d%s",tzname[0],h,tzname[1]);
-#else
-            int h = _timezone/3600;
-            int m = (_timezone - 3600 * h)/60;
-            if (m)
-                sprintf(onvif_data->timezone,"%s%d:%02d:00%s",_tzname[0],h,m,_tzname[1]);
-            else
-                sprintf(onvif_data->timezone,"%s%d%s",_tzname[0],h,_tzname[1]);
-#endif
-        }
-        UTCTime = gmtime(&rawtime);
-    }
-    if (!onvif_data->datetimetype)
-        onvif_data->datetimetype = 'M'; // manual 
-    char hour_buf[128];
-    char minute_buf[128];
-    char second_buf[128];
-    char year_buf[128];
-    char month_buf[128];
-    char day_buf[128];
-    sprintf(hour_buf, "%d", UTCTime->tm_hour);
-    sprintf(minute_buf, "%d", UTCTime->tm_min);
-    sprintf(second_buf, "%d", UTCTime->tm_sec);
-    sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
-    sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
-    sprintf(day_buf, "%d", UTCTime->tm_mday);
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
-    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "Manual");
-    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
-    xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
-    xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST onvif_data->timezone);
-    xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
-    xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
-    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
-    xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
-    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        xmlFreeDoc(reply);
-        if (result == 0 && onvif_data->datetimetype == 'N') {
-            // switch back to NTP after we have nudged it to correct 
-            time_t newtime;
-            time(&newtime);
-            if (newtime != rawtime) {
-                // save a little effort if we are within a second of the previous check 
-                if (special)
-                    UTCTime = localtime(&newtime);
-                else
-                    UTCTime = gmtime(&newtime);
-                sprintf(hour_buf, "%d", UTCTime->tm_hour);
-                sprintf(minute_buf, "%d", UTCTime->tm_min);
-                sprintf(second_buf, "%d", UTCTime->tm_sec);
-                sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
-                sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
-                sprintf(day_buf, "%d", UTCTime->tm_mday);
-            }
-            doc = xmlNewDoc(BAD_CAST "1.0");
-            xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-            xmlDocSetRootElement(doc, root);
-            xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-            xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-            xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-            xmlSetNs(root, ns_env);
-            addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-            xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-            xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
-            xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "NTP");
-            xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
-            xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
-            xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST onvif_data->timezone);
-            // Need to include date/time even though the specs say it should be ignored 
-            xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
-            xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
-            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
-            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
-            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
-            xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
-            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
-            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
-            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
-            char cmd[4096] = {0};
-            addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-            xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-            if (reply != NULL) {
-                result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-		xmlFreeDoc(reply);
-            } else {
-                result = -1;
-		strcpy(onvif_data->last_error, "setSystemDateAndTimeUsingTimezone - No XML reply");
-            }
-        }
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "setSystemDateAndTimeUsingTimezone 2 - No XML reply");
-    }
-    return result;
-}
-
-int getProfileToken(struct OnvifData *onvif_data, int profileIndex) {
-    int result;
-    onvif_data->profileToken[0] = 0;
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfiles", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        getNodeAttributen(reply, BAD_CAST "//s:Body//trt:GetProfilesResponse//trt:Profiles", BAD_CAST "token", onvif_data->profileToken, 128, profileIndex);
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getProfileToken");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getProfileToken - No XML reply");
-    }
-    return result;
-}
-
-int getTimeOffset(struct OnvifData *onvif_data) {
-    int result = 0;
-
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetSystemDateAndTime", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-
-    if (reply != NULL) {
-        char hour_buf[16];
-        char min_buf[16];
-        char sec_buf[16];
-        char year_buf[16];
-        char month_buf[16];
-        char day_buf[16];
-        char dst_buf[16];
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Hour", hour_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Minute", min_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Second", sec_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Year", year_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Month", month_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Day", day_buf, 16);
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:DaylightSavings", dst_buf, 16);
-
-    	onvif_data->dst = false;
-        int is_dst = 0;
-        if (strcmp(dst_buf, "true") == 0) {
-            is_dst = 1;
-	        onvif_data->dst = true;
-	    }
-
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:TimeZone//tt:TZ", onvif_data->timezone, 128);
-	    char dttype[16];
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:DateTimeType", dttype, 16);
-	    onvif_data->datetimetype = dttype[0]; /* M == Manual, N == NTP */
-
-        time_t now = time(NULL);
-        time_t utc_time_here = now;
-	    bool special = false;
-	    if (strcmp(onvif_data->timezone,"UTC0") == 0) {
-	        /* special case - camera is running on local time believing it is UTC */
-	        special = true;
-            struct tm *utc_here = gmtime(&now);
-            utc_here->tm_isdst = -1;
-            utc_time_here = mktime(utc_here);
-	    }
-
-        struct tm *utc_there = localtime(&now);
-        utc_there->tm_year = atoi(year_buf) - 1900;
-        utc_there->tm_mon = atoi(month_buf) - 1;
-        utc_there->tm_mday = atoi(day_buf);
-        utc_there->tm_hour = atoi(hour_buf);
-        utc_there->tm_min = atoi(min_buf);
-        utc_there->tm_sec = atoi(sec_buf);
-        utc_there->tm_isdst = is_dst;
-	    time_t utc_time_there;
-	    if (special)
-	        utc_time_there = mktime(utc_there);
-	    else
-#ifndef _WIN32
-	        utc_time_there = timegm(utc_there);
-#else
-	        utc_time_there = _mkgmtime(utc_there);
-#endif
-	    onvif_data->time_offset = utc_time_there - utc_time_here;
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getTimeOfset");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getTimeOffset - No XML reply");
-    }
-
-    return result;
-}
-
-int getStreamUri(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr getStreamUri = xmlNewTextChild(body, ns_trt, BAD_CAST "GetStreamUri", NULL);
-    xmlNodePtr streamSetup = xmlNewTextChild(getStreamUri, ns_trt, BAD_CAST "StreamSetup", NULL);
-    xmlNewTextChild(streamSetup, ns_tt, BAD_CAST "Stream", BAD_CAST "RTP-Unicast");
-    xmlNodePtr transport = xmlNewTextChild(streamSetup, ns_tt, BAD_CAST "Transport", NULL);
-    xmlNewTextChild(transport, ns_tt, BAD_CAST "Protocol", BAD_CAST "RTSP");
-    xmlNewTextChild(getStreamUri, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        getXmlValue(reply, BAD_CAST "//s:Body//trt:GetStreamUriResponse//trt:MediaUri//tt:Uri", onvif_data->stream_uri, 1024);
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getStreamUri");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getStreamUri - No XML reply");
-    }
-    return result;
-}
-
-int getDeviceInformation(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDeviceInformation", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetDeviceInformationResponse//tds:SerialNumber", onvif_data->serial_number, 128);
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " getdeviceImformation");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "getDeviceInformation - No XML reply");
-    }
-    return result;
-}
-
-void getDiscoveryXml2(char buffer[], int buf_size) {
-    char *xml_string = "<s:Envelope xmlns:s=\"http://www.w3.org/2003/05/soap-envelope\" xmlns:a=\"http://schemas.xmlsoap.org/ws/2004/08/addressing\"><s:Header><a:Action s:mustUnderstand=\"1\">http://schemas.xmlsoap.org/ws/2005/04/discovery/Probe</a:Action><a:MessageID>uuid:6bbdae2d-f229-42c8-a27b-93880fb80826</a:MessageID><a:ReplyTo><a:Address>http://schemas.xmlsoap.org/ws/2004/08/addressing/role/anonymous</a:Address></a:ReplyTo><a:To s:mustUnderstand=\"1\">urn:schemas-xmlsoap-org:ws:2005:04:discovery</a:To></s:Header><s:Body><Probe xmlns=\"http://schemas.xmlsoap.org/ws/2005/04/discovery\"><d:Types xmlns:d=\"http://schemas.xmlsoap.org/ws/2005/04/discovery\" xmlns:dp0=\"http://www.onvif.org/ver10/device/wsdl\">dp0:Device</d:Types></Probe></s:Body></s:Envelope>";
-    strcpy(buffer, xml_string);
-}
-
-void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]) {
-    for (int i=0; i<buf_size; i++)
-        buffer[i] = '\0';
-    getUUID(uuid);
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNewProp(root, BAD_CAST "xmlns:SOAP-ENV", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
-    xmlNewProp(root, BAD_CAST "xmlns:a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
-    xmlNsPtr ns_env = xmlNewNs(root, NULL, BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_a = xmlNewNs(root, NULL, BAD_CAST "a");
-    xmlSetNs(root, ns_env);
-    xmlNodePtr header = xmlNewTextChild(root, ns_env, BAD_CAST "Header", NULL);
-    xmlNodePtr action = xmlNewTextChild(header, ns_a, BAD_CAST "Action", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery/Probe");
-    xmlNewProp(action, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
-    xmlNodePtr messageid = xmlNewTextChild(header, ns_a, BAD_CAST "MessageID", BAD_CAST uuid);
-    xmlNodePtr replyto = xmlNewTextChild(header, ns_a, BAD_CAST "ReplyTo", NULL);
-    xmlNodePtr address = xmlNewTextChild(replyto, ns_a, BAD_CAST "Address", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing/role/anonymous");
-    xmlNodePtr to = xmlNewTextChild(header, ns_a, BAD_CAST "To", BAD_CAST "urn:schemas-xmlsoap-org:ws:2005:04:discovery");
-    xmlNewProp(to, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr probe = xmlNewTextChild(body, NULL, BAD_CAST "Probe", NULL);
-    xmlNewProp(probe, BAD_CAST "xmlns:p", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
-    xmlNsPtr ns_p = xmlNewNs(probe, NULL, BAD_CAST "p");
-    xmlSetNs(probe, ns_p);
-    xmlNodePtr types = xmlNewTextChild(probe, NULL, BAD_CAST "Types", BAD_CAST "dp0:NetworkVideoTransmitter");
-    xmlNewProp(types, BAD_CAST "xmlns:d", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
-    xmlNewProp(types, BAD_CAST "xmlns:dp0", BAD_CAST "http://www.onvif.org/ver10/network/wsdl");
-    xmlNsPtr ns_d = xmlNewNs(types, NULL, BAD_CAST "d");
-    xmlSetNs(types, ns_d);
-    xmlOutputBufferPtr outputbuffer = xmlAllocOutputBuffer(NULL);
-    xmlNodeDumpOutput(outputbuffer, doc, root, 0, 0, NULL);
-    int size = xmlOutputBufferGetSize(outputbuffer);
-    strcpy(buffer, (char*)xmlOutputBufferGetContent(outputbuffer));
-    xmlOutputBufferFlush(outputbuffer);
-    xmlOutputBufferClose(outputbuffer);
-    xmlFreeDoc(doc);
-}
-
-int rebootCamera(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "SystemReboot", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " rebootCamera");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "rebootCamera - No XML reply");
-    }
-  return result;
-}
-
-int hardReset(struct OnvifData *onvif_data) {
-    int result = 0;
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNodePtr setSystemFactoryDefault = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemFactoryDefault", NULL);
-    xmlNewTextChild(setSystemFactoryDefault, ns_tds, BAD_CAST "FactoryDefault", BAD_CAST "Hard");
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
-        if (result < 0)
-            strcat(onvif_data->last_error, " hardReset");
-        xmlFreeDoc(reply);
-    } else {
-        result = -1;
-        strcpy(onvif_data->last_error, "hardReset - No XML reply");
-    }
-    return result;
-}
-
-void saveSystemDateAndTime(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetSystemDateAndTime", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-void saveScopes(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetScopes", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-void saveDeviceInformation(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDeviceInformation", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-void saveCapabilities(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_tds, BAD_CAST "GetCapabilities", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-void saveProfiles(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfiles", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-void saveServiceCapabilities(char *filename, struct OnvifData *onvif_data) {
-    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
-    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
-    xmlDocSetRootElement(doc, root);
-    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
-    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
-    xmlSetNs(root, ns_env);
-    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
-    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
-    xmlNewTextChild(body, ns_trt, BAD_CAST "GetServiceCapabilities", NULL);
-    char cmd[4096] = {0};
-    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
-    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
-    if (reply != NULL) {
-        xmlSaveFormatFile(filename, reply, 1);
-        xmlFreeDoc(reply);
-    }
-}
-
-int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length) {
-    xmlChar *keyword = NULL;
-    xmlXPathContextPtr context = xmlXPathNewContext(doc);
-    if (context == NULL) {
-        return -1;
-    }
-    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
-    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
-    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
-    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
-    xmlXPathRegisterNs(context, BAD_CAST "d", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
-    xmlXPathRegisterNs(context, BAD_CAST "ter", BAD_CAST "http://www.onvif.org/ver10/error");
-    xmlXPathRegisterNs(context, BAD_CAST "a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
-
-
-    xmlXPathObjectPtr result = xmlXPathEvalExpression(xpath, context);
-    xmlXPathFreeContext(context);
-    if (result == NULL) {
-        return -2;
-    }
-
-    if (xmlXPathNodeSetIsEmpty(result->nodesetval)) {
-        if ((strcmp((char*) xpath, "//s:Body//s:Fault//s:Code//s:Subcode//s:Value") != 0) && (strcmp((char*) xpath, "//s:Body//s:Fault//s:Reason//s:Text") != 0)) {
-        }
-    return -3;
-    }
-
-    if (result) {
-        keyword = xmlNodeListGetString(doc, result->nodesetval->nodeTab[0]->xmlChildrenNode, 1);
-        if (keyword != NULL) {
-            if (strlen((char*) keyword) > buf_length-1) {
-                xmlXPathFreeObject(result);
-                xmlFree(keyword);
-                return -4;
-            } else {
-                for (int i=0; i<buf_length; i++)
-                    buf[i] = '\0';
-                strcpy(buf, (char*) keyword);
-            }
-        }
-    }
-
-    xmlXPathFreeObject(result);
-    if (keyword != NULL)
-        xmlFree(keyword);
-    return 0;
-}
-
-int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex) {
-    xmlChar *keyword = NULL;
-    xmlXPathContextPtr context = xmlXPathNewContext(doc);
-    if (context == NULL) {
-        return -1;
-    }
-    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
-    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
-    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
-    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
-    xmlXPathRegisterNs(context, BAD_CAST "ter", BAD_CAST "http://www.onvif.org/ver10/error");
-    xmlXPathRegisterNs(context, BAD_CAST "a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
-
-    xmlXPathObjectPtr result = xmlXPathEvalExpression(xpath, context);
-    xmlXPathFreeContext(context);
-    if (result == NULL) {
-        return -2;
-    }
-
-    if (xmlXPathNodeSetIsEmpty(result->nodesetval)) {
-        return -3;
-    }
-
-    if (result) {
-        if( profileIndex >= result->nodesetval->nodeNr )
-            return -5;
-
-        keyword = xmlGetProp(result->nodesetval->nodeTab[profileIndex], attribute);
-        if (keyword != NULL) {
-            if (strlen((char*) keyword) > buf_length-1) {
-                xmlXPathFreeObject(result);
-                xmlFree(keyword);
-                return -4;
-            } else {
-                for (int i=0; i<buf_length; i++)
-                    buf[i] = '\0';
-                strcpy(buf, (char*) keyword);
-            }
-        }
-    }
-
-    xmlXPathFreeObject(result);
-    if (keyword != NULL)
-        xmlFree(keyword);
-    return 0;
-}
-
-xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath) {
-    xmlXPathContextPtr context;
-    xmlXPathObjectPtr result;
-
-    context = xmlXPathNewContext(doc);
-    if (context == NULL) {
-        return NULL;
-    }
-    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
-    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
-    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
-    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
-    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
-
-    result = xmlXPathEvalExpression(xpath, context);
-    xmlXPathFreeContext(context);
-    if (result == NULL) {
-        return NULL;
-    }
-    if(xmlXPathNodeSetIsEmpty(result->nodesetval)){
-        xmlXPathFreeObject(result);
-        return NULL;
-    }
-    return result;
-}
-
-xmlDocPtr sendCommandToCamera(char *cmd, char *xaddrs) {
-    int sock = 0, valread, flags;
-    const int buffer_size = 4096;
-    struct sockaddr_in serv_addr;
-    char buffer[4096] = {0};
-
-    char tmp[128] = {0};
-    char *mark = strstr(xaddrs, "//");
-    int start = mark-xaddrs+2;
-    int tmp_len = strlen(xaddrs);
-    int j;
-    for (j=0; j<tmp_len-start; j++) {
-        tmp[j] = xaddrs[j+start];
-    }
-    tmp[j] = '\0';
-
-    mark = strstr(tmp, "/");
-    int end = mark-tmp;
-    char tmp2[128] = {0};
-    for (j=0; j<end; j++) {
-        tmp2[j] = tmp[j];
-    }
-    tmp2[j] = '\0';
-
-    char host[128] = {0};
-    char port_buf[128] = {0};
-    mark = strstr(tmp2, ":");
-    if (mark == NULL) {
-        strcpy(host, tmp2);
-        strcpy(port_buf, "80");
-    } else {
-        start = mark-tmp2;
-        for (j=0; j<start; j++) {
-            host[j] = tmp2[j];
-        }
-        host[j] = '\0';
-        tmp_len = strlen(tmp2);
-        for (j=start+1; j<tmp_len; j++) {
-            port_buf[j-(start+1)] = tmp2[j];
-        }
-        port_buf[j-(start+1)] = '\0';
-    }
-
-    int port = atoi(port_buf);
-
-#ifdef _WIN32
-    WSADATA wsaData;
-    WSAStartup(MAKEWORD(2,2), &wsaData);
-#endif
-
-    if ((sock = socket(AF_INET, SOCK_STREAM, 0)) < 0) {
-        return NULL;
-    }
-
-    memset(&serv_addr, '0', sizeof(serv_addr));
-    serv_addr.sin_family = AF_INET;
-    serv_addr.sin_port = htons(port);
-    serv_addr.sin_addr.s_addr = inet_addr(host);
-
-    if (connect(sock, (struct sockaddr *)&serv_addr, sizeof(serv_addr)) < 0) {
-        return NULL;
-    }
-
-    if (send(sock , cmd , strlen(cmd) , 0 ) < 0) {
-        return NULL;
-    }
-    valread = recv( sock , buffer, 4096, 0);
-
-    char http_terminate[5];
-    http_terminate[0] = '\r';
-    http_terminate[1] = '\n';
-    http_terminate[2] = '\r';
-    http_terminate[3] = '\n';
-    http_terminate[4] = '\0';
-
-    char * substr = strstr(buffer, http_terminate);
-    if (substr == NULL)
-        return NULL;
-
-    int i;
-    int xml_start = substr - buffer + 4;
-    if (xml_start > 1024)
-        return NULL;
-    char http_header[1024];
-    for (i=0; i<xml_start; i++) {
-        http_header[i] = buffer[i];
-    }
-    http_header[xml_start] = '\0';
-
-    substr = strstr(http_header, "Content-Length: ");
-    if (substr == NULL)
-        return NULL;
-
-    int length_start = substr - http_header + 16;
-    if ((xml_start - length_start) > 1024)
-        return NULL;
-    char str_xml_length[1024];
-    for (i=length_start; i<xml_start; i++) {
-        if (http_header[i] == '\r' && http_header[i+1] == '\n') {
-            str_xml_length[i - length_start] = '\0';
-            break;
-        } else {
-            str_xml_length[i - length_start] = http_header[i];
-        }
-    }
-    int xml_length = (int) strtol(str_xml_length, (char **)NULL, 10);
-    if (xml_length > 65536)
-        return NULL;
-    char xml_reply[65536];
-
-    for (i=0; i<valread-xml_start; i++) {
-        xml_reply[i] = buffer[i+xml_start];
-    }
-
-    int cumulative_read = valread - xml_start;
-    while (cumulative_read < xml_length) {
-        valread = recv(sock, buffer, buffer_size, 0);
-        for (i=0; i<valread; i++) {
-            xml_reply[i+cumulative_read] = buffer[i];
-        }
-        cumulative_read = cumulative_read + valread;
-    }
-    xml_reply[xml_length] = '\0';
-
-#ifdef _WIN32
-    closesocket(sock);
-    WSACleanup();
-#else
-    close(sock);
-#endif
-
-    xmlDocPtr reply = xmlParseMemory(xml_reply, xml_length);
-    char error_msg[1024] = {0};
-
-    /* Dump reply if requested */
-    if (dump_reply) {
-        dumpReply(reply);
-    }
-
-    return reply;
-}
-
-int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]) {
-    if (getXmlValue(doc, BAD_CAST "//s:Body//s:Fault//s:Code//s:Subcode//s:Value", error_msg, 1024) == 0) {
-        return -1;
-    }
-    else if (getXmlValue(doc, BAD_CAST "//s:Body//s:Fault//s:Reason//s:Text", error_msg, 1024) == 0) {
-        return -1;
-    }
-    return 0;
-}
-
-void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char *user, char *password, time_t offset) {
-    srand (time(NULL));
-
-#ifdef _WIN32
-    _setmode(0, O_BINARY);
-#endif
-
-    unsigned int nonce_chunk_size = 20;
-    unsigned char nonce_buffer[20];
-    char nonce_base64[1024] = {0};
-    char time_holder[1024] = {0};
-    char digest_base64[1024] = {0};
-
-    for (int i=0; i<nonce_chunk_size; i++) {
-        nonce_buffer[i] = (unsigned char)rand();
-    }
-
-    unsigned char nonce_result[30];
-
-    getBase64(nonce_buffer, nonce_chunk_size, nonce_result);
-    strcpy(nonce_base64, (const char *)nonce_result);
-
-    char time_buffer[1024];
-    time_t now = time(NULL);
-    now = now + offset;
-    size_t time_buffer_length = strftime(time_buffer, 1024, "%Y-%m-%dT%H:%M:%S.", gmtime(&now));
-    time_buffer[time_buffer_length] = '\0';
-    int millisec;
-    struct timeval tv;
-#ifdef _WIN32
-    static const uint64_t EPOCH = ((uint64_t) 116444736000000000ULL);
-
-    SYSTEMTIME  system_time;
-    FILETIME    file_time;
-    uint64_t    time;
-
-    GetSystemTime( &system_time );
-    SystemTimeToFileTime( &system_time, &file_time );
-    time =  ((uint64_t)file_time.dwLowDateTime )      ;
-    time += ((uint64_t)file_time.dwHighDateTime) << 32;
-
-    tv.tv_sec  = (long) ((time - EPOCH) / 10000000L);
-    tv.tv_usec = (long) (system_time.wMilliseconds * 1000);
-#else
-    gettimeofday(&tv, NULL);
-#endif
-    millisec = tv.tv_usec/1000.0;
-    char milli_buf[16] = {0};
-    sprintf(milli_buf, "%03dZ", millisec);
-    strcat(time_buffer, milli_buf);
-
-    unsigned char hash[20];
-
-    SHA1_CTX ctx;
-    SHA1Init(&ctx);
-    SHA1Update(&ctx, nonce_buffer, nonce_chunk_size);
-    SHA1Update(&ctx, (const unsigned char *)time_buffer, strlen(time_buffer));
-    SHA1Update(&ctx, (const unsigned char *)password, strlen(password));
-    SHA1Final(hash, &ctx);
-
-    unsigned int digest_chunk_size = SHA1_DIGEST_SIZE;
-    unsigned char digest_result[128];
-    getBase64(hash, digest_chunk_size, digest_result);
-
-    strcpy(time_holder, time_buffer);
-    strcpy(digest_base64, (const char *)digest_result);
-
-    xmlNsPtr ns_wsse = xmlNewNs(root, BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd", BAD_CAST "wsse");
-    xmlNsPtr ns_wsu = xmlNewNs(root, BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd", BAD_CAST "wsu");
-    xmlNodePtr header = xmlNewTextChild(root, ns_env, BAD_CAST "Header", NULL);
-    xmlNodePtr security = xmlNewTextChild(header, ns_wsse, BAD_CAST "Security", NULL);
-    xmlNewProp(security, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
-    xmlNodePtr username_token = xmlNewTextChild(security, ns_wsse, BAD_CAST "UsernameToken", NULL);
-    xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Username", BAD_CAST user);
-    xmlNodePtr pwd = xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Password", BAD_CAST digest_base64);
-    xmlNewProp(pwd, BAD_CAST "Type", BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordDigest");
-    xmlNodePtr nonce = xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Nonce", BAD_CAST nonce_base64);
-    xmlNewProp(nonce, BAD_CAST "EncodingType", BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary");
-    xmlNewTextChild(username_token, ns_wsu, BAD_CAST "Created", BAD_CAST time_holder);
-}
-
-void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result) {
-    char *c = (char *)result;
-    int cnt = 0;
-    base64_encodestate s;
-    base64_init_encodestate(&s);
-    cnt = base64_encode_block((char *)buffer, chunk_size, c, &s);
-    c += cnt;
-    cnt = base64_encode_blockend(c, &s);
-    c += cnt;
-    *c = 0;
-}
-
-void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char *xaddrs, char *post_type, char cmd[], int cmd_length) {
-    xmlOutputBufferPtr outputbuffer = xmlAllocOutputBuffer(NULL);
-    xmlNodeDumpOutput(outputbuffer, doc, root, 0, 0, NULL);
-    int size = xmlOutputBufferGetSize(outputbuffer);
-
-    char xml[8192] = {0};
-    if (size > 8191) {
-        fprintf(stderr, "xmlOutputBufferGetSize too big %d\n", size);
-        strncat(xml, (char*)xmlOutputBufferGetContent(outputbuffer), 8191);
-    } else {
-        strcpy(xml, (char*)xmlOutputBufferGetContent(outputbuffer));
-    }
-
-
-    xmlOutputBufferFlush(outputbuffer);
-    xmlOutputBufferClose(outputbuffer);
-    xmlFreeDoc(doc);
-
-    char c_xml_size[6];
-    sprintf(c_xml_size, "%d", size);
-    int xml_size_length = strlen(c_xml_size)+1;
-
-    char tmp[128] = {0};
-    char * mark = strstr(xaddrs, "//");
-    int start = mark-xaddrs+2;
-    int tmp_len = strlen(xaddrs);
-    int j;
-    for (j=0; j<tmp_len-start; j++) {
-        tmp[j] = xaddrs[j+start];
-    }
-    tmp[j] = '\0';
-
-    mark = strstr(tmp, "/");
-    int end = mark-tmp;
-    char tmp2[128] = {0};
-    for (j=0; j<end; j++) {
-        tmp2[j] = tmp[j];
-    }
-    tmp2[j] = '\0';
-
-    char host[128] = {0};
-    char port_buf[128] = {0};
-    mark = strstr(tmp2, ":");
-    if (mark == NULL) {
-        strcpy(host, tmp2);
-        strcpy(port_buf, "80");
-    } else {
-        start = mark-tmp2;
-        for (j=0; j<start; j++) {
-            host[j] = tmp2[j];
-        }
-        host[j] = '\0';
-        tmp_len = strlen(tmp2);
-        for (j=start+1; j<tmp_len; j++) {
-            port_buf[j-(start+1)] = tmp2[j];
-        }
-        port_buf[j-(start+1)] = '\0';
-    }
-    int port = atoi(port_buf);
-
-    char content[] =
-    "User-Agent: Generic\r\n"
-    "Connection: Close\r\n"
-    "Accept-Encoding: gzip, deflate\r\n"
-    "Content-Type: application/soap+xml; charset=utf-8;\r\n"
-    "Host: ";
-    char content_length[] = "\r\nContent-Length: ";
-
-    char http_terminate[5];
-    http_terminate[0] = '\r';
-    http_terminate[1] = '\n';
-    http_terminate[2] = '\r';
-    http_terminate[3] = '\n';
-    http_terminate[4] = '\0';
-
-    int p = strlen(post_type)+1;
-    int h = strlen(host)+1;
-    int c = sizeof(content);
-    int cl = sizeof(content_length);
-    int cmd_size = p + c + h + cl + xml_size_length + size + 1;
-    int i;
-    int s;
-    for (i=0; i<p-1; i++)
-        cmd[i] = post_type[i];
-    s = i;
-    for (i=0; i<c-1; i++)
-        cmd[s+i] = content[i];
-    s = s+i;
-    for (i=0; i<h-1; i++)
-        cmd[s+i] = host[i];
-    s = s+i;
-    for (i=0; i<cl-1; i++)
-        cmd[s+i] = content_length[i];
-    s = s+i;
-    for (i=0; i<xml_size_length-1; i++)
-        cmd[s+i] = c_xml_size[i];
-    s = s+i;
-    for (i=0; i<5-1; i++)
-        cmd[s+i] = http_terminate[i];
-    s = s+i;
-    for (i=0; i<size; i++)
-        cmd[s+i] = xml[i];
-    cmd[cmd_size] = '\0';
-}
-
-void getUUID(char uuid_buf[47]) {
-    srand(time(NULL));
-    strcpy(uuid_buf, "urn:uuid:");
-    for (int i=0; i<16; i++) {
-        char buf[3];
-        sprintf(buf, "%02x", (unsigned char) rand());
-        strcat(uuid_buf, buf);
-        if (i==3 || i==5 || i==7 || i==9)
-            strcat(uuid_buf, "-");
-    }
-}
-
-int broadcast(struct OnvifSession *onvif_session) {
-    strcpy(preferred_network_address, onvif_session->preferred_network_address);
-    struct sockaddr_in broadcast_address;
-    int broadcast_socket;
-    char broadcast_message[1024] = {0};
-    unsigned int address_size;
-    int error_code;
-
-    if (onvif_session->discovery_msg_id == 1)
-        getDiscoveryXml(broadcast_message, 1024, onvif_session->uuid);
-    else if (onvif_session->discovery_msg_id == 2)
-        getDiscoveryXml2(broadcast_message, 1024);
-
-    int broadcast_message_length = strlen(broadcast_message);
-    broadcast_socket = socket(AF_INET, SOCK_DGRAM, IPPROTO_UDP);
-    setSocketOptions(broadcast_socket);
-    for (int k=0; k<128; k++) {
-        for (int j=0; j<8192; j++) {
-            onvif_session->buf[k][j] = '\0';
-        }
-    }
-
-    memset((char *) &broadcast_address, 0, sizeof(broadcast_address));
-    broadcast_address.sin_family = AF_INET;
-    broadcast_address.sin_port = htons(3702);
-    broadcast_address.sin_addr.s_addr = inet_addr("239.255.255.250");
-    int status = sendto(broadcast_socket, broadcast_message, broadcast_message_length, 0, (struct sockaddr*)&broadcast_address, sizeof(broadcast_address));
-    if (status < 0) {
-        //error
-    }
-
-    int i = 0;
-    unsigned char looping = 1;
-    address_size = sizeof(broadcast_address);
-    while(looping) {
-        onvif_session->len[i] = recvfrom(broadcast_socket, onvif_session->buf[i], sizeof(onvif_session->buf[i]), 0, (struct sockaddr*) &broadcast_address, &address_size);
-        if (onvif_session->len[i] > 0) {
-            onvif_session->buf[i][onvif_session->len[i]] = '\0';
-            i++;
-        } else {
-            looping = 0;
-            if (onvif_session->len[i] < 0) {
-                //error
-            }
-        }
-    }
-
-#ifdef _WIN32
-    closesocket(broadcast_socket);
-#else
-    close(broadcast_socket);
-#endif
-
-    return i;
-}
-
-void getActiveNetworkInterfaces(struct OnvifSession* onvif_session)
-{
-#ifdef _WIN32
-    PIP_ADAPTER_INFO pAdapterInfo;
-    PIP_ADAPTER_INFO pAdapter = NULL;
-    DWORD dwRetVal = 0;
-    int count = 0;
-
-    ULONG ulOutBufLen = sizeof (IP_ADAPTER_INFO);
-    pAdapterInfo = (IP_ADAPTER_INFO *) malloc(sizeof (IP_ADAPTER_INFO));
-    if (pAdapterInfo == NULL) {
-        printf("Error allocating memory needed to call GetAdaptersinfo\n");
-        return;
-    }
-
-    if (GetAdaptersInfo(pAdapterInfo, &ulOutBufLen) == ERROR_BUFFER_OVERFLOW) {
-        free(pAdapterInfo);
-        pAdapterInfo = (IP_ADAPTER_INFO *) malloc(ulOutBufLen);
-        if (pAdapterInfo == NULL) {
-            printf("Error allocating memory needed to call GetAdaptersinfo\n");
-            return;
-        }
-    }
-
-    if ((dwRetVal = GetAdaptersInfo(pAdapterInfo, &ulOutBufLen)) == NO_ERROR) {
-        pAdapter = pAdapterInfo;
-        while (pAdapter) {
-            if (strcmp(pAdapter->IpAddressList.IpAddress.String, "0.0.0.0")) {
-                char interface_info[1024];
-                sprintf(interface_info, "%s - %s", pAdapter->IpAddressList.IpAddress.String, pAdapter->Description);
-                printf("Network interface info %s\n", interface_info);
-                //args.push_back(interface_info);
-                strncpy(onvif_session->active_network_interfaces[count], interface_info, 40);
-                count += 1;
-            }
-            pAdapter = pAdapter->Next;
-        }
-    } 
-    else {
-        printf("GetAdaptersInfo failed with error: %d", dwRetVal);
-    }
-    if (pAdapterInfo)
-        free(pAdapterInfo);
-#else
-    struct ifaddrs *ifaddr;
-    int family, s;
-    char host[NI_MAXHOST];
-    int count = 0;
-
-    if (getifaddrs(&ifaddr) == -1) {
-        printf("Error: getifaddrs failed - %s\n", strerror(errno));
-        return;
-    }
-
-    for (struct ifaddrs *ifa = ifaddr; ifa != NULL; ifa = ifa->ifa_next) {
-        if (ifa->ifa_addr == NULL)
-            continue;
-
-        family = ifa->ifa_addr->sa_family;
-
-        if (family == AF_INET ) {
-            s = getnameinfo(ifa->ifa_addr, 
-                    sizeof(struct sockaddr_in),
-                    host, NI_MAXHOST,
-                    NULL, 0, NI_NUMERICHOST);
-
-            if (s != 0) {
-                printf("getnameinfo() failed: %s\n", gai_strerror(s));
-                continue;
-            }
-
-            if (strcmp(ifa->ifa_name, "lo")) {
-                strcpy(onvif_session->active_network_interfaces[count], host);
-                strcat(onvif_session->active_network_interfaces[count], " - ");
-                strcat(onvif_session->active_network_interfaces[count], ifa->ifa_name);
-                count += 1;
-            }
-        } 
-    }
-    freeifaddrs(ifaddr);
-#endif
-}
-
-void getIPAddress(char buf[128]) {
-#ifdef _WIN32
-    PMIB_IPADDRTABLE pIPAddrTable;
-    DWORD dwSize = 0;
-    DWORD dwRetVal = 0;
-    IN_ADDR IPAddr;
-    
-    pIPAddrTable = (MIB_IPADDRTABLE *) malloc(sizeof(MIB_IPADDRTABLE));
-    if (pIPAddrTable) {
-        if (GetIpAddrTable(pIPAddrTable, &dwSize, 0) == ERROR_INSUFFICIENT_BUFFER) {
-            free(pIPAddrTable);
-            pIPAddrTable = (MIB_IPADDRTABLE *) malloc(dwSize);
-        }
-        if (pIPAddrTable == NULL) {
-            return;
-        }
-    }
-
-    if ((dwRetVal = GetIpAddrTable(pIPAddrTable, &dwSize, 0)) != NO_ERROR) {
-        return;
-    }
-
-    int p = 0;
-    while (p < (int)pIPAddrTable->dwNumEntries) {
-        if (pIPAddrTable->table[p].dwAddr != inet_addr("127.0.0.1") && pIPAddrTable->table[p].dwMask == inet_addr("255.255.255.0")) {
-            IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwAddr;
-            strcpy(buf, inet_ntoa(IPAddr));
-            p = (int)pIPAddrTable->dwNumEntries;
-        }
-        p++;
-    }
-
-    if (pIPAddrTable) {
-        free(pIPAddrTable);
-        pIPAddrTable = NULL;
-    }
-
-#else
-
-#if defined(__APPLE__) || defined(__FreeBSD__)
-
-    char *address;
-    struct ifaddrs *interfaces = NULL;
-    struct ifaddrs *temp_addr = NULL;
-    int success = 0;
-    success = getifaddrs(&interfaces);
-    if (success == 0) {
-        temp_addr = interfaces;
-        while (temp_addr != NULL) {
-            address = inet_ntoa(((struct sockaddr_in *)temp_addr->ifa_addr)->sin_addr);
-            if (strcmp(address, "127.0.0.1") != 0)
-                strcpy(buf, address);
-        }
-        temp_addr = temp_addr->ifa_next;
-    }
-    freeifaddrs(interfaces);
-
-#else
-    struct ifconf ifc;
-    struct ifreq ifr[10];
-    int sd, ifc_num, addr,mask, i;
-
-    sd = socket(PF_INET, SOCK_DGRAM, 0);
-    if (sd > 0) {
-        ifc.ifc_len = sizeof(ifr);
-        ifc.ifc_ifcu.ifcu_buf = (caddr_t)ifr;
-
-        if (ioctl(sd, SIOCGIFCONF, &ifc) == 0) {
-            ifc_num = ifc.ifc_len / sizeof(struct ifreq);
-
-            for (i = 0; i < ifc_num; ++i) {
-                if (ifr[i].ifr_addr.sa_family != AF_INET) {
-                    continue;
-                }
-
-                if (ioctl(sd, SIOCGIFNETMASK, &ifr[i]) == 0) {
-                    mask = ((struct sockaddr_in *)(&ifr[i].ifr_netmask))->sin_addr.s_addr;
-                    char mask_buf[128];
-                    sprintf(mask_buf, "%d.%d.%d.%d", INT_TO_ADDR(mask));
-                    if (strcmp(mask_buf, "255.255.255.0") == 0) {
-                        if (ioctl(sd, SIOCGIFADDR, &ifr[i]) == 0) {
-                            addr = ((struct sockaddr_in *)(&ifr[i].ifr_addr))->sin_addr.s_addr;
-                            char addr_buf[128];
-                            sprintf(addr_buf, "%d.%d.%d.%d", INT_TO_ADDR(addr));
-                            if (strcmp(addr_buf, "127.0.0.1") != 0) {
-                                printf("-----------------------------------------------%s\n", addr_buf);
-                                strcpy(buf, addr_buf);
-                            }
-                        }
-                    }
-                }
-            }
-        }
-    }
-    close(sd);
-#endif /* not  __APPLE__ || __FreeBSD__ */
-#endif /* not _WIN32 */
-}
-
-int mask2prefix(char *mask_buf) {
-    struct in_addr mask;
-    inet_pton(AF_INET, mask_buf, &mask);
-    uint32_t number = ntohl(mask.s_addr);
-    int count = 0;
-    unsigned int step = 0;
-    while (number > 0) {
-        if (number & 1) {
-            step = 1;
-            count++;
-        } else {
-            if (step) {
-                return -1;
-            }
-        }
-        number >>=1;
-    }
-    return count;
-}
-
-void prefix2mask(int prefix, char mask_buf[128]) {
-    struct in_addr mask;
-    uint32_t number;
-
-    if (prefix) {
-        number = htonl(~((1 << (32-prefix)) - 1));
-    } else {
-        number = htonl(0);
-    }
-
-    mask.s_addr = number;
-    inet_ntop(AF_INET, &mask, mask_buf, 128);
-}
-
-int setSocketOptions(int socket) {
-    struct timeval tv;
-    tv.tv_sec = 0;
-    tv.tv_usec = 500000;
-    int broadcast = 500;
-    char loopch = 0;
-    int status = 0;
-    struct in_addr localInterface;
-
-#ifdef _WIN32
-    PMIB_IPADDRTABLE pIPAddrTable;
-    DWORD dwSize = 0;
-    DWORD dwRetVal = 0;
-    IN_ADDR IPAddr;
-
-    pIPAddrTable = (MIB_IPADDRTABLE *) malloc(sizeof(MIB_IPADDRTABLE));
-    if (pIPAddrTable) {
-        if (GetIpAddrTable(pIPAddrTable, &dwSize, 0) == ERROR_INSUFFICIENT_BUFFER) {
-            free(pIPAddrTable);
-            pIPAddrTable = (MIB_IPADDRTABLE *) malloc(dwSize);
-        }
-        if (pIPAddrTable == NULL) {
-            printf("Memory allocation failed for GetIpAddrTable\n");
-            return -1;
-        }
-    }
-
-    if ((dwRetVal = GetIpAddrTable(pIPAddrTable, &dwSize, 0)) != NO_ERROR) {
-        printf("GetIpAddrTable failed with error %d\n", dwRetVal);
-        return -1;
-    }
-
-    int p = 0;
-    while (p < (int)pIPAddrTable->dwNumEntries) {
-        IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwAddr;
-        IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwMask;
-        if (pIPAddrTable->table[p].dwAddr != inet_addr("127.0.0.1") && pIPAddrTable->table[p].dwMask == inet_addr("255.255.255.0")) {
-            if (strlen(preferred_network_address) > 0) {
-                localInterface.s_addr = inet_addr(preferred_network_address);
-            }
-            else {
-                localInterface.s_addr = pIPAddrTable->table[p].dwAddr;
-            }
-            status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_IF, (const char *)&localInterface, sizeof(localInterface));
-            if (status < 0)
-                printf("ip_multicast_if error");
-            p = (int)pIPAddrTable->dwNumEntries;
-        }
-        p++;
-    }
-
-    if (pIPAddrTable) {
-        free(pIPAddrTable);
-        pIPAddrTable = NULL;
-    }
-
-    status = setsockopt(socket, SOL_SOCKET, SO_RCVTIMEO, (const char *)&broadcast, sizeof(broadcast));
-#else
-    if (strlen(preferred_network_address) > 0) {
-        localInterface.s_addr = inet_addr(preferred_network_address);
-        status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_IF, (const char *)&localInterface, sizeof(localInterface));
-        if (status < 0)
-            printf("ip_multicast_if error");
-    }
-    status = setsockopt(socket, SOL_SOCKET, SO_RCVTIMEO, (struct timeval *)&tv, sizeof(struct timeval));
-#endif
-    status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_LOOP, (char *)&loopch, sizeof(loopch));
-    return 0;
-}
-
-
-
-#ifdef __MINGW32__
-int inet_pton(int af, const char *src, void *dst) {
-    struct sockaddr_storage ss;
-    int size = sizeof(ss);
-    char src_copy[INET6_ADDRSTRLEN+1];
-
-    ZeroMemory(&ss, sizeof(ss));
-    strncpy (src_copy, src, INET6_ADDRSTRLEN+1);
-    src_copy[INET6_ADDRSTRLEN] = 0;
-
-    if (WSAStringToAddress(src_copy, af, NULL, (struct sockaddr *)&ss, &size) == 0) {
-        switch(af) {
-	case AF_INET:
-	    *(struct in_addr *)dst = ((struct sockaddr_in *)&ss)->sin_addr;
-	    return 1;
-	case AF_INET6:
-	    *(struct in6_addr *)dst = ((struct sockaddr_in6 *)&ss)->sin6_addr;
-	    return 1;
-	}
-    }
-    return 0;
-}
-
-const char *inet_ntop(int af, const void *src, char *dst, socklen_t size) {
-    struct sockaddr_storage ss;
-    unsigned long s = size;
-
-    ZeroMemory(&ss, sizeof(ss));
-    ss.ss_family = af;
-
-    switch(af) {
-    case AF_INET:
-        ((struct sockaddr_in *)&ss)->sin_addr = *(struct in_addr *)src;
-	break;
-    case AF_INET6:
-        ((struct sockaddr_in6 *)&ss)->sin6_addr = *(struct in6_addr *)src;
-	break;
-    default:
-        return NULL;
-    }
-
-    return (WSAAddressToString((struct sockaddr *)&ss, sizeof(ss), NULL, dst, &s) == 0)?dst : NULL;
-}
-#endif
-
-
-void extractOnvifService(char service[1024], bool post) {
-    int length = strlen(service);
-    char *sub = strstr(service, "//");
-    if (sub != NULL) {
-        int mark = sub - service;
-        mark = mark+2;
-
-        int i;
-        for (i=0; i<length-mark; i++) {
-            service[i] = service[i+mark];
-        }
-        service[i] = '\0';
-
-        sub = strstr(service, " ");
-        if (sub != NULL) {
-            mark = sub - service;
-            service[mark] = '\0';
-        }
-
-        length = strlen(service);
-        sub = strstr(service, "/");
-        if (sub != NULL) {
-            mark = sub - service;
-            for (i=0; i<length-mark; i++) {
-                service[i] = service[i+mark];
-            }
-            service[i] = 0;
-
-            if (post) {
-                char temp_buf[128] = {0};
-                strcat(temp_buf, "POST ");
-                strcat(temp_buf, service);
-                strcat(temp_buf, " HTTP/1.1\r\n");
-                strcpy(service, "");
-                strcpy(service, temp_buf);
-            }
-        }
-    }
-}
-
-
-void extractHost(char *xaddrs, char host[128]) {
-    char tmp[128] = {0};
-    char *mark = strstr(xaddrs, "//");
-    int start = mark-xaddrs+2;
-    int tmp_len = strlen(xaddrs);
-    int j;
-    for (j=0; j<tmp_len-start; j++) {
-        tmp[j] = xaddrs[j+start];
-    }
-    tmp[j] = '\0';
-
-    mark = strstr(tmp, "/");
-    int end = mark-tmp;
-    char tmp2[128] = {0};
-    for (j=0; j<end; j++) {
-        tmp2[j] = tmp[j];
-    }
-    tmp2[j] = '\0';
-
-    mark = strstr(tmp2, ":");
-    if (mark == NULL) {
-        strcpy(host, tmp2);
-    } else {
-        start = mark-tmp2;
-        for (j=0; j<start; j++) {
-            host[j] = tmp2[j];
-        }
-        host[j] = '\0';
-    }
-}
-
-void getScopeField(char *scope, char *field_name, char cleaned[1024]) {
-    char *field;
-    char field_contents[1024] = {0};
-    char *mark;
-    int length;
-    char *result = NULL;
-
-    field = strstr(scope, field_name);
-    if (field != NULL) {
-        field = field + strlen(field_name);
-        mark = strstr(field, " ");
-        if (mark != NULL) {
-            length = mark - field;
-            strncpy(field_contents, field, length);
-        } else {
-            strcpy(field_contents, field);
-        }
-
-        length = strlen(field_contents);
-        int offset = 0;
-        int j;
-        for (int i=0; i<length; i++) {
-            j = i - offset;
-            if (field_contents[i] == '%') {
-                char middle[3] = {0};
-                i++; offset++;
-                middle[0] = field_contents[i];
-                i++; offset++;
-                middle[1] = field_contents[i];
-                char *ptr;
-                int result = strtol(middle, &ptr, 16);
-                cleaned[j] = result;
-            } else {
-                cleaned[j] = field_contents[i];
-            }
-        }
-        cleaned[length] = '\0';
-    }
-}
-
-void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
-    xmlDocPtr xml_input = xmlParseMemory(onvif_session->buf[ordinal], onvif_session->len[ordinal]);
-    for(int i=0; i<1024; i++)
-        onvif_data->camera_name[i] = '\0';
-
-    char scopes[8192];
-    getXmlValue(xml_input, BAD_CAST "//s:Body//d:ProbeMatches//d:ProbeMatch//d:Scopes", scopes, 8192);
-
-    char temp_mfgr[1024] = {0};
-    char temp_hdwr[1024] = {0};
-
-    getScopeField(scopes, "onvif://www.onvif.org/name/", temp_mfgr);
-    getScopeField(scopes, "onvif://www.onvif.org/hardware/", temp_hdwr);
-
-    if (strlen(temp_mfgr) > 0) {
-        strcat(onvif_data->camera_name, temp_mfgr);
-    }
-    if (strlen(temp_hdwr) > 0) {
-        if (strstr(temp_mfgr, temp_hdwr) == NULL) {
-            strcat(onvif_data->camera_name, " ");
-            strcat(onvif_data->camera_name, temp_hdwr);
-        }
-    }
-
-    if (strlen(onvif_data->camera_name)  == 0)
-        strcpy(onvif_data->camera_name, "UNKNOWN CAMERA");
-
-    xmlFreeDoc(xml_input);
-}
-
-bool extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
-    bool result = false;
-    xmlDocPtr xml_input = xmlParseMemory(onvif_session->buf[ordinal], onvif_session->len[ordinal]);
-    if (getXmlValue(xml_input, BAD_CAST "//s:Body//d:ProbeMatches//d:ProbeMatch//d:XAddrs", onvif_data->xaddrs, 1024) == 0) {
-        char *sub = strstr(onvif_data->xaddrs, " ");
-        if (sub != NULL) {
-            int mark = sub - onvif_data->xaddrs;
-            onvif_data->xaddrs[mark] = '\0';
-        }
-        strcpy(onvif_data->device_service, onvif_data->xaddrs);
-        result = true;
-    }
-    xmlFreeDoc(xml_input);
-    return result;
-}
-
-void clearData(struct OnvifData *onvif_data) {
-    for (int i=0; i<16; i++) {
-        for (int j=0; j<128; j++) {
-            onvif_data->resolutions_buf[i][j] = '\0';
-        }
-    }
-    for (int i=0; i<128; i++) {
-        onvif_data->videoEncoderConfigurationToken[i] = '\0';
-        onvif_data->networkInterfaceToken[i] = '\0';
-        onvif_data->networkInterfaceName[i] = '\0';
-        onvif_data->ip_address_buf[i] = '\0';
-        onvif_data->default_gateway_buf[i] = '\0';
-        onvif_data->dns_buf[i] = '\0';
-        onvif_data->mask_buf[i] = '\0';
-        onvif_data->videoSourceConfigurationToken[i] = '\0';
-        onvif_data->video_encoder_name_buf[i] = '\0';
-        onvif_data->h264_profile_buf[i] = '\0';
-        onvif_data->multicast_address_type_buf[i] = '\0';
-        onvif_data->multicast_address_buf[i] = '\0';
-        onvif_data->session_time_out_buf[i] = '\0';
-        onvif_data->media_service[i] = '\0';
-        onvif_data->imaging_service[i] = '\0';
-        onvif_data->ptz_service[i] = '\0';
-        onvif_data->event_service[i] = '\0';
-        onvif_data->profileToken[i] = '\0';
-        onvif_data->username[i] = '\0';
-        onvif_data->password[i] = '\0';
-        onvif_data->encoding[i] = '\0';
-    	onvif_data->timezone[i] = '\0';
-    	onvif_data->ntp_type[i] = '\0';
-    	onvif_data->ntp_addr[i] = '\0';
-        onvif_data->host[i] = '\0';
-        onvif_data->serial_number[i] = '\0';
-    }
-    for (int i=0; i<1024; i++) {
-        onvif_data->xaddrs[i] = '\0';
-        onvif_data->device_service[i] = '\0';
-        onvif_data->stream_uri[i] = '\0';
-        onvif_data->camera_name[i] = '\0';
-        onvif_data->host_name[i] = '\0';
-    }
-    onvif_data->gov_length_min = 0;
-    onvif_data->gov_length_max = 0;
-    onvif_data->frame_rate_min = 0;
-    onvif_data->frame_rate_max = 0;
-    onvif_data->bitrate_min = 0;
-    onvif_data->bitrate_max = 0;
-    onvif_data->width = 0;
-    onvif_data->height = 0;
-    onvif_data->gov_length = 0;
-    onvif_data->frame_rate = 0;
-    onvif_data->bitrate = 0;
-    onvif_data->use_count = 0;
-    onvif_data->quality = 0;
-    onvif_data->multicast_port = 0;
-    onvif_data->multicast_ttl = 0;
-    onvif_data->autostart = false;
-    onvif_data->prefix_length = 0;
-    onvif_data->dhcp_enabled = false;
-    onvif_data->brightness_min = 0;
-    onvif_data->brightness_max = 0;
-    onvif_data->saturation_min = 0;
-    onvif_data->saturation_max = 0;
-    onvif_data->contrast_min = 0;
-    onvif_data->contrast_max = 0;
-    onvif_data->sharpness_min = 0;
-    onvif_data->sharpness_max = 0;
-    onvif_data->brightness = 0;
-    onvif_data->saturation = 0;
-    onvif_data->contrast = 0;
-    onvif_data->sharpness = 0;
-    onvif_data->time_offset = 0;
-    onvif_data->event_listen_port = 0;
-    onvif_data->guaranteed_frame_rate = false;
-    onvif_data->conf_width = 0;
-    onvif_data->conf_height = 0;
-    onvif_data->conf_frame_rate_limit = 0;
-    onvif_data->conf_encoding_interval = 0;
-    onvif_data->conf_bitrate_limit = 0;
-    onvif_data->datetimetype = '\0';
-    onvif_data->dst = false;
-    onvif_data->ntp_dhcp = false;
-}
-
-void copyData(struct OnvifData *dst, struct OnvifData *src) {
-    for (int i=0; i<16; i++) {
-        for (int j=0; j<128; j++) {
-            dst->resolutions_buf[i][j] = src->resolutions_buf[i][j];
-        }
-    }
-    for (int i=0; i<128; i++) {
-        dst->videoEncoderConfigurationToken[i] = src->videoEncoderConfigurationToken[i];
-        dst->networkInterfaceToken[i] = src->networkInterfaceToken[i];
-        dst->networkInterfaceName[i] = src->networkInterfaceName[i];
-        dst->ip_address_buf[i] = src->ip_address_buf[i];
-        dst->default_gateway_buf[i] = src->default_gateway_buf[i];
-        dst->dns_buf[i] = src->dns_buf[i];
-        dst->videoSourceConfigurationToken[i] = src->videoSourceConfigurationToken[i];
-        dst->video_encoder_name_buf[i] = src->video_encoder_name_buf[i];
-        dst->h264_profile_buf[i] = src->h264_profile_buf[i];
-        dst->multicast_address_type_buf[i] = src->multicast_address_type_buf[i];
-        dst->multicast_address_buf[i] = src->multicast_address_buf[i];
-        dst->session_time_out_buf[i] = src->session_time_out_buf[i];
-        dst->media_service[i] = src->media_service[i];
-        dst->imaging_service[i] = src->imaging_service[i];
-        dst->ptz_service[i] = src->ptz_service[i];
-        dst->event_service[i] = src->event_service[i];
-        dst->profileToken[i] = src->profileToken[i];
-        dst->username[i] = src->username[i];
-        dst->password[i] = src->password[i];
-        dst->encoding[i] = src->encoding[i];
-    	dst->timezone[i] = src->timezone[i];
-    	dst->ntp_type[i] = src->ntp_type[i];
-    	dst->ntp_addr[i] = src->ntp_addr[i];
-        dst->host[i] = src->host[i];
-        dst->serial_number[i] = src->serial_number[i];
-    }
-    for (int i=0; i<1024; i++) {
-        dst->xaddrs[i] = src->xaddrs[i];
-        dst->device_service[i] = src->device_service[i];
-        dst->stream_uri[i] = src->stream_uri[i];
-        dst->camera_name[i] = src->camera_name[i];
-        dst->host_name[i] = src->host_name[i];
-        dst->last_error[i] = src->last_error[i];
-    }
-    dst->gov_length_min = src->gov_length_min;
-    dst->gov_length_max = src->gov_length_max;
-    dst->frame_rate_min = src->frame_rate_min;
-    dst->frame_rate_max = src->frame_rate_max;
-    dst->bitrate_min = src->bitrate_min;
-    dst->bitrate_max = src->bitrate_max;
-    dst->width = src->width;
-    dst->height = src->height;
-    dst->gov_length = src->gov_length;
-    dst->frame_rate = src->frame_rate;
-    dst->bitrate = src->bitrate;
-    dst->use_count = src->use_count;
-    dst->quality = src->quality;
-    dst->multicast_port = src->multicast_port;
-    dst->multicast_ttl = src->multicast_ttl;
-    dst->autostart = src->autostart;
-    dst->prefix_length = src->prefix_length;
-    dst->dhcp_enabled = src->dhcp_enabled;
-    dst->brightness_min = src->brightness_min;
-    dst->brightness_max = src->brightness_max;
-    dst->saturation_min = src->saturation_min;
-    dst->saturation_max = src->saturation_max;
-    dst->contrast_min = src->contrast_min;
-    dst->contrast_max = src->contrast_max;
-    dst->sharpness_min = src->sharpness_min;
-    dst->sharpness_max = src->sharpness_max;
-    dst->brightness = src->brightness;
-    dst->saturation = src->saturation;
-    dst->contrast = src->contrast;
-    dst->sharpness = src->sharpness;
-    dst->time_offset = src->time_offset;
-    dst->event_listen_port = src->event_listen_port;
-    dst->guaranteed_frame_rate = src->guaranteed_frame_rate;
-    dst->conf_width = src->conf_width;
-    dst->conf_height = src->conf_height;
-    dst->conf_frame_rate_limit = src->conf_frame_rate_limit;
-    dst->conf_encoding_interval = src->conf_encoding_interval;
-    dst->conf_bitrate_limit = src->conf_bitrate_limit;
-    dst->datetimetype = src->datetimetype;
-    dst->dst = src->dst;
-    dst->ntp_dhcp = src->ntp_dhcp;
-}
-
-void initializeSession(struct OnvifSession *onvif_session) {
-    getUUID(onvif_session->uuid);
-    onvif_session->discovery_msg_id = 1;
-    xmlInitParser ();
-    for (int i=0; i<16; i++) {
-        for (int j=0; j<1024; j++) {
-            onvif_session->active_network_interfaces[i][j] = '\0';
-        }
-    }
-#ifdef _WIN32
-    WSADATA wsaData;
-    WSAStartup(MAKEWORD(2,2), &wsaData);
-#endif
-    strcpy(preferred_network_address, onvif_session->preferred_network_address);
-}
-
-void closeSession(struct OnvifSession *onvif_session) {
-#ifdef _WIN32
-    WSACleanup();
-#endif
-    xmlCleanupParser ();
-}
-
-bool prepareOnvifData(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
-    clearData(onvif_data);
-    getCameraName(ordinal, onvif_session, onvif_data);
-    if (!extractXAddrs(ordinal, onvif_session, onvif_data))
-        return false;
-    extractOnvifService(onvif_data->device_service, true);
-    extractHost(onvif_data->xaddrs, onvif_data->host);
-    getTimeOffset(onvif_data);
-    return true;
-}
-
-int fillRTSPn(struct OnvifData *onvif_data, int profileIndex) {
-    int result = 0;
-    result = getCapabilities(onvif_data);
-    if (result == 0) {
-        result = getProfileToken(onvif_data, profileIndex);
-        if (result == 0) {
-            result = getStreamUri(onvif_data);
-        }
-    }
-    return result;
-}
-
-bool hasPTZ(struct OnvifData* onvif_data) {
-    if (strcmp(onvif_data->ptz_service, "") == 0)
-        return false;
-    else
-        return true;
-
-}
-
-void dumpXmlNode (xmlDocPtr doc, xmlNodePtr cur_node, char *prefix) {
-    const char *name;
-    const char *value;
-    char new_prefix[1024];
-    char attr[128];
-    xmlAttrPtr prop;
-
-    /* Traverse the tree */
-    for (; cur_node; cur_node = cur_node->next) {
-        if (cur_node->type == XML_ELEMENT_NODE) {
-            name = (char *)(cur_node->name);
-            value = (const char *)xmlNodeListGetString(doc, cur_node->xmlChildrenNode, 1);
-            if (value) {
-                printf("%s%s=%s\n", prefix ? prefix : "", name, value);
-            } else {
-                sprintf(new_prefix, "%s%s.", prefix ? prefix : "", name);
-                for (prop = cur_node->properties; prop; prop = prop->next) {
-                    if (prop->children && prop->children->content) {
-                        printf("%s%s=%s\n", new_prefix, prop->name, prop->children->content);
-                    }
-                }
-            }
-        }
-        dumpXmlNode(doc, cur_node->children, new_prefix);
-    }
-}
-
-/* Dump xml document */
-void dumpReply(xmlDocPtr reply) {
-    if (reply != NULL) {
-        xmlChar *xpath = BAD_CAST "//s:Body/*";
-        xmlXPathObjectPtr body = getNodeSet(reply, xpath);
-        if (body) {
-            xmlNodeSetPtr nodeset = body->nodesetval;
-            for (int i=0; i<nodeset->nodeNr; i++) {
-                xmlNodePtr cur = nodeset->nodeTab[i];
-                /* Skip error return */
-                if (strcmp((char *)cur->name, "Fault") != 0) {
-                    printf("[%s]\n", cur->name);
-                    dumpXmlNode(reply, cur->children, NULL);
-                }
-            }
-        }
-    }
-}
-
-/* Dump all available onvif device configuration */
-void dumpConfigAll (struct OnvifData *onvif_data) {
-    xmlDocPtr reply;
-
-    dump_reply = true;
-
-    getNetworkInterfaces(onvif_data);
-    getNetworkDefaultGateway(onvif_data);
-    getDNS(onvif_data);
-    getCapabilities(onvif_data);
-    getVideoEncoderConfigurationOptions(onvif_data);
-    getVideoEncoderConfiguration(onvif_data);
-    getProfile(onvif_data);
-    getOptions(onvif_data);
-    getImagingSettings(onvif_data);
-    getFirstProfileToken(onvif_data);
-    getTimeOffset(onvif_data);
-    getNTP(onvif_data);
-    getHostname(onvif_data);
-    getStreamUri(onvif_data);
-    getDeviceInformation(onvif_data);
-
-    dump_reply = false;
-}
+/*******************************************************************************
+* onvif.c
+*
+* copyright 2018, 2023 Stephen Rhodes
+*
+* This library is free software; you can redistribute it and/or
+* modify it under the terms of the GNU Lesser General Public
+* License as published by the Free Software Foundation; either
+* version 2.1 of the License, or (at your option) any later version.
+*
+* This library is distributed in the hope that it will be useful,
+* but WITHOUT ANY WARRANTY; without even the implied warranty of
+* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+* Lesser General Public License for more details.
+*
+* You should have received a copy of the GNU Lesser General Public
+* License along with this library; if not, write to the Free Software
+* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+*
+*******************************************************************************/
+
+#include <string.h>
+#include <stdio.h>
+#include <stdlib.h>
+#include <math.h>
+#include <sys/stat.h>
+#include <libxml/parser.h>
+#include <libxml/xpath.h>
+#include "libxml/xpathInternals.h"
+
+#ifdef _WIN32
+    #include <ws2tcpip.h>
+    #include <winsock2.h>
+    #include <wincrypt.h>
+    #include <iphlpapi.h>
+    #include <fcntl.h>
+	#pragma comment(lib, "iphlpapi.lib")
+	#pragma comment(lib, "ws2_32.lib")
+#else
+    #include <sys/socket.h>
+    #include <arpa/inet.h>
+    #include <unistd.h>
+    #include <ifaddrs.h>
+    #include <sys/ioctl.h>
+    #include <sys/types.h>
+    #include <netdb.h>
+    #include <net/if.h>
+    #include <netinet/in.h>
+    #include <sys/time.h>
+#endif
+
+#include "onvif.h"
+#include "sha1.h"
+#include "cencode.h"
+#include <stdint.h>
+#include <errno.h>
+
+#define INT_TO_ADDR(_addr) \
+(_addr & 0xFF), \
+(_addr >> 8 & 0xFF), \
+(_addr >> 16 & 0xFF), \
+(_addr >> 24 & 0xFF)
+
+xmlDocPtr sendCommandToCamera(char * cmd, char * xaddrs);
+void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result);
+void getUUID(char uuid_buf[47]);
+void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char * user, char * password, time_t offset);
+void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char * xaddrs, char * post_type, char cmd[], int cmd_length);
+int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]);
+int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length);
+int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex);
+#define getNodeAttribute(doc,xpath,attribute,buf,buf_length) getNodeAttributen(doc,xpath,attribute,buf,buf_length,0)
+xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath);
+
+
+const int SHA1_DIGEST_SIZE = 20;
+char preferred_network_address[16];
+static bool dump_reply = false;
+static void dumpReply(xmlDocPtr reply);
+
+int getNetworkInterfaces(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNetworkInterfaces", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNetworkInterfacesResponse//tds:NetworkInterfaces";
+        xmlNodeSetPtr nodeset;
+        xmlChar *enabled = NULL;
+        xmlXPathObjectPtr xml_result = getNodeSet(reply, xpath);
+        if (xml_result) {
+            nodeset = xml_result->nodesetval;
+            for (int i=0; i<nodeset->nodeNr; i++) {
+                xmlNodePtr cur = nodeset->nodeTab[i];
+                xmlChar *token = xmlGetProp(cur, BAD_CAST "token");
+                xmlDocPtr temp_doc = xmlNewDoc(BAD_CAST "1.0");
+                xmlDocSetRootElement(temp_doc, cur);
+
+                bool dhcp = false;
+                char isDHCP[128];
+                xpath = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:DHCP";
+                if (getXmlValue(temp_doc, xpath, isDHCP, 128) == 0) {
+                    if (strcmp(isDHCP, "true") == 0) {
+                        dhcp = true;
+                    }
+                    onvif_data->dhcp_enabled = dhcp;
+                }
+
+                xmlChar *xpath_address;
+                xmlChar *xpath_prefix;
+                if (dhcp) {
+                    xpath_address = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:FromDHCP//tt:Address";
+                    xpath_prefix = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:FromDHCP//tt:PrefixLength";
+                } else {
+                    xpath_address = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:Manual//tt:Address";
+                    xpath_prefix = BAD_CAST "//tds:NetworkInterfaces//tt:IPv4//tt:Config//tt:Manual//tt:PrefixLength";
+                }
+
+                char ip_address_buf[128];
+                if (getXmlValue(temp_doc, xpath_address, ip_address_buf, 128) == 0) {
+                    char host[128] = {0};
+                    extractHost(onvif_data->xaddrs, host);
+
+                    if (strcmp(ip_address_buf, host) == 0) {
+                        strcpy(onvif_data->ip_address_buf, ip_address_buf);
+                        strcpy(onvif_data->networkInterfaceToken, (char*) token);
+                        char prefix_length_buf[128];
+                        if (getXmlValue(temp_doc, xpath_prefix, prefix_length_buf, 128) ==  0) {
+                            onvif_data->prefix_length = atoi(prefix_length_buf);
+                        }
+                        xpath = BAD_CAST "//tds:NetworkInterfaces//tt:Info//tt:Name";
+                        getXmlValue(temp_doc, xpath, onvif_data->networkInterfaceName, 128);
+                        i = nodeset->nodeNr;
+                    }
+                }
+                xmlFreeDoc(temp_doc);
+            }
+        }
+        if (enabled != NULL) {
+            xmlFree(enabled);
+        }
+        xmlXPathFreeObject(xml_result);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getNetworkInterfaces");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getNetworkInterfaces - No XML reply");
+    }
+    return result;
+}
+
+int setNetworkInterfaces(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setNetworkInterfaces = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNetworkInterfaces", NULL);
+    xmlNewTextChild(setNetworkInterfaces, ns_tt, BAD_CAST "InterfaceToken", BAD_CAST onvif_data->networkInterfaceName);
+    xmlNodePtr networkInterface = xmlNewTextChild(setNetworkInterfaces, ns_tt, BAD_CAST "NetworkInterface", NULL);
+    xmlNodePtr ipv4 = xmlNewTextChild(networkInterface, ns_tt, BAD_CAST "IPv4", NULL);
+    if (onvif_data->dhcp_enabled) {
+        xmlNewTextChild(ipv4, ns_tt, BAD_CAST "DHCP", BAD_CAST "true");
+    } else {
+        xmlNewTextChild(ipv4, ns_tt, BAD_CAST "DHCP", BAD_CAST "false");
+        xmlNodePtr manual = xmlNewTextChild(ipv4, ns_tt, BAD_CAST "Manual", NULL);
+        xmlNewTextChild(manual, ns_tt, BAD_CAST "Address" , BAD_CAST onvif_data->ip_address_buf);
+        char prefix_length_buf[128];
+        sprintf(prefix_length_buf, "%d", onvif_data->prefix_length);
+        xmlNewTextChild(manual, ns_tt, BAD_CAST "PrefixLength", BAD_CAST prefix_length_buf);
+    }
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body//tds:SetNetworkInterfacesResponse//tds:RebootNeeded";
+        char rebootNeeded[128];
+        if (getXmlValue(reply, xpath, rebootNeeded, 128) == 0) {
+            if (strcmp(rebootNeeded, "true") == 0) {
+                rebootCamera(onvif_data);
+            }
+        }
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setNetworkInterfaces");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setNetworkInterfaces - No XML reply");
+    }
+    return result;
+}
+
+int getNetworkDefaultGateway(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNetworkDefaultGateway", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNetworkDefaultGatewayResponse//tds:NetworkGateway//tt:IPv4Address";
+        getXmlValue(reply, xpath, onvif_data->default_gateway_buf, 128);
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getNetworkDefaultGateway");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getNetworkDefaultGateway - No XML reply");
+    }
+    return result;
+}
+
+int setNetworkDefaultGateway(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setNetworkDefaultGateway = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNetworkDefaultGateway", NULL);
+    xmlNewTextChild(setNetworkDefaultGateway, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->default_gateway_buf);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setNetworkDefaultGateway");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setNetworkDefaultGateway - No XML reply");
+    }
+    return result;
+}
+
+int getDNS(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDNS", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:FromDHCP";
+        char fromDHCP[128];
+        if (getXmlValue(reply, xpath, fromDHCP, 128) == 0) {
+            if (strcmp(fromDHCP, "true") == 0) {
+                xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:DNSFromDHCP//tt:IPv4Address";
+                if (getXmlValue(reply, xpath, onvif_data->dns_buf, 128) == 0) {}
+            } else {
+                xpath = BAD_CAST "//s:Body//tds:GetDNSResponse//tds:DNSInformation//tt:DNSManual//tt:IPv4Address";
+                if (getXmlValue(reply, xpath, onvif_data->dns_buf, 128) == 0) {}
+            }
+        }
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getDNS");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getDNS - No XML reply");
+    }
+    return result;
+}
+
+int setDNS(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    char fromDHCP_buf[128];
+    if (onvif_data->dhcp_enabled) {
+        strcpy(fromDHCP_buf, "true");
+    } else {
+        strcpy(fromDHCP_buf, "false");
+    }
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);        if (result < 0)
+            strcat(onvif_data->last_error, " getVideoEncoderConfiguration");
+
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setDNS = xmlNewTextChild(body, ns_tds, BAD_CAST "SetDNS", NULL);
+    if (!onvif_data->dhcp_enabled) {
+        xmlNodePtr dnsManual = xmlNewTextChild(setDNS, ns_tds, BAD_CAST "DNSManual", NULL);
+        xmlNewTextChild(dnsManual, ns_tt, BAD_CAST "Type", BAD_CAST "IPv4");
+        xmlNewTextChild(dnsManual, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->dns_buf);
+    } else {
+        xmlNewTextChild(setDNS, ns_tds, BAD_CAST "FromDHCP", BAD_CAST fromDHCP_buf);
+    }
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setDNS");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setDNS - No XML reply");
+    }
+    return result;
+}
+
+int getNTP(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetNTP", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+		xmlChar *xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:FromDHCP";
+		char ntp_buf[128];
+		getXmlValue(reply, xpath, ntp_buf, 128);
+		if (strcmp(ntp_buf,"true") == 0) {
+			onvif_data->ntp_dhcp = true;
+			xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:Type";
+			getXmlValue(reply, xpath, onvif_data->ntp_type, 128);
+			if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:IPv4Address";
+			else if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:IPv6Address";
+			else
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPFromDHCP//tt:DNSname";
+			getXmlValue(reply, xpath, onvif_data->ntp_addr, 128);
+		} else {
+			onvif_data->ntp_dhcp = false;
+			xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:Type";
+			getXmlValue(reply, xpath, onvif_data->ntp_type, 128);
+			if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:IPv4Address";
+			else if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:IPv6Address";
+			else
+				xpath = BAD_CAST "//s:Body//tds:GetNTPResponse//tt:NTPManual//tt:DNSname";
+			getXmlValue(reply, xpath, onvif_data->ntp_addr, 128);
+		}
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getNTP");
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getNTP - No XML reply");
+    }
+    return result;
+}
+
+int setNTP(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    char fromDHCP_buf[128];
+    if (onvif_data->ntp_dhcp) {
+        strcpy(fromDHCP_buf, "true");
+    } else {
+        strcpy(fromDHCP_buf, "false");
+    }
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setNTP = xmlNewTextChild(body, ns_tds, BAD_CAST "SetNTP", NULL);
+
+    xmlNewTextChild(setNTP, ns_tds, BAD_CAST "FromDHCP", BAD_CAST fromDHCP_buf);
+    if (!onvif_data->ntp_dhcp) {
+        xmlNodePtr ntpManual = xmlNewTextChild(setNTP, ns_tds, BAD_CAST "NTPManual", NULL);
+        xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "Type", BAD_CAST onvif_data->ntp_type);
+		if (strcmp(onvif_data->ntp_type,"IPv4") == 0)
+			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->ntp_addr);
+		else if (strcmp(onvif_data->ntp_type,"IPv6") == 0)
+			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "IPv6Address", BAD_CAST onvif_data->ntp_addr);
+		else
+			xmlNewTextChild(ntpManual, ns_tt, BAD_CAST "DNSName", BAD_CAST onvif_data->ntp_addr);
+    }
+
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setNTP");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setNTP - No XML reply");
+    }
+    return result;
+}
+
+int getHostname(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetHostname", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body//tds:GetHostnameResponse//tds:HostnameInformation//tt:FromDHCP";
+        xpath = BAD_CAST "//s:Body//tds:GetHostnameResponse//tds:HostnameInformation//tt:Name";
+        getXmlValue(reply, xpath, onvif_data->host_name, 128);
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getHostname");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getHostname - No XML reply");
+    }
+    return result;
+}
+
+int setHostname(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    if (onvif_data->host_name[0]) {
+        xmlNodePtr setHostname = xmlNewTextChild(body, ns_tds, BAD_CAST "SetHostname", NULL);
+        xmlNewTextChild(setHostname, ns_tds, BAD_CAST "Name", BAD_CAST onvif_data->host_name);
+        /* Do I also need to set FromDHCP to false ? */
+    } else {
+        xmlNodePtr setHostname = xmlNewTextChild(body, ns_tds, BAD_CAST "SetHostnameFromDHCP", NULL);
+        xmlNewTextChild(setHostname, ns_tds, BAD_CAST "FromDHCP", BAD_CAST "true");
+    }
+
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+		/* Should check for RebootNeeded=true from setHostnameFronDHCP */
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setHostname");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setHostname - No XML reply");
+    }
+    return result;
+}
+
+
+int getCapabilities(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr capabilities = xmlNewTextChild(body, ns_tds, BAD_CAST "GetCapabilities", NULL);
+    xmlNewTextChild(capabilities, ns_tds, BAD_CAST "Category", BAD_CAST "All");
+    char cmd[4096] = {0};
+
+
+    strcpy(onvif_data->device_service, onvif_data->xaddrs);
+    extractOnvifService(onvif_data->device_service, true);
+
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath;
+
+        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Events//tt:XAddr";
+        strcpy(onvif_data->event_service, "");
+        if (getXmlValue(reply, xpath, onvif_data->event_service, 128) == 0) {
+            extractOnvifService(onvif_data->event_service, true);
+        }
+
+        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Imaging//tt:XAddr";
+        strcpy(onvif_data->imaging_service, "");
+        if (getXmlValue(reply, xpath, onvif_data->imaging_service, 128) == 0)
+            extractOnvifService(onvif_data->imaging_service, true);
+
+        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:Media//tt:XAddr";
+        strcpy(onvif_data->media_service, "");
+        if (getXmlValue(reply, xpath, onvif_data->media_service, 128) == 0)
+            extractOnvifService(onvif_data->media_service, true);
+
+        xpath = BAD_CAST "//s:Body//tds:GetCapabilitiesResponse//tds:Capabilities//tt:PTZ//tt:XAddr";
+        strcpy(onvif_data->ptz_service, "");
+        if (getXmlValue(reply, xpath, onvif_data->ptz_service, 128) == 0)
+            extractOnvifService(onvif_data->ptz_service, true);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getCapabilities");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getCapabilities - No XML reply");
+    }
+    return result;
+}
+
+int getVideoEncoderConfigurationOptions(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getVideoEncoderConfigurationOptions = xmlNewTextChild(body, ns_trt, BAD_CAST "GetVideoEncoderConfigurationOptions", NULL);
+    if (onvif_data->videoEncoderConfigurationToken[0])
+        xmlNewTextChild(getVideoEncoderConfigurationOptions, ns_trt, BAD_CAST "ConfigurationToken", BAD_CAST onvif_data->videoEncoderConfigurationToken);
+    if (onvif_data->profileToken[0])
+        xmlNewTextChild(getVideoEncoderConfigurationOptions, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *width = NULL;
+        xmlChar *height = NULL;
+        xmlChar *xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:ResolutionsAvailable";
+        xmlNodeSetPtr nodeset;
+        xmlXPathObjectPtr xml_result = getNodeSet(reply, xpath);
+        int k = 0;
+        if (xml_result) {
+            nodeset = xml_result->nodesetval;
+            for (int i=0; i<nodeset->nodeNr; i++) {
+                xmlNodePtr cur = nodeset->nodeTab[i]->children;
+                while(cur != NULL) {
+                    if ((!xmlStrcmp(cur->name, (const xmlChar *) "Width"))) {
+                        width = xmlNodeListGetString(reply, cur->xmlChildrenNode, 1);
+                    }
+                    else if ((!xmlStrcmp(cur->name, (const xmlChar *) "Height"))) {
+                        height = xmlNodeListGetString(reply, cur->xmlChildrenNode, 1);
+                    }
+                    cur = cur->next;
+                }
+                char tmp[128] = {0};
+                if ((strlen((char *)width) + strlen((char *)height)) > 124) {
+                  fprintf(stderr, "xmlNodeListString return buffer overflow %zu\n", strlen((char *)width) + strlen((char *)height));
+                } else {
+                  sprintf(tmp, "%s x %s", width, height);
+                }
+
+                int size = 0;
+                bool found_size = false;
+                while (!found_size) {
+                    if (strlen(onvif_data->resolutions_buf[size]) == 0) {
+                        found_size = true;
+                    } else {
+                        size++;
+                        if (size > 15)
+                            found_size = true;
+                    }
+                }
+                bool duplicate = false;
+                for (int n=0; n<size; n++) {
+                    if (strcmp(onvif_data->resolutions_buf[n], tmp) == 0) {
+                        duplicate = true;
+                    }
+                }
+                if (!duplicate) {
+                    strcpy(onvif_data->resolutions_buf[size], tmp);
+                    k++;
+                }
+
+                if (width != NULL)
+                    xmlFree(width);
+                if (height != NULL)
+                    xmlFree(height);
+            }
+            xmlXPathFreeObject(xml_result);
+        }
+
+        char temp_buf[128];
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:GovLengthRange//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->gov_length_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:GovLengthRange//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->gov_length_max = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:FrameRateRange//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->frame_rate_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:H264//tt:FrameRateRange//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->frame_rate_max = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:Extension//tt:H264//tt:BitrateRange//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->bitrate_min = atoi(temp_buf);
+        else
+            onvif_data->bitrate_min = 128;
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationOptionsResponse//trt:Options//tt:Extension//tt:H264//tt:BitrateRange//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->bitrate_max = atoi(temp_buf);
+        else
+            onvif_data->bitrate_max = 16384;
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getVideoEncoderConfigurationOptions");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getVideoEncoderConfigurationOptions - No XML reply");
+    }
+    return result;
+}
+
+int getVideoEncoderConfiguration(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getVideoEncoderConfiguration = xmlNewTextChild(body, ns_trt, BAD_CAST "GetVideoEncoderConfiguration", NULL);
+    xmlNewTextChild(getVideoEncoderConfiguration, ns_trt, BAD_CAST "ConfigurationToken", BAD_CAST onvif_data->videoEncoderConfigurationToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath;
+        char temp_buf[128] = {0};
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Name";
+        getXmlValue(reply, xpath, onvif_data->video_encoder_name_buf, 128);
+
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:UseCount";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->use_count = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:GuaranteedFrameRate";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
+        if (strcmp(temp_buf, "true") == 0)
+            onvif_data->guaranteed_frame_rate = true;
+        else
+            onvif_data->guaranteed_frame_rate = false;
+        }
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Encoding";
+        getXmlValue(reply, xpath, onvif_data->encoding, 128);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Resolution//tt:Width";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->conf_width = atof(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Resolution//tt:Height";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->conf_height = atof(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Quality";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->quality = atof(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:FrameRateLimit";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->conf_frame_rate_limit = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:EncodingInterval";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->conf_encoding_interval = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:RateControl//tt:BitrateLimit";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->conf_bitrate_limit = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:H264//tt:H264Profile";
+        getXmlValue(reply, xpath, onvif_data->h264_profile_buf, 128);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:Type";
+        getXmlValue(reply, xpath, onvif_data->multicast_address_type_buf, 128);
+		if (strcmp(onvif_data->multicast_address_type_buf,"IPv6") == 0)
+            xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:IPv6Address";
+		else
+            xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Address//tt:IPv4Address";
+        getXmlValue(reply, xpath, onvif_data->multicast_address_buf, 128);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:Port";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->multicast_port = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:TTL";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->multicast_ttl = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:Multicast//tt:AutoStart";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
+        if (strcmp(temp_buf, "true") == 0)
+            onvif_data->autostart = true;
+        else
+            onvif_data->autostart = false;
+        }
+        xpath = BAD_CAST "//s:Body//trt:GetVideoEncoderConfigurationResponse//trt:Configuration//tt:SessionTimeout";
+        getXmlValue(reply, xpath, onvif_data->session_time_out_buf, 128);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getVideoEncoderConfiguration");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getVideoEncoderConfiguration - No XML reply");
+    }
+    return result;
+}
+
+int setVideoEncoderConfiguration(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    char frame_rate_buf[128] = {0};
+    char gov_length_buf[128] = {0};
+    char bitrate_buf[128] = {0};
+    char width_buf[128] = {0};
+    char height_buf[128] = {0};
+    char use_count_buf[128] = {0};
+    char quality_buf[128] = {0};
+    char multicast_port_buf[128] = {0};
+    char multicast_ttl_buf[128] = {0};
+    char autostart_buf[128] = {0};
+    char encoding_interval_buf[128] = {0};
+
+    sprintf(frame_rate_buf, "%d", onvif_data->frame_rate);
+    sprintf(gov_length_buf, "%d", onvif_data->gov_length);
+    sprintf(bitrate_buf, "%d", onvif_data->bitrate);
+    sprintf(use_count_buf, "%d", onvif_data->use_count);
+    sprintf(width_buf, "%d", onvif_data->width);
+    sprintf(height_buf, "%d", onvif_data->height);
+    sprintf(quality_buf, "%f", onvif_data->quality);
+    sprintf(multicast_port_buf, "%d", onvif_data->multicast_port);
+    sprintf(multicast_ttl_buf, "%d", onvif_data->multicast_ttl);
+    if (onvif_data->autostart)
+        strcpy(autostart_buf, "true");
+    else
+        strcpy(autostart_buf, "false");
+    sprintf(encoding_interval_buf, "%d", onvif_data->conf_encoding_interval);
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setVideoEncoderConfiguration = xmlNewTextChild(body, ns_trt, BAD_CAST "SetVideoEncoderConfiguration", NULL);
+    xmlNodePtr configuration = xmlNewTextChild(setVideoEncoderConfiguration, ns_trt, BAD_CAST "Configuration", NULL);
+    xmlNewProp(configuration, BAD_CAST "token", BAD_CAST onvif_data->videoEncoderConfigurationToken);
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Name", BAD_CAST onvif_data->video_encoder_name_buf);
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "UseCount", BAD_CAST use_count_buf);
+#ifdef ONVIF19060
+	/* Sad, but not supported until 19.06 release - crashes my older camera */
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "GuaranteedFrameRate", onvif_data->guaranteed_frame_rate?BAD_CAST "true":BAD_CAST "false");
+#endif
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Encoding", onvif_data->encoding[0]?BAD_CAST onvif_data->encoding:BAD_CAST "H264");
+    xmlNodePtr resolution = xmlNewTextChild(configuration, ns_tt, BAD_CAST "Resolution", NULL);
+    xmlNewTextChild(resolution, ns_tt, BAD_CAST "Width", BAD_CAST width_buf);
+    xmlNewTextChild(resolution, ns_tt, BAD_CAST "Height", BAD_CAST height_buf);
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "Quality", BAD_CAST quality_buf);
+    xmlNodePtr rateControl = xmlNewTextChild(configuration, ns_tt, BAD_CAST "RateControl", NULL);
+    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "FrameRateLimit", BAD_CAST frame_rate_buf);
+    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "EncodingInterval", BAD_CAST encoding_interval_buf);
+    xmlNewTextChild(rateControl, ns_tt, BAD_CAST "BitrateLimit", BAD_CAST bitrate_buf);
+    xmlNodePtr h264 = xmlNewTextChild(configuration, ns_tt, BAD_CAST "H264", NULL);
+    xmlNewTextChild(h264, ns_tt, BAD_CAST "GovLength", BAD_CAST gov_length_buf);
+    xmlNewTextChild(h264, ns_tt, BAD_CAST "H264Profile", BAD_CAST onvif_data->h264_profile_buf);
+    xmlNodePtr multicast = xmlNewTextChild(configuration, ns_tt, BAD_CAST "Multicast", NULL);
+    xmlNodePtr address = xmlNewTextChild(multicast, ns_tt, BAD_CAST "Address", NULL);
+    xmlNewTextChild(address, ns_tt, BAD_CAST "Type", BAD_CAST onvif_data->multicast_address_type_buf);
+    xmlNewTextChild(address, ns_tt, BAD_CAST "IPv4Address", BAD_CAST onvif_data->multicast_address_buf);
+    xmlNewTextChild(multicast, ns_tt, BAD_CAST "Port", BAD_CAST multicast_port_buf);
+    xmlNewTextChild(multicast, ns_tt, BAD_CAST "TTL", BAD_CAST multicast_ttl_buf);
+    xmlNewTextChild(multicast, ns_tt, BAD_CAST "AutoStart", BAD_CAST autostart_buf);
+    xmlNewTextChild(configuration, ns_tt, BAD_CAST "SessionTimeout", BAD_CAST onvif_data->session_time_out_buf);
+    xmlNewTextChild(setVideoEncoderConfiguration, ns_trt, BAD_CAST "ForcePersistence", BAD_CAST "true");
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setVideoEncoderConfiguration");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setVideoEncoderConfiguration - No XML reply");
+    }
+    return result;
+}
+
+int getProfile(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getProfile = xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfile", NULL);
+    xmlNewTextChild(getProfile, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        char temp_buf[128];
+
+        xmlChar *xpath;
+
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:Resolution//tt:Width";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->width = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:Resolution//tt:Height";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->height = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:RateControl//tt:FrameRateLimit";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
+            onvif_data->frame_rate = atoi(temp_buf);
+        }
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:RateControl//tt:BitrateLimit";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
+            onvif_data->bitrate = atoi(temp_buf);
+        } else {
+            onvif_data->bitrate = 0;
+        }
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration//tt:H264//tt:GovLength";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0) {
+            onvif_data->gov_length = atoi(temp_buf);
+        }
+
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoEncoderConfiguration";
+        getNodeAttribute(reply, xpath, BAD_CAST "token", onvif_data->videoEncoderConfigurationToken, 128);
+        xpath = BAD_CAST "//s:Body//trt:GetProfileResponse//trt:Profile//tt:VideoSourceConfiguration//tt:SourceToken";
+        getXmlValue(reply, xpath, onvif_data->videoSourceConfigurationToken, 128);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getProfile");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getProfile - No XML reply");
+    }
+    return result;
+}
+
+int getOptions(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getOptions = xmlNewTextChild(body, ns_timg, BAD_CAST "GetOptions", NULL);
+    xmlNewTextChild(getOptions, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath;
+        char temp_buf[128];
+
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Brightness//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->brightness_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Brightness//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->brightness_max = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:ColorSaturation//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->saturation_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:ColorSaturation//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->saturation_max = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Contrast//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->contrast_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Contrast//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->contrast_max = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Sharpness//tt:Min";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->sharpness_min = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetOptionsResponse//timg:ImagingOptions//tt:Sharpness//tt:Max";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->sharpness_max = atoi(temp_buf);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getOptions");
+        xmlFreeDoc(reply);
+     } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getOptions - No XML reply");
+    }
+    return result;
+}
+
+int getImagingSettings(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getImagingSettings = xmlNewTextChild(body, ns_timg, BAD_CAST "GetImagingSettings", NULL);
+    xmlNewTextChild(getImagingSettings, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlChar *xpath;
+        char temp_buf[128];
+
+        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Brightness";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->brightness = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:ColorSaturation";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->saturation = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Contrast";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->contrast = atoi(temp_buf);
+        xpath = BAD_CAST "//s:Body//timg:GetImagingSettingsResponse//timg:ImagingSettings//tt:Sharpness";
+        if (getXmlValue(reply, xpath, temp_buf, 128) == 0)
+            onvif_data->sharpness = atoi(temp_buf);
+
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getImagingSettings");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getImagingSettings - No XML reply");
+    }
+    return result;
+}
+
+int setImagingSettings(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    char brightness_buf[128] = {0};
+    char saturation_buf[128] = {0};
+    char contrast_buf[128] = {0};
+    char sharpness_buf[128] = {0};
+    sprintf(brightness_buf, "%d", onvif_data->brightness);
+    sprintf(saturation_buf, "%d", onvif_data->saturation);
+    sprintf(contrast_buf, "%d", onvif_data->contrast);
+    sprintf(sharpness_buf, "%d", onvif_data->sharpness);
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_timg = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl", BAD_CAST "timg");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setImagingSettings = xmlNewTextChild(body, ns_timg, BAD_CAST "SetImagingSettings", NULL);
+    xmlNewTextChild(setImagingSettings, ns_timg, BAD_CAST "VideoSourceToken", BAD_CAST onvif_data->videoSourceConfigurationToken);
+    xmlNodePtr imagingSettings = xmlNewTextChild(setImagingSettings, ns_timg, BAD_CAST "ImagingSettings", NULL);
+    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Brightness", BAD_CAST brightness_buf);
+    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "ColorSaturation", BAD_CAST saturation_buf);
+    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Contrast", BAD_CAST contrast_buf);
+    xmlNewTextChild(imagingSettings, ns_tt, BAD_CAST "Sharpness", BAD_CAST sharpness_buf);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->imaging_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setImagingSettings");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setImagingSettings - No XML reply");
+    }
+    return result;
+}
+
+int continuousMove(float x, float y, float z, struct OnvifData *onvif_data) {
+    int result = 0;
+    char pan_tilt_string[128] = {0};
+    char zoom_string[128] = {0};
+    sprintf(pan_tilt_string, "PanTilt x=\"%.*f\" y=\"%.*f\"", 2, x, 2, y);
+    sprintf(zoom_string, "Zoom x=\"%.*f\"", 2, z);
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr continuousMove = xmlNewTextChild(body, ns_ptz, BAD_CAST "ContinuousMove", NULL);
+    xmlNewTextChild(continuousMove, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    xmlNodePtr velocity = xmlNewTextChild(continuousMove, ns_ptz, BAD_CAST "Velocity", BAD_CAST NULL);
+    xmlNewTextChild(velocity, ns_tt, BAD_CAST pan_tilt_string, NULL);
+    xmlNewTextChild(velocity, ns_tt, BAD_CAST zoom_string, NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " continuousMove");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "continuousMove - No XML reply");
+    }
+    return result;
+}
+
+int moveStop(int type, struct OnvifData *onvif_data) {
+    int result = 0;
+    char pan_tilt_flag[128] = {0};
+    char zoom_flag[128] = {0};
+
+    if (type == PAN_TILT_STOP) {
+        strcpy(pan_tilt_flag, "true");
+        strcpy(zoom_flag, "false");
+    }
+    else if (type == ZOOM_STOP) {
+        strcpy(pan_tilt_flag, "false");
+        strcpy(zoom_flag, "true");
+    }
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr stop = xmlNewTextChild(body, ns_ptz, BAD_CAST "Stop", NULL);
+    xmlNewTextChild(stop, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    xmlNewTextChild(stop, ns_ptz, BAD_CAST "PanTilt", BAD_CAST pan_tilt_flag);
+    xmlNewTextChild(stop, ns_ptz, BAD_CAST "Zoom", BAD_CAST zoom_flag);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " moveStop");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "moveStop - No XML reply");
+    }
+    return result;
+}
+
+int setPreset(char *arg, struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setPreset = xmlNewTextChild(body, ns_ptz, BAD_CAST "SetPreset", NULL);
+    xmlNewTextChild(setPreset, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    xmlNewTextChild(setPreset, ns_ptz, BAD_CAST "PresetToken", BAD_CAST arg);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setPreset");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setPreset - No XML reply");
+    }
+    return result;
+}
+
+int gotoPreset(char *arg, struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_ptz = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver20/ptz/wsdl", BAD_CAST "ptz");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr gotoPreset = xmlNewTextChild(body, ns_ptz, BAD_CAST "GotoPreset", NULL);
+    xmlNewTextChild(gotoPreset, ns_ptz, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    xmlNewTextChild(gotoPreset, ns_ptz, BAD_CAST "PresetToken", BAD_CAST arg);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->ptz_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " gotoPreset");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "gotoPreset - No XML reply");
+    }
+    return result;
+}
+
+int setUser(char *new_password, struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setUser = xmlNewTextChild(body, ns_tds, BAD_CAST "SetUser", NULL);
+    xmlNodePtr user = xmlNewTextChild(setUser, ns_tds, BAD_CAST "User", NULL);
+    xmlNewTextChild(user, ns_tt, BAD_CAST "Username", BAD_CAST "admin");
+    xmlNewTextChild(user, ns_tt, BAD_CAST "Password", BAD_CAST new_password);
+    xmlNewTextChild(user, ns_tt, BAD_CAST "UserLevel", BAD_CAST "Administrator");
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setUser");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setUser - No XML reply");
+    }
+    return result;
+}
+
+int setSystemDateAndTime(struct OnvifData *onvif_data) {
+    int result = 0;
+    time_t rawtime;
+    time(&rawtime);
+    struct tm *UTCTime = localtime(&rawtime);
+    char dst_flag_buf[128];
+    if (UTCTime->tm_isdst == 1)
+        strcpy(dst_flag_buf, "true");
+    else
+        strcpy(dst_flag_buf, "false");
+    char hour_buf[128];
+    char minute_buf[128];
+    char second_buf[128];
+    char year_buf[128];
+    char month_buf[128];
+    char day_buf[128];
+    sprintf(hour_buf, "%d", UTCTime->tm_hour);
+    sprintf(minute_buf, "%d", UTCTime->tm_min);
+    sprintf(second_buf, "%d", UTCTime->tm_sec);
+    sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
+    sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
+    sprintf(day_buf, "%d", UTCTime->tm_mday);
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
+    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "Manual");
+    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
+    xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
+    xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST "UTC0");
+    xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
+    xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
+    xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " setSystemDatAndTime");
+        xmlFreeDoc(reply);
+    }
+    else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setSystemDateAndTime - No XML reply");
+    }
+    return result;
+}
+
+int setSystemDateAndTimeUsingTimezone(struct OnvifData *onvif_data) {
+    int result = 0;
+    time_t rawtime;
+    time(&rawtime);
+	bool special = false;
+    struct tm *UTCTime = localtime(&rawtime);
+    char dst_flag_buf[128];
+    if (UTCTime->tm_isdst == 1)
+        strcpy(dst_flag_buf, "true");
+    else
+        strcpy(dst_flag_buf, "false");
+    if (strcmp(onvif_data->timezone,"UTC0") == 0) {
+        special = true;
+    } else {
+        if (!onvif_data->timezone[0]) {
+#ifndef _WIN32
+            // work out a timezone to use on the camera 
+            int h = -(UTCTime->tm_gmtoff/3600);
+            int m = (UTCTime->tm_gmtoff + 3600 * h)/60;
+            if (m)
+                sprintf(onvif_data->timezone,"%s%d:%02d:00%s",tzname[0],h,m,tzname[1]);
+            else
+                sprintf(onvif_data->timezone,"%s%d%s",tzname[0],h,tzname[1]);
+#else
+            int h = _timezone/3600;
+            int m = (_timezone - 3600 * h)/60;
+            if (m)
+                sprintf(onvif_data->timezone,"%s%d:%02d:00%s",_tzname[0],h,m,_tzname[1]);
+            else
+                sprintf(onvif_data->timezone,"%s%d%s",_tzname[0],h,_tzname[1]);
+#endif
+        }
+        UTCTime = gmtime(&rawtime);
+    }
+    if (!onvif_data->datetimetype)
+        onvif_data->datetimetype = 'M'; // manual 
+    char hour_buf[128];
+    char minute_buf[128];
+    char second_buf[128];
+    char year_buf[128];
+    char month_buf[128];
+    char day_buf[128];
+    sprintf(hour_buf, "%d", UTCTime->tm_hour);
+    sprintf(minute_buf, "%d", UTCTime->tm_min);
+    sprintf(second_buf, "%d", UTCTime->tm_sec);
+    sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
+    sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
+    sprintf(day_buf, "%d", UTCTime->tm_mday);
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
+    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "Manual");
+    xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
+    xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
+    xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST onvif_data->timezone);
+    xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
+    xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
+    xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
+    xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
+    xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        xmlFreeDoc(reply);
+        if (result == 0 && onvif_data->datetimetype == 'N') {
+            // switch back to NTP after we have nudged it to correct 
+            time_t newtime;
+            time(&newtime);
+            if (newtime != rawtime) {
+                // save a little effort if we are within a second of the previous check 
+                if (special)
+                    UTCTime = localtime(&newtime);
+                else
+                    UTCTime = gmtime(&newtime);
+                sprintf(hour_buf, "%d", UTCTime->tm_hour);
+                sprintf(minute_buf, "%d", UTCTime->tm_min);
+                sprintf(second_buf, "%d", UTCTime->tm_sec);
+                sprintf(year_buf, "%d", UTCTime->tm_year + 1900);
+                sprintf(month_buf, "%d", UTCTime->tm_mon + 1);
+                sprintf(day_buf, "%d", UTCTime->tm_mday);
+            }
+            doc = xmlNewDoc(BAD_CAST "1.0");
+            xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+            xmlDocSetRootElement(doc, root);
+            xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+            xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+            xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+            xmlSetNs(root, ns_env);
+            addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+            xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+            xmlNodePtr setSystemDateAndTime = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemDateAndTime", NULL);
+            xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DateTimeType", BAD_CAST "NTP");
+            xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "DaylightSavings", BAD_CAST dst_flag_buf);
+            xmlNodePtr timeZone = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "TimeZone", NULL);
+            xmlNewTextChild(timeZone, ns_tt, BAD_CAST "TZ", BAD_CAST onvif_data->timezone);
+            // Need to include date/time even though the specs say it should be ignored 
+            xmlNodePtr utcDateTime = xmlNewTextChild(setSystemDateAndTime, ns_tds, BAD_CAST "UTCDateTime", NULL);
+            xmlNodePtr cameraTime = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Time", NULL);
+            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Hour", BAD_CAST hour_buf);
+            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Minute", BAD_CAST minute_buf);
+            xmlNewTextChild(cameraTime, ns_tt, BAD_CAST "Second", BAD_CAST second_buf);
+            xmlNodePtr cameraDate = xmlNewTextChild(utcDateTime, ns_tt, BAD_CAST "Date", NULL);
+            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Year", BAD_CAST year_buf);
+            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Month", BAD_CAST month_buf);
+            xmlNewTextChild(cameraDate, ns_tt, BAD_CAST "Day", BAD_CAST day_buf);
+            char cmd[4096] = {0};
+            addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+            xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+            if (reply != NULL) {
+                result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+		xmlFreeDoc(reply);
+            } else {
+                result = -1;
+		strcpy(onvif_data->last_error, "setSystemDateAndTimeUsingTimezone - No XML reply");
+            }
+        }
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "setSystemDateAndTimeUsingTimezone 2 - No XML reply");
+    }
+    return result;
+}
+
+int getProfileToken(struct OnvifData *onvif_data, int profileIndex) {
+    int result;
+    onvif_data->profileToken[0] = 0;
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfiles", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        getNodeAttributen(reply, BAD_CAST "//s:Body//trt:GetProfilesResponse//trt:Profiles", BAD_CAST "token", onvif_data->profileToken, 128, profileIndex);
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getProfileToken");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getProfileToken - No XML reply");
+    }
+    return result;
+}
+
+int getTimeOffset(struct OnvifData *onvif_data) {
+    int result = 0;
+
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetSystemDateAndTime", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+
+    if (reply != NULL) {
+        char hour_buf[16];
+        char min_buf[16];
+        char sec_buf[16];
+        char year_buf[16];
+        char month_buf[16];
+        char day_buf[16];
+        char dst_buf[16];
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Hour", hour_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Minute", min_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Time//tt:Second", sec_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Year", year_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Month", month_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:UTCDateTime//tt:Date//tt:Day", day_buf, 16);
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:DaylightSavings", dst_buf, 16);
+
+    	onvif_data->dst = false;
+        int is_dst = 0;
+        if (strcmp(dst_buf, "true") == 0) {
+            is_dst = 1;
+	        onvif_data->dst = true;
+	    }
+
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:TimeZone//tt:TZ", onvif_data->timezone, 128);
+	    char dttype[16];
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetSystemDateAndTimeResponse//tds:SystemDateAndTime//tt:DateTimeType", dttype, 16);
+	    onvif_data->datetimetype = dttype[0]; /* M == Manual, N == NTP */
+
+        time_t now = time(NULL);
+        time_t utc_time_here = now;
+	    bool special = false;
+	    if (strcmp(onvif_data->timezone,"UTC0") == 0) {
+	        /* special case - camera is running on local time believing it is UTC */
+	        special = true;
+            struct tm *utc_here = gmtime(&now);
+            utc_here->tm_isdst = -1;
+            utc_time_here = mktime(utc_here);
+	    }
+
+        struct tm *utc_there = localtime(&now);
+        utc_there->tm_year = atoi(year_buf) - 1900;
+        utc_there->tm_mon = atoi(month_buf) - 1;
+        utc_there->tm_mday = atoi(day_buf);
+        utc_there->tm_hour = atoi(hour_buf);
+        utc_there->tm_min = atoi(min_buf);
+        utc_there->tm_sec = atoi(sec_buf);
+        utc_there->tm_isdst = is_dst;
+	    time_t utc_time_there;
+	    if (special)
+	        utc_time_there = mktime(utc_there);
+	    else
+#ifndef _WIN32
+	        utc_time_there = timegm(utc_there);
+#else
+	        utc_time_there = _mkgmtime(utc_there);
+#endif
+	    onvif_data->time_offset = utc_time_there - utc_time_here;
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getTimeOfset");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getTimeOffset - No XML reply");
+    }
+
+    return result;
+}
+
+int getStreamUri(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlNsPtr ns_tt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/schema", BAD_CAST "tt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr getStreamUri = xmlNewTextChild(body, ns_trt, BAD_CAST "GetStreamUri", NULL);
+    xmlNodePtr streamSetup = xmlNewTextChild(getStreamUri, ns_trt, BAD_CAST "StreamSetup", NULL);
+    xmlNewTextChild(streamSetup, ns_tt, BAD_CAST "Stream", BAD_CAST "RTP-Unicast");
+    xmlNodePtr transport = xmlNewTextChild(streamSetup, ns_tt, BAD_CAST "Transport", NULL);
+    xmlNewTextChild(transport, ns_tt, BAD_CAST "Protocol", BAD_CAST "RTSP");
+    xmlNewTextChild(getStreamUri, ns_trt, BAD_CAST "ProfileToken", BAD_CAST onvif_data->profileToken);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        getXmlValue(reply, BAD_CAST "//s:Body//trt:GetStreamUriResponse//trt:MediaUri//tt:Uri", onvif_data->stream_uri, 1024);
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getStreamUri");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getStreamUri - No XML reply");
+    }
+    return result;
+}
+
+int getDeviceInformation(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDeviceInformation", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        getXmlValue(reply, BAD_CAST "//s:Body//tds:GetDeviceInformationResponse//tds:SerialNumber", onvif_data->serial_number, 128);
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " getdeviceImformation");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "getDeviceInformation - No XML reply");
+    }
+    return result;
+}
+
+void getDiscoveryXml2(char buffer[], int buf_size) {
+    char *xml_string = "<s:Envelope xmlns:s=\"http://www.w3.org/2003/05/soap-envelope\" xmlns:a=\"http://schemas.xmlsoap.org/ws/2004/08/addressing\"><s:Header><a:Action s:mustUnderstand=\"1\">http://schemas.xmlsoap.org/ws/2005/04/discovery/Probe</a:Action><a:MessageID>uuid:6bbdae2d-f229-42c8-a27b-93880fb80826</a:MessageID><a:ReplyTo><a:Address>http://schemas.xmlsoap.org/ws/2004/08/addressing/role/anonymous</a:Address></a:ReplyTo><a:To s:mustUnderstand=\"1\">urn:schemas-xmlsoap-org:ws:2005:04:discovery</a:To></s:Header><s:Body><Probe xmlns=\"http://schemas.xmlsoap.org/ws/2005/04/discovery\"><d:Types xmlns:d=\"http://schemas.xmlsoap.org/ws/2005/04/discovery\" xmlns:dp0=\"http://www.onvif.org/ver10/device/wsdl\">dp0:Device</d:Types></Probe></s:Body></s:Envelope>";
+    strcpy(buffer, xml_string);
+}
+
+void getDiscoveryXml(char buffer[], int buf_size, char uuid[47]) {
+    for (int i=0; i<buf_size; i++)
+        buffer[i] = '\0';
+    getUUID(uuid);
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNewProp(root, BAD_CAST "xmlns:SOAP-ENV", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
+    xmlNewProp(root, BAD_CAST "xmlns:a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
+    xmlNsPtr ns_env = xmlNewNs(root, NULL, BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_a = xmlNewNs(root, NULL, BAD_CAST "a");
+    xmlSetNs(root, ns_env);
+    xmlNodePtr header = xmlNewTextChild(root, ns_env, BAD_CAST "Header", NULL);
+    xmlNodePtr action = xmlNewTextChild(header, ns_a, BAD_CAST "Action", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery/Probe");
+    xmlNewProp(action, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
+    xmlNodePtr messageid = xmlNewTextChild(header, ns_a, BAD_CAST "MessageID", BAD_CAST uuid);
+    xmlNodePtr replyto = xmlNewTextChild(header, ns_a, BAD_CAST "ReplyTo", NULL);
+    xmlNodePtr address = xmlNewTextChild(replyto, ns_a, BAD_CAST "Address", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing/role/anonymous");
+    xmlNodePtr to = xmlNewTextChild(header, ns_a, BAD_CAST "To", BAD_CAST "urn:schemas-xmlsoap-org:ws:2005:04:discovery");
+    xmlNewProp(to, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr probe = xmlNewTextChild(body, NULL, BAD_CAST "Probe", NULL);
+    xmlNewProp(probe, BAD_CAST "xmlns:p", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
+    xmlNsPtr ns_p = xmlNewNs(probe, NULL, BAD_CAST "p");
+    xmlSetNs(probe, ns_p);
+    xmlNodePtr types = xmlNewTextChild(probe, NULL, BAD_CAST "Types", BAD_CAST "dp0:NetworkVideoTransmitter");
+    xmlNewProp(types, BAD_CAST "xmlns:d", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
+    xmlNewProp(types, BAD_CAST "xmlns:dp0", BAD_CAST "http://www.onvif.org/ver10/network/wsdl");
+    xmlNsPtr ns_d = xmlNewNs(types, NULL, BAD_CAST "d");
+    xmlSetNs(types, ns_d);
+    xmlOutputBufferPtr outputbuffer = xmlAllocOutputBuffer(NULL);
+    xmlNodeDumpOutput(outputbuffer, doc, root, 0, 0, NULL);
+    int size = xmlOutputBufferGetSize(outputbuffer);
+    strcpy(buffer, (char*)xmlOutputBufferGetContent(outputbuffer));
+    xmlOutputBufferFlush(outputbuffer);
+    xmlOutputBufferClose(outputbuffer);
+    xmlFreeDoc(doc);
+}
+
+int rebootCamera(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "SystemReboot", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " rebootCamera");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "rebootCamera - No XML reply");
+    }
+  return result;
+}
+
+int hardReset(struct OnvifData *onvif_data) {
+    int result = 0;
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNodePtr setSystemFactoryDefault = xmlNewTextChild(body, ns_tds, BAD_CAST "SetSystemFactoryDefault", NULL);
+    xmlNewTextChild(setSystemFactoryDefault, ns_tds, BAD_CAST "FactoryDefault", BAD_CAST "Hard");
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        result = checkForXmlErrorMsg(reply, onvif_data->last_error);
+        if (result < 0)
+            strcat(onvif_data->last_error, " hardReset");
+        xmlFreeDoc(reply);
+    } else {
+        result = -1;
+        strcpy(onvif_data->last_error, "hardReset - No XML reply");
+    }
+    return result;
+}
+
+void saveSystemDateAndTime(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetSystemDateAndTime", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+void saveScopes(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetScopes", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+void saveDeviceInformation(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetDeviceInformation", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+void saveCapabilities(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_tds = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/device/wsdl", BAD_CAST "tds");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_tds, BAD_CAST "GetCapabilities", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->device_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+void saveProfiles(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_trt, BAD_CAST "GetProfiles", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+void saveServiceCapabilities(char *filename, struct OnvifData *onvif_data) {
+    xmlDocPtr doc = xmlNewDoc(BAD_CAST "1.0");
+    xmlNodePtr root = xmlNewDocNode(doc, NULL, BAD_CAST "Envelope", NULL);
+    xmlDocSetRootElement(doc, root);
+    xmlNsPtr ns_env = xmlNewNs(root, BAD_CAST "http://www.w3.org/2003/05/soap-envelope", BAD_CAST "SOAP-ENV");
+    xmlNsPtr ns_trt = xmlNewNs(root, BAD_CAST "http://www.onvif.org/ver10/media/wsdl", BAD_CAST "trt");
+    xmlSetNs(root, ns_env);
+    addUsernameDigestHeader(root, ns_env, onvif_data->username, onvif_data->password, onvif_data->time_offset);
+    xmlNodePtr body = xmlNewTextChild(root, ns_env, BAD_CAST "Body", NULL);
+    xmlNewTextChild(body, ns_trt, BAD_CAST "GetServiceCapabilities", NULL);
+    char cmd[4096] = {0};
+    addHttpHeader(doc, root, onvif_data->xaddrs, onvif_data->media_service, cmd, 4096);
+    xmlDocPtr reply = sendCommandToCamera(cmd, onvif_data->xaddrs);
+    if (reply != NULL) {
+        xmlSaveFormatFile(filename, reply, 1);
+        xmlFreeDoc(reply);
+    }
+}
+
+int getXmlValue(xmlDocPtr doc, xmlChar *xpath, char buf[], int buf_length) {
+    xmlChar *keyword = NULL;
+    xmlXPathContextPtr context = xmlXPathNewContext(doc);
+    if (context == NULL) {
+        return -1;
+    }
+    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
+    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
+    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
+    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
+    xmlXPathRegisterNs(context, BAD_CAST "d", BAD_CAST "http://schemas.xmlsoap.org/ws/2005/04/discovery");
+    xmlXPathRegisterNs(context, BAD_CAST "ter", BAD_CAST "http://www.onvif.org/ver10/error");
+    xmlXPathRegisterNs(context, BAD_CAST "a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
+
+
+    xmlXPathObjectPtr result = xmlXPathEvalExpression(xpath, context);
+    xmlXPathFreeContext(context);
+    if (result == NULL) {
+        return -2;
+    }
+
+    if (xmlXPathNodeSetIsEmpty(result->nodesetval)) {
+        if ((strcmp((char*) xpath, "//s:Body//s:Fault//s:Code//s:Subcode//s:Value") != 0) && (strcmp((char*) xpath, "//s:Body//s:Fault//s:Reason//s:Text") != 0)) {
+        }
+    return -3;
+    }
+
+    if (result) {
+        keyword = xmlNodeListGetString(doc, result->nodesetval->nodeTab[0]->xmlChildrenNode, 1);
+        if (keyword != NULL) {
+            if (strlen((char*) keyword) > buf_length-1) {
+                xmlXPathFreeObject(result);
+                xmlFree(keyword);
+                return -4;
+            } else {
+                for (int i=0; i<buf_length; i++)
+                    buf[i] = '\0';
+                strcpy(buf, (char*) keyword);
+            }
+        }
+    }
+
+    xmlXPathFreeObject(result);
+    if (keyword != NULL)
+        xmlFree(keyword);
+    return 0;
+}
+
+int getNodeAttributen (xmlDocPtr doc, xmlChar *xpath, xmlChar *attribute, char buf[], int buf_length, int profileIndex) {
+    xmlChar *keyword = NULL;
+    xmlXPathContextPtr context = xmlXPathNewContext(doc);
+    if (context == NULL) {
+        return -1;
+    }
+    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
+    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
+    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
+    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
+    xmlXPathRegisterNs(context, BAD_CAST "ter", BAD_CAST "http://www.onvif.org/ver10/error");
+    xmlXPathRegisterNs(context, BAD_CAST "a", BAD_CAST "http://schemas.xmlsoap.org/ws/2004/08/addressing");
+
+    xmlXPathObjectPtr result = xmlXPathEvalExpression(xpath, context);
+    xmlXPathFreeContext(context);
+    if (result == NULL) {
+        return -2;
+    }
+
+    if (xmlXPathNodeSetIsEmpty(result->nodesetval)) {
+        return -3;
+    }
+
+    if (result) {
+        if( profileIndex >= result->nodesetval->nodeNr )
+            return -5;
+
+        keyword = xmlGetProp(result->nodesetval->nodeTab[profileIndex], attribute);
+        if (keyword != NULL) {
+            if (strlen((char*) keyword) > buf_length-1) {
+                xmlXPathFreeObject(result);
+                xmlFree(keyword);
+                return -4;
+            } else {
+                for (int i=0; i<buf_length; i++)
+                    buf[i] = '\0';
+                strcpy(buf, (char*) keyword);
+            }
+        }
+    }
+
+    xmlXPathFreeObject(result);
+    if (keyword != NULL)
+        xmlFree(keyword);
+    return 0;
+}
+
+xmlXPathObjectPtr getNodeSet (xmlDocPtr doc, xmlChar *xpath) {
+    xmlXPathContextPtr context;
+    xmlXPathObjectPtr result;
+
+    context = xmlXPathNewContext(doc);
+    if (context == NULL) {
+        return NULL;
+    }
+    xmlXPathRegisterNs(context, BAD_CAST "s", BAD_CAST "http://www.w3.org/2003/05/soap-envelope");
+    xmlXPathRegisterNs(context, BAD_CAST "trt", BAD_CAST "http://www.onvif.org/ver10/media/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "tt", BAD_CAST "http://www.onvif.org/ver10/schema");
+    xmlXPathRegisterNs(context, BAD_CAST "tds", BAD_CAST "http://www.onvif.org/ver10/device/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "timg", BAD_CAST "http://www.onvif.org/ver20/imaging/wsdl");
+    xmlXPathRegisterNs(context, BAD_CAST "wsa5", BAD_CAST "http://www.w3.org/2005/08/addressing");
+    xmlXPathRegisterNs(context, BAD_CAST "wsnt", BAD_CAST "http://docs.oasis-open.org/wsn/b-2");
+
+    result = xmlXPathEvalExpression(xpath, context);
+    xmlXPathFreeContext(context);
+    if (result == NULL) {
+        return NULL;
+    }
+    if(xmlXPathNodeSetIsEmpty(result->nodesetval)){
+        xmlXPathFreeObject(result);
+        return NULL;
+    }
+    return result;
+}
+
+xmlDocPtr sendCommandToCamera(char *cmd, char *xaddrs) {
+    int sock = 0, valread, flags;
+    const int buffer_size = 4096;
+    struct sockaddr_in serv_addr;
+    char buffer[4096] = {0};
+
+    char tmp[128] = {0};
+    char *mark = strstr(xaddrs, "//");
+    int start = mark-xaddrs+2;
+    int tmp_len = strlen(xaddrs);
+    int j;
+    for (j=0; j<tmp_len-start; j++) {
+        tmp[j] = xaddrs[j+start];
+    }
+    tmp[j] = '\0';
+
+    mark = strstr(tmp, "/");
+    int end = mark-tmp;
+    char tmp2[128] = {0};
+    for (j=0; j<end; j++) {
+        tmp2[j] = tmp[j];
+    }
+    tmp2[j] = '\0';
+
+    char host[128] = {0};
+    char port_buf[128] = {0};
+    mark = strstr(tmp2, ":");
+    if (mark == NULL) {
+        strcpy(host, tmp2);
+        strcpy(port_buf, "80");
+    } else {
+        start = mark-tmp2;
+        for (j=0; j<start; j++) {
+            host[j] = tmp2[j];
+        }
+        host[j] = '\0';
+        tmp_len = strlen(tmp2);
+        for (j=start+1; j<tmp_len; j++) {
+            port_buf[j-(start+1)] = tmp2[j];
+        }
+        port_buf[j-(start+1)] = '\0';
+    }
+
+    int port = atoi(port_buf);
+
+#ifdef _WIN32
+    WSADATA wsaData;
+    WSAStartup(MAKEWORD(2,2), &wsaData);
+#endif
+
+    if ((sock = socket(AF_INET, SOCK_STREAM, 0)) < 0) {
+        return NULL;
+    }
+
+    memset(&serv_addr, '0', sizeof(serv_addr));
+    serv_addr.sin_family = AF_INET;
+    serv_addr.sin_port = htons(port);
+    serv_addr.sin_addr.s_addr = inet_addr(host);
+
+    if (connect(sock, (struct sockaddr *)&serv_addr, sizeof(serv_addr)) < 0) {
+        return NULL;
+    }
+
+    if (send(sock , cmd , strlen(cmd) , 0 ) < 0) {
+        return NULL;
+    }
+    valread = recv( sock , buffer, 4096, 0);
+
+    char http_terminate[5];
+    http_terminate[0] = '\r';
+    http_terminate[1] = '\n';
+    http_terminate[2] = '\r';
+    http_terminate[3] = '\n';
+    http_terminate[4] = '\0';
+
+    char * substr = strstr(buffer, http_terminate);
+    if (substr == NULL)
+        return NULL;
+
+    int i;
+    int xml_start = substr - buffer + 4;
+    if (xml_start > 1024)
+        return NULL;
+    char http_header[1024];
+    for (i=0; i<xml_start; i++) {
+        http_header[i] = buffer[i];
+    }
+    http_header[xml_start] = '\0';
+
+    substr = strstr(http_header, "Content-Length: ");
+    if (substr == NULL)
+        return NULL;
+
+    int length_start = substr - http_header + 16;
+    if ((xml_start - length_start) > 1024)
+        return NULL;
+    char str_xml_length[1024];
+    for (i=length_start; i<xml_start; i++) {
+        if (http_header[i] == '\r' && http_header[i+1] == '\n') {
+            str_xml_length[i - length_start] = '\0';
+            break;
+        } else {
+            str_xml_length[i - length_start] = http_header[i];
+        }
+    }
+    int xml_length = (int) strtol(str_xml_length, (char **)NULL, 10);
+    if (xml_length > 65536)
+        return NULL;
+    char xml_reply[65536];
+
+    for (i=0; i<valread-xml_start; i++) {
+        xml_reply[i] = buffer[i+xml_start];
+    }
+
+    int cumulative_read = valread - xml_start;
+    while (cumulative_read < xml_length) {
+        valread = recv(sock, buffer, buffer_size, 0);
+        for (i=0; i<valread; i++) {
+            xml_reply[i+cumulative_read] = buffer[i];
+        }
+        cumulative_read = cumulative_read + valread;
+    }
+    xml_reply[xml_length] = '\0';
+
+#ifdef _WIN32
+    closesocket(sock);
+    WSACleanup();
+#else
+    close(sock);
+#endif
+
+    xmlDocPtr reply = xmlParseMemory(xml_reply, xml_length);
+    char error_msg[1024] = {0};
+
+    /* Dump reply if requested */
+    if (dump_reply) {
+        dumpReply(reply);
+    }
+
+    return reply;
+}
+
+int checkForXmlErrorMsg(xmlDocPtr doc, char error_msg[1024]) {
+    if (getXmlValue(doc, BAD_CAST "//s:Body//s:Fault//s:Code//s:Subcode//s:Value", error_msg, 1024) == 0) {
+        return -1;
+    }
+    else if (getXmlValue(doc, BAD_CAST "//s:Body//s:Fault//s:Reason//s:Text", error_msg, 1024) == 0) {
+        return -1;
+    }
+    return 0;
+}
+
+void addUsernameDigestHeader(xmlNodePtr root, xmlNsPtr ns_env, char *user, char *password, time_t offset) {
+    srand (time(NULL));
+
+#ifdef _WIN32
+    _setmode(0, O_BINARY);
+#endif
+
+    unsigned int nonce_chunk_size = 20;
+    unsigned char nonce_buffer[20];
+    char nonce_base64[1024] = {0};
+    char time_holder[1024] = {0};
+    char digest_base64[1024] = {0};
+
+    for (int i=0; i<nonce_chunk_size; i++) {
+        nonce_buffer[i] = (unsigned char)rand();
+    }
+
+    unsigned char nonce_result[30];
+
+    getBase64(nonce_buffer, nonce_chunk_size, nonce_result);
+    strcpy(nonce_base64, (const char *)nonce_result);
+
+    char time_buffer[1024];
+    time_t now = time(NULL);
+    now = now + offset;
+    size_t time_buffer_length = strftime(time_buffer, 1024, "%Y-%m-%dT%H:%M:%S.", gmtime(&now));
+    time_buffer[time_buffer_length] = '\0';
+    int millisec;
+    struct timeval tv;
+#ifdef _WIN32
+    static const uint64_t EPOCH = ((uint64_t) 116444736000000000ULL);
+
+    SYSTEMTIME  system_time;
+    FILETIME    file_time;
+    uint64_t    time;
+
+    GetSystemTime( &system_time );
+    SystemTimeToFileTime( &system_time, &file_time );
+    time =  ((uint64_t)file_time.dwLowDateTime )      ;
+    time += ((uint64_t)file_time.dwHighDateTime) << 32;
+
+    tv.tv_sec  = (long) ((time - EPOCH) / 10000000L);
+    tv.tv_usec = (long) (system_time.wMilliseconds * 1000);
+#else
+    gettimeofday(&tv, NULL);
+#endif
+    millisec = tv.tv_usec/1000.0;
+    char milli_buf[16] = {0};
+    sprintf(milli_buf, "%03dZ", millisec);
+    strcat(time_buffer, milli_buf);
+
+    unsigned char hash[20];
+
+    SHA1_CTX ctx;
+    SHA1Init(&ctx);
+    SHA1Update(&ctx, nonce_buffer, nonce_chunk_size);
+    SHA1Update(&ctx, (const unsigned char *)time_buffer, strlen(time_buffer));
+    SHA1Update(&ctx, (const unsigned char *)password, strlen(password));
+    SHA1Final(hash, &ctx);
+
+    unsigned int digest_chunk_size = SHA1_DIGEST_SIZE;
+    unsigned char digest_result[128];
+    getBase64(hash, digest_chunk_size, digest_result);
+
+    strcpy(time_holder, time_buffer);
+    strcpy(digest_base64, (const char *)digest_result);
+
+    xmlNsPtr ns_wsse = xmlNewNs(root, BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd", BAD_CAST "wsse");
+    xmlNsPtr ns_wsu = xmlNewNs(root, BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd", BAD_CAST "wsu");
+    xmlNodePtr header = xmlNewTextChild(root, ns_env, BAD_CAST "Header", NULL);
+    xmlNodePtr security = xmlNewTextChild(header, ns_wsse, BAD_CAST "Security", NULL);
+    xmlNewProp(security, BAD_CAST "SOAP-ENV:mustUnderstand", BAD_CAST "1");
+    xmlNodePtr username_token = xmlNewTextChild(security, ns_wsse, BAD_CAST "UsernameToken", NULL);
+    xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Username", BAD_CAST user);
+    xmlNodePtr pwd = xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Password", BAD_CAST digest_base64);
+    xmlNewProp(pwd, BAD_CAST "Type", BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordDigest");
+    xmlNodePtr nonce = xmlNewTextChild(username_token, ns_wsse, BAD_CAST "Nonce", BAD_CAST nonce_base64);
+    xmlNewProp(nonce, BAD_CAST "EncodingType", BAD_CAST "http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-soap-message-security-1.0#Base64Binary");
+    xmlNewTextChild(username_token, ns_wsu, BAD_CAST "Created", BAD_CAST time_holder);
+}
+
+void getBase64(unsigned char * buffer, int chunk_size, unsigned char * result) {
+    char *c = (char *)result;
+    int cnt = 0;
+    base64_encodestate s;
+    base64_init_encodestate(&s);
+    cnt = base64_encode_block((char *)buffer, chunk_size, c, &s);
+    c += cnt;
+    cnt = base64_encode_blockend(c, &s);
+    c += cnt;
+    *c = 0;
+}
+
+void addHttpHeader(xmlDocPtr doc, xmlNodePtr root, char *xaddrs, char *post_type, char cmd[], int cmd_length) {
+    xmlOutputBufferPtr outputbuffer = xmlAllocOutputBuffer(NULL);
+    xmlNodeDumpOutput(outputbuffer, doc, root, 0, 0, NULL);
+    int size = xmlOutputBufferGetSize(outputbuffer);
+
+    char xml[8192] = {0};
+    if (size > 8191) {
+        fprintf(stderr, "xmlOutputBufferGetSize too big %d\n", size);
+        strncat(xml, (char*)xmlOutputBufferGetContent(outputbuffer), 8191);
+    } else {
+        strcpy(xml, (char*)xmlOutputBufferGetContent(outputbuffer));
+    }
+
+
+    xmlOutputBufferFlush(outputbuffer);
+    xmlOutputBufferClose(outputbuffer);
+    xmlFreeDoc(doc);
+
+    char c_xml_size[6];
+    sprintf(c_xml_size, "%d", size);
+    int xml_size_length = strlen(c_xml_size)+1;
+
+    char tmp[128] = {0};
+    char * mark = strstr(xaddrs, "//");
+    int start = mark-xaddrs+2;
+    int tmp_len = strlen(xaddrs);
+    int j;
+    for (j=0; j<tmp_len-start; j++) {
+        tmp[j] = xaddrs[j+start];
+    }
+    tmp[j] = '\0';
+
+    mark = strstr(tmp, "/");
+    int end = mark-tmp;
+    char tmp2[128] = {0};
+    for (j=0; j<end; j++) {
+        tmp2[j] = tmp[j];
+    }
+    tmp2[j] = '\0';
+
+    char host[128] = {0};
+    char port_buf[128] = {0};
+    mark = strstr(tmp2, ":");
+    if (mark == NULL) {
+        strcpy(host, tmp2);
+        strcpy(port_buf, "80");
+    } else {
+        start = mark-tmp2;
+        for (j=0; j<start; j++) {
+            host[j] = tmp2[j];
+        }
+        host[j] = '\0';
+        tmp_len = strlen(tmp2);
+        for (j=start+1; j<tmp_len; j++) {
+            port_buf[j-(start+1)] = tmp2[j];
+        }
+        port_buf[j-(start+1)] = '\0';
+    }
+    int port = atoi(port_buf);
+
+    char content[] =
+    "User-Agent: Generic\r\n"
+    "Connection: Close\r\n"
+    "Accept-Encoding: gzip, deflate\r\n"
+    "Content-Type: application/soap+xml; charset=utf-8;\r\n"
+    "Host: ";
+    char content_length[] = "\r\nContent-Length: ";
+
+    char http_terminate[5];
+    http_terminate[0] = '\r';
+    http_terminate[1] = '\n';
+    http_terminate[2] = '\r';
+    http_terminate[3] = '\n';
+    http_terminate[4] = '\0';
+
+    int p = strlen(post_type)+1;
+    int h = strlen(host)+1;
+    int c = sizeof(content);
+    int cl = sizeof(content_length);
+    int cmd_size = p + c + h + cl + xml_size_length + size + 1;
+    int i;
+    int s;
+    for (i=0; i<p-1; i++)
+        cmd[i] = post_type[i];
+    s = i;
+    for (i=0; i<c-1; i++)
+        cmd[s+i] = content[i];
+    s = s+i;
+    for (i=0; i<h-1; i++)
+        cmd[s+i] = host[i];
+    s = s+i;
+    for (i=0; i<cl-1; i++)
+        cmd[s+i] = content_length[i];
+    s = s+i;
+    for (i=0; i<xml_size_length-1; i++)
+        cmd[s+i] = c_xml_size[i];
+    s = s+i;
+    for (i=0; i<5-1; i++)
+        cmd[s+i] = http_terminate[i];
+    s = s+i;
+    for (i=0; i<size; i++)
+        cmd[s+i] = xml[i];
+    cmd[cmd_size] = '\0';
+}
+
+void getUUID(char uuid_buf[47]) {
+    srand(time(NULL));
+    strcpy(uuid_buf, "urn:uuid:");
+    for (int i=0; i<16; i++) {
+        char buf[3];
+        sprintf(buf, "%02x", (unsigned char) rand());
+        strcat(uuid_buf, buf);
+        if (i==3 || i==5 || i==7 || i==9)
+            strcat(uuid_buf, "-");
+    }
+}
+
+int broadcast(struct OnvifSession *onvif_session) {
+    strcpy(preferred_network_address, onvif_session->preferred_network_address);
+    struct sockaddr_in broadcast_address;
+    int broadcast_socket;
+    char broadcast_message[1024] = {0};
+    unsigned int address_size;
+    int error_code;
+
+    if (onvif_session->discovery_msg_id == 1)
+        getDiscoveryXml(broadcast_message, 1024, onvif_session->uuid);
+    else if (onvif_session->discovery_msg_id == 2)
+        getDiscoveryXml2(broadcast_message, 1024);
+
+    int broadcast_message_length = strlen(broadcast_message);
+    broadcast_socket = socket(AF_INET, SOCK_DGRAM, IPPROTO_UDP);
+    setSocketOptions(broadcast_socket);
+    for (int k=0; k<128; k++) {
+        for (int j=0; j<8192; j++) {
+            onvif_session->buf[k][j] = '\0';
+        }
+    }
+
+    memset((char *) &broadcast_address, 0, sizeof(broadcast_address));
+    broadcast_address.sin_family = AF_INET;
+    broadcast_address.sin_port = htons(3702);
+    broadcast_address.sin_addr.s_addr = inet_addr("239.255.255.250");
+    int status = sendto(broadcast_socket, broadcast_message, broadcast_message_length, 0, (struct sockaddr*)&broadcast_address, sizeof(broadcast_address));
+    if (status < 0) {
+        //error
+    }
+
+    int i = 0;
+    unsigned char looping = 1;
+    address_size = sizeof(broadcast_address);
+    while(looping) {
+        onvif_session->len[i] = recvfrom(broadcast_socket, onvif_session->buf[i], sizeof(onvif_session->buf[i]), 0, (struct sockaddr*) &broadcast_address, &address_size);
+        if (onvif_session->len[i] > 0) {
+            onvif_session->buf[i][onvif_session->len[i]] = '\0';
+            i++;
+        } else {
+            looping = 0;
+            if (onvif_session->len[i] < 0) {
+                //error
+            }
+        }
+    }
+
+#ifdef _WIN32
+    closesocket(broadcast_socket);
+#else
+    close(broadcast_socket);
+#endif
+
+    return i;
+}
+
+void getActiveNetworkInterfaces(struct OnvifSession* onvif_session)
+{
+#ifdef _WIN32
+    PIP_ADAPTER_INFO pAdapterInfo;
+    PIP_ADAPTER_INFO pAdapter = NULL;
+    DWORD dwRetVal = 0;
+    int count = 0;
+
+    ULONG ulOutBufLen = sizeof (IP_ADAPTER_INFO);
+    pAdapterInfo = (IP_ADAPTER_INFO *) malloc(sizeof (IP_ADAPTER_INFO));
+    if (pAdapterInfo == NULL) {
+        printf("Error allocating memory needed to call GetAdaptersinfo\n");
+        return;
+    }
+
+    if (GetAdaptersInfo(pAdapterInfo, &ulOutBufLen) == ERROR_BUFFER_OVERFLOW) {
+        free(pAdapterInfo);
+        pAdapterInfo = (IP_ADAPTER_INFO *) malloc(ulOutBufLen);
+        if (pAdapterInfo == NULL) {
+            printf("Error allocating memory needed to call GetAdaptersinfo\n");
+            return;
+        }
+    }
+
+    if ((dwRetVal = GetAdaptersInfo(pAdapterInfo, &ulOutBufLen)) == NO_ERROR) {
+        pAdapter = pAdapterInfo;
+        while (pAdapter) {
+            if (strcmp(pAdapter->IpAddressList.IpAddress.String, "0.0.0.0")) {
+                char interface_info[1024];
+                sprintf(interface_info, "%s - %s", pAdapter->IpAddressList.IpAddress.String, pAdapter->Description);
+                printf("Network interface info %s\n", interface_info);
+                //args.push_back(interface_info);
+                strncpy(onvif_session->active_network_interfaces[count], interface_info, 40);
+                count += 1;
+            }
+            pAdapter = pAdapter->Next;
+        }
+    } 
+    else {
+        printf("GetAdaptersInfo failed with error: %d", dwRetVal);
+    }
+    if (pAdapterInfo)
+        free(pAdapterInfo);
+#else
+    struct ifaddrs *ifaddr;
+    int family, s;
+    char host[NI_MAXHOST];
+    int count = 0;
+
+    if (getifaddrs(&ifaddr) == -1) {
+        printf("Error: getifaddrs failed - %s\n", strerror(errno));
+        return;
+    }
+
+    for (struct ifaddrs *ifa = ifaddr; ifa != NULL; ifa = ifa->ifa_next) {
+        if (ifa->ifa_addr == NULL)
+            continue;
+
+        family = ifa->ifa_addr->sa_family;
+
+        if (family == AF_INET ) {
+            s = getnameinfo(ifa->ifa_addr, 
+                    sizeof(struct sockaddr_in),
+                    host, NI_MAXHOST,
+                    NULL, 0, NI_NUMERICHOST);
+
+            if (s != 0) {
+                printf("getnameinfo() failed: %s\n", gai_strerror(s));
+                continue;
+            }
+
+            if (strcmp(ifa->ifa_name, "lo")) {
+                strcpy(onvif_session->active_network_interfaces[count], host);
+                strcat(onvif_session->active_network_interfaces[count], " - ");
+                strcat(onvif_session->active_network_interfaces[count], ifa->ifa_name);
+                count += 1;
+            }
+        } 
+    }
+    freeifaddrs(ifaddr);
+#endif
+}
+
+void getIPAddress(char buf[128]) {
+#ifdef _WIN32
+    PMIB_IPADDRTABLE pIPAddrTable;
+    DWORD dwSize = 0;
+    DWORD dwRetVal = 0;
+    IN_ADDR IPAddr;
+    
+    pIPAddrTable = (MIB_IPADDRTABLE *) malloc(sizeof(MIB_IPADDRTABLE));
+    if (pIPAddrTable) {
+        if (GetIpAddrTable(pIPAddrTable, &dwSize, 0) == ERROR_INSUFFICIENT_BUFFER) {
+            free(pIPAddrTable);
+            pIPAddrTable = (MIB_IPADDRTABLE *) malloc(dwSize);
+        }
+        if (pIPAddrTable == NULL) {
+            return;
+        }
+    }
+
+    if ((dwRetVal = GetIpAddrTable(pIPAddrTable, &dwSize, 0)) != NO_ERROR) {
+        return;
+    }
+
+    int p = 0;
+    while (p < (int)pIPAddrTable->dwNumEntries) {
+        if (pIPAddrTable->table[p].dwAddr != inet_addr("127.0.0.1") && pIPAddrTable->table[p].dwMask == inet_addr("255.255.255.0")) {
+            IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwAddr;
+            strcpy(buf, inet_ntoa(IPAddr));
+            p = (int)pIPAddrTable->dwNumEntries;
+        }
+        p++;
+    }
+
+    if (pIPAddrTable) {
+        free(pIPAddrTable);
+        pIPAddrTable = NULL;
+    }
+
+#else
+
+#if defined(__APPLE__) || defined(__FreeBSD__)
+
+    char *address;
+    struct ifaddrs *interfaces = NULL;
+    struct ifaddrs *temp_addr = NULL;
+    int success = 0;
+    success = getifaddrs(&interfaces);
+    if (success == 0) {
+        temp_addr = interfaces;
+        while (temp_addr != NULL) {
+            address = inet_ntoa(((struct sockaddr_in *)temp_addr->ifa_addr)->sin_addr);
+            if (strcmp(address, "127.0.0.1") != 0)
+                strcpy(buf, address);
+        }
+        temp_addr = temp_addr->ifa_next;
+    }
+    freeifaddrs(interfaces);
+
+#else
+    struct ifconf ifc;
+    struct ifreq ifr[10];
+    int sd, ifc_num, addr,mask, i;
+
+    sd = socket(PF_INET, SOCK_DGRAM, 0);
+    if (sd > 0) {
+        ifc.ifc_len = sizeof(ifr);
+        ifc.ifc_ifcu.ifcu_buf = (caddr_t)ifr;
+
+        if (ioctl(sd, SIOCGIFCONF, &ifc) == 0) {
+            ifc_num = ifc.ifc_len / sizeof(struct ifreq);
+
+            for (i = 0; i < ifc_num; ++i) {
+                if (ifr[i].ifr_addr.sa_family != AF_INET) {
+                    continue;
+                }
+
+                if (ioctl(sd, SIOCGIFNETMASK, &ifr[i]) == 0) {
+                    mask = ((struct sockaddr_in *)(&ifr[i].ifr_netmask))->sin_addr.s_addr;
+                    char mask_buf[128];
+                    sprintf(mask_buf, "%d.%d.%d.%d", INT_TO_ADDR(mask));
+                    if (strcmp(mask_buf, "255.255.255.0") == 0) {
+                        if (ioctl(sd, SIOCGIFADDR, &ifr[i]) == 0) {
+                            addr = ((struct sockaddr_in *)(&ifr[i].ifr_addr))->sin_addr.s_addr;
+                            char addr_buf[128];
+                            sprintf(addr_buf, "%d.%d.%d.%d", INT_TO_ADDR(addr));
+                            if (strcmp(addr_buf, "127.0.0.1") != 0) {
+                                printf("-----------------------------------------------%s\n", addr_buf);
+                                strcpy(buf, addr_buf);
+                            }
+                        }
+                    }
+                }
+            }
+        }
+    }
+    close(sd);
+#endif /* not  __APPLE__ || __FreeBSD__ */
+#endif /* not _WIN32 */
+}
+
+int mask2prefix(char *mask_buf) {
+    struct in_addr mask;
+    inet_pton(AF_INET, mask_buf, &mask);
+    uint32_t number = ntohl(mask.s_addr);
+    int count = 0;
+    unsigned int step = 0;
+    while (number > 0) {
+        if (number & 1) {
+            step = 1;
+            count++;
+        } else {
+            if (step) {
+                return -1;
+            }
+        }
+        number >>=1;
+    }
+    return count;
+}
+
+void prefix2mask(int prefix, char mask_buf[128]) {
+    struct in_addr mask;
+    uint32_t number;
+
+    if (prefix) {
+        number = htonl(~((1 << (32-prefix)) - 1));
+    } else {
+        number = htonl(0);
+    }
+
+    mask.s_addr = number;
+    inet_ntop(AF_INET, &mask, mask_buf, 128);
+}
+
+int setSocketOptions(int socket) {
+    struct timeval tv;
+    tv.tv_sec = 0;
+    tv.tv_usec = 500000;
+    int broadcast = 500;
+    char loopch = 0;
+    int status = 0;
+    struct in_addr localInterface;
+
+#ifdef _WIN32
+    PMIB_IPADDRTABLE pIPAddrTable;
+    DWORD dwSize = 0;
+    DWORD dwRetVal = 0;
+    IN_ADDR IPAddr;
+
+    pIPAddrTable = (MIB_IPADDRTABLE *) malloc(sizeof(MIB_IPADDRTABLE));
+    if (pIPAddrTable) {
+        if (GetIpAddrTable(pIPAddrTable, &dwSize, 0) == ERROR_INSUFFICIENT_BUFFER) {
+            free(pIPAddrTable);
+            pIPAddrTable = (MIB_IPADDRTABLE *) malloc(dwSize);
+        }
+        if (pIPAddrTable == NULL) {
+            printf("Memory allocation failed for GetIpAddrTable\n");
+            return -1;
+        }
+    }
+
+    if ((dwRetVal = GetIpAddrTable(pIPAddrTable, &dwSize, 0)) != NO_ERROR) {
+        printf("GetIpAddrTable failed with error %d\n", dwRetVal);
+        return -1;
+    }
+
+    int p = 0;
+    while (p < (int)pIPAddrTable->dwNumEntries) {
+        IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwAddr;
+        IPAddr.S_un.S_addr = (u_long)pIPAddrTable->table[p].dwMask;
+        if (pIPAddrTable->table[p].dwAddr != inet_addr("127.0.0.1") && pIPAddrTable->table[p].dwMask == inet_addr("255.255.255.0")) {
+            if (strlen(preferred_network_address) > 0) {
+                localInterface.s_addr = inet_addr(preferred_network_address);
+            }
+            else {
+                localInterface.s_addr = pIPAddrTable->table[p].dwAddr;
+            }
+            status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_IF, (const char *)&localInterface, sizeof(localInterface));
+            if (status < 0)
+                printf("ip_multicast_if error");
+            p = (int)pIPAddrTable->dwNumEntries;
+        }
+        p++;
+    }
+
+    if (pIPAddrTable) {
+        free(pIPAddrTable);
+        pIPAddrTable = NULL;
+    }
+
+    status = setsockopt(socket, SOL_SOCKET, SO_RCVTIMEO, (const char *)&broadcast, sizeof(broadcast));
+#else
+    if (strlen(preferred_network_address) > 0) {
+        localInterface.s_addr = inet_addr(preferred_network_address);
+        status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_IF, (const char *)&localInterface, sizeof(localInterface));
+        if (status < 0)
+            printf("ip_multicast_if error");
+    }
+    status = setsockopt(socket, SOL_SOCKET, SO_RCVTIMEO, (struct timeval *)&tv, sizeof(struct timeval));
+#endif
+    status = setsockopt(socket, IPPROTO_IP, IP_MULTICAST_LOOP, (char *)&loopch, sizeof(loopch));
+    return 0;
+}
+
+
+
+#ifdef __MINGW32__
+int inet_pton(int af, const char *src, void *dst) {
+    struct sockaddr_storage ss;
+    int size = sizeof(ss);
+    char src_copy[INET6_ADDRSTRLEN+1];
+
+    ZeroMemory(&ss, sizeof(ss));
+    strncpy (src_copy, src, INET6_ADDRSTRLEN+1);
+    src_copy[INET6_ADDRSTRLEN] = 0;
+
+    if (WSAStringToAddress(src_copy, af, NULL, (struct sockaddr *)&ss, &size) == 0) {
+        switch(af) {
+	case AF_INET:
+	    *(struct in_addr *)dst = ((struct sockaddr_in *)&ss)->sin_addr;
+	    return 1;
+	case AF_INET6:
+	    *(struct in6_addr *)dst = ((struct sockaddr_in6 *)&ss)->sin6_addr;
+	    return 1;
+	}
+    }
+    return 0;
+}
+
+const char *inet_ntop(int af, const void *src, char *dst, socklen_t size) {
+    struct sockaddr_storage ss;
+    unsigned long s = size;
+
+    ZeroMemory(&ss, sizeof(ss));
+    ss.ss_family = af;
+
+    switch(af) {
+    case AF_INET:
+        ((struct sockaddr_in *)&ss)->sin_addr = *(struct in_addr *)src;
+	break;
+    case AF_INET6:
+        ((struct sockaddr_in6 *)&ss)->sin6_addr = *(struct in6_addr *)src;
+	break;
+    default:
+        return NULL;
+    }
+
+    return (WSAAddressToString((struct sockaddr *)&ss, sizeof(ss), NULL, dst, &s) == 0)?dst : NULL;
+}
+#endif
+
+
+void extractOnvifService(char service[1024], bool post) {
+    int length = strlen(service);
+    char *sub = strstr(service, "//");
+    if (sub != NULL) {
+        int mark = sub - service;
+        mark = mark+2;
+
+        int i;
+        for (i=0; i<length-mark; i++) {
+            service[i] = service[i+mark];
+        }
+        service[i] = '\0';
+
+        sub = strstr(service, " ");
+        if (sub != NULL) {
+            mark = sub - service;
+            service[mark] = '\0';
+        }
+
+        length = strlen(service);
+        sub = strstr(service, "/");
+        if (sub != NULL) {
+            mark = sub - service;
+            for (i=0; i<length-mark; i++) {
+                service[i] = service[i+mark];
+            }
+            service[i] = 0;
+
+            if (post) {
+                char temp_buf[128] = {0};
+                strcat(temp_buf, "POST ");
+                strcat(temp_buf, service);
+                strcat(temp_buf, " HTTP/1.1\r\n");
+                strcpy(service, "");
+                strcpy(service, temp_buf);
+            }
+        }
+    }
+}
+
+
+void extractHost(char *xaddrs, char host[128]) {
+    char tmp[128] = {0};
+    char *mark = strstr(xaddrs, "//");
+    int start = mark-xaddrs+2;
+    int tmp_len = strlen(xaddrs);
+    int j;
+    for (j=0; j<tmp_len-start; j++) {
+        tmp[j] = xaddrs[j+start];
+    }
+    tmp[j] = '\0';
+
+    mark = strstr(tmp, "/");
+    int end = mark-tmp;
+    char tmp2[128] = {0};
+    for (j=0; j<end; j++) {
+        tmp2[j] = tmp[j];
+    }
+    tmp2[j] = '\0';
+
+    mark = strstr(tmp2, ":");
+    if (mark == NULL) {
+        strcpy(host, tmp2);
+    } else {
+        start = mark-tmp2;
+        for (j=0; j<start; j++) {
+            host[j] = tmp2[j];
+        }
+        host[j] = '\0';
+    }
+}
+
+void getScopeField(char *scope, char *field_name, char cleaned[1024]) {
+    char *field;
+    char field_contents[1024] = {0};
+    char *mark;
+    int length;
+    char *result = NULL;
+
+    field = strstr(scope, field_name);
+    if (field != NULL) {
+        field = field + strlen(field_name);
+        mark = strstr(field, " ");
+        if (mark != NULL) {
+            length = mark - field;
+            strncpy(field_contents, field, length);
+        } else {
+            strcpy(field_contents, field);
+        }
+
+        length = strlen(field_contents);
+        int offset = 0;
+        int j;
+        for (int i=0; i<length; i++) {
+            j = i - offset;
+            if (field_contents[i] == '%') {
+                char middle[3] = {0};
+                i++; offset++;
+                middle[0] = field_contents[i];
+                i++; offset++;
+                middle[1] = field_contents[i];
+                char *ptr;
+                int result = strtol(middle, &ptr, 16);
+                cleaned[j] = result;
+            } else {
+                cleaned[j] = field_contents[i];
+            }
+        }
+        cleaned[length] = '\0';
+    }
+}
+
+void getCameraName(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
+    xmlDocPtr xml_input = xmlParseMemory(onvif_session->buf[ordinal], onvif_session->len[ordinal]);
+    for(int i=0; i<1024; i++)
+        onvif_data->camera_name[i] = '\0';
+
+    char scopes[8192];
+    getXmlValue(xml_input, BAD_CAST "//s:Body//d:ProbeMatches//d:ProbeMatch//d:Scopes", scopes, 8192);
+
+    char temp_mfgr[1024] = {0};
+    char temp_hdwr[1024] = {0};
+
+    getScopeField(scopes, "onvif://www.onvif.org/name/", temp_mfgr);
+    getScopeField(scopes, "onvif://www.onvif.org/hardware/", temp_hdwr);
+
+    if (strlen(temp_mfgr) > 0) {
+        strcat(onvif_data->camera_name, temp_mfgr);
+    }
+    if (strlen(temp_hdwr) > 0) {
+        if (strstr(temp_mfgr, temp_hdwr) == NULL) {
+            strcat(onvif_data->camera_name, " ");
+            strcat(onvif_data->camera_name, temp_hdwr);
+        }
+    }
+
+    if (strlen(onvif_data->camera_name)  == 0)
+        strcpy(onvif_data->camera_name, "UNKNOWN CAMERA");
+
+    xmlFreeDoc(xml_input);
+}
+
+bool extractXAddrs(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
+    bool result = false;
+    xmlDocPtr xml_input = xmlParseMemory(onvif_session->buf[ordinal], onvif_session->len[ordinal]);
+    if (getXmlValue(xml_input, BAD_CAST "//s:Body//d:ProbeMatches//d:ProbeMatch//d:XAddrs", onvif_data->xaddrs, 1024) == 0) {
+        char *sub = strstr(onvif_data->xaddrs, " ");
+        if (sub != NULL) {
+            int mark = sub - onvif_data->xaddrs;
+            onvif_data->xaddrs[mark] = '\0';
+        }
+        strcpy(onvif_data->device_service, onvif_data->xaddrs);
+        result = true;
+    }
+    xmlFreeDoc(xml_input);
+    return result;
+}
+
+void clearData(struct OnvifData *onvif_data) {
+    for (int i=0; i<16; i++) {
+        for (int j=0; j<128; j++) {
+            onvif_data->resolutions_buf[i][j] = '\0';
+        }
+    }
+    for (int i=0; i<128; i++) {
+        onvif_data->videoEncoderConfigurationToken[i] = '\0';
+        onvif_data->networkInterfaceToken[i] = '\0';
+        onvif_data->networkInterfaceName[i] = '\0';
+        onvif_data->ip_address_buf[i] = '\0';
+        onvif_data->default_gateway_buf[i] = '\0';
+        onvif_data->dns_buf[i] = '\0';
+        onvif_data->mask_buf[i] = '\0';
+        onvif_data->videoSourceConfigurationToken[i] = '\0';
+        onvif_data->video_encoder_name_buf[i] = '\0';
+        onvif_data->h264_profile_buf[i] = '\0';
+        onvif_data->multicast_address_type_buf[i] = '\0';
+        onvif_data->multicast_address_buf[i] = '\0';
+        onvif_data->session_time_out_buf[i] = '\0';
+        onvif_data->media_service[i] = '\0';
+        onvif_data->imaging_service[i] = '\0';
+        onvif_data->ptz_service[i] = '\0';
+        onvif_data->event_service[i] = '\0';
+        onvif_data->profileToken[i] = '\0';
+        onvif_data->username[i] = '\0';
+        onvif_data->password[i] = '\0';
+        onvif_data->encoding[i] = '\0';
+    	onvif_data->timezone[i] = '\0';
+    	onvif_data->ntp_type[i] = '\0';
+    	onvif_data->ntp_addr[i] = '\0';
+        onvif_data->host[i] = '\0';
+        onvif_data->serial_number[i] = '\0';
+    }
+    for (int i=0; i<1024; i++) {
+        onvif_data->xaddrs[i] = '\0';
+        onvif_data->device_service[i] = '\0';
+        onvif_data->stream_uri[i] = '\0';
+        onvif_data->camera_name[i] = '\0';
+        onvif_data->host_name[i] = '\0';
+    }
+    onvif_data->gov_length_min = 0;
+    onvif_data->gov_length_max = 0;
+    onvif_data->frame_rate_min = 0;
+    onvif_data->frame_rate_max = 0;
+    onvif_data->bitrate_min = 0;
+    onvif_data->bitrate_max = 0;
+    onvif_data->width = 0;
+    onvif_data->height = 0;
+    onvif_data->gov_length = 0;
+    onvif_data->frame_rate = 0;
+    onvif_data->bitrate = 0;
+    onvif_data->use_count = 0;
+    onvif_data->quality = 0;
+    onvif_data->multicast_port = 0;
+    onvif_data->multicast_ttl = 0;
+    onvif_data->autostart = false;
+    onvif_data->prefix_length = 0;
+    onvif_data->dhcp_enabled = false;
+    onvif_data->brightness_min = 0;
+    onvif_data->brightness_max = 0;
+    onvif_data->saturation_min = 0;
+    onvif_data->saturation_max = 0;
+    onvif_data->contrast_min = 0;
+    onvif_data->contrast_max = 0;
+    onvif_data->sharpness_min = 0;
+    onvif_data->sharpness_max = 0;
+    onvif_data->brightness = 0;
+    onvif_data->saturation = 0;
+    onvif_data->contrast = 0;
+    onvif_data->sharpness = 0;
+    onvif_data->time_offset = 0;
+    onvif_data->event_listen_port = 0;
+    onvif_data->guaranteed_frame_rate = false;
+    onvif_data->conf_width = 0;
+    onvif_data->conf_height = 0;
+    onvif_data->conf_frame_rate_limit = 0;
+    onvif_data->conf_encoding_interval = 0;
+    onvif_data->conf_bitrate_limit = 0;
+    onvif_data->datetimetype = '\0';
+    onvif_data->dst = false;
+    onvif_data->ntp_dhcp = false;
+}
+
+void copyData(struct OnvifData *dst, struct OnvifData *src) {
+    for (int i=0; i<16; i++) {
+        for (int j=0; j<128; j++) {
+            dst->resolutions_buf[i][j] = src->resolutions_buf[i][j];
+        }
+    }
+    for (int i=0; i<128; i++) {
+        dst->videoEncoderConfigurationToken[i] = src->videoEncoderConfigurationToken[i];
+        dst->networkInterfaceToken[i] = src->networkInterfaceToken[i];
+        dst->networkInterfaceName[i] = src->networkInterfaceName[i];
+        dst->ip_address_buf[i] = src->ip_address_buf[i];
+        dst->default_gateway_buf[i] = src->default_gateway_buf[i];
+        dst->dns_buf[i] = src->dns_buf[i];
+        dst->videoSourceConfigurationToken[i] = src->videoSourceConfigurationToken[i];
+        dst->video_encoder_name_buf[i] = src->video_encoder_name_buf[i];
+        dst->h264_profile_buf[i] = src->h264_profile_buf[i];
+        dst->multicast_address_type_buf[i] = src->multicast_address_type_buf[i];
+        dst->multicast_address_buf[i] = src->multicast_address_buf[i];
+        dst->session_time_out_buf[i] = src->session_time_out_buf[i];
+        dst->media_service[i] = src->media_service[i];
+        dst->imaging_service[i] = src->imaging_service[i];
+        dst->ptz_service[i] = src->ptz_service[i];
+        dst->event_service[i] = src->event_service[i];
+        dst->profileToken[i] = src->profileToken[i];
+        dst->username[i] = src->username[i];
+        dst->password[i] = src->password[i];
+        dst->encoding[i] = src->encoding[i];
+    	dst->timezone[i] = src->timezone[i];
+    	dst->ntp_type[i] = src->ntp_type[i];
+    	dst->ntp_addr[i] = src->ntp_addr[i];
+        dst->host[i] = src->host[i];
+        dst->serial_number[i] = src->serial_number[i];
+    }
+    for (int i=0; i<1024; i++) {
+        dst->xaddrs[i] = src->xaddrs[i];
+        dst->device_service[i] = src->device_service[i];
+        dst->stream_uri[i] = src->stream_uri[i];
+        dst->camera_name[i] = src->camera_name[i];
+        dst->host_name[i] = src->host_name[i];
+        dst->last_error[i] = src->last_error[i];
+    }
+    dst->gov_length_min = src->gov_length_min;
+    dst->gov_length_max = src->gov_length_max;
+    dst->frame_rate_min = src->frame_rate_min;
+    dst->frame_rate_max = src->frame_rate_max;
+    dst->bitrate_min = src->bitrate_min;
+    dst->bitrate_max = src->bitrate_max;
+    dst->width = src->width;
+    dst->height = src->height;
+    dst->gov_length = src->gov_length;
+    dst->frame_rate = src->frame_rate;
+    dst->bitrate = src->bitrate;
+    dst->use_count = src->use_count;
+    dst->quality = src->quality;
+    dst->multicast_port = src->multicast_port;
+    dst->multicast_ttl = src->multicast_ttl;
+    dst->autostart = src->autostart;
+    dst->prefix_length = src->prefix_length;
+    dst->dhcp_enabled = src->dhcp_enabled;
+    dst->brightness_min = src->brightness_min;
+    dst->brightness_max = src->brightness_max;
+    dst->saturation_min = src->saturation_min;
+    dst->saturation_max = src->saturation_max;
+    dst->contrast_min = src->contrast_min;
+    dst->contrast_max = src->contrast_max;
+    dst->sharpness_min = src->sharpness_min;
+    dst->sharpness_max = src->sharpness_max;
+    dst->brightness = src->brightness;
+    dst->saturation = src->saturation;
+    dst->contrast = src->contrast;
+    dst->sharpness = src->sharpness;
+    dst->time_offset = src->time_offset;
+    dst->event_listen_port = src->event_listen_port;
+    dst->guaranteed_frame_rate = src->guaranteed_frame_rate;
+    dst->conf_width = src->conf_width;
+    dst->conf_height = src->conf_height;
+    dst->conf_frame_rate_limit = src->conf_frame_rate_limit;
+    dst->conf_encoding_interval = src->conf_encoding_interval;
+    dst->conf_bitrate_limit = src->conf_bitrate_limit;
+    dst->datetimetype = src->datetimetype;
+    dst->dst = src->dst;
+    dst->ntp_dhcp = src->ntp_dhcp;
+}
+
+void initializeSession(struct OnvifSession *onvif_session) {
+    getUUID(onvif_session->uuid);
+    onvif_session->discovery_msg_id = 1;
+    xmlInitParser ();
+    for (int i=0; i<16; i++) {
+        for (int j=0; j<1024; j++) {
+            onvif_session->active_network_interfaces[i][j] = '\0';
+        }
+    }
+#ifdef _WIN32
+    WSADATA wsaData;
+    WSAStartup(MAKEWORD(2,2), &wsaData);
+#endif
+    strcpy(preferred_network_address, onvif_session->preferred_network_address);
+}
+
+void closeSession(struct OnvifSession *onvif_session) {
+#ifdef _WIN32
+    WSACleanup();
+#endif
+    xmlCleanupParser ();
+}
+
+bool prepareOnvifData(int ordinal, struct OnvifSession *onvif_session, struct OnvifData *onvif_data) {
+    clearData(onvif_data);
+    getCameraName(ordinal, onvif_session, onvif_data);
+    if (!extractXAddrs(ordinal, onvif_session, onvif_data))
+        return false;
+    extractOnvifService(onvif_data->device_service, true);
+    extractHost(onvif_data->xaddrs, onvif_data->host);
+    getTimeOffset(onvif_data);
+    return true;
+}
+
+int fillRTSPn(struct OnvifData *onvif_data, int profileIndex) {
+    int result = 0;
+    result = getCapabilities(onvif_data);
+    if (result == 0) {
+        result = getProfileToken(onvif_data, profileIndex);
+        if (result == 0) {
+            result = getStreamUri(onvif_data);
+        }
+    }
+    return result;
+}
+
+bool hasPTZ(struct OnvifData* onvif_data) {
+    if (strcmp(onvif_data->ptz_service, "") == 0)
+        return false;
+    else
+        return true;
+
+}
+
+void dumpXmlNode (xmlDocPtr doc, xmlNodePtr cur_node, char *prefix) {
+    const char *name;
+    const char *value;
+    char new_prefix[1024];
+    char attr[128];
+    xmlAttrPtr prop;
+
+    /* Traverse the tree */
+    for (; cur_node; cur_node = cur_node->next) {
+        if (cur_node->type == XML_ELEMENT_NODE) {
+            name = (char *)(cur_node->name);
+            value = (const char *)xmlNodeListGetString(doc, cur_node->xmlChildrenNode, 1);
+            if (value) {
+                printf("%s%s=%s\n", prefix ? prefix : "", name, value);
+            } else {
+                sprintf(new_prefix, "%s%s.", prefix ? prefix : "", name);
+                for (prop = cur_node->properties; prop; prop = prop->next) {
+                    if (prop->children && prop->children->content) {
+                        printf("%s%s=%s\n", new_prefix, prop->name, prop->children->content);
+                    }
+                }
+            }
+        }
+        dumpXmlNode(doc, cur_node->children, new_prefix);
+    }
+}
+
+/* Dump xml document */
+void dumpReply(xmlDocPtr reply) {
+    if (reply != NULL) {
+        xmlChar *xpath = BAD_CAST "//s:Body/*";
+        xmlXPathObjectPtr body = getNodeSet(reply, xpath);
+        if (body) {
+            xmlNodeSetPtr nodeset = body->nodesetval;
+            for (int i=0; i<nodeset->nodeNr; i++) {
+                xmlNodePtr cur = nodeset->nodeTab[i];
+                /* Skip error return */
+                if (strcmp((char *)cur->name, "Fault") != 0) {
+                    printf("[%s]\n", cur->name);
+                    dumpXmlNode(reply, cur->children, NULL);
+                }
+            }
+        }
+    }
+}
+
+/* Dump all available onvif device configuration */
+void dumpConfigAll (struct OnvifData *onvif_data) {
+    xmlDocPtr reply;
+
+    dump_reply = true;
+
+    getNetworkInterfaces(onvif_data);
+    getNetworkDefaultGateway(onvif_data);
+    getDNS(onvif_data);
+    getCapabilities(onvif_data);
+    getVideoEncoderConfigurationOptions(onvif_data);
+    getVideoEncoderConfiguration(onvif_data);
+    getProfile(onvif_data);
+    getOptions(onvif_data);
+    getImagingSettings(onvif_data);
+    getFirstProfileToken(onvif_data);
+    getTimeOffset(onvif_data);
+    getNTP(onvif_data);
+    getHostname(onvif_data);
+    getStreamUri(onvif_data);
+    getDeviceInformation(onvif_data);
+
+    dump_reply = false;
+}
```

### Comparing `libonvif-2.0.10/src/onvif.cpp` & `libonvif-2.0.9/src/onvif.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-/*******************************************************************************
-* onvif.cpp
-*
-* copyright 2023 Stephen Rhodes
-*
-* This library is free software; you can redistribute it and/or
-* modify it under the terms of the GNU Lesser General Public
-* License as published by the Free Software Foundation; either
-* version 2.1 of the License, or (at your option) any later version.
-*
-* This library is distributed in the hope that it will be useful,
-* but WITHOUT ANY WARRANTY; without even the implied warranty of
-* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-* Lesser General Public License for more details.
-*
-* You should have received a copy of the GNU Lesser General Public
-* License along with this library; if not, write to the Free Software
-* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-*
-*******************************************************************************/
-
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <pybind11/operators.h>
-#include <pybind11/functional.h>
-#include "onvifboss.h"
-
-namespace py = pybind11;
-
-namespace libonvif
-{
-
-PYBIND11_MODULE(libonvif, m)
-{
-    m.doc() = "pybind11 onvif plugin";
-    py::class_<Session>(m, "Session")
-        .def(py::init<>())
-        .def("active_interface", &Session::active_interface)
-        .def("getActiveInterfaces", &Session::getActiveInterfaces);
-    py::class_<Manager>(m, "Manager")
-        .def(py::init<>())
-        .def("startDiscover", &Manager::startDiscover)
-        .def("startFill", &Manager::startFill)
-        .def("startUpdateVideo", &Manager::startUpdateVideo)
-        .def("startUpdateImage", &Manager::startUpdateImage)
-        .def("startUpdateNetwork", &Manager::startUpdateNetwork)
-        .def("startUpdateTime" ,&Manager::startUpdateTime)
-        .def("startReboot", &Manager::startReboot)
-        .def("startReset", &Manager::startReset)
-        .def("startSetUser", &Manager::startSetUser)
-        .def("startSet", &Manager::startSet)
-        .def("startSetGotoPreset", &Manager::startSetGotoPreset)
-        .def("startMove", &Manager::startMove)
-        .def("startStop", &Manager::startStop)
-        .def_readwrite("discovered", &Manager::discovered)
-        .def_readwrite("getCredential", &Manager::getCredential)
-        .def_readwrite("getData", &Manager::getData)
-        .def_readwrite("filled", &Manager::filled)
-        .def_readwrite("preset", &Manager::preset)
-        .def_readwrite("x", &Manager::x)
-        .def_readwrite("y", &Manager::y)
-        .def_readwrite("z", &Manager::z)
-        .def_readwrite("stop_type", &Manager::stop_type)
-        .def_readwrite("new_password", &Manager::new_password)
-        .def_readwrite("interface", &Manager::interface)
-        .def_readwrite("onvif_data", &Manager::onvif_data);
-    py::class_<Data>(m, "Data")
-        .def(py::init<>())
-        .def(py::init<const Data&>())
-        .def("xaddrs", &Data::xaddrs)
-        .def("stream_uri", &Data::stream_uri)
-        .def("serial_number", &Data::serial_number)
-        .def("camera_name", &Data::camera_name)
-        .def("host", &Data::host)
-        .def("last_error", &Data::last_error)
-        .def("clearLastError", &Data::clearLastError)
-        .def("resolutions_buf", &Data::resolutions_buf)
-        .def("width", &Data::width)
-        .def("setWidth", &Data::setWidth)
-        .def("height", &Data::height)
-        .def("setHeight", &Data::setHeight)
-        .def("frame_rate_max", &Data::frame_rate_max)
-        .def("frame_rate_min", &Data::frame_rate_min)
-        .def("frame_rate", &Data::frame_rate)
-        .def("setFrameRate", &Data::setFrameRate)
-        .def("gov_length_max", &Data::gov_length_max)
-        .def("gov_length_min", &Data::gov_length_min)
-        .def("gov_length", &Data::gov_length)
-        .def("setGovLength", &Data::setGovLength)
-        .def("bitrate_max", &Data::bitrate_max)
-        .def("bitrate_min", &Data::bitrate_min)
-        .def("bitrate", &Data::bitrate)
-        .def("setBitrate", &Data::setBitrate)
-        .def("brightness_max", &Data::brightness_max)
-        .def("brightness_min", &Data::brightness_min)
-        .def("brightness", &Data::brightness)
-        .def("setBrightness", &Data::setBrightness)
-        .def("saturation_max", &Data::saturation_max)
-        .def("saturation_min", &Data::saturation_min)
-        .def("saturation", &Data::saturation)
-        .def("setSaturation", &Data::setSaturation)
-        .def("contrast_max", &Data::contrast_max)
-        .def("contrast_min", &Data::contrast_min)
-        .def("contrast", &Data::contrast)
-        .def("setContrast", &Data::setContrast)
-        .def("sharpness_max", &Data::sharpness_max)
-        .def("sharpness_min", &Data::sharpness_min)
-        .def("sharpness", &Data::sharpness)
-        .def("setSharpness", &Data::setSharpness)
-        .def("dhcp_enabled", &Data::dhcp_enabled)
-        .def("setDHCPEnabled", &Data::setDHCPEnabled)
-        .def("ip_address_buf", &Data::ip_address_buf)
-        .def("setIPAddressBuf", &Data::setIPAddressBuf)
-        .def("default_gateway_buf", &Data::default_gateway_buf)
-        .def("setDefaultGatewayBuf", &Data::setDefaultGatewayBuf)
-        .def("dns_buf", &Data::dns_buf)
-        .def("setDNSBuf", &Data::setDNSBuf)
-        .def("prefix_length", &Data::prefix_length)
-        .def("setPrefixLength", &Data::setPrefixLength)
-        .def("mask_buf", &Data::mask_buf)
-        .def("setMaskBuf", &Data::setMaskBuf)
-        .def("username", &Data::username)
-        .def("setUsername", &Data::setUsername)
-        .def("password", &Data::password)
-        .def("setPassword", &Data::setPassword)
-        .def("time_offset", &Data::time_offset)
-        .def("setTimeOffset", &Data::setTimeOffset)
-        .def("clear", &Data::clear)
-        .def(py::self == py::self)
-        .def_readwrite("ipAddressChanged", &Data::ipAddressChanged)
-        .def_readwrite("alias", &Data::alias)
-        .def_readwrite("filled", &Data::filled)
-        .def_readwrite("cancelled", &Data::cancelled);
-
-    m.attr("__version__") = "2.0.10";
-}
-
-
+/*******************************************************************************
+* onvif.cpp
+*
+* copyright 2023 Stephen Rhodes
+*
+* This library is free software; you can redistribute it and/or
+* modify it under the terms of the GNU Lesser General Public
+* License as published by the Free Software Foundation; either
+* version 2.1 of the License, or (at your option) any later version.
+*
+* This library is distributed in the hope that it will be useful,
+* but WITHOUT ANY WARRANTY; without even the implied warranty of
+* MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+* Lesser General Public License for more details.
+*
+* You should have received a copy of the GNU Lesser General Public
+* License along with this library; if not, write to the Free Software
+* Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+*
+*******************************************************************************/
+
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include <pybind11/operators.h>
+#include <pybind11/functional.h>
+#include "onvifboss.h"
+
+namespace py = pybind11;
+
+namespace libonvif
+{
+
+PYBIND11_MODULE(libonvif, m)
+{
+    m.doc() = "pybind11 onvif plugin";
+    py::class_<Session>(m, "Session")
+        .def(py::init<>())
+        .def("active_interface", &Session::active_interface)
+        .def("getActiveInterfaces", &Session::getActiveInterfaces);
+    py::class_<Manager>(m, "Manager")
+        .def(py::init<>())
+        .def("startDiscover", &Manager::startDiscover)
+        .def("startFill", &Manager::startFill)
+        .def("startUpdateVideo", &Manager::startUpdateVideo)
+        .def("startUpdateImage", &Manager::startUpdateImage)
+        .def("startUpdateNetwork", &Manager::startUpdateNetwork)
+        .def("startUpdateTime" ,&Manager::startUpdateTime)
+        .def("startReboot", &Manager::startReboot)
+        .def("startReset", &Manager::startReset)
+        .def("startSetUser", &Manager::startSetUser)
+        .def("startSet", &Manager::startSet)
+        .def("startSetGotoPreset", &Manager::startSetGotoPreset)
+        .def("startMove", &Manager::startMove)
+        .def("startStop", &Manager::startStop)
+        .def_readwrite("discovered", &Manager::discovered)
+        .def_readwrite("getCredential", &Manager::getCredential)
+        .def_readwrite("getData", &Manager::getData)
+        .def_readwrite("filled", &Manager::filled)
+        .def_readwrite("preset", &Manager::preset)
+        .def_readwrite("x", &Manager::x)
+        .def_readwrite("y", &Manager::y)
+        .def_readwrite("z", &Manager::z)
+        .def_readwrite("stop_type", &Manager::stop_type)
+        .def_readwrite("new_password", &Manager::new_password)
+        .def_readwrite("interface", &Manager::interface)
+        .def_readwrite("onvif_data", &Manager::onvif_data);
+    py::class_<Data>(m, "Data")
+        .def(py::init<>())
+        .def(py::init<const Data&>())
+        .def("xaddrs", &Data::xaddrs)
+        .def("stream_uri", &Data::stream_uri)
+        .def("serial_number", &Data::serial_number)
+        .def("camera_name", &Data::camera_name)
+        .def("host", &Data::host)
+        .def("last_error", &Data::last_error)
+        .def("clearLastError", &Data::clearLastError)
+        .def("resolutions_buf", &Data::resolutions_buf)
+        .def("width", &Data::width)
+        .def("setWidth", &Data::setWidth)
+        .def("height", &Data::height)
+        .def("setHeight", &Data::setHeight)
+        .def("frame_rate_max", &Data::frame_rate_max)
+        .def("frame_rate_min", &Data::frame_rate_min)
+        .def("frame_rate", &Data::frame_rate)
+        .def("setFrameRate", &Data::setFrameRate)
+        .def("gov_length_max", &Data::gov_length_max)
+        .def("gov_length_min", &Data::gov_length_min)
+        .def("gov_length", &Data::gov_length)
+        .def("setGovLength", &Data::setGovLength)
+        .def("bitrate_max", &Data::bitrate_max)
+        .def("bitrate_min", &Data::bitrate_min)
+        .def("bitrate", &Data::bitrate)
+        .def("setBitrate", &Data::setBitrate)
+        .def("brightness_max", &Data::brightness_max)
+        .def("brightness_min", &Data::brightness_min)
+        .def("brightness", &Data::brightness)
+        .def("setBrightness", &Data::setBrightness)
+        .def("saturation_max", &Data::saturation_max)
+        .def("saturation_min", &Data::saturation_min)
+        .def("saturation", &Data::saturation)
+        .def("setSaturation", &Data::setSaturation)
+        .def("contrast_max", &Data::contrast_max)
+        .def("contrast_min", &Data::contrast_min)
+        .def("contrast", &Data::contrast)
+        .def("setContrast", &Data::setContrast)
+        .def("sharpness_max", &Data::sharpness_max)
+        .def("sharpness_min", &Data::sharpness_min)
+        .def("sharpness", &Data::sharpness)
+        .def("setSharpness", &Data::setSharpness)
+        .def("dhcp_enabled", &Data::dhcp_enabled)
+        .def("setDHCPEnabled", &Data::setDHCPEnabled)
+        .def("ip_address_buf", &Data::ip_address_buf)
+        .def("setIPAddressBuf", &Data::setIPAddressBuf)
+        .def("default_gateway_buf", &Data::default_gateway_buf)
+        .def("setDefaultGatewayBuf", &Data::setDefaultGatewayBuf)
+        .def("dns_buf", &Data::dns_buf)
+        .def("setDNSBuf", &Data::setDNSBuf)
+        .def("prefix_length", &Data::prefix_length)
+        .def("setPrefixLength", &Data::setPrefixLength)
+        .def("mask_buf", &Data::mask_buf)
+        .def("setMaskBuf", &Data::setMaskBuf)
+        .def("username", &Data::username)
+        .def("setUsername", &Data::setUsername)
+        .def("password", &Data::password)
+        .def("setPassword", &Data::setPassword)
+        .def("time_offset", &Data::time_offset)
+        .def("setTimeOffset", &Data::setTimeOffset)
+        .def("clear", &Data::clear)
+        .def(py::self == py::self)
+        .def_readwrite("ipAddressChanged", &Data::ipAddressChanged)
+        .def_readwrite("alias", &Data::alias)
+        .def_readwrite("filled", &Data::filled)
+        .def_readwrite("cancelled", &Data::cancelled);
+
+    m.attr("__version__") = "2.0.9";
+}
+
+
 }
```

### Comparing `libonvif-2.0.10/src/sha1.c` & `libonvif-2.0.9/src/sha1.c`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,321 +1,321 @@
-/*
-SHA-1 in C
-By Steve Reid <steve@edmweb.com>
-100% Public Domain
-
-The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
-hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
-is in the public domain of the country from which the work is published, or (b) hereby dedicates 
-whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
-the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
-associated work, and for these purposes, is described as a "dedicator" below.
-
-A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
-recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
-is not in the public domain.
-
-Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
-Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
-in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
-Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
-rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
-
-Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
-transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
-non-commercial, and in any way, including by methods that have not yet been invented or conceived.
-
-CC0 for Public Domain Dedication
-This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
-to the public domain, we recommend CC0.
-
-Test Vectors (from FIPS PUB 180-1)
-"abc"
-  A9993E36 4706816A BA3E2571 7850C26C 9CD0D89D
-"abcdbcdecdefdefgefghfghighijhijkijkljklmklmnlmnomnopnopq"
-  84983E44 1C3BD26E BAAE4AA1 F95129E5 E54670F1
-A million repetitions of "a"
-  34AA973C D4C4DAA4 F61EEB2B DBAD2731 6534016F
-*/
-
-/* #define LITTLE_ENDIAN * This should be #define'd already, if true. */
-/* #define SHA1HANDSOFF * Copies data before messing with it. */
-
-#define SHA1HANDSOFF
-
-#include <stdio.h>
-#include <string.h>
-
-/* for uint32_t */
-#include <stdint.h>
-
-#include "sha1.h"
-
-
-#define rol(value, bits) (((value) << (bits)) | ((value) >> (32 - (bits))))
-
-/* blk0() and blk() perform the initial expand. */
-/* I got the idea of expanding during the round function from SSLeay */
-#if BYTE_ORDER == LITTLE_ENDIAN
-#define blk0(i) (block->l[i] = (rol(block->l[i],24)&0xFF00FF00) \
-    |(rol(block->l[i],8)&0x00FF00FF))
-#elif BYTE_ORDER == BIG_ENDIAN
-#define blk0(i) block->l[i]
-#else
-#error "Endianness not defined!"
-#endif
-#define blk(i) (block->l[i&15] = rol(block->l[(i+13)&15]^block->l[(i+8)&15] \
-    ^block->l[(i+2)&15]^block->l[i&15],1))
-
-/* (R0+R1), R2, R3, R4 are the different operations used in SHA1 */
-#define R0(v,w,x,y,z,i) z+=((w&(x^y))^y)+blk0(i)+0x5A827999+rol(v,5);w=rol(w,30);
-#define R1(v,w,x,y,z,i) z+=((w&(x^y))^y)+blk(i)+0x5A827999+rol(v,5);w=rol(w,30);
-#define R2(v,w,x,y,z,i) z+=(w^x^y)+blk(i)+0x6ED9EBA1+rol(v,5);w=rol(w,30);
-#define R3(v,w,x,y,z,i) z+=(((w|x)&y)|(w&x))+blk(i)+0x8F1BBCDC+rol(v,5);w=rol(w,30);
-#define R4(v,w,x,y,z,i) z+=(w^x^y)+blk(i)+0xCA62C1D6+rol(v,5);w=rol(w,30);
-
-
-/* Hash a single 512-bit block. This is the core of the algorithm. */
-
-void SHA1Transform(
-    uint32_t state[5],
-    const unsigned char buffer[64]
-)
-{
-    uint32_t a, b, c, d, e;
-
-    typedef union
-    {
-        unsigned char c[64];
-        uint32_t l[16];
-    } CHAR64LONG16;
-
-#ifdef SHA1HANDSOFF
-    CHAR64LONG16 block[1];      /* use array to appear as a pointer */
-
-    memcpy(block, buffer, 64);
-#else
-    /* The following had better never be used because it causes the
-     * pointer-to-const buffer to be cast into a pointer to non-const.
-     * And the result is written through.  I threw a "const" in, hoping
-     * this will cause a diagnostic.
-     */
-    CHAR64LONG16 *block = (const CHAR64LONG16 *) buffer;
-#endif
-    /* Copy context->state[] to working vars */
-    a = state[0];
-    b = state[1];
-    c = state[2];
-    d = state[3];
-    e = state[4];
-    /* 4 rounds of 20 operations each. Loop unrolled. */
-    R0(a, b, c, d, e, 0);
-    R0(e, a, b, c, d, 1);
-    R0(d, e, a, b, c, 2);
-    R0(c, d, e, a, b, 3);
-    R0(b, c, d, e, a, 4);
-    R0(a, b, c, d, e, 5);
-    R0(e, a, b, c, d, 6);
-    R0(d, e, a, b, c, 7);
-    R0(c, d, e, a, b, 8);
-    R0(b, c, d, e, a, 9);
-    R0(a, b, c, d, e, 10);
-    R0(e, a, b, c, d, 11);
-    R0(d, e, a, b, c, 12);
-    R0(c, d, e, a, b, 13);
-    R0(b, c, d, e, a, 14);
-    R0(a, b, c, d, e, 15);
-    R1(e, a, b, c, d, 16);
-    R1(d, e, a, b, c, 17);
-    R1(c, d, e, a, b, 18);
-    R1(b, c, d, e, a, 19);
-    R2(a, b, c, d, e, 20);
-    R2(e, a, b, c, d, 21);
-    R2(d, e, a, b, c, 22);
-    R2(c, d, e, a, b, 23);
-    R2(b, c, d, e, a, 24);
-    R2(a, b, c, d, e, 25);
-    R2(e, a, b, c, d, 26);
-    R2(d, e, a, b, c, 27);
-    R2(c, d, e, a, b, 28);
-    R2(b, c, d, e, a, 29);
-    R2(a, b, c, d, e, 30);
-    R2(e, a, b, c, d, 31);
-    R2(d, e, a, b, c, 32);
-    R2(c, d, e, a, b, 33);
-    R2(b, c, d, e, a, 34);
-    R2(a, b, c, d, e, 35);
-    R2(e, a, b, c, d, 36);
-    R2(d, e, a, b, c, 37);
-    R2(c, d, e, a, b, 38);
-    R2(b, c, d, e, a, 39);
-    R3(a, b, c, d, e, 40);
-    R3(e, a, b, c, d, 41);
-    R3(d, e, a, b, c, 42);
-    R3(c, d, e, a, b, 43);
-    R3(b, c, d, e, a, 44);
-    R3(a, b, c, d, e, 45);
-    R3(e, a, b, c, d, 46);
-    R3(d, e, a, b, c, 47);
-    R3(c, d, e, a, b, 48);
-    R3(b, c, d, e, a, 49);
-    R3(a, b, c, d, e, 50);
-    R3(e, a, b, c, d, 51);
-    R3(d, e, a, b, c, 52);
-    R3(c, d, e, a, b, 53);
-    R3(b, c, d, e, a, 54);
-    R3(a, b, c, d, e, 55);
-    R3(e, a, b, c, d, 56);
-    R3(d, e, a, b, c, 57);
-    R3(c, d, e, a, b, 58);
-    R3(b, c, d, e, a, 59);
-    R4(a, b, c, d, e, 60);
-    R4(e, a, b, c, d, 61);
-    R4(d, e, a, b, c, 62);
-    R4(c, d, e, a, b, 63);
-    R4(b, c, d, e, a, 64);
-    R4(a, b, c, d, e, 65);
-    R4(e, a, b, c, d, 66);
-    R4(d, e, a, b, c, 67);
-    R4(c, d, e, a, b, 68);
-    R4(b, c, d, e, a, 69);
-    R4(a, b, c, d, e, 70);
-    R4(e, a, b, c, d, 71);
-    R4(d, e, a, b, c, 72);
-    R4(c, d, e, a, b, 73);
-    R4(b, c, d, e, a, 74);
-    R4(a, b, c, d, e, 75);
-    R4(e, a, b, c, d, 76);
-    R4(d, e, a, b, c, 77);
-    R4(c, d, e, a, b, 78);
-    R4(b, c, d, e, a, 79);
-    /* Add the working vars back into context.state[] */
-    state[0] += a;
-    state[1] += b;
-    state[2] += c;
-    state[3] += d;
-    state[4] += e;
-    /* Wipe variables */
-    a = b = c = d = e = 0;
-#ifdef SHA1HANDSOFF
-    memset(block, '\0', sizeof(block));
-#endif
-}
-
-
-/* SHA1Init - Initialize new context */
-
-void SHA1Init(
-    SHA1_CTX * context
-)
-{
-    /* SHA1 initialization constants */
-    context->state[0] = 0x67452301;
-    context->state[1] = 0xEFCDAB89;
-    context->state[2] = 0x98BADCFE;
-    context->state[3] = 0x10325476;
-    context->state[4] = 0xC3D2E1F0;
-    context->count[0] = context->count[1] = 0;
-}
-
-
-/* Run your data through this. */
-
-void SHA1Update(
-    SHA1_CTX * context,
-    const unsigned char *data,
-    uint32_t len
-)
-{
-    uint32_t i;
-
-    uint32_t j;
-
-    j = context->count[0];
-    if ((context->count[0] += len << 3) < j)
-        context->count[1]++;
-    context->count[1] += (len >> 29);
-    j = (j >> 3) & 63;
-    if ((j + len) > 63)
-    {
-        memcpy(&context->buffer[j], data, (i = 64 - j));
-        SHA1Transform(context->state, context->buffer);
-        for (; i + 63 < len; i += 64)
-        {
-            SHA1Transform(context->state, &data[i]);
-        }
-        j = 0;
-    }
-    else
-        i = 0;
-    memcpy(&context->buffer[j], &data[i], len - i);
-}
-
-
-/* Add padding and return the message digest. */
-
-void SHA1Final(
-    unsigned char digest[20],
-    SHA1_CTX * context
-)
-{
-    unsigned i;
-
-    unsigned char finalcount[8];
-
-    unsigned char c;
-
-#if 0    /* untested "improvement" by DHR */
-    /* Convert context->count to a sequence of bytes
-     * in finalcount.  Second element first, but
-     * big-endian order within element.
-     * But we do it all backwards.
-     */
-    unsigned char *fcp = &finalcount[8];
-
-    for (i = 0; i < 2; i++)
-    {
-        uint32_t t = context->count[i];
-
-        int j;
-
-        for (j = 0; j < 4; t >>= 8, j++)
-            *--fcp = (unsigned char) t}
-#else
-    for (i = 0; i < 8; i++)
-    {
-        finalcount[i] = (unsigned char) ((context->count[(i >= 4 ? 0 : 1)] >> ((3 - (i & 3)) * 8)) & 255);      /* Endian independent */
-    }
-#endif
-    c = 0200;
-    SHA1Update(context, &c, 1);
-    while ((context->count[0] & 504) != 448)
-    {
-        c = 0000;
-        SHA1Update(context, &c, 1);
-    }
-    SHA1Update(context, finalcount, 8); /* Should cause a SHA1Transform() */
-    for (i = 0; i < 20; i++)
-    {
-        digest[i] = (unsigned char)
-            ((context->state[i >> 2] >> ((3 - (i & 3)) * 8)) & 255);
-    }
-    /* Wipe variables */
-    memset(context, '\0', sizeof(*context));
-    memset(&finalcount, '\0', sizeof(finalcount));
-}
-
-void SHA1(
-    char *hash_out,
-    const char *str,
-    int len)
-{
-    SHA1_CTX ctx;
-    unsigned int ii;
-
-    SHA1Init(&ctx);
-    for (ii=0; ii<len; ii+=1)
-        SHA1Update(&ctx, (const unsigned char*)str + ii, 1);
-    SHA1Final((unsigned char *)hash_out, &ctx);
-    hash_out[20] = '\0';
-}
-
+/*
+SHA-1 in C
+By Steve Reid <steve@edmweb.com>
+100% Public Domain
+
+The person or persons who have associated work with this document (the "Dedicator" or "Certifier") 
+hereby either (a) certifies that, to the best of his knowledge, the work of authorship identified 
+is in the public domain of the country from which the work is published, or (b) hereby dedicates 
+whatever copyright the dedicators holds in the work of authorship identified below (the "Work") to 
+the public domain. A certifier, moreover, dedicates any copyright interest he may have in the 
+associated work, and for these purposes, is described as a "dedicator" below.
+
+A certifier has taken reasonable steps to verify the copyright status of this work. Certifier 
+recognizes that his good faith efforts may not shield him from liability if in fact the work certified 
+is not in the public domain.
+
+Dedicator makes this dedication for the benefit of the public at large and to the detriment of the 
+Dedicator's heirs and successors. Dedicator intends this dedication to be an overt act of relinquishment 
+in perpetuity of all present and future rights under copyright law, whether vested or contingent, in the 
+Work. Dedicator understands that such relinquishment of all rights includes the relinquishment of all 
+rights to enforce (by lawsuit or otherwise) those copyrights in the Work.
+
+Dedicator recognizes that, once placed in the public domain, the Work may be freely reproduced, distributed, 
+transmitted, used, modified, built upon, or otherwise exploited by anyone for any purpose, commercial or 
+non-commercial, and in any way, including by methods that have not yet been invented or conceived.
+
+CC0 for Public Domain Dedication
+This tool is based on United States law and may not be applicable outside the US. For dedicating new works 
+to the public domain, we recommend CC0.
+
+Test Vectors (from FIPS PUB 180-1)
+"abc"
+  A9993E36 4706816A BA3E2571 7850C26C 9CD0D89D
+"abcdbcdecdefdefgefghfghighijhijkijkljklmklmnlmnomnopnopq"
+  84983E44 1C3BD26E BAAE4AA1 F95129E5 E54670F1
+A million repetitions of "a"
+  34AA973C D4C4DAA4 F61EEB2B DBAD2731 6534016F
+*/
+
+/* #define LITTLE_ENDIAN * This should be #define'd already, if true. */
+/* #define SHA1HANDSOFF * Copies data before messing with it. */
+
+#define SHA1HANDSOFF
+
+#include <stdio.h>
+#include <string.h>
+
+/* for uint32_t */
+#include <stdint.h>
+
+#include "sha1.h"
+
+
+#define rol(value, bits) (((value) << (bits)) | ((value) >> (32 - (bits))))
+
+/* blk0() and blk() perform the initial expand. */
+/* I got the idea of expanding during the round function from SSLeay */
+#if BYTE_ORDER == LITTLE_ENDIAN
+#define blk0(i) (block->l[i] = (rol(block->l[i],24)&0xFF00FF00) \
+    |(rol(block->l[i],8)&0x00FF00FF))
+#elif BYTE_ORDER == BIG_ENDIAN
+#define blk0(i) block->l[i]
+#else
+#error "Endianness not defined!"
+#endif
+#define blk(i) (block->l[i&15] = rol(block->l[(i+13)&15]^block->l[(i+8)&15] \
+    ^block->l[(i+2)&15]^block->l[i&15],1))
+
+/* (R0+R1), R2, R3, R4 are the different operations used in SHA1 */
+#define R0(v,w,x,y,z,i) z+=((w&(x^y))^y)+blk0(i)+0x5A827999+rol(v,5);w=rol(w,30);
+#define R1(v,w,x,y,z,i) z+=((w&(x^y))^y)+blk(i)+0x5A827999+rol(v,5);w=rol(w,30);
+#define R2(v,w,x,y,z,i) z+=(w^x^y)+blk(i)+0x6ED9EBA1+rol(v,5);w=rol(w,30);
+#define R3(v,w,x,y,z,i) z+=(((w|x)&y)|(w&x))+blk(i)+0x8F1BBCDC+rol(v,5);w=rol(w,30);
+#define R4(v,w,x,y,z,i) z+=(w^x^y)+blk(i)+0xCA62C1D6+rol(v,5);w=rol(w,30);
+
+
+/* Hash a single 512-bit block. This is the core of the algorithm. */
+
+void SHA1Transform(
+    uint32_t state[5],
+    const unsigned char buffer[64]
+)
+{
+    uint32_t a, b, c, d, e;
+
+    typedef union
+    {
+        unsigned char c[64];
+        uint32_t l[16];
+    } CHAR64LONG16;
+
+#ifdef SHA1HANDSOFF
+    CHAR64LONG16 block[1];      /* use array to appear as a pointer */
+
+    memcpy(block, buffer, 64);
+#else
+    /* The following had better never be used because it causes the
+     * pointer-to-const buffer to be cast into a pointer to non-const.
+     * And the result is written through.  I threw a "const" in, hoping
+     * this will cause a diagnostic.
+     */
+    CHAR64LONG16 *block = (const CHAR64LONG16 *) buffer;
+#endif
+    /* Copy context->state[] to working vars */
+    a = state[0];
+    b = state[1];
+    c = state[2];
+    d = state[3];
+    e = state[4];
+    /* 4 rounds of 20 operations each. Loop unrolled. */
+    R0(a, b, c, d, e, 0);
+    R0(e, a, b, c, d, 1);
+    R0(d, e, a, b, c, 2);
+    R0(c, d, e, a, b, 3);
+    R0(b, c, d, e, a, 4);
+    R0(a, b, c, d, e, 5);
+    R0(e, a, b, c, d, 6);
+    R0(d, e, a, b, c, 7);
+    R0(c, d, e, a, b, 8);
+    R0(b, c, d, e, a, 9);
+    R0(a, b, c, d, e, 10);
+    R0(e, a, b, c, d, 11);
+    R0(d, e, a, b, c, 12);
+    R0(c, d, e, a, b, 13);
+    R0(b, c, d, e, a, 14);
+    R0(a, b, c, d, e, 15);
+    R1(e, a, b, c, d, 16);
+    R1(d, e, a, b, c, 17);
+    R1(c, d, e, a, b, 18);
+    R1(b, c, d, e, a, 19);
+    R2(a, b, c, d, e, 20);
+    R2(e, a, b, c, d, 21);
+    R2(d, e, a, b, c, 22);
+    R2(c, d, e, a, b, 23);
+    R2(b, c, d, e, a, 24);
+    R2(a, b, c, d, e, 25);
+    R2(e, a, b, c, d, 26);
+    R2(d, e, a, b, c, 27);
+    R2(c, d, e, a, b, 28);
+    R2(b, c, d, e, a, 29);
+    R2(a, b, c, d, e, 30);
+    R2(e, a, b, c, d, 31);
+    R2(d, e, a, b, c, 32);
+    R2(c, d, e, a, b, 33);
+    R2(b, c, d, e, a, 34);
+    R2(a, b, c, d, e, 35);
+    R2(e, a, b, c, d, 36);
+    R2(d, e, a, b, c, 37);
+    R2(c, d, e, a, b, 38);
+    R2(b, c, d, e, a, 39);
+    R3(a, b, c, d, e, 40);
+    R3(e, a, b, c, d, 41);
+    R3(d, e, a, b, c, 42);
+    R3(c, d, e, a, b, 43);
+    R3(b, c, d, e, a, 44);
+    R3(a, b, c, d, e, 45);
+    R3(e, a, b, c, d, 46);
+    R3(d, e, a, b, c, 47);
+    R3(c, d, e, a, b, 48);
+    R3(b, c, d, e, a, 49);
+    R3(a, b, c, d, e, 50);
+    R3(e, a, b, c, d, 51);
+    R3(d, e, a, b, c, 52);
+    R3(c, d, e, a, b, 53);
+    R3(b, c, d, e, a, 54);
+    R3(a, b, c, d, e, 55);
+    R3(e, a, b, c, d, 56);
+    R3(d, e, a, b, c, 57);
+    R3(c, d, e, a, b, 58);
+    R3(b, c, d, e, a, 59);
+    R4(a, b, c, d, e, 60);
+    R4(e, a, b, c, d, 61);
+    R4(d, e, a, b, c, 62);
+    R4(c, d, e, a, b, 63);
+    R4(b, c, d, e, a, 64);
+    R4(a, b, c, d, e, 65);
+    R4(e, a, b, c, d, 66);
+    R4(d, e, a, b, c, 67);
+    R4(c, d, e, a, b, 68);
+    R4(b, c, d, e, a, 69);
+    R4(a, b, c, d, e, 70);
+    R4(e, a, b, c, d, 71);
+    R4(d, e, a, b, c, 72);
+    R4(c, d, e, a, b, 73);
+    R4(b, c, d, e, a, 74);
+    R4(a, b, c, d, e, 75);
+    R4(e, a, b, c, d, 76);
+    R4(d, e, a, b, c, 77);
+    R4(c, d, e, a, b, 78);
+    R4(b, c, d, e, a, 79);
+    /* Add the working vars back into context.state[] */
+    state[0] += a;
+    state[1] += b;
+    state[2] += c;
+    state[3] += d;
+    state[4] += e;
+    /* Wipe variables */
+    a = b = c = d = e = 0;
+#ifdef SHA1HANDSOFF
+    memset(block, '\0', sizeof(block));
+#endif
+}
+
+
+/* SHA1Init - Initialize new context */
+
+void SHA1Init(
+    SHA1_CTX * context
+)
+{
+    /* SHA1 initialization constants */
+    context->state[0] = 0x67452301;
+    context->state[1] = 0xEFCDAB89;
+    context->state[2] = 0x98BADCFE;
+    context->state[3] = 0x10325476;
+    context->state[4] = 0xC3D2E1F0;
+    context->count[0] = context->count[1] = 0;
+}
+
+
+/* Run your data through this. */
+
+void SHA1Update(
+    SHA1_CTX * context,
+    const unsigned char *data,
+    uint32_t len
+)
+{
+    uint32_t i;
+
+    uint32_t j;
+
+    j = context->count[0];
+    if ((context->count[0] += len << 3) < j)
+        context->count[1]++;
+    context->count[1] += (len >> 29);
+    j = (j >> 3) & 63;
+    if ((j + len) > 63)
+    {
+        memcpy(&context->buffer[j], data, (i = 64 - j));
+        SHA1Transform(context->state, context->buffer);
+        for (; i + 63 < len; i += 64)
+        {
+            SHA1Transform(context->state, &data[i]);
+        }
+        j = 0;
+    }
+    else
+        i = 0;
+    memcpy(&context->buffer[j], &data[i], len - i);
+}
+
+
+/* Add padding and return the message digest. */
+
+void SHA1Final(
+    unsigned char digest[20],
+    SHA1_CTX * context
+)
+{
+    unsigned i;
+
+    unsigned char finalcount[8];
+
+    unsigned char c;
+
+#if 0    /* untested "improvement" by DHR */
+    /* Convert context->count to a sequence of bytes
+     * in finalcount.  Second element first, but
+     * big-endian order within element.
+     * But we do it all backwards.
+     */
+    unsigned char *fcp = &finalcount[8];
+
+    for (i = 0; i < 2; i++)
+    {
+        uint32_t t = context->count[i];
+
+        int j;
+
+        for (j = 0; j < 4; t >>= 8, j++)
+            *--fcp = (unsigned char) t}
+#else
+    for (i = 0; i < 8; i++)
+    {
+        finalcount[i] = (unsigned char) ((context->count[(i >= 4 ? 0 : 1)] >> ((3 - (i & 3)) * 8)) & 255);      /* Endian independent */
+    }
+#endif
+    c = 0200;
+    SHA1Update(context, &c, 1);
+    while ((context->count[0] & 504) != 448)
+    {
+        c = 0000;
+        SHA1Update(context, &c, 1);
+    }
+    SHA1Update(context, finalcount, 8); /* Should cause a SHA1Transform() */
+    for (i = 0; i < 20; i++)
+    {
+        digest[i] = (unsigned char)
+            ((context->state[i >> 2] >> ((3 - (i & 3)) * 8)) & 255);
+    }
+    /* Wipe variables */
+    memset(context, '\0', sizeof(*context));
+    memset(&finalcount, '\0', sizeof(finalcount));
+}
+
+void SHA1(
+    char *hash_out,
+    const char *str,
+    int len)
+{
+    SHA1_CTX ctx;
+    unsigned int ii;
+
+    SHA1Init(&ctx);
+    for (ii=0; ii<len; ii+=1)
+        SHA1Update(&ctx, (const unsigned char*)str + ii, 1);
+    SHA1Final((unsigned char *)hash_out, &ctx);
+    hash_out[20] = '\0';
+}
+
```

