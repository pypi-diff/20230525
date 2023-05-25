# Comparing `tmp/coconut-develop-3.0.1.post0.dev3.tar.gz` & `tmp/coconut-develop-3.0.1.post0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev3.tar", last modified: Thu May 25 08:46:00 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.1.post0.dev4.tar", last modified: Thu May 25 09:19:54 2023, max compression
```

## Comparing `coconut-develop-3.0.1.post0.dev3.tar` & `coconut-develop-3.0.1.post0.dev4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/FAQ.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/DOCS.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/__coconut__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/constants_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/suite.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/src/runnable.coco
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/main_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/api.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/__coconut__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)    99363 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    92661 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut_py2/kernel.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-25 08:45:59.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    35759 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     8222 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-25 08:46:00.000000 coconut-develop-3.0.1.post0.dev3/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-25 08:09:21.000000 coconut-develop-3.0.1.post0.dev3/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11385 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/FAQ.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     5197 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)   194456 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    41755 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4539 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/constants_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    46206 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    62412 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5144 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    42032 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/suite.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     3356 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    21735 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/src/runnable.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/__coconut__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)    99363 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)    31830 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    92661 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58706 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   191434 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47243 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10729 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut_py2/kernel.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-05-25 09:19:53.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    44044 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     8255 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23425 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35759 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8222 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12685 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7577 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-05-25 09:19:54.000000 coconut-develop-3.0.1.post0.dev4/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13686 2023-05-25 08:46:46.000000 coconut-develop-3.0.1.post0.dev4/CONTRIBUTING.md
```

### Comparing `coconut-develop-3.0.1.post0.dev3/README.rst` & `coconut-develop-3.0.1.post0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/conf.py` & `coconut-develop-3.0.1.post0.dev4/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/FAQ.md` & `coconut-develop-3.0.1.post0.dev4/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/_coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev4/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/_coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev4/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/LICENSE.txt` & `coconut-develop-3.0.1.post0.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/setup.py` & `coconut-develop-3.0.1.post0.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/xontrib/coconut.py` & `coconut-develop-3.0.1.post0.dev4/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/HELP.md` & `coconut-develop-3.0.1.post0.dev4/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/DOCS.md` & `coconut-develop-3.0.1.post0.dev4/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/__coconut__/__init__.pyi` & `coconut-develop-3.0.1.post0.dev4/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/__coconut__/__init__.py` & `coconut-develop-3.0.1.post0.dev4/__coconut__/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/highlighter.py` & `coconut-develop-3.0.1.post0.dev4/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/api.py` & `coconut-develop-3.0.1.post0.dev4/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/constants_test.py` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/src/extras.coco` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/main_test.py` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/__main__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/tests/__init__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/convenience.pyi` & `coconut-develop-3.0.1.post0.dev4/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/convenience.py` & `coconut-develop-3.0.1.post0.dev4/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/__coconut__.pyi` & `coconut-develop-3.0.1.post0.dev4/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/api.pyi` & `coconut-develop-3.0.1.post0.dev4/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/root.py` & `coconut-develop-3.0.1.post0.dev4/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.1"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 3
+DEVELOP = 4
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/requirements.py` & `coconut-develop-3.0.1.post0.dev4/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/main.py` & `coconut-develop-3.0.1.post0.dev4/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/__coconut__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/templates/header.py_template`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/header.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/header.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/grammar.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/matching.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/compiler.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/util.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/compiler/__init__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/icoconut/root.py` & `coconut-develop-3.0.1.post0.dev4/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/icoconut/embed.py` & `coconut-develop-3.0.1.post0.dev4/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/icoconut/__main__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/icoconut/__init__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/mypy.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/watch.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/command.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/command.pyi` & `coconut-develop-3.0.1.post0.dev4/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/cli.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/util.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/command/__init__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/__init__.pyi` & `coconut-develop-3.0.1.post0.dev4/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/terminal.py` & `coconut-develop-3.0.1.post0.dev4/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/exceptions.py` & `coconut-develop-3.0.1.post0.dev4/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/constants.py` & `coconut-develop-3.0.1.post0.dev4/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/_pyparsing.py` & `coconut-develop-3.0.1.post0.dev4/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/integrations.py` & `coconut-develop-3.0.1.post0.dev4/coconut/integrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,65 +92,67 @@
     """Implements Coconut's _load_xontrib_."""
     loaded = False
     compiler = None
     runner = None
     timing_info = []
 
     @memoize_with_exceptions(128)
-    def _base_memoized_parse_xonsh(self, code):
+    def memoized_parse_xonsh(self, code):
         return self.compiler.parse_xonsh(code, keep_state=True)
 
-    def memoized_parse_xonsh(self, code):
+    def compile_code(self, code):
         """Memoized self.compiler.parse_xonsh."""
