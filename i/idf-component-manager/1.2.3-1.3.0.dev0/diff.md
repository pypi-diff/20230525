# Comparing `tmp/idf_component_manager-1.2.3.tar.gz` & `tmp/idf_component_manager-1.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_component_manager-1.2.3.tar", last modified: Thu May 25 14:55:35 2023, max compression
+gzip compressed data, was "idf_component_manager-1.3.0.dev0.tar", last modified: Fri Mar 17 13:04:13 2023, max compression
```

## Comparing `idf_component_manager-1.2.3.tar` & `idf_component_manager-1.3.0.dev0.tar`

### file list

```diff
@@ -1,93 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8565 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4448 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     9939 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     6568 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/cmake_component_requirements.py
--rw-rw-rw-   0 root         (0) root         (0)    23288 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_manager/core.py
--rw-rw-rw-   0 root         (0) root         (0)     6209 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/dependencies.py
--rwxrwxrwx   0 root         (0) root         (0)     7130 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/idf_extensions.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/local_component_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager/prepare_components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/prepare_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/prepare_components/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4014 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/prepare_components/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     3362 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/service_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager/templates/
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/templates/idf_component_template.yml
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager/version_solver/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6279 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/assignment.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/constraint.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/failure.py
--rw-rw-rw-   0 root         (0) root         (0)    14629 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/incompatibility.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/incompatibility_cause.py
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/package.py
--rw-rw-rw-   0 root         (0) root         (0)     4188 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/package_source.py
--rw-rw-rw-   0 root         (0) root         (0)     7477 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/partial_solution.py
--rw-rw-rw-   0 root         (0) root         (0)    12692 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/range.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/result.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/set_relation.py
--rw-rw-rw-   0 root         (0) root         (0)     6444 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/term.py
--rw-rw-rw-   0 root         (0) root         (0)     6996 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/union.py
--rw-rw-rw-   0 root         (0) root         (0)    15350 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/version_solver.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_manager/version_solver/version_solver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8565 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3356 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-25 14:55:35.000000 idf_component_manager-1.2.3/idf_component_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      167 2023-05-25 14:42:49.000000 idf_component_manager-1.2.3/idf_component_tools/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    15506 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/api_client.py
--rw-rw-rw-   0 root         (0) root         (0)      585 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/api_client_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/api_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     2965 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/archive_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2017 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/build_system_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     4600 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/file_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/file_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     7932 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/git_client.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/hash_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.676093 idf_component_manager-1.2.3/idf_component_tools/lock/
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/lock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3673 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/lock/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/idf_component_tools/manifest/
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/env_expander.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/if_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4908 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/manager.py
--rw-rw-rw-   0 root         (0) root         (0)    10889 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     2217 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/solved_component.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/solved_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)    11035 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/manifest/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/idf_component_tools/semver/
--rw-rw-rw-   0 root         (0) root         (0)      452 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    32541 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/semver/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2753 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/serialization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/idf_component_tools/sources/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6347 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/sources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/sources/fetcher.py
--rw-rw-rw-   0 root         (0) root         (0)     7127 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/sources/git.py
--rw-rw-rw-   0 root         (0) root         (0)     1206 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/sources/idf.py
--rw-rw-rw-   0 root         (0) root         (0)     4516 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/sources/local.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-05-25 10:00:58.000000 idf_component_manager-1.2.3/idf_component_tools/sources/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9264 2023-05-25 14:03:07.000000 idf_component_manager-1.2.3/idf_component_tools/sources/web_service.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 14:55:35.680093 idf_component_manager-1.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3129 2023-05-25 12:08:05.000000 idf_component_manager-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-03-17 11:19:02.000000 idf_component_manager-1.3.0.dev0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4448 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5993 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/component.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-03-09 10:32:22.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/project.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cli/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6568 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/cmake_component_requirements.py
+-rw-rw-rw-   0 root         (0) root         (0)    23423 2023-03-16 12:16:26.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     6209 2023-01-17 19:22:12.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9022 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/dependencies.py
+-rwxrwxrwx   0 root         (0) root         (0)     7671 2023-03-16 12:16:26.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/idf_extensions.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/local_component_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4014 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     3390 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/service_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/templates/idf_component_template.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/assignment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/constraint.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/failure.py
+-rw-rw-rw-   0 root         (0) root         (0)    14629 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py
+-rw-rw-rw-   0 root         (0) root         (0)     1428 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12692 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/range.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/result.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/set_relation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6444 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/term.py
+-rw-rw-rw-   0 root         (0) root         (0)     6996 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/union.py
+-rw-rw-rw-   0 root         (0) root         (0)    15350 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6130 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/version_solver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.564516 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11845 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3716 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-03-17 13:04:13.000000 idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-03-17 10:17:13.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15599 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      585 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_client_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/api_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/archive_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/build_system_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     4633 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-01-18 12:34:38.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     6240 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/file_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/file_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     8366 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/git_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3422 2023-01-18 11:58:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/hash_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4050 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/lock/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/
+-rw-rw-rw-   0 root         (0) root         (0)      872 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/env_expander.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/if_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11187 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13069 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      452 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33154 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/semver/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2753 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/serialization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6349 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2486 2023-01-18 11:58:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/fetcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     7127 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/git.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/idf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4528 2023-02-27 13:02:30.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/local.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-01-10 11:43:54.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9291 2023-03-16 19:00:46.000000 idf_component_manager-1.3.0.dev0/idf_component_tools/sources/web_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2023-03-17 11:19:02.000000 idf_component_manager-1.3.0.dev0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-17 13:04:13.568516 idf_component_manager-1.3.0.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3162 2023-01-17 21:31:48.000000 idf_component_manager-1.3.0.dev0/setup.py
```

### Comparing `idf_component_manager-1.2.3/LICENSE` & `idf_component_manager-1.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/README.md` & `idf_component_manager-1.3.0.dev0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -142,19 +142,61 @@
 
 ```yaml
 examples:
   - path: ../some/path
   - path: ../some/other_path
 ```
 
