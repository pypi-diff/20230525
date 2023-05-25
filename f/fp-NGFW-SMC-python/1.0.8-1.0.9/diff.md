# Comparing `tmp/fp-NGFW-SMC-python-1.0.8.tar.gz` & `tmp/fp-NGFW-SMC-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp-NGFW-SMC-python-1.0.8.tar", last modified: Thu Aug 19 16:24:44 2021, max compression
+gzip compressed data, was "dist/fp-NGFW-SMC-python-1.0.9.tar", last modified: Thu Sep 16 16:10:18 2021, max compression
```

## Comparing `fp-NGFW-SMC-python-1.0.8.tar` & `fp-NGFW-SMC-python-1.0.9.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/actions/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/actions/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1530 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/compat.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/vpn/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    23611 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/vpn/route.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    31166 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/vpn/elements.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18296 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/vpn/policy.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/vpn/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/api/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7760 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/configloader.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9734 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/exceptions.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10080 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/web.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1638 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/entry_point.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4996 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/common.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    31469 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/api/session.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/api/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/base/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4834 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/structs.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3713 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/decorators.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    30755 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/collection.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    35044 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/model.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1991 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/mixins.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/base/util.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/base/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    36208 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/rule.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      236 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/qos.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5565 2021-07-29 15:34:35.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/ips.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    28311 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/rule_nat.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1258 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/file_filtering.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7991 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/layer3.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7403 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/policy.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    33260 2021-06-24 16:53:58.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/rule_elements.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5677 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/layer2.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3564 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/policy/interface.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15218 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/situations.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9206 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/profiles.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    33025 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/servers.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    16968 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/other.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10685 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/group.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    19748 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/protocols.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    22308 2021-05-27 19:10:46.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/netlink.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    24307 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/network.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2784 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/helpers.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10646 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/service.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     8525 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/user.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       13 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/elements/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    21126 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/ospf.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6289 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/bgp_access_list.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15892 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/route_map.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7514 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/access_list.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    24490 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/bgp.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3904 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/prefix_list.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/routing/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1788 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/license.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    12818 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/servers.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10238 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/users.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7688 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/reports.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    13409 2021-07-29 15:34:35.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/system.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9553 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/tasks.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4791 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/role.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5412 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/access_rights.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3361 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/vpn.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6454 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/tls_common.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    27909 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/tls.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    28326 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/scheduled_tasks.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3774 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/administration/updates.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/smc/core/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    41302 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/route.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7706 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/core/waiters.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9335 2021-06-24 16:53:58.000000 fp-NGFW-SMC-python-1.0.8/smc/core/contact_address.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    58534 2021-05-27 19:10:46.000000 fp-NGFW-SMC-python-1.0.8/smc/core/engine.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5588 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/resource.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      285 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/hardware.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    32388 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/node.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    16006 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/addon.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    59200 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.8/smc/core/collection.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    47199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/engines.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    25199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/sub_interfaces.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15428 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/general.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10872 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/core/engine_vss.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)   100393 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.8/smc/core/interfaces.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/smc/core/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2893 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.8/smc/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      251 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.8/smc/__version__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3569 2021-03-30 16:36:44.000000 fp-NGFW-SMC-python-1.0.8/README.rst
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    11489 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/HISTORY.rst
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18078 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/PKG-INFO
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       31 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/MANIFEST.in
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       67 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/setup.cfg
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1384 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.8/setup.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        4 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/top_level.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/dependency_links.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2324 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/SOURCES.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       17 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/requires.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18078 2021-08-19 16:24:44.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/PKG-INFO
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-08-19 16:24:40.000000 fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/not-zip-safe
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/actions/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/actions/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1530 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.9/smc/compat.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/vpn/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    23611 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/vpn/route.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    31166 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/vpn/elements.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18296 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/vpn/policy.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/vpn/__init__.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/api/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7760 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/api/configloader.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9734 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/api/exceptions.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10080 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/api/web.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1638 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/api/entry_point.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4996 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/api/common.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    31615 2021-09-16 15:30:09.000000 fp-NGFW-SMC-python-1.0.9/smc/api/session.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/api/__init__.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/base/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4834 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/structs.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3713 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/decorators.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    30755 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/collection.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    35044 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/model.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1991 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/mixins.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/base/util.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/base/__init__.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    36208 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/rule.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      236 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/qos.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5565 2021-07-29 15:34:35.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/ips.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    28311 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/rule_nat.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1258 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/file_filtering.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7991 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/layer3.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7403 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/policy.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    33260 2021-06-24 16:53:58.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/rule_elements.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5677 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/layer2.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3564 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/policy/interface.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15218 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/situations.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9206 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/profiles.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    33025 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/servers.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    16968 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/other.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10685 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/group.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    19748 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/protocols.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    22308 2021-05-27 19:10:46.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/netlink.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    24307 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/network.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2784 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/helpers.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10646 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/service.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     8525 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/user.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       13 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/elements/__init__.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    21126 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/ospf.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6289 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/bgp_access_list.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15892 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/route_map.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7514 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/access_list.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    24490 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/bgp.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3904 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/prefix_list.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/routing/__init__.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1788 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/license.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    12818 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/servers.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10238 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/users.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7688 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/reports.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    13409 2021-07-29 15:34:35.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/system.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9553 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/tasks.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4791 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/role.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5412 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/access_rights.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3361 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/vpn.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6454 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/tls_common.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    27909 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/tls.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    28326 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/scheduled_tasks.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3774 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/administration/updates.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/smc/core/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    41302 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/route.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7706 2021-08-19 15:31:41.000000 fp-NGFW-SMC-python-1.0.9/smc/core/waiters.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9335 2021-06-24 16:53:58.000000 fp-NGFW-SMC-python-1.0.9/smc/core/contact_address.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    58534 2021-05-27 19:10:46.000000 fp-NGFW-SMC-python-1.0.9/smc/core/engine.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5588 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/resource.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      285 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/hardware.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    32388 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/node.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    16006 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/addon.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    59200 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.9/smc/core/collection.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    47199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/engines.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    25199 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/sub_interfaces.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    15428 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/general.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    10872 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/core/engine_vss.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)   100393 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-1.0.9/smc/core/interfaces.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/smc/core/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2893 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-1.0.9/smc/__init__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      251 2021-09-16 15:30:09.000000 fp-NGFW-SMC-python-1.0.9/smc/__version__.py
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3569 2021-03-30 16:36:44.000000 fp-NGFW-SMC-python-1.0.9/README.rst
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    11489 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/HISTORY.rst
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18078 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/PKG-INFO
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       31 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/MANIFEST.in
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       67 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/setup.cfg
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1384 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-1.0.9/setup.py
+drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-09-16 16:10:18.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        4 2021-09-16 16:10:17.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/top_level.txt
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-09-16 16:10:17.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     2324 2021-09-16 16:10:17.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       17 2021-09-16 16:10:17.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/requires.txt
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    18078 2021-09-16 16:10:17.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/PKG-INFO
+-rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-09-16 16:10:13.000000 fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/not-zip-safe
```

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/compat.py` & `fp-NGFW-SMC-python-1.0.9/smc/compat.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/vpn/route.py` & `fp-NGFW-SMC-python-1.0.9/smc/vpn/route.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/vpn/elements.py` & `fp-NGFW-SMC-python-1.0.9/smc/vpn/elements.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/vpn/policy.py` & `fp-NGFW-SMC-python-1.0.9/smc/vpn/policy.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/configloader.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/configloader.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/exceptions.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/web.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/web.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/entry_point.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/entry_point.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/common.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/common.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/api/session.py` & `fp-NGFW-SMC-python-1.0.9/smc/api/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,15 +582,18 @@
         """
         json = {"domain": self.domain}
 
         credential = self.credential
         params = {}
 
         if credential.provider_name.startswith("lms"):
-            params = dict(login=credential._login, pwd=credential._pwd)
+            if self.domain:
+                params = dict(login=credential._login, pwd=credential._pwd, domain=self.domain)
+            else:
+                params = dict(login=credential._login, pwd=credential._pwd)
         else:
             json.update(authenticationkey=credential._api_key)
 
         if kwargs:
             json.update(**kwargs)
             # Store in case we need to rebuild later
             self._extra_args.update(**kwargs)
```

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/structs.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/structs.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/decorators.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/decorators.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/collection.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/collection.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/model.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/model.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/mixins.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/mixins.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/base/util.py` & `fp-NGFW-SMC-python-1.0.9/smc/base/util.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/rule.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/rule.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/ips.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/ips.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/rule_nat.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/rule_nat.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/file_filtering.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/file_filtering.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/layer3.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/layer3.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/policy.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/policy.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/rule_elements.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/rule_elements.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/layer2.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/layer2.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/policy/interface.py` & `fp-NGFW-SMC-python-1.0.9/smc/policy/interface.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/situations.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/situations.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/profiles.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/profiles.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/servers.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/servers.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/other.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/other.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/group.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/group.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/protocols.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/protocols.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/netlink.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/netlink.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/network.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/network.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/helpers.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/helpers.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/service.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/service.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/elements/user.py` & `fp-NGFW-SMC-python-1.0.9/smc/elements/user.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/ospf.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/ospf.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/bgp_access_list.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/bgp_access_list.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/route_map.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/route_map.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/access_list.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/access_list.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/bgp.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/bgp.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/routing/prefix_list.py` & `fp-NGFW-SMC-python-1.0.9/smc/routing/prefix_list.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/license.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/license.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/servers.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/servers.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/user_auth/users.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/user_auth/users.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/reports.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/reports.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/system.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/system.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/tasks.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/tasks.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/role.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/role.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/access_rights.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/access_rights.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/vpn.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/vpn.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/tls_common.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/tls_common.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/certificates/tls.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/certificates/tls.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/scheduled_tasks.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/scheduled_tasks.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/administration/updates.py` & `fp-NGFW-SMC-python-1.0.9/smc/administration/updates.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/route.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/route.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/waiters.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/waiters.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/contact_address.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/contact_address.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/engine.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/engine.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/resource.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/resource.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/node.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/node.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/addon.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/addon.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/collection.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/collection.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/engines.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/engines.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/sub_interfaces.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/sub_interfaces.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/general.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/general.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/engine_vss.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/engine_vss.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/core/interfaces.py` & `fp-NGFW-SMC-python-1.0.9/smc/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/smc/__init__.py` & `fp-NGFW-SMC-python-1.0.9/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/README.rst` & `fp-NGFW-SMC-python-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/HISTORY.rst` & `fp-NGFW-SMC-python-1.0.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/PKG-INFO` & `fp-NGFW-SMC-python-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fp-NGFW-SMC-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python based API to Forcepoint NGFW Management Center
 Home-page: http://github.com/Forcepoint/fp-NGFW-SMC-python
 Author: Forcepoint
 Author-email: PSIRT@forcepoint.com
 License: Apache 2.0
 Description: |Python version|
```

### Comparing `fp-NGFW-SMC-python-1.0.8/setup.py` & `fp-NGFW-SMC-python-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/SOURCES.txt` & `fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-1.0.8/fp_NGFW_SMC_python.egg-info/PKG-INFO` & `fp-NGFW-SMC-python-1.0.9/fp_NGFW_SMC_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fp-NGFW-SMC-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python based API to Forcepoint NGFW Management Center
 Home-page: http://github.com/Forcepoint/fp-NGFW-SMC-python
 Author: Forcepoint
 Author-email: PSIRT@forcepoint.com
 License: Apache 2.0
 Description: |Python version|
```

