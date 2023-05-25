# Comparing `tmp/fabric-3.0.1.tar.gz` & `tmp/fabric-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp3qw33273/dist/fabric-3.0.1.tar", last modified: Sat Apr 29 18:59:33 2023, max compression
+gzip compressed data, was "/tmp/tmphwn625pb/dist/fabric-3.1.0.tar", last modified: Thu May 25 18:13:20 2023, max compression
```

## Comparing `fabric-3.0.1.tar` & `fabric-3.1.0.tar`

### file list

```diff
@@ -1,123 +1,126 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/integration/
--rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric-3.0.1/integration/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric-3.0.1/integration/group.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/integration/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.1/integration/_support/funky-perms.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.1/integration/_support/file.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-01-20 23:13:54.000000 fabric-3.0.1/integration/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-01-20 23:13:54.000000 fabric-3.0.1/integration/concurrency.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-04-29 18:59:33.000000 fabric-3.0.1/PKG-INFO
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/top_level.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     2647 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     4230 2023-04-29 17:40:23.000000 fabric-3.0.1/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2857 2023-01-20 23:13:54.000000 fabric-3.0.1/tasks.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric/
--rw-r--r--   0 jforcier  (1000) users      (100)    44996 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/connection.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric/testing/
--rw-r--r--   0 jforcier  (1000) users      (100)    14911 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/testing/base.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5368 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/testing/fixtures.py
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/testing/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6610 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/tunnels.py
--rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/__main__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6702 2023-04-29 17:52:38.000000 fabric-3.0.1/fabric/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13791 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-29 18:58:51.000000 fabric-3.0.1/fabric/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/group.py
--rw-r--r--   0 jforcier  (1000) users      (100)      287 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-29 18:59:33.000000 fabric-3.0.1/setup.cfg
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/group.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/json_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/json_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/json_conf/fabric.json
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/ssh_config/
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/system.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_multi_recursive.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/both_proxies.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/runtime.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/runtime_identity.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_recursive.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/user.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_multi.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/overridden_hostname.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/prompting.py
--rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/runtime_fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/config.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/yml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/yml_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/yml_conf/fabric.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/yaml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/yaml_conf/fabric.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/yaml_conf/fabfile.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/py_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/py_conf/fabric.py
--rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/py_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2047 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1083 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1189 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)    59747 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7306 2023-04-29 17:52:38.000000 fabric-3.0.1/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13902 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric-3.0.1/MANIFEST.in
--rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric-3.0.1/README.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      417 2023-04-28 15:33:01.000000 fabric-3.0.1/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/_shared_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/_shared_static/logo.png
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric-3.0.1/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    15513 2023-04-29 18:58:49.000000 fabric-3.0.1/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/troubleshooting.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/www/upgrading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/installing-1.x.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/roadmap.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/www/changelog-v1.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/shared_conf.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5010 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/cli.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    15384 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/docs/getting-started.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/group.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/connection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/tunnels.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/transfer.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/concepts/networking.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     4078 2023-04-29 17:40:23.000000 fabric-3.0.1/sites/docs/concepts/authentication.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10159 2023-04-29 17:40:23.000000 fabric-3.0.1/sites/docs/concepts/configuration.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/upgrading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric-3.0.1/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric-3.1.0/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric-3.1.0/LICENSE
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)    15384 2023-05-12 17:44:52.000000 fabric-3.1.0/sites/docs/getting-started.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/upgrading.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/tunnels.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/transfer.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2023-05-25 18:06:31.000000 fabric-3.1.0/sites/docs/api/auth.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/connection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/group.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     5223 2023-05-25 18:06:31.000000 fabric-3.1.0/sites/docs/cli.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-05-12 17:44:52.000000 fabric-3.1.0/sites/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/docs/concepts/networking.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     4078 2023-05-11 20:34:05.000000 fabric-3.1.0/sites/docs/concepts/authentication.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10676 2023-05-25 18:06:31.000000 fabric-3.1.0/sites/docs/concepts/configuration.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/www/installing-1.x.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric-3.1.0/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-05-12 17:44:52.000000 fabric-3.1.0/sites/www/upgrading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/www/troubleshooting.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric-3.1.0/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-05-12 17:44:52.000000 fabric-3.1.0/sites/www/changelog-v1.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric-3.1.0/sites/www/installing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    17277 2023-05-25 18:13:19.000000 fabric-3.1.0/sites/www/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric-3.1.0/sites/www/roadmap.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric-3.1.0/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric-3.1.0/sites/www/index.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/sites/_shared_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric-3.1.0/sites/_shared_static/logo.png
+-rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-05-12 17:44:52.000000 fabric-3.1.0/sites/shared_conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6702 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric-3.1.0/fabric/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    45993 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7979 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-05-09 23:14:26.000000 fabric-3.1.0/fabric/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/tunnels.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14381 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     9086 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/auth.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric-3.1.0/fabric/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      540 2023-05-25 18:06:31.000000 fabric-3.1.0/fabric/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/group.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric/testing/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5368 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/testing/fixtures.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric-3.1.0/fabric/testing/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14911 2023-05-12 17:44:52.000000 fabric-3.1.0/fabric/testing/base.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric-3.1.0/fabric/exceptions.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2700 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2023-05-25 18:13:20.000000 fabric-3.1.0/fabric.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)      549 2023-05-25 18:06:31.000000 fabric-3.1.0/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    59810 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    10450 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/auth.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14899 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7306 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1197 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2114 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/_util.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/config.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/prompting.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/runtime_fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/json_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/json_conf/fabric.json
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/json_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/yml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/yml_conf/fabric.yml
+-rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/yml_conf/fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/py_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/py_conf/fabric.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/py_conf/fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/ssh_config/
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/user.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/system.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/proxyjump.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/both_proxies.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/runtime_identity.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/overridden_hostname.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/proxyjump_multi.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/runtime.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/proxyjump_multi_recursive.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/ssh_config/proxyjump_recursive.conf
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/tests/_support/yaml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric-3.1.0/tests/_support/yaml_conf/fabric.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.1.0/tests/_support/yaml_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-05-12 17:44:52.000000 fabric-3.1.0/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1301 2023-05-25 18:06:31.000000 fabric-3.1.0/tests/init.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-05-25 18:13:20.000000 fabric-3.1.0/setup.cfg
+-rw-r--r--   0 jforcier  (1000) users      (100)     4246 2023-05-25 00:37:09.000000 fabric-3.1.0/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric-3.1.0/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2889 2023-05-25 18:12:55.000000 fabric-3.1.0/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-05-25 18:13:20.000000 fabric-3.1.0/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/integration/
+-rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-05-12 17:44:52.000000 fabric-3.1.0/integration/connection.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-05-25 18:13:20.000000 fabric-3.1.0/integration/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.1.0/integration/_support/funky-perms.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.1.0/integration/_support/file.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric-3.1.0/integration/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric-3.1.0/integration/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-05-12 17:44:52.000000 fabric-3.1.0/integration/concurrency.py
```

### Comparing `fabric-3.0.1/integration/transfer.py` & `fabric-3.1.0/integration/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/integration/group.py` & `fabric-3.1.0/integration/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/integration/connection.py` & `fabric-3.1.0/integration/connection.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/integration/concurrency.py` & `fabric-3.1.0/integration/concurrency.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/PKG-INFO` & `fabric-3.1.0/fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric
-Version: 3.0.1
+Version: 3.1.0
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
```

### Comparing `fabric-3.0.1/fabric.egg-info/SOURCES.txt` & `fabric-3.1.0/fabric.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.rst
 dev-requirements.txt
 setup.py
 tasks.py
 fabric/__init__.py
 fabric/__main__.py
 fabric/_version.py
