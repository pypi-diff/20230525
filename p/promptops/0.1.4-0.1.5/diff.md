# Comparing `tmp/promptops-0.1.4.tar.gz` & `tmp/promptops-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.4.tar", last modified: Wed May 24 15:24:39 2023, max compression
+gzip compressed data, was "promptops-0.1.5.tar", last modified: Thu May 25 18:39:37 2023, max compression
```

## Comparing `promptops-0.1.4.tar` & `promptops-0.1.5.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.039405 promptops-0.1.4/
--rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.4/LICENSE.txt
--rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-24 15:24:39.039596 promptops-0.1.4/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1292 2023-05-24 14:55:10.000000 promptops-0.1.4/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.013963 promptops-0.1.4/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.015551 promptops-0.1.4/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1368 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.016141 promptops-0.1.4/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.016882 promptops-0.1.4/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.017563 promptops-0.1.4/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.018478 promptops-0.1.4/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1233 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.019318 promptops-0.1.4/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.020245 promptops-0.1.4/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.4/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.026289 promptops-0.1.4/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      942 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/cancellable.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)      394 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/feedback.py
--rw-r--r--   0 vasily     (501) staff       (20)     3609 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.031230 promptops-0.1.4/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)     7050 2023-05-24 15:23:14.000000 promptops-0.1.4/promptops/main.py
--rw-r--r--   0 vasily     (501) staff       (20)       28 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/nux.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.033023 promptops-0.1.4/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     3908 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    16290 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.033676 promptops-0.1.4/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     6435 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/recipes/creation.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.034477 promptops-0.1.4/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.035449 promptops-0.1.4/promptops/secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/secrets/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      326 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2292 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.037870 promptops-0.1.4/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3332 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     1635 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     1789 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     2543 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/similarity.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.039031 promptops-0.1.4/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     7026 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     3990 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-05-24 15:09:41.000000 promptops-0.1.4/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.4/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-24 15:24:39.028626 promptops-0.1.4/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-24 15:24:38.000000 promptops-0.1.4/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     1962 2023-05-24 15:24:39.000000 promptops-0.1.4/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-05-24 15:24:38.000000 promptops-0.1.4/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-05-24 15:24:38.000000 promptops-0.1.4/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      209 2023-05-24 15:24:38.000000 promptops-0.1.4/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-05-24 15:24:38.000000 promptops-0.1.4/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.4/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       78 2023-05-24 15:24:39.040270 promptops-0.1.4/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.4/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.324385 promptops-0.1.5/
+-rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.5/LICENSE.txt
+-rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-25 18:39:37.324543 promptops-0.1.5/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     1292 2023-05-24 14:55:10.000000 promptops-0.1.5/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.300650 promptops-0.1.5/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.302274 promptops-0.1.5/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1368 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.302813 promptops-0.1.5/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.303370 promptops-0.1.5/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.303842 promptops-0.1.5/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.304710 promptops-0.1.5/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1233 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.305474 promptops-0.1.5/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.306163 promptops-0.1.5/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.5/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.311293 promptops-0.1.5/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      394 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/feedback.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3836 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.316155 promptops-0.1.5/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7060 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/main.py
+-rw-r--r--   0 vasily     (501) staff       (20)       28 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/nux.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.318122 promptops-0.1.5/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    16123 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.318899 promptops-0.1.5/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6435 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/recipes/creation.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.319703 promptops-0.1.5/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.320467 promptops-0.1.5/promptops/secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/secrets/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      326 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2292 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.322954 promptops-0.1.5/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3367 2023-05-25 18:38:08.000000 promptops-0.1.5/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1097 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1635 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1789 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2543 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/similarity.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.324069 promptops-0.1.5/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7026 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3990 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-05-25 18:38:54.000000 promptops-0.1.5/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.5/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-05-25 18:39:37.313501 promptops-0.1.5/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     1929 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     1937 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      209 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-05-25 18:39:37.000000 promptops-0.1.5/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.5/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       78 2023-05-25 18:39:37.325199 promptops-0.1.5/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     1967 2023-05-24 14:41:57.000000 promptops-0.1.5/setup.py
```

### Comparing `promptops-0.1.4/LICENSE.txt` & `promptops-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/PKG-INFO` & `promptops-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.4
+Version: 0.1.5
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
```

### Comparing `promptops-0.1.4/README.md` & `promptops-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/comms/dtos.py` & `promptops-0.1.5/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/comms/http_reporter.py` & `promptops-0.1.5/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/comms/ws.py` & `promptops-0.1.5/local_runner/comms/ws.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/config/config.py` & `promptops-0.1.5/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/creds/creds.py` & `promptops-0.1.5/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/exec/manager.py` & `promptops-0.1.5/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/handler/handler.py` & `promptops-0.1.5/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/main.py` & `promptops-0.1.5/local_runner/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/registration/registration.py` & `promptops-0.1.5/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/local_runner/tokens/issuer.py` & `promptops-0.1.5/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/corrections.py` & `promptops-0.1.5/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/history.py` & `promptops-0.1.5/promptops/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         cmd = item["text"]
         vector = np.array(item["embeddings"])
         items.append((cmd, vector))
 
     return items
 
 
