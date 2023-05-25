# Comparing `tmp/wok_code-2.0.7.tar.gz` & `tmp/wok_code-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wok_code-2.0.7.tar", last modified: Tue May  9 17:25:50 2023, max compression
+gzip compressed data, was "dist/wok_code-2.0.8.tar", last modified: Thu May 25 08:46:35 2023, max compression
```

## Comparing `wok_code-2.0.7.tar` & `wok_code-2.0.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.7/wok_code.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      950 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1931 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-09 17:25:50.000000 wok_code-2.0.7/setup.cfg
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/__main__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3056 2023-05-09 13:43:39.000000 wok_code-2.0.7/wok_code/do_gitignore.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/gen_addons_table.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/rm_dir_with_space.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.7/wok_code/pgconf.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/tests/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6539 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_gen_readme.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/tests/test_filepo.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/tests/test_license_mgnt.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7806 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/ssh.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     8389 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/pypi.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/cvt_csv_2_xml.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/scripts/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    64039 2023-04-30 14:24:57.000000 wok_code-2.0.7/wok_code/scripts/please.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/to_pep8.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3912 2023-05-09 17:24:49.000000 wok_code-2.0.7/wok_code/scripts/setup.info
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6865 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/main.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/makepo_it.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/cvt_csv_coa.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/scripts/run_odoo_debug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17827 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/dist_pkg.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/generate_random_codes.py
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)    29444 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/run_odoo_debug.sh
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/wget_odoo_repositories.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-09 17:25:50.000000 wok_code-2.0.7/wok_code/scripts/config/
--rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.7/wok_code/scripts/config/to_odoo_py2.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.7/wok_code/scripts/config/to_odoo_py3.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.7/wok_code/scripts/config/to_new_api.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.7/wok_code/scripts/config/globals.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.7/wok_code/scripts/config/to_old_api.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.7/wok_code/scripts/config/globals_xml.yml
--rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please_apache.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/scripts/dist_pkg.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26398 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/do_migrate.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_translation_old.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    83221 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/gen_readme.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    10100 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/lint_2_compare.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    42912 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/deploy_odoo.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please_z0bug.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46376 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_translation.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/odoo_dependencies.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.7/wok_code/scripts/license_mgnt.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/cvt_csv_2_rst.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/please.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/scripts/do_odoo_site.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.7/wok_code/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/eval_gtin.py
--rw-r--r--   0 odoo      (1000) odoo      (1000)    14663 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/do_git_checkout_new_branch.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/topep8
--rwxr-xr-x   0 odoo      (1000) odoo      (1000)     2242 2023-05-02 18:41:06.000000 wok_code-2.0.7/wok_code/install_python_3_from_source.sh
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/cvt_script.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_oca.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/do_set_utf8.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6896 2023-01-21 13:24:11.000000 wok_code-2.0.7/wok_code/please.man
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_zero.2p8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.7/wok_code/to_pep8.2p8
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.7/wok_code/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-05-09 16:01:24.000000 wok_code-2.0.7/wok_code/cvt_script
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3912 2023-05-09 16:01:24.000000 wok_code-2.0.7/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-09 17:25:50.000000 wok_code-2.0.7/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    47243 2023-05-09 17:25:50.000000 wok_code-2.0.7/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        9 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 06:35:40.000000 wok_code-2.0.8/wok_code.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      948 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1931 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       64 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:46:35.000000 wok_code-2.0.8/setup.cfg
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/__main__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3053 2023-05-13 12:31:38.000000 wok_code-2.0.8/wok_code/do_gitignore.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7186 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/gen_addons_table.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      205 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/rm_dir_with_space.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3082 2023-04-23 10:48:07.000000 wok_code-2.0.8/wok_code/pgconf.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/tests/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6517 2023-05-20 15:28:26.000000 wok_code-2.0.8/wok_code/tests/test_gen_readme.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     2229 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/tests/test_please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2028 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/tests/test_filepo.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4939 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/tests/test_license_mgnt.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7806 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/ssh.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     9119 2023-05-21 13:36:02.000000 wok_code-2.0.8/wok_code/pypi.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6744 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/cvt_csv_2_xml.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/scripts/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    61313 2023-05-25 08:46:18.000000 wok_code-2.0.8/wok_code/scripts/please.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    71159 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/to_pep8.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3910 2023-05-25 06:21:29.000000 wok_code-2.0.8/wok_code/scripts/setup.info
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6865 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/main.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4990 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/makepo_it.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    21516 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/cvt_csv_coa.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/scripts/run_odoo_debug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    17944 2023-05-21 05:45:17.000000 wok_code-2.0.8/wok_code/scripts/dist_pkg.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1225 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/generate_random_codes.py
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)    29393 2023-05-25 06:20:46.000000 wok_code-2.0.8/wok_code/scripts/run_odoo_debug.sh
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    30263 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/wget_odoo_repositories.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:46:35.000000 wok_code-2.0.8/wok_code/scripts/config/
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      224 2023-04-12 07:55:02.000000 wok_code-2.0.8/wok_code/scripts/config/to_odoo_py2.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      173 2023-04-12 07:50:10.000000 wok_code-2.0.8/wok_code/scripts/config/to_odoo_py3.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      893 2023-04-12 07:02:48.000000 wok_code-2.0.8/wok_code/scripts/config/to_new_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      373 2023-04-12 10:49:14.000000 wok_code-2.0.8/wok_code/scripts/config/globals.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)      698 2023-04-12 06:43:18.000000 wok_code-2.0.8/wok_code/scripts/config/to_old_api.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)        0 2023-04-12 07:23:52.000000 wok_code-2.0.8/wok_code/scripts/config/globals_xml.yml
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     7066 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please_apache.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      992 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/scripts/dist_pkg.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    26568 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/do_migrate.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    25546 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_translation_old.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    86505 2023-05-22 09:12:11.000000 wok_code-2.0.8/wok_code/scripts/gen_readme.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    11743 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/lint_2_compare.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    42912 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/deploy_odoo.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     5550 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please_z0bug.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    46376 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_translation.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    31823 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/odoo_dependencies.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    10070 2023-01-27 08:05:01.000000 wok_code-2.0.8/wok_code/scripts/license_mgnt.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5357 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/cvt_csv_2_rst.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    22434 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/please.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5937 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/scripts/do_odoo_site.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      606 2023-04-21 11:43:14.000000 wok_code-2.0.8/wok_code/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2176 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/eval_gtin.py
+-rw-r--r--   0 odoo      (1000) odoo      (1000)    14663 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/do_git_checkout_new_branch.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    32228 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/topep8
+-rwxr-xr-x   0 odoo      (1000) odoo      (1000)     2242 2023-05-02 18:41:06.000000 wok_code-2.0.8/wok_code/install_python_3_from_source.sh
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1150 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/cvt_script.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1672 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_oca.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2646 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/do_set_utf8.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6897 2023-05-18 06:33:56.000000 wok_code-2.0.8/wok_code/please.man
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2667 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_zero.2p8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     5228 2022-12-09 05:08:44.000000 wok_code-2.0.8/wok_code/to_pep8.2p8
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       81 2023-01-27 10:18:10.000000 wok_code-2.0.8/wok_code/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20904 2023-05-20 07:43:28.000000 wok_code-2.0.8/wok_code/cvt_script
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3910 2023-05-20 07:43:28.000000 wok_code-2.0.8/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1730 2023-05-25 08:46:35.000000 wok_code-2.0.8/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    46083 2023-05-25 06:21:25.000000 wok_code-2.0.8/README.rst
```

### Comparing `wok_code-2.0.7/wok_code.egg-info/entry_points.txt` & `wok_code-2.0.8/wok_code.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 do_odoo_site.py = wok_code.scripts.do_odoo_site:main
 gen_readme.py = wok_code.scripts.gen_readme:main
 lint_2_compare = wok_code.scripts.lint_2_compare:main
 makepo_it.py = wok_code.scripts.makepo_it:main
 odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main
 odoo_translation.py = wok_code.scripts.odoo_translation:main
 please = wok_code.scripts.please:main
-run_odoo_debug = odoo_score.scripts.run_odoo_debug:main
+run_odoo_debug = wok_code.scripts.run_odoo_debug:main
 to_pep8.py = wok_code.scripts.to_pep8:main
 wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main
 wok_code-info = wok_code.scripts.main:main
```

### Comparing `wok_code-2.0.7/wok_code.egg-info/SOURCES.txt` & `wok_code-2.0.8/wok_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code.egg-info/PKG-INFO` & `wok_code-2.0.8/wok_code.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wok-code
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `wok_code-2.0.7/wok_code/do_gitignore.py` & `wok_code-2.0.8/wok_code/do_gitignore.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if os.path.isfile(ffn):
             os.rename(ffn, bakfile)
         with open(ffn, 'w') as fd:
             fd.write(target)
             print('Created file %s' % ffn)
 
 
-def main(argv):
+def main(argv=None):
     argv = argv or sys.argv[1:]
     path = None
     for param in argv:
         if param.startswith('-'):
             pass
         else:
             path = os.path.expanduser(param)
@@ -87,8 +87,8 @@
     else:
         print('Path %s does not exist!' % sys.argv[0])
         return 2
     return 0
 
 
 if __name__ == "__main__":
-    exit(main(sys.argv))
+    exit(main())
```

### Comparing `wok_code-2.0.7/wok_code/gen_addons_table.py` & `wok_code-2.0.8/wok_code/gen_addons_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from past.builtins import cmp
 
 standard_library.install_aliases()  # noqa: E402
 
 
 MARKERS = r'(\[//\]: # \(addons\))|(\[//\]: # \(end addons\))'
 MANIFESTS = ('__openerp__.py', '__manifest__.py')
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 class UserError(Exception):
     def __init__(self, msg):
         self.msg = msg
```

### Comparing `wok_code-2.0.7/wok_code/pgconf.py` & `wok_code-2.0.8/wok_code/pgconf.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/tests/test_gen_readme.py` & `wok_code-2.0.8/wok_code/tests/test_gen_readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-#!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # Copyright (C) 2015-2023 SHS-AV s.r.l. (<http://www.zeroincombenze.org>)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 """
     Zeroincombenze® unit test library for python programs Regression Test Suite
 """
 import os
 import sys
 
 from python_plus import _c
 from z0lib import z0lib
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
-MODULE_ID = 'z0bug_odoo'
+MODULE_ID = "z0bug_odoo"
 TEST_FAILED = 1
 TEST_SUCCESS = 0
-ODOO_VERSIONS = ('7.0', '10.0', '12.0')
+ODOO_VERSIONS = ("7.0", "10.0", "12.0")
 
 DESCR_FN = r"""Lorem ipsum
 -----------
 
 Lorem ipsum **dolor** sit amet
 .. \$if branch in '%s'
 consectetur *adipiscing* elit
