# Comparing `tmp/lzstring_optimized-0.4.0.tar.gz` & `tmp/lzstring_optimized-0.5.0.tar.gz`

## Comparing `lzstring_optimized-0.4.0.tar` & `lzstring_optimized-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 lzstring_optimized-0.4.0/Cargo.toml
--rw-r--r--   0     1001      121     6148 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/.DS_Store
--rw-r--r--   0     1001      121      242 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/.github/workflows/build-wheels.sh
--rw-r--r--   0     1001      121     2791 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/.github/workflows/build.yaml
--rw-r--r--   0     1001      121        6 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/.gitignore
--rw-r--r--   0     1001      121       69 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/README.md
--rw-r--r--   0     1001      121       34 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/lzstring_optimized/__init__.py
--rw-r--r--   0     1001      121      102 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/lzstring_optimized/lzstring_optimized.pyi
--rw-r--r--   0     1001      121        0 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/lzstring_optimized/py.typed
--rw-r--r--   0     1001      121      195 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/pyproject.toml
--rw-r--r--   0     1001      121      432 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/run.py
--rw-r--r--   0     1001      121     2042 2022-09-08 04:05:41.000000 lzstring_optimized-0.4.0/src/lib.rs
--rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 lzstring_optimized-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      365 1970-01-01 00:00:00.000000 lzstring_optimized-0.5.0/Cargo.toml
+-rw-r--r--   0     1001      123     6148 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.DS_Store
+-rw-r--r--   0     1001      123      242 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.github/workflows/build-wheels.sh
+-rw-r--r--   0     1001      123     2847 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.github/workflows/build.yaml
+-rw-r--r--   0     1001      123        6 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/.gitignore
+-rw-r--r--   0     1001      123       69 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/README.md
+-rw-r--r--   0     1001      123       34 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/__init__.py
+-rw-r--r--   0     1001      123      102 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/lzstring_optimized.pyi
+-rw-r--r--   0     1001      123        0 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/lzstring_optimized/py.typed
+-rw-r--r--   0     1001      123      195 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/pyproject.toml
+-rw-r--r--   0     1001      123      432 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/run.py
+-rw-r--r--   0     1001      123     2042 2023-05-25 14:16:46.000000 lzstring_optimized-0.5.0/src/lib.rs
+-rw-r--r--   0     1001      123     6863 2023-05-25 14:18:47.000000 lzstring_optimized-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 lzstring_optimized-0.5.0/PKG-INFO
```

### Comparing `lzstring_optimized-0.4.0/.DS_Store` & `lzstring_optimized-0.5.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `lzstring_optimized-0.4.0/.github/workflows/build.yaml` & `lzstring_optimized-0.5.0/.github/workflows/build.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
           profile: minimal
           toolchain: stable
           override: true
       - uses: messense/maturin-action@v1
         with:
           maturin-version: latest
           command: build
-          args: --release --sdist -i 3.8 3.9 3.10
+          args: --release --sdist -i 3.8 3.9 3.10 3.11
       #  - name: Build wheels
       #    run: |
       #      curl https://sh.rustup.rs -sSf | sh -s -- -y
       #      source $HOME/.cargo/env
       #      rustup default nightly-2019-12-11
       #      bash .github/workflows/build-wheels.sh
       - uses: actions/upload-artifact@v1
@@ -35,15 +35,15 @@
           name: linux-wheels
           path: target/wheels/
 
   osx-wheels:
     runs-on: macos-latest
     strategy:
       matrix:
-        python-version: [3.8, 3.9, "3.10"]
+        python-version: [3.8, 3.9, "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v1
       - uses: actions-rs/toolchain@v1
         with:
           toolchain: nightly
           default: true
       - uses: actions/setup-python@v2
@@ -84,14 +84,15 @@
       - uses: actions/download-artifact@v3
 
       - name: Display structure of downloaded files
         run: ls -R
 
       - run: mkdir wheels
       - run: mv ./linux-wheels/* wheels
+      - run: mv ./osx-3.11-wheel/* wheels
       - run: mv ./osx-3.10-wheel/* wheels
       - run: mv ./osx-3.9-wheel/* wheels
       - run: mv ./osx-3.8-wheel/* wheels
       - run: mv ./windows-wheels/* wheels
 
 
       - name: Display structure of downloaded files
@@ -99,8 +100,8 @@
 
       - name: Publish a Python distribution to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages_dir: wheels/
           verify_metadata: false
-          
+
```

### Comparing `lzstring_optimized-0.4.0/src/lib.rs` & `lzstring_optimized-0.5.0/src/lib.rs`

 * *Files identical despite different names*

