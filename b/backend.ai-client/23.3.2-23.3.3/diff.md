# Comparing `tmp/backend.ai-client-23.3.2.tar.gz` & `tmp/backend.ai-client-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-client-23.3.2.tar", last modified: Fri May  5 07:08:22 2023, max compression
+gzip compressed data, was "backend.ai-client-23.3.3.tar", last modified: Thu May 25 17:30:45 2023, max compression
```

## Comparing `backend.ai-client-23.3.2.tar` & `backend.ai-client-23.3.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.030498 backend.ai-client-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-05 07:08:22.030498 backend.ai-client-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.010497 backend.ai-client-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.010497 backend.ai-client-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.014498 backend.ai-client-23.3.2/ai/backend/client/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.018498 backend.ai-client-23.3.2/ai/backend/client/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.022498 backend.ai-client-23.3.2/ai/backend/client/cli/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/license.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/admin/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/pretty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/cli/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.026498 backend.ai-client-23.3.2/ai/backend/client/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/bgtask.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/server_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/func/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/load_balancing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.030498 backend.ai-client-23.3.2/ai/backend/client/output/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/output/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30097 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/ai/backend/client/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:22.030498 backend.ai-client-23.3.2/backend.ai_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-05 07:08:22.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 07:08:22.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:22.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 07:08:22.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:22.000000 backend.ai-client-23.3.2/backend.ai_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:22.030498 backend.ai-client-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-05 07:08:21.000000 backend.ai-client-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.361149 backend.ai-client-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-25 17:30:45.361149 backend.ai-client-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.337149 backend.ai-client-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.337149 backend.ai-client-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.341149 backend.ai-client-23.3.3/ai/backend/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.349149 backend.ai-client-23.3.3/ai/backend/client/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.353149 backend.ai-client-23.3.3/ai/backend/client/cli/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/admin/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12150 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/pretty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31836 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48183 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27326 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/cli/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.357149 backend.ai-client-23.3.3/ai/backend/client/func/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/bgtask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11666 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/server_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49999 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/func/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/load_balancing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.357149 backend.ai-client-23.3.3/ai/backend/client/output/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/output/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    30097 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/ai/backend/client/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.361149 backend.ai-client-23.3.3/backend.ai_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:45.000000 backend.ai-client-23.3.3/backend.ai_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:45.361149 backend.ai-client-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-25 17:30:44.000000 backend.ai-client-23.3.3/setup.py
```

### Comparing `backend.ai-client-23.3.2/PKG-INFO` & `backend.ai-client-23.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/x-rst
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-23.3.2/ai/backend/client/auth.py` & `backend.ai-client-23.3.3/ai/backend/client/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/__init__.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/acl.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/agent.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/domain.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/etcd.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/group.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/image.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/keypair.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/license.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/license.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/manager.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/resource.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/resource_policy.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/scaling_group.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/session.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/storage.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/user.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/admin/vfolder.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/admin/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/announcement.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/announcement.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/app.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/app.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/config.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -192,7 +192,32 @@
 
     with Session() as session:
         try:
             session.Auth.update_password(old_password, new_password, new_password2)
             print_done("Password updated.")
         except Exception as e:
             print_error(e)