-def index_history(show_progress=False):
+def index_history(show_progress: bool = None):
     progress = None
     if show_progress:
         from promptops.loading.progress import ProgressSpinner
 
         progress = ProgressSpinner(100)
         progress.increment(1)
 
@@ -77,24 +77,29 @@
     prev_commands = get_shell().get_full_history()
 
     if show_progress:
         progress.increment(3)
 
     indexed_commands = {obj if isinstance(obj, str) else obj["cmd"] for obj in db.objects}
     delta = list(set(prev_commands) - indexed_commands)
+    batch_size = 32
 
+    if show_progress is None and len(delta) > batch_size:
+        from promptops.loading.progress import ProgressSpinner
+        show_progress = True
+        progress = ProgressSpinner(100)
+        progress.increment(4)
     if show_progress:
         progress.increment(2)
 
     if len(delta) == 0:
         if show_progress:
             progress.set(100)
         return
 
-    batch_size = 32
     progress_inc = (100 - 6) // (len(delta) / batch_size)
 
     for i in range(0, len(delta), batch_size):
         for cmd, vector in embedding_batch(delta[i : i + batch_size]):
             db.add(vector, {"cmd": cmd, "ignore": False})
         if show_progress:
             progress.increment(progress_inc)
```

### Comparing `promptops-0.1.4/promptops/loading/base.py` & `promptops-0.1.5/promptops/loading/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/loading/pong.py` & `promptops-0.1.5/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/loading/progress.py` & `promptops-0.1.5/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/loading/promptops.py` & `promptops-0.1.5/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/loading/simple.py` & `promptops-0.1.5/promptops/loading/simple.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/main.py` & `promptops-0.1.5/promptops/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from promptops import user
 from promptops.recipes.creation import workflow_entrypoint
 
 ENDPOINT_ENV = "PROMPTOPS_ENDPOINT"
 
 
 def runner_mode(args):
-    from feedback import feedback
+    from promptops.feedback import feedback
 
     feedback(
         {
             "event": "runner_mode",
         }
     )
```

### Comparing `promptops-0.1.4/promptops/query/explanation.py` & `promptops-0.1.5/promptops/query/explanation.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,30 +55,45 @@
 
 
 class ReturningThread(threading.Thread):
     def __init__(self, target, args=None, kwargs=None, daemon=False):
         super().__init__(target=self.run, daemon=daemon)
         self._return_value = None
         self._exception = None
+        self._finished = False
         self.function = target
         self.args = args or []
         self.kwargs = kwargs or {}
+        self._done_callbacks = []
 
     def run(self):
         try:
             self._return_value = self.function(*self.args, **self.kwargs)
         except Exception as e:
             self._exception = e
+        self._finished = True
+        for fn in self._done_callbacks:
+            fn(self)
 
     def join(self, timeout=None) -> any:
         super().join(timeout)
         if self._exception is not None:
             raise self._exception
         return self._return_value
 
+    def add_done_callback(self, fn):
+        self._done_callbacks.append(fn)
+
+    def result(self):
+        if not self._finished:
+            raise RuntimeError("not finished")
+        if self._exception is not None:
+            raise self._exception
+        return self._return_value
+
 
 def _loading_animation(spinner, should_continue: Callable[[], bool]):
     while should_continue():
         spinner.step()
         time.sleep(0.1)