+## Environment variables
+
+| Variable                                    | Default value (or example for required) | Required? | Description                                                                                     |
+| ------------------------------------------- | --------------------------------------- | --------- | ----------------------------------------------------------------------------------------------- |
+| IDF_COMPONENT_API_TOKEN                     |                                         | no        | API token to access the component registry                                                      |
+| IDF_COMPONENT_REGISTRY_URL                  | https://components.espressif.com/       | no        | URL of the default component registry                                                           |
+| IDF_COMPONENT_STORAGE_URL                   | https://components-file.espressif.com/  | no        | URL of the default file storage server                                                          |
+| IDF_COMPONENT_REGISTRY_PROFILE              | default                                 | no        | Profile in the config file to use for component registry                                        |
+| IDF_COMPONENT_API_CACHE_EXPIRATION_MINUTES  | 5                                       | no        | API Cache expiration time in minutes                                                            |
+| IDF_COMPONENT_CACHE_PATH                    | \* Depends on OS                        | no        | Cache directory for component manager                                                           |
+| COMPONENT_MANAGER_JOB_TIMEOUT               | 300                                     | no        | Timeout in seconds to wait for component processing                                             |
+| IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS  | 0                                       | no        | Overwrite files in the managed_component directory, even if they have been modified by the user |
+| IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS | 0                                       | no        | Ignore unknown files in managed_components directory                                            |
+
 ## Contributions Guide
 
 We welcome all contributions to the Component Manager project.
 
 You can contribute by fixing bugs, adding features, adding documentation, or reporting an [issue](https://github.com/espressif/idf-component-manager/issues). We accept contributions via [Github Pull Requests](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).
 
 Before reporting an issue, make sure you've searched for a similar one that was already created. If you are reporting a new issue, please follow the Issue Template.
 
+## Installing a development version of the component manager
+
+You can install the development version of the component manager from the main branch of this repository:
+
+**On Linux/macOS:**
+
+Go to the directory with your ESP-IDF installation and run:
+
+```bash
+# activate ESP-IDF environment
+source ./export.sh # or . ./export.fish, if you use fish shell
+# remove old version of the component manager
+python -m pip uninstall -y idf-component-manager
+# install the development version (from the main branch)
+python -m pip install git+https://github.com/espressif/idf-component-manager.git@main
+```
+
+**On Windows:**
+
+Run `ESP-IDF PowerShell Environment` or `ESP-IDF Command Prompt (cmd.exe)` from the Start menu and run the following command:
+
+```powershell
+# remove old version of the component manager
+python -m pip uninstall -y idf-component-manager
+# install the development version (from the main branch)
+python -m pip install git+https://github.com/espressif/idf-component-manager.git@main
+```
+
 ## Resources
 
 - The Python Package Index project page https://pypi.org/project/idf-component-manager/
 - The Component Manager section in the [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-guides/tools/idf-component-manager.html)
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/__main__.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/cmake_component_requirements.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/cmake_component_requirements.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/core.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from idf_component_tools.api_client_errors import APIClientError, NetworkConnectionError, VersionNotFound
 from idf_component_tools.archive_tools import pack_archive, unpack_archive
 from idf_component_tools.build_system_tools import build_name
 from idf_component_tools.errors import FatalError, GitError, ManifestError, NothingToDoError
 from idf_component_tools.file_tools import check_unexpected_component_files, copy_filtered_directory, create_directory
 from idf_component_tools.git_client import GitClient
 from idf_component_tools.hash_tools import (
-    HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error, validate_dir_with_hash_file)
+    HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error, validate_managed_component_hash)
 from idf_component_tools.manifest import (
     MANIFEST_FILENAME, WEB_DEPENDENCY_REGEX, Manifest, ManifestManager, ProjectRequirements)
 from idf_component_tools.semver import SimpleSpec, Version
 from idf_component_tools.sources import WebServiceSource
 
 from .cmake_component_requirements import CMakeRequirementsManager, ComponentName, handle_project_requirements
 from .core_utils import (
@@ -291,15 +291,15 @@
         undeleted_components = []
         for component_dir in managed_components_dir.glob('*/'):
 
             if not (managed_components_dir / component_dir).is_dir():
                 continue
 
             try:
-                validate_dir_with_hash_file(str(managed_components_dir / component_dir))
+                validate_managed_component_hash(str(managed_components_dir / component_dir))
                 shutil.rmtree(str(managed_components_dir / component_dir))
             except (HashNotEqualError, HashNotSHA256Error):
                 undeleted_components.append(component_dir.name)
             except HashDoesNotExistError:
                 pass
 
         if undeleted_components:
@@ -520,7 +520,11 @@
             for requirement in requirements.keys():
                 name = requirement.name
                 if name not in main_reqs and name != 'main' and isinstance(main_reqs, list):
                     main_reqs.append(name)
 
         handle_project_requirements(requirements)
         requirements_manager.dump(requirements)
+
+    def update_dependencies(self, **kwargs):
+        if os.path.isfile(self.lock_path):
+            os.remove(self.lock_path)
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/core_utils.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/core_utils.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/dependencies.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import shutil
 
+from idf_component_manager.core_utils import raise_component_modified_error
 from idf_component_manager.utils import print_info
+from idf_component_manager.version_solver.helper import parse_root_dep_conflict_constraints
+from idf_component_manager.version_solver.mixology.failure import SolverFailure
+from idf_component_manager.version_solver.mixology.package import Package
+from idf_component_manager.version_solver.version_solver import VersionSolver
 from idf_component_tools.build_system_tools import build_name
-from idf_component_tools.errors import ComponentModifiedError, FetchingError, SolverError, hint, warn
-from idf_component_tools.hash_tools import ValidatingHashError, validate_dir_with_hash_file
+from idf_component_tools.environment import getenv_bool
+from idf_component_tools.errors import (
+    ComponentModifiedError, FetchingError, InvalidComponentHashError, SolverError, hint, warn)
+from idf_component_tools.hash_tools import ValidatingHashError, validate_managed_component_hash
 from idf_component_tools.lock import LockManager
-from idf_component_tools.manifest import ProjectRequirements, SolvedComponent, SolvedManifest
+from idf_component_tools.manifest import HashedComponentVersion, ProjectRequirements, SolvedComponent, SolvedManifest
 from idf_component_tools.sources.fetcher import ComponentFetcher
 
-from .core_utils import raise_component_modified_error
-from .version_solver.helper import parse_root_dep_conflict_constraints
-from .version_solver.mixology.failure import SolverFailure
-from .version_solver.mixology.package import Package
-from .version_solver.version_solver import VersionSolver
-
 
 def check_manifests_targets(project_requirements):  # type: (ProjectRequirements) -> None
     for manifest in project_requirements.manifests:
         if not manifest.targets:
             continue
 
         if project_requirements.target not in manifest.targets:
@@ -30,15 +31,15 @@
 
 
 def get_unused_components(unused_files_with_components, managed_components_path):  # type: (set[str], str) -> set[str]
     unused_components = set()
 
     for component in unused_files_with_components:
         try:
-            validate_dir_with_hash_file(os.path.join(managed_components_path, component))
+            validate_managed_component_hash(os.path.join(managed_components_path, component))
             unused_components.add(component)
         except ValidatingHashError:
             pass
 
     return unused_components
 
 
@@ -52,15 +53,15 @@
     unused_components = get_unused_components(unused_files_with_components, managed_components_path)
     unused_files = unused_files_with_components - unused_components
     if unused_components:
         print_info('Deleting {} unused components'.format(len(unused_components)))
         for unused_component_name in unused_components:
             print_info(' {}'.format(unused_component_name))
             shutil.rmtree(os.path.join(managed_components_path, unused_component_name))
-    if unused_files and os.getenv('IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS') != '1':
+    if unused_files and not getenv_bool('IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS'):
         warning = '{} unexpected files and directories were found in the "managed_components" directory:'.format(
             len(unused_files))
 
         for unexpected_name in unused_files:
             warning += ' {}'.format(unexpected_name)
 
         warning += (
@@ -69,28 +70,50 @@
             'IGNORE_UNKNOWN_FILES_FOR_MANAGED_COMPONENTS=1')
         warn(warning)
 
 
 def is_solve_required(project_requirements, solution):
     # type: (ProjectRequirements, SolvedManifest) -> bool
 
-    if project_requirements.manifest_hash != solution.manifest_hash\
-            or (solution.target and project_requirements.target != solution.target):
+    if not solution.manifest_hash:
+        print_info('Dependencies lock doesn\'t exist, solving dependencies.')
+        return True
+
+    if project_requirements.manifest_hash != solution.manifest_hash:
+        print_info('Manifest hash changed, solving dependencies.')
+        return True
+
+    if solution.target and project_requirements.target != solution.target:
+        print_info(
+            'Target changed from {} to {}, solving dependencies.'.format(solution.target, project_requirements.target))
         return True
 
     for component in solution.dependencies:
+        # Handle meta components, like ESP-IDF
         if not component.source.meta:
             continue
 
         try:
-            component_version = component.source.versions(component.name).versions[0]
+            component_version = component.source.versions(component.name).versions[0]  # type: HashedComponentVersion
 
             if component_version != component.version:
+                print_info(
+                    'Dependency "{}" version changed from {} to {}, solving dependencies.'.format(
+                        component, component.version, component_version))
                 return True
+
+            if component_version.component_hash != component.component_hash:
+                raise InvalidComponentHashError(
+                    'The hash sum of the component "{}" does not match the one recorded in your dependencies.lock '
+                    'file. This could be due to a potential spoofing of the download server, or your lock file may '
+                    'have become corrupted. Please review the lock file and verify the download server\'s '
+                    'authenticity to ensure the component\'s security and integrity.'.format(component))
+
         except IndexError:
+            print_info('Dependency "{}" version changed, solving dependencies.'.format(component))
             return True
 
     return False
 
 
 def print_dot():
     print_info('.', nl=False)
@@ -100,15 +123,14 @@
     # type: (ProjectRequirements, str, str) -> tuple[set[str], dict[str, str]]
     '''Solves dependencies and download components'''
     lock_manager = LockManager(lock_path)
     solution = lock_manager.load()
     check_manifests_targets(project_requirements)
 
     if is_solve_required(project_requirements, solution):
-        print_info('Solving dependencies requirements')
         solver = VersionSolver(project_requirements, solution, component_solved_callback=print_dot)
 
         try:
             solution = solver.solve()
         except SolverFailure as e:
             conflict_constraints = parse_root_dep_conflict_constraints(e)
             components_introduce_conflict = []
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/idf_extensions.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/idf_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import sys
 import warnings
 
 from idf_component_manager.utils import CLICK_SUPPORTS_SHOW_DEFAULT, print_error, showwarning
 from idf_component_tools.errors import FatalError
@@ -87,14 +87,20 @@
             sys.exit(e.exit_code)
 
     def global_callback(ctx, global_args, tasks):
         copy_tasks = list(tasks)
         for index, task in enumerate(copy_tasks):
             if task.name == 'fullclean':
                 tasks.insert(index + 1, ctx.invoke(ctx.command.get_command(ctx, 'remove_managed_components')))
+            elif task.name == 'update-dependencies':
+                reconfigure = ctx.invoke(ctx.command.get_command(ctx, 'reconfigure'))
+                # reсonfigure does not take any parameters.
+                # More information in the idf.py implementation (idf.py/execute_tasks)
+                reconfigure.action_args = {}
+                tasks.insert(index + 1, reconfigure)
 
     return {
         'global_action_callbacks': [global_callback],
         'actions': {
             'create-manifest': {
                 'callback': callback,
                 'help': 'Create manifest for specified component.',
@@ -192,9 +198,13 @@
                         'help': (
                             'Set the path for the new project. The project '
                             'will be created directly in the given folder if it does not contain anything'),
                         'required': False,
                     }
                 ],
             },
+            'update-dependencies': {
+                'callback': callback,
+                'help': 'Update dependencies of the project',
+            }
         },
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/local_component_list.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/local_component_list.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/prepare_components/prepare.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/prepare_components/prepare.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/service_details.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/service_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 from collections import namedtuple
 
 from idf_component_manager.utils import print_info
 from idf_component_tools.api_client import APIClient
 from idf_component_tools.config import ConfigManager, component_registry_url
 from idf_component_tools.constants import DEFAULT_NAMESPACE