```

### Comparing `wok_code-2.0.7/wok_code/tests/test_please.py` & `wok_code-2.0.8/wok_code/tests/test_please.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import sys
 
 from z0lib import z0lib
 from zerobug import z0test
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 MODULE_ID = 'wok_code'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `wok_code-2.0.7/wok_code/tests/test_filepo.py` & `wok_code-2.0.8/wok_code/tests/test_filepo.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/tests/test_license_mgnt.py` & `wok_code-2.0.8/wok_code/tests/test_license_mgnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 import os
 import sys
 
 from wok_code.scripts import license_mgnt
 from zerobug import z0test, z0testodoo
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 MODULE_ID = 'devel_tool'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `wok_code-2.0.7/wok_code/ssh.py` & `wok_code-2.0.8/wok_code/ssh.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 def get_remote_user():
     local_user = os.environ['USER']
     user = None
     default_user = None
     for key, item in DATA[host].items():
```

### Comparing `wok_code-2.0.7/wok_code/pypi.sh` & `wok_code-2.0.8/wok_code/pypi.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # set -x
-__version__=2.0.7
+__version__=2.0.8
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
   [[ -d $HOME/odoo/devel ]] && HOME_DEVEL="$HOME/odoo/devel" || HOME_DEVEL="$HOME/devel"
 fi
 
 run_traced() {
     local xcmd="$1"
     local sts=0
@@ -21,14 +21,25 @@
     OPTS=""
     [[ $opts =~ -.*n ]] && OPTS="$OPTS -n"
     echo -e "\n===[$pkg]==="
     [[ $PWD != $srcdir ]] && run_traced "cd $srcdir"
     run_traced "please $OPTS replace"
 }
 