+
+
+@main.command()
+@click.argument("domain", metavar="USER_ID")
+@click.argument("user_id", metavar="USER_ID")
+@click.argument("current_password", metavar="CURRENT_PASSWORD")
+@click.argument("new_password", metavar="NEW_PASSWORD")
+def update_password_no_auth(domain, user_id, current_password, new_password):
+    """
+    Update user's password. This is used to update `EXPIRED` password only.
+    """
+    with Session() as session:
+        try:
+            config = get_config()
+            if config.endpoint_type == "session":
+                session.Auth.update_password_no_auth_in_session(
+                    user_id, current_password, new_password
+                )
+            else:
+                session.Auth.update_password_no_auth(
+                    domain, user_id, current_password, new_password
+                )
+            print_done("Password updated.")
+        except Exception as e:
+            print_error(e)
```

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/dotfile.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/extensions.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/logs.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/main.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/model.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/pagination.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/params.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/params.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/pretty.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/pretty.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/proxy.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/proxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/run.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/run.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/server_log.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/service.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/session.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/session_template.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/ssh.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/ssh.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/cli/vfolder.py` & `backend.ai-client-23.3.3/ai/backend/client/cli/vfolder.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,20 @@
     default=None,
     help=(
         "The local parent directory which contains the file to be uploaded. "
         "[default: current working directory]"
     ),
 )
 @click.option(
+    "-r",
+    "--recursive",
+    is_flag=True,
+    help="Upload the given directory recursively.",
+)
+@click.option(
     "--chunk-size",
     type=ByteSizeParamType(),
     default=humanize.naturalsize(DEFAULT_CHUNK_SIZE, binary=True, gnu=True),
     help=(
         'Transfer the file with the given chunk size with binary suffixes (e.g., "16m"). '
         "Set this between 8 to 64 megabytes for high-speed disks (e.g., SSD RAID) "
         "and networks (e.g., 40 GbE) for the maximum throughput."
@@ -252,28 +258,29 @@
     help=(
         "Overrides storage proxy address. "
         'The value must shape like "X1=Y1,X2=Y2...". '
         "Each Yn address must at least include the IP address "
         "or the hostname and may include the protocol part and the port number to replace."
     ),
 )
-def upload(name, filenames, base_dir, chunk_size, override_storage_proxy):
+def upload(name, filenames, base_dir, recursive, chunk_size, override_storage_proxy):
     """
     TUS Upload a file to the virtual folder from the current working directory.
     The files with the same names will be overwritten.
 
     \b
     NAME: Name of a virtual folder.
     FILENAMES: Paths of the files to be uploaded.
     """
     with Session() as session:
         try:
             session.VFolder(name).upload(
                 filenames,
                 basedir=base_dir,
+                recursive=recursive,
                 chunk_size=chunk_size,
                 show_progress=True,
                 address_map=override_storage_proxy
                 or APIConfig.DEFAULTS["storage_proxy_address_map"],
             )
             print_done("Done.")
         except Exception as e:
```

### Comparing `backend.ai-client-23.3.2/ai/backend/client/compat.py` & `backend.ai-client-23.3.3/ai/backend/client/compat.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/config.py` & `backend.ai-client-23.3.3/ai/backend/client/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/exceptions.py` & `backend.ai-client-23.3.3/ai/backend/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/acl.py` & `backend.ai-client-23.3.3/ai/backend/client/func/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/admin.py` & `backend.ai-client-23.3.3/ai/backend/client/func/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/agent.py` & `backend.ai-client-23.3.3/ai/backend/client/func/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/auth.py` & `backend.ai-client-23.3.3/ai/backend/client/func/auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -61,7 +61,50 @@
                 "old_password": old_password,
                 "new_password": new_password,
                 "new_password2": new_password2,
             }
         )
         async with rqst.fetch() as resp:
             return await resp.json()
