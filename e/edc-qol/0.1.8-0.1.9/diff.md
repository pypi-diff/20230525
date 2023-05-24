# Comparing `tmp/edc-qol-0.1.8.tar.gz` & `tmp/edc-qol-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-qol-0.1.8.tar", last modified: Fri Aug 26 02:24:21 2022, max compression
+gzip compressed data, was "edc-qol-0.1.9.tar", last modified: Sun Sep 25 22:14:39 2022, max compression
```

## Comparing `edc-qol-0.1.8.tar` & `edc-qol-0.1.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.743811 edc-qol-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2021-09-23 18:00:25.000000 edc-qol-0.1.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-23 18:00:25.000000 edc-qol-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.733140 edc-qol-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.736958 edc-qol-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 22:39:38.000000 edc-qol-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1865 2022-06-01 23:17:43.000000 edc-qol-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 22:39:38.000000 edc-qol-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:39:38.000000 edc-qol-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)      127 2021-09-23 18:00:25.000000 edc-qol-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:17:43.000000 edc-qol-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-22 14:41:01.000000 edc-qol-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:17:43.000000 edc-qol-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     2036 2022-08-26 02:24:21.743936 edc-qol-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1014 2021-11-10 00:38:30.000000 edc-qol-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-26 02:24:14.000000 edc-qol-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:39:38.000000 edc-qol-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.738385 edc-qol-0.1.8/edc_qol/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.739526 edc-qol-0.1.8/edc_qol/admin/
--rw-r--r--   0 erikvw     (501) staff       (20)      146 2021-11-15 23:58:04.000000 edc-qol-0.1.8/edc_qol/admin/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2227 2022-08-23 02:20:25.000000 edc-qol-0.1.8/edc_qol/admin/eq5d3l_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4388 2022-08-23 02:20:25.000000 edc-qol-0.1.8/edc_qol/admin/sf12_admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      159 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      233 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/auth_objects.py
--rw-r--r--   0 erikvw     (501) staff       (20)      311 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2918 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/choices.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1067 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/constants.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.740054 edc-qol-0.1.8/edc_qol/forms/
--rw-r--r--   0 erikvw     (501) staff       (20)      108 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/forms/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1021 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/forms/eq5d3l_form.py
--rw-r--r--   0 erikvw     (501) staff       (20)      381 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/forms/sf12_form.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.740885 edc-qol-0.1.8/edc_qol/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)    19330 2022-08-10 22:39:38.000000 edc-qol-0.1.8/edc_qol/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)    23365 2022-08-10 22:39:38.000000 edc-qol-0.1.8/edc_qol/migrations/0002_historicalsf12_sf12.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1371 2022-07-06 07:01:21.000000 edc-qol-0.1.8/edc_qol/migrations/0003_auto_20220704_1841.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 22:30:02.000000 edc-qol-0.1.8/edc_qol/migrations/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.741215 edc-qol-0.1.8/edc_qol/model_mixins/
--rw-r--r--   0 erikvw     (501) staff       (20)       94 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/model_mixins/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1820 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/model_mixins/eq5d3l_model_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3204 2022-08-10 22:39:38.000000 edc-qol-0.1.8/edc_qol/model_mixins/sf12_model_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.741587 edc-qol-0.1.8/edc_qol/models/
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/models/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      713 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/models/eq5d3l.py
--rw-r--r--   0 erikvw     (501) staff       (20)      705 2022-06-21 18:27:55.000000 edc-qol-0.1.8/edc_qol/models/sf12.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.741913 edc-qol-0.1.8/edc_qol/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.743067 edc-qol-0.1.8/edc_qol/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.743675 edc-qol-0.1.8/edc_qol/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      923 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/tests/mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)      448 2022-08-26 02:24:13.000000 edc-qol-0.1.8/edc_qol/tests/tests/test_auths.py
--rw-r--r--   0 erikvw     (501) staff       (20)      225 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/tests/tests/test_eq5d3l_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)      219 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/tests/tests/test_sf12_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)      280 2021-09-23 18:00:25.000000 edc-qol-0.1.8/edc_qol/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      669 2021-11-10 00:38:30.000000 edc-qol-0.1.8/edc_qol/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-26 02:24:21.739045 edc-qol-0.1.8/edc_qol.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     2036 2022-08-26 02:24:21.000000 edc-qol-0.1.8/edc_qol.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1595 2022-08-26 02:24:21.000000 edc-qol-0.1.8/edc_qol.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-26 02:24:21.000000 edc-qol-0.1.8/edc_qol.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-09-23 17:29:25.000000 edc-qol-0.1.8/edc_qol.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        8 2022-08-26 02:24:21.000000 edc-qol-0.1.8/edc_qol.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1717 2022-08-10 22:39:38.000000 edc-qol-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1625 2022-06-01 23:17:43.000000 edc-qol-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-08-26 02:24:21.744300 edc-qol-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.517840 edc-qol-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2021-09-23 18:00:25.000000 edc-qol-0.1.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-09-23 18:00:25.000000 edc-qol-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.507317 edc-qol-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.511213 edc-qol-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 22:39:38.000000 edc-qol-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1865 2022-06-01 23:17:43.000000 edc-qol-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:14:31.000000 edc-qol-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 22:39:38.000000 edc-qol-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)      127 2021-09-23 18:00:25.000000 edc-qol-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2022-06-01 23:17:43.000000 edc-qol-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-09-22 14:41:01.000000 edc-qol-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:17:43.000000 edc-qol-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     2036 2022-09-25 22:14:39.517981 edc-qol-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1014 2021-11-10 00:38:30.000000 edc-qol-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:14:31.000000 edc-qol-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-10 22:39:38.000000 edc-qol-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.512726 edc-qol-0.1.9/edc_qol/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.513713 edc-qol-0.1.9/edc_qol/admin/
+-rw-r--r--   0 erikvw     (501) staff       (20)      146 2021-11-15 23:58:04.000000 edc-qol-0.1.9/edc_qol/admin/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2240 2022-09-25 22:14:31.000000 edc-qol-0.1.9/edc_qol/admin/eq5d3l_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4401 2022-09-25 22:14:31.000000 edc-qol-0.1.9/edc_qol/admin/sf12_admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      159 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      233 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/auth_objects.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      311 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2918 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/choices.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1067 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/constants.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.514031 edc-qol-0.1.9/edc_qol/forms/
+-rw-r--r--   0 erikvw     (501) staff       (20)      108 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/forms/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1019 2022-09-25 22:14:31.000000 edc-qol-0.1.9/edc_qol/forms/eq5d3l_form.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      379 2022-09-25 22:14:31.000000 edc-qol-0.1.9/edc_qol/forms/sf12_form.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.514917 edc-qol-0.1.9/edc_qol/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)    19330 2022-08-10 22:39:38.000000 edc-qol-0.1.9/edc_qol/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)    23365 2022-08-10 22:39:38.000000 edc-qol-0.1.9/edc_qol/migrations/0002_historicalsf12_sf12.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1371 2022-07-06 07:01:21.000000 edc-qol-0.1.9/edc_qol/migrations/0003_auto_20220704_1841.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 22:30:02.000000 edc-qol-0.1.9/edc_qol/migrations/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.515432 edc-qol-0.1.9/edc_qol/model_mixins/
+-rw-r--r--   0 erikvw     (501) staff       (20)       94 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/model_mixins/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1820 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/model_mixins/eq5d3l_model_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3204 2022-08-10 22:39:38.000000 edc-qol-0.1.9/edc_qol/model_mixins/sf12_model_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.515800 edc-qol-0.1.9/edc_qol/models/
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/models/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      713 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/models/eq5d3l.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      705 2022-06-21 18:27:55.000000 edc-qol-0.1.9/edc_qol/models/sf12.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.516032 edc-qol-0.1.9/edc_qol/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.516969 edc-qol-0.1.9/edc_qol/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.517717 edc-qol-0.1.9/edc_qol/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      923 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/tests/mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      448 2022-08-26 02:24:13.000000 edc-qol-0.1.9/edc_qol/tests/tests/test_auths.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      225 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/tests/tests/test_eq5d3l_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      219 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/tests/tests/test_sf12_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      280 2021-09-23 18:00:25.000000 edc-qol-0.1.9/edc_qol/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      669 2021-11-10 00:38:30.000000 edc-qol-0.1.9/edc_qol/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:14:39.513404 edc-qol-0.1.9/edc_qol.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2036 2022-09-25 22:14:39.000000 edc-qol-0.1.9/edc_qol.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1595 2022-09-25 22:14:39.000000 edc-qol-0.1.9/edc_qol.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:14:39.000000 edc-qol-0.1.9/edc_qol.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-09-23 17:29:25.000000 edc-qol-0.1.9/edc_qol.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        8 2022-09-25 22:14:39.000000 edc-qol-0.1.9/edc_qol.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1717 2022-08-10 22:39:38.000000 edc-qol-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1625 2022-06-01 23:17:43.000000 edc-qol-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1282 2022-09-25 22:14:39.518335 edc-qol-0.1.9/setup.cfg
```

### Comparing `edc-qol-0.1.8/.github/workflows/build.yml` & `edc-qol-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/.gitignore` & `edc-qol-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/.pre-commit-config.yaml` & `edc-qol-0.1.9/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
```

### Comparing `edc-qol-0.1.8/LICENSE` & `edc-qol-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/PKG-INFO` & `edc-qol-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-qol
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quality of Life instrument forms/models for the clinicedc/edc and other django projects
 Home-page: https://github.com/clinicedc/edc-qol
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc EuroQol EQ-5D-3L,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-qol-0.1.8/README.rst` & `edc-qol-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/admin/eq5d3l_admin.py` & `edc-qol-0.1.9/edc_qol/admin/eq5d3l_admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib import admin
 from django.utils.html import format_html
 from django_audit_fields.admin import audit_fieldset_tuple
