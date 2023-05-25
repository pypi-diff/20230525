# Comparing `tmp/regipy-3.1.5.tar.gz` & `tmp/regipy-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regipy-3.1.5.tar", last modified: Thu Feb 23 10:07:20 2023, max compression
+gzip compressed data, was "regipy-3.1.6.tar", last modified: Thu May 25 10:53:09 2023, max compression
```

## Comparing `regipy-3.1.5.tar` & `regipy-3.1.6.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.043032 regipy-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-23 10:07:00.000000 regipy-3.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-23 10:07:00.000000 regipy-3.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-23 10:07:20.043032 regipy-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-02-23 10:07:00.000000 regipy-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-23 10:07:00.000000 regipy-3.1.5/docs/PLUGINS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-23 10:07:00.000000 regipy-3.1.5/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/regipy/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/hive_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/regipy/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/regipy/plugins/amcache/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/amcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/amcache/amcache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/regipy/plugins/bcd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/bcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/bcd/boot_entry_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/ntuser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/installed_programs_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/network_drives.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/shellbags_ntuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/tsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/typed_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/typed_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/user_assist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/winrar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/winscp_saved_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/ntuser/word_wheel_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/plugin_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/sam/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/sam/local_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/security/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/security/domain_sid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/software/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/image_file_execution_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/installed_programs.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/last_logon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/printdemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/profilelist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/software/uac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/system/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/active_controlset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/bam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/bootkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/computer_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/system/external/
--rwxr-xr-x   0 runner    (1001) docker     (123)    17381 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/external/ShimCacheParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/host_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/safeboot_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/shimcache.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/timezone_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/usbstor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/system/wdigest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.039032 regipy-3.1.5/regipy/plugins/usrclass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/usrclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/usrclass/classes_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/regdiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    26689 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/security_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-02-23 10:07:00.000000 regipy-3.1.5/regipy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 10:07:20.035032 regipy-3.1.5/regipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-23 10:07:20.000000 regipy-3.1.5/regipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 10:07:20.043032 regipy-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-23 10:07:00.000000 regipy-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.084046 regipy-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 10:52:52.000000 regipy-3.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 10:52:52.000000 regipy-3.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 10:53:09.080046 regipy-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-05-25 10:52:52.000000 regipy-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.068045 regipy-3.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 10:52:52.000000 regipy-3.1.6/docs/PLUGINS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-25 10:52:52.000000 regipy-3.1.6/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.068045 regipy-3.1.6/regipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/hive_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/amcache/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/amcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/amcache/amcache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/bcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/bcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/bcd/boot_entry_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/ntuser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/installed_programs_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/network_drives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/shellbags_ntuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/tsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/typed_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/typed_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/user_assist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/winrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/winscp_saved_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/ntuser/word_wheel_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/plugin_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/sam/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/sam/local_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/security/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/security/domain_sid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy/plugins/software/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/image_file_execution_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/installed_programs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/last_logon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/printdemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/profilelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/software/uac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.080046 regipy-3.1.6/regipy/plugins/system/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/active_controlset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/bam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/bootkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/computer_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.080046 regipy-3.1.6/regipy/plugins/system/external/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17381 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/external/ShimCacheParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/host_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/network_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/safeboot_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/shimcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/timezone_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/usbstor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/system/wdigest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.080046 regipy-3.1.6/regipy/plugins/usrclass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/usrclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/usrclass/classes_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/regdiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26689 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/security_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-25 10:52:52.000000 regipy-3.1.6/regipy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:53:09.072046 regipy-3.1.6/regipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 10:53:09.000000 regipy-3.1.6/regipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 10:53:09.084046 regipy-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-25 10:52:52.000000 regipy-3.1.6/setup.py
```

### Comparing `regipy-3.1.5/LICENSE` & `regipy-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/PKG-INFO` & `regipy-3.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 3.1.5
+Version: 3.1.6
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `regipy-3.1.5/README.md` & `regipy-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/docs/PLUGINS.md` & `regipy-3.1.6/docs/PLUGINS.md`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/docs/README.rst` & `regipy-3.1.6/docs/README.rst`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/cli.py` & `regipy-3.1.6/regipy/cli.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/cli_utils.py` & `regipy-3.1.6/regipy/cli_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/exceptions.py` & `regipy-3.1.6/regipy/exceptions.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/hive_types.py` & `regipy-3.1.6/regipy/hive_types.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/__init__.py` & `regipy-3.1.6/regipy/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,7 +31,8 @@
 from .system.safeboot_configuration import SafeBootConfigurationPlugin
 from .system.services import ServicesPlugin
 from .system.shimcache import ShimCachePlugin
 from .system.timezone_data import TimezoneDataPlugin
 from .system.usbstor import USBSTORPlugin
 from .system.wdigest import WDIGESTPlugin
 from .usrclass.classes_installer import ClassesInstallerPlugin
+from .system.network_data import NetworkDataPlugin
```