-from idf_component_tools.errors import FatalError
+from idf_component_tools.errors import FatalError, UserDeprecationWarning
 
 ServiceDetails = namedtuple('ServiceDetails', ['client', 'namespace'])
 
 
 class NamespaceError(FatalError):
     pass
 
@@ -47,15 +47,15 @@
 
     profile_name_env_deprecated = os.getenv('IDF_COMPONENT_SERVICE_PROFILE')
 
     if profile_name_env_deprecated:
         warnings.warn(
             'IDF_COMPONENT_SERVICE_PROFILE environment variable is deprecated. '
             'Please use IDF_COMPONENT_REGISTRY_PROFILE instead',
-            category=DeprecationWarning)
+            category=UserDeprecationWarning)
 
     profile_name_env = os.getenv('IDF_COMPONENT_REGISTRY_PROFILE')
 
     if profile_name_env and profile_name_env_deprecated:
         warnings.warn(
             'Both IDF_COMPONENT_SERVICE_PROFILE and IDF_COMPONENT_REGISTRY_PROFILE '
             'environment variables are defined. The value of IDF_COMPONENT_REGISTRY_PROFILE is used.')
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/templates/idf_component_template.yml` & `idf_component_manager-1.3.0.dev0/idf_component_manager/templates/idf_component_template.yml`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/utils.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
+import re
 
 import click
 from packaging import version
 
 from idf_component_tools.errors import UserHint
 
 try:
@@ -44,7 +45,10 @@
         bg=None,  # type: str | None
         bold=None,  # type: str | None
         underline=None,  # type: str | None
         blink=None,  # type: str | None
         **kwargs  # type: 'Any'
 ):  # type: (...) -> None
     click.secho(message, fg=fg, bg=bg, bold=bold, underline=underline, blink=blink, **kwargs)
+
+
+RE_PATTERN = type(re.compile(''))  # this is a workaround for `re.Pattern` for python<3.7
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/helper.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/helper.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/assignment.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/assignment.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/constraint.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/constraint.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/failure.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/failure.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/incompatibility.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/incompatibility_cause.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/incompatibility_cause.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/package.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/package_source.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/package_source.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/partial_solution.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/partial_solution.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/range.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/range.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/result.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/result.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/term.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/term.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/union.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/union.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/mixology/version_solver.py` & `idf_component_manager-1.3.0.dev0/idf_component_manager/version_solver/mixology/version_solver.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_manager/version_solver/version_solver.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/local.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,120 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-from idf_component_tools.errors import DependencySolveError, SolverError
-from idf_component_tools.manifest import (
-    ComponentRequirement, Manifest, ProjectRequirements, SolvedComponent, SolvedManifest)
-
-from .helper import PackageSource
-from .mixology.package import Package
-from .mixology.version_solver import VersionSolver as Solver
+import os
+from pathlib import Path
+
+from ..errors import SourceError, warn
+from ..manifest import MANIFEST_FILENAME, ComponentWithVersions, HashedComponentVersion, ManifestManager
+from .base import BaseSource
 
 try:
-    from typing import Callable, Optional
+    from typing import Dict
 except ImportError:
     pass
 
 
-class VersionSolver(object):
-    """
-    The version solver that finds a set of package versions
-    satisfies the root package's dependencies.
-    """
-    def __init__(self, requirements, old_solution=None, component_solved_callback=None):
-        # type: (ProjectRequirements, Optional[SolvedManifest], Optional[Callable[[], None]]) -> None
-        self.requirements = requirements
-        self.old_solution = old_solution
-        self.component_solved_callback = component_solved_callback
-
-        self._source = PackageSource()
-        self._solver = Solver(self._source)
-        self._target = None
-        self._overriders = set()  # type: set[str]
-
-    def solve(self):  # type: () -> SolvedManifest
-        for manifest in self.requirements.manifests:
-            self.solve_manifest(manifest)
-
-        self._source.override_dependencies(self._overriders)
-
-        result = self._solver.solve()
-
-        solved_components = []
-        for package, version in result.decisions.items():
-            if package == Package.root():
-                continue
-            kwargs = {'name': package.name, 'source': package.source, 'version': version}
-            if package.source.component_hash_required:
-                kwargs['component_hash'] = version.component_hash
-            solved_components.append(SolvedComponent(**kwargs))  # type: ignore
-        return SolvedManifest(solved_components, self.requirements.manifest_hash, self.requirements.target)
-
-    def solve_manifest(self, manifest):  # type: (Manifest) -> None
-        for requirement in manifest.dependencies:  # type: ComponentRequirement
-            self._source.root_dep(Package(requirement.name, requirement.source), requirement.version_spec)
-            try:
-                self.solve_component(requirement)
-            except DependencySolveError as e:
-                raise SolverError(
-                    'Solver failed processing dependency "{dependency}" '
-                    'from the manifest file "{path}".\n{original_error}'.format(
-                        path=manifest.path, dependency=e.dependency, original_error=str(e)))
-            except SolverError as e:
-                raise SolverError(
-                    'Solver failed processing manifest file "{path}".'
-                    '\n{original_error}'.format(path=manifest.path, original_error=str(e)))
+class ManifestContextError(SourceError):
+    pass
 
-    def solve_component(self, requirement):  # type: (ComponentRequirement) -> None
-        try:
-            cmp_with_versions = requirement.source.versions(
-                name=requirement.name, spec=requirement.version_spec, target=self.requirements.target)
-        except Exception as e:
-            raise DependencySolveError(str(e), dependency=requirement.name)
-
-        for version in cmp_with_versions.versions:
-            if requirement.source.is_overrider:
-                self._overriders.add(requirement.name)
-
-            self._source.add(
-                Package(requirement.name, requirement.source),
-                version,
-                deps={Package(req.name, req.source): req.version_spec
-                      for req in version.dependencies} if version.dependencies else {})
-
-            if version.dependencies:
-                for dep in version.dependencies:
-                    self.solve_component(dep)
 
-        if self.component_solved_callback:
-            self.component_solved_callback()
+class SourcePathError(SourceError):
+    pass
+
+
+class LocalSource(BaseSource):
+    NAME = 'local'
+
+    def __init__(self, source_details, **kwargs):
+        super(LocalSource, self).__init__(source_details=source_details, **kwargs)
+
+        self.is_overrider = 'override_path' in source_details
+        self._raw_path = Path(source_details.get('override_path' if self.is_overrider else 'path'))
+
+    @property
+    def _path(self):  # type: () -> Path
+        try:
+            if self._manifest_manager:
+                path = (Path(self._manifest_manager.path).parent / self._raw_path).resolve()
+            elif not self._manifest_manager and self._raw_path.is_absolute():
+                path = self._raw_path.resolve()
+            else:
+                raise ManifestContextError(
+                    "Can't reliably evaluate relative path without context: {}".format(str(self._raw_path)))
+
+            if not path.is_dir():  # for Python > 3.6, where .resolve(strict=False)
+                raise OSError()
+
+        except OSError:
+            raise SourcePathError('Invalid source path, should be a directory: %s' % str(self._raw_path))
+
+        if self.is_overrider and path / 'CMakeLists.txt' not in path.iterdir():
+            raise SourcePathError(
+                'The override_path you\'re using is pointing to directory "%s" that is not a component.' % str(path))
+
+        return path
+
+    @classmethod
+    def required_keys(cls):
+        return {'path': 'str'}
+
+    @classmethod
+    def optional_keys(cls):
+        return {'override_path': 'str'}
+
+    @staticmethod
+    def is_me(name, details):
+        return bool(details.get('path', None)) or 'override_path' in details
+
+    @property
+    def hash_key(self):
+        return self.source_details.get('path')
+
+    def download(self, component, download_path):
+        directory_name = os.path.basename(str(self._path))
+        component_with_namespace = component.name.replace('/', '__')
+        namespace_and_component = component.name.split('/')
+        component_without_namespace = namespace_and_component[-1]
+        if component_without_namespace != directory_name and component_with_namespace != directory_name:
+            alternative_name = ' or "{}"'.format(component_with_namespace) if len(namespace_and_component) == 2 else ''
+            warn(
+                'Component name "{component_name}" doesn\'t match the directory name "{directory_name}".\n'.format(
+                    component_name=component.name,
+                    directory_name=directory_name,
+                ) +
+                'ESP-IDF CMake build system uses directory names as names of components, so different names may break '
+                + 'requirements resolution. To avoid the problem rename the component directory to ' +
+                '"{component_without_namespace}"{alternative_name}'.format(
+                    component_without_namespace=component_without_namespace, alternative_name=alternative_name))
+        return str(self._path)
+
+    def versions(self, name, details=None, spec='*', target=None):
+        """For local return version from manifest, or * if manifest not found"""
+        manifest_path = self._path / MANIFEST_FILENAME
+        name = self._path.name
+
+        version_str = '*'
+        targets = []
+        dependencies = []
+
+        if manifest_path.is_file():
+            manifest = ManifestManager(str(manifest_path), name=name).load()
+            if manifest.version:
+                version_str = str(manifest.version)
+
+            if manifest.targets:  # only check when exists
+                if target and target not in manifest.targets:
+                    return ComponentWithVersions(name=name, versions=[])
+
+                targets = manifest.targets
+
+            dependencies = manifest.dependencies
+
+        return ComponentWithVersions(
+            name=name, versions=[HashedComponentVersion(version_str, targets=targets, dependencies=dependencies)])
+
+    def serialize(self):  # type: () -> Dict
+        return {
+            'path': str(self._path),
+            'type': self.name,
+        }
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager.egg-info/SOURCES.txt` & `idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 idf_component_manager/__init__.py
 idf_component_manager/__main__.py
-idf_component_manager/cli.py
 idf_component_manager/cmake_component_requirements.py
 idf_component_manager/core.py
 idf_component_manager/core_utils.py
 idf_component_manager/dependencies.py
 idf_component_manager/idf_extensions.py
 idf_component_manager/local_component_list.py
 idf_component_manager/service_details.py
 idf_component_manager/utils.py
 idf_component_manager.egg-info/PKG-INFO
 idf_component_manager.egg-info/SOURCES.txt
 idf_component_manager.egg-info/dependency_links.txt
 idf_component_manager.egg-info/entry_points.txt
 idf_component_manager.egg-info/requires.txt
 idf_component_manager.egg-info/top_level.txt
+idf_component_manager/cli/__init__.py
+idf_component_manager/cli/autocompletion.py
+idf_component_manager/cli/cache.py
+idf_component_manager/cli/component.py
+idf_component_manager/cli/constants.py
+idf_component_manager/cli/core.py
+idf_component_manager/cli/manifest.py
+idf_component_manager/cli/project.py
+idf_component_manager/cli/utils.py
 idf_component_manager/prepare_components/__init__.py
 idf_component_manager/prepare_components/__main__.py
 idf_component_manager/prepare_components/prepare.py
 idf_component_manager/templates/idf_component_template.yml
 idf_component_manager/version_solver/__init__.py
 idf_component_manager/version_solver/helper.py
 idf_component_manager/version_solver/version_solver.py
@@ -46,14 +55,15 @@
 idf_component_tools/api_client.py
 idf_component_tools/api_client_errors.py
 idf_component_tools/api_schemas.py
 idf_component_tools/archive_tools.py
 idf_component_tools/build_system_tools.py
 idf_component_tools/config.py
 idf_component_tools/constants.py
+idf_component_tools/environment.py
 idf_component_tools/errors.py
 idf_component_tools/file_cache.py
 idf_component_tools/file_tools.py
 idf_component_tools/git_client.py
 idf_component_tools/hash_tools.py
 idf_component_tools/serialization.py
 idf_component_tools/lock/__init__.py
```