-        # .strip() outside the memoization
-        return self._base_memoized_parse_xonsh(code.strip())
+        # hide imports to avoid circular dependencies
+        from coconut.exceptions import CoconutException
+        from coconut.terminal import format_error
+        from coconut.util import get_clock_time
+        from coconut.terminal import logger
 
-    def new_parse(self, parser, code, mode="exec", *args, **kwargs):
-        """Coconut-aware version of xonsh's _parse."""
-        if self.loaded and mode not in disabled_xonsh_modes:
-            # hide imports to avoid circular dependencies
-            from coconut.exceptions import CoconutException
-            from coconut.terminal import format_error
-            from coconut.util import get_clock_time
-            from coconut.terminal import logger
+        parse_start_time = get_clock_time()
+        quiet, logger.quiet = logger.quiet, True
+        try:
+            # .strip() outside the memoization
+            code = self.memoized_parse_xonsh(code.strip())
+        except CoconutException as err:
+            err_str = format_error(err).splitlines()[0]
+            code += "  #" + err_str
+        finally:
+            logger.quiet = quiet
+            self.timing_info.append(("parse", get_clock_time() - parse_start_time))
 
-            parse_start_time = get_clock_time()
-            quiet, logger.quiet = logger.quiet, True
-            try:
-                code = self.memoized_parse_xonsh(code)
-            except CoconutException as err:
-                err_str = format_error(err).splitlines()[0]
-                code += "  #" + err_str
-            finally:
-                logger.quiet = quiet
-                self.timing_info.append(("parse", get_clock_time() - parse_start_time))
-        return parser.__class__.parse(parser, code, mode=mode, *args, **kwargs)
+        return code
 
     def new_try_subproc_toks(self, ctxtransformer, node, *args, **kwargs):
         """Version of try_subproc_toks that handles the fact that Coconut
         code may have different columns than Python code."""
         mode = ctxtransformer.mode
         if self.loaded:
             ctxtransformer.mode = "eval"
         try:
             return ctxtransformer.__class__.try_subproc_toks(ctxtransformer, node, *args, **kwargs)
         finally:
             ctxtransformer.mode = mode
 
-    def new_ctxvisit(self, ctxtransformer, node, inp, *args, **kwargs):
+    def new_parse(self, parser, code, mode="exec", *args, **kwargs):
+        """Coconut-aware version of xonsh's _parse."""
+        if self.loaded and mode not in disabled_xonsh_modes:
+            code = self.compile_code(code)
+        return parser.__class__.parse(parser, code, mode=mode, *args, **kwargs)
+
+    def new_ctxvisit(self, ctxtransformer, node, inp, ctx, mode="exec", *args, **kwargs):
         """Version of ctxvisit that ensures looking up original lines in inp
         using Coconut line numbers will work properly."""
-        if self.loaded:
+        if self.loaded and mode not in disabled_xonsh_modes:
             from xonsh.tools import get_logical_line
 
             # hide imports to avoid circular dependencies
             from coconut.terminal import logger
             from coconut.compiler.util import extract_line_num_from_comment
 
-            compiled = self.memoized_parse_xonsh(inp)
+            compiled = self.compile_code(inp)
 
             original_lines = tuple(inp.splitlines())
             used_lines = set()
             new_inp_lines = []
             last_ln = 1
             for compiled_line in compiled.splitlines():
                 ln = extract_line_num_from_comment(compiled_line, default=last_ln + 1)
@@ -162,15 +164,16 @@
                 if line in used_lines:
                     line = ""
                 else:
                     used_lines.add(line)
                 new_inp_lines.append(line)
                 last_ln = ln
             inp = "\n".join(new_inp_lines) + "\n"
-        return ctxtransformer.__class__.ctxvisit(ctxtransformer, node, inp, *args, **kwargs)
+
+        return ctxtransformer.__class__.ctxvisit(ctxtransformer, node, inp, ctx, mode, *args, **kwargs)
 
     def __call__(self, xsh, **kwargs):
         # hide imports to avoid circular dependencies
         from coconut.util import get_clock_time
 
         start_time = get_clock_time()
```

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/util.py` & `coconut-develop-3.0.1.post0.dev4/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/__main__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut/__init__.py` & `coconut-develop-3.0.1.post0.dev4/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/PKG-INFO` & `coconut-develop-3.0.1.post0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.1.post0.dev3
+Version: 3.0.1.post0.dev4
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
```

### Comparing `coconut-develop-3.0.1.post0.dev3/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.1.post0.dev4/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.1.post0.dev3/CONTRIBUTING.md` & `coconut-develop-3.0.1.post0.dev4/CONTRIBUTING.md`

 * *Files identical despite different names*

