# Comparing `tmp/onefuzz-8.1.0.tar.gz` & `tmp/onefuzz-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.1.0.tar", last modified: Mon May  8 15:54:48 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.2.0.tar", last modified: Wed May 24 18:21:25 2023, max compression
```

## Comparing `onefuzz-8.1.0.tar` & `onefuzz-8.2.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/
--rw-rw-rw-   0        0        0     1162 2023-05-08 15:53:57.000000 onefuzz-8.1.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-05-08 15:53:57.000000 onefuzz-8.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-05-08 15:54:48.000000 onefuzz-8.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-05-08 15:53:57.000000 onefuzz-8.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/extra/
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-05-08 15:53:57.000000 onefuzz-8.1.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-05-08 15:53:58.000000 onefuzz-8.1.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    68842 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22112 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1223 2023-05-08 15:54:47.000000 onefuzz-8.1.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    31082 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0     1682 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10491 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    42155 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8788 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9530 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10649 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      344 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-05-08 15:53:57.000000 onefuzz-8.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-05-08 15:53:57.000000 onefuzz-8.1.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      458 2023-05-08 15:53:58.000000 onefuzz-8.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 15:54:48.000000 onefuzz-8.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-05-08 15:53:57.000000 onefuzz-8.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-05-08 15:53:57.000000 onefuzz-8.1.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/
+-rw-rw-rw-   0        0        0     1162 2023-05-24 18:20:34.000000 onefuzz-8.2.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-05-24 18:20:34.000000 onefuzz-8.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-05-24 18:21:25.000000 onefuzz-8.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-05-24 18:20:34.000000 onefuzz-8.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-05-24 18:20:34.000000 onefuzz-8.2.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/extra/
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-05-24 18:20:34.000000 onefuzz-8.2.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-05-24 18:20:35.000000 onefuzz-8.2.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    67797 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1059 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22112 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1223 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31058 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0     1682 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10491 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     6837 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    42114 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8788 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9530 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10649 2023-05-24 18:20:34.000000 onefuzz-8.2.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-05-24 18:21:25.000000 onefuzz-8.2.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      344 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-24 18:21:24.000000 onefuzz-8.2.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-05-24 18:20:34.000000 onefuzz-8.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-05-24 18:20:34.000000 onefuzz-8.2.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      458 2023-05-24 18:20:35.000000 onefuzz-8.2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 18:21:25.000000 onefuzz-8.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-05-24 18:20:34.000000 onefuzz-8.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 18:21:25.000000 onefuzz-8.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-24 18:20:34.000000 onefuzz-8.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-05-24 18:20:34.000000 onefuzz-8.2.0/tests/test_template_helper.py
```

### Comparing `onefuzz-8.1.0/LICENSE` & `onefuzz-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/PKG-INFO` & `onefuzz-8.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.1.0
+Version: 8.2.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.1.0/README.md` & `onefuzz-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/domato.py` & `onefuzz-8.2.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/get-running.py` & `onefuzz-8.2.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/honggfuzz.py` & `onefuzz-8.2.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.2.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.2.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.2.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.2.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.2.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/examples/oss-fuzz-target.py` & `onefuzz-8.2.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/api.py` & `onefuzz-8.2.0/onefuzz/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1447,42 +1447,34 @@
             ),
         )
 
     def list(
         self,
         *,
         state: Optional[List[enums.NodeState]] = None,
-        scaleset_id: Optional[UUID_EXPANSION] = None,
+        scaleset_id: Optional[str] = None,
         pool_name: Optional[primitives.PoolName] = None,
     ) -> List[models.Node]:
         self.logger.debug("list nodes")
-        scaleset_id_expanded: Optional[UUID] = None
 
         if pool_name is not None:
             pool_name = primitives.PoolName(
                 self._disambiguate(
                     "name",
                     str(pool_name),
                     lambda x: False,
                     lambda: [x.name for x in self.onefuzz.pools.list()],
                 )
             )
 
-        if scaleset_id is not None:
-            scaleset_id_expanded = self._disambiguate_uuid(
-                "scaleset_id",
-                scaleset_id,
-                lambda: [str(x.scaleset_id) for x in self.onefuzz.scalesets.list()],
-            )
-
         return self._req_model_list(
             "GET",
             models.Node,
             data=requests.NodeSearch(
-                scaleset_id=scaleset_id_expanded, state=state, pool_name=pool_name
+                scaleset_id=scaleset_id, state=state, pool_name=pool_name
             ),
         )
 
     def add_ssh_key(
         self, machine_id: UUID_EXPANSION, *, public_key: str
     ) -> responses.BoolResult:
         self.logger.debug("add ssh public key to node: %s", machine_id)