### Comparing `idf_component_manager-1.2.3/idf_component_manager.egg-info/requires.txt` & `idf_component_manager-1.3.0.dev0/idf_component_manager.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 future
 packaging
 requests<3
-urllib3<2
 requests-file
 requests-toolbelt
 schema
 six
 tqdm<5
 
 [:python_version < "3"]
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/api_client.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from requests_file import FileAdapter
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 from schema import Schema, SchemaError
 from tqdm import tqdm
 
 # Import whole module to avoid circular dependencies
 import idf_component_tools as tools
-from idf_component_tools import file_cache
 from idf_component_tools.__version__ import __version__
 from idf_component_tools.errors import warn
+from idf_component_tools.file_cache import FileCache as ComponentFileCache
 from idf_component_tools.semver import SimpleSpec, Version
 
 from .api_client_errors import (
     KNOWN_API_ERRORS, APIClientError, ComponentNotFound, NetworkConnectionError, NoRegistrySet, StorageFileNotFound,
     VersionNotFound)
 from .api_schemas import (
     API_INFORMATION_SCHEMA, COMPONENT_SCHEMA, ERROR_SCHEMA, TASK_STATUS_SCHEMA, VERSION_UPLOAD_SCHEMA)
@@ -59,19 +59,22 @@
             'Please set the variable to the number of minutes. '
             'Using the default value of {} minutes.'.format(DEFAULT_API_CACHE_EXPIRATION_MINUTES))
         return DEFAULT_API_CACHE_EXPIRATION_MINUTES
 
 
 def create_session(
         cache=False,  # type: bool
-        cache_path=file_cache.FileCache.path(),  # type: str
+        cache_path=None,  # type: str | None
         cache_time=None,  # type: int | None
         token=None,  # type: str | None
 ):  # type: (...) -> requests.Session
 