+fabric/auth.py
 fabric/config.py
 fabric/connection.py
 fabric/exceptions.py
 fabric/executor.py
 fabric/group.py
 fabric/main.py
 fabric/runners.py
@@ -36,14 +37,15 @@
 sites/shared_conf.py
 sites/_shared_static/logo.png
 sites/docs/cli.rst
 sites/docs/conf.py
 sites/docs/getting-started.rst
 sites/docs/index.rst
 sites/docs/upgrading.rst
+sites/docs/api/auth.rst
 sites/docs/api/config.rst
 sites/docs/api/connection.rst
 sites/docs/api/exceptions.rst
 sites/docs/api/executor.rst
 sites/docs/api/group.rst
 sites/docs/api/runners.rst
 sites/docs/api/tasks.rst
@@ -63,14 +65,15 @@
 sites/www/index.rst
 sites/www/installing-1.x.rst
 sites/www/installing.rst
 sites/www/roadmap.rst
 sites/www/troubleshooting.rst
 sites/www/upgrading.rst
 tests/_util.py
+tests/auth.py
 tests/config.py
 tests/conftest.py
 tests/connection.py
 tests/executor.py
 tests/group.py
 tests/init.py
 tests/main.py
```

### Comparing `fabric-3.0.1/fabric.egg-info/PKG-INFO` & `fabric-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric
-Version: 3.0.1
+Version: 3.1.0
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
```

### Comparing `fabric-3.0.1/setup.py` & `fabric-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         "Source": "https://github.com/fabric/fabric",
         "Issues": "https://github.com/fabric/fabric/issues",
         "Changelog": "https://www.fabfile.org/changelog.html",
         "CI": "https://app.circleci.com/pipelines/github/fabric/fabric",
         "Twitter": "https://twitter.com/pyfabric",
     },
     python_requres=">=3.6",