@@ -1506,15 +1498,15 @@
 class Scaleset(Endpoint):
     """Interact with managed scaleset pools"""
 
     endpoint = "scaleset"
 
     def _expand_scaleset_machine(
         self,
-        scaleset_id: UUID_EXPANSION,
+        scaleset_id: str,
         machine_id: UUID_EXPANSION,
         *,
         include_auth: bool = False,
     ) -> Tuple[models.Scaleset, UUID]:
         scaleset = self.get(scaleset_id, include_auth=include_auth)
 
         if scaleset.nodes is None:
@@ -1573,62 +1565,40 @@
                 spot_instances=spot_instances,
                 ephemeral_os_disks=ephemeral_os_disks,
                 tags=tags,
                 auto_scale=auto_scale,
             ),
         )
 
-    def shutdown(
-        self, scaleset_id: UUID_EXPANSION, *, now: bool = False
-    ) -> responses.BoolResult:
-        scaleset_id_expanded = self._disambiguate_uuid(
-            "scaleset_id",
-            scaleset_id,
-            lambda: [str(x.scaleset_id) for x in self.list()],
-        )
-
-        self.logger.debug("shutdown scaleset: %s (now: %s)", scaleset_id_expanded, now)
+    def shutdown(self, scaleset_id: str, *, now: bool = False) -> responses.BoolResult:
+        self.logger.debug("shutdown scaleset: %s (now: %s)", scaleset_id, now)
         return self._req_model(
             "DELETE",
             responses.BoolResult,
-            data=requests.ScalesetStop(scaleset_id=scaleset_id_expanded, now=now),
+            data=requests.ScalesetStop(scaleset_id=scaleset_id, now=now),
         )
 
-    def get(
-        self, scaleset_id: UUID_EXPANSION, *, include_auth: bool = False
-    ) -> models.Scaleset:
+    def get(self, scaleset_id: str, *, include_auth: bool = False) -> models.Scaleset:
         self.logger.debug("get scaleset: %s", scaleset_id)
-        scaleset_id_expanded = self._disambiguate_uuid(
-            "scaleset_id",
-            scaleset_id,
-            lambda: [str(x.scaleset_id) for x in self.list()],
-        )
-
         return self._req_model(
             "GET",
             models.Scaleset,
             data=requests.ScalesetSearch(
-                scaleset_id=scaleset_id_expanded, include_auth=include_auth
+                scaleset_id=scaleset_id, include_auth=include_auth
             ),
         )
 
     def update(
-        self, scaleset_id: UUID_EXPANSION, *, size: Optional[int] = None
+        self, scaleset_id: str, *, size: Optional[int] = None
     ) -> models.Scaleset:
         self.logger.debug("update scaleset: %s", scaleset_id)
-        scaleset_id_expanded = self._disambiguate_uuid(
-            "scaleset_id",
-            scaleset_id,
-            lambda: [str(x.scaleset_id) for x in self.list()],
-        )
-
         return self._req_model(
             "PATCH",
             models.Scaleset,
-            data=requests.ScalesetUpdate(scaleset_id=scaleset_id_expanded, size=size),
+            data=requests.ScalesetUpdate(scaleset_id=scaleset_id, size=size),
         )
 
     def list(
         self,
         *,
         state: Optional[List[enums.ScalesetState]] = None,
     ) -> List[models.Scaleset]:
@@ -1641,15 +1611,15 @@
 class ScalesetProxy(Endpoint):
     """Interact with Scaleset Proxies (NOTE: This API is unstable)"""
 
     endpoint = "proxy"
 
     def delete(
         self,
-        scaleset_id: UUID_EXPANSION,
+        scaleset_id: str,
         machine_id: UUID_EXPANSION,
         *,
         dst_port: Optional[int] = None,
     ) -> responses.BoolResult:
         """Stop a proxy node"""
 
         (
@@ -1677,15 +1647,15 @@
         """Reset the proxy for an existing region"""
 
         return self._req_model(
             "PATCH", responses.BoolResult, data=requests.ProxyReset(region=region)
         )
 
     def get(
-        self, scaleset_id: UUID_EXPANSION, machine_id: UUID_EXPANSION, dst_port: int
+        self, scaleset_id: str, machine_id: UUID_EXPANSION, dst_port: int
     ) -> responses.ProxyGetResult:
         """Get information about a specific job"""
         (
             scaleset,
             machine_id_expanded,
         ) = self.onefuzz.scalesets._expand_scaleset_machine(scaleset_id, machine_id)
 
@@ -1701,15 +1671,15 @@
                 dst_port=dst_port,
             ),
         )
         return proxy
 
     def create(
         self,
-        scaleset_id: UUID_EXPANSION,
+        scaleset_id: str,
         machine_id: UUID_EXPANSION,
         dst_port: int,
         *,
         duration: Optional[int] = 1,
     ) -> responses.ProxyGetResult:
         """Create a proxy"""
         (
```

### Comparing `onefuzz-8.1.0/onefuzz/azcopy.py` & `onefuzz-8.2.0/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.2.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/backend.py` & `onefuzz-8.2.0/onefuzz/backend.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/cli.py` & `onefuzz-8.2.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/data/licenses.json` & `onefuzz-8.2.0/onefuzz/data/licenses.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {'3': "{'Version': '5.11.0'}", '4': "{'Version': '2023.3'}", '6': "{'Version': '4.6.1'}"}*

```diff
@@ -17,33 +17,33 @@
         "URL": "https://github.com/erocarrera/pefile",
         "Version": "2023.2.7"
     },
     {
         "License": "GNU General Public License v2 (GPLv2)",
         "Name": "pyinstaller",
         "URL": "https://www.pyinstaller.org/",
-        "Version": "5.10.1"
+        "Version": "5.11.0"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
-        "Version": "2023.2"
+        "Version": "2023.3"
     },
     {
         "License": "BSD",
         "Name": "pywin32-ctypes",
         "URL": "https://github.com/enthought/pywin32-ctypes",
         "Version": "0.2.0"
     },
     {
         "License": "Python Software Foundation License",
         "Name": "typing-extensions",
         "URL": "UNKNOWN",
-        "Version": "4.5.0"
+        "Version": "4.6.1"
     },
     {
         "License": "MIT License",
         "Name": "zipp",
         "URL": "https://github.com/jaraco/zipp",
         "Version": "3.15.0"
     }
```

### Comparing `onefuzz-8.1.0/onefuzz/data/privacy.txt` & `onefuzz-8.2.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/debug.py` & `onefuzz-8.2.0/onefuzz/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,27 +99,27 @@
         )
 
 
 class DebugScaleset(Command):
     """Debug tasks"""
 
     def _get_proxy_setup(
-        self, scaleset_id: UUID, machine_id: UUID, port: int, duration: Optional[int]
+        self, scaleset_id: str, machine_id: UUID, port: int, duration: Optional[int]
     ) -> Tuple[bool, str, Optional[Tuple[str, int]]]:
         proxy = self.onefuzz.scaleset_proxy.create(
             scaleset_id, machine_id, port, duration=duration
         )
         if proxy.ip is None:
             return (False, "waiting on proxy ip", None)
 
         return (True, "waiting on proxy port", (proxy.ip, proxy.forward.src_port))
 
     def rdp(
         self,
-        scaleset_id: UUID_EXPANSION,
+        scaleset_id: str,
         machine_id: UUID_EXPANSION,
         duration: Optional[int] = 1,
     ) -> None:
         (
             scaleset,
             machine_id_expanded,
         ) = self.onefuzz.scalesets._expand_scaleset_machine(
@@ -140,15 +140,15 @@
 
         ip, port = setup
         with rdp_connect(ip, scaleset.auth.password, port=port):
             return
 
     def ssh(
         self,
-        scaleset_id: UUID_EXPANSION,
+        scaleset_id: str,
         machine_id: UUID_EXPANSION,
         duration: Optional[int] = 1,
         command: Optional[str] = None,
     ) -> None:
         (
             scaleset,
             machine_id_expanded,
@@ -181,15 +181,15 @@
 
     def list_nodes(self, task_id: UUID_EXPANSION) -> Optional[List[NodeAssignment]]:
         task = self.onefuzz.tasks.get(task_id)
         return task.nodes
 
     def _get_node(
         self, task_id: UUID_EXPANSION, node_id: Optional[UUID]
-    ) -> Tuple[UUID, UUID]:
+    ) -> Tuple[str, UUID]:
         nodes = self.list_nodes(task_id)
         if not nodes:
             raise Exception("task is not currently executing on nodes")
 
         if node_id is not None:
             for node in nodes:
                 if node.node_id == node_id and node.scaleset_id is not None:
```

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/builder.py` & `onefuzz-8.2.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/cache.py` & `onefuzz-8.2.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.2.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.2.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/main.py` & `onefuzz-8.2.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/job_templates/manage.py` & `onefuzz-8.2.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/rdp.py` & `onefuzz-8.2.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/ssh.py` & `onefuzz-8.2.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/cache.py` & `onefuzz-8.2.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/cmd.py` & `onefuzz-8.2.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/raw.py` & `onefuzz-8.2.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/signalr.py` & `onefuzz-8.2.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/top.py` & `onefuzz-8.2.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/status/top_view.py` & `onefuzz-8.2.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/template.py` & `onefuzz-8.2.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/templates/__init__.py` & `onefuzz-8.2.0/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/templates/afl.py` & `onefuzz-8.2.0/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.2.0/onefuzz/templates/libfuzzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,33 +62,24 @@
         check_retry_count: Optional[int] = None,
         crash_report_timeout: Optional[int] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
         check_fuzzer_help: bool = False,
-        no_check_fuzzer_help: bool = False,
         expect_crash_on_failure: bool = False,
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[str] = None,
         source_allowlist: Optional[str] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
     ) -> None:
-        if check_fuzzer_help:
-            self.logger.warning(
-                "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
-            )
-        check_fuzzer_help = not no_check_fuzzer_help
-        del no_check_fuzzer_help
-
         target_options = target_options or []
-
         regression_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (
                 ContainerType.regression_reports,
                 containers[ContainerType.regression_reports],
@@ -893,14 +884,15 @@
         colocate_all_tasks: bool = False,
         crash_report_timeout: Optional[int] = 1,
         check_retry_count: Optional[int] = 300,
         check_fuzzer_help: bool = False,
         no_check_fuzzer_help: bool = False,
         extra_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
+        readonly_inputs: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer tasks, wrapped via qemu-user (PREVIEW FEATURE)
         """
         if check_fuzzer_help:
             self.logger.warning(
                 "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
@@ -946,15 +938,15 @@
             ContainerType.crashes,
             ContainerType.reports,
             ContainerType.unique_reports,
             ContainerType.no_repro,
         )
 
         if existing_inputs:
-            self.onefuzz.containers.get(existing_inputs)
+            self.onefuzz.containers.get(existing_inputs)  # ensure it exists
             helper.containers[ContainerType.inputs] = existing_inputs
         else:
             helper.define_containers(ContainerType.inputs)
 
         if crashes:
             self.onefuzz.containers.get(crashes)
             helper.containers[ContainerType.crashes] = crashes
@@ -964,29 +956,33 @@
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (ContainerType.inputs, helper.containers[ContainerType.inputs]),
         ]
 
         if extra_container is not None:
             fuzzer_containers.append((ContainerType.extra, extra_container))
 
+        if readonly_inputs is not None:
+            self.onefuzz.containers.get(readonly_inputs)  # ensure it exists
+            fuzzer_containers.append((ContainerType.readonly_inputs, readonly_inputs))
+
         helper.create_containers()
 
         target_exe_blob_name = helper.setup_relative_blob_name(target_exe, None)
 
         wrapper_name = File(target_exe_blob_name + "-wrapper.sh")
 
         with tempfile.TemporaryDirectory() as tempdir:
             if sysroot:
                 setup_path = File(os.path.join(tempdir, "setup.sh"))
                 with open(setup_path, "w", newline="\n") as handle:
                     sysroot_filename = helper.setup_relative_blob_name(sysroot, None)
                     handle.write(
                         "#!/bin/bash\n"
                         "set -ex\n"
-                        "sudo apt-get install -y qemu-user g++-aarch64-linux-gnu libasan5-arm64-cross\n"
+                        "sudo apt-get -o DPkg::Lock::Timeout=600 install -y qemu-user g++-aarch64-linux-gnu libasan5-arm64-cross\n"
                         'cd $(dirname "$(readlink -f "$0")")\n'
                         "mkdir -p sysroot\n"
                         "tar -C sysroot -zxvf %s\n" % sysroot_filename
                     )
 
                 wrapper_path = File(os.path.join(tempdir, wrapper_name))
                 with open(wrapper_path, "w", newline="\n") as handle:
```

### Comparing `onefuzz-8.1.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.2.0/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/templates/radamsa.py` & `onefuzz-8.2.0/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz/templates/regression.py` & `onefuzz-8.2.0/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.2.0/onefuzz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.1.0
+Version: 8.2.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.1.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.2.0/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/setup.py` & `onefuzz-8.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.1.0/tests/test_template_helper.py` & `onefuzz-8.2.0/tests/test_template_helper.py`

 * *Files identical despite different names*

