# Comparing `tmp/backend.ai-kernel-23.3.2.tar.gz` & `tmp/backend.ai-kernel-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
+gzip compressed data, was "backend.ai-kernel-23.3.3.tar", last modified: Thu May 25 17:30:39 2023, max compression
```

## Comparing `backend.ai-kernel-23.3.2.tar` & `backend.ai-kernel-23.3.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.666858 backend.ai-kernel-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.666858 backend.ai-kernel-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/app/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36848 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/c/
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/git/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/golang/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/golang/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/haskell/
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/haskell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/intrinsic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/java/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.674858 backend.ai-kernel-23.3.2/ai/backend/kernel/julia/
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/jupyter_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.678858 backend.ai-kernel-23.3.2/ai/backend/kernel/lua/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/lua/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.678858 backend.ai-kernel-23.3.2/ai/backend/kernel/nodejs/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/nodejs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.678858 backend.ai-kernel-23.3.2/ai/backend/kernel/octave/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/octave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.678858 backend.ai-kernel-23.3.2/ai/backend/kernel/php/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/php/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.678858 backend.ai-kernel-23.3.2/ai/backend/kernel/python/
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/turtle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/sitecustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/r/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/r/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/r_server_ms/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/r_server_ms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/rust/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/rust/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/scheme/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/scheme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/service_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/aws_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/aws_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/aws_polly/inproc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/h2o/
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/h2o/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.682858 backend.ai-kernel-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-05 07:08:12.000000 backend.ai-kernel-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.317121 backend.ai-kernel-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.317121 backend.ai-kernel-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.321121 backend.ai-kernel-23.3.3/ai/backend/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.321121 backend.ai-kernel-23.3.3/ai/backend/kernel/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36687 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/git/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/golang/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/golang/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/haskell/
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/haskell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/intrinsic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/java/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/jupyter_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/lua/
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/lua/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/nodejs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/nodejs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/octave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/octave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/php/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/php/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.325121 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/sitecustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/r/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/r/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/r_server_ms/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/r_server_ms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/rust/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/scheme/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/scheme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/service_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/aws_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/aws_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/aws_polly/inproc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/h2o/
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/h2o/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:39.000000 backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:39.329121 backend.ai-kernel-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-25 17:30:38.000000 backend.ai-kernel-23.3.3/setup.py
```

### Comparing `backend.ai-kernel-23.3.2/PKG-INFO` & `backend.ai-kernel-23.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Kernel Runner
```

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/__main__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/app/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/app/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/base.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from jupyter_client.kernelspec import KernelSpecManager
 
 from .compat import current_loop
 from .intrinsic import (
     init_sshd_service,
     prepare_sshd_service,
     prepare_ttyd_service,
-    prepare_vscode_service,
 )
 from .jupyter_client import aexecute_interactive
 from .logging import BraceStyleAdapter, setup_logger
 from .service import ServiceParser
 from .utils import wait_local_port_open
 
 log = BraceStyleAdapter(logging.getLogger())
@@ -612,16 +611,14 @@
                 cmdargs: Optional[Sequence[Union[str, os.PathLike]]]
                 env: Mapping[str, str]
                 cmdargs, env = None, {}
                 if service_info["name"] == "ttyd":
                     cmdargs, env = await prepare_ttyd_service(service_info)
                 elif service_info["name"] == "sshd":
                     cmdargs, env = await prepare_sshd_service(service_info)
-                elif service_info["name"] == "vscode":
-                    cmdargs, env = await prepare_vscode_service(service_info)
                 elif self.service_parser is not None:
                     self.service_parser.variables["ports"] = service_info["ports"]
                     cmdargs, env = await self.service_parser.start_service(
                         service_info["name"],
                         self.child_env.keys(),
                         service_info["options"],
                     )
```

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/c/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/c/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/compat.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/cpp/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/git/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/git/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/golang/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/golang/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/haskell/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/haskell/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/intrinsic.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/intrinsic.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,24 +153,7 @@
     elif Path("/bin/ash").exists():
         shell = "ash"
 
     cmdargs = ["/opt/backend.ai/bin/ttyd", "-p", service_info["port"], f"/bin/{shell}"]
     if shell != "ash":  # Currently Alpine-based containers are not supported.
         cmdargs += ["-c", "/opt/kernel/tmux -2 attach"]
     return cmdargs, {}
-
-
-async def prepare_vscode_service(service_info):
-    # NOTE: This will be replaced as intrinsic binary: /opt/kernel/vscode/...
-    extension_dir = Path("/home/work/.vscode-exts")
-    extension_dir.mkdir(parents=True, exist_ok=True)
-    return [
-        "/usr/local/bin/code-server",
-        "--auth",
-        "none",
-        "--bind-addr",
-        "0.0.0.0",
-        "--port",
-        str(service_info["port"]),
-        "--extensions-dir",
-        str(extension_dir),
-    ], {"PWD": "/home/work"}
```

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/java/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/java/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/julia/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/julia/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/jupyter_client.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/jupyter_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/logging.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/logging.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/lua/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/lua/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/nodejs/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/nodejs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/octave/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/octave/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/php/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/php/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/canvas.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/canvas.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/color.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/color.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/drawing/turtle.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/drawing/turtle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/sitecustomize.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/python/types.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/python/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/r/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/r/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/r_server_ms/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/r_server_ms/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/rust/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/rust/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/scheme/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/scheme/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/service.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/service_actions.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/service_actions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/terminal.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/terminal.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/utils.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/aws_polly/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/aws_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/aws_polly/inproc.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/aws_polly/inproc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/ai/backend/kernel/vendor/h2o/__init__.py` & `backend.ai-kernel-23.3.3/ai/backend/kernel/vendor/h2o/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/PKG-INFO` & `backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Kernel Runner
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI Kernel Runner
```

### Comparing `backend.ai-kernel-23.3.2/backend.ai_kernel.egg-info/SOURCES.txt` & `backend.ai-kernel-23.3.3/backend.ai_kernel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-23.3.2/backend_shim.py` & `backend.ai-kernel-23.3.3/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `backend.ai-kernel-23.3.2/setup.py` & `backend.ai-kernel-23.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 5 - Production/Stable',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Kernel Runner',
     'install_requires': (
         'aiohttp~=3.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
@@ -71,11 +72,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.2
+    'version': """23.03.3
 """,
     'zip_safe': False,
 })
```