+    if cache_path is None:
+        cache_path = ComponentFileCache().path()
+
     cache_time = cache_time or env_cache_time()
     if cache and cache_time:
         api_adapter = CacheControlAdapter(
             max_retries=MAX_RETRIES,
             heuristic=ExpiresAfter(minutes=cache_time),
             cache=FileCache(os.path.join(cache_path, '.api_client')))
     else:
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/api_client_errors.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_client_errors.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/api_schemas.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/api_schemas.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/archive_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/archive_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/build_system_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/build_system_tools.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/config.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import warnings
 from io import open
 
 import yaml
 from schema import And, Optional, Or, Regex, Schema, SchemaError
 from six import string_types
 
 from idf_component_tools.constants import COMPILED_URL_RE
-from idf_component_tools.errors import FatalError
+from idf_component_tools.errors import FatalError, UserDeprecationWarning
 
 from .constants import IDF_COMPONENT_REGISTRY_URL, IDF_COMPONENT_STORAGE_URL
 
 DEFAULT_CONFIG_DIR = os.path.join('~', '.espressif')
 CONFIG_DIR = os.environ.get('IDF_TOOLS_PATH') or os.path.expanduser(DEFAULT_CONFIG_DIR)
 
 CONFIG_SCHEMA = Schema(
@@ -96,15 +96,15 @@
     env_registry_url = os.getenv('IDF_COMPONENT_REGISTRY_URL')
     env_registry_api_url = os.getenv('DEFAULT_COMPONENT_SERVICE_URL')
 
     if env_registry_api_url:
         warnings.warn(
             'DEFAULT_COMPONENT_SERVICE_URL environment variable pointing to the registy API is deprecated. '
             'Set component registry URL to IDF_COMPONENT_REGISTRY_URL',
-            category=DeprecationWarning)
+            category=UserDeprecationWarning)
 
     if env_registry_url and env_registry_api_url:
         warnings.warn(
             'Both DEFAULT_COMPONENT_SERVICE_URL and IDF_COMPONENT_REGISTRY_URL '
             'environment variables are defined. The value of IDF_COMPONENT_REGISTRY_URL is used.')
 
     if env_registry_url:
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/constants.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 # Copyright (c) 2017, Jon Schlinkert.
 # Originally released under the MIT License.
 
 import re
 
 URL_RE = (
     r'^https?://'  # http:// or https://
-    r'(?:(?:[A-Z0-9](?:[A-Z0-9-]{0,61}[A-Z0-9])?\.)+(?:[A-Z]{2,6}\.?|[A-Z0-9-]{2,}\.?)|'  # domain
+    # here use A-Za-z even with re.IGNORECASE is because json schema does not support flags
+    r'(?:(?:[A-Za-z0-9](?:[A-Za-z0-9-]{0,61}[A-Za-z0-9])?\.)+(?:[A-Za-z]{2,6}\.?|[A-Za-z0-9-]{2,}\.?)|'  # domain
     r'localhost|'  # or localhost
     r'\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})'  # or ip
     r'(?::\d+)?'  # optional port
     r'(?:/?|[/?]\S+)$')
 COMPILED_URL_RE = re.compile(URL_RE, re.IGNORECASE)
 
-GIT_URL_RE = r'^(?:git|ssh|https?|git@[-\w.]+):(//)?(.*?)(\.git)(/?|#[-\d\w._]+?)$'
+GIT_URL_RE = r'^(?:git|ssh|https?|git@[-\w.]+):(\/\/)?(.*)(\.git)?(/?|#[-\d\w._]+?)$'
 COMPILED_GIT_URL_RE = re.compile(GIT_URL_RE, re.IGNORECASE)
 
 # Registry related constants
 DEFAULT_NAMESPACE = 'espressif'
 IDF_COMPONENT_REGISTRY_URL = 'https://components.espressif.com/'
 IDF_COMPONENT_STORAGE_URL = 'https://components-file.espressif.com/'
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/errors.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import warnings
 
 try:
     from typing import Any
 except ImportError:
     pass
 
 
 class UserHint(Warning):
     pass
 
 
+class UserDeprecationWarning(UserWarning):
+    pass
+
+
 def warn(message):  # type: (Exception | str) -> None
     warnings.warn(str(message))
 
 
 def hint(message):  # type: (Exception | str) -> None
     warnings.warn(str(message), category=UserHint)
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/file_cache.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/file_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,48 +4,67 @@
 # Contains elements taken from "appdirs" python package
 # https://github.com/ActiveState/appdirs/tree/1.4.3
 # Copyright (c) 2005-2010 ActiveState Software Inc.
 # Copyright (c) 2013 Eddy Petrisor
 # Originally released under MIT license
 """Classes to work with file cache"""
 
+import errno
 import os
+import shutil
 import sys
 
+from idf_component_tools.errors import FatalError
+from idf_component_tools.file_tools import directory_size
 
-class FileCache(object):
-    """Common functions to work with components cache"""
 
-    _path = None
-
-    @classmethod
-    def path(cls):
-        if not cls._path:
-            cls._path = cls.cache_path()
-
-            if not os.path.exists(cls._path):
-                os.makedirs(cls._path)
-
-        return cls._path
-
-    @classmethod
-    def cache_path(cls):
-        """Path of cache directory"""
-        system_cache_path = SystemCachePath()
-
-        if sys.platform.startswith('win'):
-            cache_directory = system_cache_path.cache_path_win()
-            return os.path.join(cache_directory, 'Espressif', 'ComponentManager', 'Cache')
+def system_cache_path():  # type: () -> str
+    """Path of system cache directory"""
+    system_cache_path = SystemCachePath()
+
+    if sys.platform.startswith('win'):
+        cache_directory = system_cache_path.cache_path_win()
+        return os.path.join(cache_directory, 'Espressif', 'ComponentManager', 'Cache')
+    else:
+        if sys.platform == 'darwin':
+            cache_directory = system_cache_path.cache_path_macos()
         else:
-            if sys.platform == 'darwin':
-                cache_directory = system_cache_path.cache_path_macos()
-            else:
-                cache_directory = system_cache_path.cache_path_unix()
+            cache_directory = system_cache_path.cache_path_unix()
+
+        return os.path.join(cache_directory, 'Espressif', 'ComponentManager')
+
+
+class FileCache(object):
+    """Common functions to work with components cache"""
+    def __init__(self, path=None):  # type: (str | None) -> None
+        self._path = path  # type: str | None
 
-            return os.path.join(cache_directory, 'Espressif', 'ComponentManager')
+    def path(self):  # type: () -> str
+        """Path of cache directory. Make directory if it doesn't exist"""
+        if not self._path:
+            self._path = os.getenv('IDF_COMPONENT_CACHE_PATH')
+
+        if not self._path:
+            self._path = system_cache_path()
+
+        try:
+            os.makedirs(self._path)
+        except OSError as e:
+            if e.errno != errno.EEXIST:
+                raise FatalError('Failed to create cache directory: {}'.format(self._path))
+
+        return self._path
+
+    def clear(self):  # type: () -> None
+        '''Clear cache directory'''
+        shutil.rmtree(self.path())
+
+    def size(self):  # type: () -> int
+        """Disk usage of cache directory"""
+        return directory_size(self.path())
 
 
 class SystemCachePath(object):
     """Methods to fetch user specific cache path for every platform"""
 
     PY3 = sys.version_info[0] == 3
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/file_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/file_tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -149,7 +149,36 @@
     for root, _dirs, files in os.walk(str(path)):
         unexpected_files = UNEXPECTED_FILES.intersection(files)
         if unexpected_files:
             warn(
                 'Unexpected files "{files}" found in the component directory "{path}". '
                 'Please check if these files should be ignored'.format(
                     files=', '.join(unexpected_files), path=os.path.relpath(root, start=str(path))))
+
+
+def directory_size(dir_path):  # type: (str) -> int
+    '''Return the total size of all files in the directory tree'''
+    total_size = 0
+    directory = Path(dir_path)
+    for file in directory.glob('**/*'):
+        try:
+            total_size += os.stat(str(file)).st_size
+        except OSError:
+            pass
+    return total_size
+
+
+def human_readable_size(size):  # type: (int) -> str
+    '''Return a human readable string representation of a data size'''
+    if size < 0:
+        raise ValueError('size must be non-negative')
+
+    if size < 1024:
+        return '{} bytes'.format(size)
+
+    if size < 1024**2:
+        return '{:.2f} KB'.format(size / 1024.0)
+
+    if size < 1024**3:
+        return '{:.2f} MB'.format(size / (1024.0**2))
+
+    return '{:.2f} GB'.format(size / (1024.0**3))
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/git_client.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/git_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,17 @@
             Commit id of the current checkout
         """
         commit_id = self.get_commit_id_by_ref(repo, bare_path, ref)
 
         # Checkout required branch
         checkout_command = ['--work-tree', checkout_path, '--git-dir', bare_path, 'checkout', '--force', commit_id]
         if selected_paths:
+            if '.gitmodules' not in selected_paths and self.has_gitmodules_by_ref(repo, bare_path, commit_id):
+                # avoid submodule update failed
+                selected_paths += ['.gitmodules']
             checkout_command += ['--'] + selected_paths
         self.run(checkout_command)
 
         # And remove all untracked files
         self.run(['--work-tree', checkout_path, '--git-dir', bare_path, 'clean', '--force'])
         # Submodules
         if with_submodules:
@@ -159,14 +162,19 @@
 
         else:
             # Set to latest commit from remote's HEAD
             ref = self.run(['ls-remote', '--exit-code', 'origin', 'HEAD'], cwd=bare_path)[:40]
 
         return self.run(['rev-parse', '--verify', ref], cwd=bare_path).strip()
 
+    @_git_cmd
+    @_bare_repo
+    def has_gitmodules_by_ref(self, repo, bare_path, ref):  # type: (str, str, str) -> bool
+        return '.gitmodules' in self.run(['ls-tree', '--name-only', ref], cwd=bare_path).splitlines()
+
     def run(self, args, cwd=None, env=None):  # type: (List[str], str | None, dict | None) -> str
         if cwd is None:
             cwd = os.getcwd()
         env_copy = dict(os.environ)
         if env:
             env_copy.update(env)
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/hash_tools.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/hash_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import json
 import os
 import re
 from hashlib import sha256
 from io import open
 from pathlib import Path
 
-from .file_tools import filtered_paths
+from idf_component_tools.environment import getenv_bool
+from idf_component_tools.file_tools import filtered_paths
 
 try:
     from typing import Any, Iterable, Text
 except ImportError:
     pass
 
 BLOCK_SIZE = 65536
@@ -95,15 +96,19 @@
 
 
 def validate_filtered_dir(root, component_hash):  # type: (Text | Path, str) -> bool
     """Validate component in managed directory"""
     return validate_dir(root, component_hash, exclude=['**/.component_hash'], exclude_default=False)
 
 
-def validate_dir_with_hash_file(root):  # type: (str) -> None
+def validate_managed_component_hash(root):  # type: (str) -> None
+    '''Validate managed components directory, raise exception if validation fails'''
+    if getenv_bool('IDF_COMPONENT_OVERWRITE_MANAGED_COMPONENTS'):
+        return
+
     hash_file_path = os.path.join(root, HASH_FILENAME)
 
     if not os.path.isdir(root) or not os.path.exists(hash_file_path):
         raise HashDoesNotExistError()
 
     with open(hash_file_path, mode='r', encoding='utf-8') as f:
         hash_from_file = f.read().strip()
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/lock/manager.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/lock/manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from collections import OrderedDict
 from io import open
 
 from schema import And, Optional, Or, Schema, SchemaError, Use
 from six import string_types
 from yaml import Node, SafeDumper, YAMLError
 from yaml import dump as dump_yaml
 from yaml import safe_load
 
 import idf_component_tools as tools
 
-from ..build_system_tools import get_env_idf_target
+from ..build_system_tools import get_env_idf_target, get_idf_version
 from ..errors import LockError
-from ..manifest import SolvedManifest
+from ..manifest import ComponentVersion, SolvedComponent, SolvedManifest
 from ..manifest.validator import known_targets
+from ..sources import IDFSource
 
 FORMAT_VERSION = '1.0.0'
 
 EMPTY_LOCK = {
     'manifest_hash': None,
     'version': FORMAT_VERSION,
 }
@@ -59,14 +60,21 @@
         self._path = path
 
     def exists(self):
         return os.path.isfile(self._path)
 
     def dump(self, solution):  # type: (SolvedManifest) -> None
         """Writes updated lockfile to disk"""
+        # add idf version if not in solution.dependencies
+        if 'idf' not in solution.solved_components:
+            solution.dependencies.append(SolvedComponent(
+                'idf',
+                ComponentVersion(get_idf_version()),
+                IDFSource(),
+            ))
 
         try:
             with open(self._path, mode='w', encoding='utf-8') as f:
                 # inject format version
                 solution_dict = solution.serialize()
                 solution_dict['version'] = FORMAT_VERSION
                 solution_dict['target'] = get_env_idf_target()
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/__init__.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/constants.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/constants.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/env_expander.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/env_expander.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/if_parser.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/if_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,14 +37,30 @@
     def __init__(self, clause, bool_value):  # type: (str, bool) -> None
         self.clause = clause
         self.bool_value = bool_value
 
     def __repr__(self):
         return '{} ({})'.format(self.clause, self.bool_value)
 
+    @staticmethod
+    def regex_str():
+        if_idf_version = IF_IDF_VERSION_REGEX
+        # remove the name group
+        if_idf_version = re.sub(r'\(\?P<\w+>', '(?:', if_idf_version)
+        # remove the first ^ and the last $ and make it as a group
+        if_idf_version = '(' + if_idf_version[1:-1] + ')'
+
+        if_target = IF_TARGET_REGEX
+        # remove the name group
+        if_target = re.sub(r'\(\?P<\w+>', '(?:', if_idf_version)
+        # remove the first ^ and the last $ and make it as a group
+        if_target = '(' + if_target[1:-1] + ')'
+
+        return '^{}|{}$'.format(if_idf_version, if_target)
+
 
 def _eval_str(s):  # type: (str) -> str
     _s = s.strip()
     if not (_s[0] == _s[-1] == '"'):
         _s = '"{}"'.format(_s.replace('"', r'\"'))
 
     try:
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/manager.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
-import copy
 import os
 import sys
 from io import open
 
 import yaml
 
 from ..errors import ManifestError
@@ -52,15 +51,15 @@
         self.check_required_fields = check_required_fields
 
     def validate(self):
         validator = ManifestValidator(
             self.manifest_tree, check_required_fields=self.check_required_fields, version=self.version)
         self._validation_errors = validator.validate_normalize()
         self._is_valid = not self._validation_errors
-        self._normalized_manifest_tree = copy.deepcopy(validator.manifest_tree)
+        self._normalized_manifest_tree = validator.manifest_tree
         return self
 
     @property
     def is_valid(self):
         if self._is_valid is None:
             self.validate()
 
@@ -136,16 +135,16 @@
 
             error_desc.append(UPDATE_SUGGESTION)
 
             raise ManifestError('\n'.join(error_desc))
 
         for name, details in self.normalized_manifest_tree.get('dependencies', {}).items():
             if 'rules' in details:
-                self.normalized_manifest_tree['dependencies'][name]['rules'] = [rule['if'] for rule in details['rules']]
+                self.manifest_tree['dependencies'][name]['rules'] = [rule['if'] for rule in details['rules']]
 
-        return Manifest.fromdict(self.normalized_manifest_tree, name=self.name, manifest_manager=self)
+        return Manifest.fromdict(self.manifest_tree, name=self.name, manifest_manager=self)
 
     def dump(self, path=None):  # type: (str | None) -> None
         if path is None:
             path = self.path
 
         dump_tree(path, self.manifest_tree)
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/manifest.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,21 @@
 
         return all(if_clause.bool_value for if_clause in self.if_clauses)
 
     def __repr__(self):  # type: () -> str
         return 'ComponentRequirement("{}", {}, version_spec="{}", public={})'.format(
             self._name, self.source, self.version_spec, self.public)
 
+    def __str__(self):  # type: () -> str
+        # if local source, avoid circular dependency
+        if self.source.name == 'local':
+            return '{}({})'.format(self._name, self.source._path)  # type: ignore
+        else:
+            return '{}({})'.format(self._name, self._version_spec)
+
 
 @total_ordering
 @serializable(like='str')
 class ComponentVersion(object):
     def __init__(self, version_string, dependencies=None):  # type: (str, list[ComponentRequirement] | None) -> None
         """
         version_string - can be `*`, git commit hash (hex, 160 bit) or valid semantic version string