-    install_requires=["invoke>=2.0", "paramiko>=2.4"],
+    install_requires=["invoke>=2.0", "paramiko>=2.4", "decorator>=5"],
     extras_require={
         # For folks who want to use fabric.testing package, eg
         # MockRemote/MockSFTP
         "testing": [],  # no longer (for now?) needs anything special
         # For folks who want to use fabric.testing.fixtures' pytest fixtures
         "pytest": ["pytest>=7"],
     },
```

### Comparing `fabric-3.0.1/tasks.py` & `fabric-3.1.0/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os import getcwd
 import sys
 
 from invocations import ci
-from invocations.checks import blacken
+from invocations import checks
 from invocations.docs import docs, www, sites, watch_docs
 from invocations.pytest import (
     test,
     integration as integration_,
     coverage as coverage_,
 )
 from invocations.packaging import release
@@ -80,15 +80,16 @@
         tester=test,
         additional_testers=[integration],
         codecov=codecov,
     )
 
 
 ns = Collection(
-    blacken,
+    checks.blacken,  # backwards compat
+    checks,
     ci,
     coverage,
     docs,
     integration,
     release,
     sites,
     test,
@@ -98,15 +99,15 @@
 )
 ns.configure(
     {
         "packaging": {
             # NOTE: this is currently for identifying the source directory.
             # Should it get used for actual releasing, needs changing.
             "package": "fabric",
-            "sign": True,
+            "sign": False,
             "wheel": True,
             "check_desc": True,
             "changelog_file": "sites/www/changelog.rst",
             "rebuild_with_env": dict(PACKAGE_AS_FABRIC2="yes"),
         }
     }
 )
```

### Comparing `fabric-3.0.1/fabric/connection.py` & `fabric-3.1.0/fabric/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from contextlib import contextmanager
 from io import StringIO
 from threading import Event
 import socket
 
-try:
-    from invoke.vendor.decorator import decorator
-except ImportError:
-    from decorator import decorator
-
+from decorator import decorator
 from invoke import Context
 from invoke.exceptions import ThreadException
 from paramiko.agent import AgentRequestHandler
 from paramiko.client import SSHClient, AutoAddPolicy
 from paramiko.config import SSHConfig
 from paramiko.proxy import ProxyCommand
 
@@ -459,15 +455,15 @@
 
         #: The `paramiko.client.SSHClient` instance this connection wraps.
         client = SSHClient()
         client.set_missing_host_key_policy(AutoAddPolicy())
         self.client = client
 
         #: A convenience handle onto the return value of
-        #: ``self.client.get_transport()``.
+        #: ``self.client.get_transport()`` (after connection time).
         self.transport = None
 
         if inline_ssh_env is None:
             inline_ssh_env = self.config.inline_ssh_env
         #: Whether to construct remote command lines with env vars prefixed
         #: inline.
         self.inline_ssh_env = inline_ssh_env
@@ -600,15 +596,22 @@
         Also saves a handle to the now-set Transport object for easier access.
 
         Various connect-time settings (and/or their corresponding :ref:`SSH
         config options <ssh-config>`) are utilized here in the call to
         `SSHClient.connect <paramiko.client.SSHClient.connect>`. (For details,
         see :doc:`the configuration docs </concepts/configuration>`.)
 
+        :returns:
+            The result of the internal call to `.SSHClient.connect`, if
+            performing an initial connection; ``None`` otherwise.
+
         .. versionadded:: 2.0
+        .. versionchanged:: 3.1
+            Now returns the inner Paramiko connect call's return value instead
+            of always returning the implicit ``None``.
         """
         # Short-circuit
         if self.is_connected:
             return
         err = "Refusing to be ambiguous: connect() kwarg '{}' was given both via regular arg and via connect_kwargs!"  # noqa
         # These may not be given, period
         for key in """