+
+    @api_function
+    @classmethod
+    async def update_password_no_auth(
+        cls, domain: str, user_id: str, current_password: str, new_password: str
+    ) -> dict:
+        """
+        Update user's password. This is used to update `EXPIRED` password only.
+        This function fetch a request to manager.
+        """
+
+        rqst = Request("POST", "/auth/update-password-no-auth")
+        rqst.set_json(
+            {
+                "domain": domain,
+                "username": user_id,
+                "current_password": current_password,
+                "new_password": new_password,
+            }
+        )
+        async with rqst.fetch(anonymous=True) as resp:
+            return await resp.json()
+
+    @api_function
+    @classmethod
+    async def update_password_no_auth_in_session(
+        cls, user_id: str, current_password: str, new_password: str
+    ) -> dict:
+        """
+        Update user's password. This is used to update `EXPIRED` password only.
+        This function fetch a request to webserver.
+        """
+
+        rqst = Request("POST", "/server/update-password-no-auth")
+        rqst.set_json(
+            {
+                "username": user_id,
+                "current_password": current_password,
+                "new_password": new_password,
+            }
+        )
+        async with rqst.fetch(anonymous=True) as resp:
+            return await resp.json()
```

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/base.py` & `backend.ai-client-23.3.3/ai/backend/client/func/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/bgtask.py` & `backend.ai-client-23.3.3/ai/backend/client/func/bgtask.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/domain.py` & `backend.ai-client-23.3.3/ai/backend/client/func/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/dotfile.py` & `backend.ai-client-23.3.3/ai/backend/client/func/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/etcd.py` & `backend.ai-client-23.3.3/ai/backend/client/func/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/group.py` & `backend.ai-client-23.3.3/ai/backend/client/func/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/image.py` & `backend.ai-client-23.3.3/ai/backend/client/func/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/keypair.py` & `backend.ai-client-23.3.3/ai/backend/client/func/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/keypair_resource_policy.py` & `backend.ai-client-23.3.3/ai/backend/client/func/keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/manager.py` & `backend.ai-client-23.3.3/ai/backend/client/func/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/model.py` & `backend.ai-client-23.3.3/ai/backend/client/func/model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/resource.py` & `backend.ai-client-23.3.3/ai/backend/client/func/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/scaling_group.py` & `backend.ai-client-23.3.3/ai/backend/client/func/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/server_log.py` & `backend.ai-client-23.3.3/ai/backend/client/func/server_log.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/service.py` & `backend.ai-client-23.3.3/ai/backend/client/func/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/session.py` & `backend.ai-client-23.3.3/ai/backend/client/func/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/session_template.py` & `backend.ai-client-23.3.3/ai/backend/client/func/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/storage.py` & `backend.ai-client-23.3.3/ai/backend/client/func/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/system.py` & `backend.ai-client-23.3.3/ai/backend/client/func/system.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/user.py` & `backend.ai-client-23.3.3/ai/backend/client/func/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/func/vfolder.py` & `backend.ai-client-23.3.3/ai/backend/client/func/vfolder.py`

 * *Files 6% similar despite different names*

```diff
@@ -313,31 +313,28 @@
                 if dst_dir is not None:
                     params["dst_dir"] = dst_dir
                 download_url = URL(overriden_url).with_query(params)
             await self._download_file(
                 file_path, download_url, chunk_size, max_retries, show_progress
             )
 
-    @api_function
-    async def upload(
+    async def _upload_files(
         self,
-        files: Sequence[Union[str, Path]],
-        *,
+        file_paths: Sequence[Path],
         basedir: Union[str, Path] = None,
         dst_dir: Union[str, Path] = None,
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         address_map: Optional[Mapping[str, str]] = None,
-        show_progress: bool = False,
     ) -> None:
         base_path = Path.cwd() if basedir is None else Path(basedir).resolve()
-        if basedir:
-            files = [basedir / Path(file) for file in files]
-        else:
-            files = [Path(file).resolve() for file in files]
-        for file_path in files:
+        for file_path in file_paths:
+            if file_path.is_dir():
+                raise BackendClientError(
+                    f"Failed to upload {file_path}. Use recursive option to upload directories."
+                )
             file_size = Path(file_path).stat().st_size
             rqst = Request("POST", "/folders/{}/request-upload".format(self.name))
             rqst.set_json(
                 {
                     "path": "{}".format(str(Path(file_path).relative_to(base_path))),
                     "size": int(file_size),
                 }
@@ -370,35 +367,86 @@
                 file_stream=input_file,
                 url=upload_url,
                 upload_checksum=False,
                 chunk_size=chunk_size,
             )
             await uploader.upload()
             input_file.close()
-        return None
+
+    async def _upload_recursively(
+        self,
+        source: Sequence[Path],
+        basedir: Union[str, Path] = None,
+        dst_dir: Union[str, Path] = None,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        address_map: Optional[Mapping[str, str]] = None,
+    ) -> None:
+        dir_list: list[Path] = []
+        file_list: list[Path] = []
+        base_path = Path.cwd() if basedir is None else Path(basedir).resolve()
+        for path in source:
+            if path.is_file():
+                file_list.append(path)
+            else:
+                await self._mkdir(path.relative_to(base_path))
+                dir_list.append(path)
+        await self._upload_files(file_list, basedir, dst_dir, chunk_size, address_map)
+        for dir in dir_list:
+            await self._upload_recursively(
+                list(dir.glob("*")), basedir, dst_dir, chunk_size, address_map
+            )
 
     @api_function
-    async def mkdir(
+    async def upload(
+        self,
+        sources: Sequence[Union[str, Path]],
+        *,
+        basedir: Union[str, Path] = None,
+        recursive: bool = False,
+        dst_dir: Union[str, Path] = None,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        address_map: Optional[Mapping[str, str]] = None,
+        show_progress: bool = False,
+    ) -> None:
+        if basedir:
+            src_paths = [basedir / Path(src) for src in sources]
+        else:
+            src_paths = [Path(src).resolve() for src in sources]
+        if recursive:
+            await self._upload_recursively(src_paths, basedir, dst_dir, chunk_size, address_map)
+        else:
+            await self._upload_files(src_paths, basedir, dst_dir, chunk_size, address_map)
+
+    async def _mkdir(
         self,
         path: Union[str, Path],
         parents: Optional[bool] = False,
         exist_ok: Optional[bool] = False,
-    ):
+    ) -> str:
         rqst = Request("POST", "/folders/{}/mkdir".format(self.name))
         rqst.set_json(
             {
                 "path": path,
                 "parents": parents,
                 "exist_ok": exist_ok,
             }
         )
         async with rqst.fetch() as resp:
             return await resp.text()
 
     @api_function
+    async def mkdir(
+        self,
+        path: Union[str, Path],
+        parents: Optional[bool] = False,
+        exist_ok: Optional[bool] = False,
+    ) -> str:
+        return await self._mkdir(path, parents, exist_ok)
+
+    @api_function
     async def rename_file(self, target_path: str, new_name: str):
         rqst = Request("POST", "/folders/{}/rename-file".format(self.name))
         rqst.set_json(
             {
                 "target_path": target_path,
                 "new_name": new_name,
             }
```