### Comparing `regipy-3.1.5/regipy/plugins/amcache/amcache.py` & `regipy-3.1.6/regipy/plugins/amcache/amcache.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/bcd/boot_entry_list.py` & `regipy-3.1.6/regipy/plugins/bcd/boot_entry_list.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/installed_programs_ntuser.py` & `regipy-3.1.6/regipy/plugins/ntuser/installed_programs_ntuser.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/network_drives.py` & `regipy-3.1.6/regipy/plugins/ntuser/network_drives.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/persistence.py` & `regipy-3.1.6/regipy/plugins/ntuser/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/shellbags_ntuser.py` & `regipy-3.1.6/regipy/plugins/ntuser/shellbags_ntuser.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/tsclient.py` & `regipy-3.1.6/regipy/plugins/ntuser/tsclient.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/typed_paths.py` & `regipy-3.1.6/regipy/plugins/ntuser/typed_paths.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/typed_urls.py` & `regipy-3.1.6/regipy/plugins/ntuser/typed_urls.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/user_assist.py` & `regipy-3.1.6/regipy/plugins/ntuser/user_assist.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/winrar.py` & `regipy-3.1.6/regipy/plugins/ntuser/winrar.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/winscp_saved_sessions.py` & `regipy-3.1.6/regipy/plugins/ntuser/winscp_saved_sessions.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/ntuser/word_wheel_query.py` & `regipy-3.1.6/regipy/plugins/ntuser/word_wheel_query.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/plugin.py` & `regipy-3.1.6/regipy/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/plugin_template.py` & `regipy-3.1.6/regipy/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/sam/local_sid.py` & `regipy-3.1.6/regipy/plugins/sam/local_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/security/domain_sid.py` & `regipy-3.1.6/regipy/plugins/security/domain_sid.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/classes_installer.py` & `regipy-3.1.6/regipy/plugins/software/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/image_file_execution_options.py` & `regipy-3.1.6/regipy/plugins/software/image_file_execution_options.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/installed_programs.py` & `regipy-3.1.6/regipy/plugins/software/installed_programs.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/last_logon.py` & `regipy-3.1.6/regipy/plugins/software/last_logon.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/persistence.py` & `regipy-3.1.6/regipy/plugins/software/persistence.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/printdemon.py` & `regipy-3.1.6/regipy/plugins/software/printdemon.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/profilelist.py` & `regipy-3.1.6/regipy/plugins/software/profilelist.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/tracing.py` & `regipy-3.1.6/regipy/plugins/software/tracing.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/software/uac.py` & `regipy-3.1.6/regipy/plugins/software/uac.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/active_controlset.py` & `regipy-3.1.6/regipy/plugins/system/active_controlset.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/bam.py` & `regipy-3.1.6/regipy/plugins/system/bam.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/bootkey.py` & `regipy-3.1.6/regipy/plugins/system/bootkey.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/computer_name.py` & `regipy-3.1.6/regipy/plugins/system/computer_name.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/external/ShimCacheParser.py` & `regipy-3.1.6/regipy/plugins/system/external/ShimCacheParser.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/host_domain_name.py` & `regipy-3.1.6/regipy/plugins/system/host_domain_name.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/routes.py` & `regipy-3.1.6/regipy/plugins/system/routes.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/safeboot_configuration.py` & `regipy-3.1.6/regipy/plugins/system/safeboot_configuration.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/services.py` & `regipy-3.1.6/regipy/plugins/system/services.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/shimcache.py` & `regipy-3.1.6/regipy/plugins/system/shimcache.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/timezone_data.py` & `regipy-3.1.6/regipy/plugins/system/timezone_data.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/usbstor.py` & `regipy-3.1.6/regipy/plugins/system/usbstor.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/system/wdigest.py` & `regipy-3.1.6/regipy/plugins/system/wdigest.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/usrclass/classes_installer.py` & `regipy-3.1.6/regipy/plugins/usrclass/classes_installer.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/plugins/utils.py` & `regipy-3.1.6/regipy/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/recovery.py` & `regipy-3.1.6/regipy/recovery.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/regdiff.py` & `regipy-3.1.6/regipy/regdiff.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/registry.py` & `regipy-3.1.6/regipy/registry.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/security_utils.py` & `regipy-3.1.6/regipy/security_utils.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/structs.py` & `regipy-3.1.6/regipy/structs.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy/utils.py` & `regipy-3.1.6/regipy/utils.py`

 * *Files identical despite different names*

### Comparing `regipy-3.1.5/regipy.egg-info/PKG-INFO` & `regipy-3.1.6/regipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regipy
-Version: 3.1.5
+Version: 3.1.6
 Summary: Python Registry Parser
 Home-page: https://github.com/mkorman90/regipy/
 Author: Martin G. Korman
 Author-email: martin@centauri.co.il
 License: MIT
 Keywords: Python,Python3,registry,windows registry,registry parser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `regipy-3.1.5/regipy.egg-info/SOURCES.txt` & `regipy-3.1.6/regipy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 regipy/plugins/software/uac.py
 regipy/plugins/system/__init__.py
 regipy/plugins/system/active_controlset.py
 regipy/plugins/system/bam.py
 regipy/plugins/system/bootkey.py
 regipy/plugins/system/computer_name.py
 regipy/plugins/system/host_domain_name.py
+regipy/plugins/system/network_data.py
 regipy/plugins/system/routes.py
 regipy/plugins/system/safeboot_configuration.py
 regipy/plugins/system/services.py
 regipy/plugins/system/shimcache.py
 regipy/plugins/system/timezone_data.py
 regipy/plugins/system/usbstor.py
 regipy/plugins/system/wdigest.py
```

### Comparing `regipy-3.1.5/setup.py` & `regipy-3.1.6/setup.py`

 * *Files identical despite different names*