+from edc_model_admin.dashboard import ModelAdminSubjectDashboardMixin
 from edc_model_admin.history import SimpleHistoryAdmin
-from edc_model_admin.mixins import ModelAdminInstitutionMixin
 
 from ..admin_site import edc_qol_admin
 from ..forms import Eq5d3lForm
 from ..models import Eq5d3l
 
 eq5d3l_description = """
 <H5><B><font color="orange">Interviewer to read</font></B></H5>
@@ -59,15 +59,15 @@
         "usual_activities": admin.VERTICAL,
         "pain_discomfort": admin.VERTICAL,
         "anxiety_depression": admin.VERTICAL,
     }
 
 
 @admin.register(Eq5d3l, site=edc_qol_admin)
-class Eq5d3lAdmin(ModelAdminInstitutionMixin, SimpleHistoryAdmin):
+class Eq5d3lAdmin(ModelAdminSubjectDashboardMixin, SimpleHistoryAdmin):
 
     form = Eq5d3lForm
 
     fieldsets = (
         (None, {"fields": ("subject_identifier", "report_datetime")}),
         *eq5d3l_fieldsets(),
         audit_fieldset_tuple,
```

### Comparing `edc-qol-0.1.8/edc_qol/admin/sf12_admin.py` & `edc-qol-0.1.9/edc_qol/admin/sf12_admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.contrib import admin
 from django.utils.html import format_html
 from django_audit_fields.admin import audit_fieldset_tuple
+from edc_model_admin.dashboard import ModelAdminSubjectDashboardMixin
 from edc_model_admin.history import SimpleHistoryAdmin
-from edc_model_admin.mixins import ModelAdminInstitutionMixin
 
 from ..admin_site import edc_qol_admin
 from ..forms import Sf12Form
 from ..models import Sf12
 
 additional_instructions = format_html(
     "<p>"
@@ -124,15 +124,15 @@
         "social_activities_interfered": admin.VERTICAL,
         "work_less_carefully_emotional": admin.VERTICAL,
         "work_limited_physical_health": admin.VERTICAL,
     }
 
 
 @admin.register(Sf12, site=edc_qol_admin)
-class Sf12Admin(ModelAdminInstitutionMixin, SimpleHistoryAdmin):
+class Sf12Admin(ModelAdminSubjectDashboardMixin, SimpleHistoryAdmin):
 
     form = Sf12Form
 
     fieldsets = (
         (None, {"fields": ("subject_identifier", "report_datetime")}),
         *sf12_fieldsets(),
         audit_fieldset_tuple,
```

### Comparing `edc-qol-0.1.8/edc_qol/choices.py` & `edc-qol-0.1.9/edc_qol/choices.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/constants.py` & `edc-qol-0.1.9/edc_qol/constants.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/forms/eq5d3l_form.py` & `edc-qol-0.1.9/edc_qol/forms/eq5d3l_form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django import forms
+from edc_crf.crf_form_validator import CrfFormValidator
 from edc_crf.modelform_mixins import CrfModelFormMixin
-from edc_form_validators.form_validator import FormValidator
 from edc_model.widgets import SliderWidget
 
 from ..models import Eq5d3l
 
 
-class Eq5d3lFormValidator(FormValidator):
+class Eq5d3lFormValidator(CrfFormValidator):
     def clean(self) -> None:
         self.confirm_scores_match()
 
     def confirm_scores_match(self):
         confirmed = self.cleaned_data.get("health_today_score_confirmed")
         if confirmed is not None:
             if int(self.cleaned_data.get("health_today_score_slider", "0")) != confirmed:
```

### Comparing `edc-qol-0.1.8/edc_qol/migrations/0001_initial.py` & `edc-qol-0.1.9/edc_qol/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/migrations/0002_historicalsf12_sf12.py` & `edc-qol-0.1.9/edc_qol/migrations/0002_historicalsf12_sf12.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/migrations/0003_auto_20220704_1841.py` & `edc-qol-0.1.9/edc_qol/migrations/0003_auto_20220704_1841.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/model_mixins/eq5d3l_model_mixin.py` & `edc-qol-0.1.9/edc_qol/model_mixins/eq5d3l_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/model_mixins/sf12_model_mixin.py` & `edc-qol-0.1.9/edc_qol/model_mixins/sf12_model_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/models/eq5d3l.py` & `edc-qol-0.1.9/edc_qol/models/eq5d3l.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/models/sf12.py` & `edc-qol-0.1.9/edc_qol/models/sf12.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-local-private.pem` & `edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/tests/etc/user-rsa-restricted-private.pem` & `edc-qol-0.1.9/edc_qol/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/tests/tests/mixins.py` & `edc-qol-0.1.9/edc_qol/tests/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol/utils.py` & `edc-qol-0.1.9/edc_qol/utils.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/edc_qol.egg-info/PKG-INFO` & `edc-qol-0.1.9/edc_qol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-qol
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quality of Life instrument forms/models for the clinicedc/edc and other django projects
 Home-page: https://github.com/clinicedc/edc-qol
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc EuroQol EQ-5D-3L,CRF,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-qol-0.1.8/edc_qol.egg-info/SOURCES.txt` & `edc-qol-0.1.9/edc_qol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/pyproject.toml` & `edc-qol-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/runtests.py` & `edc-qol-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-qol-0.1.8/setup.cfg` & `edc-qol-0.1.9/setup.cfg`

 * *Files identical despite different names*

