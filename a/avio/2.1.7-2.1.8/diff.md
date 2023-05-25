# Comparing `tmp/avio-2.1.7.tar.gz` & `tmp/avio-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avio-2.1.7.tar", last modified: Thu May 18 20:21:44 2023, max compression
+gzip compressed data, was "avio-2.1.8.tar", last modified: Thu May 25 17:35:01 2023, max compression
```

## Comparing `avio-2.1.7.tar` & `avio-2.1.8.tar`

### file list

```diff
@@ -1,324 +1,326 @@
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.185180 avio-2.1.7/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2798 2023-05-05 16:51:23.000000 avio-2.1.7/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11357 2023-05-05 16:51:23.000000 avio-2.1.7/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      147 2023-05-05 16:51:23.000000 avio-2.1.7/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1869 2023-05-18 20:21:44.185180 avio-2.1.7/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1325 2023-05-05 16:51:23.000000 avio-2.1.7/README.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.161180 avio-2.1.7/cmake/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3496 2023-05-05 16:51:23.000000 avio-2.1.7/cmake/FindFFmpeg.cmake
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.161180 avio-2.1.7/include/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1251 2023-05-05 16:51:23.000000 avio-2.1.7/include/Clock.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2559 2023-05-05 16:51:23.000000 avio-2.1.7/include/Decoder.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3142 2023-05-05 16:51:23.000000 avio-2.1.7/include/Display.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2290 2023-05-05 16:51:23.000000 avio-2.1.7/include/Encoder.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2402 2023-05-05 16:51:23.000000 avio-2.1.7/include/Exception.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2719 2023-05-05 16:51:23.000000 avio-2.1.7/include/Filter.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1968 2023-05-05 16:51:23.000000 avio-2.1.7/include/Frame.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1249 2023-05-05 16:51:23.000000 avio-2.1.7/include/Packet.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1941 2023-05-05 16:51:23.000000 avio-2.1.7/include/Pipe.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4179 2023-05-18 17:29:58.000000 avio-2.1.7/include/Player.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5327 2023-05-05 16:51:23.000000 avio-2.1.7/include/Queue.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3071 2023-05-05 16:51:23.000000 avio-2.1.7/include/Reader.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1977 2023-05-05 16:51:23.000000 avio-2.1.7/include/Writer.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6747 2023-05-05 16:51:23.000000 avio-2.1.7/include/avio.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.161180 avio-2.1.7/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1271 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.appveyor.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      996 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.clang-format
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2605 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.clang-tidy
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2196 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.cmake-format.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1308 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.codespell-ignore-lines
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.git
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       18 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.gitattributes
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/.github/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/CODEOWNERS
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15284 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/CONTRIBUTING.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2561 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      328 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/dependabot.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      116 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       50 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/labeler_merged.yml
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/.github/matchers/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      668 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/matchers/pylint.json
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/pull_request_template.md
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/.github/workflows/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    32023 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/ci.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2127 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/configure.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1460 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/format.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      559 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/labeler.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2558 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/pip.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2865 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.github/workflows/upstream.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      502 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.gitignore
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4332 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       62 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/.readthedocs.yml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11983 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1684 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/LICENSE
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      223 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/MANIFEST.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7686 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/README.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/docs/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      607 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/Doxyfile
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7417 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/Makefile
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.157180 avio-2.1.7/pybind11/docs/_static/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/docs/_static/css/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/_static/css/custom.css
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.165180 avio-2.1.7/pybind11/docs/advanced/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/docs/advanced/cast/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3937 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/chrono.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3429 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/custom.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/eigen.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3889 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/functional.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1556 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12371 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/overview.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9586 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/stl.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8863 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/cast/strings.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    47796 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/classes.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8453 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/embedding.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17796 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/exceptions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26729 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/functions.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15651 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/misc.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/docs/advanced/pycpp/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      278 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/pycpp/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17161 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/pycpp/numpy.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/pycpp/object.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/pycpp/utilities.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6377 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/advanced/smart_ptrs.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9240 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/basics.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2856 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/benchmark.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/benchmark.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   114174 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/changelog.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16380 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/classes.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/docs/cmake/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      273 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/cmake/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    25777 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/compiling.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11559 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/conf.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13177 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/faq.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      613 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/index.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3277 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/installing.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3079 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/limitations.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    61034 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/pybind11-logo.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    44653 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/pybind11_vs_boost_python1.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    87708 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    41121 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/pybind11_vs_boost_python2.png
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    85853 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2647 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/reference.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4414 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/release.rst
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23489 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/docs/upgrade.rst
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.157180 avio-2.1.7/pybind11/include/
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/include/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23959 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/attr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7069 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/buffer_info.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    65660 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/cast.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8458 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/chrono.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      120 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2096 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/complex.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/include/pybind11/detail/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28251 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/class.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    52866 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/common.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5491 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/descr.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17869 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/init.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    26498 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/internals.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    42613 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/type_caster_base.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1625 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/detail/typeid.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/include/pybind11/eigen/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    31418 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/eigen/matrix.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18108 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/eigen/tensor.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/eigen.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13471 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/embed.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4731 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/eval.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5002 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/functional.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8262 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/gil.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8862 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/iostream.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    79408 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/numpy.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9103 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/operators.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2734 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/options.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)   126420 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/pybind11.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    94641 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/pytypes.h
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.169180 avio-2.1.7/pybind11/include/pybind11/stl/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4185 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/stl/filesystem.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    15399 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/stl.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    29824 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/include/pybind11/stl_bind.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2765 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/noxfile.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.173180 avio-2.1.7/pybind11/pybind11/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      414 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/__init__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/__main__.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      233 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/_version.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/commands.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/py.typed
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17609 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pybind11/setup_helpers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1261 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1618 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4877 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21675 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5876 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/conftest.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11736 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/constructor_stats.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3578 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/cross_module_gil_utils.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1776 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      396 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      940 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/env.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/extra_python_package/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/extra_python_package/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8296 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/extra_python_package/test_files.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/extra_setuptools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/extra_setuptools/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4153 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2847 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/local_bindings.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/object.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4517 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/pybind11_tests.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2685 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/pybind11_tests.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/pytest.ini
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      600 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/requirements.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      855 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_async.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      534 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_async.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8567 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_buffers.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4841 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_buffers.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16025 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_builtin_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    17245 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_builtin_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4118 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_call_policies.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6549 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_call_policies.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10858 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_callbacks.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6246 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_callbacks.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3370 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_chrono.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5695 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_chrono.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    24874 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_class.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14815 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_class.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2639 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/embed.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/installed_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1171 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/installed_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1293 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/installed_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      152 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/main.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1353 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1163 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1368 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      198 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_cmake_build/test.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3831 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_const_name.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      589 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_const_name.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5615 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_constants_and_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1498 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_constants_and_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10886 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_copy_move.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_copy_move.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7280 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_custom_type_casters.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3980 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_custom_type_casters.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1259 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_custom_type_setup.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1089 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_custom_type_setup.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4557 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_docstring_options.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2423 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_docstring_options.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19350 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eigen_matrix.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    28867 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eigen_matrix.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      473 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eigen_tensor.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10590 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eigen_tensor.inl
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9456 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eigen_tensor.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tests/test_embed/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1798 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/CMakeLists.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1315 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/catch.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      543 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/external_module.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16535 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/test_interpreter.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      237 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/test_interpreter.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      275 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_embed/test_trampoline.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5722 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_enum.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8903 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_enum.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eval.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1143 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eval.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      119 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_eval_call.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11904 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_exceptions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      399 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_exceptions.h
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12774 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_exceptions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18155 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_factory_constructors.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    16519 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_factory_constructors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5311 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_gil_scoped.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8540 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_gil_scoped.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3960 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_iostream.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7286 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_iostream.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9444 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    13757 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_kwargs_and_defaults.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4401 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_local_bindings.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8049 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_local_bindings.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21388 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_methods_and_attributes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18134 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_methods_and_attributes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4121 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_modules.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4191 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_modules.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12305 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_multiple_inheritance.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11874 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_multiple_inheritance.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    19861 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_array.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20356 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_array.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21114 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_dtypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14394 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_dtypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4487 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_vectorize.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9686 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_numpy_vectorize.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2777 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_opaque_types.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1847 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_opaque_types.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9132 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_operator_overloading.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4333 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_operator_overloading.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6719 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_pickling.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2720 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_pickling.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    30750 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_pytypes.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    23630 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_pytypes.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21153 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_sequences_and_iterators.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8021 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_sequences_and_iterators.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    18898 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_smart_ptr.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9530 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_smart_ptr.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    21587 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_stl.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12235 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_stl.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4622 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_stl_binders.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9174 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_stl_binders.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     4617 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      741 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_tagbased_polymorphic.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1855 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_thread.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      826 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_thread.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      603 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_union.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      148 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_union.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    22991 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_virtual_functions.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12919 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/test_virtual_functions.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3226 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/valgrind-numpy-scipy.supp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2657 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tests/valgrind-python.supp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.181180 avio-2.1.7/pybind11/tools/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2350 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/FindCatch.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3105 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/FindEigen3.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11190 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/FindPythonLibsNew.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      817 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/JoinPaths.cmake
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1423 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/check-style.sh
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      952 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/cmake_uninstall.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1040 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1031 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/libsize.py
--rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1311 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/make_changelog.py
--rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pybind11.pc.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    14033 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pybind11Common.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6930 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pybind11Config.cmake.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8960 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pybind11NewTools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8361 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pybind11Tools.cmake
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       94 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2104 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/setup_global.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1234 2023-05-05 16:51:26.000000 avio-2.1.7/pybind11/tools/setup_main.py.in
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1351 2023-05-18 20:21:36.000000 avio-2.1.7/pyproject.toml
--rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-18 20:21:44.185180 avio-2.1.7/setup.cfg
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3072 2023-05-18 20:21:30.000000 avio-2.1.7/setup.py
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.185180 avio-2.1.7/src/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2189 2023-05-05 16:51:23.000000 avio-2.1.7/src/Clock.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     8368 2023-05-05 16:51:23.000000 avio-2.1.7/src/Decoder.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    20694 2023-05-18 17:29:58.000000 avio-2.1.7/src/Display.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11378 2023-05-05 16:51:23.000000 avio-2.1.7/src/Encoder.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6430 2023-05-05 16:51:23.000000 avio-2.1.7/src/Exception.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     7061 2023-05-05 16:51:23.000000 avio-2.1.7/src/Filter.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     6318 2023-05-05 16:51:23.000000 avio-2.1.7/src/Frame.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     2296 2023-05-05 16:51:23.000000 avio-2.1.7/src/Packet.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     5126 2023-05-05 16:51:23.000000 avio-2.1.7/src/Pipe.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    11632 2023-05-05 16:51:23.000000 avio-2.1.7/src/Player.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    12986 2023-05-05 16:51:23.000000 avio-2.1.7/src/Reader.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     3739 2023-05-05 16:51:23.000000 avio-2.1.7/src/Writer.cpp
--rw-rw-r--   0 stephen   (1000) stephen   (1000)    10459 2023-05-18 20:21:25.000000 avio-2.1.7/src/avio.cpp
-drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-18 20:21:44.185180 avio-2.1.7/src/avio.egg-info/
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     1869 2023-05-18 20:21:44.000000 avio-2.1.7/src/avio.egg-info/PKG-INFO
--rw-rw-r--   0 stephen   (1000) stephen   (1000)     9620 2023-05-18 20:21:44.000000 avio-2.1.7/src/avio.egg-info/SOURCES.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-18 20:21:44.000000 avio-2.1.7/src/avio.egg-info/dependency_links.txt
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-18 17:30:13.000000 avio-2.1.7/src/avio.egg-info/not-zip-safe
--rw-rw-r--   0 stephen   (1000) stephen   (1000)        5 2023-05-18 20:21:44.000000 avio-2.1.7/src/avio.egg-info/top_level.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.763257 avio-2.1.8/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2873 2023-05-25 17:26:47.000000 avio-2.1.8/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11558 2023-05-25 17:26:47.000000 avio-2.1.8/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      151 2023-05-25 17:26:47.000000 avio-2.1.8/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1869 2023-05-25 17:35:01.763257 avio-2.1.8/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1374 2023-05-25 17:26:47.000000 avio-2.1.8/README.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/avio/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      564 2023-05-25 17:26:47.000000 avio-2.1.8/avio/__init__.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/avio.egg-info/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1869 2023-05-25 17:35:01.000000 avio-2.1.8/avio.egg-info/PKG-INFO
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9617 2023-05-25 17:35:01.000000 avio-2.1.8/avio.egg-info/SOURCES.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-25 17:35:01.000000 avio-2.1.8/avio.egg-info/dependency_links.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        1 2023-05-25 17:29:33.000000 avio-2.1.8/avio.egg-info/not-zip-safe
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        5 2023-05-25 17:35:01.000000 avio-2.1.8/avio.egg-info/top_level.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/cmake/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3416 2023-05-25 17:26:47.000000 avio-2.1.8/cmake/FindFFmpeg.cmake
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/include/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1251 2023-05-25 17:26:47.000000 avio-2.1.8/include/Clock.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2559 2023-05-25 17:26:47.000000 avio-2.1.8/include/Decoder.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3142 2023-05-25 17:26:47.000000 avio-2.1.8/include/Display.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2383 2023-05-25 17:26:47.000000 avio-2.1.8/include/Encoder.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2402 2023-05-25 17:26:47.000000 avio-2.1.8/include/Exception.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2719 2023-05-25 17:26:47.000000 avio-2.1.8/include/Filter.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1968 2023-05-25 17:26:47.000000 avio-2.1.8/include/Frame.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1296 2023-05-25 17:26:47.000000 avio-2.1.8/include/Packet.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1941 2023-05-25 17:26:47.000000 avio-2.1.8/include/Pipe.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4334 2023-05-25 17:26:47.000000 avio-2.1.8/include/Player.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5327 2023-05-25 17:26:47.000000 avio-2.1.8/include/Queue.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3071 2023-05-25 17:26:47.000000 avio-2.1.8/include/Reader.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2061 2023-05-25 17:26:47.000000 avio-2.1.8/include/Writer.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6747 2023-05-25 17:26:47.000000 avio-2.1.8/include/avio.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.743257 avio-2.1.8/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1271 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.appveyor.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      996 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.clang-format
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2605 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.clang-tidy
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2196 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1308 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.codespell-ignore-lines
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       52 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.git
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       18 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.gitattributes
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.743257 avio-2.1.8/pybind11/.github/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      182 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/CODEOWNERS
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15284 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/CONTRIBUTING.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.743257 avio-2.1.8/pybind11/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2561 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      328 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      162 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/dependabot.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      116 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/labeler.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       50 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/labeler_merged.yml
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.743257 avio-2.1.8/pybind11/.github/matchers/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      668 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/matchers/pylint.json
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      645 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/pull_request_template.md
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.743257 avio-2.1.8/pybind11/.github/workflows/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    32023 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/ci.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2127 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/configure.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1460 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/format.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      559 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/labeler.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2558 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/pip.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2865 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.github/workflows/upstream.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      502 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.gitignore
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4332 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       62 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/.readthedocs.yml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11983 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1684 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/LICENSE
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      223 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/MANIFEST.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7686 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/README.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      607 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/Doxyfile
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7417 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/Makefile
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/pybind11/docs/_static/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/_static/css/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       37 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/_static/css/custom.css
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/advanced/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/advanced/cast/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3937 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/chrono.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3429 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/custom.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14283 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/eigen.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3889 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/functional.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1556 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12371 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/overview.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9586 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/stl.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8863 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/cast/strings.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    47796 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/classes.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8453 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/embedding.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17796 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/exceptions.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26729 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/functions.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15651 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/misc.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/advanced/pycpp/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      278 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/pycpp/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17161 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9030 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/pycpp/object.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5710 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6377 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/advanced/smart_ptrs.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9240 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/basics.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2856 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/benchmark.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/benchmark.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   114174 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/changelog.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16380 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/classes.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.747257 avio-2.1.8/pybind11/docs/cmake/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      273 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/cmake/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    25777 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/compiling.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11559 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/conf.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13177 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/faq.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      613 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/index.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3277 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/installing.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3079 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/limitations.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    61034 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/pybind11-logo.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    44653 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    87708 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    41121 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    85853 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2647 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/reference.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4414 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/release.rst
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      149 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/requirements.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23489 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/docs/upgrade.rst
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.739257 avio-2.1.8/pybind11/include/
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.751257 avio-2.1.8/pybind11/include/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23959 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/attr.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7069 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/buffer_info.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    65660 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/cast.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8458 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/chrono.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      120 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/common.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2096 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/complex.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.751257 avio-2.1.8/pybind11/include/pybind11/detail/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    28251 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/class.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    52866 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/common.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5491 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/descr.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17869 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/init.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    26498 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/internals.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    42613 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1625 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/detail/typeid.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.751257 avio-2.1.8/pybind11/include/pybind11/eigen/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    31418 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/eigen/matrix.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18108 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/eigen/tensor.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      316 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/eigen.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13471 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/embed.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4731 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/eval.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5002 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/functional.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8262 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/gil.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8862 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/iostream.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    79408 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/numpy.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9103 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/operators.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2734 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/options.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)   126420 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/pybind11.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    94641 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/pytypes.h
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.751257 avio-2.1.8/pybind11/include/pybind11/stl/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4185 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/stl/filesystem.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    15399 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/stl.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    29824 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/include/pybind11/stl_bind.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2765 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/noxfile.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.751257 avio-2.1.8/pybind11/pybind11/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      414 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/__init__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1360 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/__main__.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      233 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/_version.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1226 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/commands.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/py.typed
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17609 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pybind11/setup_helpers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1261 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1618 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4877 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21675 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5876 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/conftest.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11736 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/constructor_stats.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3578 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/cross_module_gil_utils.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1776 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      396 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/eigen_tensor_avoid_stl_array.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      940 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/env.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/extra_python_package/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/extra_python_package/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8296 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/extra_python_package/test_files.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/extra_setuptools/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/extra_setuptools/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4153 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2847 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/local_bindings.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5743 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/object.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6264 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4517 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/pybind11_tests.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2685 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/pybind11_tests.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      768 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/pytest.ini
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      600 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/requirements.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      855 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_async.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      534 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_async.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8567 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_buffers.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4841 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_buffers.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16025 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_builtin_casters.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    17245 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_builtin_casters.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4118 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_call_policies.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6549 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_call_policies.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10858 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_callbacks.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6246 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_callbacks.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3370 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_chrono.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5695 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_chrono.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    24874 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_class.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14815 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_class.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2639 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      673 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/embed.cpp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/installed_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1171 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/installed_function/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1293 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/installed_target/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1685 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      152 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/main.cpp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1353 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1163 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1368 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      198 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_cmake_build/test.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3831 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_const_name.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      589 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_const_name.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5615 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_constants_and_functions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1498 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_constants_and_functions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10886 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_copy_move.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4796 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_copy_move.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7280 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_custom_type_casters.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3980 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_custom_type_casters.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1259 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_custom_type_setup.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1089 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_custom_type_setup.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4557 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_docstring_options.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2423 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_docstring_options.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19350 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eigen_matrix.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    28867 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eigen_matrix.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      473 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eigen_tensor.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10590 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eigen_tensor.inl
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9456 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eigen_tensor.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.759257 avio-2.1.8/pybind11/tests/test_embed/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1798 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/CMakeLists.txt
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1315 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/catch.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      543 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/external_module.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16535 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      237 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/test_interpreter.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      275 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_embed/test_trampoline.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5722 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_enum.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8903 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_enum.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3168 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eval.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1143 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eval.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      119 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_eval_call.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11904 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_exceptions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      399 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_exceptions.h
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12774 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_exceptions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18155 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_factory_constructors.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    16519 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_factory_constructors.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5311 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_gil_scoped.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8540 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_gil_scoped.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3960 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_iostream.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7286 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_iostream.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9444 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    13757 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_kwargs_and_defaults.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4401 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_local_bindings.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8049 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_local_bindings.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21388 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_methods_and_attributes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18134 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_methods_and_attributes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4121 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_modules.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4191 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_modules.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12305 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_multiple_inheritance.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11874 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_multiple_inheritance.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    19861 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_array.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20356 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_array.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21114 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_dtypes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14394 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_dtypes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4487 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_vectorize.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9686 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_numpy_vectorize.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2777 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_opaque_types.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1847 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_opaque_types.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9132 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_operator_overloading.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4333 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_operator_overloading.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6719 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_pickling.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2720 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_pickling.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    30750 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_pytypes.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    23630 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_pytypes.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21153 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8021 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_sequences_and_iterators.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    18898 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_smart_ptr.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9530 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_smart_ptr.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    21587 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_stl.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12235 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_stl.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4622 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_stl_binders.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     9174 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_stl_binders.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     4617 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      741 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_tagbased_polymorphic.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1855 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_thread.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      826 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_thread.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      603 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_union.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      148 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_union.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    22991 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_virtual_functions.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12919 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/test_virtual_functions.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3226 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2657 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tests/valgrind-python.supp
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.763257 avio-2.1.8/pybind11/tools/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2350 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/FindCatch.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3105 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/FindEigen3.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11190 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/FindPythonLibsNew.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      817 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/JoinPaths.cmake
+-rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1423 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/check-style.sh
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      952 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/cmake_uninstall.cmake.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1040 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1031 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/libsize.py
+-rwxrwxr-x   0 stephen   (1000) stephen   (1000)     1311 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/make_changelog.py
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)      196 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pybind11.pc.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    14033 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pybind11Common.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6930 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pybind11Config.cmake.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8960 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pybind11NewTools.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8361 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pybind11Tools.cmake
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       94 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2104 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/setup_global.py.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1234 2023-05-25 17:26:50.000000 avio-2.1.8/pybind11/tools/setup_main.py.in
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     1391 2023-05-25 17:26:47.000000 avio-2.1.8/pyproject.toml
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)       38 2023-05-25 17:35:01.763257 avio-2.1.8/setup.cfg
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2394 2023-05-25 17:26:47.000000 avio-2.1.8/setup.py
+drwxrwxr-x   0 stephen   (1000) stephen   (1000)        0 2023-05-25 17:35:01.763257 avio-2.1.8/src/
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2189 2023-05-25 17:26:47.000000 avio-2.1.8/src/Clock.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     8368 2023-05-25 17:26:47.000000 avio-2.1.8/src/Decoder.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    20694 2023-05-25 17:26:47.000000 avio-2.1.8/src/Display.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11703 2023-05-25 17:26:47.000000 avio-2.1.8/src/Encoder.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6430 2023-05-25 17:26:47.000000 avio-2.1.8/src/Exception.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     7061 2023-05-25 17:26:47.000000 avio-2.1.8/src/Filter.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     6318 2023-05-25 17:26:47.000000 avio-2.1.8/src/Frame.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     2393 2023-05-25 17:26:47.000000 avio-2.1.8/src/Packet.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     5126 2023-05-25 17:26:47.000000 avio-2.1.8/src/Pipe.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    11993 2023-05-25 17:26:47.000000 avio-2.1.8/src/Player.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    12986 2023-05-25 17:26:47.000000 avio-2.1.8/src/Reader.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)     3876 2023-05-25 17:26:47.000000 avio-2.1.8/src/Writer.cpp
+-rw-rw-r--   0 stephen   (1000) stephen   (1000)    10665 2023-05-25 17:26:47.000000 avio-2.1.8/src/avio.cpp
```

### Comparing `avio-2.1.7/CMakeLists.txt` & `avio-2.1.8/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -D__STDC_CONSTANT_MACROS")
 
 list(PREPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake)
 
 if(WIN32)