+do_wep() {
+    [[ $pkg =~ (python-plus|z0bug-odoo) ]] && fn=${pkg//-/_} || fn=$pkg
+    srcdir="$HOME_DEVEL/pypi/$fn"
+    OPTS=""
+    [[ $opts =~ -.*n ]] && OPTS="$OPTS -n"
+    echo -e "\n===[$pkg]==="
+    [[ $PWD != $srcdir ]] && run_traced "cd $srcdir"
+    run_traced "please $OPTS wep"
+}
+
+
 act=""
 pypi=""
 opts=""
 tgtdir=""
 branch=""
 prm=""
 
@@ -44,41 +55,43 @@
         [[ $1 =~ -.*b ]] && prm="branch"
         [[ $1 =~ -.*B ]] && opts=${opts}B
         [[ $1 =~ -.*d ]] && prm="tgtdir"
         [[ $1 =~ -.*f ]] && opts=${opts}f
         [[ $1 =~ -.*i ]] && opts=${opts}i
         [[ $1 =~ -.*I ]] && opts=${opts}I
         [[ $1 =~ -.*n ]] && opts=${opts}n
+        [[ $1 =~ -.*q ]] && opts=${opts}q
         [[ $1 =~ -.*U ]] && act="update"
         [[ $1 =~ -.*y ]] && opts=${opts}y
         [[ $1 =~ -.*Z ]] && opts=${opts}Z
     fi
     shift
 done
 [[ -n "$opts" ]] && opts="-$opts"
-HLPCMDLIST="cvt_script|diff|dir|docs|git-add|info|install|libdir|list|meld|replace|show|travis|travis-summary|update|update+replace|version"
+HLPCMDLIST="cvt_script|diff|dir|docs|git-add|info|install|libdir|list|meld|replace|show|travis|travis-summary|update|update+replace|version|wep"
 ACT2VME="^(dir|info|show|install|libdir|update|update\+replace|update)$"
-ACT2TOOLS="^(docs|git-add|list|replace|travis|travis-summary|version)$"
-PKGS_LIST="clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
-PKGS_LIST_RE="(${PKGS_LIST// /|})"
-PKGS_LIST_RE=${PKGS_LIST_RE//-/.}
+ACT2TOOLS="^(docs|git-add|list|replace|travis|travis-summary|version|wep)$"
+LOCAL_PKGS="clodoo lisa odoo_score oerplib3 os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
+LOCAL_PKGS_RE="(${LOCAL_PKGS// /|})"
+LOCAL_PKGS_RE=${LOCAL_PKGS_RE//-/.}
 ODOO_ROOT=$(dirname $HOME_DEVEL)
 [[ -z "$act" || ! $act =~ ($HLPCMDLIST) ]] && act="help"
 [[ $act == "help" ]] && echo "$0 [-h|-B|-f|-I|-l|-n|-U|-y|-Z] [-d VENV] [-b BRANCH] $HLPCMDLIST|help [PYPI_PKG]" && exit 0
 b=$(basename $PWD)
-[[ -z "$pypi" && $(dirname $PWD) == $HOME_DEVEL/pypi/$b && $b =~ $PKGS_LIST_RE ]] && pypi=$b
-[[ -z "$pypi" ]] && pypi="$PKGS_LIST" || pypi="${pypi//,/ }"
+[[ -z "$pypi" && $(dirname $PWD) == $HOME_DEVEL/pypi/$b && $b =~ $LOCAL_PKGS_RE ]] && pypi=$b
+[[ -z "$pypi" ]] && pypi="$LOCAL_PKGS" || pypi="${pypi//,/ }"
 [[ -z "$tgtdir" ]] && tgtdir="$ODOO_ROOT/VME/* $HOME_DEVEL/venv" || tgtdir="$(readlink -f $tgtdir)/*"
 [[ $tgtdir =~ ^[~/.] ]] || tgtdir="$ODOO_ROOT/$tgtdir"
 [[ $act =~ $ACT2TOOLS ]] && tgtdir=$HOME_DEVEL/pypi/tools
 [[ -n $branch ]] && branch="(${branch//,/|})"
 echo "$0 $act '$pypi' -d $tgtdir -b $branch $opts"
 act2=$act
 for d in $tgtdir; do
-    [[ $act =~ "list" ]] && echo "$PKGS_LIST" && run_traced "find $ODOO_ROOT/tools -maxdepth 1 -type d|grep -Ev \"(/|.git|docs|egg-info|license_text|templates|tests|z0tester)$\"|sort|cut -d/ -f5" && continue
+    [[ $act =~ "list" && ! $opts =~ -.*B ]] && echo -e "\n$LOCAL_PKGS" && run_traced "find $ODOO_ROOT/tools -maxdepth 1 -type d|grep -Ev \"(/|.git|.idea|docs|egg-info|license_text|templates|tests|z0tester)$\"|sort|cut -d/ -f5|tr '\n' ' '" && echo "" && continue
+    [[ $act =~ "list" && $opts =~ -.*B ]] && echo -e "\n$LOCAL_PKGS" && run_traced "find $HOME_DEVEL/pypi -maxdepth 1 -type d|grep -Ev \"(/|.git|.idea|docs|egg-info|license_text|templates|tests|z0tester)$\"|sort|cut -d/ -f6|tr '\n' ' '" && echo "" && continue
     if [[ $act =~ $ACT2VME || ( $act =~ (diff|meld) && -n $branch ) ]]; then
         [[ -d "$d" ]] || continue
         [[ -n "$branch" && ! $d =~ $branch ]] && continue
         # [[ $d =~ VME(3.5|3.6) ]] && continue
         echo "[$d]"
         pypath=
         [[ -d $d/lib/python2.7/site-packages ]] && pypath=$d/lib/python2.7/site-packages
@@ -110,15 +123,15 @@
             elif [[ $act =~ (install|update+replace|update) && -n $pypath && -L $pypath/$fn  ]]; then
                 run_traced "rm -f $pypath/$fn"
                 [[ $act == "update" ]] && act2="install"
             fi
             run_traced "vem $d $act2 $pkg2 $OPTS"
         elif [[ $act == "dir" ]]; then
             srcdir=$(vem $d show $pkg 2>/dev/null|grep "[Ll]ocation:"|awk -F: '{print $2}')
-            [[ -n $srcdir ]] && run_traced "dir -lh $srcdir/$fn"|| echo "No ptah found for $pkg"
+            [[ -n $srcdir ]] && run_traced "dir -lh $srcdir/$fn"|| echo "No path found for $pkg"
         elif [[ $act == "libdir" ]]; then
             run_traced "ls -d $pypath/$fn"
 	      elif [[ $act =~ (travis|travis-summary) ]]; then
 	          [[ $pkg == "tools" ]] && continue
             srcdir="$HOME_DEVEL/pypi/$fn/$fn"
             OPTS=""
             [[ $opts =~ -.*n ]] && OPTS="$OPTS -n"
@@ -163,14 +176,16 @@
             [[ $opts =~ -.*n ]] && OPTS="${OPTS}n"
             [[ $opts =~ -.*y ]] && OPTS="${OPTS}y"
             for f in $(find $srcdir -type f); do
                 mime=$(file --mime-type -b $f)
                 [[ $mime == "text/x-shellscript" || $f =~ .sh$ ]] || continue
                 run_traced "cvt_script $OPTS $f"
             done
+        elif [[ $act == "wep" ]]; then
+            do_wep
         else
             echo "Invalid command!"
             exit 1
         fi
     done
     [[ ! $act =~ $ACT2VME ]] && break
 done
```

### Comparing `wok_code-2.0.7/wok_code/cvt_csv_2_xml.py` & `wok_code-2.0.8/wok_code/cvt_csv_2_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.7/wok_code/scripts/please.sh` & `wok_code-2.0.8/wok_code/scripts/please.sh`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # please
 # Developer shell
 #
 # This free software is released under GNU Affero GPL3
 # author: Antonio M. Vigliotti - antoniomaria.vigliotti@gmail.com
 # (C) 2015-2023 by SHS-AV s.r.l. - http://www.shs-av.com - info@shs-av.com
 #
-# set -x  #debug
 READLINK=$(which greadlink 2>/dev/null) || READLINK=$(which readlink 2>/dev/null)
 export READLINK
 # Based on template 2.0.0
 THIS=$(basename "$0")
 TDIR=$(readlink -f $(dirname $0))
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
 if [[ -z $HOME_DEVEL || ! -d $HOME_DEVEL ]]; then
@@ -407,27 +406,27 @@
   local sts=$STS_SUCCESS
   local rpt=$1
   local n p s v
   [[ -z $rpt || ! $rpt =~ (pypi|testpypi) ]] && rpt=pypi
   if [[ "$PRJNAME" != "Odoo" ]]; then
     if twine --version &>/dev/null; then
       run_traced "cd $PKGPATH"
-      s=$?; [ ${s-0} -ne 0 ] && sts=$s
-      [[ -f $PRJPATH/README.rst ]] && run_traced "cp $PRJPATH/README.rst ./"
+      s=$?; [[ ${s-0} -ne 0 ]] && sts=$s
+      [[ -f $PRJPATH/README.rst ]] && run_traced "mv $PRJPATH/README.rst ./"
       v=$(python setup.py --version)
       n=$(python setup.py --name)
       p=$(find dist -name "${n}-${v}.tar.gz")
       if [[ -z "$p" || $opt_force -gt 0 ]]; then
         run_traced "python setup.py build sdist"
-        s=$?; [ ${s-0} -ne 0 ] && sts=$s
+        s=$?; [[ ${s-0} -ne 0 ]] && sts=$s
       fi
       p=$(find dist -name "${n}-${v}.tar.gz")
       [[ -z $p ]] && echo "Internal error: file tar not found!" && return 127
       run_traced "twine upload $p -r $rpt"
-      s=$?; [ ${s-0} -ne 0 ] && sts=$s
+      s=$?; [[ ${s-0} -ne 0 ]] && sts=$s
     else
       echo "Command twine not found!"
       echo "Do pip install twine"
       sts=1
     fi
   fi
   return $sts
@@ -616,119 +615,14 @@
       echo "File $f not found"
       break
     fi
   done
   return $s
 }
 
-#do_build() {
-#  #do_build pgkname tar
-#  local sts=$STS_SUCCESS
-#  local rpt=pypi
-#  local f i l n p s v x y PKGLIST invalid PASSED
-#  local SETUP=./setup.sh
-#  local xx="$(get_cfg_value 0 filedel)"
-#  local yy="$(get_cfg_value 0 fileignore)"
-#  if [ $opt_keep -ne 0 ]; then
-#    xx="$xx $yy"
-#  else
-#    xx="$xx $yy tests/"
-#  fi
-#  if [ "$PRJNAME" != "Odoo" ]; then
-#    run_traced "cd $PKGPATH"
-#    # run_traced "mkdir -p tmp"
-#    s=$?; [ ${s-0} -ne 0 ] && sts=$s
-#    n=$(cat setup.py | grep "name *=" | awk -F= '{print $2}' | grep --color=never -Eo '[a-zA-Z0-9_-]+' | head -n1)
-#    v=$(cat setup.py | grep version | grep --color=never -Eo '[0-9]+\.[0-9]+\.[0-9]+' | head -n1)
-#    if [ ! -f "$n*$v*tar.gz" -o $opt_force -gt 0 ]; then
-#      PKGLIST=$(cat setup.py | grep "# PKGLIST=" | awk -F= '{print $2}')
-#      if [ -n "$PKGLIST" ]; then
-#        PKGLIST=${PKGLIST//,/ }
-#      else
-#        if [ "$PRJNAME" == "lisa" ]; then
-#          cp ../../clodoo/clodoo/odoorc ./
-#          cp ../../z0lib/z0lib/z0librc ./
-#        fi
-#        x="find . -type f"
-#        for f in $xx "setup.*"; do
-#          if [ "${f: -1}" == "/" ]; then
-#            x="$x -not -path '*/$f*'"
-#          else
-#            x="$x -not -name '*$f'"
-#          fi
-#        done
-#        eval $x >./tmp.log
-#        PKGLIST="$(cat ./tmp.log)"
-#        rm -f ./tmp.log
-#      fi
-#      invalid=
-#      for f in $PKGLIST; do
-#        if [ -f $f ]; then
-#          :
-#          #cp $f $PKGPATH/tmp
-#        else
-#          invalid=$f
-#        fi
-#      done
-#      if [ -n "$invalid" ]; then
-#        echo "File $f not found"
-#        return 1
-#      fi
-#      p="$n-$v.tar.gz"
-#      if [ -f $p ]; then
-#        run_traced "rm -f $p"
-#      fi
-#      echo "# $p" >$SETUP
-#      f=
-#      for i in {2..9}; do
-#        x=$(echo $PRJPATH | awk -F/ '{print $'$i'}')
-#        if [ -n "$x" ]; then
-#          f=$f/$x
-#          if [ $i -gt 3 ]; then
-#            echo "mkdir -p $f" >>$SETUP
-#          fi
-#        fi
-#      done
-#      l=${#PKGPATH}
-#      f=".${PRJPATH:l}" # subroot
-#      l=${#f}
-#      ((l++))
-#      PASSED=
-#      x="-cf"
-#      for f in $PKGLIST; do
-#        y=$(dirname ./${f:l})
-#        if [ "$y" != "." ]; then
-#          y=$(dirname ${f:l})
-#          if [[ " $PASSED " =~ [[:space:]]$y[[:space:]] ]]; then
-#            :
-#          else
-#            echo "mkdir -p $PRJPATH/$y" >>$SETUP
-#            PASSED="$PASSED $y"
-#          fi
-#          y=$y/
-#        else
-#          y=
-#        fi
-#        run_traced "tar $x $p $f"
-#        x=${x/c/r}
-#        # if [ -f "$f" ]; then rm -f $f; fi
-#        echo "cp -p $f $PKGPATH/$y" >>$SETUP
-#      done
-#      chmod +x $SETUP
-#      if [ -x $PRJPATH/setup.sh ]; then
-#        run_traced "cp $PRJPATH/setup.sh $SETUP"
-#      fi
-#      run_traced "tar $x $p $SETUP"
-#      run_traced "rm -f $SETUP"
-#    fi
-#  fi
-#  return $sts
-#}
-
-
 do_docs() {
   wlog "do_docs"
   local docs_dir=./docs
   local author version theme SETUP b f l t x
   local opts src_png odoo_fver REPO
   [[ $opt_dbg -ne 0 || $PWD =~ /devel/pypi/ ]] && opts=-B || opts=
   if [ "$PRJNAME" == "Odoo" ]; then
@@ -1482,22 +1376,22 @@
     done
   fi
   return 0
 }
 #
 #do_show_status() {
 #  local s v1 v2 v x y
-#  local PKGS_LIST=$(get_cfg_value 0 "PKGS_LIST")
+#  local LOCAL_PKGS=$(get_cfg_value 0 "LOCAL_PKGS")
 #  pushd $HOME/tools >/dev/null
 #  local PKGS=$(git status -s | grep -E "^ M" | awk '{print $2}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
 #  local PKGS_V=$(git diff -G__version__ --compact-summary | awk '{print $1}' | awk -F/ '{print $1}' | grep -v "^[0-9]" | sort -u | tr "\n" "|")
 #  [[ -n "$PKGS" ]] && PKGS="(${PKGS:0:-1})" || PKGS="()"
 #  [[ -n "$PKGS_V" ]] && PKGS_V="(${PKGS_V:0:-1})" || PKGS_V="()"
 #  popd >/dev/null
-#  for pkg in $PKGS_LIST tools; do
+#  for pkg in $LOCAL_PKGS tools; do
 #    x=""
 #    [[ $opt_force -ne 0 ]] && echo -e "\e[1m[ $pkg ]\e[0m"
 #    [[ $opt_force -eq 0 ]] && echo -e "[ $pkg ]"
 #    [[ $pkg =~ (python-plus|z0bug-odoo) ]] && pkg="${pkg//-/_}"
 #    if [[ $pkg == "tools" ]]; then
 #      for fn in egg-info licence_text templates .travis.yml install_tools.sh odoo_default_tnl.xlsx setup.py; do
 #        vfdiff -X diff $HOME/$pkg/$fn $HOME_DEVEL/pypi/$pkg/$fn -q >/dev/null
@@ -1686,17 +1580,18 @@
     "© 2015-2023 by zeroincombenze®\nhttps://zeroincombenze-tools.readthedocs.io/\nAuthor: antoniomaria.vigliotti@gmail.com"
   exit 0
 fi
 
 ACT2VME="^(dir|info|show|install|libdir|update|update\+replace|update)$"
 ACT2PYPI="^(docs|git-add|list|replace|travis|travis-summary|version)$"
 ACT2TOOLS="^(docs|git-add|list|replace|travis|travis-summary|version)$"
-PKGS_LIST="clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
-PKGS_LIST_RE="(${PKGS_LIST// /|})"
-PKGS_LIST_RE=${PKGS_LIST_RE//-/.}
+# LOCAL_PKGS="clodoo lisa odoo_score os0 python-plus travis_emulator wok_code z0bug-odoo z0lib zar zerobug"
+LOCAL_PKGS=$(find $HOME_DEVEL/pypi -maxdepth 1 -type d|grep -Ev "(/|.git|.idea|docs|egg-info|license_text|templates|tools|tests|z0tester)$"|sort|cut -d/ -f6)
+LOCAL_PKGS_RE="(${LOCAL_PKGS// /|})"
+LOCAL_PKGS_RE=${LOCAL_PKGS_RE//-/.}
 
 # opts_travis
 conf_default
 [[ $opt_verbose -gt 2 ]] && set -x
 
 sts=$STS_SUCCESS
 sts_bash=127
@@ -1719,15 +1614,15 @@
   actions=${actions//,/ }
   for action in $actions; do
     [[ "${action:0:3}" == "if-" ]] && opt_dry_run=1 && cmd="do_${action:3}"
     cmd="do_${action/-/_}"
     if [[ "$(type -t $cmd)" == "function" ]]; then
       if [[ $PRJNAME == "pypi" && $PKGNAME == "pypi" ]]; then
         [[ ! $action =~ $ACT2PYPI ]] && echo "Action $action not applicable on this directory" && continue
-        [[ $action =~ $ACT2TOOLS ]] && pkgs_list="$PKGS_LIST tools" || pkgs_list="$PKGS_LIST"
+        [[ $action =~ $ACT2TOOLS ]] && pkgs_list="$LOCAL_PKGS tools" || pkgs_list="$LOCAL_PKGS"
         for fn in $pkgs_list; do
           echo -e "\n===[$fn]==="
           pfn="${fn/-/_}"
           [[ $fn == "tools" ]] && run_traced "pushd $HOME_DEVEL/pypi/$pfn >/dev/null" || run_traced "pushd $HOME_DEVEL/pypi/$pfn/$pfn >/dev/null"
           eval $cmd "'$sub1'" "'$sub2'" "'$sub3'"
           sts=$?
           run_traced "popd >/dev/null"
```

### Comparing `wok_code-2.0.7/wok_code/scripts/to_pep8.py` & `wok_code-2.0.8/wok_code/scripts/to_pep8.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 except ImportError:
     import z0lib
 try:
     from python_plus.python_plus import _c, _u
 except ImportError:
     from python_plus import _c, _u
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 LICENSES = ('gpl', 'agpl', 'lgpl', 'opl', 'oee')
 METAS = ('0', '6.1', '7.0', '8.0', '9.0', '10.0', '11.0', '12.0', '13.0', '14.0')
 AUTHORS_TEMPLATE = """
 * LibrERP enterprise network <LibrERP-network>
 * SHS-AV s.r.l. <https://www.zeroincombenze.it>
 * Didotech s.r.l. <https://www.didotech.com>
```

### Comparing `wok_code-2.0.7/wok_code/scripts/setup.info` & `wok_code-2.0.8/wok_code/scripts/setup.info`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.7',
+    version='2.0.8',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -87,12 +87,12 @@
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
             'to_pep8.py = wok_code.scripts.to_pep8:main',
             'wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main',
-            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
+            'run_odoo_debug = wok_code.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `wok_code-2.0.7/wok_code/scripts/main.py` & `wok_code-2.0.8/wok_code/scripts/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `wok_code-2.0.7/wok_code/scripts/makepo_it.py` & `wok_code-2.0.8/wok_code/scripts/makepo_it.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from __future__ import print_function
 
 import os.path
 import sys
 import argparse
 # import pdb
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 PO_DEFAULT = """
 # Translation of Odoo Server.
 # This file contains the translation of the following modules:
 #   * MODULE
 #
 msgid ""
```

### Comparing `wok_code-2.0.7/wok_code/scripts/cvt_csv_coa.py` & `wok_code-2.0.8/wok_code/scripts/cvt_csv_coa.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import argparse
 import time
 
 from os0 import os0
 from python_plus import unicodes
 from clodoo import transodoo
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 msg_time = time.time()
 VALID_ACTIONS = ("export-comparable", "export-full", "export-z0bug", "export-group")
 VERSIONS = ["6.1", "7.0", "8.0", "9.0", "10.0", "11.0", "12.0", "13.0", "14.0"]
 
 
 class CvtCsvFile(object):
```

### Comparing `wok_code-2.0.7/wok_code/scripts/run_odoo_debug.py` & `wok_code-2.0.8/wok_code/scripts/run_odoo_debug.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/scripts/dist_pkg.sh` & `wok_code-2.0.8/wok_code/scripts/dist_pkg.sh`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 # main
 OPTOPTS=(h        C         c        D        F         f         n            O         o        P         p         q           R         S        u       V           v           W          w         -)
 OPTDEST=(opt_help opt_cpush opt_conf opt_push opt_fetch opt_force opt_dry_run  opt_cpush opt_ids  opt_cpush opt_dpath opt_verbose opt_cpush opt_sts  opt_upd opt_version opt_verbose opt_whatis opt_cpush opt_sync)
 OPTACTI=("+"      "*>"      "="      "*>"     "1>"      1         1            "*>"      "=>"     "*>"      "="       0           "*>"      "=>"     1       "*"         "+"         "=>"       "*>"      "1>")
 OPTDEFL=(1        ""        ""       ""       0         0         0            ""        ""       ""        ""        0           ""        ""       0       ""          -1          ""         ""        0)
 OPTMETA=("help"   "commit"  "file"   ""       "fetch"   ""        "do nothing" ""        "prj_id" "push"    "path"    "quiet"     "replace" "status" "upd"   "version"   "verbose"   "param"    "wep"     "sync")
@@ -369,11 +369,14 @@
 [[ ! -d $LGITPATH ]] && echo "Destination path $LGITPATH not found!" && exit $STS_FAILED
 robocopy_init "$PRJNAME" "$PKGNAME"
 if [[ $opt_fetch -eq 0 ]]; then
   [[ $PKGNAME != "tools" ]] &&  run_traced "cp $PKGPATH/setup.py $PRJPATH/scripts/setup.info"
   [[ -f $PRJPATH/setup.py && -f $PRJPATH/scripts/setup.info ]] &&  run_traced "rm -f $PRJPATH/setup.py"
   [[ -x $PRJPATH/replace.sh ]] && run_traced "$PRJPATH/replace.sh"
   [[ ! -x $PRJPATH/replace.sh ]] && robocopy "$PRJPATH" "$LGITPATH"
-  [[ $PKGNAME != "tools" && -f $PKGPATH/setup.py ]] &&  run_traced "cp $PKGPATH/setup.py $LGITPATH/setup.py"
-  [[ -f "$PRJPATH/scripts/setup.info" ]] &&  run_traced "cp $PRJPATH/scripts/setup.info $LGITPATH/scripts/setup.info"
+  if [[ $PKGNAME != "tools" ]]; then
+    [[ -f $PKGPATH/setup.py ]] &&  run_traced "cp $PKGPATH/setup.py $LGITPATH/setup.py"
+    [[ -f $PKGPATH/README.rst ]] &&  run_traced "cp $PKGPATH/README.rst $LGITPATH/README.rst"
+    [[ -f "$PRJPATH/scripts/setup.info" ]] &&  run_traced "cp $PRJPATH/scripts/setup.info $LGITPATH/scripts/setup.info"
+  fi
 fi
 exit $STS_SUCCESS
```

### Comparing `wok_code-2.0.7/wok_code/scripts/generate_random_codes.py` & `wok_code-2.0.8/wok_code/scripts/generate_random_codes.py`

 * *Files identical despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 # import os
 import argparse
 from random import random, randint
 import vatnumber
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 def gen_vatnumber(opt_args):
     found = False
     while not found:
         seed = "%7.7s%3.03i" % (random() * 10000000, randint(1, 99))
         for i in range(10):
```

### Comparing `wok_code-2.0.7/wok_code/scripts/run_odoo_debug.sh` & `wok_code-2.0.8/wok_code/scripts/run_odoo_debug.sh`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 run_traced_debug() {
     if [[ $opt_verbose -gt 1 ]]; then
         run_traced "$1"
     elif [[ $opt_dry_run -eq 0 ]]; then
         eval $1
     fi
@@ -102,16 +102,14 @@
       [[ $v -ge 6 ]] && coverage report --rcfile=$COVERAGE_PROCESS_START --data-file=$COVERAGE_DATA_FILE $opts -m || coverage report --rcfile=$COVERAGE_PROCESS_START $opts -m
     fi
 }
 
 set_log_filename() {
     # UDI (Unique DB Identifier): format "{pkgname}_{git_org}{major_version}"
     # UMLI (Unique Module Log Identifier): format "{git_org}{major_version}.{repos}.{pkgname}"
-    # set -x  #debug
-    # local odoo_ver=$(build_odoo_param MAJVER ${BRANCH})
     local m
     [[ -n $opt_modules ]] && m="${opt_modules//,/+}" || m="$PKGNAME"
     [[ -z $GIT_ORGID ]] && GIT_ORGID="$(build_odoo_param GIT_ORGID '.')"
     [[ -n $ODOO_GIT_ORGID && $GIT_ORGID =~ $ODOO_GIT_ORGID ]] && UDI="$m" || UDI="$m_${GIT_ORGID}"
     [[ $PRJNAME == "Odoo" && -n $UDI ]] && UDI="${UDI}_${odoo_ver}"
     [[ $PRJNAME == "Odoo" && -z $UDI ]] && UDI="${odoo_ver}"
     [[ $PRJNAME == "Odoo" ]] && UMLI="${GIT_ORGID}${odoo_ver}" || UMLI="${GIT_ORGID}"
@@ -291,24 +289,25 @@
 [[ -z $odoo_root || ! -d $odoo_root ]] && echo "Odoo path $odoo_root not found!" && exit 1
 odoo_ver=$(build_odoo_param MAJVER $odoo_fver)
 LCONFN=$(build_odoo_param LCONFN $odoo_fver)
 script=$(build_odoo_param BIN "$odoo_root" search)
 [[ -z "$script" ]] && echo "No odoo script found!!" && exit 1
 ODOO_RUNDIR=$(dirname $script)
 VDIR=$(build_odoo_param VDIR "$odoo_root")
+[[ ! -d $VDIR ]] && VDIR=""
 [[ $opt_verbose -gt 1 && -n "$VDIR" ]] && echo "# Found $VDIR virtual directory"
 set_log_filename
 
 if [[ -n $opt_rport ]]; then
     RPCPORT=$opt_rport
 elif [[ $opt_test -ne 0 ]]; then
     [[ opt_dbg -gt 1 ]] && RPCPORT=$(build_odoo_param RPCPORT $odoo_fver DEBUG) || RPCPORT=$((($(date +%s) % 46000) + 19000))
 elif [[ -f $opt_conf ]]; then
-    RPCPORT=$(grep ^xmlrpc_port $CONFN | awk -F= '{print $2}' | tr -d " ")
-    [[ -z "$RPCPORT" ]] && RPCPORT=$(grep ^http_port $CONFN | awk -F= '{print $2}' | tr -d " ")
+    RPCPORT=$(grep ^http_port $CONFN | awk -F= '{print $2}' | tr -d " ")
+    [[ -z "$RPCPORT" ]] && RPCPORT=$(grep ^xmlrpc_port $CONFN | awk -F= '{print $2}' | tr -d " ")
 elif [[ $opt_web -ne 0 ]]; then
     RPCPORT=$(build_odoo_param RPCPORT $odoo_fver $GIT_ORGID)
 elif [[ -f $CONFN ]]; then
     RPCPORT=$(grep ^xmlrpc_port $CONFN | awk -F= '{print $2}' | tr -d " ")
     [[ -z "$RPCPORT" ]] && RPCPORT=$(grep ^http_port $CONFN | awk -F= '{print $2}' | tr -d " ")
 else
     RPCPORT=$(build_odoo_param RPCPORT $odoo_fver $GIT_ORGID)
```

### Comparing `wok_code-2.0.7/wok_code/scripts/wget_odoo_repositories.py` & `wok_code-2.0.8/wok_code/scripts/wget_odoo_repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #     from z0lib.z0lib import z0lib
 # except ImportError:
 #     try:
 #         from z0lib import z0lib
 #     except ImportError:
 #         import z0lib
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 ROOT_URL = 'https://api.github.com/repos/zeroincombenze/'
 USER_URL = 'https://api.github.com/users/'
 REPNAME_ACC_CLO = 'OCB'
 DEVEL_REPS = [
     'Odoo-samples',
     'VME',
```

### Comparing `wok_code-2.0.7/wok_code/scripts/config/to_new_api.yml` & `wok_code-2.0.8/wok_code/scripts/config/to_new_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/scripts/config/to_old_api.yml` & `wok_code-2.0.8/wok_code/scripts/config/to_old_api.yml`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/scripts/please_apache.py` & `wok_code-2.0.8/wok_code/scripts/please_apache.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 APACHE_TEMPLATE = """##################################################################
 # Odoo service %(odoo_branch)s
 # Domain: <%(protocol)s://%(domain)s>
 #
 <VirtualHost *:%(apache_port)s>
     ServerAdmin %(email)s
```

### Comparing `wok_code-2.0.7/wok_code/scripts/dist_pkg.py` & `wok_code-2.0.8/wok_code/scripts/dist_pkg.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/scripts/do_migrate.py` & `wok_code-2.0.8/wok_code/scripts/do_migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import argparse
 import re
 import lxml.etree as ET
 import yaml
 from python_plus import _b
 from z0lib import z0lib
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 # RULES: every rule is list has the following format:
 # EREGEX, (ACTION, PARAMETERS), ...
 # where
 # - EREGEX is an enhanced regular expression to apply the rule.
 # - ACTION is the action to apply on current line
 # - PARAMETERS are the values to supply on action
@@ -366,15 +366,15 @@
             self.ctr_tag_odoo -= 1
         return True, offset
 
     def matches_utf8(self, nro):
         offset = 0
         if (
             self.opt_args.python_ver
-            and self.opt_args.python_ver.startswith("2")
+            and self.py23 == 2 or self.python_future
             and self.utf8_decl_nro < 0
         ):
             self.utf8_decl_nro = nro
         else:
             del self.lines[nro]
             offset = -1
         return False, offset
@@ -656,19 +656,23 @@
             path = os.path.dirname(path)
         if self.is_xml:
             if prettier_config:
                 cmd = ("npx prettier --plugin=@prettier/plugin-xml --config=%s"
                        % prettier_config)
             else:
                 cmd = "npx prettier --plugin=@prettier/plugin-xml --print-width=88"
-            cmd = cmd + " --no-xml-self-closing-space --tab-width=4 --write "
+            cmd += " --no-xml-self-closing-space --tab-width=4 --prose-wrap=always"
+            cmd += " --write "
             cmd += out_ffn
             z0lib.run_traced(cmd)
         else:
-            cmd = "black --skip-string-normalization -q %s" % out_ffn
+            opts = "--skip-source-first-line"
+            if self.py23 == 2 or self.python_future:
+                opts += " --skip-string-normalization"
+            cmd = "black %s -q %s" % (opts, out_ffn)
             z0lib.run_traced(cmd)
 
     def close(self):
         if self.opt_args.output:
             if os.path.isdir(self.opt_args.output):
                 out_ffn = os.path.join(self.opt_args.output,
                                        os.path.basename(self.ffn))
```

### Comparing `wok_code-2.0.7/wok_code/scripts/odoo_translation_old.py` & `wok_code-2.0.8/wok_code/scripts/odoo_translation_old.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 MAX_RECS = 100
 PUNCT = [' ', '.', ',', '!', ':']
 TNL_DICT = {}
 TNL_ACTION = {}
 SYNTAX = {'string': re.compile('"([^"\\\n]|\\.|\\\n)*"')}
 VERSIONS = ('16.0', '15.0', '14.0', '13.0', '12.0', '11.0',
```

### Comparing `wok_code-2.0.7/wok_code/scripts/gen_readme.py` & `wok_code-2.0.8/wok_code/scripts/gen_readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,20 +113,21 @@
     from python_plus.python_plus import _b, _c, _u
 except ImportError:
     from python_plus import _b, _c, _u
 # import pdb
 standard_library.install_aliases()
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 RED = "\033[1;31m"
 GREEN = "\033[1;32m"
 YELLOW = "\033[1;33m"
 CLEAR = "\033[0;m"
+RMODE = "rU" if sys.version_info[0] == 2 else "r"
 GIT_USER = {
     "zero": "zeroincombenze",
     "oca": "OCA",
     "powerp": "PowERP-cloud",
     "didotech": "didotech",
 }
 DEFINED_SECTIONS = [
@@ -250,15 +251,15 @@
     "ù": "&ugrave;",
     "ú": "&uacute;",
 }
 RST2HTML_GRYMB = {
     "|check|": '<span class="fa fa-check-square-o" style="color:green"/>',
     "|no_check|": '<span class="fa fa-close" style="color:red"/>',
     "|menu|": '<span class="fa fa-navicon"/>',
-    "|right_do|": '<span class="fa fa-caret-right"/>',
+    '|right_do|': "<span class='fa fa-caret-right'/>",
     "|exclamation|": '<span class="fa fa-exclamation" style="color:orange"/>',
     "|late|": '<span class="fa fa-calendar-times-o" style="color:red"/>',
     "|same|": '<span class="fa fa-retweet"  style="color:blue"/>',
     "|warning|": '<span class="fa fa-exclamation-triangle" style="color:orange"/>',
     "|info|": '<span class="fa fa-info-circle" style="color:blue"/>',
     "|halt|": '<span class="fa fa-minus-circle" style="color:red"/>',
     "|circle|": '<span class="fa fa-circle"/>',
@@ -332,25 +333,32 @@
         if full_fn.endswith(".rst"):
             full_fn = os.path.join(
                 os.path.dirname(full_fn),
                 "%s.rst" % os.path.basename(full_fn)[0:-4].upper(),
             )
             if os.path.isfile(full_fn):
                 return True, full_fn
+        if template.startswith("history."):
+            full_fn = os.path.join(
+                os.path.dirname(full_fn),
+                "CHANGELOG.rst",
+            )
+            if os.path.isfile(full_fn):
+                return True, full_fn
         return False, full_fn
 
     def search_tmpl(ctx, template, body):
         found = False
         if body:
             layered_template = "%s_%s" % (ctx["odoo_layer"], template)
             product_template = "%s_%s" % (ctx["product_doc"], template)
         else:
             layered_template = product_template = False
         for src_path in iter_template_path(
-            ctx, debug_mode=ctx["dbg_template"], body=body
+            ctx, debug_mode=ctx["debug_template"], body=body
         ):
             if body:
                 full_fn = get_full_fn(ctx, src_path, product_template)
                 if os.path.isfile(full_fn):
                     found = True
                     break
                 found, full_fn = alternate_name(full_fn)
@@ -367,15 +375,15 @@
             if os.path.isfile(full_fn):
                 found = True
                 break
             found, full_fn = alternate_name(full_fn)
             if found:
                 break
             if template == "acknowledges.txt":
-                full_fn = get_full_fn(ctx, src_path, "contributors.txt")
+                full_fn = get_full_fn(ctx, src_path, "CONTRIBUTORS.txt")
                 if os.path.isfile(full_fn):
                     found = True
                     break
         if not body and not found:
             full_fn = ""
         return found, full_fn
 
@@ -411,19 +419,18 @@
 .. $fi
 .. $if branch in '6.1' '7.0' '8.0' '9.0' '10.0'
 * python 2.7+ (best 2.7.5+)
 * postgresql 9.2+ (best 9.5)
 .. $fi
 """
     if os.path.isfile(os.path.join(ctx["path_name"], "requirements.txt")):
-        fd = open(os.path.join(ctx["path_name"], "requirements.txt"), "rU")
-        for pkg in _u(fd.read()).split("\n"):
-            if pkg and pkg[0] != "#":
-                text += "* %s\n" % pkg.strip()
-        fd.close()
+        with open(os.path.join(ctx["path_name"], "requirements.txt"), RMODE) as fd:
+            for pkg in _u(fd.read()).split("\n"):
+                if pkg and pkg[0] != "#":
+                    text += "* %s\n" % pkg.strip()
     return text
 
 
 def get_default_available_addons(ctx):
     if "addons_info" not in ctx:
         return ""
     text = ""
@@ -1282,15 +1289,15 @@
     full_fn_csv = False
     if full_fn.endswith(".csv"):
         full_fn_csv = full_fn
         full_fn = "%s.rst" % full_fn_csv[:-4]
         os.system(
             "cvt_csv_2_rst.py -b %s -q %s %s" % (ctx["branch"], full_fn_csv, full_fn)
         )
-    with open(full_fn, "r") as fd:
+    with open(full_fn, RMODE) as fd:
         source = _u(fd.read())
     if full_fn_csv:
         os.unlink(full_fn)
     if len(source) and filename == "acknowledges.txt":
         state, source1 = parse_source(
             ctx, source.replace("branch", "prior_branch"), state=state
         )
@@ -1307,52 +1314,52 @@
     if len(source):
         if ctx["trace_file"]:
             mark = '.. !! from "%s"\n\n' % filename
             source = mark + source
         full_hfn = get_template_fn(ctx, "header_" + filename)
         header = ""
         if full_hfn:
-            fd = open(full_hfn, "rU")
+            fd = open(full_hfn, RMODE)
             header = _u(fd.read())
             fd.close()
             if len(header) and ctx["trace_file"]:
                 mark = '.. !! from "%s"\n\n' % full_hfn
                 header = mark + header
         full_ffn = get_template_fn(ctx, "footer_" + filename)
         footer = ""
         if full_ffn:
-            fd = open(full_ffn, "rU")
+            fd = open(full_ffn, RMODE)
             footer = _u(fd.read())
             fd.close()
             if len(footer) and ctx["trace_file"]:
                 mark = '.. !! from "%s"\n\n' % full_ffn
                 footer = mark + footer
         source = header + source + footer
     return parse_source(ctx, source, state=state)
 
 
 def read_manifest_file(ctx, manifest_path, force_version=None):
     try:
-        manifest = ast.literal_eval(open(manifest_path).read())
+        manifest = ast.literal_eval(open(manifest_path, RMODE).read())
     except (ImportError, IOError, SyntaxError):
         raise Exception("Wrong manifest file %s" % manifest_path)
     if force_version:
         manifest["version"] = adj_version(ctx, manifest.get("version", ""))
     return unicodes(manifest)
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_history(ctx, full_fn, module=None):
     if module:
-        with open(full_fn, "r") as fd:
+        with open(full_fn, RMODE) as fd:
             ctx["histories"] += tail(_u(fd.read()), max_days=60, module=module)
-    with open(full_fn, "r") as fd:
+    with open(full_fn, RMODE) as fd:
         ctx["history-summary"] += tail(
             _u(fd.read()), max_ctr=1, max_days=15, module=module
         )
 
 
 def read_setup(ctx):
     if ctx["product_doc"] == "pypi":
@@ -1361,21 +1368,29 @@
         MANIFEST_LIST = ("./setup.py",)
     for manifest in MANIFEST_LIST:
         manifest_filename = os.path.abspath(os.path.join(ctx["path_name"], manifest))
         if os.path.isfile(manifest_filename):
             break
         manifest_filename = ""
     if manifest_filename:
-        with open(manifest_filename, "r") as fd:
-            content = _b(
-                fd.read()
-                .replace("setup(", "fake_setup(")
-                .replace("setup (", "fake_setup(")
-            )
-            exec(content)
+        if ctx["odoo_layer"] == "module" and ctx["rewrite_manifest"]:
+            complete_setup(ctx, manifest_filename)
+        with open(manifest_filename, RMODE) as fd:
+            content = fd.read()
+            content = re.sub(r"setup *\(", "fake_setup(", content)
+            if (
+                "README.rst" in content
+                and not os.path.isfile("../README.rst")
+                and not os.path.isfile("README.rst")
+            ):
+                with open("../README.rst", "w"):
+                    pass
+            if os.path.isfile("../README.rst"):
+                content = content.replace("README.rst", "../README.rst")
+            exec(_b(content))
             ctx["manifest"] = globals()["setup_args"]
         ctx["manifest_filename"] = manifest_filename
     else:
         if not ctx["suppress_warning"]:
             print_red_message("*** Warning: manifest file not found!")
         ctx["manifest"] = {}
     ctx["history-summary"] = ""
@@ -1389,15 +1404,15 @@
                 if os.path.isfile(full_fn):
                     read_history(ctx, full_fn, module=os.path.basename(dir))
         ctx["histories"] = sort_history(ctx["histories"])
         ctx["history-summary"] = sort_history(ctx["history-summary"])
     else:
         full_fn = os.path.join(".", "egg-info", "history.rst")
         if os.path.isfile(full_fn):
-            with open(full_fn, "r") as fd:
+            with open(full_fn, RMODE) as fd:
                 read_history(ctx, full_fn)
 
 
 def read_manifest(ctx):
     if ctx["odoo_layer"] != "module":
         ctx["manifest"] = {}
         return
@@ -1480,19 +1495,19 @@
                         addons_info[module_name]["installable"] = False
                     if module2search:
                         break
                 except KeyError:
                     pass
                 full_fn = os.path.join(root, "egg-info", "history.rst")
                 if os.path.isfile(full_fn):
-                    with open(full_fn, "r") as fd:
+                    with open(full_fn, RMODE) as fd:
                         ctx["histories"] += tail(
                             _u(fd.read()), max_days=180, module=module_name
                         )
-                        with open(full_fn, "r") as fd:
+                        with open(full_fn, RMODE) as fd:
                             ctx["history-summary"] += tail(
                                 _u(fd.read()),
                                 max_ctr=1,
                                 max_days=15,
                                 module=module_name,
                             )
     if not module2search:
@@ -1626,15 +1641,15 @@
     ctx["manifest"] = saved_manifest
 
 
 def manifest_contents(ctx):
     full_fn = ctx["manifest_filename"]
     source = ""
     if full_fn:
-        fd = open(full_fn, "r")
+        fd = open(full_fn, RMODE)
         source = _u(fd.read())
         fd.close()
     target = ""
     for line in source.split("\n"):
         if not line or line[0] != "#":
             break
         target += line + "\n"
@@ -1676,15 +1691,15 @@
             print_red_message(
                 "*** Warning: manifest %s %s does not match required %s!"
                 % (item, ctx["manifest"][item], AUTHINFO[item])
             )
             print("Use -W switch to force required value!")
         elif item == "depends":
             modules = []
-            for module in ctx["manifest"][item]:
+            for module in ctx["manifest"].get(item, []):
                 new_module = transodoo.translate_from_to(
                     ctx,
                     "ir.module.module",
                     module,
                     ctx["from_version"],
                     ctx["odoo_vid"],
                     ttype="module"
@@ -1776,18 +1791,24 @@
         ctx["dst_file"] = ctx["output_file"]
     elif ctx["write_html"]:
         if os.path.isdir("./static/description"):
             ctx["dst_file"] = "./static/description/index.html"
         else:
             ctx["dst_file"] = "./index.html"
         ctx["trace_file"] = False
-    elif ctx["odoo_layer"] == "module" and ctx["rewrite_manifest"]:
+    elif (
+        ctx["product_doc"] == "odoo"
+        and ctx["odoo_layer"] == "module"
+        and ctx["rewrite_manifest"]
+    ):
         ctx["dst_file"] = ctx["manifest_filename"]
     elif ctx["odoo_layer"] == "module" and ctx["write_man_page"]:
         ctx["dst_file"] = "page.man"
+    elif os.path.isfile("../setup.py"):
+        ctx["dst_file"] = "../README.rst"
     else:
         ctx["dst_file"] = "./README.rst"
     if ctx["odoo_layer"] != "module":
         ctx["manifest"] = {"name": "repos_name", "development_status": "Alfa"}
     if ctx["product_doc"] == "odoo":
         ctx["development_status"] = (
             ctx["manifest"].get(
@@ -1820,14 +1841,71 @@
         ctx["local_path"] = "%s/%s/%s/" % (
             ctx["ODOO_ROOT"],
             ctx["branch"],
             ctx["repos_name"],
         )
 
 
+def setup_names(fn, email=None):
+    if email == "name":
+        with open(fn, RMODE) as fd:
+            return ", ".join([
+                x.split("*", 1)[1].split("<", 1)[0].strip()
+                if x.startswith("*") else x.split("<", 1)[0].strip()
+                for x in fd.read().split("\n") if x
+            ])
+    elif email == "email":
+        with open(fn, RMODE) as fd:
+            return ", ".join([
+                "<" + x.split("*", 1)[1].split("<", 1)[1].strip()
+                if x.startswith("*") else "<" + x.split("<", 1)[1].strip()
+                for x in fd.read().split("\n") if x
+            ])
+    else:
+        with open(fn, RMODE) as fd:
+            return ", ".join([
+                x.split("*", 1)[0].strip() if x.startswith("*") else x.strip()
+                for x in fd.read().split("\n") if x
+            ])
+
+
+def complete_setup(ctx, setup_fn):
+    with open(setup_fn, RMODE) as fd:
+        AUTH_RE = re.compile("^author *=")
+        EMAIL_RE = re.compile("^author_email *=")
+        SOURCE_ROOT = "https://github.com/zeroincombenze/tools"
+        URL_RE = re.compile(r"^ +url=[\"']")
+        SOURCE_URL_RE = re.compile("^source_url *=")
+        SOURCE_URL = SOURCE_ROOT + "/tree/master/%s"
+        DOC_URL_RE = re.compile("^doc_url *=")
+        DOC_URL = "https://zeroincombenze-tools.readthedocs.io/en/latest/%s"
+        CHANGELOG_RE = re.compile("^changelog_url *=")
+        CHANGELOG_URL = SOURCE_ROOT + "/blob/master/%s/egg-info/CHANGELOG.rst"
+        contents = ""
+        for line in fd.read().split("\n"):
+            if AUTH_RE.match(line):
+                line = "author = \"%s\"" % setup_names(
+                    "egg-info/CONTRIBUTORS.txt", email="name")
+            elif EMAIL_RE.match(line):
+                line = "author_email = \"%s\"" % setup_names(
+                    "egg-info/CONTRIBUTORS.txt",  email="email")
+            elif URL_RE.match(line):
+                line = line.split("=")[0] + ("=\"%s\"," % SOURCE_ROOT)
+            elif SOURCE_URL_RE.match(line):
+                line = "source_url = \"%s\"" % (SOURCE_URL % ctx["module_name"])
+            elif DOC_URL_RE.match(line):
+                line = "doc_url = \"%s\"" % (DOC_URL % ctx["module_name"])
+            elif CHANGELOG_RE.match(line):
+                line = "changelog_url = \"%s\"" % (CHANGELOG_URL % ctx["module_name"])
+            contents += line
+            contents += "\n"
+    with open(setup_fn, "w") as fd:
+        fd.write(contents)
+
+
 def read_purge_readme(ctx, source):
     if source is None:
         return "", "", ""
     lines = source.split("\n")
     out_sections = {"description": "", "authors": "", "contributors": ""}
     cur_sect = "description"
     ix = 0
@@ -1941,29 +2019,29 @@
                     header = "%s (%s)" % (
                         ctx["manifest"].get("version", ""),
                         ctx["today"],
                     )
                     dash = "~" * len(header)
                     line = "* [IMP] Created documentation directory"
                     ctx[section] = "%s\n%s\n\n%s\n" % (header, dash, line)
-                if path == "./readme" and section == "CONTRIBUTORS":
+                if path == "./readme" and section == "contributors":
                     fd.write(_c(ctx["authors"]))
                 fd.write(_c(ctx[section.lower()]))
 
     if os.path.isdir("./egg-info"):
         for section in (
             "authors",
             "contributors",
             "description",
             "descrizione",
             "history",
         ):
             write_file("./egg-info", section)
     elif os.path.isdir("./readme"):
-        for section in ("CONTRIBUTORS", "DESCRIPTION"):
+        for section in ("contributors", "description"):
             write_file("./readme", section)
 
 
 def generate_readme(ctx):
     def validate_authors_contributors(ctx):
         contributors = ""
         for line in ctx["contributors"].split("\n"):
@@ -2046,35 +2124,30 @@
         "rdme_description",
         "rdme_authors",
         "rdme_contributors",
     ):
         ctx[section] = ""
     # Read predefined section / tags
     if ctx["odoo_layer"] == "module":
-        for fn in ("./README.md", "./README.rst"):
+        for fn in ("./README.md", "./README.rst", "../README.rst"):
             if not os.path.isfile(fn):
                 continue
-            with open(fn, "rU") as fd:
+            with open(fn, RMODE) as fd:
                 (
                     ctx["rdme_description"],
                     ctx["rdme_authors"],
                     ctx["rdme_contributors"],
                 ) = read_purge_readme(ctx, _u(fd.read()))
             break
 
     ctx = read_manifest_setup(ctx)
     set_default_values(ctx)
     ctx["license_mgnt"] = license_mgnt.License()
     ctx["license_mgnt"].add_copyright(ctx["git_orgid"], "", "", "", "")
-    for section in DEFINED_TAG:
-        out_fmt = None
-        ctx[section] = parse_local_file(
-            ctx, "%s.txt" % section, ignore_ntf=True, out_fmt=out_fmt, section=section
-        )[1]
-    for section in DEFINED_SECTIONS:
+    for section in DEFINED_TAG + DEFINED_SECTIONS:
         out_fmt = None
         ctx[section] = parse_local_file(
             ctx, "%s.rst" % section, ignore_ntf=True, out_fmt=out_fmt, section=section
         )[1]
         if section in ZERO_PYPI_SECTS and ctx.get("submodules"):
             for sub in ctx.get("submodules").split(" "):
                 ctx[section] += "\n\n"
@@ -2113,14 +2186,16 @@
             ctx, parse_local_file(ctx, ctx["template_name"], out_fmt="html")[1]
         )
     else:
         if not ctx["template_name"]:
             ctx["template_name"] = "readme_main_%s.rst" % ctx["odoo_layer"]
         target = parse_local_file(ctx, ctx["template_name"], out_fmt="rst")[1]
     if ctx["rewrite_manifest"] and ctx["odoo_layer"] == "module":
+        if ctx["product_doc"] != "odoo":
+            return
         target = manifest_contents(ctx)
     tmpfile = "%s.tmp" % ctx["dst_file"]
     bakfile = "%s.bak" % ctx["dst_file"]
     dst_file = ctx["dst_file"]
     if ctx["opt_verbose"]:
         print("Writing %s" % dst_file)
     with open(tmpfile, "w") as fd:
@@ -2160,15 +2235,15 @@
         "Generate README", "© 2018-2023 by SHS-AV s.r.l.", version=__version__
     )
     parser.add_argument("-h")
     parser.add_argument(
         "-b", "--odoo-branch", action="store", default=".", dest="odoo_vid"
     )
     parser.add_argument(
-        "-B", "--debug-template", action="store_true", dest="dbg_template"
+        "-B", "--debug-template", action="store_true", dest="debug_template"
     )
     parser.add_argument("-F", "--from-version", dest="from_version")
     parser.add_argument("-G", "--git-org", action="store", dest="git_orgid")
     parser.add_argument("-g", "--gpl-info", action="store", dest="opt_gpl", default="")
     parser.add_argument(
         "-H", "--write-index_html", action="store_true", dest="write_html"
     )
```

### Comparing `wok_code-2.0.7/wok_code/scripts/lint_2_compare.py` & `wok_code-2.0.8/wok_code/scripts/lint_2_compare.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import os
 import sys
 import argparse
 from lxml import etree
+import re
 
 from python_plus import _b, _u
 from z0lib import z0lib
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 IGNORE_DIRS = (".idea", ".git", "egg-info", "setup")
+REGEX_CM = re.compile("(^ *#|^.* #)")
+REGEX_OE = re.compile(r"([\"'])https?://www.openerp.com([\"'])")
+REGEX_OO = re.compile(r"([\"'])https?://(www.)?odoo.com([\"'])")
 
 
 def get_names(left_path, right_path):
     left_base = right_base = ''
     while left_path and right_path and left_path != right_path:
         left_base = os.path.basename(left_path)
         right_base = os.path.basename(right_path)
@@ -55,14 +59,15 @@
 
 
 def cp_file(opt_args, left_diff_path, right_diff_path, left_path, right_path, base):
     if (
         base.endswith(".pyc")
         or ((base.endswith(".po") or base.endswith(".pot")) and opt_args.ignore_po)
         or (base.startswith("README") and opt_args.ignore_doc)
+        or (base.startswith("LICENSE") and opt_args.ignore_doc)
     ):
         return
     elif os.path.isfile(left_path):
         if base.endswith(".xml"):
             format_xml(opt_args, left_path, os.path.join(left_diff_path, base))
         else:
             z0lib.run_traced(
@@ -132,61 +137,90 @@
             matchdir_based(
                 opt_args, left_diff_path, right_diff_path, left_path, right_path, base
             )
     else:
         match(opt_args, left_diff_path, right_diff_path, left_path, right_path)
 
 
-def remove_comment(root, files):
+def remove_comment(opt_args, root, files, compare_path=None):
+    def remove_identical_files(left_dir, right_dir, fn):
+        left_path = os.path.join(left_dir, fn)
+        right_path = os.path.join(right_dir, fn)
+        sts, stdout, stderr = z0lib.run_traced(
+            'diff -r %s %s' % (left_path, right_path),
+            verbose=False,
+            dry_run=opt_args.dry_run)
+        if sts == 0:
+            os.unlink(left_path)
+            os.unlink(right_path)
     for fn in files:
         ffn = os.path.join(root, fn)
         if not ffn.endswith(".py"):
+            if opt_args.purge and compare_path:
+                remove_identical_files(root, compare_path, fn)
             continue
         source = ""
         with open(ffn, "r") as fd:
             for line in fd.read().split("\n"):
-                if not line.strip().startswith("#"):
-                    source += ("%s\n" % line)
+                line = REGEX_OE.sub(r"\1https://www.odoo.com\2", line)
+                line = REGEX_OO.sub(r"\1https://www.odoo.com\2", line)
+                x = REGEX_CM.match(line)
+                if x:
+                    source += ("%s\n" % (line[x.start():x.end()-1].rstrip() or "#"))
+                else:
+                    source += ("%s\n" % line.rstrip())
         with open(ffn, "w") as fd:
             fd.write(source)
+        if opt_args.purge and compare_path:
+            remove_identical_files(root, compare_path, fn)
 
 
 def lintdir(opt_args, left_path, right_path):
     z0lib.run_traced('black %s' % left_path,
                      verbose=opt_args.dry_run,
                      dry_run=opt_args.dry_run)
     z0lib.run_traced('black %s' % right_path,
                      verbose=opt_args.dry_run,
                      dry_run=opt_args.dry_run)
     if opt_args.ignore_doc:
         for root, _dirs, files in os.walk(left_path):
-            remove_comment(root, files)
+            remove_comment(opt_args, root, files)
         for root, _dirs, files in os.walk(right_path):
-            remove_comment(root, files)
+            compare_path = None
+            if root.startswith(right_path):
+                compare_path = left_path + root[len(right_path):]
+            remove_comment(opt_args, root, files, compare_path=compare_path)
 
 
 def main(cli_args=None):
     cli_args = cli_args or sys.argv[1:]
     parser = argparse.ArgumentParser(
-        description="Compare 2 paths after formatted them",
+        description="Compare 2 paths after formatted them in the same way",
         epilog="© 2021-2023 by SHS-AV s.r.l."
     )
     parser.add_argument('-b', '--odoo-version')
-    parser.add_argument('-c', '--cache', help="Use cached values")
-    parser.add_argument("-d", "--ignore-doc", action="store_true")
+    parser.add_argument('-c', '--cache', action="store_true", help="Use cached values")
+    parser.add_argument(
+        "-d", "--ignore-doc",
+        action="store_true",
+        help="Ignore README, docs and comment in files")
     parser.add_argument("-i", "--ignore-po", action="store_true")
-    parser.add_argument("-m", "--meld", action="store_true", help='use meld')
+    parser.add_argument("-m", "--meld", action="store_true", help='Use meld')
+    parser.add_argument(
+        "-P", "--purge",
+        action="store_true",
+        help='Purge identical files on temporary dirs')
     parser.add_argument("-n", "--dry-run", dest="dry_run", action="store_true")
     parser.add_argument('-v', '--verbose', action='count', default=0)
     parser.add_argument('-V', '--version', action="version", version=__version__)
     parser.add_argument('left_path')
     parser.add_argument('right_path', nargs='?')
     opt_args = parser.parse_args(cli_args)
     if not opt_args.right_path:
-        # When just 1 path is issued, current directory become teh left path
+        # When just 1 path is issued, current directory become the left path
         # that is the reference path
         opt_args.right_path = os.path.abspath(opt_args.left_path)
         opt_args.left_path = os.path.abspath(os.getcwd())
     else:
         opt_args.right_path = os.path.abspath(opt_args.right_path)
     opt_args.left_path = os.path.abspath(opt_args.left_path)
     if (
@@ -238,19 +272,22 @@
         z0lib.run_traced('chmod -R -w %s' % left_diff_path,
                          verbose=opt_args.dry_run,
                          dry_run=opt_args.dry_run)
         z0lib.run_traced('chmod -R -w %s' % right_diff_path,
                          verbose=opt_args.dry_run,
                          dry_run=opt_args.dry_run)
     if opt_args.meld:
-        z0lib.run_traced('meld.exe %s %s' % (left_diff_path, right_diff_path),
-                         verbose=True,
-                         dry_run=opt_args.dry_run)
+        sts, stdout, stderr = z0lib.run_traced(
+            'meld.exe %s %s' % (left_diff_path, right_diff_path),
+            verbose=True,
+            dry_run=opt_args.dry_run)
     else:
-        z0lib.run_traced('diff -r %s %s' % (left_diff_path, right_diff_path),
-                         verbose=True,
-                         dry_run=opt_args.dry_run)
-    return 0
+        sts, stdout, stderr = z0lib.run_traced(
+            'diff -r %s %s' % (left_diff_path, right_diff_path),
+            verbose=True,
+            dry_run=opt_args.dry_run)
+    print(stdout, stderr)
+    return sts
 
 
 if __name__ == "__main__":
     exit(main())
```

### Comparing `wok_code-2.0.7/wok_code/scripts/deploy_odoo.py` & `wok_code-2.0.8/wok_code/scripts/deploy_odoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     from wok_code.scripts.wget_odoo_repositories import main as get_list_from_url
 try:
     from clodoo.clodoo import build_odoo_param
 except ImportError:
     from clodoo import build_odoo_param
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 MANIFEST_FILES = ["__manifest__.py", "__odoo__.py", "__openerp__.py", "__terp__.py"]
 
 ODOO_VALID_VERSIONS = (
     "16.0",
     "15.0",
     "14.0",
```

### Comparing `wok_code-2.0.7/wok_code/scripts/please_z0bug.py` & `wok_code-2.0.8/wok_code/scripts/please_z0bug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 class PleaseZ0bug(object):
 
     def __init__(self, please):
         self.please = please
```

### Comparing `wok_code-2.0.7/wok_code/scripts/odoo_translation.py` & `wok_code-2.0.8/wok_code/scripts/odoo_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
 # from python_plus import unicodes
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 MODULE_SEP = "\ufffa"
 
 # (<en>, <it>, <module>, <result>, ovverride)
 TEST_DATA = [
     ("name", "nome", None, "nome"),
```

### Comparing `wok_code-2.0.7/wok_code/scripts/odoo_dependencies.py` & `wok_code-2.0.8/wok_code/scripts/odoo_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 except ImportError:
     from z0lib import z0lib
 try:
     from clodoo import clodoo
 except ImportError:
     import clodoo
 
-__version__ = '2.0.7'
+__version__ = '2.0.8'
 
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 MAX_DEEP = 20
 UNDEF_DEEP = MAX_DEEP + 5
 MISSED = 99
```

### Comparing `wok_code-2.0.7/wok_code/scripts/license_mgnt.py` & `wok_code-2.0.8/wok_code/scripts/license_mgnt.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/scripts/cvt_csv_2_rst.py` & `wok_code-2.0.8/wok_code/scripts/cvt_csv_2_rst.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from z0lib import z0lib
 except ImportError:
     import z0lib
 
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 msg_time = time.time()
 
 
 def msg_burst(text):
     global msg_time
     t = time.time() - msg_time
```

### Comparing `wok_code-2.0.7/wok_code/scripts/please.py` & `wok_code-2.0.8/wok_code/scripts/please.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 except ImportError:
     from .please_z0bug import PleaseZ0bug                                  # noqa: F401
 try:
     from please_apache import PleaseApache                                 # noqa: F401
 except ImportError:
     from .please_apache import PleaseApache                                # noqa: F401
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 KNOWN_ACTIONS = [
     "help",
     "chkconfig",
     "config",
     "docs",
     "duplicate",
```

### Comparing `wok_code-2.0.7/wok_code/scripts/do_odoo_site.py` & `wok_code-2.0.8/wok_code/scripts/do_odoo_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     SSLCertificateKeyFile
     Include /etc/letsencrypt/options-ssl-apache.conf
     SSLCertificateChainFile
 </VirtualHost>
 </IfModule>
 """
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 class CreateConfig(object):
 
     def __init__(self, domain, opt_args):
         self.opt_args = opt_args
         if "." in domain:
```

### Comparing `wok_code-2.0.7/wok_code/scripts/__init__.py` & `wok_code-2.0.8/wok_code/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/eval_gtin.py` & `wok_code-2.0.8/wok_code/eval_gtin.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/do_git_checkout_new_branch.py` & `wok_code-2.0.8/wok_code/do_git_checkout_new_branch.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import re
 import sys
 import os
 import argparse
 
 from z0lib import z0lib
 
-__version__ = "2.0.7"
+__version__ = "2.0.8"
 
 
 class RepoCheckout(object):
 
     def __init__(self, opt_args):
         self.opt_args = opt_args
         if opt_args.odoo_branch not in ("16.0", "15.0", "14.0", "13.0", "12.0", "11.0",
```

### Comparing `wok_code-2.0.7/wok_code/topep8` & `wok_code-2.0.8/wok_code/topep8`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 # [[ -f $TDIR/../../python_plus/list_requirements.py ]] && LISTREQ=$TDIR/../../python_plus/list_requirements.py || LISTREQ=list_requirements.py
 YAML_TMPL=~/dev/pypi/z0bug_odd/z0bug_odoo/sample_files/.travis.yml
 NO_APT_GET="(build-essential|curl|git|gradle|gzip|java|lessc|less-plugin-clean-css|nodejs|npm|openssl|python-setuptools|python-simplejson|PhantomJS|rvm|ruby|sass|scss|tesseract|wget|wkhtmltopdf|zip)"
 
 expand_macro() {
   local t p v lne lne1
```

### Comparing `wok_code-2.0.7/wok_code/install_python_3_from_source.sh` & `wok_code-2.0.8/wok_code/install_python_3_from_source.sh`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/cvt_script.man` & `wok_code-2.0.8/wok_code/cvt_script.man`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/to_oca.2p8` & `wok_code-2.0.8/wok_code/to_oca.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/do_set_utf8.py` & `wok_code-2.0.8/wok_code/do_set_utf8.py`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/please.man` & `wok_code-2.0.8/wok_code/please.man`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,15 @@
 Remote hosts are in \fBtgtNpath\fR parameter of \fBplease config\fR action (where N is a number 1-9).
 .RE
 .P
 \fBreplace\fR
 .RS
 Copy all files of current PYPI project into tools directory.
 .br
-Current project must be one of included projects of tools repository. The project names to manage are in \fBPKGS_LIST\fR parameter of \fBplease config\fR action.
+Current project must be one of included projects of tools repository. The project names to manage are in \fBLOCAL_PKGS\fR parameter of \fBplease config\fR action.
 .RE
 .P
 \fBreplica DIRECTORY\fR
 .RS
 Copy the selected directory into all other versions of current Odoo module.
 .br
 Use this action mainly for replicate documentation directory.
```

### Comparing `wok_code-2.0.7/wok_code/to_zero.2p8` & `wok_code-2.0.8/wok_code/to_zero.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/to_pep8.2p8` & `wok_code-2.0.8/wok_code/to_pep8.2p8`

 * *Files identical despite different names*

### Comparing `wok_code-2.0.7/wok_code/cvt_script` & `wok_code-2.0.8/wok_code/cvt_script`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.7
+__version__=2.0.8
 
 #//Only human upgradable code/
 # blk1 => z0librc
 # blk2 => odoorc
 # blk3 => travisrc
 # blk4 => zarrc
 # blk8 => TESTDIR= ...
```

### Comparing `wok_code-2.0.7/setup.py` & `wok_code-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     install_requires.append('translators')
     install_requires.append('twine')
 else:
     install_requires.append('twine==1.15.0')
 
 setup(
     name='wok_code',
-    version='2.0.7',
+    version='2.0.8',
     description='Python developers tools',
     long_description="""
 Various tools at your fingertips.
 
 The available tools are:
 
 * cvt_csv_2_rst.py: convert csv file into rst file
@@ -87,12 +87,12 @@
             'lint_2_compare = wok_code.scripts.lint_2_compare:main',
             'makepo_it.py = wok_code.scripts.makepo_it:main',
             'odoo_dependencies.py = wok_code.scripts.odoo_dependencies:main',
             'odoo_translation.py = wok_code.scripts.odoo_translation:main',
             'please = wok_code.scripts.please:main',
             'to_pep8.py = wok_code.scripts.to_pep8:main',
             'wget_odoo_repositories.py = wok_code.scripts.wget_odoo_repositories:main',
-            'run_odoo_debug = odoo_score.scripts.run_odoo_debug:main',
+            'run_odoo_debug = wok_code.scripts.run_odoo_debug:main',
         ]
     },
     zip_safe=False,
 )
```

### Comparing `wok_code-2.0.7/PKG-INFO` & `wok_code-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wok_code
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python developers tools
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `wok_code-2.0.7/README.rst` & `wok_code-2.0.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
-==============
-wok_code 2.0.7
-==============
+======
+ 2.0.8
+======
 
 
 
-|Maturity| |Build Status| |Coverage Status| |license gpl|
+|Maturity| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -787,68 +787,59 @@
 |
 |
 
 Getting started
 ===============
 
 
-|
-
-Installation
-------------
-
 Installation
 ------------
 
 Zeroincombenze tools require:
 
-* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20
-* python 2.7, some tools require python 3.6+
+* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+* python 2.7+, some tools require python 3.6+
 * bash 5.0+
 
 Current version via Git
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     git clone https://github.com/zeroincombenze/tools.git
     cd ./tools
     ./install_tools.sh -p
-    source /opt/odoo/devel/activate_tools
-
+    source $HOME/devel/activate_tools
 
-Upgrade
--------
 
 Upgrade
 -------
 
-Current stable version
-~~~~~~~~~~~~~~~~~~~~~~
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
     ./install_tools.sh -U
-    source /opt/odoo/devel/activate_tools
-
-Current development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-::
-
-    cd $HOME
-    ./install_tools.sh -Ud
-    source /opt/odoo/devel/activate_tools
+    source $HOME/devel/activate_tools
 
 
 History
 -------
 
+2.0.8 (2023-05-09)
+~~~~~~~~~~~~~~~~~~
+
+* [FIX] Install run_odoo_debug
+* [FIX] Install do_git_ignore
+* [IMP] lint_2_compare: ignore odoo/openerp test string and LICENSE files
+* [IMP] lint_2_compare: new switch ---purge do not load identical files (quick diff)
+
 2.0.7 (2023-05-08)
 ~~~~~~~~~~~~~~~~~~
 
 * [IMP] deply_odoo: new action git-push
 * [REF] odoo_translation: new implementation
 * [FIX] run_odoo_debug: minor fixes
 * [NEW] do_git_checkout_new_branch: new command
@@ -920,22 +911,14 @@
 ~~~~~~~~~~~~~~~~~~~~
 
 * [FIX] deploy_odoo: show actual branch and organization
 * [FIX] deploy_odoo: update read from directory
 * [IMP] deploy_odoo: new command list repo info
 * [IMP] deploy_odoo: new feature link to repositories
 
-2.0.0.2 (2022-09-10)
-~~~~~~~~~~~~~~~~~~~~
-
-* [FIX] deploy_odoo: add path in addons_path of directory exists
-* [FIX] deploy_odoo: clone oca repositories with --single-branch option
-* [IMP] manage_pypi: improvements
-* [FIX] please lint|test
-
 
 
 |
 |
 
 Credits
 =======
@@ -946,58 +929,40 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
-Contributors
-------------
-
 
 
 |
 
-This module is part of tools project.
+This module is part of  project.
 
-Last Update / Ultimo aggiornamento: 2023-05-09
+Last Update / Ultimo aggiornamento: 
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
-.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
-    :target: https://travis-ci.com/zeroincombenze/tools
-    :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
-.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
-    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
-    :alt: Coverage
-.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
-    :alt: Codecov
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
     :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
     :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
-.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
-    :target: https://codecov.io/gh/OCA/tools/branch/2.0
-    :alt: Codecov
-.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
-   :target: https://odoo-italia.org
-   :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
 .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
 .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
```

