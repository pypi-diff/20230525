# Comparing `tmp/gemmi-program-0.6.1.tar.gz` & `tmp/gemmi-program-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemmi-program-0.6.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "gemmi-program-0.6.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `gemmi-program-0.6.1.tar` & `gemmi-program-0.6.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       15 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/.gitignore
--rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/CMakeLists.txt
--rw-r--r--   0        0        0      689 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/README.md
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1239 2022-11-09 12:37:21.000000 gemmi-program-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       15 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/.gitignore
+-rw-r--r--   0        0        0      907 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1038 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/README.md
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     1588 2022-11-09 12:37:21.000000 gemmi-program-0.6.2/PKG-INFO
```

### Comparing `gemmi-program-0.6.1/.github/workflows/wheels.yml` & `gemmi-program-0.6.2/.github/workflows/wheels.yml`

 * *Files 14% similar despite different names*

```diff
@@ -26,22 +26,22 @@
           - os: macos-11
             arch: "x86_64 arm64"
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.12.2
+      uses: pypa/cibuildwheel@v2.12.3
       env:
         CIBW_BUILD: ${{ github.event.inputs.cibw_build }}
         CIBW_SKIP: ${{ github.event.inputs.cibw_skip }}
         CIBW_ARCHS: "${{ matrix.arch }}"
         # increase pip debugging output
         CIBW_BUILD_VERBOSITY: 1
 
     - run: ls -lh wheelhouse
       shell: bash
 
     - uses: actions/upload-artifact@v3
       with:
-        name: wheels
+        name: program_wheels
         path: wheelhouse/*.whl
```

### Comparing `gemmi-program-0.6.1/CMakeLists.txt` & `gemmi-program-0.6.2/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # and use this options when building:
 set(GEMMI_VERSION_INFO "from wheel")
 
 include(FetchContent)
 FetchContent_Declare(
   gemmi
   GIT_REPOSITORY https://github.com/project-gemmi/gemmi.git
-  GIT_TAG        7639b1f421207db15d76d1d5f7a813990a634633 # v0.6.1
+  GIT_TAG        3f7b8d74971a0ee009347ceb5ae6780023861e62 # v0.6.2
 )
 
 # We don't want to install all gemmi files.
 # https://stackoverflow.com/questions/65527126/disable-install-for-fetchcontent
 FetchContent_GetProperties(gemmi)
 if (NOT gemmi_POPULATED)
   FetchContent_Populate(gemmi)
```

### Comparing `gemmi-program-0.6.1/pyproject.toml` & `gemmi-program-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["scikit-build-core==0.2.1"]
+requires = ["scikit-build-core==0.4.2"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "gemmi-program"
-version = "0.6.1"
+version = "0.6.2"
 requires-python = ">=3.8"
 description="gemmi (program executable only)"
 readme = "README.md"
 authors = [{name="Marcin Wojdyr", email="wojdyr@gmail.com"}]
 urls.repository = "https://github.com/project-gemmi/gemmi_program_wheel"
 license = {text = "MPL-2.0"}  # or, at your option, LGPL-3.0
 classifiers = [
```

### Comparing `gemmi-program-0.6.1/PKG-INFO` & `gemmi-program-0.6.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 Metadata-Version: 2.1
 Name: gemmi-program
-Version: 0.6.1
+Version: 0.6.2
 Summary: gemmi (program executable only)
 Author-Email: Marcin Wojdyr <wojdyr@gmail.com>
 License: MPL-2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: Repository, https://github.com/project-gemmi/gemmi_program_wheel
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## gemmi executable in a wheel
 
-Packaging [gemmi](https://gemmi.readthedocs.io/en/latest/utils.html),
-a command-line program from a crystallographic / structural biology project
-also called [gemmi](https://gemmi.readthedocs.io/en/latest/utils.html),
-as a python wheel that installable with pip.
+Here we provide the command-line program
+[gemmi](https://gemmi.readthedocs.io/en/latest/utils.html)
+in [wheels](https://github.com/project-gemmi/gemmi_program_wheel).
 
+It is, in PyPI, distributed separately from the Python extension module
+[gemmi](https://pypi.org/project/gemmi/),
+because, unlike the module, it does not depend on Python version.
 
-### how to make wheels after gemmi release
+### notes for myself -- how to make wheels after gemmi release
 
 * update `GIT_TAG` in CMakeLists.txt and `version` in pyproject.toml
 * (optionally) update version of cibuildwheel in .github/workflows/wheels.yml
+  and scikit-build-core in pyproject.toml
 * test locally with `pip wheel .`
 * make source distribution of this repo: `python -m build --sdist`
-* build wheels in GitHub Actions
-* download the wheels, check them, upload sdist and wheels to PyPI
+* git push changes to build wheels in [GitHub Actions][1]
+* download the wheels, check them, upload sdist and wheels to PyPI:
+
+      twine upload dist/gemmi-program-$VERSION.tar.gz
+      twine upload wheels/gemmi_program-$VERSION-*.whl
+
+[1]: https://github.com/project-gemmi/gemmi_program_wheel/actions
```