```

### Comparing `promptops-0.1.4/promptops/query/messages.py` & `promptops-0.1.5/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/query/query.py` & `promptops-0.1.5/promptops/query/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import prompt_toolkit
 
 from promptops import settings
 from promptops import trace
 from promptops import user
 from promptops.ui import prompts
 from promptops.ui import selections
-from promptops.cancellable import ThreadPoolExecutor
 from promptops.loading import Simple, loading_animation
 from promptops import similarity
 from promptops import corrections
 from promptops.corrections import get_correction
 from promptops.feedback import feedback
 from promptops import history
 from promptops import settings_store
@@ -45,22 +44,22 @@
 
 
 def run(cmd: Result) -> (int, Optional[str]):
     if cmd.lang == "shell":
         proc = subprocess.run(
             cmd.script, shell=True, start_new_session=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
-        if proc.stdout and str(proc.stdout) != "":
+        if proc.stdout and len(proc.stdout) > 0:
             sys.stdout.write(proc.stdout.decode("utf-8"))
-        if proc.stderr and str(proc.stderr) != "":
+        if proc.stderr and len(proc.stderr) > 0:
             sys.stdout.write(proc.stderr.decode("utf-8"))
         sys.stdout.flush()
 
         history.add(scrub_secrets.scrub_line(".bash_history", cmd.script), proc.returncode)
-        return proc.returncode, str(proc.stderr)
+        return proc.returncode, proc.stderr.decode("utf-8")
     else:
         raise NotImplementedError(f"{cmd.lang} not implemented yet")
 
 
 def corrections_search(embedding):
     db = corrections.get_db()
     similar = db.search(embedding, k=3, min_similarity=0.8)
@@ -84,50 +83,50 @@
     confirmed: str = ""
     question: str = None
     options: list = None
 
 
 def revise_loop(questions: list[str], prev_results: list[list[str]]) -> ConfirmResult:
     embedding = similarity.embedding(text="\n".join(questions))
-    with loading_animation(Simple("thinking...")), ThreadPoolExecutor(max_workers=5) as tpe:
-        cs_task = tpe.submit(corrections_search, embedding)
-        hs_task = tpe.submit(history.check_history, embedding)
-
     update_lock = threading.Lock()
     corrected_results = []
-    similar_corrections = cs_task.result()
+
+    similar_corrections = corrections_search(embedding)
     logging.debug("found %d similar corrections", len(similar_corrections))
     if len(similar_corrections) > 0:
         for qa, score in similar_corrections:
             logging.debug(f"- {score:.2f}: {qa.question} -> {qa.corrected}")
             corrected_results.append(Result(script=qa.corrected, origin="history"))
-    history_results = hs_task.result()
+
+    history_results = history.check_history(embedding)
     logging.debug("found %d similar history results", len(history_results))
     if len(history_results) > 0:
         for r, score in history_results:
             logging.debug(f"- {score:.2f}: {r}")
     history_results = [
         Result(script=r if isinstance(r, str) else r["cmd"], explanation="loaded from shell history", origin="history")
         for r, _ in history_results
     ]
 
     results = corrected_results + history_results
     results = deduplicate(results)
 
-    tpe = ThreadPoolExecutor(max_workers=2)
     ui = None
     tasks = [
-        tpe.submit(
+        ReturningThread(
             query,
-            q=questions[-1],
-            prev_questions=questions[:-1],
-            corrected_results=[qa for qa, _ in similar_corrections],
-            prev_results=prev_results,
-            similar_history=[r.script for r in history_results],
-            history_context=[],
+            kwargs=dict(
+                q=questions[-1],
+                prev_questions=questions[:-1],
+                corrected_results=[qa for qa, _ in similar_corrections],
+                prev_results=prev_results,
+                similar_history=[r.script for r in history_results],
+                history_context=[],
+            ),
+            daemon=True,
         )
     ]
     num_running = len(tasks)
 
     def update_results(extra):
         with update_lock:
             nonlocal num_running
@@ -136,27 +135,28 @@
             results.extend(extra)
             if ui:
                 options = [pretty_result(r) for r in results]
                 if num_running == 0:
                     options += [make_revise_option()]
                 ui.reset_options(options, is_loading=num_running > 0)
 
-    def done_callback(future):
-        if future.exception():
-            print(future.exception())
-        update_results(future.result())
+    def done_callback(thread: ReturningThread):
+        try:
+            update_results(thread.result())
+        except Exception as exc:
+            logging.exception(exc)
 
     for task in tasks:
-        task.add_done_callback(tpe.cancellable_callback(done_callback))
+        task.add_done_callback(done_callback)
+        task.start()
 
     if len(results) == 0:
         with loading_animation(Simple("thinking...")):
-            tpe.shutdown(wait=True)
+            results = [r for t in tasks for r in t.join()]
         num_running = 0
-        results = [r for t in tasks for r in t.result()]
         results = deduplicate(results)
         if len(results) == 0:
             feedback({"event": "no-results"})
             print("couldn't find any results, try rephrasing your question or providing more context")
             selected = prompts.confirm_clarify("")
             if selected == prompts.EXIT:
                 raise KeyboardInterrupt()
@@ -278,18 +278,18 @@
         f"looks like the command failed (return code was not 0), would you like us to attempt to fix it?"
     )
     if selected == prompts.GO_BACK:
         return None
     elif selected == prompts.EXIT:
         raise KeyboardInterrupt()
 
-    with loading_animation(Simple("thinking...")), ThreadPoolExecutor(max_workers=5) as tpe:
-        ce_task = tpe.submit(get_correction, prompt=prompt, command=command, error=error)
-
-    result = ce_task.result()
+    with loading_animation(Simple("thinking...")):
+        ce_task = ReturningThread(target=get_correction, kwargs=dict(prompt=prompt, command=command, error=error), daemon=True)
+        ce_task.start()
+        result = ce_task.join()
 
     results = [
         Result(script=result, explanation=f"Revised previous command: {command}"),
     ]
     options = [pretty_result(r) for r in results]
     ui = selections.UI(options, False, loading_text=random.choice(messages.QUERY))
```

### Comparing `promptops-0.1.4/promptops/query.py` & `promptops-0.1.5/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/recipes/creation.py` & `promptops-0.1.5/promptops/recipes/creation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/scrub_secrets/scrub.py` & `promptops-0.1.5/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/secrets/scrub.py` & `promptops-0.1.5/promptops/secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/settings_store.py` & `promptops-0.1.5/promptops/settings_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/shells/base.py` & `promptops-0.1.5/promptops/shells/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     def get_full_history(self):
         history = self._read_history_file()
         cmds = self._get_cmds_from_lines(history)
         return scrub_lines(self.history_file, list(filter_commands(cmds)))
 
     def _read_history_file(self):
         fname = os.path.expanduser(self.history_file)
-        with open(fname, "r") as f:
+        with open(fname, "r", encoding="utf-8", errors="ignore") as f:
             return [line.strip() for line in f if line.strip() != ""]
 
     def _get_cmds_from_lines(self, history):
         raise NotImplementedError()
 
     def get_recent_history(self, look_back: int = 10):
         raise NotImplementedError()
```

### Comparing `promptops-0.1.4/promptops/shells/bash.py` & `promptops-0.1.5/promptops/shells/bash.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/shells/common.py` & `promptops-0.1.5/promptops/shells/common.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/shells/fish.py` & `promptops-0.1.5/promptops/shells/fish.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/shells/zsh.py` & `promptops-0.1.5/promptops/shells/zsh.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/similarity.py` & `promptops-0.1.5/promptops/similarity.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/ui/prompts.py` & `promptops-0.1.5/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/ui/selections.py` & `promptops-0.1.5/promptops/ui/selections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/ui.py` & `promptops-0.1.5/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/user.py` & `promptops-0.1.5/promptops/user.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops/version_check.py` & `promptops-0.1.5/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.4/promptops.egg-info/PKG-INFO` & `promptops-0.1.5/promptops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.4
+Version: 0.1.5
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
```

### Comparing `promptops-0.1.4/promptops.egg-info/SOURCES.txt` & `promptops-0.1.5/promptops.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 local_runner/handler/censor.py
 local_runner/handler/handler.py
 local_runner/registration/__init__.py
 local_runner/registration/registration.py
 local_runner/tokens/__init__.py
 local_runner/tokens/issuer.py
 promptops/__init__.py
-promptops/cancellable.py
 promptops/corrections.py
 promptops/feedback.py
 promptops/history.py
 promptops/main.py
 promptops/nux.py
 promptops/query.py
 promptops/settings.py
```

### Comparing `promptops-0.1.4/setup.py` & `promptops-0.1.5/setup.py`

 * *Files identical despite different names*