+    list(PREPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake-win)
     add_compile_options("/EHsc")
     set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS TRUE)
     set(BUILD_SHARED_LIBS TRUE)
 endif()
 
 add_definitions(-w)
```

### Comparing `avio-2.1.7/LICENSE` & `avio-2.1.8/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `avio-2.1.7/PKG-INFO` & `avio-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: avio
-Version: 2.1.7
+Version: 2.1.8
 Summary: A python module for processing media streams
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libavio
 Project-URL: Bug Tracker, https://github.com/sr99622/libavio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # avio
 
 Python library for processing media streams
```

### Comparing `avio-2.1.7/cmake/FindFFmpeg.cmake` & `avio-2.1.8/cmake/FindFFmpeg.cmake`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-#*******************************************************************************
-# FindFFmpeg.cmake
+#/********************************************************************
+# libavio/cmake/FindFFmpeg.cmake
 #
-# Copyright (c) 2022 Stephen Rhodes 
+# Copyright (c) 2022  Stephen Rhodes
 #
-# This program is free software; you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation; either version 2 of the License, or
-# (at your option) any later version.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
-# You should have received a copy of the GNU General Public License along
-# with this program; if not, write to the Free Software Foundation, Inc.,
-# 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #
-#******************************************************************************/
+#*********************************************************************/
 
 macro(find_component_library var library_name)
     find_library(${var} NAME ${library_name}
         HINTS
+            $ENV{FFMPEG_INSTALL_DIR}/lib
             $ENV{CONDA_PREFIX}
     )
 endmacro()
 
 macro(find_component_include_dir var header_name)
     find_path(${var} ${header_name}
         HINTS
+            $ENV{FFMPEG_INSTALL_DIR}/include
             $ENV{CONDA_PREFIX}
     )
 endmacro()
 
 find_package(PkgConfig QUIET)
 if (PKG_CONFIG_FOUND)
     pkg_check_modules(FFMPEG
```

### Comparing `avio-2.1.7/include/Clock.h` & `avio-2.1.8/include/Clock.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Decoder.h` & `avio-2.1.8/include/Decoder.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Display.h` & `avio-2.1.8/include/Display.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Encoder.h` & `avio-2.1.8/include/Encoder.h`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-#ifndef ENCODER_H
-#define ENCODER_H
-
-extern "C" {
-#include <libavutil/avassert.h>
-#include <libavutil/channel_layout.h>
-#include <libavutil/opt.h>
-#include <libavutil/mathematics.h>
-#include <libavutil/timestamp.h>
-#include <libavcodec/avcodec.h>
-#include <libavformat/avformat.h>
-#include <libswscale/swscale.h>
-#include <libswresample/swresample.h>
-}
-
-#include "Exception.h"
-#include "Queue.h"
-#include "Frame.h"
-#include "Packet.h"
-#include "Writer.h"
-
-namespace avio
-{
-
-class Encoder
-{
-public:
-    Encoder(Writer* writer, AVMediaType mediaType);
-    ~Encoder();
-    void openVideoStream();
-    void openAudioStream();
-    void init();
-    int encode(Frame& f);
-    void close();
-    bool cmpFrame(AVFrame* frame);
-    bool opened = false;
-
-    Writer* writer;
-    AVMediaType mediaType;
-    std::string strMediaType;
-
-    AVStream* stream = NULL;
-    AVCodecContext* enc_ctx = NULL;
-    AVPacket* pkt = NULL;
-    SwsContext* sws_ctx = NULL;
-    SwrContext* swr_ctx = NULL;
-    AVFrame* cvt_frame = NULL;
-
-    AVBufferRef* hw_frames_ref = NULL;
-    AVBufferRef* hw_device_ctx = NULL;
-    AVFrame* hw_frame = NULL;
-
-    AVHWDeviceType hw_device_type = AV_HWDEVICE_TYPE_NONE;
-    std::string hw_video_codec_name;
-    std::string profile;
-    AVPixelFormat hw_pix_fmt = AV_PIX_FMT_NONE;
-    AVPixelFormat sw_pix_fmt = AV_PIX_FMT_NONE;
-
-    AVPixelFormat pix_fmt = AV_PIX_FMT_NONE;
-    int width = 0;
-    int height = 0;
-    int video_bit_rate = 0;
-    int gop_size = 0;
-    AVRational frame_rate = av_make_q(0, 0);
-    AVRational video_time_base = av_make_q(0, 0);
-    AVDictionary* opts = NULL;
-
-    AVSampleFormat sample_fmt = AV_SAMPLE_FMT_NONE;
-    uint64_t channel_layout = 0;
-    int audio_bit_rate = 0;
-    int sample_rate = 0;
-    int nb_samples = 0;
-    int channels = 0;
-    AVRational audio_time_base = av_make_q(0, 0);
-    void set_channel_layout_mono() { channel_layout = AV_CH_LAYOUT_MONO; }
-    void set_channel_layout_stereo() { channel_layout = AV_CH_LAYOUT_STEREO; }
-    int64_t total_samples = 0;
-
-    bool show_frames = false;
-
-    int64_t pts_offset = 0;
-    bool first_pass = true;
-
-    Queue<Frame>* frame_q = nullptr;
-
-    int frame_q_max_size = 0;
-
-	std::function<void(const std::string&)> infoCallback = nullptr;
-    ExceptionHandler ex;
-};
-
-}
-
+#ifndef ENCODER_H
+#define ENCODER_H
+
+extern "C" {
+#include <libavutil/avassert.h>
+#include <libavutil/channel_layout.h>
+#include <libavutil/opt.h>
+#include <libavutil/mathematics.h>
+#include <libavutil/timestamp.h>
+#include <libavcodec/avcodec.h>
+#include <libavformat/avformat.h>
+#include <libswscale/swscale.h>
+#include <libswresample/swresample.h>
+}
+
+#include "Exception.h"
+#include "Queue.h"
+#include "Frame.h"
+#include "Packet.h"
+#include "Writer.h"
+
+namespace avio
+{
+
+class Encoder
+{
+public:
+    Encoder(Writer* writer, AVMediaType mediaType);
+    ~Encoder();
+    void openVideoStream();
+    void openAudioStream();
+    void init();
+    int encode(Frame& f);
+    void close();
+    bool cmpFrame(AVFrame* frame);
+    bool opened = false;
+
+    Writer* writer;
+    AVMediaType mediaType;
+    std::string strMediaType;
+
+    AVStream* stream = NULL;
+    AVCodecContext* enc_ctx = NULL;
+    AVPacket* pkt = NULL;
+    SwsContext* sws_ctx = NULL;
+    SwrContext* swr_ctx = NULL;
+    AVFrame* cvt_frame = NULL;
+
+    AVBufferRef* hw_frames_ref = NULL;
+    AVBufferRef* hw_device_ctx = NULL;
+    AVFrame* hw_frame = NULL;
+
+    AVHWDeviceType hw_device_type = AV_HWDEVICE_TYPE_NONE;
+    std::string hw_video_codec_name;
+    std::string profile;
+    AVPixelFormat hw_pix_fmt = AV_PIX_FMT_NONE;
+    AVPixelFormat sw_pix_fmt = AV_PIX_FMT_NONE;
+
+    AVPixelFormat pix_fmt = AV_PIX_FMT_NONE;
+    int width = 0;
+    int height = 0;
+    int video_bit_rate = 0;
+    int gop_size = 0;
+    AVRational frame_rate = av_make_q(0, 0);
+    AVRational video_time_base = av_make_q(0, 0);
+    AVDictionary* opts = NULL;
+
+    AVSampleFormat sample_fmt = AV_SAMPLE_FMT_NONE;
+    uint64_t channel_layout = 0;
+    int audio_bit_rate = 0;
+    int sample_rate = 0;
+    int nb_samples = 0;
+    int channels = 0;
+    AVRational audio_time_base = av_make_q(0, 0);
+    void set_channel_layout_mono() { channel_layout = AV_CH_LAYOUT_MONO; }
+    void set_channel_layout_stereo() { channel_layout = AV_CH_LAYOUT_STEREO; }
+    int64_t total_samples = 0;
+
+    bool show_frames = false;
+
+    int64_t pts_offset = 0;
+    bool first_pass = true;
+
+    Queue<Frame>* frame_q = nullptr;
+
+    int frame_q_max_size = 0;
+
+	std::function<void(const std::string&)> infoCallback = nullptr;
+    ExceptionHandler ex;
+};
+
+}
+
 #endif // ENCODER_H
```

### Comparing `avio-2.1.7/include/Exception.h` & `avio-2.1.8/include/Exception.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Filter.h` & `avio-2.1.8/include/Filter.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Frame.h` & `avio-2.1.8/include/Frame.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Packet.h` & `avio-2.1.8/include/Packet.h`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-/********************************************************************
-* libavio/include/Packet.h
-*
-* Copyright (c) 2022  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#ifndef PACKET_H
-#define PACKET_H
-
-extern "C" {
-#include "libavcodec/avcodec.h"
-}
-
-namespace avio
-{
-
-class Packet
-{
-public:
-    Packet();
-    ~Packet();
-    Packet(const Packet& other);
-    Packet(Packet&& other) noexcept;
-    Packet(AVPacket* src);
-    Packet& operator=(const Packet& other);
-    Packet& operator=(Packet&& other) noexcept;
-    bool isValid() const { return m_pkt ? true : false; }
-    std::string description() const;
-
-    AVPacket* m_pkt = nullptr;
-};
-
-}
-
+/********************************************************************
+* libavio/include/Packet.h
+*
+* Copyright (c) 2022  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#ifndef PACKET_H
+#define PACKET_H
+
+extern "C" {
+#include "libavcodec/avcodec.h"
+}
+
+namespace avio
+{
+
+class Packet
+{
+public:
+    Packet();
+    ~Packet();
+    Packet(const Packet& other);
+    Packet(Packet&& other) noexcept;
+    Packet(AVPacket* src);
+    Packet& operator=(const Packet& other);
+    Packet& operator=(Packet&& other) noexcept;
+    bool isValid() const { return m_pkt ? true : false; }
+    std::string description() const;
+
+    AVPacket* m_pkt = nullptr;
+};
+
+}
+
 #endif // PACKET_H
```

### Comparing `avio-2.1.7/include/Pipe.h` & `avio-2.1.8/include/Pipe.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Player.h` & `avio-2.1.8/include/Player.h`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-/********************************************************************
-* libavio/include/Player.h
-*
-* Copyright (c) 2022  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#ifndef PLAYER_H
-#define PLAYER_H
-
-#include "Exception.h"
-#include "Queue.h"
-#include "Reader.h"
-#include "Decoder.h"
-#include "Pipe.h"
-#include "Filter.h"
-#include "Display.h"
-#include "Packet.h"
-#include "Encoder.h"
-#include "Writer.h"
-#include <functional>
-
-#define P ((Player*)player)
-
-namespace avio
-{
-
-class Player
-{
-
-public:
-    Reader*   reader       = nullptr;
-    Decoder*  videoDecoder = nullptr;
-    Decoder*  audioDecoder = nullptr;
-    Filter*   videoFilter  = nullptr;
-    Filter*   audioFilter  = nullptr;
-    Display*  display      = nullptr;
-    Encoder*  videoEncoder = nullptr;
-    Encoder*  audioEncoder = nullptr;
-    Writer*   writer       = nullptr;
-
-    Queue<Packet>* vpq_reader;
-    Queue<Frame>*  vfq_decoder;
-    Queue<Frame>*  vfq_filter;
-    Queue<Frame>*  vfq_display;
-    Queue<Packet>* apq_reader;
-    Queue<Frame>*  afq_decoder;
-    Queue<Frame>*  afq_filter;
-    Queue<Frame>*  afq_display;
-
-    std::function<int(void)> width = nullptr;
-    std::function<int(void)> height = nullptr;
-    std::function<void(float)> progressCallback = nullptr;
-    std::function<void(const Frame&)> renderCallback = nullptr;
-    std::function<Frame(Frame&)> pythonCallback  = nullptr;
-    std::function<Frame(Frame&)> pyAudioCallback = nullptr;
-    std::function<void(int64_t)> cbMediaPlayingStarted = nullptr;
-    std::function<void(void)> cbMediaPlayingStopped = nullptr;
-    std::function<void(const std::string&)> infoCallback = nullptr;
-    std::function<void(const std::string&)> errorCallback = nullptr;
-
-    uint64_t hWnd = 0;
-    std::string uri;
-    std::string video_filter = "null";
-    std::string audio_filter = "anull";
-    AVHWDeviceType hw_device_type = AV_HWDEVICE_TYPE_NONE;
-
-    bool running = false;
-    bool mute = false;
-    int volume = 100;
-    int last_progress = 0;
-    bool process_pause = false;
-    bool post_encode = false;
-    bool hw_encoding = false;
-    int keyframe_cache_size = 1;
-
-    int vpq_size = 0;
-    int apq_size = 0;
-
-    bool disable_video = false;
-    bool disable_audio = false;
-
-    Player() { av_log_set_level(AV_LOG_PANIC); }
-    ~Player() { }
-
-    bool isPaused();
-    bool isPiping();
-    bool isEncoding();
-    bool isRecording();
-    void togglePaused();
-    void togglePiping(const std::string& filename);
-    void toggleEncoding(const std::string& filename);
-    void toggleRecording(const std::string& filename);
-    void key_event(int keyCode);
-    void clear_queues();
-    void clear_decoders();
-    void run();
-    void start();
-    void seek(float arg);
-    void setMute(bool arg);
-    void setVolume(int arg);
-    bool checkForStreamHeader();
-
-    std::string getVideoCodec() const {
-        std::string result = "Unknown codec";
-        if (reader)
-            result = reader->str_video_codec();
-        return result;
-    }
-
-    int getVideoWidth() {
-        int result = 0;
-        if (reader)
-            result = reader->width();
-        return result;
-    }
-
-    int getVideoHeight() {
-        int result = 0;
-        if (reader)
-            result = reader->height();
-        return result;
-    }
-
-    int getVideoFrameRate() {
-        int result = 0;
-        if (reader)
-            result = (int)av_q2d(reader->frame_rate());
-        return result;
-    }
-
-    int getVideoBitrate() {
-        int result = 0;
-        if (reader)
-            result = reader->video_bit_rate();
-        return result;
-    }
-
-};
-
-
-}
-
+/********************************************************************
+* libavio/include/Player.h
+*
+* Copyright (c) 2022  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#ifndef PLAYER_H
+#define PLAYER_H
+
+#include "Exception.h"
+#include "Queue.h"
+#include "Reader.h"
+#include "Decoder.h"
+#include "Pipe.h"
+#include "Filter.h"
+#include "Display.h"
+#include "Packet.h"
+#include "Encoder.h"
+#include "Writer.h"
+#include <functional>
+
+#define P ((Player*)player)
+
+namespace avio
+{
+
+class Player
+{
+
+public:
+    Reader*   reader       = nullptr;
+    Decoder*  videoDecoder = nullptr;
+    Decoder*  audioDecoder = nullptr;
+    Filter*   videoFilter  = nullptr;
+    Filter*   audioFilter  = nullptr;
+    Display*  display      = nullptr;
+    Encoder*  videoEncoder = nullptr;
+    Encoder*  audioEncoder = nullptr;
+    Writer*   writer       = nullptr;
+
+    Queue<Packet>* vpq_reader;
+    Queue<Frame>*  vfq_decoder;
+    Queue<Frame>*  vfq_filter;
+    Queue<Frame>*  vfq_display;
+    Queue<Packet>* apq_reader;
+    Queue<Frame>*  afq_decoder;
+    Queue<Frame>*  afq_filter;
+    Queue<Frame>*  afq_display;
+
+    std::function<int(void)> width = nullptr;
+    std::function<int(void)> height = nullptr;
+    std::function<void(float)> progressCallback = nullptr;
+    std::function<void(const Frame&)> renderCallback = nullptr;
+    std::function<Frame(Frame&)> pythonCallback  = nullptr;
+    std::function<Frame(Frame&)> pyAudioCallback = nullptr;
+    std::function<void(int64_t)> cbMediaPlayingStarted = nullptr;
+    std::function<void(void)> cbMediaPlayingStopped = nullptr;
+    std::function<void(const std::string&)> infoCallback = nullptr;
+    std::function<void(const std::string&)> errorCallback = nullptr;
+
+    uint64_t hWnd = 0;
+    std::string uri;
+    std::string video_filter = "null";
+    std::string audio_filter = "anull";
+    AVHWDeviceType hw_device_type = AV_HWDEVICE_TYPE_NONE;
+
+    bool running = false;
+    bool mute = false;
+    int volume = 100;
+    int last_progress = 0;
+    bool process_pause = false;
+    bool post_encode = false;
+    bool hw_encoding = false;
+    int keyframe_cache_size = 1;
+
+    int vpq_size = 0;
+    int apq_size = 0;
+
+    bool disable_video = false;
+    bool disable_audio = false;
+
+    Player() { av_log_set_level(AV_LOG_PANIC); }
+    ~Player() { }
+
+    bool isPaused();
+    bool isPiping();
+    bool isEncoding();
+    bool isRecording();
+    void togglePaused();
+    void togglePiping(const std::string& filename);
+    void toggleEncoding(const std::string& filename);
+    void toggleRecording(const std::string& filename);
+    void key_event(int keyCode);
+    void clear_queues();
+    void clear_decoders();
+    void run();
+    void start();
+    void seek(float arg);
+    void setMute(bool arg);
+    void setVolume(int arg);
+    bool checkForStreamHeader();
+
+    std::string getVideoCodec() const {
+        std::string result = "Unknown codec";
+        if (reader)
+            result = reader->str_video_codec();
+        return result;
+    }
+
+    int getVideoWidth() {
+        int result = 0;
+        if (reader)
+            result = reader->width();
+        return result;
+    }
+
+    int getVideoHeight() {
+        int result = 0;
+        if (reader)
+            result = reader->height();
+        return result;
+    }
+
+    int getVideoFrameRate() {
+        int result = 0;
+        if (reader)
+            result = (int)av_q2d(reader->frame_rate());
+        return result;
+    }
+
+    int getVideoBitrate() {
+        int result = 0;
+        if (reader)
+            result = reader->video_bit_rate();
+        return result;
+    }
+
+};
+
+
+}
+
 #endif // PLAYER_H
```

### Comparing `avio-2.1.7/include/Queue.h` & `avio-2.1.8/include/Queue.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Reader.h` & `avio-2.1.8/include/Reader.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/include/Writer.h` & `avio-2.1.8/include/Writer.h`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-/********************************************************************
-* libavio/include/Writer.h
-*
-* Copyright (c) 2023  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#ifndef WRITER_H
-#define WRITER_H
-
-extern "C" {
-#include <libavutil/avassert.h>
-#include <libavutil/channel_layout.h>
-#include <libavutil/opt.h>
-#include <libavutil/mathematics.h>
-#include <libavutil/timestamp.h>
-#include <libavcodec/avcodec.h>
-#include <libavformat/avformat.h>
-#include <libswscale/swscale.h>
-#include <libswresample/swresample.h>
-}
-
-#include <mutex>
-
-#include "Exception.h"
-
-namespace avio
-{
-
-enum class EncoderState {
-    MIXED,
-    OPEN,
-    CLOSED
-};
-
-class Writer
-{
-public:
-    Writer(const std::string& format);
-    ~Writer();
-    void open();
-    void write(AVPacket* pkt);
-    void close();
-    void init();
-    EncoderState getEncoderState();
-
-    AVFormatContext* fmt_ctx = NULL;
-    int video_stream_id = AVERROR_STREAM_NOT_FOUND;
-    int audio_stream_id = AVERROR_STREAM_NOT_FOUND;
-
-    std::string m_format;
-    std::string write_dir;
-    std::string filename;
-
-    void* videoEncoder = nullptr;
-    void* audioEncoder = nullptr;
-    bool enabled = false;
-    bool opened = false;
-
-    bool show_video_pkts = false;
-    bool show_audio_pkts = false;
-
-    std::mutex mutex;
-
-	std::function<void(const std::string&)> infoCallback = nullptr;
-    ExceptionHandler ex;
-
-};
-
-}
-
-#endif // WRITER_H
+/********************************************************************
+* libavio/include/Writer.h
+*
+* Copyright (c) 2023  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#ifndef WRITER_H
+#define WRITER_H
+
+extern "C" {
+#include <libavutil/avassert.h>
+#include <libavutil/channel_layout.h>
+#include <libavutil/opt.h>
+#include <libavutil/mathematics.h>
+#include <libavutil/timestamp.h>
+#include <libavcodec/avcodec.h>
+#include <libavformat/avformat.h>
+#include <libswscale/swscale.h>
+#include <libswresample/swresample.h>
+}
+
+#include <mutex>
+
+#include "Exception.h"
+
+namespace avio
+{
+
+enum class EncoderState {
+    MIXED,
+    OPEN,
+    CLOSED
+};
+
+class Writer
+{
+public:
+    Writer(const std::string& format);
+    ~Writer();
+    void open();
+    void write(AVPacket* pkt);
+    void close();
+    void init();
+    EncoderState getEncoderState();
+
+    AVFormatContext* fmt_ctx = NULL;
+    int video_stream_id = AVERROR_STREAM_NOT_FOUND;
+    int audio_stream_id = AVERROR_STREAM_NOT_FOUND;
+
+    std::string m_format;
+    std::string write_dir;
+    std::string filename;
+
+    void* videoEncoder = nullptr;
+    void* audioEncoder = nullptr;
+    bool enabled = false;
+    bool opened = false;
+
+    bool show_video_pkts = false;
+    bool show_audio_pkts = false;
+
+    std::mutex mutex;
+
+	std::function<void(const std::string&)> infoCallback = nullptr;
+    ExceptionHandler ex;
+
+};
+
+}
+
+#endif // WRITER_H
```

### Comparing `avio-2.1.7/include/avio.h` & `avio-2.1.8/include/avio.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.appveyor.yml` & `avio-2.1.8/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.clang-format` & `avio-2.1.8/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.clang-tidy` & `avio-2.1.8/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.cmake-format.yaml` & `avio-2.1.8/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.codespell-ignore-lines` & `avio-2.1.8/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/CONTRIBUTING.md` & `avio-2.1.8/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `avio-2.1.8/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/matchers/pylint.json` & `avio-2.1.8/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/pull_request_template.md` & `avio-2.1.8/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/ci.yml` & `avio-2.1.8/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/configure.yml` & `avio-2.1.8/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/format.yml` & `avio-2.1.8/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/labeler.yml` & `avio-2.1.8/pybind11/.github/workflows/labeler.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/pip.yml` & `avio-2.1.8/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.github/workflows/upstream.yml` & `avio-2.1.8/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/.pre-commit-config.yaml` & `avio-2.1.8/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/CMakeLists.txt` & `avio-2.1.8/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/LICENSE` & `avio-2.1.8/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/README.rst` & `avio-2.1.8/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/Doxyfile` & `avio-2.1.8/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/Makefile` & `avio-2.1.8/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/chrono.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/custom.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/eigen.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/functional.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/index.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/overview.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/stl.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/cast/strings.rst` & `avio-2.1.8/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/classes.rst` & `avio-2.1.8/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/embedding.rst` & `avio-2.1.8/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/exceptions.rst` & `avio-2.1.8/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/functions.rst` & `avio-2.1.8/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/misc.rst` & `avio-2.1.8/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/pycpp/numpy.rst` & `avio-2.1.8/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/pycpp/object.rst` & `avio-2.1.8/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/pycpp/utilities.rst` & `avio-2.1.8/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/advanced/smart_ptrs.rst` & `avio-2.1.8/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/basics.rst` & `avio-2.1.8/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/benchmark.py` & `avio-2.1.8/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/benchmark.rst` & `avio-2.1.8/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/changelog.rst` & `avio-2.1.8/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/classes.rst` & `avio-2.1.8/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/compiling.rst` & `avio-2.1.8/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/conf.py` & `avio-2.1.8/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/faq.rst` & `avio-2.1.8/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/index.rst` & `avio-2.1.8/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/installing.rst` & `avio-2.1.8/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/limitations.rst` & `avio-2.1.8/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/pybind11-logo.png` & `avio-2.1.8/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/pybind11_vs_boost_python1.png` & `avio-2.1.8/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/pybind11_vs_boost_python1.svg` & `avio-2.1.8/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/pybind11_vs_boost_python2.png` & `avio-2.1.8/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/pybind11_vs_boost_python2.svg` & `avio-2.1.8/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/reference.rst` & `avio-2.1.8/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/release.rst` & `avio-2.1.8/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/docs/upgrade.rst` & `avio-2.1.8/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/attr.h` & `avio-2.1.8/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/buffer_info.h` & `avio-2.1.8/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/cast.h` & `avio-2.1.8/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/chrono.h` & `avio-2.1.8/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/complex.h` & `avio-2.1.8/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/class.h` & `avio-2.1.8/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/common.h` & `avio-2.1.8/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/descr.h` & `avio-2.1.8/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/init.h` & `avio-2.1.8/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/internals.h` & `avio-2.1.8/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/type_caster_base.h` & `avio-2.1.8/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/detail/typeid.h` & `avio-2.1.8/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/eigen/matrix.h` & `avio-2.1.8/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/eigen/tensor.h` & `avio-2.1.8/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/embed.h` & `avio-2.1.8/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/eval.h` & `avio-2.1.8/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/functional.h` & `avio-2.1.8/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/gil.h` & `avio-2.1.8/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/iostream.h` & `avio-2.1.8/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/numpy.h` & `avio-2.1.8/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/operators.h` & `avio-2.1.8/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/options.h` & `avio-2.1.8/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/pybind11.h` & `avio-2.1.8/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/pytypes.h` & `avio-2.1.8/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/stl/filesystem.h` & `avio-2.1.8/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/stl.h` & `avio-2.1.8/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/include/pybind11/stl_bind.h` & `avio-2.1.8/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/noxfile.py` & `avio-2.1.8/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/pybind11/__main__.py` & `avio-2.1.8/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/pybind11/commands.py` & `avio-2.1.8/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/pybind11/setup_helpers.py` & `avio-2.1.8/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/pyproject.toml` & `avio-2.1.8/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/setup.cfg` & `avio-2.1.8/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/setup.py` & `avio-2.1.8/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/conftest.py` & `avio-2.1.8/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/constructor_stats.h` & `avio-2.1.8/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/cross_module_gil_utils.cpp` & `avio-2.1.8/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `avio-2.1.8/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/env.py` & `avio-2.1.8/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/extra_python_package/test_files.py` & `avio-2.1.8/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/extra_setuptools/test_setuphelper.py` & `avio-2.1.8/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/local_bindings.h` & `avio-2.1.8/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/object.h` & `avio-2.1.8/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/pybind11_cross_module_tests.cpp` & `avio-2.1.8/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/pybind11_tests.cpp` & `avio-2.1.8/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/pybind11_tests.h` & `avio-2.1.8/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/pytest.ini` & `avio-2.1.8/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/requirements.txt` & `avio-2.1.8/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_async.cpp` & `avio-2.1.8/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_async.py` & `avio-2.1.8/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_buffers.cpp` & `avio-2.1.8/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_buffers.py` & `avio-2.1.8/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_builtin_casters.cpp` & `avio-2.1.8/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_builtin_casters.py` & `avio-2.1.8/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_call_policies.cpp` & `avio-2.1.8/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_call_policies.py` & `avio-2.1.8/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_callbacks.cpp` & `avio-2.1.8/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_callbacks.py` & `avio-2.1.8/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_chrono.cpp` & `avio-2.1.8/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_chrono.py` & `avio-2.1.8/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_class.cpp` & `avio-2.1.8/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_class.py` & `avio-2.1.8/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/embed.cpp` & `avio-2.1.8/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_const_name.cpp` & `avio-2.1.8/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_const_name.py` & `avio-2.1.8/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_constants_and_functions.cpp` & `avio-2.1.8/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_constants_and_functions.py` & `avio-2.1.8/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_copy_move.cpp` & `avio-2.1.8/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_copy_move.py` & `avio-2.1.8/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_custom_type_casters.cpp` & `avio-2.1.8/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_custom_type_casters.py` & `avio-2.1.8/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_custom_type_setup.cpp` & `avio-2.1.8/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_custom_type_setup.py` & `avio-2.1.8/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_docstring_options.cpp` & `avio-2.1.8/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_docstring_options.py` & `avio-2.1.8/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eigen_matrix.cpp` & `avio-2.1.8/pybind11/tests/test_eigen_matrix.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eigen_matrix.py` & `avio-2.1.8/pybind11/tests/test_eigen_matrix.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eigen_tensor.inl` & `avio-2.1.8/pybind11/tests/test_eigen_tensor.inl`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eigen_tensor.py` & `avio-2.1.8/pybind11/tests/test_eigen_tensor.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_embed/CMakeLists.txt` & `avio-2.1.8/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_embed/catch.cpp` & `avio-2.1.8/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_embed/external_module.cpp` & `avio-2.1.8/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_embed/test_interpreter.cpp` & `avio-2.1.8/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_enum.cpp` & `avio-2.1.8/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_enum.py` & `avio-2.1.8/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eval.cpp` & `avio-2.1.8/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_eval.py` & `avio-2.1.8/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_exceptions.cpp` & `avio-2.1.8/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_exceptions.py` & `avio-2.1.8/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_factory_constructors.cpp` & `avio-2.1.8/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_factory_constructors.py` & `avio-2.1.8/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_gil_scoped.cpp` & `avio-2.1.8/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_gil_scoped.py` & `avio-2.1.8/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_iostream.cpp` & `avio-2.1.8/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_iostream.py` & `avio-2.1.8/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_kwargs_and_defaults.cpp` & `avio-2.1.8/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_kwargs_and_defaults.py` & `avio-2.1.8/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_local_bindings.cpp` & `avio-2.1.8/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_local_bindings.py` & `avio-2.1.8/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_methods_and_attributes.cpp` & `avio-2.1.8/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_methods_and_attributes.py` & `avio-2.1.8/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_modules.cpp` & `avio-2.1.8/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_modules.py` & `avio-2.1.8/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_multiple_inheritance.cpp` & `avio-2.1.8/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_multiple_inheritance.py` & `avio-2.1.8/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_array.cpp` & `avio-2.1.8/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_array.py` & `avio-2.1.8/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_dtypes.cpp` & `avio-2.1.8/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_dtypes.py` & `avio-2.1.8/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_vectorize.cpp` & `avio-2.1.8/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_numpy_vectorize.py` & `avio-2.1.8/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_opaque_types.cpp` & `avio-2.1.8/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_opaque_types.py` & `avio-2.1.8/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_operator_overloading.cpp` & `avio-2.1.8/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_operator_overloading.py` & `avio-2.1.8/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_pickling.cpp` & `avio-2.1.8/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_pickling.py` & `avio-2.1.8/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_pytypes.cpp` & `avio-2.1.8/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_pytypes.py` & `avio-2.1.8/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_sequences_and_iterators.cpp` & `avio-2.1.8/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_sequences_and_iterators.py` & `avio-2.1.8/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_smart_ptr.cpp` & `avio-2.1.8/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_smart_ptr.py` & `avio-2.1.8/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_stl.cpp` & `avio-2.1.8/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_stl.py` & `avio-2.1.8/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_stl_binders.cpp` & `avio-2.1.8/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_stl_binders.py` & `avio-2.1.8/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_tagbased_polymorphic.cpp` & `avio-2.1.8/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_tagbased_polymorphic.py` & `avio-2.1.8/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_thread.cpp` & `avio-2.1.8/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_thread.py` & `avio-2.1.8/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_union.cpp` & `avio-2.1.8/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_virtual_functions.cpp` & `avio-2.1.8/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/test_virtual_functions.py` & `avio-2.1.8/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/valgrind-numpy-scipy.supp` & `avio-2.1.8/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tests/valgrind-python.supp` & `avio-2.1.8/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/FindCatch.cmake` & `avio-2.1.8/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/FindEigen3.cmake` & `avio-2.1.8/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/FindPythonLibsNew.cmake` & `avio-2.1.8/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/JoinPaths.cmake` & `avio-2.1.8/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/check-style.sh` & `avio-2.1.8/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/cmake_uninstall.cmake.in` & `avio-2.1.8/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/codespell_ignore_lines_from_errors.py` & `avio-2.1.8/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/libsize.py` & `avio-2.1.8/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/make_changelog.py` & `avio-2.1.8/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/pybind11Common.cmake` & `avio-2.1.8/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/pybind11Config.cmake.in` & `avio-2.1.8/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/pybind11NewTools.cmake` & `avio-2.1.8/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/pybind11Tools.cmake` & `avio-2.1.8/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/setup_global.py.in` & `avio-2.1.8/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pybind11/tools/setup_main.py.in` & `avio-2.1.8/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/pyproject.toml` & `avio-2.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-#/********************************************************************
-# libavio/pyproject.toml
-#
-# Copyright (c) 2023  Stephen Rhodes
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-#*********************************************************************/
-
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "avio"
-version = "2.1.7"
-authors = [
-    { name="Stephen Rhodes", email="sr99622@gmail.com" },
-]
-description = "A python module for processing media streams"
-readme = "README.md"
-requires-python = ">=3.6"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/sr99622/libavio"
+#/********************************************************************
+# libavio/pyproject.toml
+#
+# Copyright (c) 2023  Stephen Rhodes
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+#*********************************************************************/
+
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "avio"
+version = "2.1.8"
+authors = [
+    { name="Stephen Rhodes", email="sr99622@gmail.com" },
+]
+description = "A python module for processing media streams"
+readme = "README.md"
+requires-python = ">=3.6"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: Apache Software License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/sr99622/libavio"
 "Bug Tracker" = "https://github.com/sr99622/libavio/issues"
```

### Comparing `avio-2.1.7/src/Clock.cpp` & `avio-2.1.8/src/Clock.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Decoder.cpp` & `avio-2.1.8/src/Decoder.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Display.cpp` & `avio-2.1.8/src/Display.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Encoder.cpp` & `avio-2.1.8/src/Encoder.cpp`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,325 +1,325 @@
-/********************************************************************
-* libavio/src/Encoder.cpp
-*
-* Copyright (c) 2022  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#include "Encoder.h"
-
-namespace avio
-{
-
-Encoder::Encoder(Writer* writer, AVMediaType mediaType) : mediaType(mediaType), writer(writer)
-{
-    if (mediaType == AVMEDIA_TYPE_VIDEO) this->writer->videoEncoder = this;
-    if (mediaType == AVMEDIA_TYPE_AUDIO) this->writer->audioEncoder = this;
-}
-
-void Encoder::init()
-{
-    const char* str = av_get_media_type_string(mediaType);
-    strMediaType = (str ? str : "UNKOWN MEDIA TYPE");
-
-    switch (mediaType) {
-    case AVMEDIA_TYPE_VIDEO:
-        openVideoStream();
-        break;
-    case AVMEDIA_TYPE_AUDIO:
-        openAudioStream();
-        break;
-    default:
-        std::string msg = "Encoder constructor failed: unknown media type";
-        if (infoCallback) infoCallback(msg);
-        else std::cout << msg << std::endl;
-    }
-}
-
-Encoder::~Encoder()
-{
-    close();
-}
-
-void Encoder::close()
-{
-    if (enc_ctx)       avcodec_free_context(&enc_ctx);
-    if (pkt)           av_packet_free(&pkt);
-    if (hw_frame)      av_frame_free(&hw_frame);
-    if (hw_device_ctx) av_buffer_unref(&hw_device_ctx);
-    if (cvt_frame)     av_frame_free(&cvt_frame);
-    opened = false;
-}
-
-void Encoder::openVideoStream()
-{
-    if (!writer->fmt_ctx) 
-        writer->init();
-
-    AVFormatContext* fmt_ctx = writer->fmt_ctx;
-    AVCodecID codec_id = writer->fmt_ctx->oformat->video_codec;
-
-    first_pass = true;
-    pts_offset = 0;
-
-    try {
-        const AVCodec* codec;
-        ex.ck(pkt = av_packet_alloc(), APA);
-
-        if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
-            codec = avcodec_find_encoder_by_name(hw_video_codec_name.c_str());
-            std::stringstream str;
-            str << "avcodec_find_encoder_by_name: " << hw_video_codec_name;
-            if (!codec) throw Exception(str.str());
-        }
-        else {
-            codec = avcodec_find_encoder(fmt_ctx->oformat->video_codec);
-            if (!codec) throw Exception("avcodec_find_encoder");
-        }
-
-        ex.ck(stream = avformat_new_stream(fmt_ctx, NULL), ANS);
-        stream->id = fmt_ctx->nb_streams - 1;
-        writer->video_stream_id = stream->id;
-        ex.ck(enc_ctx = avcodec_alloc_context3(codec), AAC3);
-
-        enc_ctx->codec_id = codec_id;
-        enc_ctx->bit_rate = video_bit_rate;
-        enc_ctx->width = width;
-        enc_ctx->height = height;
-        enc_ctx->framerate = frame_rate;
-        stream->time_base = video_time_base;
-        enc_ctx->time_base = video_time_base;
-        enc_ctx->gop_size = gop_size;
-
-        cvt_frame = av_frame_alloc();
-        cvt_frame->width = enc_ctx->width;
-        cvt_frame->height = enc_ctx->height;
-        cvt_frame->format = AV_PIX_FMT_YUV420P;
-        av_frame_get_buffer(cvt_frame, 0);
-        av_frame_make_writable(cvt_frame);
-
-        if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
-            enc_ctx->pix_fmt = hw_pix_fmt;
-            if (!profile.empty())
-                av_opt_set(enc_ctx->priv_data, "profile", profile.c_str(), 0);
-
-            ex.ck(av_hwdevice_ctx_create(&hw_device_ctx, hw_device_type, NULL, NULL, 0), AHCC);
-            ex.ck(hw_frames_ref = av_hwframe_ctx_alloc(hw_device_ctx), AHCA);
-
-            AVHWFramesContext* frames_ctx = (AVHWFramesContext*)(hw_frames_ref->data);
-            frames_ctx->format = hw_pix_fmt;
-            frames_ctx->sw_format = sw_pix_fmt;
-            frames_ctx->width = width;
-            frames_ctx->height = height;
-            frames_ctx->initial_pool_size = 20;
-
-            ex.ck(av_hwframe_ctx_init(hw_frames_ref), AHCI);
-            ex.ck(enc_ctx->hw_frames_ctx = av_buffer_ref(hw_frames_ref), ABR);
-            av_buffer_unref(&hw_frames_ref);
-
-            ex.ck(hw_frame = av_frame_alloc(), AFA);
-            ex.ck(av_hwframe_get_buffer(enc_ctx->hw_frames_ctx, hw_frame, 0), AHGB);
-        }
-        else {
-            enc_ctx->pix_fmt = pix_fmt;
-        }
-
-        if (enc_ctx->codec_id == AV_CODEC_ID_MPEG2VIDEO) enc_ctx->max_b_frames = 2;
-        if (enc_ctx->codec_id == AV_CODEC_ID_MPEG1VIDEO) enc_ctx->mb_decision = 2;
-
-        if (fmt_ctx->oformat->flags & AVFMT_GLOBALHEADER)
-            enc_ctx->flags |= AV_CODEC_FLAG_GLOBAL_HEADER;
-
-        ex.ck(avcodec_open2(enc_ctx, codec, &opts), AO2);
-        ex.ck(avcodec_parameters_from_context(stream->codecpar, enc_ctx), APFC);
-
-        opened = true;
-    }
-    catch (const Exception& e) {
-        std::stringstream str;
-        str << "Encoder video stream constructor exception: " << e.what();
-        if (infoCallback) infoCallback(str.str());
-        else std::cout << str.str() << std::endl;
-        close();
-    }
-}
-
-void Encoder::openAudioStream()
-{
-    if (!writer->fmt_ctx) 
-        writer->init();
-
-    AVFormatContext* fmt_ctx = writer->fmt_ctx;
-    AVCodecID codec_id = writer->fmt_ctx->oformat->audio_codec;
-
-    first_pass = true;
-    pts_offset = 0;
-
-    try {
-        const AVCodec* codec;
-        codec = avcodec_find_encoder(codec_id);
-
-        if (!codec)
-            throw Exception(std::string("avcodec_find_decoder could not find ") + avcodec_get_name(codec_id));
-
-        ex.ck(pkt = av_packet_alloc(), APA);
-        ex.ck(stream = avformat_new_stream(fmt_ctx, NULL), ANS);
-        stream->id = fmt_ctx->nb_streams - 1;
-        writer->audio_stream_id = stream->id;
-        ex.ck(enc_ctx = avcodec_alloc_context3(codec), AAC3);
-
-        enc_ctx->sample_fmt = sample_fmt;
-        enc_ctx->bit_rate = audio_bit_rate;
-        enc_ctx->sample_rate = sample_rate;
-        enc_ctx->channel_layout = channel_layout;
-        enc_ctx->channels = av_get_channel_layout_nb_channels(enc_ctx->channel_layout);
-        enc_ctx->frame_size = nb_samples;
-        stream->time_base = audio_time_base;
-
-        cvt_frame = av_frame_alloc();
-        cvt_frame->channels = enc_ctx->channels;
-        cvt_frame->channel_layout = enc_ctx->channel_layout;
-        cvt_frame->format = sample_fmt;
-        cvt_frame->nb_samples = nb_samples;
-        av_frame_get_buffer(cvt_frame, 0);
-        av_frame_make_writable(cvt_frame);
-
-        if (fmt_ctx->oformat->flags & AVFMT_GLOBALHEADER)
-            enc_ctx->flags |= AV_CODEC_FLAG_GLOBAL_HEADER;
-
-        ex.ck(avcodec_open2(enc_ctx, codec, NULL), AO2);
-        ex.ck(avcodec_parameters_from_context(stream->codecpar, enc_ctx), APFC);
-
-        opened = true;
-    }
-    catch (const Exception& e) {
-        std::stringstream str;
-        str << "AudioStream constructor exception: " << e.what();
-        if (infoCallback) infoCallback(str.str());
-        else std::cout << str.str() << std::endl;
-        close();
-    }
-}
-
-bool Encoder::cmpFrame(AVFrame* frame)
-{
-    if (mediaType == AVMEDIA_TYPE_VIDEO)
-        return (frame->width == width && frame->height == height && frame->format == pix_fmt);
-    if (mediaType == AVMEDIA_TYPE_AUDIO)
-        return (frame->channels == channels && frame->channel_layout == channel_layout &&
-            frame->nb_samples == nb_samples && frame->format == sample_fmt);
-
-    return false;
-}
-
-int Encoder::encode(Frame& f)
-{
-    int ret = 0;
-
-    try {
-
-        f.set_pts(stream);
-        AVFrame* frame = f.m_frame;
-
-        if (frame) {
-            if (mediaType == AVMEDIA_TYPE_VIDEO && !cmpFrame(frame)) {
-                if (!sws_ctx) {
-                    ex.ck(sws_ctx = sws_getContext(frame->width, frame->height, (AVPixelFormat)frame->format,
-                        enc_ctx->width, enc_ctx->height, AV_PIX_FMT_YUV420P, SWS_BICUBIC, NULL, NULL, NULL), SGC);
-                }
-
-                ex.ck(sws_scale(sws_ctx, frame->data, frame->linesize, 0, enc_ctx->height,
-                    cvt_frame->data, cvt_frame->linesize), SS);
-
-                cvt_frame->pts = av_rescale_q(frame->pts, video_time_base, enc_ctx->time_base);
-                frame = cvt_frame;
-            }
-
-            if (mediaType == AVMEDIA_TYPE_AUDIO && !cmpFrame(frame)) {
-                if (!swr_ctx) {
-                    ex.ck(swr_ctx = swr_alloc(), SA);
-                    av_opt_set_int(swr_ctx, "in_channel_count", frame->channels, 0);
-                    av_opt_set_int(swr_ctx, "out_channel_count", channels, 0);
-                    av_opt_set_channel_layout(swr_ctx, "in_channel_layout", frame->channel_layout, 0);
-                    av_opt_set_channel_layout(swr_ctx, "out_channel_layout", channel_layout, 0);
-                    av_opt_set_int(swr_ctx, "in_sample_rate", frame->sample_rate, 0);
-                    av_opt_set_int(swr_ctx, "out_sample_rate", sample_rate, 0);
-                    av_opt_set_sample_fmt(swr_ctx, "in_sample_fmt", (AVSampleFormat)frame->format, 0);
-                    av_opt_set_sample_fmt(swr_ctx, "out_sample_fmt", sample_fmt, 0);
-                    ex.ck(swr_init(swr_ctx), SI);
-                }
-
-                ex.ck(swr_convert(swr_ctx, cvt_frame->data, cvt_frame->nb_samples, (const uint8_t**)frame->data, frame->nb_samples), SC);
-
-                cvt_frame->pts = av_rescale_q(total_samples, av_make_q(1, enc_ctx->sample_rate), enc_ctx->time_base);
-                cvt_frame->sample_rate = sample_rate;
-                total_samples += nb_samples;
-                frame = cvt_frame;
-            }
-
-            if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
-                av_frame_copy_props(hw_frame, frame);
-                ex.ck(av_hwframe_transfer_data(hw_frame, frame, 0), AHTD);
-                ex.ck(avcodec_send_frame(enc_ctx, hw_frame), ASF);
-            }
-            else {
-                ex.ck(avcodec_send_frame(enc_ctx, frame), "avcodec_send_frame");
-            }
-        }
-        else {
-            ex.ck(ret = avcodec_send_frame(enc_ctx, NULL), "avcodec_send_frame");
-        }
-
-        while (ret >= 0) {
-            ret = avcodec_receive_packet(enc_ctx, pkt);
-            if (ret == AVERROR(EAGAIN) || ret == AVERROR_EOF)
-                break;
-            else if (ret < 0) 
-                ex.ck(ret, CmdTag::ARP);
-
-            pkt->stream_index = stream->index;
-
-            AVPacket* tmp = av_packet_alloc();
-
-            // needed to prevent corruption in dts
-            if (pkt->dts > pkt->pts) 
-                pkt->dts = pkt->pts - 2;
-
-            tmp = av_packet_clone(pkt);
-
-            if (first_pass) {
-                pts_offset = tmp->pts;
-                first_pass = false;
-            }
-            tmp->pts -= pts_offset;
-            tmp->dts -= pts_offset;
-
-            writer->write(tmp);
-
-        }
-    }
-    catch (const Exception& e) {
-        if (strcmp(e.what(), "End of file")) {
-            std::stringstream str;
-            str << strMediaType << " encode exception: " << e.what(); 
-            if (infoCallback) infoCallback(str.str());
-            else std::cout << str.str() << std::endl;
-        }
-    }
-
-    return ret;
-}
-
-
-}
+/********************************************************************
+* libavio/src/Encoder.cpp
+*
+* Copyright (c) 2022  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#include "Encoder.h"
+
+namespace avio
+{
+
+Encoder::Encoder(Writer* writer, AVMediaType mediaType) : mediaType(mediaType), writer(writer)
+{
+    if (mediaType == AVMEDIA_TYPE_VIDEO) this->writer->videoEncoder = this;
+    if (mediaType == AVMEDIA_TYPE_AUDIO) this->writer->audioEncoder = this;
+}
+
+void Encoder::init()
+{
+    const char* str = av_get_media_type_string(mediaType);
+    strMediaType = (str ? str : "UNKOWN MEDIA TYPE");
+
+    switch (mediaType) {
+    case AVMEDIA_TYPE_VIDEO:
+        openVideoStream();
+        break;
+    case AVMEDIA_TYPE_AUDIO:
+        openAudioStream();
+        break;
+    default:
+        std::string msg = "Encoder constructor failed: unknown media type";
+        if (infoCallback) infoCallback(msg);
+        else std::cout << msg << std::endl;
+    }
+}
+
+Encoder::~Encoder()
+{
+    close();
+}
+
+void Encoder::close()
+{
+    if (enc_ctx)       avcodec_free_context(&enc_ctx);
+    if (pkt)           av_packet_free(&pkt);
+    if (hw_frame)      av_frame_free(&hw_frame);
+    if (hw_device_ctx) av_buffer_unref(&hw_device_ctx);
+    if (cvt_frame)     av_frame_free(&cvt_frame);
+    opened = false;
+}
+
+void Encoder::openVideoStream()
+{
+    if (!writer->fmt_ctx) 
+        writer->init();
+
+    AVFormatContext* fmt_ctx = writer->fmt_ctx;
+    AVCodecID codec_id = writer->fmt_ctx->oformat->video_codec;
+
+    first_pass = true;
+    pts_offset = 0;
+
+    try {
+        const AVCodec* codec;
+        ex.ck(pkt = av_packet_alloc(), APA);
+
+        if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
+            codec = avcodec_find_encoder_by_name(hw_video_codec_name.c_str());
+            std::stringstream str;
+            str << "avcodec_find_encoder_by_name: " << hw_video_codec_name;
+            if (!codec) throw Exception(str.str());
+        }
+        else {
+            codec = avcodec_find_encoder(fmt_ctx->oformat->video_codec);
+            if (!codec) throw Exception("avcodec_find_encoder");
+        }
+
+        ex.ck(stream = avformat_new_stream(fmt_ctx, NULL), ANS);
+        stream->id = fmt_ctx->nb_streams - 1;
+        writer->video_stream_id = stream->id;
+        ex.ck(enc_ctx = avcodec_alloc_context3(codec), AAC3);
+
+        enc_ctx->codec_id = codec_id;
+        enc_ctx->bit_rate = video_bit_rate;
+        enc_ctx->width = width;
+        enc_ctx->height = height;
+        enc_ctx->framerate = frame_rate;
+        stream->time_base = video_time_base;
+        enc_ctx->time_base = video_time_base;
+        enc_ctx->gop_size = gop_size;
+
+        cvt_frame = av_frame_alloc();
+        cvt_frame->width = enc_ctx->width;
+        cvt_frame->height = enc_ctx->height;
+        cvt_frame->format = AV_PIX_FMT_YUV420P;
+        av_frame_get_buffer(cvt_frame, 0);
+        av_frame_make_writable(cvt_frame);
+
+        if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
+            enc_ctx->pix_fmt = hw_pix_fmt;
+            if (!profile.empty())
+                av_opt_set(enc_ctx->priv_data, "profile", profile.c_str(), 0);
+
+            ex.ck(av_hwdevice_ctx_create(&hw_device_ctx, hw_device_type, NULL, NULL, 0), AHCC);
+            ex.ck(hw_frames_ref = av_hwframe_ctx_alloc(hw_device_ctx), AHCA);
+
+            AVHWFramesContext* frames_ctx = (AVHWFramesContext*)(hw_frames_ref->data);
+            frames_ctx->format = hw_pix_fmt;
+            frames_ctx->sw_format = sw_pix_fmt;
+            frames_ctx->width = width;
+            frames_ctx->height = height;
+            frames_ctx->initial_pool_size = 20;
+
+            ex.ck(av_hwframe_ctx_init(hw_frames_ref), AHCI);
+            ex.ck(enc_ctx->hw_frames_ctx = av_buffer_ref(hw_frames_ref), ABR);
+            av_buffer_unref(&hw_frames_ref);
+
+            ex.ck(hw_frame = av_frame_alloc(), AFA);
+            ex.ck(av_hwframe_get_buffer(enc_ctx->hw_frames_ctx, hw_frame, 0), AHGB);
+        }
+        else {
+            enc_ctx->pix_fmt = pix_fmt;
+        }
+
+        if (enc_ctx->codec_id == AV_CODEC_ID_MPEG2VIDEO) enc_ctx->max_b_frames = 2;
+        if (enc_ctx->codec_id == AV_CODEC_ID_MPEG1VIDEO) enc_ctx->mb_decision = 2;
+
+        if (fmt_ctx->oformat->flags & AVFMT_GLOBALHEADER)
+            enc_ctx->flags |= AV_CODEC_FLAG_GLOBAL_HEADER;
+
+        ex.ck(avcodec_open2(enc_ctx, codec, &opts), AO2);
+        ex.ck(avcodec_parameters_from_context(stream->codecpar, enc_ctx), APFC);
+
+        opened = true;
+    }
+    catch (const Exception& e) {
+        std::stringstream str;
+        str << "Encoder video stream constructor exception: " << e.what();
+        if (infoCallback) infoCallback(str.str());
+        else std::cout << str.str() << std::endl;
+        close();
+    }
+}
+
+void Encoder::openAudioStream()
+{
+    if (!writer->fmt_ctx) 
+        writer->init();
+
+    AVFormatContext* fmt_ctx = writer->fmt_ctx;
+    AVCodecID codec_id = writer->fmt_ctx->oformat->audio_codec;
+
+    first_pass = true;
+    pts_offset = 0;
+
+    try {
+        const AVCodec* codec;
+        codec = avcodec_find_encoder(codec_id);
+
+        if (!codec)
+            throw Exception(std::string("avcodec_find_decoder could not find ") + avcodec_get_name(codec_id));
+
+        ex.ck(pkt = av_packet_alloc(), APA);
+        ex.ck(stream = avformat_new_stream(fmt_ctx, NULL), ANS);
+        stream->id = fmt_ctx->nb_streams - 1;
+        writer->audio_stream_id = stream->id;
+        ex.ck(enc_ctx = avcodec_alloc_context3(codec), AAC3);
+
+        enc_ctx->sample_fmt = sample_fmt;
+        enc_ctx->bit_rate = audio_bit_rate;
+        enc_ctx->sample_rate = sample_rate;
+        enc_ctx->channel_layout = channel_layout;
+        enc_ctx->channels = av_get_channel_layout_nb_channels(enc_ctx->channel_layout);
+        enc_ctx->frame_size = nb_samples;
+        stream->time_base = audio_time_base;
+
+        cvt_frame = av_frame_alloc();
+        cvt_frame->channels = enc_ctx->channels;
+        cvt_frame->channel_layout = enc_ctx->channel_layout;
+        cvt_frame->format = sample_fmt;
+        cvt_frame->nb_samples = nb_samples;
+        av_frame_get_buffer(cvt_frame, 0);
+        av_frame_make_writable(cvt_frame);
+
+        if (fmt_ctx->oformat->flags & AVFMT_GLOBALHEADER)
+            enc_ctx->flags |= AV_CODEC_FLAG_GLOBAL_HEADER;
+
+        ex.ck(avcodec_open2(enc_ctx, codec, NULL), AO2);
+        ex.ck(avcodec_parameters_from_context(stream->codecpar, enc_ctx), APFC);
+
+        opened = true;
+    }
+    catch (const Exception& e) {
+        std::stringstream str;
+        str << "AudioStream constructor exception: " << e.what();
+        if (infoCallback) infoCallback(str.str());
+        else std::cout << str.str() << std::endl;
+        close();
+    }
+}
+
+bool Encoder::cmpFrame(AVFrame* frame)
+{
+    if (mediaType == AVMEDIA_TYPE_VIDEO)
+        return (frame->width == width && frame->height == height && frame->format == pix_fmt);
+    if (mediaType == AVMEDIA_TYPE_AUDIO)
+        return (frame->channels == channels && frame->channel_layout == channel_layout &&
+            frame->nb_samples == nb_samples && frame->format == sample_fmt);
+
+    return false;
+}
+
+int Encoder::encode(Frame& f)
+{
+    int ret = 0;
+
+    try {
+
+        f.set_pts(stream);
+        AVFrame* frame = f.m_frame;
+
+        if (frame) {
+            if (mediaType == AVMEDIA_TYPE_VIDEO && !cmpFrame(frame)) {
+                if (!sws_ctx) {
+                    ex.ck(sws_ctx = sws_getContext(frame->width, frame->height, (AVPixelFormat)frame->format,
+                        enc_ctx->width, enc_ctx->height, AV_PIX_FMT_YUV420P, SWS_BICUBIC, NULL, NULL, NULL), SGC);
+                }
+
+                ex.ck(sws_scale(sws_ctx, frame->data, frame->linesize, 0, enc_ctx->height,
+                    cvt_frame->data, cvt_frame->linesize), SS);
+
+                cvt_frame->pts = av_rescale_q(frame->pts, video_time_base, enc_ctx->time_base);
+                frame = cvt_frame;
+            }
+
+            if (mediaType == AVMEDIA_TYPE_AUDIO && !cmpFrame(frame)) {
+                if (!swr_ctx) {
+                    ex.ck(swr_ctx = swr_alloc(), SA);
+                    av_opt_set_int(swr_ctx, "in_channel_count", frame->channels, 0);
+                    av_opt_set_int(swr_ctx, "out_channel_count", channels, 0);
+                    av_opt_set_channel_layout(swr_ctx, "in_channel_layout", frame->channel_layout, 0);
+                    av_opt_set_channel_layout(swr_ctx, "out_channel_layout", channel_layout, 0);
+                    av_opt_set_int(swr_ctx, "in_sample_rate", frame->sample_rate, 0);
+                    av_opt_set_int(swr_ctx, "out_sample_rate", sample_rate, 0);
+                    av_opt_set_sample_fmt(swr_ctx, "in_sample_fmt", (AVSampleFormat)frame->format, 0);
+                    av_opt_set_sample_fmt(swr_ctx, "out_sample_fmt", sample_fmt, 0);
+                    ex.ck(swr_init(swr_ctx), SI);
+                }
+
+                ex.ck(swr_convert(swr_ctx, cvt_frame->data, cvt_frame->nb_samples, (const uint8_t**)frame->data, frame->nb_samples), SC);
+
+                cvt_frame->pts = av_rescale_q(total_samples, av_make_q(1, enc_ctx->sample_rate), enc_ctx->time_base);
+                cvt_frame->sample_rate = sample_rate;
+                total_samples += nb_samples;
+                frame = cvt_frame;
+            }
+
+            if (hw_device_type != AV_HWDEVICE_TYPE_NONE) {
+                av_frame_copy_props(hw_frame, frame);
+                ex.ck(av_hwframe_transfer_data(hw_frame, frame, 0), AHTD);
+                ex.ck(avcodec_send_frame(enc_ctx, hw_frame), ASF);
+            }
+            else {
+                ex.ck(avcodec_send_frame(enc_ctx, frame), "avcodec_send_frame");
+            }
+        }
+        else {
+            ex.ck(ret = avcodec_send_frame(enc_ctx, NULL), "avcodec_send_frame");
+        }
+
+        while (ret >= 0) {
+            ret = avcodec_receive_packet(enc_ctx, pkt);
+            if (ret == AVERROR(EAGAIN) || ret == AVERROR_EOF)
+                break;
+            else if (ret < 0) 
+                ex.ck(ret, CmdTag::ARP);
+
+            pkt->stream_index = stream->index;
+
+            AVPacket* tmp = av_packet_alloc();
+
+            // needed to prevent corruption in dts
+            if (pkt->dts > pkt->pts) 
+                pkt->dts = pkt->pts - 2;
+
+            tmp = av_packet_clone(pkt);
+
+            if (first_pass) {
+                pts_offset = tmp->pts;
+                first_pass = false;
+            }
+            tmp->pts -= pts_offset;
+            tmp->dts -= pts_offset;
+
+            writer->write(tmp);
+
+        }
+    }
+    catch (const Exception& e) {
+        if (strcmp(e.what(), "End of file")) {
+            std::stringstream str;
+            str << strMediaType << " encode exception: " << e.what(); 
+            if (infoCallback) infoCallback(str.str());
+            else std::cout << str.str() << std::endl;
+        }
+    }
+
+    return ret;
+}
+
+
+}
```

### Comparing `avio-2.1.7/src/Exception.cpp` & `avio-2.1.8/src/Exception.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Filter.cpp` & `avio-2.1.8/src/Filter.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Frame.cpp` & `avio-2.1.8/src/Frame.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Pipe.cpp` & `avio-2.1.8/src/Pipe.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Player.cpp` & `avio-2.1.8/src/Player.cpp`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-/********************************************************************
-* libavio//src/Player.cpp
-*
-* Copyright (c) 2023  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#include <algorithm>
-#include "Player.h"
-#include "avio.h"
-
-namespace avio
-{
-
-bool Player::isPaused()
-{
-    bool result = false;
-    if (display) result = display->paused;
-    return result;
-}
-
-void Player::setMute(bool arg)
-{
-    mute = arg;
-    if (display) display->mute = arg;
-}
-
-void Player::setVolume(int arg)
-{
-    volume = arg;
-    if (display) display->volume = (float)arg / 100.0f;
-}
-
-void Player::togglePaused()
-{
-    if (display) display->togglePause();
-}
-
-void Player::seek(float arg)
-{
-    if (reader) reader->request_seek(arg);
-}
-
-void Player::togglePiping(const std::string& filename)
-{
-    if (reader) {
-        reader->pipe_out_filename = filename;
-        reader->request_pipe_write = !reader->request_pipe_write;
-    }
-}
-
-void Player::toggleEncoding(const std::string& filename)
-{
-    if (writer) {
-        writer->filename = filename;
-        writer->enabled = !writer->enabled;
-    }
-}
-
-void Player::toggleRecording(const std::string& filename)
-{
-    if (post_encode) {
-        toggleEncoding(filename);
-    }
-    else {
-        togglePiping(filename);
-    }
-}
-
-bool Player::isPiping()
-{
-    bool result = false;
-    if (reader) result = reader->request_pipe_write;
-    return result;
-}
-
-bool Player::isEncoding()
-{
-    bool result = false;
-    if (writer) result = writer->enabled;
-    return result;
-}
-
-bool Player::isRecording()
-{
-    if (post_encode)
-        return isEncoding();
-    else
-        return isPiping();
-}
-
-void Player::clear_queues()
-{
-    if (reader->vpq)  reader->vpq->clear();
-    if (reader->apq)  reader->apq->clear();
-    if (videoDecoder) videoDecoder->frame_q->clear();
-    if (videoFilter)  videoFilter->frame_out_q->clear();
-    if (audioDecoder) audioDecoder->frame_q->clear();
-    if (audioFilter)  audioFilter->frame_out_q->clear();
-}
-
-void Player::clear_decoders()
-{
-    if (videoDecoder) videoDecoder->flush();
-    if (audioDecoder) audioDecoder->flush();
-}
-
-void Player::key_event(int keyCode)
-{
-    SDL_Event event;
-    event.type = SDL_KEYDOWN;
-    event.key.keysym.sym = keyCode;
-    SDL_PushEvent(&event);
-}
-
-bool Player::checkForStreamHeader()
-{
-    std::string tmp = uri;
-
-    if (tmp.rfind("rtsp://", 0) == 0)
-        return true;
-    if (tmp.rfind("http://", 0) == 0)
-        return true;
-    if (tmp.rfind("https://", 0) == 0)
-        return true;
-    if (tmp.rfind("RTSP://", 0) == 0)
-        return true;
-    if (tmp.rfind("HTTP://", 0) == 0)
-        return true;
-    if (tmp.rfind("HTTPS://", 0) == 0)
-        return true;
-
-    return false;
-}
-
-void Player::start()
-{
-    std::thread process_thread([&]() { run(); });
-    process_thread.detach();
-}
-
-void Player::run()
-{
-    std::thread* reader_thread        = nullptr;
-    std::thread* video_decoder_thread = nullptr;
-    std::thread* video_filter_thread  = nullptr;
-    std::thread* video_encoder_thread = nullptr;
-    std::thread* audio_decoder_thread = nullptr;
-    std::thread* audio_filter_thread  = nullptr;
-    std::thread* audio_encoder_thread = nullptr;
-
-    try {
-        running = true;
-
-        vpq_reader  = new Queue<Packet>;
-        vfq_decoder = new Queue<Frame>;
-        vfq_filter  = new Queue<Frame>;
-        vfq_display = new Queue<Frame>;
-        apq_reader  = new Queue<Packet>;
-        afq_decoder = new Queue<Frame>;
-        afq_filter  = new Queue<Frame>;
-        afq_display = new Queue<Frame>;
-
-        reader = new Reader(uri.c_str());
-        reader->errorCallback = errorCallback;
-        reader->infoCallback = infoCallback;
-        reader->disable_video = disable_video;
-        reader->disable_audio = disable_audio;
-        reader->keyframe_cache_size = keyframe_cache_size;
-
-        if (disable_video) {
-            std::cout << "player video disabled" << std::endl;
-        }
-
-        if (disable_audio) {
-            std::cout << "player audio disabled" << std::endl;
-        }
-
-        reader->showStreamParameters();
-
-        writer = new Writer("mp4");
-        writer->infoCallback = infoCallback;
-
-        if (reader->has_video() && !disable_video) {
-            const AVPixFmtDescriptor* desc = av_pix_fmt_desc_get(reader->pix_fmt());
-            if (!desc) throw avio::Exception("No pixel format in video stream");
-
-            reader->vpq = vpq_reader;
-
-            videoDecoder = new Decoder(reader, AVMEDIA_TYPE_VIDEO, hw_device_type);
-            videoDecoder->pkt_q = vpq_reader;
-            videoDecoder->frame_q = vfq_decoder;
-            videoDecoder->errorCallback = errorCallback;
-            videoDecoder->infoCallback = infoCallback;
-
-            videoFilter = new Filter(*videoDecoder, video_filter.c_str());
-            videoFilter->frame_in_q = vfq_decoder;
-            videoFilter->frame_out_q = vfq_filter;
-            videoFilter->errorCallback = errorCallback;
-            videoFilter->infoCallback = infoCallback;
-
-            bool video_encoder_enabled = true;
-            if (video_encoder_enabled) {
-                
-                videoEncoder = new Encoder(writer, AVMEDIA_TYPE_VIDEO);
-                videoEncoder->frame_q = vfq_display;
-                videoEncoder->width = videoFilter->width();
-                videoEncoder->height = videoFilter->height();
-                videoEncoder->frame_rate = reader->frame_rate();
-                videoEncoder->video_time_base = reader->video_time_base();
-                videoEncoder->video_bit_rate = reader->video_bit_rate();
-
-                videoEncoder->gop_size = 30;
-                videoEncoder->profile = "high";
-                videoEncoder->pix_fmt = AV_PIX_FMT_YUV420P;
-
-                if (hw_encoding) {
-                    videoEncoder->hw_video_codec_name = "h264_nvenc";
-                    videoEncoder->hw_device_type = AV_HWDEVICE_TYPE_CUDA;
-                    videoEncoder->hw_pix_fmt = AV_PIX_FMT_CUDA;
-                    videoEncoder->sw_pix_fmt = AV_PIX_FMT_YUV420P;
-                }
-
-                videoEncoder->infoCallback = infoCallback;
-            }
-        }
-
-        if (reader->has_audio() && !disable_audio) {
-            reader->apq = apq_reader;
-
-            audioDecoder = new Decoder(reader, AVMEDIA_TYPE_AUDIO);
-            audioDecoder->pkt_q = apq_reader;
-            audioDecoder->frame_q = afq_decoder;
-            audioDecoder->errorCallback = errorCallback;
-            audioDecoder->infoCallback = infoCallback;
-
-            audioFilter = new Filter(*audioDecoder, audio_filter.c_str());
-            audioFilter->frame_in_q = afq_decoder;
-            audioFilter->frame_out_q = afq_filter;
-            audioFilter->errorCallback = errorCallback;
-            audioFilter->infoCallback = infoCallback;
-
-            bool audio_encoder_enabled = true;
-            if (audio_encoder_enabled) {
-                audioEncoder = new Encoder(writer, AVMEDIA_TYPE_AUDIO);
-                audioEncoder->frame_q = afq_display;
-                audioEncoder->sample_fmt = AV_SAMPLE_FMT_FLTP;
-                audioEncoder->audio_bit_rate = reader->audio_bit_rate();
-                audioEncoder->sample_rate = reader->sample_rate();
-                audioEncoder->audio_time_base = reader->audio_time_base();
-                audioEncoder->nb_samples = reader->frame_size();
-                audioEncoder->channels = reader->channels();
-                if (audioEncoder->channels = 1)
-                    audioEncoder->set_channel_layout_mono();
-                else 
-                    audioEncoder->set_channel_layout_stereo();
-                audioEncoder->infoCallback = infoCallback;
-            }
-        }
-
-        if (checkForStreamHeader()) {
-            if (vpq_size) reader->apq_max_size = vpq_size;
-            if (apq_size) reader->vpq_max_size = vpq_size;
-        }
-
-        reader_thread = new std::thread(read, reader, this);
-        if (videoDecoder) video_decoder_thread = new std::thread(decode, videoDecoder);
-        if (videoFilter)  video_filter_thread  = new std::thread(filter, videoFilter);
-        if (videoEncoder) video_encoder_thread = new std::thread(write, writer, videoEncoder);
-        if (audioDecoder) audio_decoder_thread = new std::thread(decode, audioDecoder);
-        if (audioFilter)  audio_filter_thread  = new std::thread(filter, audioFilter);
-        if (audioEncoder) audio_encoder_thread = new std::thread(write, writer, audioEncoder);
-
-        display = new Display(reader, this);
-        if (videoFilter) {
-            display->vfq_in = videoFilter->frame_out_q;
-            if (videoEncoder)
-                display->vfq_out = vfq_display;
-        }
-        if (audioFilter) {
-            display->afq_in = audioFilter->frame_out_q;
-            display->initAudio(audioFilter);
-            if (audioEncoder)
-                display->afq_out = afq_display;
-        }
-        display->mute = mute;
-        display->volume = (float)volume / 100.0f;
-        display->hWnd = hWnd;
-
-        if (cbMediaPlayingStarted) cbMediaPlayingStarted(reader->duration());
-        display->display();
-
-        if (isRecording()) 
-            toggleRecording("");
-
-        running = false;
-    }
-    catch (const Exception& e) {
-        if (errorCallback)
-            errorCallback(e.what());
-        else 
-            std::cout << e.what() << std::endl;
-        running = false;
-    }
-    
-    if (reader) {
-        if (reader->vpq) reader->vpq->close();
-        if (reader->apq) reader->apq->close();
-    }
-
-    if (reader_thread) reader_thread->join();
-    if (video_decoder_thread) video_decoder_thread->join();
-    if (video_filter_thread)  video_filter_thread->join();
-    if (video_encoder_thread) video_encoder_thread->join();
-    if (audio_decoder_thread) audio_decoder_thread->join();
-    if (audio_filter_thread)  audio_filter_thread->join();
-    if (audio_encoder_thread) audio_encoder_thread->join();
-
-    if (reader_thread) delete reader_thread;
-    if (video_decoder_thread) delete video_decoder_thread;
-    if (video_filter_thread)  delete video_filter_thread;
-    if (video_encoder_thread) delete video_encoder_thread;
-    if (audio_decoder_thread) delete audio_decoder_thread;
-    if (audio_filter_thread)  delete audio_filter_thread;
-    if (audio_encoder_thread) delete audio_encoder_thread;
-
-    if (reader)       delete reader;
-    if (writer)       delete writer;
-    if (videoFilter)  delete videoFilter;
-    if (videoDecoder) delete videoDecoder;
-    if (videoEncoder) delete videoEncoder;
-    if (audioFilter)  delete audioFilter;
-    if (audioDecoder) delete audioDecoder;
-    if (audioEncoder) delete audioEncoder;
-    if (display)      delete display;
-
-    if (vpq_reader)  delete  vpq_reader;  
-    if (vfq_decoder) delete  vfq_decoder;
-    if (vfq_filter)  delete  vfq_filter;
-    if (vfq_display) delete  vfq_display;
-    if (apq_reader)  delete  apq_reader;
-    if (afq_decoder) delete  afq_decoder;
-    if (afq_filter)  delete  afq_filter;
-    if (afq_display) delete  afq_display;
-
-    if (cbMediaPlayingStopped) cbMediaPlayingStopped();
-    
-}
-
+/********************************************************************
+* libavio//src/Player.cpp
+*
+* Copyright (c) 2023  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#include <algorithm>
+#include "Player.h"
+#include "avio.h"
+
+namespace avio
+{
+
+bool Player::isPaused()
+{
+    bool result = false;
+    if (display) result = display->paused;
+    return result;
+}
+
+void Player::setMute(bool arg)
+{
+    mute = arg;
+    if (display) display->mute = arg;
+}
+
+void Player::setVolume(int arg)
+{
+    volume = arg;
+    if (display) display->volume = (float)arg / 100.0f;
+}
+
+void Player::togglePaused()
+{
+    if (display) display->togglePause();
+}
+
+void Player::seek(float arg)
+{
+    if (reader) reader->request_seek(arg);
+}
+
+void Player::togglePiping(const std::string& filename)
+{
+    if (reader) {
+        reader->pipe_out_filename = filename;
+        reader->request_pipe_write = !reader->request_pipe_write;
+    }
+}
+
+void Player::toggleEncoding(const std::string& filename)
+{
+    if (writer) {
+        writer->filename = filename;
+        writer->enabled = !writer->enabled;
+    }
+}
+
+void Player::toggleRecording(const std::string& filename)
+{
+    if (post_encode) {
+        toggleEncoding(filename);
+    }
+    else {
+        togglePiping(filename);
+    }
+}
+
+bool Player::isPiping()
+{
+    bool result = false;
+    if (reader) result = reader->request_pipe_write;
+    return result;
+}
+
+bool Player::isEncoding()
+{
+    bool result = false;
+    if (writer) result = writer->enabled;
+    return result;
+}
+
+bool Player::isRecording()
+{
+    if (post_encode)
+        return isEncoding();
+    else
+        return isPiping();
+}
+
+void Player::clear_queues()
+{
+    if (reader->vpq)  reader->vpq->clear();
+    if (reader->apq)  reader->apq->clear();
+    if (videoDecoder) videoDecoder->frame_q->clear();
+    if (videoFilter)  videoFilter->frame_out_q->clear();
+    if (audioDecoder) audioDecoder->frame_q->clear();
+    if (audioFilter)  audioFilter->frame_out_q->clear();
+}
+
+void Player::clear_decoders()
+{
+    if (videoDecoder) videoDecoder->flush();
+    if (audioDecoder) audioDecoder->flush();
+}
+
+void Player::key_event(int keyCode)
+{
+    SDL_Event event;
+    event.type = SDL_KEYDOWN;
+    event.key.keysym.sym = keyCode;
+    SDL_PushEvent(&event);
+}
+
+bool Player::checkForStreamHeader()
+{
+    std::string tmp = uri;
+
+    if (tmp.rfind("rtsp://", 0) == 0)
+        return true;
+    if (tmp.rfind("http://", 0) == 0)
+        return true;
+    if (tmp.rfind("https://", 0) == 0)
+        return true;
+    if (tmp.rfind("RTSP://", 0) == 0)
+        return true;
+    if (tmp.rfind("HTTP://", 0) == 0)
+        return true;
+    if (tmp.rfind("HTTPS://", 0) == 0)
+        return true;
+
+    return false;
+}
+
+void Player::start()
+{
+    std::thread process_thread([&]() { run(); });
+    process_thread.detach();
+}
+
+void Player::run()
+{
+    std::thread* reader_thread        = nullptr;
+    std::thread* video_decoder_thread = nullptr;
+    std::thread* video_filter_thread  = nullptr;
+    std::thread* video_encoder_thread = nullptr;
+    std::thread* audio_decoder_thread = nullptr;
+    std::thread* audio_filter_thread  = nullptr;
+    std::thread* audio_encoder_thread = nullptr;
+
+    try {
+        running = true;
+
+        vpq_reader  = new Queue<Packet>;
+        vfq_decoder = new Queue<Frame>;
+        vfq_filter  = new Queue<Frame>;
+        vfq_display = new Queue<Frame>;
+        apq_reader  = new Queue<Packet>;
+        afq_decoder = new Queue<Frame>;
+        afq_filter  = new Queue<Frame>;
+        afq_display = new Queue<Frame>;
+
+        reader = new Reader(uri.c_str());
+        reader->errorCallback = errorCallback;
+        reader->infoCallback = infoCallback;
+        reader->disable_video = disable_video;
+        reader->disable_audio = disable_audio;
+        reader->keyframe_cache_size = keyframe_cache_size;
+
+        if (disable_video) {
+            std::cout << "player video disabled" << std::endl;
+        }
+
+        if (disable_audio) {
+            std::cout << "player audio disabled" << std::endl;
+        }
+
+        reader->showStreamParameters();
+
+        writer = new Writer("mp4");
+        writer->infoCallback = infoCallback;
+
+        if (reader->has_video() && !disable_video) {
+            const AVPixFmtDescriptor* desc = av_pix_fmt_desc_get(reader->pix_fmt());
+            if (!desc) throw avio::Exception("No pixel format in video stream");
+
+            reader->vpq = vpq_reader;
+
+            videoDecoder = new Decoder(reader, AVMEDIA_TYPE_VIDEO, hw_device_type);
+            videoDecoder->pkt_q = vpq_reader;
+            videoDecoder->frame_q = vfq_decoder;
+            videoDecoder->errorCallback = errorCallback;
+            videoDecoder->infoCallback = infoCallback;
+
+            videoFilter = new Filter(*videoDecoder, video_filter.c_str());
+            videoFilter->frame_in_q = vfq_decoder;
+            videoFilter->frame_out_q = vfq_filter;
+            videoFilter->errorCallback = errorCallback;
+            videoFilter->infoCallback = infoCallback;
+
+            bool video_encoder_enabled = true;
+            if (video_encoder_enabled) {
+                
+                videoEncoder = new Encoder(writer, AVMEDIA_TYPE_VIDEO);
+                videoEncoder->frame_q = vfq_display;
+                videoEncoder->width = videoFilter->width();
+                videoEncoder->height = videoFilter->height();
+                videoEncoder->frame_rate = reader->frame_rate();
+                videoEncoder->video_time_base = reader->video_time_base();
+                videoEncoder->video_bit_rate = reader->video_bit_rate();
+
+                videoEncoder->gop_size = 30;
+                videoEncoder->profile = "high";
+                videoEncoder->pix_fmt = AV_PIX_FMT_YUV420P;
+
+                if (hw_encoding) {
+                    videoEncoder->hw_video_codec_name = "h264_nvenc";
+                    videoEncoder->hw_device_type = AV_HWDEVICE_TYPE_CUDA;
+                    videoEncoder->hw_pix_fmt = AV_PIX_FMT_CUDA;
+                    videoEncoder->sw_pix_fmt = AV_PIX_FMT_YUV420P;
+                }
+
+                videoEncoder->infoCallback = infoCallback;
+            }
+        }
+
+        if (reader->has_audio() && !disable_audio) {
+            reader->apq = apq_reader;
+
+            audioDecoder = new Decoder(reader, AVMEDIA_TYPE_AUDIO);
+            audioDecoder->pkt_q = apq_reader;
+            audioDecoder->frame_q = afq_decoder;
+            audioDecoder->errorCallback = errorCallback;
+            audioDecoder->infoCallback = infoCallback;
+
+            audioFilter = new Filter(*audioDecoder, audio_filter.c_str());
+            audioFilter->frame_in_q = afq_decoder;
+            audioFilter->frame_out_q = afq_filter;
+            audioFilter->errorCallback = errorCallback;
+            audioFilter->infoCallback = infoCallback;
+
+            bool audio_encoder_enabled = true;
+            if (audio_encoder_enabled) {
+                audioEncoder = new Encoder(writer, AVMEDIA_TYPE_AUDIO);
+                audioEncoder->frame_q = afq_display;
+                audioEncoder->sample_fmt = AV_SAMPLE_FMT_FLTP;
+                audioEncoder->audio_bit_rate = reader->audio_bit_rate();
+                audioEncoder->sample_rate = reader->sample_rate();
+                audioEncoder->audio_time_base = reader->audio_time_base();
+                audioEncoder->nb_samples = reader->frame_size();
+                audioEncoder->channels = reader->channels();
+                if (audioEncoder->channels = 1)
+                    audioEncoder->set_channel_layout_mono();
+                else 
+                    audioEncoder->set_channel_layout_stereo();
+                audioEncoder->infoCallback = infoCallback;
+            }
+        }
+
+        if (checkForStreamHeader()) {
+            if (vpq_size) reader->apq_max_size = vpq_size;
+            if (apq_size) reader->vpq_max_size = vpq_size;
+        }
+
+        reader_thread = new std::thread(read, reader, this);
+        if (videoDecoder) video_decoder_thread = new std::thread(decode, videoDecoder);
+        if (videoFilter)  video_filter_thread  = new std::thread(filter, videoFilter);
+        if (videoEncoder) video_encoder_thread = new std::thread(write, writer, videoEncoder);
+        if (audioDecoder) audio_decoder_thread = new std::thread(decode, audioDecoder);
+        if (audioFilter)  audio_filter_thread  = new std::thread(filter, audioFilter);
+        if (audioEncoder) audio_encoder_thread = new std::thread(write, writer, audioEncoder);
+
+        display = new Display(reader, this);
+        if (videoFilter) {
+            display->vfq_in = videoFilter->frame_out_q;
+            if (videoEncoder)
+                display->vfq_out = vfq_display;
+        }
+        if (audioFilter) {
+            display->afq_in = audioFilter->frame_out_q;
+            display->initAudio(audioFilter);
+            if (audioEncoder)
+                display->afq_out = afq_display;
+        }
+        display->mute = mute;
+        display->volume = (float)volume / 100.0f;
+        display->hWnd = hWnd;
+
+        if (cbMediaPlayingStarted) cbMediaPlayingStarted(reader->duration());
+        display->display();
+
+        if (isRecording()) 
+            toggleRecording("");
+
+        running = false;
+    }
+    catch (const Exception& e) {
+        if (errorCallback)
+            errorCallback(e.what());
+        else 
+            std::cout << e.what() << std::endl;
+        running = false;
+    }
+    
+    if (reader) {
+        if (reader->vpq) reader->vpq->close();
+        if (reader->apq) reader->apq->close();
+    }
+
+    if (reader_thread) reader_thread->join();
+    if (video_decoder_thread) video_decoder_thread->join();
+    if (video_filter_thread)  video_filter_thread->join();
+    if (video_encoder_thread) video_encoder_thread->join();
+    if (audio_decoder_thread) audio_decoder_thread->join();
+    if (audio_filter_thread)  audio_filter_thread->join();
+    if (audio_encoder_thread) audio_encoder_thread->join();
+
+    if (reader_thread) delete reader_thread;
+    if (video_decoder_thread) delete video_decoder_thread;
+    if (video_filter_thread)  delete video_filter_thread;
+    if (video_encoder_thread) delete video_encoder_thread;
+    if (audio_decoder_thread) delete audio_decoder_thread;
+    if (audio_filter_thread)  delete audio_filter_thread;
+    if (audio_encoder_thread) delete audio_encoder_thread;
+
+    if (reader)       delete reader;
+    if (writer)       delete writer;
+    if (videoFilter)  delete videoFilter;
+    if (videoDecoder) delete videoDecoder;
+    if (videoEncoder) delete videoEncoder;
+    if (audioFilter)  delete audioFilter;
+    if (audioDecoder) delete audioDecoder;
+    if (audioEncoder) delete audioEncoder;
+    if (display)      delete display;
+
+    if (vpq_reader)  delete  vpq_reader;  
+    if (vfq_decoder) delete  vfq_decoder;
+    if (vfq_filter)  delete  vfq_filter;
+    if (vfq_display) delete  vfq_display;
+    if (apq_reader)  delete  apq_reader;
+    if (afq_decoder) delete  afq_decoder;
+    if (afq_filter)  delete  afq_filter;
+    if (afq_display) delete  afq_display;
+
+    if (cbMediaPlayingStopped) cbMediaPlayingStopped();
+    
+}
+
 }
```

### Comparing `avio-2.1.7/src/Reader.cpp` & `avio-2.1.8/src/Reader.cpp`

 * *Files identical despite different names*

### Comparing `avio-2.1.7/src/Writer.cpp` & `avio-2.1.8/src/Writer.cpp`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-/********************************************************************
-* libavio/src/Writer.cpp
-*
-* Copyright (c) 2023  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#include "Writer.h"
-#include "Encoder.h"
-
-namespace avio
-{
-
-Writer::Writer(const std::string& format) : m_format(format)
-{
-
-}
-
-Writer::~Writer()
-{
-
-}
-
-void Writer::init()
-{
-    ex.ck(avformat_alloc_output_context2(&fmt_ctx, NULL, m_format.c_str(), NULL), AAOC2);
-}
-
-void Writer::open()
-{
-    std::unique_lock<std::mutex> lock(mutex);
-    try {
-        if (getEncoderState() == EncoderState::OPEN && !opened) {
-            if (!(fmt_ctx->oformat->flags & AVFMT_NOFILE))
-                ex.ck(avio_open(&fmt_ctx->pb, filename.c_str(), AVIO_FLAG_WRITE), AO);
-
-            ex.ck(avformat_write_header(fmt_ctx, NULL), AWH);
-            opened = true;
-        }
-    }
-    catch (const Exception& e) {
-        std::stringstream str;
-        str << "Writer::open exception: " << e.what();
-        if (infoCallback) infoCallback(str.str());
-        else std::cout << str.str() << std::endl;
-    }
-}
-
-void Writer::write(AVPacket* pkt)
-{
-    std::unique_lock<std::mutex> lock(mutex);
-    try {
-        ex.ck(av_interleaved_write_frame(fmt_ctx, pkt), AIWF);
-    }
-    catch (const Exception& e) {
-        std::stringstream str;
-        str << "Writer::write exception: " << e.what();
-        if (infoCallback) infoCallback(str.str());
-        else std::cout << str.str() << std::endl;
-    }
-}
-
-void Writer::close()
-{
-    std::unique_lock<std::mutex> lock(mutex);
-    try {
-        if (getEncoderState() == EncoderState::CLOSED && opened) {
-            ex.ck(av_write_trailer(fmt_ctx), AWT);
-
-            if (!(fmt_ctx->oformat->flags & AVFMT_NOFILE))
-                ex.ck(avio_closep(&fmt_ctx->pb), AC);
-
-            avformat_free_context(fmt_ctx);
-            fmt_ctx = NULL;
-
-            opened = false;
-        }
-    }
-    catch (const Exception& e) {
-        std::stringstream str;
-        str << "Writer::close exception: " << e.what();
-        if (infoCallback) infoCallback(str.str());
-        else std::cout << str.str() << std::endl;
-    }
-}
-
-EncoderState Writer::getEncoderState()
-{
-    bool videoEncoderOpen = false;
-    bool videoEncoderClosed = false;
-    if (videoEncoder) {
-        if (((Encoder*)videoEncoder)->opened)
-            videoEncoderOpen = true;
-        else
-            videoEncoderClosed = true;
-    }
-
-    bool audioEncoderOpen = false;
-    bool audioEncoderClosed = false;
-    if (audioEncoder) {
-        if (((Encoder*)audioEncoder)->opened)
-            audioEncoderOpen = true;
-        else
-            audioEncoderClosed = true;
-    }
-
-    if (videoEncoderOpen && audioEncoderOpen)
-        return EncoderState::OPEN;
-    if (videoEncoderOpen && !audioEncoder)
-        return EncoderState::OPEN;
-    if (!videoEncoder && audioEncoderOpen)
-        return EncoderState::OPEN;
-
-    if (videoEncoderClosed && audioEncoderClosed)
-        return EncoderState::CLOSED;
-    if (videoEncoderClosed && !audioEncoder)
-        return EncoderState::CLOSED;
-    if (!videoEncoder && audioEncoderClosed)
-        return EncoderState::CLOSED;
-
-    return EncoderState::MIXED;
-
-}
-
-}
+/********************************************************************
+* libavio/src/Writer.cpp
+*
+* Copyright (c) 2023  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#include "Writer.h"
+#include "Encoder.h"
+
+namespace avio
+{
+
+Writer::Writer(const std::string& format) : m_format(format)
+{
+
+}
+
+Writer::~Writer()
+{
+
+}
+
+void Writer::init()
+{
+    ex.ck(avformat_alloc_output_context2(&fmt_ctx, NULL, m_format.c_str(), NULL), AAOC2);
+}
+
+void Writer::open()
+{
+    std::unique_lock<std::mutex> lock(mutex);
+    try {
+        if (getEncoderState() == EncoderState::OPEN && !opened) {
+            if (!(fmt_ctx->oformat->flags & AVFMT_NOFILE))
+                ex.ck(avio_open(&fmt_ctx->pb, filename.c_str(), AVIO_FLAG_WRITE), AO);
+
+            ex.ck(avformat_write_header(fmt_ctx, NULL), AWH);
+            opened = true;
+        }
+    }
+    catch (const Exception& e) {
+        std::stringstream str;
+        str << "Writer::open exception: " << e.what();
+        if (infoCallback) infoCallback(str.str());
+        else std::cout << str.str() << std::endl;
+    }
+}
+
+void Writer::write(AVPacket* pkt)
+{
+    std::unique_lock<std::mutex> lock(mutex);
+    try {
+        ex.ck(av_interleaved_write_frame(fmt_ctx, pkt), AIWF);
+    }
+    catch (const Exception& e) {
+        std::stringstream str;
+        str << "Writer::write exception: " << e.what();
+        if (infoCallback) infoCallback(str.str());
+        else std::cout << str.str() << std::endl;
+    }
+}
+
+void Writer::close()
+{
+    std::unique_lock<std::mutex> lock(mutex);
+    try {
+        if (getEncoderState() == EncoderState::CLOSED && opened) {
+            ex.ck(av_write_trailer(fmt_ctx), AWT);
+
+            if (!(fmt_ctx->oformat->flags & AVFMT_NOFILE))
+                ex.ck(avio_closep(&fmt_ctx->pb), AC);
+
+            avformat_free_context(fmt_ctx);
+            fmt_ctx = NULL;
+
+            opened = false;
+        }
+    }
+    catch (const Exception& e) {
+        std::stringstream str;
+        str << "Writer::close exception: " << e.what();
+        if (infoCallback) infoCallback(str.str());
+        else std::cout << str.str() << std::endl;
+    }
+}
+
+EncoderState Writer::getEncoderState()
+{
+    bool videoEncoderOpen = false;
+    bool videoEncoderClosed = false;
+    if (videoEncoder) {
+        if (((Encoder*)videoEncoder)->opened)
+            videoEncoderOpen = true;
+        else
+            videoEncoderClosed = true;
+    }
+
+    bool audioEncoderOpen = false;
+    bool audioEncoderClosed = false;
+    if (audioEncoder) {
+        if (((Encoder*)audioEncoder)->opened)
+            audioEncoderOpen = true;
+        else
+            audioEncoderClosed = true;
+    }
+
+    if (videoEncoderOpen && audioEncoderOpen)
+        return EncoderState::OPEN;
+    if (videoEncoderOpen && !audioEncoder)
+        return EncoderState::OPEN;
+    if (!videoEncoder && audioEncoderOpen)
+        return EncoderState::OPEN;
+
+    if (videoEncoderClosed && audioEncoderClosed)
+        return EncoderState::CLOSED;
+    if (videoEncoderClosed && !audioEncoder)
+        return EncoderState::CLOSED;
+    if (!videoEncoder && audioEncoderClosed)
+        return EncoderState::CLOSED;
+
+    return EncoderState::MIXED;
+
+}
+
+}
```

### Comparing `avio-2.1.7/src/avio.cpp` & `avio-2.1.8/src/avio.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-/********************************************************************
-* libavio/src/avio.cpp
-*
-* Copyright (c) 2023  Stephen Rhodes
-*
-* Licensed under the Apache License, Version 2.0 (the "License");
-* you may not use this file except in compliance with the License.
-* You may obtain a copy of the License at
-*
-*    http://www.apache.org/licenses/LICENSE-2.0
-*
-* Unless required by applicable law or agreed to in writing, software
-* distributed under the License is distributed on an "AS IS" BASIS,
-* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-* See the License for the specific language governing permissions and
-* limitations under the License.
-*
-*********************************************************************/
-
-#include <pybind11/pybind11.h>
-#include <pybind11/stl.h>
-#include <pybind11/functional.h>
-#include "avio.h"
-#include "Display.h"
-#include "Frame.h"
-
-namespace py = pybind11;
-
-namespace avio
-{
-
-PYBIND11_MODULE(avio, m)
-{
-    m.doc() = "pybind11 av plugin";
-    py::class_<Player>(m, "Player")
-        .def(py::init<>())
-        .def("run", &Player::run)
-        .def("start", &Player::start)
-        .def("seek", &Player::seek)
-        .def("isPaused", &Player::isPaused)
-        .def("isPiping", &Player::isPiping)
-        .def("isRecording", &Player::isRecording)
-        .def("isEncoding", &Player::isEncoding)
-        .def("setVolume", &Player::setVolume)
-        .def("setMute", &Player::setMute)
-        .def("togglePaused", &Player::togglePaused)
-        .def("togglePiping", &Player::togglePiping)
-        .def("toggleEncoding", &Player::toggleEncoding)
-        .def("toggleRecording", &Player::toggleRecording)
-        .def("getVideoCodec", &Player::getVideoCodec)
-        .def("getVideoWidth", &Player::getVideoWidth)
-        .def("getVideoHeight", &Player::getVideoHeight)
-        .def("getVideoFrameRate", &Player::getVideoFrameRate)
-        .def("getVideoBitrate", &Player::getVideoBitrate)
-        .def_readwrite("running", &Player::running)
-        .def_readwrite("width", &Player::width)
-        .def_readwrite("height", &Player::height)
-        .def_readwrite("disable_video", &Player::disable_video)
-        .def_readwrite("disable_audio", &Player::disable_audio)
-        .def_readwrite("progressCallback", &Player::progressCallback)
-        .def_readwrite("renderCallback", &Player::renderCallback)
-        .def_readwrite("pythonCallback", &Player::pythonCallback)
-        .def_readwrite("pyAudioCallback", &Player::pyAudioCallback)
-        .def_readwrite("infoCallback", &Player::infoCallback)
-        .def_readwrite("errorCallback", &Player::errorCallback)
-        .def_readwrite("cbMediaPlayingStarted", &Player::cbMediaPlayingStarted)
-        .def_readwrite("cbMediaPlayingStopped", &Player::cbMediaPlayingStopped)
-        .def_readwrite("uri", &Player::uri)
-        .def_readwrite("hWnd", &Player::hWnd)
-        .def_readwrite("vpq_size", &Player::vpq_size)
-        .def_readwrite("apq_size", &Player::apq_size)
-        .def_readwrite("video_filter", &Player::video_filter)
-        .def_readwrite("audio_filter", &Player::audio_filter)
-        .def_readwrite("keyframe_cache_size", &Player::keyframe_cache_size)
-        .def_readwrite("process_pause", &Player::process_pause)
-        .def_readwrite("post_encode", &Player::post_encode)
-        .def_readwrite("hw_encoding", &Player::hw_encoding)
-        .def_readwrite("hw_device_type", &Player::hw_device_type);
-    py::class_<Reader>(m, "Reader")
-        .def(py::init<const char*>())
-        .def("start_time", &Reader::start_time)
-        .def("duration", &Reader::duration)
-        .def("bit_rate", &Reader::bit_rate)
-        .def("has_video", &Reader::has_video)
-        .def("width", &Reader::width)
-        .def("height", &Reader::height)
-        .def("frame_rate", &Reader::frame_rate)
-        .def("pix_fmt", &Reader::pix_fmt)
-        .def("str_pix_fmt", &Reader::str_pix_fmt)
-        .def("video_codec", &Reader::video_codec)
-        .def("str_video_codec", &Reader::str_video_codec)
-        .def("video_bit_rate", &Reader::video_bit_rate)
-        .def("video_time_base", &Reader::video_time_base)
-        .def("has_audio", &Reader::has_audio)
-        .def("channels", &Reader::channels)
-        .def("sample_rate", &Reader::sample_rate)
-        .def("frame_size", &Reader::frame_size)
-        .def("channel_layout", &Reader::channel_layout)
-        .def("str_channel_layout", &Reader::str_channel_layout)
-        .def("sample_format", &Reader::sample_format)
-        .def("str_sample_format", &Reader::str_sample_format)
-        .def("audio_codec", &Reader::audio_codec)
-        .def("str_audio_codec", &Reader::str_audio_codec)
-        .def("audio_bit_rate", &Reader::audio_bit_rate)
-        .def("audio_time_base", &Reader::audio_time_base)
-        .def("request_seek", &Reader::request_seek)
-        .def("start_from", &Reader::start_from)
-        .def("end_at", &Reader::end_at)
-        .def_readwrite("pipe_out_filename", &Reader::pipe_out_filename)
-        .def_readwrite("vpq_max_size", &Reader::vpq_max_size)
-        .def_readwrite("apq_max_size", &Reader::apq_max_size)
-        .def_readwrite("show_video_pkts", &Reader::show_video_pkts)
-        .def_readwrite("show_audio_pkts", &Reader::show_audio_pkts);
-    py::class_<Frame>(m, "Frame", py::buffer_protocol())
-        .def(py::init<>())
-        .def(py::init<const Frame&>())
-        .def("isValid", &Frame::isValid)
-        .def("invalidate", &Frame::invalidate)
-        .def("width", &Frame::width)
-        .def("height", &Frame::height)
-        .def("stride", &Frame::stride)
-        .def("nb_samples", &Frame::nb_samples)
-        .def("sample_rate", &Frame::sample_rate)
-        .def("channels", &Frame::channels)
-        .def_readwrite("m_rts", &Frame::m_rts)
-        .def_buffer([](Frame &m) -> py::buffer_info {
-            if (m.height() == 0 && m.width() == 0) {
-                return py::buffer_info(
-                    m.data(),
-                    sizeof(float),
-                    py::format_descriptor<float>::format(),
-                    1,
-                    { m.nb_samples() * m.channels() },
-                    { sizeof(float) }
-                );
-            }
-            else {
-                py::ssize_t element_size = sizeof(uint8_t);
-                std::string fmt_desc =  py::format_descriptor<uint8_t>::format();
-                std::vector<py::ssize_t> dims = { m.height(), m.width(), 3};
-                py::ssize_t ndim = dims.size();
-                std::vector<py::ssize_t> strides = { sizeof(uint8_t) * m.stride(), (py::ssize_t)(sizeof(uint8_t) * ndim), sizeof(uint8_t) };
-                return py::buffer_info(m.data(), element_size, fmt_desc, ndim, dims, strides);
-            }
-        });
-    py::class_<AVRational>(m, "AVRational")
-        .def(py::init<>())
-        .def_readwrite("num", &AVRational::num)
-        .def_readwrite("den", &AVRational::den);
-    py::enum_<AVMediaType>(m, "AVMediaType")
-        .value("AVMEDIA_TYPE_UNKNOWN", AVMediaType::AVMEDIA_TYPE_UNKNOWN)
-        .value("AVMEDIA_TYPE_VIDEO", AVMediaType::AVMEDIA_TYPE_VIDEO)
-        .value("AVMEDIA_TYPE_AUDIO", AVMediaType::AVMEDIA_TYPE_AUDIO)
-        .export_values();
-    py::enum_<AVPixelFormat>(m, "AVPixelFormat")
-        .value("AV_PIX_FMT_NONE", AVPixelFormat::AV_PIX_FMT_NONE)
-        .value("AV_PIX_FMT_YUV420P", AVPixelFormat::AV_PIX_FMT_YUV420P)
-        .value("AV_PIX_FMT_RGB24", AVPixelFormat::AV_PIX_FMT_RGB24)
-        .value("AV_PIX_FMT_BGR24", AVPixelFormat::AV_PIX_FMT_BGR24)
-        .value("AV_PIX_FMT_NV12", AVPixelFormat::AV_PIX_FMT_NV12)
-        .value("AV_PIX_FMT_NV21", AVPixelFormat::AV_PIX_FMT_NV21)
-        .value("AV_PIX_FMT_RGBA", AVPixelFormat::AV_PIX_FMT_RGBA)
-        .value("AV_PIX_FMT_BGRA", AVPixelFormat::AV_PIX_FMT_BGRA)
-        .value("AV_PIX_FMT_VAAPI", AVPixelFormat::AV_PIX_FMT_VAAPI)
-        .value("AV_PIX_FMT_CUDA", AVPixelFormat::AV_PIX_FMT_CUDA)
-        .value("AV_PIX_FMT_QSV", AVPixelFormat::AV_PIX_FMT_QSV)
-        .value("AV_PIX_FMT_D3D11VA_VLD", AVPixelFormat::AV_PIX_FMT_D3D11VA_VLD)
-        .value("AV_PIX_FMT_VDPAU", AVPixelFormat::AV_PIX_FMT_VDPAU)
-        .value("AV_PIX_FMT_D3D11", AVPixelFormat::AV_PIX_FMT_D3D11)
-        .value("AV_PIX_FMT_OPENCL", AVPixelFormat::AV_PIX_FMT_OPENCL)
-        .value("AV_PIX_FMT_GRAY8", AVPixelFormat::AV_PIX_FMT_GRAY8)
-        .export_values();
-    py::enum_<AVHWDeviceType>(m, "AVHWDeviceType")
-        .value("AV_HWDEVICE_TYPE_NONE", AVHWDeviceType::AV_HWDEVICE_TYPE_NONE)
-        .value("AV_HWDEVICE_TYPE_VDPAU", AVHWDeviceType::AV_HWDEVICE_TYPE_VDPAU)
-        .value("AV_HWDEVICE_TYPE_CUDA", AVHWDeviceType::AV_HWDEVICE_TYPE_CUDA)
-        .value("AV_HWDEVICE_TYPE_VAAPI", AVHWDeviceType::AV_HWDEVICE_TYPE_VAAPI)
-        .value("AV_HWDEVICE_TYPE_DXVA2", AVHWDeviceType::AV_HWDEVICE_TYPE_DXVA2)
-        .value("AV_HWDEVICE_TYPE_QSV", AVHWDeviceType::AV_HWDEVICE_TYPE_QSV)
-        .value("AV_HWDEVICE_TYPE_VIDEOTOOLBOX", AVHWDeviceType::AV_HWDEVICE_TYPE_VIDEOTOOLBOX)
-        .value("AV_HWDEVICE_TYPE_D3D11VA", AVHWDeviceType::AV_HWDEVICE_TYPE_D3D11VA)
-        .value("AV_HWDEVICE_TYPE_DRM", AVHWDeviceType::AV_HWDEVICE_TYPE_DRM)
-        .value("AV_HWDEVICE_TYPE_OPENCL", AVHWDeviceType::AV_HWDEVICE_TYPE_OPENCL)
-        .value("AV_HWDEVICE_TYPE_MEDIACODEC", AVHWDeviceType::AV_HWDEVICE_TYPE_MEDIACODEC)
-        .export_values();
-    py::enum_<AVSampleFormat>(m, "AVSampleFormat")
-        .value("AV_SAMPLE_FMT_NONE", AVSampleFormat::AV_SAMPLE_FMT_NONE)
-        .value("AV_SAMPLE_FMT_U8", AVSampleFormat::AV_SAMPLE_FMT_U8)
-        .value("AV_SAMPLE_FMT_S16", AVSampleFormat::AV_SAMPLE_FMT_S16)
-        .value("AV_SAMPLE_FMT_S32", AVSampleFormat::AV_SAMPLE_FMT_S32)
-        .value("AV_SAMPLE_FMT_FLT", AVSampleFormat::AV_SAMPLE_FMT_FLT)
-        .value("AV_SAMPLE_FMT_DBL", AVSampleFormat::AV_SAMPLE_FMT_DBL)
-        .value("AV_SAMPLE_FMT_U8P", AVSampleFormat::AV_SAMPLE_FMT_U8P)
-        .value("AV_SAMPLE_FMT_S16P", AVSampleFormat::AV_SAMPLE_FMT_S16P)
-        .value("AV_SAMPLE_FMT_S32P", AVSampleFormat::AV_SAMPLE_FMT_S32P)
-        .value("AV_SAMPLE_FMT_FLTP", AVSampleFormat::AV_SAMPLE_FMT_FLTP)
-        .value("AV_SAMPLE_FMT_DBLP", AVSampleFormat::AV_SAMPLE_FMT_DBLP)
-        .value("AV_SAMPLE_FMT_S64", AVSampleFormat::AV_SAMPLE_FMT_S64)
-        .value("AV_SAMPLE_FMT_S64P", AVSampleFormat::AV_SAMPLE_FMT_S64P)
-        .value("AV_SAMPLE_FMT_NB", AVSampleFormat::AV_SAMPLE_FMT_NB)
-        .export_values();
-
-    m.attr("__version__") = "2.1.7";
-
-}
-
+/********************************************************************
+* libavio/src/avio.cpp
+*
+* Copyright (c) 2023  Stephen Rhodes
+*
+* Licensed under the Apache License, Version 2.0 (the "License");
+* you may not use this file except in compliance with the License.
+* You may obtain a copy of the License at
+*
+*    http://www.apache.org/licenses/LICENSE-2.0
+*
+* Unless required by applicable law or agreed to in writing, software
+* distributed under the License is distributed on an "AS IS" BASIS,
+* WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+* See the License for the specific language governing permissions and
+* limitations under the License.
+*
+*********************************************************************/
+
+#include <pybind11/pybind11.h>
+#include <pybind11/stl.h>
+#include <pybind11/functional.h>
+#include "avio.h"
+#include "Display.h"
+#include "Frame.h"
+
+namespace py = pybind11;
+
+namespace avio
+{
+
+PYBIND11_MODULE(avio, m)
+{
+    m.doc() = "pybind11 av plugin";
+    py::class_<Player>(m, "Player")
+        .def(py::init<>())
+        .def("run", &Player::run)
+        .def("start", &Player::start)
+        .def("seek", &Player::seek)
+        .def("isPaused", &Player::isPaused)
+        .def("isPiping", &Player::isPiping)
+        .def("isRecording", &Player::isRecording)
+        .def("isEncoding", &Player::isEncoding)
+        .def("setVolume", &Player::setVolume)
+        .def("setMute", &Player::setMute)
+        .def("togglePaused", &Player::togglePaused)
+        .def("togglePiping", &Player::togglePiping)
+        .def("toggleEncoding", &Player::toggleEncoding)
+        .def("toggleRecording", &Player::toggleRecording)
+        .def("getVideoCodec", &Player::getVideoCodec)
+        .def("getVideoWidth", &Player::getVideoWidth)
+        .def("getVideoHeight", &Player::getVideoHeight)
+        .def("getVideoFrameRate", &Player::getVideoFrameRate)
+        .def("getVideoBitrate", &Player::getVideoBitrate)
+        .def_readwrite("running", &Player::running)
+        .def_readwrite("width", &Player::width)
+        .def_readwrite("height", &Player::height)
+        .def_readwrite("disable_video", &Player::disable_video)
+        .def_readwrite("disable_audio", &Player::disable_audio)
+        .def_readwrite("progressCallback", &Player::progressCallback)
+        .def_readwrite("renderCallback", &Player::renderCallback)
+        .def_readwrite("pythonCallback", &Player::pythonCallback)
+        .def_readwrite("pyAudioCallback", &Player::pyAudioCallback)
+        .def_readwrite("infoCallback", &Player::infoCallback)
+        .def_readwrite("errorCallback", &Player::errorCallback)
+        .def_readwrite("cbMediaPlayingStarted", &Player::cbMediaPlayingStarted)
+        .def_readwrite("cbMediaPlayingStopped", &Player::cbMediaPlayingStopped)
+        .def_readwrite("uri", &Player::uri)
+        .def_readwrite("hWnd", &Player::hWnd)
+        .def_readwrite("vpq_size", &Player::vpq_size)
+        .def_readwrite("apq_size", &Player::apq_size)
+        .def_readwrite("video_filter", &Player::video_filter)
+        .def_readwrite("audio_filter", &Player::audio_filter)
+        .def_readwrite("keyframe_cache_size", &Player::keyframe_cache_size)
+        .def_readwrite("process_pause", &Player::process_pause)
+        .def_readwrite("post_encode", &Player::post_encode)
+        .def_readwrite("hw_encoding", &Player::hw_encoding)
+        .def_readwrite("hw_device_type", &Player::hw_device_type);
+    py::class_<Reader>(m, "Reader")
+        .def(py::init<const char*>())
+        .def("start_time", &Reader::start_time)
+        .def("duration", &Reader::duration)
+        .def("bit_rate", &Reader::bit_rate)
+        .def("has_video", &Reader::has_video)
+        .def("width", &Reader::width)
+        .def("height", &Reader::height)
+        .def("frame_rate", &Reader::frame_rate)
+        .def("pix_fmt", &Reader::pix_fmt)
+        .def("str_pix_fmt", &Reader::str_pix_fmt)
+        .def("video_codec", &Reader::video_codec)
+        .def("str_video_codec", &Reader::str_video_codec)
+        .def("video_bit_rate", &Reader::video_bit_rate)
+        .def("video_time_base", &Reader::video_time_base)
+        .def("has_audio", &Reader::has_audio)
+        .def("channels", &Reader::channels)
+        .def("sample_rate", &Reader::sample_rate)
+        .def("frame_size", &Reader::frame_size)
+        .def("channel_layout", &Reader::channel_layout)
+        .def("str_channel_layout", &Reader::str_channel_layout)
+        .def("sample_format", &Reader::sample_format)
+        .def("str_sample_format", &Reader::str_sample_format)
+        .def("audio_codec", &Reader::audio_codec)
+        .def("str_audio_codec", &Reader::str_audio_codec)
+        .def("audio_bit_rate", &Reader::audio_bit_rate)
+        .def("audio_time_base", &Reader::audio_time_base)
+        .def("request_seek", &Reader::request_seek)
+        .def("start_from", &Reader::start_from)
+        .def("end_at", &Reader::end_at)
+        .def_readwrite("pipe_out_filename", &Reader::pipe_out_filename)
+        .def_readwrite("vpq_max_size", &Reader::vpq_max_size)
+        .def_readwrite("apq_max_size", &Reader::apq_max_size)
+        .def_readwrite("show_video_pkts", &Reader::show_video_pkts)
+        .def_readwrite("show_audio_pkts", &Reader::show_audio_pkts);
+    py::class_<Frame>(m, "Frame", py::buffer_protocol())
+        .def(py::init<>())
+        .def(py::init<const Frame&>())
+        .def("isValid", &Frame::isValid)
+        .def("invalidate", &Frame::invalidate)
+        .def("width", &Frame::width)
+        .def("height", &Frame::height)
+        .def("stride", &Frame::stride)
+        .def("nb_samples", &Frame::nb_samples)
+        .def("sample_rate", &Frame::sample_rate)
+        .def("channels", &Frame::channels)
+        .def_readwrite("m_rts", &Frame::m_rts)
+        .def_buffer([](Frame &m) -> py::buffer_info {
+            if (m.height() == 0 && m.width() == 0) {
+                return py::buffer_info(
+                    m.data(),
+                    sizeof(float),
+                    py::format_descriptor<float>::format(),
+                    1,
+                    { m.nb_samples() * m.channels() },
+                    { sizeof(float) }
+                );
+            }
+            else {
+                py::ssize_t element_size = sizeof(uint8_t);
+                std::string fmt_desc =  py::format_descriptor<uint8_t>::format();
+                std::vector<py::ssize_t> dims = { m.height(), m.width(), 3};
+                py::ssize_t ndim = dims.size();
+                std::vector<py::ssize_t> strides = { sizeof(uint8_t) * m.stride(), (py::ssize_t)(sizeof(uint8_t) * ndim), sizeof(uint8_t) };
+                return py::buffer_info(m.data(), element_size, fmt_desc, ndim, dims, strides);
+            }
+        });
+    py::class_<AVRational>(m, "AVRational")
+        .def(py::init<>())
+        .def_readwrite("num", &AVRational::num)
+        .def_readwrite("den", &AVRational::den);
+    py::enum_<AVMediaType>(m, "AVMediaType")
+        .value("AVMEDIA_TYPE_UNKNOWN", AVMediaType::AVMEDIA_TYPE_UNKNOWN)
+        .value("AVMEDIA_TYPE_VIDEO", AVMediaType::AVMEDIA_TYPE_VIDEO)
+        .value("AVMEDIA_TYPE_AUDIO", AVMediaType::AVMEDIA_TYPE_AUDIO)
+        .export_values();
+    py::enum_<AVPixelFormat>(m, "AVPixelFormat")
+        .value("AV_PIX_FMT_NONE", AVPixelFormat::AV_PIX_FMT_NONE)
+        .value("AV_PIX_FMT_YUV420P", AVPixelFormat::AV_PIX_FMT_YUV420P)
+        .value("AV_PIX_FMT_RGB24", AVPixelFormat::AV_PIX_FMT_RGB24)
+        .value("AV_PIX_FMT_BGR24", AVPixelFormat::AV_PIX_FMT_BGR24)
+        .value("AV_PIX_FMT_NV12", AVPixelFormat::AV_PIX_FMT_NV12)
+        .value("AV_PIX_FMT_NV21", AVPixelFormat::AV_PIX_FMT_NV21)
+        .value("AV_PIX_FMT_RGBA", AVPixelFormat::AV_PIX_FMT_RGBA)
+        .value("AV_PIX_FMT_BGRA", AVPixelFormat::AV_PIX_FMT_BGRA)
+        .value("AV_PIX_FMT_VAAPI", AVPixelFormat::AV_PIX_FMT_VAAPI)
+        .value("AV_PIX_FMT_CUDA", AVPixelFormat::AV_PIX_FMT_CUDA)
+        .value("AV_PIX_FMT_QSV", AVPixelFormat::AV_PIX_FMT_QSV)
+        .value("AV_PIX_FMT_D3D11VA_VLD", AVPixelFormat::AV_PIX_FMT_D3D11VA_VLD)
+        .value("AV_PIX_FMT_VDPAU", AVPixelFormat::AV_PIX_FMT_VDPAU)
+        .value("AV_PIX_FMT_D3D11", AVPixelFormat::AV_PIX_FMT_D3D11)
+        .value("AV_PIX_FMT_OPENCL", AVPixelFormat::AV_PIX_FMT_OPENCL)
+        .value("AV_PIX_FMT_GRAY8", AVPixelFormat::AV_PIX_FMT_GRAY8)
+        .export_values();
+    py::enum_<AVHWDeviceType>(m, "AVHWDeviceType")
+        .value("AV_HWDEVICE_TYPE_NONE", AVHWDeviceType::AV_HWDEVICE_TYPE_NONE)
+        .value("AV_HWDEVICE_TYPE_VDPAU", AVHWDeviceType::AV_HWDEVICE_TYPE_VDPAU)
+        .value("AV_HWDEVICE_TYPE_CUDA", AVHWDeviceType::AV_HWDEVICE_TYPE_CUDA)
+        .value("AV_HWDEVICE_TYPE_VAAPI", AVHWDeviceType::AV_HWDEVICE_TYPE_VAAPI)
+        .value("AV_HWDEVICE_TYPE_DXVA2", AVHWDeviceType::AV_HWDEVICE_TYPE_DXVA2)
+        .value("AV_HWDEVICE_TYPE_QSV", AVHWDeviceType::AV_HWDEVICE_TYPE_QSV)
+        .value("AV_HWDEVICE_TYPE_VIDEOTOOLBOX", AVHWDeviceType::AV_HWDEVICE_TYPE_VIDEOTOOLBOX)
+        .value("AV_HWDEVICE_TYPE_D3D11VA", AVHWDeviceType::AV_HWDEVICE_TYPE_D3D11VA)
+        .value("AV_HWDEVICE_TYPE_DRM", AVHWDeviceType::AV_HWDEVICE_TYPE_DRM)
+        .value("AV_HWDEVICE_TYPE_OPENCL", AVHWDeviceType::AV_HWDEVICE_TYPE_OPENCL)
+        .value("AV_HWDEVICE_TYPE_MEDIACODEC", AVHWDeviceType::AV_HWDEVICE_TYPE_MEDIACODEC)
+        .export_values();
+    py::enum_<AVSampleFormat>(m, "AVSampleFormat")
+        .value("AV_SAMPLE_FMT_NONE", AVSampleFormat::AV_SAMPLE_FMT_NONE)
+        .value("AV_SAMPLE_FMT_U8", AVSampleFormat::AV_SAMPLE_FMT_U8)
+        .value("AV_SAMPLE_FMT_S16", AVSampleFormat::AV_SAMPLE_FMT_S16)
+        .value("AV_SAMPLE_FMT_S32", AVSampleFormat::AV_SAMPLE_FMT_S32)
+        .value("AV_SAMPLE_FMT_FLT", AVSampleFormat::AV_SAMPLE_FMT_FLT)
+        .value("AV_SAMPLE_FMT_DBL", AVSampleFormat::AV_SAMPLE_FMT_DBL)
+        .value("AV_SAMPLE_FMT_U8P", AVSampleFormat::AV_SAMPLE_FMT_U8P)
+        .value("AV_SAMPLE_FMT_S16P", AVSampleFormat::AV_SAMPLE_FMT_S16P)
+        .value("AV_SAMPLE_FMT_S32P", AVSampleFormat::AV_SAMPLE_FMT_S32P)
+        .value("AV_SAMPLE_FMT_FLTP", AVSampleFormat::AV_SAMPLE_FMT_FLTP)
+        .value("AV_SAMPLE_FMT_DBLP", AVSampleFormat::AV_SAMPLE_FMT_DBLP)
+        .value("AV_SAMPLE_FMT_S64", AVSampleFormat::AV_SAMPLE_FMT_S64)
+        .value("AV_SAMPLE_FMT_S64P", AVSampleFormat::AV_SAMPLE_FMT_S64P)
+        .value("AV_SAMPLE_FMT_NB", AVSampleFormat::AV_SAMPLE_FMT_NB)
+        .export_values();
+
+    m.attr("__version__") = "2.1.8";
+
+}
+
 }
```

### Comparing `avio-2.1.7/src/avio.egg-info/PKG-INFO` & `avio-2.1.8/avio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: avio
-Version: 2.1.7
+Version: 2.1.8
 Summary: A python module for processing media streams
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libavio
 Project-URL: Bug Tracker, https://github.com/sr99622/libavio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # avio
 
 Python library for processing media streams
```

### Comparing `avio-2.1.7/src/avio.egg-info/SOURCES.txt` & `avio-2.1.8/avio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 CMakeLists.txt
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+avio/__init__.py
+avio.egg-info/PKG-INFO
+avio.egg-info/SOURCES.txt
+avio.egg-info/dependency_links.txt
+avio.egg-info/not-zip-safe
+avio.egg-info/top_level.txt
 cmake/FindFFmpeg.cmake
 include/Clock.h
 include/Decoder.h
 include/Display.h
 include/Encoder.h
 include/Exception.h
 include/Filter.h
@@ -275,13 +281,8 @@
 src/Filter.cpp
 src/Frame.cpp
 src/Packet.cpp
 src/Pipe.cpp
 src/Player.cpp
 src/Reader.cpp
 src/Writer.cpp
-src/avio.cpp
-src/avio.egg-info/PKG-INFO
-src/avio.egg-info/SOURCES.txt
-src/avio.egg-info/dependency_links.txt
-src/avio.egg-info/not-zip-safe
-src/avio.egg-info/top_level.txt
+src/avio.cpp
```