@@ -634,17 +637,38 @@
         if self.gateway:
             kwargs["sock"] = self.open_gateway()
         if self.connect_timeout:
             kwargs["timeout"] = self.connect_timeout
         # Strip out empty defaults for less noisy debugging
         if "key_filename" in kwargs and not kwargs["key_filename"]:
             del kwargs["key_filename"]
+        auth_strategy_class = self.authentication.strategy_class
+        if auth_strategy_class is not None:
+            # Pop connect_kwargs related to auth to avoid giving Paramiko
+            # conflicting signals.
+            for key in (
+                "allow_agent",
+                "key_filename",
+                "look_for_keys",
+                "passphrase",
+                "password",
+                "pkey",
+                "username",
+            ):
+                kwargs.pop(key, None)
+
+            kwargs["auth_strategy"] = auth_strategy_class(
+                ssh_config=self.ssh_config,
+                fabric_config=self.config,
+                username=self.user,
+            )
         # Actually connect!
-        self.client.connect(**kwargs)
+        result = self.client.connect(**kwargs)
         self.transport = self.client.get_transport()
+        return result
 
     def open_gateway(self):
         """
         Obtain a socket-like object from `gateway`.
 
         :returns:
             A ``direct-tcpip`` `paramiko.channel.Channel`, if `gateway` was a
```

### Comparing `fabric-3.0.1/fabric/testing/base.py` & `fabric-3.1.0/fabric/testing/base.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/testing/fixtures.py` & `fabric-3.1.0/fabric/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/util.py` & `fabric-3.1.0/fabric/util.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/main.py` & `fabric-3.1.0/fabric/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 CLI entrypoint & parser configuration.
 
 Builds on top of Invoke's core functionality for same.
 """
 
 import getpass
+from pathlib import Path
 
-from invoke import Argument, Collection, Program
+from invoke import Argument, Collection, Exit, Program
 from invoke import __version__ as invoke
-from paramiko import __version__ as paramiko
+from paramiko import __version__ as paramiko, Agent
 
 from . import __version__ as fabric
 from . import Config, Executor
 
 
 class Fab(Program):
     def print_version(self):
@@ -30,14 +31,19 @@
             Argument(
                 names=("i", "identity"),
                 kind=list,  # Same as OpenSSH, can give >1 key
                 # TODO: automatically add hint about iterable-ness to Invoke
                 # help display machinery?
                 help="Path to runtime SSH identity (key) file. May be given multiple times.",  # noqa
             ),