@@ -272,20 +279,20 @@
         else:
             raise TypeError('Version is not semantic')
 
 
 class HashedComponentVersion(ComponentVersion):
     def __init__(self, *args, **kwargs):
         component_hash = kwargs.pop('component_hash', None)
-        dependencies = kwargs.pop('dependencies', [])
+        dependencies = kwargs.pop('dependencies', []) or []
         targets = kwargs.pop('targets', [])
         super(HashedComponentVersion, self).__init__(*args, **kwargs)
 
         self.component_hash = component_hash
-        self.dependencies = dependencies  # type: list[ComponentRequirement] | None
+        self.dependencies = dependencies  # type: list[ComponentRequirement]
         self.targets = targets
 
     def __hash__(self):
         return hash(self.component_hash) if self.component_hash else hash(str(self))
 
     @property
     def text(self):
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/solved_component.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_component.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,16 +37,19 @@
         self.source = source
         self.component_hash = component_hash
 
         if dependencies is None:
             dependencies = []
         self.dependencies = dependencies
 
+    def __repr__(self):
+        return 'SolvedComponent <{}({}) {}>'.format(self.name, self.version, self.component_hash)
+
     def __str__(self):
-        return 'SolvedComponent: %s %s %s' % (self.name, self.version, self.component_hash)
+        return '{}({})'.format(self.name, self.version)
 
     @classmethod
     def fromdict(cls, details):
         try:
             source_details = dict(details['source'])
             source_name = source_details.pop('type')
             source = BaseSource.fromdict(source_name, source_details)
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/solved_manifest.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/solved_manifest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 from .solved_component import SolvedComponent
 
 try:
     from typing import Dict, List, Optional
 except ImportError:
@@ -47,7 +47,11 @@
             'target': self.target,
         }
 
         if dependencies:
             solution['dependencies'] = dependencies
 
         return solution
+
+    @property
+    def solved_components(self):  # type: () -> dict[str, SolvedComponent]
+        return {cmp.name: cmp for cmp in self.dependencies}
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/manifest/validator.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/manifest/validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-# SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
+# SPDX-FileCopyrightText: 2022 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 import re
 import sys
 
 from schema import And, Optional, Or, Regex, Schema, SchemaError, Use
 from six import string_types
 
 import idf_component_tools as tools
+from idf_component_manager.utils import RE_PATTERN
 
 from ..constants import COMPILED_GIT_URL_RE, COMPILED_URL_RE
 from ..errors import SourceError
-from ..semver import Version
+from ..semver import SimpleSpec, Version
 from .constants import FULL_SLUG_REGEX, LINKS, TAGS_REGEX
-from .if_parser import parse_if_clause
+from .if_parser import IfClause, parse_if_clause
 
 try:
-    from typing import Iterable, List
+    from typing import Any, Callable, Iterable, List
 except ImportError:
     pass
 
 KNOWN_ROOT_KEYS = [
     'name',  # Name key is ignored
     'maintainers',
     'dependencies',
@@ -29,15 +30,15 @@
     'version',
     'description',
     'files',
     'tags',
     'examples'
 ] + LINKS
 
-DEFAULT_KNOWN_TARGETS = ['esp32', 'esp32s2', 'esp32c3', 'esp32s3', 'esp32c2', 'esp32c6', 'esp32h2', 'linux']
+DEFAULT_KNOWN_TARGETS = ['esp32', 'esp32s2', 'esp32c3', 'esp32s3', 'linux', 'esp32h2', 'esp32h4', 'esp32c2', 'esp32c6']
 
 KNOWN_FILES_KEYS = [
     'include',
     'exclude',
 ]
 
 KNOWN_EXAMPLES_KEYS = ['path']