### Comparing `backend.ai-client-23.3.2/ai/backend/client/load_balancing.py` & `backend.ai-client-23.3.3/ai/backend/client/load_balancing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/__init__.py` & `backend.ai-client-23.3.3/ai/backend/client/output/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/console.py` & `backend.ai-client-23.3.3/ai/backend/client/output/console.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/fields.py` & `backend.ai-client-23.3.3/ai/backend/client/output/fields.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/formatters.py` & `backend.ai-client-23.3.3/ai/backend/client/output/formatters.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/json.py` & `backend.ai-client-23.3.3/ai/backend/client/output/json.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/output/types.py` & `backend.ai-client-23.3.3/ai/backend/client/output/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/pagination.py` & `backend.ai-client-23.3.3/ai/backend/client/pagination.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/request.py` & `backend.ai-client-23.3.3/ai/backend/client/request.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/session.py` & `backend.ai-client-23.3.3/ai/backend/client/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/utils.py` & `backend.ai-client-23.3.3/ai/backend/client/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/ai/backend/client/versioning.py` & `backend.ai-client-23.3.3/ai/backend/client/versioning.py`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/backend.ai_client.egg-info/PKG-INFO` & `backend.ai-client-23.3.3/backend.ai_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-client
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Client SDK
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/x-rst
 
 Backend.AI Client
 =================
```

### Comparing `backend.ai-client-23.3.2/backend.ai_client.egg-info/SOURCES.txt` & `backend.ai-client-23.3.3/backend.ai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-client-23.3.2/backend_shim.py` & `backend.ai-client-23.3.3/backend_shim.py`

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

### Comparing `backend.ai-client-23.3.2/setup.py` & `backend.ai-client-23.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,33 +12,34 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 5 - Production/Stable',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Client SDK',
     'entry_points': {
         'backendai_cli_v10': [
             '_ = ai.backend.client.cli.main:main',
         ],
     },
     'install_requires': (
         'aiohttp~=3.8.1',
         'aiotusclient~=0.1.4',
         'appdirs~=1.4.4',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.2
+        """backend.ai-cli==23.03.3
 """,
-        """backend.ai-common==23.03.2
+        """backend.ai-common==23.03.3
 """,
-        """backend.ai-plugin==23.03.2
+        """backend.ai-plugin==23.03.3
 """,
         'click>=7.1.2',
         'faker~=13.12.0',
         'humanize>=3.1.0',
         'inquirer~=2.9.2',
         'janus~=1.0.0',
         'multidict>=6.0',
@@ -278,11 +279,11 @@
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