+            Argument(
+                names=("list-agent-keys",),
+                kind=bool,
+                help="Display ssh-agent key list, and exit.",
+            ),
             # TODO: worth having short flags for these prompt args?
             Argument(
                 names=("prompt-for-login-password",),
                 kind=bool,
                 help="Request an upfront SSH-auth password prompt.",
             ),
             Argument(
@@ -113,22 +119,24 @@
         # NOTE: must do parent before our work, in case users want to disable
         # SSH config loading within a runtime-level conf file/flag.
         super().update_config(merge=False)
         self.config.set_runtime_ssh_path(self.args["ssh-config"].value)
         self.config.load_ssh_config()
         # Load -i identity file, if given, into connect_kwargs, at overrides
         # level.
-        # TODO: this feels a little gross, but since the parent has already
-        # called load_overrides, this is best we can do for now w/o losing
-        # data. Still feels correct; just might be cleaner to have even more
-        # Config API members around this sort of thing. Shrug.
         connect_kwargs = {}
-        path = self.args["identity"].value
-        if path:
-            connect_kwargs["key_filename"] = path
+        paths = self.args["identity"].value
+        if paths:
+            connect_kwargs["key_filename"] = paths
+            # New, non-sshclient based config location
+            # Also new: Path! (which we couldn't use above until paramiko knew
+            # about it)
+            self.config._overrides["authentication"] = dict(
+                identities=[Path(x) for x in paths]
+            )
         # Ditto for connect timeout
         timeout = self.args["connect-timeout"].value
         if timeout:
             connect_kwargs["timeout"] = timeout
         # Secrets prompts that want to happen at handoff time instead of
         # later/at user-time.
         # TODO: should this become part of Invoke proper in case other
@@ -136,19 +144,45 @@
         # already doing a similar thing there for sudo password...
         if self.args["prompt-for-login-password"].value:
             prompt = "Enter login password for use with SSH auth: "
             connect_kwargs["password"] = getpass.getpass(prompt)
         if self.args["prompt-for-passphrase"].value:
             prompt = "Enter passphrase for use unlocking SSH keys: "
             connect_kwargs["passphrase"] = getpass.getpass(prompt)
+        # TODO: this (directly manipulating _overrides) feels a little gross,
+        # but since the parent has already called load_overrides, this is best
+        # we can do for now w/o losing data. Still feels correct; just might be
+        # cleaner to have even more Config API members around this sort of
+        # thing. Shrug.
         self.config._overrides["connect_kwargs"] = connect_kwargs
         # Since we gave merge=False above, we must do it ourselves here. (Also
         # allows us to 'compile' our overrides manipulation.)
         self.config.merge()
 
+    # TODO: make this an explicit hookpoint in Invoke, i.e. some default-noop
+    # method called at the end of parse_core() that we can override here
+    # instead of doing this.
+    def parse_core(self, *args, **kwargs):
+        super().parse_core(*args, **kwargs)
+        if self.args["list-agent-keys"].value:
+            keys = Agent().get_keys()
+            for key in keys:
+                tpl = "{} {} {} ({})"
+                # TODO: _could_ use new PKey.__repr__ but I like the mimicry of
+                # OpenSSH ssh-add -l for now...
+                print(
+                    tpl.format(
+                        key.get_bits(),
+                        key.fingerprint,
+                        key.comment,
+                        key.algorithm_name,
+                    )
+                )
+            raise Exit
+
 
 # Mostly a concession to testing.
 def make_program():
     return Fab(
         name="Fabric",
         version=fabric,
         executor_class=Executor,
```

### Comparing `fabric-3.0.1/fabric/transfer.py` & `fabric-3.1.0/fabric/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/tunnels.py` & `fabric-3.1.0/fabric/tunnels.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/runners.py` & `fabric-3.1.0/fabric/runners.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/exceptions.py` & `fabric-3.1.0/fabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/config.py` & `fabric-3.1.0/fabric/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,29 +283,40 @@
         documentation for the base values, such as the config subtrees
         controlling behavior of ``run`` or how ``tasks`` behave.
 
         For Fabric-specific modifications and additions to the Invoke-level
         defaults, see our own config docs at :ref:`default-values`.
 
         .. versionadded:: 2.0
+        .. versionchanged:: 3.1
+            Added the ``authentication`` settings section, plus sub-attributes
+            such as ``authentication.strategy_class``.
         """
         # TODO: hrm should the run-related things actually be derived from the
         # runner_class? E.g. Local defines local stuff, Remote defines remote
         # stuff? Doesn't help with the final config tree tho...
         # TODO: as to that, this is a core problem, Fabric wants split
         # local/remote stuff, eg replace_env wants to be False for local and
         # True remotely; shell wants to differ depending on target (and either
         # way, does not want to use local interrogation for remote)
         # TODO: is it worth moving all of our 'new' settings to a discrete
         # namespace for cleanliness' sake? e.g. ssh.port, ssh.user etc.
         # It wouldn't actually simplify this code any, but it would make it
         # easier for users to determine what came from which library/repo.
         defaults = InvokeConfig.global_defaults()
+        # TODO 4.0: this is already a mess, strongly consider a new 'ssh'
+        # subtree because otherwise it's guessing where, or whether, 'ssh' is
+        # in the setting name! i.e. 'inline_ssh_env' -> ssh.use_inline_env,
+        # 'load_ssh_configs' -> ssh.load_configs, 'ssh_config_path' ->
+        # ssh.config_path, etc
         ours = {
-            # New settings
+            "authentication": {
+                "identities": [],
+                "strategy_class": None,
+            },
             "connect_kwargs": {},
             "forward_agent": False,
             "gateway": None,
             "inline_ssh_env": True,
             "load_ssh_configs": True,
             "port": 22,
             "runners": {"remote": Remote, "remote_shell": RemoteShell},
```

### Comparing `fabric-3.0.1/fabric/tasks.py` & `fabric-3.1.0/fabric/tasks.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/executor.py` & `fabric-3.1.0/fabric/executor.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/fabric/group.py` & `fabric-3.1.0/fabric/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/group.py` & `fabric-3.1.0/tests/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/_support/fabfile.py` & `fabric-3.1.0/tests/_support/fabfile.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/_util.py` & `fabric-3.1.0/tests/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     elif test == "contains":
         assert out in output
     elif test == "regex":
         assert re.match(out, output)
     else:
         err = "Don't know how to expect that <stdout> {} <expected>!"
         assert False, err.format(test)
+    # Safety check: no stderr
+    assert not sys.stderr.getvalue()
 
 
 def faux_v1_env():
     # Close enough to v1 _AttributeDict...
     # Contains a copy of enough of v1's defaults to prevent us having to do a
     # lot of extra .get()s...meh
     return Lexicon(
```

### Comparing `fabric-3.0.1/tests/config.py` & `fabric-3.1.0/tests/config.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/executor.py` & `fabric-3.1.0/tests/executor.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/conftest.py` & `fabric-3.1.0/tests/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # flake8: noqa
-from fabric.testing.fixtures import client, remote, sftp, sftp_objs, transfer
-
 from os.path import isfile, expanduser
+from unittest.mock import patch
 
 from pytest import fixture
 
-from unittest.mock import patch
+# Set up icecream globally for convenience.
+from icecream import install as install_icecream
+
+from fabric.testing.fixtures import client, remote, sftp, sftp_objs, transfer
+
+
+install_icecream()
 
 
 # TODO: does this want to end up in the public fixtures module too?
 @fixture(autouse=True)
 def no_user_ssh_config():
     """
     Cowardly refuse to ever load what looks like user SSH config paths.
```

### Comparing `fabric-3.0.1/tests/init.py` & `fabric-3.1.0/tests/init.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import fabric
-from fabric import _version, connection, runners, group, tasks, executor
+from fabric import _version, connection, runners, group, tasks, executor, auth
 
 
 class init:
     "__init__"
 
     def version_and_version_info(self):
         for name in ("__version_info__", "__version__"):
@@ -40,7 +40,10 @@
         assert fabric.task is tasks.task
 
     def Task(self):
         assert fabric.Task is tasks.Task
 
     def Executor(self):
         assert fabric.Executor is executor.Executor
+
+    def OpenSSHAuthStrategy(self):
+        assert fabric.OpenSSHAuthStrategy is auth.OpenSSHAuthStrategy
```

### Comparing `fabric-3.0.1/tests/connection.py` & `fabric-3.1.0/tests/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,16 +647,17 @@
             assert Connection("a-host", user="a-user") < Connection(
                 "a-host", user="b-user"
             )
             # then port...
             assert Connection("a-host", port=1) < Connection("a-host", port=2)
 
     class open:
-        def has_no_required_args_and_returns_None(self, client):
-            assert Connection("host").open() is None
+        def has_no_required_args_and_returns_value_of_connect(self, client):
+            retval = Connection("host").open()
+            assert retval is client.connect.return_value
 
         def calls_SSHClient_connect(self, client):
             "calls paramiko.SSHClient.connect() with correct args"
             Connection("host").open()
             client.connect.assert_called_with(
                 username=get_local_user(), hostname="host", port=22
             )
```

### Comparing `fabric-3.0.1/tests/runners.py` & `fabric-3.1.0/tests/runners.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/transfer.py` & `fabric-3.1.0/tests/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/util.py` & `fabric-3.1.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/tests/main.py` & `fabric-3.1.0/tests/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import os
 import sys
 import re
 
 from invoke import run
 from invoke.util import cd
 from unittest.mock import patch
+from paramiko.agent import AgentKey, Message
 import pytest  # because WHY would you expose @skip normally? -_-
 from pytest_relaxed import raises
 
 from fabric.config import Config
 from fabric.main import make_program
 from fabric.exceptions import NothingToDo
 
@@ -50,14 +51,38 @@
         def exposes_hosts_flag_in_help(self):
             expect("--help", "-H STRING, --hosts=STRING", test="contains")
 
         def executes_remainder_as_anonymous_task(self, remote):
             remote.expect(host="myhost", cmd="whoami")
             make_program().run("fab -H myhost -- whoami", exit=False)
 
+        @patch("paramiko.agent.Agent.get_keys")
+        def can_list_agent_keys(self, get_keys):
+            agent_keys = []
+            for type_, bits, comment in (
+                ("ecdsa", b"dummy", "woody"),
+                ("rsa", b"ventriloquist", "bob"),
+                ("ed25519", b"stagehand", "smith"),
+            ):
+                # Looks like a pubkey blob from an agent
+                m = Message()
+                m.add_string(type_)
+                m.add_string(bits)
+                agent_keys.append(
+                    AgentKey(agent=None, blob=bytes(m), comment=comment)
+                )
+
+            get_keys.return_value = agent_keys
+            expected = """
+0 SHA256:r7SOU1pAlEWmRE57Swf0OQHg9tlYicKaLx2DxGbDVk8 woody (ECDSA)
+0 SHA256:2qZYGN+eIVfmhwpQUMje7uG4+7tZquM5LBwNaHCBsqg bob (RSA)
+0 SHA256:4seJT+aN1aTPIudGupnXsZ1z20r+GCIAAKEA4MHnwvA smith (ED25519)
+""".lstrip()
+            expect("--list-agent-keys", expected)
+
         def uses_FABRIC_env_prefix(self, environ):
             environ["FABRIC_RUN_ECHO"] = "1"
             with cd(support):
                 make_program().run("fab expect-from-env")
 
         def basic_pre_and_post_tasks_still_work(self):
             with cd(support):
```

### Comparing `fabric-3.0.1/tests/task.py` & `fabric-3.1.0/tests/task.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/README.rst` & `fabric-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/_shared_static/logo.png` & `fabric-3.1.0/sites/_shared_static/logo.png`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/conf.py` & `fabric-3.1.0/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/faq.rst` & `fabric-3.1.0/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/installing.rst` & `fabric-3.1.0/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/changelog.rst` & `fabric-3.1.0/sites/www/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,56 @@
 Changelog
 =========
 
 .. note::
     Looking for the Fabric 1.x changelog? See :doc:`/changelog-v1`.
 
 .. warning::
-    Keep in mind that Fabric is largely a thin wrapper around `Paramiko
+    Keep in mind that Fabric is largely a wrapper around `Paramiko
     <https://paramiko.org/changelog.html>`_  and `Invoke
-    <https://pyinvoke.org/changelog.html>`_ - just because Fabric itself hasn't
-    had a release in a while doesn't mean its capabilities aren't improving!
-    Click those projects' names in this paragraph to visit their changelogs and
-    see what you might get if you upgrade your dependencies.
+    <https://pyinvoke.org/changelog.html>`_ - Fabric's capabilities can often
+    improve simply by upgrading your copies of those libraries! Click their
+    names in this paragraph to visit their changelogs and see what you might get
+    if you upgrade your dependencies.
 
+- :release:`3.1.0 <2023-05-25>`
+- :feature:`-` Implement opt-in support for Paramiko 3.2's
+  `~paramiko.auth_strategy.AuthStrategy` machinery, as follows:
+
+  - Added a new module and class, `fabric.auth.OpenSSHAuthStrategy`, which
+    leverages aforementioned new Paramiko functionality to marry loaded SSH
+    config files with Fabric-level and runtime-level parameters, arriving at
+    what should be OpenSSH-client-compatible authentication behavior. See its
+    API docs for details.
+  - Added new :ref:`configuration settings <fab-configuration>`:
+
+    - ``authentication.strategy_class``, which defaults to ``None``, but can be
+      set to ``OpenSSHAuthStrategy`` to opt-in to the new behavior.
+    - ``authentication.identities``, which defaults to the empty list, and can
+      be a list of private key paths for use by the new strategy class.
+
+  .. warning::
+    This feature is **EXPERIMENTAL**, **incomplete**, and subject to change!
+
+    (For example, it lacks passphrase support, and doesn't implement 100% of
+    all auth sources yet, focusing mostly on private keys and
+    interactive-password.)
+
+- :feature:`-` Add a new CLI flag to ``fab``, ``fab --list-agent-keys``, which
+  will attempt to connect to your local SSH agent and print a key list,
+  similarly to ``ssh-add -l``. This is mostly useful for expectations-checking
+  Fabric and Paramiko's agent functionality, or for situations where you might
+  not have ``ssh-add`` handy.
+
+  .. warning:: This feature requires Paramiko 3.2 or above.
+
+- :bug:`2263 major` Explicitly add our dependency on ``decorator`` to
+  ``setup.py`` instead of using Invoke's old, now removed, vendored copy of
+  same. This allows Fabric to happily use Invoke 2.1 and above. Thanks to Luke
+  Robison, Nick Humrich, and others, for the reports.
 - :release:`3.0.1 <2023-04-29>`
 - :bug:`2241` A typo prevented Fabric's command runner from properly calling
   its superclass ``stop()`` method, which in tandem with a related Invoke bug
   meant messy or long shutdowns in many scenarios. Thanks to Orlando
   Rodríguez for report and initial patch.
 - :release:`3.0.0 <2023-01-20>`
 - :bug:`1981 major` (fixed in :issue:`2195`) Automatically close any open SFTP
```

### Comparing `fabric-3.0.1/sites/www/index.rst` & `fabric-3.1.0/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/contact.rst` & `fabric-3.1.0/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/development.rst` & `fabric-3.1.0/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/troubleshooting.rst` & `fabric-3.1.0/sites/www/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/upgrading.rst` & `fabric-3.1.0/sites/www/upgrading.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/installing-1.x.rst` & `fabric-3.1.0/sites/www/installing-1.x.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/roadmap.rst` & `fabric-3.1.0/sites/www/roadmap.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/www/changelog-v1.rst` & `fabric-3.1.0/sites/www/changelog-v1.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/shared_conf.py` & `fabric-3.1.0/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/index.rst` & `fabric-3.1.0/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/conf.py` & `fabric-3.1.0/sites/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/cli.rst` & `fabric-3.1.0/sites/docs/cli.rst`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     setting (which is read by `.Connection`, and eventually makes its way into
     Paramiko; see the docstring for `.Connection` for details.)
 
     Typically this can be thought of as identical to ``ssh -i <path>``, i.e.
     supplying a specific, runtime private key file. Like ``ssh -i``, it builds
     an iterable of strings and may be given multiple times.
 
+    New in version 3.1: this also ends up in the ``authentication.identities``
+    :doc:`configuration value </concepts/configuration>` and will be referenced
+    by `fabric.auth.OpenSSHAuthStrategy`, if in use.
+
     Default: ``[]``.
 
 .. option:: --prompt-for-login-password
 
     Causes Fabric to prompt 'up front' for a value to store as the
     ``connect_kwargs.password`` config setting (used by Paramiko when
     authenticating via passwords and, in some versions, also used for key
```

### Comparing `fabric-3.0.1/sites/docs/getting-started.rst` & `fabric-3.1.0/sites/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/api/testing.rst` & `fabric-3.1.0/sites/docs/api/testing.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/concepts/networking.rst` & `fabric-3.1.0/sites/docs/concepts/networking.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/concepts/authentication.rst` & `fabric-3.1.0/sites/docs/concepts/authentication.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.1/sites/docs/concepts/configuration.rst` & `fabric-3.1.0/sites/docs/concepts/configuration.rst`

 * *Files 6% similar despite different names*

```diff
@@ -78,19 +78,29 @@
 
 .. warning::
     Many of these are also configurable via :ref:`ssh_config files
     <ssh-config>`. **Such values take precedence over those defined via the
     core configuration**, so make sure you're aware of whether you're loading
     such files (or :ref:`disable them to be sure <disabling-ssh-config>`).
 
+- ``authentication``: Authentication-related options.
+
+    - ``identities``: A list of private key paths (`str` or `pathlib.Path`) to
+      use for authentication. This is filled in by :option:`fab -i <-i>` as
+      well.
+    - ``strategy_class``: If given (defaults to ``None``), must be a subclass
+      of `~paramiko.auth_strategy.AuthStrategy`; when not ``None``, triggers
+      use of this new Paramiko authentication framework. Fabric 3.1 ships with
+      `~fabric.auth.OpenSSHAuthStrategy`; see its API doc entry for how this
+      interacts with things like ``connect_kwargs``.
+
 - ``connect_kwargs``: Keyword arguments (`dict`) given to `SSHClient.connect
   <paramiko.client.SSHClient.connect>` when `.Connection` performs that method
-  call. This is the primary configuration vector for many SSH-related options,
-  such as selecting private keys, toggling forwarding of SSH agents, etc.
-  Default: ``{}``.
+  call. This is often a way of supplying options Fabric has no native setting
+  for. Default: ``{}``.
 - ``forward_agent``: Whether to attempt forwarding of your local SSH
   authentication agent to the remote end. Default: ``False`` (same as in
   OpenSSH.)
 - ``gateway``: Used as the default value of the ``gateway`` kwarg for
   `.Connection`. May be any value accepted by that argument. Default: ``None``.
 - ``load_ssh_configs``: Whether to automatically seek out :ref:`SSH config
   files <ssh-config>`. When ``False``, no automatic loading occurs. Default:
```

### Comparing `fabric-3.0.1/LICENSE` & `fabric-3.1.0/LICENSE`

 * *Files identical despite different names*