@@ -131,14 +132,54 @@
             Optional('issues'): Regex(COMPILED_URL_RE, error=LINKS_URL_ERROR.format('issues')),
             Optional('discussion'): Regex(COMPILED_URL_RE, error=LINKS_URL_ERROR.format('discussion')),
         },
         error='Invalid manifest format',
     )
 
 
+def manifest_json_schema():  # type: () -> dict
+    def replace_regex_pattern_with_pattern_str(pat):  # type: (re.Pattern) -> Any
+        return pat.pattern
+
+    def process_nested_regex(
+            obj,  # type: dict[str, Any] | list | str | Any
+            func  # type: Callable[[re.Pattern], Any]
+    ):
+        # type: (...) -> dict[str, Any] | list | str | Any
+
+        if isinstance(obj, dict):
+            if not obj.get('required', []):
+                obj.pop('required', None)  # jsonschema 2.5.1 for python 3.4 does not support empty `required` field
+            return {k: process_nested_regex(v, func) for k, v in obj.items()}
+        elif isinstance(obj, RE_PATTERN):
+            return func(obj)
+        elif isinstance(obj, (list, tuple)):
+            # yaml dict won't have other iterable data types
+            return [process_nested_regex(i, func) for i in obj]
+
+        # we don't process other data types, like numbers
+        return obj
+
+    json_schema = manifest_schema().json_schema(
+        'idf-component-manager')  # here id should be an url to use $ref in the future
+    # `version` field is too complicated to be auto-generated. we use an approx regex instead
+    json_schema['properties']['version'] = {'type': 'string', 'pattern': SimpleSpec.regex_str()}
+    # `dependency` field we're using arbitrary string as key
+    json_schema['properties']['dependencies']['additionalProperties'] = {
+        'anyOf': Schema(dependency_schema()).json_schema('#dependency')['anyOf']
+    }
+    # the IfClause should be a string as well
+    _anyof = json_schema['properties']['dependencies']['additionalProperties']['anyOf']
+    _anyof[1]['properties']['rules']['items']['properties']['if'] = {'type': 'string', 'pattern': IfClause.regex_str()}
+    # `re.Pattern` should use the pattern string instead
+    json_schema = process_nested_regex(json_schema, replace_regex_pattern_with_pattern_str)
+
+    return json_schema
+
+
 class ManifestValidator(object):
     """Validator for manifest object, checks for structure, known fields and valid values"""
     def __init__(
             self, parsed_manifest, check_required_fields=False, version=None):  # type: (dict, bool, str | None) -> None
         self.manifest_tree = parsed_manifest
         self.version = version
         self._errors = []  # type: List[str]
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/semver/base.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/semver/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -819,14 +819,26 @@
 
 
 class SimpleSpec(BaseSpec):
     @classmethod
     def _parse_to_clause(cls, expression):
         return cls.Parser.parse(expression)
 
+    @classmethod
+    def regex_str(cls):
+        naive_spec_string = cls.Parser.NAIVE_SPEC.pattern
+        # remove the \n and the extra spaces
+        naive_spec_string = ''.join([line.strip() for line in naive_spec_string.split()])
+        # remove the name group
+        naive_spec_string = re.sub(r'\(\?P<\w+>', '(?:', naive_spec_string)
+        # remove the first ^ and the last $ and make it as a group
+        naive_spec_group = '(' + naive_spec_string[1:-1] + ')'
+        # ^group(,group)*$ means it could be a comma separated lists
+        return '^{}(,{})*$'.format(naive_spec_group, naive_spec_group)
+
     class Parser:
         NUMBER = r'\*|0|[1-9][0-9]*'
         NAIVE_SPEC = re.compile(
             r"""^
             (?P<op><|<=||=|==|>=|>|!=|\^|~|~=)
             (?P<major>{nb})(?:\.(?P<minor>{nb})(?:\.(?P<patch>{nb}))?)?
             (?:~(?P<revision>\d+))?
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/serialization.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/serialization.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/__init__.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/base.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             system_cache_path=None,  # type: str | None
             manifest_manager=None,  # type: ManifestManager | None
     ):  # type: (...) -> None
         self._source_details = source_details or {}
         self._hash_key = None
 
         if system_cache_path is None:
-            system_cache_path = FileCache.path()
+            system_cache_path = FileCache().path()
         self.system_cache_path = system_cache_path
 
         self.is_overrider = False
 
         unknown_keys = [key for key in self._source_details.keys() if key not in self.known_keys()]
         if unknown_keys:
             raise SourceError('Unknown keys in dependency details: %s' % ', '.join(unknown_keys))
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/fetcher.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 from io import open
 
 from ..build_system_tools import build_name
 from ..errors import ComponentModifiedError, InvalidComponentHashError
 from ..hash_tools import (
-    HASH_FILENAME, HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error, validate_dir_with_hash_file)
+    HASH_FILENAME, HashDoesNotExistError, HashNotEqualError, HashNotSHA256Error, validate_managed_component_hash)
 from ..manifest import SolvedComponent
 
 try:
     from typing import TYPE_CHECKING
 
     if TYPE_CHECKING:
         from . import BaseSource
@@ -31,15 +31,15 @@
         self.component = solved_component
         self.components_path = components_path
         self.managed_path = os.path.join(self.components_path, build_name(self.component.name))
 
     def download(self):  # type: () -> str | None
         """If necessary, it downloads component and returns local path to component directory"""
         try:
-            validate_dir_with_hash_file(self.managed_path)
+            validate_managed_component_hash(self.managed_path)
         except HashNotEqualError:
             raise ComponentModifiedError(
                 'Component directory was modified on the disk since the last run of '
                 'the CMake')
         except HashNotSHA256Error:
             raise InvalidComponentHashError(
                 'File .component_hash for component "{}" in the managed '
```

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/git.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/git.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/idf.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/idf.py`

 * *Files identical despite different names*

### Comparing `idf_component_manager-1.2.3/idf_component_tools/sources/web_service.py` & `idf_component_manager-1.3.0.dev0/idf_component_tools/sources/web_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 IDF_COMPONENT_REGISTRY_API_URL = '{}api/'.format(IDF_COMPONENT_REGISTRY_URL)
 
 
 def download_archive(url, download_dir):  # type: (str, str) -> str
     session = api_client.create_session(cache=False)
 
     try:
-        with session.get(url, stream=True, allow_redirects=True) as r:
+        with session.get(url, stream=True, allow_redirects=True) as r:  # type: requests.Response
             # Trying to get extension from url
             original_filename = url.split('/')[-1]
 
             try:
                 extension = get_format_from_path(original_filename)[1]
             except ArchiveError:
                 extension = None
```

### Comparing `idf_component_manager-1.2.3/setup.py` & `idf_component_manager-1.3.0.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     'future',
     'packaging',
     'pathlib;python_version<"3.4"',
     'pyyaml<=5.2;python_version=="3.4.*"',
     'pyyaml>5.2;python_version>="3.5"',
     'pyyaml<=5.2;python_version=="2.7.*"',
     'requests<3',
-    'urllib3<2',
     'requests-file',
     'requests-toolbelt',
     'schema',
     'six',
     'tqdm<5',
 ]
 
@@ -74,14 +73,15 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
     ],
     packages=setuptools.find_packages(
         exclude=('*.tests', '*.tests.*', 'tests.*', 'tests', '*_tests', '*_tests_*', 'tests_*')),
     scripts=[],
     install_requires=REQUIRES,
     python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
```

