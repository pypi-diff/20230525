# Comparing `tmp/pyvmomi-8.0.1.0.tar.gz` & `tmp/pyvmomi-8.0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvmomi-8.0.1.0.tar", last modified: Fri May  5 22:56:03 2023, max compression
+gzip compressed data, was "pyvmomi-8.0.1.0.1.tar", last modified: Thu May 25 15:14:36 2023, max compression
```

## Comparing `pyvmomi-8.0.1.0.tar` & `pyvmomi-8.0.1.0.1.tar`

### file list

```diff
@@ -1,218 +1,222 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.377829 pyvmomi-8.0.1.0/
--rw-rw-rw-   0        0        0    11510 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-04-24 20:06:46.000000 pyvmomi-8.0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      238 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0/NOTICE.txt
--rw-rw-rw-   0        0        0     4865 2023-05-05 22:56:03.378830 pyvmomi-8.0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3258 2023-04-27 12:08:03.000000 pyvmomi-8.0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.889850 pyvmomi-8.0.1.0/pyVim/
--rw-rw-rw-   0        0        0      163 2022-11-24 20:53:17.000000 pyvmomi-8.0.1.0/pyVim/__init__.py
--rw-rw-rw-   0        0        0    38332 2023-03-09 21:15:31.000000 pyvmomi-8.0.1.0/pyVim/connect.py
--rw-rw-rw-   0        0        0    62300 2023-02-06 16:32:40.000000 pyvmomi-8.0.1.0/pyVim/sso.py
--rw-rw-rw-   0        0        0    12028 2023-04-28 08:19:44.000000 pyvmomi-8.0.1.0/pyVim/task.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.971534 pyvmomi-8.0.1.0/pyVmomi/
--rw-rw-rw-   0        0        0      836 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Cache.py
--rw-rw-rw-   0        0        0     9634 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Differ.py
--rw-rw-rw-   0        0        0      932 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Feature.py
--rw-rw-rw-   0        0        0    12510 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Iso8601.py
--rw-rw-rw-   0        0        0     1470 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Security.py
--rw-rw-rw-   0        0        0    74293 2023-05-03 19:43:28.000000 pyvmomi-8.0.1.0/pyVmomi/SoapAdapter.py
--rw-rw-rw-   0        0        0     2165 2023-05-03 19:30:54.000000 pyvmomi-8.0.1.0/pyVmomi/StubAdapterAccessorImpl.py
--rw-rw-rw-   0        0        0      644 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/Version.py
--rw-rw-rw-   0        0        0     5752 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/VmomiJSONEncoder.py
--rw-rw-rw-   0        0        0    72988 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/VmomiSupport.py
--rw-rw-rw-   0        0        0     3002 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/__init__.py
--rw-rw-rw-   0        0        0     5225 2023-05-03 19:34:10.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_core.py
--rw-rw-rw-   0        0        0    88121 2023-05-03 19:34:17.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_eam.py
--rw-rw-rw-   0        0        0   121683 2023-05-03 19:38:39.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_pbm.py
--rw-rw-rw-   0        0        0    12391 2023-05-03 19:39:45.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_query.py
--rw-rw-rw-   0        0        0   136338 2023-05-03 19:39:58.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_sms.py
--rw-rw-rw-   0        0        0  1319281 2023-05-03 19:40:28.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfo_vim.py
--rw-rw-rw-   0        0        0      692 2023-05-03 19:33:57.000000 pyvmomi-8.0.1.0/pyVmomi/_typeinfos.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.974534 pyvmomi-8.0.1.0/pyVmomi/eam/
--rw-rw-rw-   0        0        0     6485 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.976534 pyvmomi-8.0.1.0/pyVmomi/eam/fault/
--rw-rw-rw-   0        0        0     1348 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.978534 pyvmomi-8.0.1.0/pyVmomi/eam/issue/
--rw-rw-rw-   0        0        0     4807 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.981534 pyvmomi-8.0.1.0/pyVmomi/eam/issue/cluster/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.983534 pyvmomi-8.0.1.0/pyVmomi/eam/issue/cluster/agent/
--rw-rw-rw-   0        0        0     1135 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/cluster/agent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.985535 pyvmomi-8.0.1.0/pyVmomi/eam/issue/integrity/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/integrity/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.987535 pyvmomi-8.0.1.0/pyVmomi/eam/issue/integrity/agency/
--rw-rw-rw-   0        0        0      205 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/integrity/agency/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.990536 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.993535 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/agency/
--rw-rw-rw-   0        0        0      652 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/agency/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.996539 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/agent/
--rw-rw-rw-   0        0        0      166 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/issue/personality/agent/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:02.999538 pyvmomi-8.0.1.0/pyVmomi/eam/lccm/
--rw-rw-rw-   0        0        0     6252 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/lccm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.002536 pyvmomi-8.0.1.0/pyVmomi/eam/vib/
--rw-rw-rw-   0        0        0      601 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/eam/vib/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.005554 pyvmomi-8.0.1.0/pyVmomi/pbm/
--rw-rw-rw-   0        0        0     2812 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.007545 pyvmomi-8.0.1.0/pyVmomi/pbm/auth/
--rw-rw-rw-   0        0        0       92 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/auth/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.010547 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/
--rw-rw-rw-   0        0        0     1965 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.013534 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/provider/
--rw-rw-rw-   0        0        0     2473 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.015536 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/types/
--rw-rw-rw-   0        0        0      606 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/capability/types/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.018553 pyvmomi-8.0.1.0/pyVmomi/pbm/compliance/
--rw-rw-rw-   0        0        0     3083 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/compliance/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.021538 pyvmomi-8.0.1.0/pyVmomi/pbm/fault/
--rw-rw-rw-   0        0        0     1631 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.023538 pyvmomi-8.0.1.0/pyVmomi/pbm/placement/
--rw-rw-rw-   0        0        0     2425 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/placement/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.026538 pyvmomi-8.0.1.0/pyVmomi/pbm/profile/
--rw-rw-rw-   0        0        0     6423 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/profile/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.029539 pyvmomi-8.0.1.0/pyVmomi/pbm/profile/provider/
--rw-rw-rw-   0        0        0      531 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/profile/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.031537 pyvmomi-8.0.1.0/pyVmomi/pbm/provider/
--rw-rw-rw-   0        0        0       86 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.034538 pyvmomi-8.0.1.0/pyVmomi/pbm/replication/
--rw-rw-rw-   0        0        0      548 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/pbm/replication/__init__.pyi
--rw-rw-rw-   0        0        0        0 2023-04-24 10:28:17.000000 pyvmomi-8.0.1.0/pyVmomi/py.typed
--rw-rw-rw-   0        0        0      244 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0/pyVmomi/pyVmomiSettings.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.037548 pyvmomi-8.0.1.0/pyVmomi/sms/
--rw-rw-rw-   0        0        0     4882 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.040549 pyvmomi-8.0.1.0/pyVmomi/sms/fault/
--rw-rw-rw-   0        0        0     2941 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.043546 pyvmomi-8.0.1.0/pyVmomi/sms/fault/replication/
--rw-rw-rw-   0        0        0      689 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/fault/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.046548 pyvmomi-8.0.1.0/pyVmomi/sms/provider/
--rw-rw-rw-   0        0        0     5999 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/provider/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.050070 pyvmomi-8.0.1.0/pyVmomi/sms/storage/
--rw-rw-rw-   0        0        0     7274 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/storage/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.053088 pyvmomi-8.0.1.0/pyVmomi/sms/storage/replication/
--rw-rw-rw-   0        0        0     8613 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/sms/storage/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.057082 pyvmomi-8.0.1.0/pyVmomi/vim/
--rw-rw-rw-   0        0        0   154809 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/vim/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.061079 pyvmomi-8.0.1.0/pyVmomi/vim/action/
--rw-rw-rw-   0        0        0     1297 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/action/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.065082 pyvmomi-8.0.1.0/pyVmomi/vim/alarm/
--rw-rw-rw-   0        0        0     7405 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/vim/alarm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.068078 pyvmomi-8.0.1.0/pyVmomi/vim/cluster/
--rw-rw-rw-   0        0        0    28575 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/vim/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.071529 pyvmomi-8.0.1.0/pyVmomi/vim/dvs/
--rw-rw-rw-   0        0        0    38167 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/vim/dvs/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.075893 pyvmomi-8.0.1.0/pyVmomi/vim/encryption/
--rw-rw-rw-   0        0        0    10414 2023-05-05 22:37:43.000000 pyvmomi-8.0.1.0/pyVmomi/vim/encryption/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.079902 pyvmomi-8.0.1.0/pyVmomi/vim/event/
--rw-rw-rw-   0        0        0    55591 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/event/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.084891 pyvmomi-8.0.1.0/pyVmomi/vim/ext/
--rw-rw-rw-   0        0        0     1066 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/ext/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.089890 pyvmomi-8.0.1.0/pyVmomi/vim/fault/
--rw-rw-rw-   0        0        0    78582 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vim/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.093890 pyvmomi-8.0.1.0/pyVmomi/vim/host/
--rw-rw-rw-   0        0        0   187062 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.099079 pyvmomi-8.0.1.0/pyVmomi/vim/net/
--rw-rw-rw-   0        0        0     5666 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vim/net/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.104085 pyvmomi-8.0.1.0/pyVmomi/vim/option/
--rw-rw-rw-   0        0        0     2102 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/option/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.108085 pyvmomi-8.0.1.0/pyVmomi/vim/profile/
--rw-rw-rw-   0        0        0    10264 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/profile/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.112087 pyvmomi-8.0.1.0/pyVmomi/vim/profile/cluster/
--rw-rw-rw-   0        0        0      966 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/profile/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.115087 pyvmomi-8.0.1.0/pyVmomi/vim/profile/host/
--rw-rw-rw-   0        0        0    18331 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/profile/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.117087 pyvmomi-8.0.1.0/pyVmomi/vim/scheduler/
--rw-rw-rw-   0        0        0     4606 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/scheduler/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.119079 pyvmomi-8.0.1.0/pyVmomi/vim/tenant/
--rw-rw-rw-   0        0        0      414 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/tenant/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.122081 pyvmomi-8.0.1.0/pyVmomi/vim/vcha/
--rw-rw-rw-   0        0        0     6527 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vcha/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.125084 pyvmomi-8.0.1.0/pyVmomi/vim/view/
--rw-rw-rw-   0        0        0     1417 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/view/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.129082 pyvmomi-8.0.1.0/pyVmomi/vim/vm/
--rw-rw-rw-   0        0        0    83052 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.133079 pyvmomi-8.0.1.0/pyVmomi/vim/vm/check/
--rw-rw-rw-   0        0        0     1611 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/check/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.137090 pyvmomi-8.0.1.0/pyVmomi/vim/vm/customization/
--rw-rw-rw-   0        0        0     5700 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/customization/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.140170 pyvmomi-8.0.1.0/pyVmomi/vim/vm/device/
--rw-rw-rw-   0        0        0    39345 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/device/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.144177 pyvmomi-8.0.1.0/pyVmomi/vim/vm/guest/
--rw-rw-rw-   0        0        0    11325 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/guest/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.147092 pyvmomi-8.0.1.0/pyVmomi/vim/vm/replication/
--rw-rw-rw-   0        0        0      510 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vm/replication/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.149133 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/
--rw-rw-rw-   0        0        0        0 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.151852 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/cluster/
--rw-rw-rw-   0        0        0      496 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/cluster/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.153752 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/host/
--rw-rw-rw-   0        0        0     4534 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vsan/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.156750 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/
--rw-rw-rw-   0        0        0     5698 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.159752 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/host/
--rw-rw-rw-   0        0        0     3294 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/host/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.163752 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/vcenter/
--rw-rw-rw-   0        0        0     4737 2023-05-05 22:37:44.000000 pyvmomi-8.0.1.0/pyVmomi/vim/vslm/vcenter/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.166750 pyvmomi-8.0.1.0/pyVmomi/vmodl/
--rw-rw-rw-   0        0        0     1323 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vmodl/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.169755 pyvmomi-8.0.1.0/pyVmomi/vmodl/fault/
--rw-rw-rw-   0        0        0     1286 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vmodl/fault/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.173750 pyvmomi-8.0.1.0/pyVmomi/vmodl/query/
--rw-rw-rw-   0        0        0     5537 2023-05-05 22:37:45.000000 pyvmomi-8.0.1.0/pyVmomi/vmodl/query/__init__.pyi
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.196759 pyvmomi-8.0.1.0/pyvmomi.egg-info/
--rw-rw-rw-   0        0        0     4865 2023-05-05 22:56:02.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4710 2023-05-05 22:56:02.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 22:56:02.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-05 22:56:02.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-05 22:56:02.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-24 20:22:03.000000 pyvmomi-8.0.1.0/pyvmomi.egg-info/zip-safe
--rw-rw-rw-   0        0        0       12 2022-11-24 21:14:55.000000 pyvmomi-8.0.1.0/requirements.txt
--rw-rw-rw-   0        0        0      112 2023-05-05 22:56:03.380831 pyvmomi-8.0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3004 2023-04-27 12:07:18.000000 pyvmomi-8.0.1.0/setup.py
--rw-rw-rw-   0        0        0       42 2023-02-06 15:29:30.000000 pyvmomi-8.0.1.0/test-requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.245770 pyvmomi-8.0.1.0/tests/
--rw-rw-rw-   0        0        0      485 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/README.rst
--rw-rw-rw-   0        0        0     1581 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.281295 pyvmomi-8.0.1.0/tests/files/
--rw-rw-rw-   0        0        0    72751 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_datacenter_explode.expect
--rw-rw-rw-   0        0        0     7005 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_datastore_explode.expect
--rw-rw-rw-   0        0        0  1403229 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_host_explode.expect
--rw-rw-rw-   0        0        0     1120 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_network_explode.expect
--rw-rw-rw-   0        0        0    83829 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_default.expect
--rw-rw-rw-   0        0        0    84925 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_objs_match.expect
--rw-rw-rw-   0        0        0    67681 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_strip_dynamic.expect
--rw-rw-rw-   0        0        0   138420 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_type_match.expect
--rw-rw-rw-   0        0        0     3881 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/files/unknown_method.xml
-drwxrwxrwx   0        0        0        0 2023-05-05 22:56:03.373834 pyvmomi-8.0.1.0/tests/fixtures/
--rw-rw-rw-   0        0        0    19046 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/basic_connection.yaml
--rw-rw-rw-   0        0        0     6611 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/basic_connection_bad_password.yaml
--rw-rw-rw-   0        0        0    24770 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/basic_container_view.yaml
--rw-rw-rw-   0        0        0      619 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/http_proxy.yaml
--rw-rw-rw-   0        0        0    25823 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/iso8601_set_datetime.yaml
--rw-rw-rw-   0        0        0    30887 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/pbm_check_compatibility.yaml
--rw-rw-rw-   0        0        0    23423 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/root_folder_parent.yaml
--rw-rw-rw-   0        0        0    22129 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/smart_connection.yaml
--rw-rw-rw-   0        0        0      329 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/ssl_tunnel.yaml
--rw-rw-rw-   0        0        0      605 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/ssl_tunnel_http_failure.yaml
--rw-rw-rw-   0        0        0    19039 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/sspi_connection.yaml
--rw-rw-rw-   0        0        0   128012 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_datacenter_explode.yaml
--rw-rw-rw-   0        0        0    72776 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_datastore_explode.yaml
--rw-rw-rw-   0        0        0  1229165 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_host_explode.yaml
--rw-rw-rw-   0        0        0    59413 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_network_explode.yaml
--rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_default.yaml
--rw-rw-rw-   0        0        0   201173 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_objs.yaml
--rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml
--rw-rw-rw-   0        0        0   272726 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_type.yaml
--rw-rw-rw-   0        0        0     3233 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_simple_request_serializer.yaml
--rw-rw-rw-   0        0        0    22674 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/test_vm_config_iso8601.yaml
--rw-rw-rw-   0        0        0   236577 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/fixtures/vm_nic_data.yaml
--rw-rw-rw-   0        0        0     5839 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_connect.py
--rw-rw-rw-   0        0        0     1740 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_container_view.py
--rw-rw-rw-   0        0        0     1389 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_deserializer.py
--rw-rw-rw-   0        0        0     4360 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_iso8601.py
--rw-rw-rw-   0        0        0     7305 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_json.py
--rw-rw-rw-   0        0        0     1396 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_managed_object.py
--rw-rw-rw-   0        0        0     2592 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_pbm_check_compatibility.py
--rw-rw-rw-   0        0        0     5051 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_serializer.py
--rw-rw-rw-   0        0        0      432 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_vim_session_oriented_stub.py
--rw-rw-rw-   0        0        0     3086 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tests/test_virtual_machine_object.py
--rw-rw-rw-   0        0        0      103 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.673256 pyvmomi-8.0.1.0.1/
+-rw-rw-rw-   0        0        0    11510 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      172 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      238 2022-07-08 07:50:02.000000 pyvmomi-8.0.1.0.1/NOTICE.txt
+-rw-rw-rw-   0        0        0     4867 2023-05-25 15:14:36.674343 pyvmomi-8.0.1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3258 2023-04-27 12:08:03.000000 pyvmomi-8.0.1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:35.974528 pyvmomi-8.0.1.0.1/pyVim/
+-rw-rw-rw-   0        0        0      163 2022-11-24 20:53:17.000000 pyvmomi-8.0.1.0.1/pyVim/__init__.py
+-rw-rw-rw-   0        0        0    38332 2023-03-09 21:15:31.000000 pyvmomi-8.0.1.0.1/pyVim/connect.py
+-rw-rw-rw-   0        0        0    62300 2023-02-06 16:32:40.000000 pyvmomi-8.0.1.0.1/pyVim/sso.py
+-rw-rw-rw-   0        0        0    12028 2023-04-28 08:19:44.000000 pyvmomi-8.0.1.0.1/pyVim/task.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.200574 pyvmomi-8.0.1.0.1/pyVmomi/
+-rw-rw-rw-   0        0        0      836 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Cache.py
+-rw-rw-rw-   0        0        0     9634 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Differ.py
+-rw-rw-rw-   0        0        0      932 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Feature.py
+-rw-rw-rw-   0        0        0    12510 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Iso8601.py
+-rw-rw-rw-   0        0        0     1470 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Security.py
+-rw-rw-rw-   0        0        0    74293 2023-05-03 19:43:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/SoapAdapter.py
+-rw-rw-rw-   0        0        0     2165 2023-05-03 19:30:54.000000 pyvmomi-8.0.1.0.1/pyVmomi/StubAdapterAccessorImpl.py
+-rw-rw-rw-   0        0        0      644 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/Version.py
+-rw-rw-rw-   0        0        0     5752 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/VmomiJSONEncoder.py
+-rw-rw-rw-   0        0        0    72988 2023-05-16 12:11:40.000000 pyvmomi-8.0.1.0.1/pyVmomi/VmomiSupport.py
+-rw-rw-rw-   0        0        0     3002 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/__init__.py
+-rw-rw-rw-   0        0        0     5225 2023-05-03 19:34:10.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_core.py
+-rw-rw-rw-   0        0        0    88121 2023-05-03 19:34:17.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_eam.py
+-rw-rw-rw-   0        0        0   121683 2023-05-03 19:38:39.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_pbm.py
+-rw-rw-rw-   0        0        0    12391 2023-05-03 19:39:45.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_query.py
+-rw-rw-rw-   0        0        0   136338 2023-05-03 19:39:58.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_sms.py
+-rw-rw-rw-   0        0        0  1319281 2023-05-14 19:31:15.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_vim.py
+-rw-rw-rw-   0        0        0      692 2023-05-03 19:33:57.000000 pyvmomi-8.0.1.0.1/pyVmomi/_typeinfos.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.206172 pyvmomi-8.0.1.0.1/pyVmomi/eam/
+-rw-rw-rw-   0        0        0    15066 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.208230 pyvmomi-8.0.1.0.1/pyVmomi/eam/fault/
+-rw-rw-rw-   0        0        0     2426 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.212198 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/
+-rw-rw-rw-   0        0        0     8674 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.214791 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/
+-rw-rw-rw-   0        0        0       19 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.217852 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/agent/
+-rw-rw-rw-   0        0        0     1971 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/cluster/agent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.220796 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/
+-rw-rw-rw-   0        0        0       20 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.224301 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/agency/
+-rw-rw-rw-   0        0        0      205 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/integrity/agency/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.227309 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/
+-rw-rw-rw-   0        0        0       27 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.230325 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agency/
+-rw-rw-rw-   0        0        0     1204 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agency/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.233339 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agent/
+-rw-rw-rw-   0        0        0      166 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/issue/personality/agent/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.235968 pyvmomi-8.0.1.0.1/pyVmomi/eam/lccm/
+-rw-rw-rw-   0        0        0    16188 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/lccm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.240979 pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/
+-rw-rw-rw-   0        0        0     1336 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.244056 pyvmomi-8.0.1.0.1/pyVmomi/pbm/
+-rw-rw-rw-   0        0        0     5081 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.247612 pyvmomi-8.0.1.0.1/pyVmomi/pbm/auth/
+-rw-rw-rw-   0        0        0       92 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/auth/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.250625 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/
+-rw-rw-rw-   0        0        0     4437 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.255106 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/provider/
+-rw-rw-rw-   0        0        0     4965 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.260100 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/types/
+-rw-rw-rw-   0        0        0     1231 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/types/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.265305 pyvmomi-8.0.1.0.1/pyVmomi/pbm/compliance/
+-rw-rw-rw-   0        0        0     6060 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/compliance/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.269310 pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/
+-rw-rw-rw-   0        0        0     3064 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.272529 pyvmomi-8.0.1.0.1/pyVmomi/pbm/placement/
+-rw-rw-rw-   0        0        0     4175 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/placement/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.278055 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/
+-rw-rw-rw-   0        0        0    11494 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.282076 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/provider/
+-rw-rw-rw-   0        0        0     1318 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/profile/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.286576 pyvmomi-8.0.1.0.1/pyVmomi/pbm/provider/
+-rw-rw-rw-   0        0        0       86 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.289562 pyvmomi-8.0.1.0.1/pyVmomi/pbm/replication/
+-rw-rw-rw-   0        0        0      881 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pbm/replication/__init__.pyi
+-rw-rw-rw-   0        0        0        0 2023-05-05 22:57:58.000000 pyvmomi-8.0.1.0.1/pyVmomi/py.typed
+-rw-rw-rw-   0        0        0      244 2023-05-03 19:26:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/pyVmomiSettings.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.292564 pyvmomi-8.0.1.0.1/pyVmomi/sms/
+-rw-rw-rw-   0        0        0     7021 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.296077 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/
+-rw-rw-rw-   0        0        0     5403 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.299078 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/replication/
+-rw-rw-rw-   0        0        0     1081 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/fault/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.301079 pyvmomi-8.0.1.0.1/pyVmomi/sms/provider/
+-rw-rw-rw-   0        0        0    10967 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/provider/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.305666 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/
+-rw-rw-rw-   0        0        0    16413 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.309635 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/replication/
+-rw-rw-rw-   0        0        0    19257 2023-05-25 14:47:28.000000 pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.312635 pyvmomi-8.0.1.0.1/pyVmomi/vim/
+-rw-rw-rw-   0        0        0   297305 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.316153 pyvmomi-8.0.1.0.1/pyVmomi/vim/action/
+-rw-rw-rw-   0        0        0     2202 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/action/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.319198 pyvmomi-8.0.1.0.1/pyVmomi/vim/alarm/
+-rw-rw-rw-   0        0        0    15604 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/alarm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.322153 pyvmomi-8.0.1.0.1/pyVmomi/vim/cluster/
+-rw-rw-rw-   0        0        0    63584 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.325243 pyvmomi-8.0.1.0.1/pyVmomi/vim/dvs/
+-rw-rw-rw-   0        0        0   100848 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/dvs/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.328273 pyvmomi-8.0.1.0.1/pyVmomi/vim/encryption/
+-rw-rw-rw-   0        0        0    19092 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/encryption/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.332312 pyvmomi-8.0.1.0.1/pyVmomi/vim/event/
+-rw-rw-rw-   0        0        0   106110 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/event/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.334746 pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/
+-rw-rw-rw-   0        0        0     2402 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.337752 pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/
+-rw-rw-rw-   0        0        0   143157 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.340846 pyvmomi-8.0.1.0.1/pyVmomi/vim/host/
+-rw-rw-rw-   0        0        0   437042 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.344396 pyvmomi-8.0.1.0.1/pyVmomi/vim/net/
+-rw-rw-rw-   0        0        0    11910 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/net/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.347363 pyvmomi-8.0.1.0.1/pyVmomi/vim/option/
+-rw-rw-rw-   0        0        0     4185 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/option/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.350374 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/
+-rw-rw-rw-   0        0        0    20853 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.354878 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/cluster/
+-rw-rw-rw-   0        0        0     1372 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.358893 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/
+-rw-rw-rw-   0        0        0    36486 2023-05-25 14:47:29.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.361935 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/profileEngine/
+-rw-rw-rw-   0        0        0      190 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/profile/host/profileEngine/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.366492 pyvmomi-8.0.1.0.1/pyVmomi/vim/scheduler/
+-rw-rw-rw-   0        0        0     9113 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/scheduler/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.369503 pyvmomi-8.0.1.0.1/pyVmomi/vim/storageDrs/
+-rw-rw-rw-   0        0        0    24800 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/storageDrs/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.372496 pyvmomi-8.0.1.0.1/pyVmomi/vim/tenant/
+-rw-rw-rw-   0        0        0      414 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/tenant/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.376024 pyvmomi-8.0.1.0.1/pyVmomi/vim/vcha/
+-rw-rw-rw-   0        0        0    12321 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vcha/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.380061 pyvmomi-8.0.1.0.1/pyVmomi/vim/view/
+-rw-rw-rw-   0        0        0     1417 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/view/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.383022 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/
+-rw-rw-rw-   0        0        0   188045 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.386550 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/check/
+-rw-rw-rw-   0        0        0     2058 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/check/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.390560 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/customization/
+-rw-rw-rw-   0        0        0    12143 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/customization/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.394098 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/device/
+-rw-rw-rw-   0        0        0    85963 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/device/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.398109 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/guest/
+-rw-rw-rw-   0        0        0    17968 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/guest/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.401105 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/replication/
+-rw-rw-rw-   0        0        0     1024 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vm/replication/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.404103 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/
+-rw-rw-rw-   0        0        0       27 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.406649 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/cluster/
+-rw-rw-rw-   0        0        0     1168 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/cluster/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.408643 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/host/
+-rw-rw-rw-   0        0        0     9828 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vsan/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.411654 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/
+-rw-rw-rw-   0        0        0    12685 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.416150 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/
+-rw-rw-rw-   0        0        0     3294 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.419154 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/
+-rw-rw-rw-   0        0        0     5459 2023-05-25 14:47:30.000000 pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.422157 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/
+-rw-rw-rw-   0        0        0     2287 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.424267 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/
+-rw-rw-rw-   0        0        0     2055 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.428321 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/query/
+-rw-rw-rw-   0        0        0    10309 2023-05-25 14:47:31.000000 pyvmomi-8.0.1.0.1/pyVmomi/vmodl/query/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.444571 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/
+-rw-rw-rw-   0        0        0     4867 2023-05-25 15:14:34.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4798 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 15:14:34.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-25 15:14:35.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 20:22:03.000000 pyvmomi-8.0.1.0.1/pyvmomi.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       12 2022-11-24 21:14:55.000000 pyvmomi-8.0.1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      112 2023-05-25 15:14:36.676003 pyvmomi-8.0.1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     3006 2023-05-25 15:03:35.000000 pyvmomi-8.0.1.0.1/setup.py
+-rw-rw-rw-   0        0        0       42 2023-02-06 15:29:30.000000 pyvmomi-8.0.1.0.1/test-requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.546796 pyvmomi-8.0.1.0.1/tests/
+-rw-rw-rw-   0        0        0      485 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/README.rst
+-rw-rw-rw-   0        0        0     1581 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.590707 pyvmomi-8.0.1.0.1/tests/files/
+-rw-rw-rw-   0        0        0    72751 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_datacenter_explode.expect
+-rw-rw-rw-   0        0        0     7005 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_datastore_explode.expect
+-rw-rw-rw-   0        0        0  1403229 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_host_explode.expect
+-rw-rw-rw-   0        0        0     1120 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_network_explode.expect
+-rw-rw-rw-   0        0        0    83829 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_default.expect
+-rw-rw-rw-   0        0        0    84925 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_objs_match.expect
+-rw-rw-rw-   0        0        0    67681 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_strip_dynamic.expect
+-rw-rw-rw-   0        0        0   138420 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_type_match.expect
+-rw-rw-rw-   0        0        0     3881 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/files/unknown_method.xml
+drwxrwxrwx   0        0        0        0 2023-05-25 15:14:36.669274 pyvmomi-8.0.1.0.1/tests/fixtures/
+-rw-rw-rw-   0        0        0    19046 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection.yaml
+-rw-rw-rw-   0        0        0     6611 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection_bad_password.yaml
+-rw-rw-rw-   0        0        0    24770 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/basic_container_view.yaml
+-rw-rw-rw-   0        0        0      619 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/http_proxy.yaml
+-rw-rw-rw-   0        0        0    25823 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/iso8601_set_datetime.yaml
+-rw-rw-rw-   0        0        0    30887 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/pbm_check_compatibility.yaml
+-rw-rw-rw-   0        0        0    23423 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/root_folder_parent.yaml
+-rw-rw-rw-   0        0        0    22129 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/smart_connection.yaml
+-rw-rw-rw-   0        0        0      329 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel.yaml
+-rw-rw-rw-   0        0        0      605 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel_http_failure.yaml
+-rw-rw-rw-   0        0        0    19039 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/sspi_connection.yaml
+-rw-rw-rw-   0        0        0   128012 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datacenter_explode.yaml
+-rw-rw-rw-   0        0        0    72776 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datastore_explode.yaml
+-rw-rw-rw-   0        0        0  1229165 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_host_explode.yaml
+-rw-rw-rw-   0        0        0    59413 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_network_explode.yaml
+-rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_default.yaml
+-rw-rw-rw-   0        0        0   201173 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_objs.yaml
+-rw-rw-rw-   0        0        0   155062 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml
+-rw-rw-rw-   0        0        0   272726 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_type.yaml
+-rw-rw-rw-   0        0        0     3233 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_simple_request_serializer.yaml
+-rw-rw-rw-   0        0        0    22674 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/test_vm_config_iso8601.yaml
+-rw-rw-rw-   0        0        0   236577 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/fixtures/vm_nic_data.yaml
+-rw-rw-rw-   0        0        0     5839 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_connect.py
+-rw-rw-rw-   0        0        0     1740 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_container_view.py
+-rw-rw-rw-   0        0        0     1389 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_deserializer.py
+-rw-rw-rw-   0        0        0     4360 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_iso8601.py
+-rw-rw-rw-   0        0        0     7305 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_json.py
+-rw-rw-rw-   0        0        0     1396 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_managed_object.py
+-rw-rw-rw-   0        0        0     2592 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_pbm_check_compatibility.py
+-rw-rw-rw-   0        0        0     5051 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_serializer.py
+-rw-rw-rw-   0        0        0      432 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_vim_session_oriented_stub.py
+-rw-rw-rw-   0        0        0     3086 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tests/test_virtual_machine_object.py
+-rw-rw-rw-   0        0        0      103 2022-07-08 07:50:03.000000 pyvmomi-8.0.1.0.1/tox.ini
```

### Comparing `pyvmomi-8.0.1.0/LICENSE.txt` & `pyvmomi-8.0.1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/PKG-INFO` & `pyvmomi-8.0.1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvmomi
-Version: 8.0.1.0
+Version: 8.0.1.0.1
 Summary: VMware vSphere Python SDK
 Home-page: https://github.com/vmware/pyvmomi
 Author: VMware, Inc.
 Author-email: jhu@vmware.com
 License: License :: OSI Approved :: Apache Software License
 Keywords: pyvmomi,vsphere,vmware,esx
 Platform: Windows
```

### Comparing `pyvmomi-8.0.1.0/README.rst` & `pyvmomi-8.0.1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVim/connect.py` & `pyvmomi-8.0.1.0.1/pyVim/connect.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVim/sso.py` & `pyvmomi-8.0.1.0.1/pyVim/sso.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVim/task.py` & `pyvmomi-8.0.1.0.1/pyVim/task.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Cache.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Cache.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Differ.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Differ.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Feature.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Feature.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Iso8601.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Iso8601.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Security.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Security.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/SoapAdapter.py` & `pyvmomi-8.0.1.0.1/pyVmomi/SoapAdapter.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/StubAdapterAccessorImpl.py` & `pyvmomi-8.0.1.0.1/pyVmomi/StubAdapterAccessorImpl.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/Version.py` & `pyvmomi-8.0.1.0.1/pyVmomi/Version.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/VmomiJSONEncoder.py` & `pyvmomi-8.0.1.0.1/pyVmomi/VmomiJSONEncoder.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/VmomiSupport.py` & `pyvmomi-8.0.1.0.1/pyVmomi/VmomiSupport.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/__init__.py` & `pyvmomi-8.0.1.0.1/pyVmomi/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_core.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_core.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_eam.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_eam.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_pbm.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_pbm.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_query.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_query.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_sms.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_sms.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfo_vim.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfo_vim.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/_typeinfos.py` & `pyvmomi-8.0.1.0.1/pyVmomi/_typeinfos.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/pbm/capability/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/ext/__init__.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 from typing import List
-from pyVmomi import pbm, vmodl
-from pyVmomi.VmomiSupport import ManagedObject
+from pyVmomi import vim, vmodl
 
 
-class CapabilityMetadataManager(ManagedObject): ...
-
-
-class CapabilityInstance(vmodl.DynamicData):
-    @property
-    def id(self) -> CapabilityMetadata.UniqueId: ...
-    @property
-    def constraint(self) -> List[ConstraintInstance]: ...
-
-
-class CapabilityMetadata(vmodl.DynamicData):
+class ExtendedProductInfo(vmodl.DynamicData):
     @property
-    def id(self) -> CapabilityMetadata.UniqueId: ...
+    def companyUrl(self) -> str: ...
+    @companyUrl.setter
+    def companyUrl(self, value: str):
+        self._companyUrl = value
     @property
-    def summary(self) -> pbm.ExtendedElementDescription: ...
+    def productUrl(self) -> str: ...
+    @productUrl.setter
+    def productUrl(self, value: str):
+        self._productUrl = value
     @property
-    def mandatory(self) -> bool: ...
+    def managementUrl(self) -> str: ...
+    @managementUrl.setter
+    def managementUrl(self, value: str):
+        self._managementUrl = value
     @property
-    def hint(self) -> bool: ...
-    @property
-    def keyId(self) -> str: ...
-    @property
-    def allowMultipleConstraints(self) -> bool: ...
-    @property
-    def propertyMetadata(self) -> List[PropertyMetadata]: ...
-
-
-    class UniqueId(vmodl.DynamicData):
-        @property
-        def namespace(self) -> str: ...
-        @property
-        def id(self) -> str: ...
+    def self(self) -> vim.ManagedEntity: ...
+    @self.setter
+    def self(self, value: vim.ManagedEntity):
+        self._self = value
 
 
-class ConstraintInstance(vmodl.DynamicData):
+class ManagedByInfo(vmodl.DynamicData):
     @property
-    def propertyInstance(self) -> List[PropertyInstance]: ...
-
-
-class GenericTypeInfo(TypeInfo):
+    def extensionKey(self) -> str: ...
+    @extensionKey.setter
+    def extensionKey(self, value: str):
+        self._extensionKey = value
     @property
-    def genericTypeName(self) -> str: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
 
 
-class PropertyInstance(vmodl.DynamicData):
+class ManagedEntityInfo(vmodl.DynamicData):
     @property
-    def id(self) -> str: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def operator(self) -> str: ...
+    def smallIconUrl(self) -> str: ...
+    @smallIconUrl.setter
+    def smallIconUrl(self, value: str):
+        self._smallIconUrl = value
     @property
-    def value(self) -> object: ...
+    def iconUrl(self) -> str: ...
+    @iconUrl.setter
+    def iconUrl(self, value: str):
+        self._iconUrl = value
+    @property
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
 
 
-class PropertyMetadata(vmodl.DynamicData):
-    @property
-    def id(self) -> str: ...
-    @property
-    def summary(self) -> pbm.ExtendedElementDescription: ...
+class SolutionManagerInfo(vmodl.DynamicData):
     @property
-    def mandatory(self) -> bool: ...
+    def tab(self) -> List[SolutionManagerInfo.TabInfo]: ...
+    @tab.setter
+    def tab(self, value: List[SolutionManagerInfo.TabInfo]):
+        self._tab = value
     @property
-    def type(self) -> TypeInfo: ...
-    @property
-    def defaultValue(self) -> object: ...
-    @property
-    def allowedValue(self) -> object: ...
-    @property
-    def requirementsTypeHint(self) -> str: ...
+    def smallIconUrl(self) -> str: ...
+    @smallIconUrl.setter
+    def smallIconUrl(self, value: str):
+        self._smallIconUrl = value
 
 
-class TypeInfo(vmodl.DynamicData):
-    @property
-    def typeName(self) -> str: ...
+    class TabInfo(vmodl.DynamicData):
+        @property
+        def label(self) -> str: ...
+        @label.setter
+        def label(self, value: str):
+            self._label = value
+        @property
+        def url(self) -> str: ...
+        @url.setter
+        def url(self, value: str):
+            self._url = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/pbm/compliance/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/pbm/fault/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,110 @@
 from typing import List
-from enum import Enum
 from pyVmomi import pbm, vmodl
-from datetime import datetime
-from pyVmomi.VmomiSupport import ManagedObject, long
 
 
-class ComplianceManager(ManagedObject):
-    def CheckCompliance(self, entities: List[pbm.ServerObjectRef], profile: pbm.profile.ProfileId) -> List[ComplianceResult]: ...
-    def FetchComplianceResult(self, entities: List[pbm.ServerObjectRef], profile: pbm.profile.ProfileId) -> List[ComplianceResult]: ...
-    def CheckRollupCompliance(self, entity: List[pbm.ServerObjectRef]) -> List[RollupComplianceResult]: ...
-    def FetchRollupComplianceResult(self, entity: List[pbm.ServerObjectRef]) -> List[RollupComplianceResult]: ...
-    def QueryByRollupComplianceStatus(self, status: str) -> List[pbm.ServerObjectRef]: ...
+class AlreadyExists(PBMFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-class ComplianceResult(vmodl.DynamicData):
-    @property
-    def checkTime(self) -> datetime: ...
-    @property
-    def entity(self) -> pbm.ServerObjectRef: ...
-    @property
-    def profile(self) -> pbm.profile.ProfileId: ...
-    @property
-    def complianceTaskStatus(self) -> str: ...
+class CapabilityProfilePropertyMismatchFault(PropertyMismatchFault):
     @property
-    def complianceStatus(self) -> str: ...
-    @property
-    def mismatch(self) -> bool: ...
-    @property
-    def violatedPolicies(self) -> List[PolicyStatus]: ...
-    @property
-    def errorCause(self) -> List[vmodl.MethodFault]: ...
+    def resourcePropertyInstance(self) -> pbm.capability.PropertyInstance: ...
+    @resourcePropertyInstance.setter
+    def resourcePropertyInstance(self, value: pbm.capability.PropertyInstance):
+        self._resourcePropertyInstance = value
+
+
+class CompatibilityCheckFault(PBMFault):
     @property
-    def operationalStatus(self) -> OperationalStatus: ...
+    def hub(self) -> pbm.placement.PlacementHub: ...
+    @hub.setter
+    def hub(self, value: pbm.placement.PlacementHub):
+        self._hub = value
+
+
+class DefaultProfileAppliesFault(CompatibilityCheckFault): ...
+
+
+class DuplicateName(PBMFault):
     @property
-    def info(self) -> pbm.ExtendedElementDescription: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-    class ComplianceStatus(Enum):
-        compliant = "compliant"
-        nonCompliant = "noncompliant"
-        unknown = "unknown"
-        notApplicable = "notapplicable"
-        outOfDate = "outofdate"
+class IncompatibleVendorSpecificRuleSet(CapabilityProfilePropertyMismatchFault): ...
 
 
-    class ComplianceTaskStatus(Enum):
-        inProgress = "inprogress"
-        success = "success"
-        failed = "failed"
+class InvalidLogin(PBMFault): ...
 
 
-class FetchEntityHealthStatusSpec(vmodl.DynamicData):
+class LegacyHubsNotSupported(PBMFault):
     @property
-    def objectRef(self) -> pbm.ServerObjectRef: ...
-    @property
-    def backingId(self) -> str: ...
+    def hubs(self) -> List[pbm.placement.PlacementHub]: ...
+    @hubs.setter
+    def hubs(self, value: List[pbm.placement.PlacementHub]):
+        self._hubs = value
 
 
-class OperationalStatus(vmodl.DynamicData):
-    @property
-    def healthy(self) -> bool: ...
-    @property
-    def operationETA(self) -> datetime: ...
-    @property
-    def operationProgress(self) -> long: ...
-    @property
-    def transitional(self) -> bool: ...
+class NoPermission():
 
 
-class PolicyStatus(vmodl.DynamicData):
-    @property
-    def expectedValue(self) -> pbm.capability.CapabilityInstance: ...
-    @property
-    def currentValue(self) -> pbm.capability.CapabilityInstance: ...
+    class EntityPrivileges(vmodl.DynamicData):
+        @property
+        def profileId(self) -> pbm.profile.ProfileId: ...
+        @profileId.setter
+        def profileId(self, value: pbm.profile.ProfileId):
+            self._profileId = value
+        @property
+        def privilegeIds(self) -> List[str]: ...
+        @privilegeIds.setter
+        def privilegeIds(self, value: List[str]):
+            self._privilegeIds = value
 
 
-class RollupComplianceResult(vmodl.DynamicData):
-    @property
-    def oldestCheckTime(self) -> datetime: ...
-    @property
-    def entity(self) -> pbm.ServerObjectRef: ...
+class NonExistentHubs(PBMFault):
     @property
-    def overallComplianceStatus(self) -> str: ...
-    @property
-    def overallComplianceTaskStatus(self) -> str: ...
-    @property
-    def result(self) -> List[ComplianceResult]: ...
+    def hubs(self) -> List[pbm.placement.PlacementHub]: ...
+    @hubs.setter
+    def hubs(self, value: List[pbm.placement.PlacementHub]):
+        self._hubs = value
+
+
+class NotFound(PBMFault): ...
+
+
+class PBMFault(vmodl.MethodFault): ...
+
+
+class ProfileStorageFault(PBMFault): ...
+
+
+class PropertyMismatchFault(CompatibilityCheckFault):
     @property
-    def errorCause(self) -> List[vmodl.MethodFault]: ...
+    def capabilityInstanceId(self) -> pbm.capability.CapabilityMetadata.UniqueId: ...
+    @capabilityInstanceId.setter
+    def capabilityInstanceId(self, value: pbm.capability.CapabilityMetadata.UniqueId):
+        self._capabilityInstanceId = value
     @property
-    def profileMismatch(self) -> bool: ...
+    def requirementPropertyInstance(self) -> pbm.capability.PropertyInstance: ...
+    @requirementPropertyInstance.setter
+    def requirementPropertyInstance(self, value: pbm.capability.PropertyInstance):
+        self._requirementPropertyInstance = value
 
 
-class HealthStatus(pbm.version.v7_0): ...
+class ResourceInUse(PBMFault):
+    @property
+    def type(self) -> type: ...
+    @type.setter
+    def type(self, value: type):
+        self._type = value
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/pbm/fault/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vmodl/fault/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,71 +1,87 @@
-from typing import List
-from pyVmomi import pbm, vmodl
+from pyVmomi import vmodl
+from pyVmomi.VmomiSupport import ManagedObject, PropertyPath
 
 
-class AlreadyExists(PBMFault):
-    @property
-    def name(self) -> str: ...
-
+class HostCommunication(vmodl.RuntimeFault): ...
 
-class CapabilityProfilePropertyMismatchFault(PropertyMismatchFault):
-    @property
-    def resourcePropertyInstance(self) -> pbm.capability.PropertyInstance: ...
 
-
-class CompatibilityCheckFault(PBMFault):
-    @property
-    def hub(self) -> pbm.placement.PlacementHub: ...
+class HostNotConnected(HostCommunication): ...
 
 
-class DefaultProfileAppliesFault(CompatibilityCheckFault): ...
+class HostNotReachable(HostCommunication): ...
 
 
-class DuplicateName(PBMFault):
+class InvalidArgument(vmodl.RuntimeFault):
     @property
-    def name(self) -> str: ...
+    def invalidProperty(self) -> PropertyPath: ...
+    @invalidProperty.setter
+    def invalidProperty(self, value: PropertyPath):
+        self._invalidProperty = value
 
 
-class IncompatibleVendorSpecificRuleSet(CapabilityProfilePropertyMismatchFault): ...
+class InvalidRequest(vmodl.RuntimeFault): ...
 
 
-class InvalidLogin(PBMFault): ...
+class InvalidType(InvalidRequest):
+    @property
+    def argument(self) -> PropertyPath: ...
+    @argument.setter
+    def argument(self, value: PropertyPath):
+        self._argument = value
 
 
-class LegacyHubsNotSupported(PBMFault):
+class ManagedObjectNotFound(vmodl.RuntimeFault):
     @property
-    def hubs(self) -> List[pbm.placement.PlacementHub]: ...
+    def obj(self) -> ManagedObject: ...
+    @obj.setter
+    def obj(self, value: ManagedObject):
+        self._obj = value
 
 
-class EntityPrivileges(vmodl.DynamicData):
+class MethodNotFound(InvalidRequest):
     @property
-    def profileId(self) -> pbm.profile.ProfileId: ...
+    def receiver(self) -> ManagedObject: ...
+    @receiver.setter
+    def receiver(self, value: ManagedObject):
+        self._receiver = value
     @property
-    def privilegeIds(self) -> List[str]: ...
+    def method(self) -> str: ...
+    @method.setter
+    def method(self, value: str):
+        self._method = value
 
 
-class NonExistentHubs(PBMFault):
-    @property
-    def hubs(self) -> List[pbm.placement.PlacementHub]: ...
+class NotEnoughLicenses(vmodl.RuntimeFault): ...
 
 
-class NotFound(PBMFault): ...
+class NotImplemented(vmodl.RuntimeFault): ...
 
 
-class PBMFault(vmodl.MethodFault): ...
+class NotSupported(vmodl.RuntimeFault): ...
 
 
-class ProfileStorageFault(PBMFault): ...
+class RequestCanceled(vmodl.RuntimeFault): ...
 
 
-class PropertyMismatchFault(CompatibilityCheckFault):
-    @property
-    def capabilityInstanceId(self) -> pbm.capability.CapabilityMetadata.UniqueId: ...
+class SecurityError(vmodl.RuntimeFault): ...
+
+
+class SystemError(vmodl.RuntimeFault):
     @property
-    def requirementPropertyInstance(self) -> pbm.capability.PropertyInstance: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
 
-class ResourceInUse(PBMFault):
+class UnexpectedFault(vmodl.RuntimeFault):
     @property
-    def type(self) -> type: ...
+    def faultName(self) -> type: ...
+    @faultName.setter
+    def faultName(self, value: type):
+        self._faultName = value
     @property
-    def name(self) -> str: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/fault/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,4710 +1,5466 @@
-from typing import List
+from typing import List, Literal
 from enum import Enum
-from pyVmomi import HbrManager, OvfConsumer, storageDrs, vApp, vim, vmodl
+from pyVmomi import vim, vmodl
 from datetime import datetime
-from pyVmomi.VmomiSupport import ManagedMethod, ManagedObject, NoneType, byte, double, long
-from . import alarm, cluster, dvs, encryption, event, ext, host, option, profile, scheduler, tenant, vcha, view, vm, vsan, vslm
+from pyVmomi.VmomiSupport import ManagedObject, PropertyPath, long
 
 
-class AuthorizationManager(ManagedObject):
+class ActiveDirectoryFault(VimFault):
     @property
-    def privilegeList(self) -> List[AuthorizationManager.Privilege]: ...
+    def errorCode(self) -> int: ...
+    @errorCode.setter
+    def errorCode(self, value: int):
+        self._errorCode = value
+
+
+class ActiveVMsBlockingEVC(EVCConfigFault):
+    @property
+    def evcMode(self) -> str: ...
+    @evcMode.setter
+    def evcMode(self, value: str):
+        self._evcMode = value
+    @property
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
     @property
-    def roleList(self) -> List[AuthorizationManager.Role]: ...
-    @property
-    def description(self) -> AuthorizationDescription: ...
-    def AddRole(self, name: str, privIds: List[str]) -> int: ...
-    def RemoveRole(self, roleId: int, failIfUsed: bool) -> NoneType: ...
-    def UpdateRole(self, roleId: int, newName: str, privIds: List[str]) -> NoneType: ...
-    def MergePermissions(self, srcRoleId: int, dstRoleId: int) -> NoneType: ...
-    def RetrieveRolePermissions(self, roleId: int) -> List[AuthorizationManager.Permission]: ...
-    def RetrieveEntityPermissions(self, entity: ManagedEntity, inherited: bool) -> List[AuthorizationManager.Permission]: ...
-    def RetrieveAllPermissions(self) -> List[AuthorizationManager.Permission]: ...
-    def SetEntityPermissions(self, entity: ManagedEntity, permission: List[AuthorizationManager.Permission]) -> NoneType: ...
-    def ResetEntityPermissions(self, entity: ManagedEntity, permission: List[AuthorizationManager.Permission]) -> NoneType: ...
-    def RemoveEntityPermission(self, entity: ManagedEntity, user: str, isGroup: bool) -> NoneType: ...
-    def HasPrivilegeOnEntity(self, entity: ManagedEntity, sessionId: str, privId: List[str]) -> List[bool]: ...
-    def HasPrivilegeOnEntities(self, entity: List[ManagedEntity], sessionId: str, privId: List[str]) -> List[AuthorizationManager.EntityPrivilege]: ...
-    def HasUserPrivilegeOnEntities(self, entities: List[ManagedObject], userName: str, privId: List[str]) -> List[AuthorizationManager.EntityPrivilege]: ...
-    def FetchUserPrivilegeOnEntities(self, entities: List[ManagedEntity], userName: str) -> List[AuthorizationManager.UserPrivilegeResult]: ...
+    def hostName(self) -> List[str]: ...
+    @hostName.setter
+    def hostName(self, value: List[str]):
+        self._hostName = value
 
 
-    class EntityPrivilege(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedEntity: ...
-        @property
-        def privAvailability(self) -> List[AuthorizationManager.PrivilegeAvailability]: ...
+class AdminDisabled(HostConfigFault): ...
 
 
-    class Permission(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedEntity: ...
-        @property
-        def principal(self) -> str: ...
-        @property
-        def group(self) -> bool: ...
-        @property
-        def roleId(self) -> int: ...
-        @property
-        def propagate(self) -> bool: ...
+class AdminNotDisabled(HostConfigFault): ...
 
 
-    class Privilege(vmodl.DynamicData):
-        @property
-        def privId(self) -> str: ...
-        @property
-        def onParent(self) -> bool: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def privGroupName(self) -> str: ...
+class AffinityConfigured(MigrationFault):
+    @property
+    def configuredAffinity(self) -> List[str]: ...
+    @configuredAffinity.setter
+    def configuredAffinity(self, value: List[str]):
+        self._configuredAffinity = value
 
 
-    class PrivilegeAvailability(vmodl.DynamicData):
-        @property
-        def privId(self) -> str: ...
-        @property
-        def isGranted(self) -> bool: ...
+    class Affinity(Enum):
+        memory = "memory"
+        cpu = "cpu"
 
 
-    class Role(vmodl.DynamicData):
-        @property
-        def roleId(self) -> int: ...
-        @property
-        def system(self) -> bool: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def info(self) -> Description: ...
-        @property
-        def privilege(self) -> List[str]: ...
+class AgentInstallFailed(HostConnectFault):
+    @property
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
+    @property
+    def statusCode(self) -> int: ...
+    @statusCode.setter
+    def statusCode(self, value: int):
+        self._statusCode = value
+    @property
+    def installerOutput(self) -> str: ...
+    @installerOutput.setter
+    def installerOutput(self, value: str):
+        self._installerOutput = value
+
+
+    class Reason(Enum):
+        NotEnoughSpaceOnDevice = "NotEnoughSpaceOnDevice"
+        PrepareToUpgradeFailed = "PrepareToUpgradeFailed"
+        AgentNotRunning = "AgentNotRunning"
+        AgentNotReachable = "AgentNotReachable"
+        InstallTimedout = "InstallTimedout"
+        SignatureVerificationFailed = "SignatureVerificationFailed"
+        AgentUploadFailed = "AgentUploadFailed"
+        AgentUploadTimedout = "AgentUploadTimedout"
+        UnknownInstallerError = "UnknownInstallerError"
+
+
+class AlreadyBeingManaged(HostConnectFault):
+    @property
+    def ipAddress(self) -> str: ...
+    @ipAddress.setter
+    def ipAddress(self, value: str):
+        self._ipAddress = value
 
 
-    class UserPrivilegeResult(vmodl.DynamicData):
+class AlreadyConnected(HostConnectFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class AlreadyExists(VimFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class AlreadyUpgraded(VimFault): ...
+
+
+class AnswerFileUpdateFailed(VimFault):
+    @property
+    def failure(self) -> List[AnswerFileUpdateFailed.UpdateFailure]: ...
+    @failure.setter
+    def failure(self, value: List[AnswerFileUpdateFailed.UpdateFailure]):
+        self._failure = value
+
+
+    class UpdateFailure(vmodl.DynamicData):
         @property
-        def entity(self) -> ManagedEntity: ...
+        def userInputPath(self) -> vim.profile.ProfilePropertyPath: ...
+        @userInputPath.setter
+        def userInputPath(self, value: vim.profile.ProfilePropertyPath):
+            self._userInputPath = value
         @property
-        def privileges(self) -> List[str]: ...
+        def errMsg(self) -> vmodl.LocalizableMessage: ...
+        @errMsg.setter
+        def errMsg(self, value: vmodl.LocalizableMessage):
+            self._errMsg = value
+
 
+class ApplicationQuiesceFault(SnapshotFault): ...
 
-class CertificateManager(ManagedObject):
-    def RefreshCACertificatesAndCRLs(self, host: List[HostSystem]) -> Task: ...
-    def RefreshCertificates(self, host: List[HostSystem]) -> Task: ...
-    def RevokeCertificates(self, host: List[HostSystem]) -> Task: ...
 
+class AuthMinimumAdminPermission(VimFault): ...
 
-class ClusterComputeResource(ComputeResource):
+
+class BackupBlobReadFailure(DvsFault):
     @property
-    def configuration(self) -> cluster.ConfigInfo: ...
+    def entityName(self) -> str: ...
+    @entityName.setter
+    def entityName(self, value: str):
+        self._entityName = value
+    @property
+    def entityType(self) -> str: ...
+    @entityType.setter
+    def entityType(self, value: str):
+        self._entityType = value
     @property
-    def recommendation(self) -> List[cluster.Recommendation]: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
+
+
+class BackupBlobWriteFailure(DvsFault):
     @property
-    def drsRecommendation(self) -> List[cluster.DrsRecommendation]: ...
+    def entityName(self) -> str: ...
+    @entityName.setter
+    def entityName(self, value: str):
+        self._entityName = value
+    @property
+    def entityType(self) -> str: ...
+    @entityType.setter
+    def entityType(self, value: str):
+        self._entityType = value
     @property
-    def summaryEx(self) -> ClusterComputeResource.Summary: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
+
+
+class BlockedByFirewall(HostConfigFault): ...
+
+
+class CAMServerRefusedConnection(InvalidCAMServer): ...
+
+
+class CannotAccessFile(FileFault): ...
+
+
+class CannotAccessLocalSource(VimFault): ...
+
+
+class CannotAccessNetwork(CannotAccessVmDevice):
+    @property
+    def network(self) -> vim.Network: ...
+    @network.setter
+    def network(self, value: vim.Network):
+        self._network = value
+
+
+class CannotAccessVmComponent(VmConfigFault): ...
+
+
+class CannotAccessVmConfig(CannotAccessVmComponent):
     @property
-    def hciConfig(self) -> ClusterComputeResource.HCIConfigInfo: ...
+    def reason(self) -> vmodl.MethodFault: ...
+    @reason.setter
+    def reason(self, value: vmodl.MethodFault):
+        self._reason = value
+
+
+class CannotAccessVmDevice(CannotAccessVmComponent):
     @property
-    def migrationHistory(self) -> List[cluster.DrsMigration]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def actionHistory(self) -> List[cluster.ActionHistory]: ...
+    def backing(self) -> str: ...
+    @backing.setter
+    def backing(self, value: str):
+        self._backing = value
     @property
-    def drsFault(self) -> List[cluster.DrsFaults]: ...
-    def ConfigureHCI(self, clusterSpec: ClusterComputeResource.HCIConfigSpec, hostInputs: List[ClusterComputeResource.HostConfigurationInput]) -> Task: ...
-    def ExtendHCI(self, hostInputs: List[ClusterComputeResource.HostConfigurationInput], vSanConfigSpec: SDDCBase) -> Task: ...
-    def AbandonHciWorkflow(self) -> NoneType: ...
-    def ValidateHCIConfiguration(self, hciConfigSpec: ClusterComputeResource.HCIConfigSpec, hosts: List[HostSystem]) -> List[ClusterComputeResource.ValidationResultBase]: ...
-    def Reconfigure(self, spec: cluster.ConfigSpec, modify: bool) -> Task: ...
-    def ApplyRecommendation(self, key: str) -> NoneType: ...
-    def CancelRecommendation(self, key: str) -> NoneType: ...
-    def RecommendHostsForVm(self, vm: VirtualMachine, pool: ResourcePool) -> List[cluster.HostRecommendation]: ...
-    def AddHost(self, spec: host.ConnectSpec, asConnected: bool, resourcePool: ResourcePool, license: str) -> Task: ...
-    def MoveInto(self, host: List[HostSystem]) -> Task: ...
-    def MoveHostInto(self, host: HostSystem, resourcePool: ResourcePool) -> Task: ...
-    def RefreshRecommendation(self) -> NoneType: ...
-    def EvcManager(self) -> cluster.EVCManager: ...
-    def RetrieveDasAdvancedRuntimeInfo(self) -> cluster.DasAdvancedRuntimeInfo: ...
-    def EnterMaintenanceMode(self, host: List[HostSystem], option: List[option.OptionValue]) -> cluster.EnterMaintenanceResult: ...
-    def PlaceVm(self, placementSpec: cluster.PlacementSpec) -> cluster.PlacementResult: ...
-    def FindRulesForVm(self, vm: VirtualMachine) -> List[cluster.RuleInfo]: ...
-    def StampAllRulesWithUuid(self) -> Task: ...
-    def GetResourceUsage(self) -> cluster.ResourceUsageSummary: ...
-    def SetCryptoMode(self, cryptoMode: str) -> NoneType: ...
-    def GetSystemVMsRestrictedDatastores(self) -> List[Datastore]: ...
+    def connected(self) -> bool: ...
+    @connected.setter
+    def connected(self, value: bool):
+        self._connected = value
 
 
-    class ClusterConfigResult(vmodl.DynamicData):
-        @property
-        def failedHosts(self) -> List[Folder.FailedHostResult]: ...
-        @property
-        def configuredHosts(self) -> List[HostSystem]: ...
+class CannotAccessVmDisk(CannotAccessVmDevice):
+    @property
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
 
 
-    class DVSConfigurationValidation(ClusterComputeResource.ValidationResultBase):
-        @property
-        def isDvsValid(self) -> bool: ...
-        @property
-        def isDvpgValid(self) -> bool: ...
+class CannotAddHostWithFTVmAsStandalone(HostConnectFault): ...
 
 
-    class DVSSetting(vmodl.DynamicData):
-        @property
-        def dvSwitch(self) -> DistributedVirtualSwitch: ...
-        @property
-        def pnicDevices(self) -> List[str]: ...
-        @property
-        def dvPortgroupSetting(self) -> List[ClusterComputeResource.DVSSetting.DVPortgroupToServiceMapping]: ...
+class CannotAddHostWithFTVmToDifferentCluster(HostConnectFault): ...
 
 
-        class DVPortgroupToServiceMapping(vmodl.DynamicData):
-            @property
-            def dvPortgroup(self) -> dvs.DistributedVirtualPortgroup: ...
-            @property
-            def service(self) -> str: ...
+class CannotAddHostWithFTVmToNonHACluster(HostConnectFault): ...
 
 
-    class DvsProfile(vmodl.DynamicData):
-        @property
-        def dvsName(self) -> str: ...
-        @property
-        def dvSwitch(self) -> DistributedVirtualSwitch: ...
-        @property
-        def pnicDevices(self) -> List[str]: ...
-        @property
-        def dvPortgroupMapping(self) -> List[ClusterComputeResource.DvsProfile.DVPortgroupSpecToServiceMapping]: ...
+class CannotChangeDrsBehaviorForFtSecondary(VmFaultToleranceIssue):
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-        class DVPortgroupSpecToServiceMapping(vmodl.DynamicData):
-            @property
-            def dvPortgroupSpec(self) -> dvs.DistributedVirtualPortgroup.ConfigSpec: ...
-            @property
-            def dvPortgroup(self) -> dvs.DistributedVirtualPortgroup: ...
-            @property
-            def service(self) -> str: ...
+class CannotChangeHaSettingsForFtSecondary(VmFaultToleranceIssue):
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class HCIConfigInfo(vmodl.DynamicData):
-        @property
-        def workflowState(self) -> str: ...
-        @property
-        def dvsSetting(self) -> List[ClusterComputeResource.DVSSetting]: ...
-        @property
-        def configuredHosts(self) -> List[HostSystem]: ...
-        @property
-        def hostConfigProfile(self) -> ClusterComputeResource.HostConfigurationProfile: ...
+class CannotChangeVsanClusterUuid(VsanFault): ...
 
 
-    class HCIConfigSpec(vmodl.DynamicData):
-        @property
-        def dvsProf(self) -> List[ClusterComputeResource.DvsProfile]: ...
-        @property
-        def hostConfigProfile(self) -> ClusterComputeResource.HostConfigurationProfile: ...
-        @property
-        def vSanConfigSpec(self) -> SDDCBase: ...
-        @property
-        def vcProf(self) -> ClusterComputeResource.VCProfile: ...
+class CannotChangeVsanNodeUuid(VsanFault): ...
 
 
-    class HostConfigurationInput(vmodl.DynamicData):
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def hostVmkNics(self) -> List[ClusterComputeResource.HostVmkNicInfo]: ...
-        @property
-        def allowedInNonMaintenanceMode(self) -> bool: ...
+class CannotComputeFTCompatibleHosts(VmFaultToleranceIssue):
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class HostConfigurationProfile(vmodl.DynamicData):
-        @property
-        def dateTimeConfig(self) -> host.DateTimeConfig: ...
-        @property
-        def lockdownMode(self) -> host.HostAccessManager.LockdownMode: ...
+class CannotCreateFile(FileFault): ...
 
 
-    class HostConfigurationValidation(ClusterComputeResource.ValidationResultBase):
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def isDvsSettingValid(self) -> bool: ...
-        @property
-        def isVmknicSettingValid(self) -> bool: ...
-        @property
-        def isNtpSettingValid(self) -> bool: ...
-        @property
-        def isLockdownModeValid(self) -> bool: ...
+class CannotDecryptPasswords(CustomizationFault): ...
 
 
-    class HostVmkNicInfo(vmodl.DynamicData):
-        @property
-        def nicSpec(self) -> host.VirtualNic.Specification: ...
-        @property
-        def service(self) -> str: ...
+class CannotDeleteFile(FileFault): ...
 
 
-    class Summary(ComputeResource.Summary):
-        @property
-        def currentFailoverLevel(self) -> int: ...
-        @property
-        def admissionControlInfo(self) -> cluster.DasAdmissionControlInfo: ...
-        @property
-        def numVmotions(self) -> int: ...
-        @property
-        def targetBalance(self) -> int: ...
-        @property
-        def currentBalance(self) -> int: ...
-        @property
-        def drsScore(self) -> int: ...
-        @property
-        def numVmsPerDrsScoreBucket(self) -> List[int]: ...
-        @property
-        def usageSummary(self) -> cluster.UsageSummary: ...
-        @property
-        def currentEVCModeKey(self) -> str: ...
-        @property
-        def currentEVCGraphicsModeKey(self) -> str: ...
-        @property
-        def dasData(self) -> cluster.DasData: ...
-        @property
-        def clusterMaintenanceModeStatus(self) -> str: ...
-        @property
-        def vcsHealthStatus(self) -> str: ...
-        @property
-        def vcsSlots(self) -> List[ClusterComputeResource.VcsSlots]: ...
+class CannotDisableDrsOnClustersWithVApps(vmodl.RuntimeFault): ...
 
 
-        class QuickStats(vmodl.DynamicData):
-            @property
-            def overallCpuUsage(self) -> long: ...
-            @property
-            def overallCpuDemand(self) -> long: ...
-            @property
-            def guestMemoryUsage(self) -> long: ...
-            @property
-            def hostMemoryUsage(self) -> long: ...
-            @property
-            def distributedCpuEntitlement(self) -> long: ...
-            @property
-            def distributedMemoryEntitlement(self) -> long: ...
-            @property
-            def staticCpuEntitlement(self) -> int: ...
-            @property
-            def staticMemoryEntitlement(self) -> int: ...
-            @property
-            def privateMemory(self) -> long: ...
-            @property
-            def sharedMemory(self) -> long: ...
-            @property
-            def swappedMemory(self) -> long: ...
-            @property
-            def balloonedMemory(self) -> long: ...
-            @property
-            def overheadMemory(self) -> long: ...
-            @property
-            def consumedOverheadMemory(self) -> long: ...
-            @property
-            def compressedMemory(self) -> long: ...
-
-
-        class MaintenanceModeState(Enum):
-            normal = "normal"
-            enteringMaintenance = "enteringmaintenance"
-            inMaintenance = "inmaintenance"
+class CannotDisableSnapshot(VmConfigFault): ...
 
 
-    class VCProfile(vmodl.DynamicData):
-        @property
-        def clusterSpec(self) -> cluster.ConfigSpecEx: ...
-        @property
-        def evcModeKey(self) -> str: ...
-        @property
-        def evcGraphicsModeKey(self) -> str: ...
+class CannotDisconnectHostWithFaultToleranceVm(VimFault):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-    class ValidationResultBase(vmodl.DynamicData):
-        @property
-        def info(self) -> List[vmodl.LocalizableMessage]: ...
+class CannotEnableVmcpForCluster(VimFault):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+    @property
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
 
-    class VcsSlots(vmodl.DynamicData):
-        @property
-        def systemId(self) -> str: ...
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def datastore(self) -> List[Datastore]: ...
-        @property
-        def totalSlots(self) -> int: ...
+class CannotModifyConfigCpuRequirements(MigrationFault): ...
+
+
+class CannotMoveFaultToleranceVm(VimFault):
+    @property
+    def moveType(self) -> str: ...
+    @moveType.setter
+    def moveType(self, value: str):
+        self._moveType = value
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class HCIWorkflowState(Enum):
-        in_progress = "in_progress"
-        done = "done"
-        invalid = "invalid"
+    class MoveType(Enum):
+        resourcePool = "resourcePool"
+        cluster = "cluster"
 
 
-    class VcsHealthStatus(Enum):
-        healthy = "healthy"
-        degraded = "degraded"
-        nonhealthy = "nonhealthy"
+class CannotMoveHostWithFaultToleranceVm(VimFault): ...
 
 
-class ComputeResource(ManagedEntity):
+class CannotMoveVmWithDeltaDisk(MigrationFault):
     @property
-    def resourcePool(self) -> ResourcePool: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
+
+
+class CannotMoveVmWithNativeDeltaDisk(MigrationFault): ...
+
+
+class CannotMoveVsanEnabledHost(VsanFault): ...
+
+
+class CannotPlaceWithoutPrerequisiteMoves(VimFault): ...
+
+
+class CannotPowerOffVmInCluster(InvalidState):
     @property
-    def host(self) -> List[HostSystem]: ...
+    def operation(self) -> str: ...
+    @operation.setter
+    def operation(self, value: str):
+        self._operation = value
     @property
-    def datastore(self) -> List[Datastore]: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def network(self) -> List[Network]: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+    class Operation(Enum):
+        suspend = "suspend"
+        powerOff = "powerOff"
+        guestShutdown = "guestShutdown"
+        guestSuspend = "guestSuspend"
+
+
+class CannotReconfigureVsanWhenHaEnabled(VsanFault): ...
+
+
+class CannotUseNetwork(VmConfigFault):
     @property
-    def summary(self) -> ComputeResource.Summary: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def environmentBrowser(self) -> EnvironmentBrowser: ...
+    def backing(self) -> str: ...
+    @backing.setter
+    def backing(self, value: str):
+        self._backing = value
     @property
-    def configurationEx(self) -> ComputeResource.ConfigInfo: ...
+    def connected(self) -> bool: ...
+    @connected.setter
+    def connected(self, value: bool):
+        self._connected = value
     @property
-    def lifecycleManaged(self) -> bool: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def configManagerEnabled(self) -> bool: ...
-    def ReconfigureEx(self, spec: ComputeResource.ConfigSpec, modify: bool) -> Task: ...
+    def network(self) -> vim.Network: ...
+    @network.setter
+    def network(self, value: vim.Network):
+        self._network = value
 
 
-    class ConfigInfo(vmodl.DynamicData):
-        @property
-        def vmSwapPlacement(self) -> str: ...
-        @property
-        def spbmEnabled(self) -> bool: ...
-        @property
-        def defaultHardwareVersionKey(self) -> str: ...
-        @property
-        def maximumHardwareVersionKey(self) -> str: ...
+class ClockSkew(HostConfigFault): ...
 
 
-    class ConfigSpec(vmodl.DynamicData):
-        @property
-        def vmSwapPlacement(self) -> str: ...
-        @property
-        def spbmEnabled(self) -> bool: ...
-        @property
-        def defaultHardwareVersionKey(self) -> str: ...
-        @property
-        def desiredSoftwareSpec(self) -> DesiredSoftwareSpec: ...
-        @property
-        def maximumHardwareVersionKey(self) -> str: ...
-        @property
-        def enableConfigManager(self) -> bool: ...
+class CloneFromSnapshotNotSupported(MigrationFault): ...
 
 
-    class HostSPBMLicenseInfo(vmodl.DynamicData):
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def licenseState(self) -> ComputeResource.HostSPBMLicenseInfo.HostSPBMLicenseState: ...
+class CollectorAddressUnset(DvsFault): ...
 
 
-        class HostSPBMLicenseState(Enum):
-            licensed = "licensed"
-            unlicensed = "unlicensed"
-            unknown = "unknown"
+class ConcurrentAccess(VimFault): ...
 
 
-class CustomFieldsManager(ManagedObject):
+class ConflictingConfiguration(DvsFault):
     @property
-    def field(self) -> List[CustomFieldsManager.FieldDef]: ...
-    def AddFieldDefinition(self, name: str, moType: type, fieldDefPolicy: PrivilegePolicyDef, fieldPolicy: PrivilegePolicyDef) -> CustomFieldsManager.FieldDef: ...
-    def RemoveFieldDefinition(self, key: int) -> NoneType: ...
-    def RenameFieldDefinition(self, key: int, name: str) -> NoneType: ...
-    def SetField(self, entity: ManagedEntity, key: int, value: str) -> NoneType: ...
+    def configInConflict(self) -> List[ConflictingConfiguration.Config]: ...
+    @configInConflict.setter
+    def configInConflict(self, value: List[ConflictingConfiguration.Config]):
+        self._configInConflict = value
 
 
-    class FieldDef(vmodl.DynamicData):
-        @property
-        def key(self) -> int: ...
+    class Config(vmodl.DynamicData):
         @property
-        def name(self) -> str: ...
-        @property
-        def type(self) -> type: ...
+        def entity(self) -> vim.ManagedEntity: ...
+        @entity.setter
+        def entity(self, value: vim.ManagedEntity):
+            self._entity = value
         @property
-        def managedObjectType(self) -> type: ...
-        @property
-        def fieldDefPrivileges(self) -> PrivilegePolicyDef: ...
-        @property
-        def fieldInstancePrivileges(self) -> PrivilegePolicyDef: ...
+        def propertyPath(self) -> str: ...
+        @propertyPath.setter
+        def propertyPath(self, value: str):
+            self._propertyPath = value
 
 
-    class StringValue(CustomFieldsManager.Value):
-        @property
-        def value(self) -> str: ...
+class ConflictingDatastoreFound(vmodl.RuntimeFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+    @property
+    def url(self) -> str: ...
+    @url.setter
+    def url(self, value: str):
+        self._url = value
 
 
-    class Value(vmodl.DynamicData):
-        @property
-        def key(self) -> int: ...
+class ConnectedIso(OvfExport):
+    @property
+    def cdrom(self) -> vim.vm.device.VirtualCdrom: ...
+    @cdrom.setter
+    def cdrom(self, value: vim.vm.device.VirtualCdrom):
+        self._cdrom = value
+    @property
+    def filename(self) -> str: ...
+    @filename.setter
+    def filename(self, value: str):
+        self._filename = value
 
 
-class CustomizationSpecManager(ManagedObject):
+class CpuCompatibilityUnknown(CpuIncompatible): ...
+
+
+class CpuHotPlugNotSupported(VmConfigFault): ...
+
+
+class CpuIncompatible(VirtualHardwareCompatibilityIssue):
+    @property
+    def level(self) -> int: ...
+    @level.setter
+    def level(self, value: int):
+        self._level = value
+    @property
+    def registerName(self) -> str: ...
+    @registerName.setter
+    def registerName(self, value: str):
+        self._registerName = value
     @property
-    def info(self) -> List[CustomizationSpecInfo]: ...
+    def registerBits(self) -> str: ...
+    @registerBits.setter
+    def registerBits(self, value: str):
+        self._registerBits = value
     @property
-    def encryptionKey(self) -> List[byte]: ...
-    def Exists(self, name: str) -> bool: ...
-    def Get(self, name: str) -> CustomizationSpecItem: ...
-    def Create(self, item: CustomizationSpecItem) -> NoneType: ...
-    def Overwrite(self, item: CustomizationSpecItem) -> NoneType: ...
-    def Delete(self, name: str) -> NoneType: ...
-    def Duplicate(self, name: str, newName: str) -> NoneType: ...
-    def Rename(self, name: str, newName: str) -> NoneType: ...
-    def SpecItemToXml(self, item: CustomizationSpecItem) -> str: ...
-    def XmlToSpecItem(self, specItemXml: str) -> CustomizationSpecItem: ...
-    def CheckResources(self, guestOs: str) -> NoneType: ...
+    def desiredBits(self) -> str: ...
+    @desiredBits.setter
+    def desiredBits(self, value: str):
+        self._desiredBits = value
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-class Datacenter(ManagedEntity):
+class CpuIncompatible1ECX(CpuIncompatible):
     @property
-    def vmFolder(self) -> Folder: ...
+    def sse3(self) -> bool: ...
+    @sse3.setter
+    def sse3(self, value: bool):
+        self._sse3 = value
     @property
-    def hostFolder(self) -> Folder: ...
+    def pclmulqdq(self) -> bool: ...
+    @pclmulqdq.setter
+    def pclmulqdq(self, value: bool):
+        self._pclmulqdq = value
     @property
-    def datastoreFolder(self) -> Folder: ...
+    def ssse3(self) -> bool: ...
+    @ssse3.setter
+    def ssse3(self, value: bool):
+        self._ssse3 = value
     @property
-    def networkFolder(self) -> Folder: ...
+    def sse41(self) -> bool: ...
+    @sse41.setter
+    def sse41(self, value: bool):
+        self._sse41 = value
     @property
-    def datastore(self) -> List[Datastore]: ...
+    def sse42(self) -> bool: ...
+    @sse42.setter
+    def sse42(self, value: bool):
+        self._sse42 = value
     @property
-    def network(self) -> List[Network]: ...
+    def aes(self) -> bool: ...
+    @aes.setter
+    def aes(self, value: bool):
+        self._aes = value
     @property
-    def configuration(self) -> Datacenter.ConfigInfo: ...
-    def BatchQueryConnectInfo(self, hostSpecs: List[host.ConnectSpec]) -> List[Datacenter.BasicConnectInfo]: ...
-    def QueryConnectionInfo(self, hostname: str, port: int, username: str, password: str, sslThumbprint: str) -> host.ConnectInfo: ...
-    def QueryConnectionInfoViaSpec(self, spec: host.ConnectSpec) -> host.ConnectInfo: ...
-    def PowerOnVm(self, vm: List[VirtualMachine], option: List[option.OptionValue]) -> Task: ...
-    def QueryConfigOptionDescriptor(self) -> List[vm.ConfigOptionDescriptor]: ...
-    def Reconfigure(self, spec: Datacenter.ConfigSpec, modify: bool) -> Task: ...
-
-
-    class BasicConnectInfo(vmodl.DynamicData):
-        @property
-        def hostname(self) -> str: ...
-        @property
-        def error(self) -> vmodl.MethodFault: ...
-        @property
-        def serverIp(self) -> str: ...
-        @property
-        def numVm(self) -> int: ...
-        @property
-        def numPoweredOnVm(self) -> int: ...
-        @property
-        def hostProductInfo(self) -> AboutInfo: ...
-        @property
-        def hardwareVendor(self) -> str: ...
-        @property
-        def hardwareModel(self) -> str: ...
+    def other(self) -> bool: ...
+    @other.setter
+    def other(self, value: bool):
+        self._other = value
+    @property
+    def otherOnly(self) -> bool: ...
+    @otherOnly.setter
+    def otherOnly(self, value: bool):
+        self._otherOnly = value
 
 
-class Datastore(ManagedEntity):
-    @property
-    def info(self) -> Datastore.Info: ...
+class CpuIncompatible81EDX(CpuIncompatible):
     @property
-    def summary(self) -> Datastore.Summary: ...
+    def nx(self) -> bool: ...
+    @nx.setter
+    def nx(self, value: bool):
+        self._nx = value
     @property
-    def host(self) -> List[Datastore.HostMount]: ...
+    def ffxsr(self) -> bool: ...
+    @ffxsr.setter
+    def ffxsr(self, value: bool):
+        self._ffxsr = value
     @property
-    def vm(self) -> List[VirtualMachine]: ...
+    def rdtscp(self) -> bool: ...
+    @rdtscp.setter
+    def rdtscp(self, value: bool):
+        self._rdtscp = value
     @property
-    def browser(self) -> host.DatastoreBrowser: ...
+    def lm(self) -> bool: ...
+    @lm.setter
+    def lm(self, value: bool):
+        self._lm = value
     @property
-    def capability(self) -> Datastore.Capability: ...
+    def other(self) -> bool: ...
+    @other.setter
+    def other(self, value: bool):
+        self._other = value
     @property
-    def iormConfiguration(self) -> StorageResourceManager.IORMConfigInfo: ...
-    def Refresh(self) -> NoneType: ...
-    def RefreshStorageInfo(self) -> NoneType: ...
-    def UpdateVirtualMachineFiles(self, mountPathDatastoreMapping: List[Datastore.MountPathDatastorePair]) -> Task: ...
-    def RenameDatastore(self, newName: str) -> NoneType: ...
-    def DestroyDatastore(self) -> NoneType: ...
-    def EnterMaintenanceMode(self) -> storageDrs.StoragePlacementResult: ...
-    def ExitMaintenanceMode(self) -> Task: ...
-    def IsClusteredVmdkEnabled(self) -> bool: ...
-    def UpdateVVolVirtualMachineFiles(self, failoverPair: List[Datastore.VVolContainerFailoverPair]) -> Task: ...
+    def otherOnly(self) -> bool: ...
+    @otherOnly.setter
+    def otherOnly(self, value: bool):
+        self._otherOnly = value
 
 
-    class HostMount(vmodl.DynamicData):
-        @property
-        def key(self) -> HostSystem: ...
-        @property
-        def mountInfo(self) -> host.MountInfo: ...
+class CustomizationFault(VimFault): ...
 
 
-    class Info(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def url(self) -> str: ...
-        @property
-        def freeSpace(self) -> long: ...
-        @property
-        def maxFileSize(self) -> long: ...
-        @property
-        def maxVirtualDiskCapacity(self) -> long: ...
-        @property
-        def maxMemoryFileSize(self) -> long: ...
-        @property
-        def timestamp(self) -> datetime: ...
-        @property
-        def containerId(self) -> str: ...
-        @property
-        def aliasOf(self) -> str: ...
+class CustomizationPending(CustomizationFault): ...
 
 
-    class MountPathDatastorePair(vmodl.DynamicData):
-        @property
-        def oldMountPath(self) -> str: ...
-        @property
-        def datastore(self) -> Datastore: ...
+class DVPortNotSupported(DeviceBackingNotSupported): ...
 
 
-    class VVolContainerFailoverPair(vmodl.DynamicData):
-        @property
-        def srcContainer(self) -> str: ...
-        @property
-        def tgtContainer(self) -> str: ...
-        @property
-        def vvolMapping(self) -> List[KeyValue]: ...
+class DasConfigFault(VimFault):
+    @property
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
+    @property
+    def output(self) -> str: ...
+    @output.setter
+    def output(self, value: str):
+        self._output = value
+    @property
+    def event(self) -> List[vim.event.Event]: ...
+    @event.setter
+    def event(self, value: List[vim.event.Event]):
+        self._event = value
 
 
-    class Accessible(Enum):
-        True
-        False
+    class DasConfigFaultReason(Enum):
+        HostNetworkMisconfiguration = "HostNetworkMisconfiguration"
+        HostMisconfiguration = "HostMisconfiguration"
+        InsufficientPrivileges = "InsufficientPrivileges"
+        NoPrimaryAgentAvailable = "NoPrimaryAgentAvailable"
+        Other = "Other"
+        NoDatastoresConfigured = "NoDatastoresConfigured"
+        CreateConfigVvolFailed = "CreateConfigVvolFailed"
+        VSanNotSupportedOnHost = "VSanNotSupportedOnHost"
+        DasNetworkMisconfiguration = "DasNetworkMisconfiguration"
+        SetDesiredImageSpecFailed = "SetDesiredImageSpecFailed"
+        ApplyHAVibsOnClusterFailed = "ApplyHAVibsOnClusterFailed"
 
 
-class DatastoreNamespaceManager(ManagedObject):
-    def CreateDirectory(self, datastore: Datastore, displayName: str, policy: str, size: long) -> str: ...
-    def DeleteDirectory(self, datacenter: Datacenter, datastorePath: str) -> NoneType: ...
-    def ConvertNamespacePathToUuidPath(self, datacenter: Datacenter, namespaceUrl: str) -> str: ...
-    def IncreaseDirectorySize(self, datacenter: Datacenter, stableName: str, size: long) -> NoneType: ...
-    def QueryDirectoryInfo(self, datacenter: Datacenter, stableName: str) -> DatastoreNamespaceManager.DirectoryInfo: ...
+class DatabaseError(vmodl.RuntimeFault): ...
+
+
+class DatacenterMismatch(MigrationFault):
+    @property
+    def invalidArgument(self) -> List[DatacenterMismatch.Argument]: ...
+    @invalidArgument.setter
+    def invalidArgument(self, value: List[DatacenterMismatch.Argument]):
+        self._invalidArgument = value
+    @property
+    def expectedDatacenter(self) -> vim.Datacenter: ...
+    @expectedDatacenter.setter
+    def expectedDatacenter(self, value: vim.Datacenter):
+        self._expectedDatacenter = value
 
 
-    class DirectoryInfo(vmodl.DynamicData):
+    class Argument(vmodl.DynamicData):
         @property
-        def capacity(self) -> long: ...
+        def entity(self) -> vim.ManagedEntity: ...
+        @entity.setter
+        def entity(self, value: vim.ManagedEntity):
+            self._entity = value
         @property
-        def used(self) -> long: ...
+        def inputDatacenter(self) -> vim.Datacenter: ...
+        @inputDatacenter.setter
+        def inputDatacenter(self, value: vim.Datacenter):
+            self._inputDatacenter = value
 
 
-class DiagnosticManager(ManagedObject):
-    def QueryDescriptions(self, host: HostSystem) -> List[DiagnosticManager.LogDescriptor]: ...
-    def Browse(self, host: HostSystem, key: str, start: int, lines: int) -> DiagnosticManager.LogHeader: ...
-    def GenerateLogBundles(self, includeDefault: bool, host: List[HostSystem]) -> Task: ...
-    def FetchAuditRecords(self, token: str) -> DiagnosticManager.AuditRecordResult: ...
-    def EmitSyslogMark(self, message: str) -> NoneType: ...
+class DatastoreNotWritableOnHost(InvalidDatastore):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class AuditRecordResult(vmodl.DynamicData):
-        @property
-        def records(self) -> List[str]: ...
-        @property
-        def nextToken(self) -> str: ...
+class DeltaDiskFormatNotSupported(VmConfigFault):
+    @property
+    def datastore(self) -> List[vim.Datastore]: ...
+    @datastore.setter
+    def datastore(self, value: List[vim.Datastore]):
+        self._datastore = value
+    @property
+    def deltaDiskFormat(self) -> str: ...
+    @deltaDiskFormat.setter
+    def deltaDiskFormat(self, value: str):
+        self._deltaDiskFormat = value
 
 
-    class BundleInfo(vmodl.DynamicData):
-        @property
-        def system(self) -> HostSystem: ...
-        @property
-        def url(self) -> str: ...
+class DestinationSwitchFull(CannotAccessNetwork): ...
 
 
-    class LogDescriptor(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def fileName(self) -> str: ...
-        @property
-        def creator(self) -> str: ...
-        @property
-        def format(self) -> str: ...
-        @property
-        def mimeType(self) -> str: ...
-        @property
-        def info(self) -> Description: ...
+class DestinationVsanDisabled(CannotMoveVsanEnabledHost):
+    @property
+    def destinationCluster(self) -> str: ...
+    @destinationCluster.setter
+    def destinationCluster(self, value: str):
+        self._destinationCluster = value
 
 
-        class Creator(Enum):
-            vpxd = "vpxd"
-            vpxa = "vpxa"
-            hostd = "hostd"
-            serverd = "serverd"
-            install = "install"
-            vpxClient = "vpxclient"
-            recordLog = "recordlog"
+class DeviceBackingNotSupported(DeviceNotSupported):
+    @property
+    def backing(self) -> str: ...
+    @backing.setter
+    def backing(self, value: str):
+        self._backing = value
 
 
-        class Format(Enum):
-            plain = "plain"
+class DeviceControllerNotSupported(DeviceNotSupported):
+    @property
+    def controller(self) -> str: ...
+    @controller.setter
+    def controller(self, value: str):
+        self._controller = value
 
 
-    class LogHeader(vmodl.DynamicData):
-        @property
-        def lineStart(self) -> int: ...
-        @property
-        def lineEnd(self) -> int: ...
-        @property
-        def lineText(self) -> List[str]: ...
+class DeviceHotPlugNotSupported(InvalidDeviceSpec): ...
 
 
-class DistributedVirtualSwitch(ManagedEntity):
-    @property
-    def uuid(self) -> str: ...
-    @property
-    def capability(self) -> DistributedVirtualSwitch.Capability: ...
+class DeviceNotFound(InvalidDeviceSpec): ...
+
+
+class DeviceNotSupported(VirtualHardwareCompatibilityIssue):
     @property
-    def summary(self) -> DistributedVirtualSwitch.Summary: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def config(self) -> DistributedVirtualSwitch.ConfigInfo: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
+
+
+class DeviceUnsupportedForVmPlatform(InvalidDeviceSpec): ...
+
+
+class DeviceUnsupportedForVmVersion(InvalidDeviceSpec):
     @property
-    def networkResourcePool(self) -> List[dvs.NetworkResourcePool]: ...
+    def currentVersion(self) -> str: ...
+    @currentVersion.setter
+    def currentVersion(self, value: str):
+        self._currentVersion = value
     @property
-    def portgroup(self) -> List[dvs.DistributedVirtualPortgroup]: ...
-    @property
-    def runtime(self) -> DistributedVirtualSwitch.RuntimeInfo: ...
-    def FetchPortKeys(self, criteria: dvs.PortCriteria) -> List[str]: ...
-    def FetchPorts(self, criteria: dvs.PortCriteria) -> List[dvs.DistributedVirtualPort]: ...
-    def QueryUsedVlanId(self) -> List[int]: ...
-    def Reconfigure(self, spec: DistributedVirtualSwitch.ConfigSpec) -> Task: ...
-    def PerformProductSpecOperation(self, operation: str, productSpec: dvs.ProductSpec) -> Task: ...
-    def Merge(self, dvs: DistributedVirtualSwitch) -> Task: ...
-    def AddPortgroups(self, spec: List[dvs.DistributedVirtualPortgroup.ConfigSpec]) -> Task: ...
-    def MovePort(self, portKey: List[str], destinationPortgroupKey: str) -> Task: ...
-    def UpdateCapability(self, capability: DistributedVirtualSwitch.Capability) -> NoneType: ...
-    def ReconfigurePort(self, port: List[dvs.DistributedVirtualPort.ConfigSpec]) -> Task: ...
-    def RefreshPortState(self, portKeys: List[str]) -> NoneType: ...
-    def RectifyHost(self, hosts: List[HostSystem]) -> Task: ...
-    def UpdateNetworkResourcePool(self, configSpec: List[dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
-    def AddNetworkResourcePool(self, configSpec: List[dvs.NetworkResourcePool.ConfigSpec]) -> NoneType: ...
-    def RemoveNetworkResourcePool(self, key: List[str]) -> NoneType: ...
-    def ReconfigureVmVnicNetworkResourcePool(self, configSpec: List[dvs.VmVnicNetworkResourcePool.ConfigSpec]) -> Task: ...
-    def EnableNetworkResourceManagement(self, enable: bool) -> NoneType: ...
-    def Rollback(self, entityBackup: dvs.EntityBackup.Config) -> Task: ...
-    def AddPortgroup(self, spec: dvs.DistributedVirtualPortgroup.ConfigSpec) -> Task: ...
-    def UpdateHealthCheckConfig(self, healthCheckConfig: List[DistributedVirtualSwitch.HealthCheckConfig]) -> Task: ...
-    def LookupPortgroup(self, portgroupKey: str) -> dvs.DistributedVirtualPortgroup: ...
+    def expectedVersion(self) -> str: ...
+    @expectedVersion.setter
+    def expectedVersion(self, value: str):
+        self._expectedVersion = value
 
 
-    class BackupRestoreCapability(vmodl.DynamicData):
-        @property
-        def backupRestoreSupported(self) -> bool: ...
+class DigestNotSupported(DeviceNotSupported): ...
 
 
-    class ContactInfo(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def contact(self) -> str: ...
+class DirectoryNotEmpty(FileFault): ...
 
 
-    class CreateSpec(vmodl.DynamicData):
-        @property
-        def configSpec(self) -> DistributedVirtualSwitch.ConfigSpec: ...
-        @property
-        def productInfo(self) -> dvs.ProductSpec: ...
-        @property
-        def capability(self) -> DistributedVirtualSwitch.Capability: ...
+class DisableAdminNotSupported(HostConfigFault): ...
 
 
-    class FeatureCapability(vmodl.DynamicData):
-        @property
-        def networkResourceManagementSupported(self) -> bool: ...
-        @property
-        def vmDirectPathGen2Supported(self) -> bool: ...
-        @property
-        def nicTeamingPolicy(self) -> List[str]: ...
-        @property
-        def networkResourcePoolHighShareValue(self) -> int: ...
-        @property
-        def networkResourceManagementCapability(self) -> DistributedVirtualSwitch.NetworkResourceManagementCapability: ...
-        @property
-        def healthCheckCapability(self) -> DistributedVirtualSwitch.HealthCheckFeatureCapability: ...
-        @property
-        def rollbackCapability(self) -> DistributedVirtualSwitch.RollbackCapability: ...
-        @property
-        def backupRestoreCapability(self) -> DistributedVirtualSwitch.BackupRestoreCapability: ...
-        @property
-        def networkFilterSupported(self) -> bool: ...
-        @property
-        def macLearningSupported(self) -> bool: ...
+class DisallowedChangeByService(vmodl.RuntimeFault):
+    @property
+    def serviceName(self) -> str: ...
+    @serviceName.setter
+    def serviceName(self, value: str):
+        self._serviceName = value
+    @property
+    def disallowedChange(self) -> str: ...
+    @disallowedChange.setter
+    def disallowedChange(self, value: str):
+        self._disallowedChange = value
 
 
-    class HealthCheckConfig(vmodl.DynamicData):
-        @property
-        def enable(self) -> bool: ...
-        @property
-        def interval(self) -> int: ...
+    class DisallowedChange(Enum):
+        hotExtendDisk = "hotExtendDisk"
 
 
-    class HealthCheckFeatureCapability(vmodl.DynamicData): ...
+class DisallowedDiskModeChange(InvalidDeviceSpec): ...
 
 
-    class HostInfrastructureTrafficResource(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def description(self) -> str: ...
-        @property
-        def allocationInfo(self) -> DistributedVirtualSwitch.HostInfrastructureTrafficResource.ResourceAllocation: ...
+class DisallowedMigrationDeviceAttached(MigrationFault):
+    @property
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
 
 
-        class ResourceAllocation(vmodl.DynamicData):
-            @property
-            def limit(self) -> long: ...
-            @property
-            def shares(self) -> SharesInfo: ...
-            @property
-            def reservation(self) -> long: ...
+class DisallowedOperationOnFailoverHost(vmodl.RuntimeFault):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
+    @property
+    def hostname(self) -> str: ...
+    @hostname.setter
+    def hostname(self, value: str):
+        self._hostname = value
 
 
-    class NameArrayUplinkPortPolicy(DistributedVirtualSwitch.UplinkPortPolicy):
-        @property
-        def uplinkPortName(self) -> List[str]: ...
+class DisconnectedHostsBlockingEVC(EVCConfigFault): ...
 
 
-    class NetworkResourceManagementCapability(vmodl.DynamicData):
-        @property
-        def networkResourceManagementSupported(self) -> bool: ...
-        @property
-        def networkResourcePoolHighShareValue(self) -> int: ...
-        @property
-        def qosSupported(self) -> bool: ...
-        @property
-        def userDefinedNetworkResourcePoolsSupported(self) -> bool: ...
-        @property
-        def networkResourceControlVersion3Supported(self) -> bool: ...
-        @property
-        def userDefinedInfraTrafficPoolSupported(self) -> bool: ...
+class DiskHasPartitions(VsanDiskFault): ...
 
 
-    class ResourceRuntimeInfo(vmodl.DynamicData):
-        @property
-        def capacity(self) -> int: ...
-        @property
-        def usage(self) -> int: ...
-        @property
-        def available(self) -> int: ...
-        @property
-        def allocatedResource(self) -> List[dvs.VmVnicNetworkResourcePool.VnicAllocatedResource]: ...
-        @property
-        def vmVnicNetworkResourcePoolRuntime(self) -> List[dvs.VmVnicNetworkResourcePool.RuntimeInfo]: ...
+class DiskIsLastRemainingNonSSD(VsanDiskFault): ...
 
 
-    class RollbackCapability(vmodl.DynamicData):
-        @property
-        def rollbackSupported(self) -> bool: ...
+class DiskIsNonLocal(VsanDiskFault): ...
 
 
-    class RuntimeInfo(vmodl.DynamicData):
-        @property
-        def hostMemberRuntime(self) -> List[dvs.HostMember.RuntimeInfo]: ...
-        @property
-        def resourceRuntimeInfo(self) -> DistributedVirtualSwitch.ResourceRuntimeInfo: ...
+class DiskIsUSB(VsanDiskFault): ...
 
 
-    class SwitchPolicy(vmodl.DynamicData):
-        @property
-        def autoPreInstallAllowed(self) -> bool: ...
-        @property
-        def autoUpgradeAllowed(self) -> bool: ...
-        @property
-        def partialUpgradeAllowed(self) -> bool: ...
+class DiskMoveTypeNotSupported(MigrationFault): ...
+
+
+class DiskNotSupported(VirtualHardwareCompatibilityIssue):
+    @property
+    def disk(self) -> int: ...
+    @disk.setter
+    def disk(self, value: int):
+        self._disk = value
+
 
+class DiskTooSmall(VsanDiskFault): ...
 
-    class UplinkPortPolicy(vmodl.DynamicData): ...
+
+class DomainNotFound(ActiveDirectoryFault):
+    @property
+    def domainName(self) -> str: ...
+    @domainName.setter
+    def domainName(self, value: str):
+        self._domainName = value
 
 
-    class HostInfrastructureTrafficClass(Enum):
-        management = "management"
-        faultTolerance = "faulttolerance"
-        vmotion = "vmotion"
-        virtualMachine = "virtualmachine"
-        iSCSI = "iscsi"
-        nfs = "nfs"
-        hbr = "hbr"
-        vsan = "vsan"
-        vdp = "vdp"
-        backupNfc = "backupnfc"
-        nvmetcp = "nvmetcp"
+class DrsDisabledOnVm(VimFault): ...
+
+
+class DrsVmotionIncompatibleFault(VirtualHardwareCompatibilityIssue):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class NetworkResourceControlVersion(Enum):
-        version2 = "version2"
-        version3 = "version3"
+class DuplicateDisks(VsanDiskFault): ...
 
 
-    class NicTeamingPolicyMode(Enum):
-        loadbalance_ip = "loadbalance_ip"
-        loadbalance_srcmac = "loadbalance_srcmac"
-        loadbalance_srcid = "loadbalance_srcid"
-        failover_explicit = "failover_explicit"
-        loadbalance_loadbased = "loadbalance_loadbased"
+class DuplicateName(VimFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+    @property
+    def object(self) -> ManagedObject: ...
+    @object.setter
+    def object(self, value: ManagedObject):
+        self._object = value
 
 
-    class ProductSpecOperationType(Enum):
-        preInstall = "preinstall"
-        upgrade = "upgrade"
-        notifyAvailableUpgrade = "notifyavailableupgrade"
-        proceedWithUpgrade = "proceedwithupgrade"
-        updateBundleInfo = "updatebundleinfo"
+class DuplicateVsanNetworkInterface(VsanFault):
+    @property
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
 
-class EnvironmentBrowser(ManagedObject):
+class DvsApplyOperationFault(DvsFault):
     @property
-    def datastoreBrowser(self) -> host.DatastoreBrowser: ...
-    def QueryConfigOptionDescriptor(self) -> List[vm.ConfigOptionDescriptor]: ...
-    def QueryConfigOption(self, key: str, host: HostSystem) -> vm.ConfigOption: ...
-    def QueryConfigOptionEx(self, spec: EnvironmentBrowser.ConfigOptionQuerySpec) -> vm.ConfigOption: ...
-    def QueryConfigTarget(self, host: HostSystem) -> vm.ConfigTarget: ...
-    def QueryTargetCapabilities(self, host: HostSystem) -> host.Capability: ...
+    def objectFault(self) -> List[DvsApplyOperationFault.FaultOnObject]: ...
+    @objectFault.setter
+    def objectFault(self, value: List[DvsApplyOperationFault.FaultOnObject]):
+        self._objectFault = value
 
 
-    class ConfigOptionQuerySpec(vmodl.DynamicData):
+    class FaultOnObject(vmodl.DynamicData):
         @property
-        def key(self) -> str: ...
+        def objectId(self) -> str: ...
+        @objectId.setter
+        def objectId(self, value: str):
+            self._objectId = value
         @property
-        def host(self) -> HostSystem: ...
+        def type(self) -> type: ...
+        @type.setter
+        def type(self, value: type):
+            self._type = value
         @property
-        def guestId(self) -> List[str]: ...
+        def fault(self) -> vmodl.MethodFault: ...
+        @fault.setter
+        def fault(self, value: vmodl.MethodFault):
+            self._fault = value
 
 
-class ExtensibleManagedObject(ManagedObject):
+class DvsFault(VimFault): ...
+
+
+class DvsNotAuthorized(DvsFault):
     @property
-    def value(self) -> List[CustomFieldsManager.Value]: ...
+    def sessionExtensionKey(self) -> str: ...
+    @sessionExtensionKey.setter
+    def sessionExtensionKey(self, value: str):
+        self._sessionExtensionKey = value
     @property
-    def availableField(self) -> List[CustomFieldsManager.FieldDef]: ...
-    def SetCustomValue(self, key: str, value: str) -> NoneType: ...
+    def dvsExtensionKey(self) -> str: ...
+    @dvsExtensionKey.setter
+    def dvsExtensionKey(self, value: str):
+        self._dvsExtensionKey = value
 
 
-class ExtensionManager(ManagedObject):
+class DvsOperationBulkFault(DvsFault):
     @property
-    def extensionList(self) -> List[Extension]: ...
-    def UnregisterExtension(self, extensionKey: str) -> NoneType: ...
-    def FindExtension(self, extensionKey: str) -> Extension: ...
-    def RegisterExtension(self, extension: Extension) -> NoneType: ...
-    def UpdateExtension(self, extension: Extension) -> NoneType: ...
-    def GetPublicKey(self) -> str: ...
-    def SetPublicKey(self, extensionKey: str, publicKey: str) -> NoneType: ...
-    def SetCertificate(self, extensionKey: str, certificatePem: str) -> NoneType: ...
-    def QueryManagedBy(self, extensionKey: str) -> List[ManagedEntity]: ...
-    def QueryExtensionIpAllocationUsage(self, extensionKeys: List[str]) -> List[ExtensionManager.IpAllocationUsage]: ...
+    def hostFault(self) -> List[DvsOperationBulkFault.FaultOnHost]: ...
+    @hostFault.setter
+    def hostFault(self, value: List[DvsOperationBulkFault.FaultOnHost]):
+        self._hostFault = value
 
 
-    class IpAllocationUsage(vmodl.DynamicData):
+    class FaultOnHost(vmodl.DynamicData):
         @property
-        def extensionKey(self) -> str: ...
+        def host(self) -> vim.HostSystem: ...
+        @host.setter
+        def host(self, value: vim.HostSystem):
+            self._host = value
         @property
-        def numAddresses(self) -> int: ...
+        def fault(self) -> vmodl.MethodFault: ...
+        @fault.setter
+        def fault(self, value: vmodl.MethodFault):
+            self._fault = value
 
 
-class FileManager(ManagedObject):
-    def MoveFile(self, sourceName: str, sourceDatacenter: Datacenter, destinationName: str, destinationDatacenter: Datacenter, force: bool) -> Task: ...
-    def CopyFile(self, sourceName: str, sourceDatacenter: Datacenter, destinationName: str, destinationDatacenter: Datacenter, force: bool) -> Task: ...
-    def DeleteFile(self, name: str, datacenter: Datacenter) -> Task: ...
-    def MakeDirectory(self, name: str, datacenter: Datacenter, createParentDirectories: bool) -> NoneType: ...
-    def ChangeOwner(self, name: str, datacenter: Datacenter, owner: str) -> NoneType: ...
+class DvsScopeViolated(DvsFault):
+    @property
+    def scope(self) -> List[vim.ManagedEntity]: ...
+    @scope.setter
+    def scope(self, value: List[vim.ManagedEntity]):
+        self._scope = value
+    @property
+    def entity(self) -> vim.ManagedEntity: ...
+    @entity.setter
+    def entity(self, value: vim.ManagedEntity):
+        self._entity = value
 
 
-class Folder(ManagedEntity):
+class EVCAdmissionFailed(NotSupportedHostInCluster):
     @property
-    def childType(self) -> List[type]: ...
+    def faults(self) -> List[vmodl.MethodFault]: ...
+    @faults.setter
+    def faults(self, value: List[vmodl.MethodFault]):
+        self._faults = value
+
+
+class EVCAdmissionFailedCPUFeaturesForMode(EVCAdmissionFailed):
     @property
-    def childEntity(self) -> List[ManagedEntity]: ...
+    def currentEVCModeKey(self) -> str: ...
+    @currentEVCModeKey.setter
+    def currentEVCModeKey(self, value: str):
+        self._currentEVCModeKey = value
+
+
+class EVCAdmissionFailedCPUModel(EVCAdmissionFailed): ...
+
+
+class EVCAdmissionFailedCPUModelForMode(EVCAdmissionFailed):
     @property
-    def namespace(self) -> str: ...
-    def CreateFolder(self, name: str) -> Folder: ...
-    def MoveInto(self, list: List[ManagedEntity]) -> Task: ...
-    def CreateVm(self, config: vm.ConfigSpec, pool: ResourcePool, host: HostSystem) -> Task: ...
-    def RegisterVm(self, path: str, name: str, asTemplate: bool, pool: ResourcePool, host: HostSystem) -> Task: ...
-    def CreateCluster(self, name: str, spec: cluster.ConfigSpec) -> ClusterComputeResource: ...
-    def CreateClusterEx(self, name: str, spec: cluster.ConfigSpecEx) -> ClusterComputeResource: ...
-    def AddStandaloneHost(self, spec: host.ConnectSpec, compResSpec: ComputeResource.ConfigSpec, addConnected: bool, license: str) -> Task: ...
-    def CreateDatacenter(self, name: str) -> Datacenter: ...
-    def UnregisterAndDestroy(self) -> Task: ...
-    def CreateDistributedVirtualSwitch(self, spec: DistributedVirtualSwitch.CreateSpec) -> Task: ...
-    def CreateStoragePod(self, name: str) -> StoragePod: ...
-    def BatchAddStandaloneHosts(self, newHosts: List[Folder.NewHostSpec], compResSpec: ComputeResource.ConfigSpec, addConnected: bool) -> Task: ...
-    def BatchAddHostsToCluster(self, cluster: ClusterComputeResource, newHosts: List[Folder.NewHostSpec], existingHosts: List[HostSystem], compResSpec: ComputeResource.ConfigSpec, desiredState: str) -> Task: ...
+    def currentEVCModeKey(self) -> str: ...
+    @currentEVCModeKey.setter
+    def currentEVCModeKey(self, value: str):
+        self._currentEVCModeKey = value
 
 
-    class BatchAddHostsToClusterResult(vmodl.DynamicData):
-        @property
-        def hostsAddedToCluster(self) -> List[HostSystem]: ...
-        @property
-        def hostsFailedInventoryAdd(self) -> List[Folder.FailedHostResult]: ...
-        @property
-        def hostsFailedMoveToCluster(self) -> List[Folder.FailedHostResult]: ...
+class EVCAdmissionFailedCPUVendor(EVCAdmissionFailed):
+    @property
+    def clusterCPUVendor(self) -> str: ...
+    @clusterCPUVendor.setter
+    def clusterCPUVendor(self, value: str):
+        self._clusterCPUVendor = value
+    @property
+    def hostCPUVendor(self) -> str: ...
+    @hostCPUVendor.setter
+    def hostCPUVendor(self, value: str):
+        self._hostCPUVendor = value
 
 
-    class BatchAddStandaloneHostsResult(vmodl.DynamicData):
-        @property
-        def addedHosts(self) -> List[HostSystem]: ...
-        @property
-        def hostsFailedInventoryAdd(self) -> List[Folder.FailedHostResult]: ...
+class EVCAdmissionFailedCPUVendorUnknown(EVCAdmissionFailed): ...
 
 
-    class FailedHostResult(vmodl.DynamicData):
-        @property
-        def hostName(self) -> str: ...
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def context(self) -> vmodl.LocalizableMessage: ...
-        @property
-        def fault(self) -> vmodl.MethodFault: ...
+class EVCAdmissionFailedHostDisconnected(EVCAdmissionFailed): ...
 
 
-    class NewHostSpec(vmodl.DynamicData):
-        @property
-        def hostCnxSpec(self) -> host.ConnectSpec: ...
-        @property
-        def esxLicense(self) -> str: ...
+class EVCAdmissionFailedHostSoftware(EVCAdmissionFailed): ...
 
 
-    class DesiredHostState(Enum):
-        maintenance = "maintenance"
-        non_maintenance = "non_maintenance"
+class EVCAdmissionFailedHostSoftwareForMode(EVCAdmissionFailed): ...
 
 
-class HealthUpdateManager(ManagedObject):
-    def RegisterProvider(self, name: str, healthUpdateInfo: List[HealthUpdateInfo]) -> str: ...
-    def UnregisterProvider(self, providerId: str) -> NoneType: ...
-    def QueryProviderList(self) -> List[str]: ...
-    def HasProvider(self, id: str) -> bool: ...
-    def QueryProviderName(self, id: str) -> str: ...
-    def QueryHealthUpdateInfos(self, providerId: str) -> List[HealthUpdateInfo]: ...
-    def AddMonitoredEntities(self, providerId: str, entities: List[ManagedEntity]) -> NoneType: ...
-    def RemoveMonitoredEntities(self, providerId: str, entities: List[ManagedEntity]) -> NoneType: ...
-    def QueryMonitoredEntities(self, providerId: str) -> List[ManagedEntity]: ...
-    def HasMonitoredEntity(self, providerId: str, entity: ManagedEntity) -> bool: ...
-    def QueryUnmonitoredHosts(self, providerId: str, cluster: ClusterComputeResource) -> List[HostSystem]: ...
-    def PostHealthUpdates(self, providerId: str, updates: List[HealthUpdate]) -> NoneType: ...
-    def QueryHealthUpdates(self, providerId: str) -> List[HealthUpdate]: ...
-    def AddFilter(self, providerId: str, filterName: str, infoIds: List[str]) -> str: ...
-    def QueryFilterList(self, providerId: str) -> List[str]: ...
-    def QueryFilterName(self, filterId: str) -> str: ...
-    def QueryFilterInfoIds(self, filterId: str) -> List[str]: ...
-    def QueryFilterEntities(self, filterId: str) -> List[ManagedEntity]: ...
-    def AddFilterEntities(self, filterId: str, entities: List[ManagedEntity]) -> NoneType: ...
-    def RemoveFilterEntities(self, filterId: str, entities: List[ManagedEntity]) -> NoneType: ...
-    def RemoveFilter(self, filterId: str) -> NoneType: ...
+class EVCAdmissionFailedVmActive(EVCAdmissionFailed): ...
 
 
-class HistoryCollector(ManagedObject):
+class EVCConfigFault(VimFault):
     @property
-    def filter(self) -> object: ...
-    def SetLatestPageSize(self, maxCount: int) -> NoneType: ...
-    def Rewind(self) -> NoneType: ...
-    def Reset(self) -> NoneType: ...
-    def Remove(self) -> NoneType: ...
+    def faults(self) -> List[vmodl.MethodFault]: ...
+    @faults.setter
+    def faults(self, value: List[vmodl.MethodFault]):
+        self._faults = value
 
 
-class HostSystem(ManagedEntity):
-    @property
-    def runtime(self) -> host.RuntimeInfo: ...
+class EVCModeIllegalByVendor(EVCConfigFault):
     @property
-    def summary(self) -> host.Summary: ...
+    def clusterCPUVendor(self) -> str: ...
+    @clusterCPUVendor.setter
+    def clusterCPUVendor(self, value: str):
+        self._clusterCPUVendor = value
     @property
-    def hardware(self) -> host.HardwareInfo: ...
+    def modeCPUVendor(self) -> str: ...
+    @modeCPUVendor.setter
+    def modeCPUVendor(self, value: str):
+        self._modeCPUVendor = value
+
+
+class EVCModeUnsupportedByHosts(EVCConfigFault):
     @property
-    def capability(self) -> host.Capability: ...
+    def evcMode(self) -> str: ...
+    @evcMode.setter
+    def evcMode(self, value: str):
+        self._evcMode = value
     @property
-    def licensableResource(self) -> LicenseManager.LicensableResourceInfo: ...
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
     @property
-    def remediationState(self) -> HostSystem.RemediationState: ...
+    def hostName(self) -> List[str]: ...
+    @hostName.setter
+    def hostName(self, value: List[str]):
+        self._hostName = value
+
+
+class EVCUnsupportedByHostHardware(EVCConfigFault):
     @property
-    def precheckRemediationResult(self) -> profile.host.ProfileManager.ApplyHostConfigSpec: ...
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
     @property
-    def remediationResult(self) -> profile.host.ProfileManager.ApplyHostConfigResult: ...
+    def hostName(self) -> List[str]: ...
+    @hostName.setter
+    def hostName(self, value: List[str]):
+        self._hostName = value
+
+
+class EVCUnsupportedByHostSoftware(EVCConfigFault):
     @property
-    def complianceCheckState(self) -> HostSystem.ComplianceCheckState: ...
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
     @property
-    def complianceCheckResult(self) -> profile.ComplianceResult: ...
+    def hostName(self) -> List[str]: ...
+    @hostName.setter
+    def hostName(self, value: List[str]):
+        self._hostName = value
+
+
+class EightHostLimitViolated(VmConfigFault): ...
+
+
+class EncryptionKeyRequired(InvalidState):
     @property
-    def configManager(self) -> host.ConfigManager: ...
+    def requiredKey(self) -> List[vim.encryption.CryptoKeyId]: ...
+    @requiredKey.setter
+    def requiredKey(self, value: List[vim.encryption.CryptoKeyId]):
+        self._requiredKey = value
+
+
+class ExpiredAddonLicense(ExpiredFeatureLicense): ...
+
+
+class ExpiredEditionLicense(ExpiredFeatureLicense): ...
+
+
+class ExpiredFeatureLicense(NotEnoughLicenses):
     @property
-    def config(self) -> host.ConfigInfo: ...
+    def feature(self) -> str: ...
+    @feature.setter
+    def feature(self, value: str):
+        self._feature = value
     @property
-    def vm(self) -> List[VirtualMachine]: ...
+    def count(self) -> int: ...
+    @count.setter
+    def count(self, value: int):
+        self._count = value
     @property
-    def datastore(self) -> List[Datastore]: ...
+    def expirationDate(self) -> datetime: ...
+    @expirationDate.setter
+    def expirationDate(self, value: datetime):
+        self._expirationDate = value
+
+
+class ExtendedFault(VimFault):
     @property
-    def network(self) -> List[Network]: ...
+    def faultTypeId(self) -> str: ...
+    @faultTypeId.setter
+    def faultTypeId(self, value: str):
+        self._faultTypeId = value
     @property
-    def datastoreBrowser(self) -> host.DatastoreBrowser: ...
+    def data(self) -> List[vim.KeyValue]: ...
+    @data.setter
+    def data(self, value: List[vim.KeyValue]):
+        self._data = value
+
+
+class FailToEnableSPBM(NotEnoughLicenses):
     @property
-    def systemResources(self) -> host.SystemResourceInfo: ...
+    def cs(self) -> vim.ComputeResource: ...
+    @cs.setter
+    def cs(self, value: vim.ComputeResource):
+        self._cs = value
     @property
-    def answerFileValidationState(self) -> profile.host.AnswerFileStatusResult: ...
+    def csName(self) -> str: ...
+    @csName.setter
+    def csName(self, value: str):
+        self._csName = value
     @property
-    def answerFileValidationResult(self) -> profile.host.AnswerFileStatusResult: ...
-    def QueryTpmAttestationReport(self) -> host.TpmAttestationReport: ...
-    def QueryConnectionInfo(self) -> host.ConnectInfo: ...
-    def UpdateSystemResources(self, resourceInfo: host.SystemResourceInfo) -> NoneType: ...
-    def UpdateSystemSwapConfiguration(self, sysSwapConfig: host.SystemSwapConfiguration) -> NoneType: ...
-    def Reconnect(self, cnxSpec: host.ConnectSpec, reconnectSpec: HostSystem.ReconnectSpec) -> Task: ...
-    def Disconnect(self) -> Task: ...
-    def EnterMaintenanceMode(self, timeout: int, evacuatePoweredOffVms: bool, maintenanceSpec: host.MaintenanceSpec) -> Task: ...
-    def ExitMaintenanceMode(self, timeout: int) -> Task: ...
-    def Reboot(self, force: bool) -> Task: ...
-    def Shutdown(self, force: bool) -> Task: ...
-    def EnterStandbyMode(self, timeoutSec: int, evacuatePoweredOffVms: bool) -> Task: ...
-    def ExitStandbyMode(self, timeoutSec: int) -> Task: ...
-    def QueryOverhead(self, memorySize: long, videoRamSize: int, numVcpus: int) -> long: ...
-    def QueryOverheadEx(self, vmConfigInfo: vm.ConfigInfo) -> long: ...
-    def ReconfigureDAS(self) -> Task: ...
-    def UpdateFlags(self, flagInfo: host.FlagInfo) -> NoneType: ...
-    def EnterLockdownMode(self) -> NoneType: ...
-    def ExitLockdownMode(self) -> NoneType: ...
-    def AcquireCimServicesTicket(self) -> HostServiceTicket: ...
-    def UpdateIpmi(self, ipmiInfo: host.IpmiInfo) -> NoneType: ...
-    def RetrieveHardwareUptime(self) -> long: ...
-    def PrepareCrypto(self) -> NoneType: ...
-    def EnableCrypto(self, keyPlain: encryption.CryptoKeyPlain) -> NoneType: ...
-    def ConfigureCryptoKey(self, keyId: encryption.CryptoKeyId) -> NoneType: ...
-    def QueryProductLockerLocation(self) -> str: ...
-    def UpdateProductLockerLocation(self, path: str) -> Task: ...
-    def RetrieveFreeEpcMemory(self) -> long: ...
+    def hostLicenseStates(self) -> List[vim.ComputeResource.HostSPBMLicenseInfo]: ...
+    @hostLicenseStates.setter
+    def hostLicenseStates(self, value: List[vim.ComputeResource.HostSPBMLicenseInfo]):
+        self._hostLicenseStates = value
 
 
-    class ComplianceCheckState(vmodl.DynamicData):
-        @property
-        def state(self) -> str: ...
-        @property
-        def checkTime(self) -> datetime: ...
+class FailToLockFaultToleranceVMs(vmodl.RuntimeFault):
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
+    @property
+    def alreadyLockedVm(self) -> vim.VirtualMachine: ...
+    @alreadyLockedVm.setter
+    def alreadyLockedVm(self, value: vim.VirtualMachine):
+        self._alreadyLockedVm = value
 
 
-    class ReconnectSpec(vmodl.DynamicData):
-        @property
-        def syncState(self) -> bool: ...
+class FaultToleranceAntiAffinityViolated(MigrationFault):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class RemediationState(vmodl.DynamicData):
-        @property
-        def state(self) -> str: ...
-        @property
-        def operationTime(self) -> datetime: ...
+class FaultToleranceCannotEditMem(VmConfigFault):
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
 
 
-    class ConnectionState(Enum):
-        connected = "connected"
-        notResponding = "notresponding"
-        disconnected = "disconnected"
+class FaultToleranceCpuIncompatible(CpuIncompatible):
+    @property
+    def model(self) -> bool: ...
+    @model.setter
+    def model(self, value: bool):
+        self._model = value
+    @property
+    def family(self) -> bool: ...
+    @family.setter
+    def family(self, value: bool):
+        self._family = value
+    @property
+    def stepping(self) -> bool: ...
+    @stepping.setter
+    def stepping(self, value: bool):
+        self._stepping = value
 
 
-    class CryptoState(Enum):
-        incapable = "incapable"
-        prepared = "prepared"
-        safe = "safe"
-        pendingIncapable = "pendingincapable"
+class FaultToleranceNeedsThickDisk(MigrationFault):
+    @property
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class PowerState(Enum):
-        poweredOn = "poweredon"
-        poweredOff = "poweredoff"
-        standBy = "standby"
-        unknown = "unknown"
+class FaultToleranceNotLicensed(VmFaultToleranceIssue):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-    class StandbyMode(Enum):
-        entering = "entering"
-        exiting = "exiting"
-        in = "in"
-        none = "none"
+class FaultToleranceNotSameBuild(MigrationFault):
+    @property
+    def build(self) -> str: ...
+    @build.setter
+    def build(self, value: str):
+        self._build = value
 
 
-class HttpNfcLease(ManagedObject):
-    @property
-    def initializeProgress(self) -> int: ...
-    @property
-    def transferProgress(self) -> int: ...
-    @property
-    def mode(self) -> str: ...
+class FaultTolerancePrimaryPowerOnNotAttempted(VmFaultToleranceIssue):
     @property
-    def capabilities(self) -> HttpNfcLease.Capabilities: ...
+    def secondaryVm(self) -> vim.VirtualMachine: ...
+    @secondaryVm.setter
+    def secondaryVm(self, value: vim.VirtualMachine):
+        self._secondaryVm = value
     @property
-    def info(self) -> HttpNfcLease.Info: ...
+    def primaryVm(self) -> vim.VirtualMachine: ...
+    @primaryVm.setter
+    def primaryVm(self, value: vim.VirtualMachine):
+        self._primaryVm = value
+
+
+class FaultToleranceVmNotDasProtected(VimFault):
     @property
-    def state(self) -> HttpNfcLease.State: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def error(self) -> vmodl.MethodFault: ...
-    def GetManifest(self) -> List[HttpNfcLease.ManifestEntry]: ...
-    def SetManifestChecksumType(self, deviceUrlsToChecksumTypes: List[KeyValue]) -> NoneType: ...
-    def Complete(self) -> NoneType: ...
-    def Abort(self, fault: vmodl.MethodFault) -> NoneType: ...
-    def Progress(self, percent: int) -> NoneType: ...
-    def PullFromUrls(self, files: List[HttpNfcLease.SourceFile]) -> Task: ...
-    def ProbeUrls(self, files: List[HttpNfcLease.SourceFile], timeout: int) -> List[HttpNfcLease.ProbeResult]: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class Capabilities(vmodl.DynamicData):
-        @property
-        def pullModeSupported(self) -> bool: ...
-        @property
-        def corsSupported(self) -> bool: ...
+class FcoeFault(VimFault): ...
 
 
-    class DatastoreLeaseInfo(vmodl.DynamicData):
-        @property
-        def datastoreKey(self) -> str: ...
-        @property
-        def hosts(self) -> List[HttpNfcLease.HostInfo]: ...
+class FcoeFaultPnicHasNoPortSet(FcoeFault):
+    @property
+    def nicDevice(self) -> str: ...
+    @nicDevice.setter
+    def nicDevice(self, value: str):
+        self._nicDevice = value
 
 
-    class DeviceUrl(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def importKey(self) -> str: ...
-        @property
-        def url(self) -> str: ...
-        @property
-        def sslThumbprint(self) -> str: ...
-        @property
-        def disk(self) -> bool: ...
-        @property
-        def targetId(self) -> str: ...
-        @property
-        def datastoreKey(self) -> str: ...
-        @property
-        def fileSize(self) -> long: ...
+class FeatureRequirementsNotMet(VirtualHardwareCompatibilityIssue):
+    @property
+    def featureRequirement(self) -> List[vim.vm.FeatureRequirement]: ...
+    @featureRequirement.setter
+    def featureRequirement(self, value: List[vim.vm.FeatureRequirement]):
+        self._featureRequirement = value
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class HostInfo(vmodl.DynamicData):
-        @property
-        def url(self) -> str: ...
-        @property
-        def sslThumbprint(self) -> str: ...
+class FileAlreadyExists(FileFault): ...
 
 
-    class ManifestEntry(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def sha1(self) -> str: ...
-        @property
-        def checksum(self) -> str: ...
-        @property
-        def checksumType(self) -> str: ...
-        @property
-        def size(self) -> long: ...
-        @property
-        def disk(self) -> bool: ...
-        @property
-        def capacity(self) -> long: ...
-        @property
-        def populatedSize(self) -> long: ...
+class FileBackedPortNotSupported(DeviceNotSupported): ...
 
 
-        class ChecksumType(Enum):
-            sha1 = "sha1"
-            sha256 = "sha256"
+class FileFault(VimFault):
+    @property
+    def file(self) -> str: ...
+    @file.setter
+    def file(self, value: str):
+        self._file = value
 
 
-    class ProbeResult(vmodl.DynamicData):
-        @property
-        def serverAccessible(self) -> bool: ...
+class FileLocked(FileFault): ...
 
 
-    class SourceFile(vmodl.DynamicData):
-        @property
-        def targetDeviceId(self) -> str: ...
-        @property
-        def url(self) -> str: ...
-        @property
-        def memberName(self) -> str: ...
-        @property
-        def create(self) -> bool: ...
-        @property
-        def sslThumbprint(self) -> str: ...
-        @property
-        def httpHeaders(self) -> List[KeyValue]: ...
-        @property
-        def size(self) -> long: ...
+class FileNameTooLong(FileFault): ...
 
 
-    class Mode(Enum):
-        pushOrGet = "pushorget"
-        pull = "pull"
+class FileNotFound(FileFault): ...
 
 
-class IoFilterManager(ManagedObject):
-    def InstallIoFilter(self, vibUrl: str, compRes: ComputeResource) -> Task: ...
-    def UninstallIoFilter(self, filterId: str, compRes: ComputeResource) -> Task: ...
-    def UpgradeIoFilter(self, filterId: str, compRes: ComputeResource, vibUrl: str) -> Task: ...
-    def QueryIssue(self, filterId: str, compRes: ComputeResource) -> IoFilterManager.QueryIssueResult: ...
-    def QueryIoFilterInfo(self, compRes: ComputeResource) -> List[IoFilterManager.ClusterIoFilterInfo]: ...
-    def ResolveInstallationErrorsOnHost(self, filterId: str, host: HostSystem) -> Task: ...
-    def ResolveInstallationErrorsOnCluster(self, filterId: str, cluster: ClusterComputeResource) -> Task: ...
-    def QueryDisksUsingFilter(self, filterId: str, compRes: ComputeResource) -> List[vm.device.VirtualDiskId]: ...
+class FileNotWritable(FileFault): ...
 
 
-    class ClusterIoFilterInfo(IoFilterManager.IoFilterInfo):
-        @property
-        def opType(self) -> str: ...
-        @property
-        def vibUrl(self) -> str: ...
+class FileTooLarge(FileFault):
+    @property
+    def datastore(self) -> str: ...
+    @datastore.setter
+    def datastore(self, value: str):
+        self._datastore = value
+    @property
+    def fileSize(self) -> long: ...
+    @fileSize.setter
+    def fileSize(self, value: long):
+        self._fileSize = value
+    @property
+    def maxFileSize(self) -> long: ...
+    @maxFileSize.setter
+    def maxFileSize(self, value: long):
+        self._maxFileSize = value
 
 
-    class HostIoFilterInfo(IoFilterManager.IoFilterInfo):
-        @property
-        def available(self) -> bool: ...
+class FilesystemQuiesceFault(SnapshotFault): ...
 
 
-    class IoFilterInfo(vmodl.DynamicData):
-        @property
-        def id(self) -> str: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def vendor(self) -> str: ...
-        @property
-        def version(self) -> str: ...
-        @property
-        def type(self) -> str: ...
-        @property
-        def summary(self) -> str: ...
-        @property
-        def releaseDate(self) -> str: ...
+class FilterInUse(ResourceInUse):
+    @property
+    def disk(self) -> List[vim.vm.device.VirtualDiskId]: ...
+    @disk.setter
+    def disk(self, value: List[vim.vm.device.VirtualDiskId]):
+        self._disk = value
 
 
-    class QueryIssueResult(vmodl.DynamicData):
-        @property
-        def opType(self) -> str: ...
-        @property
-        def hostIssue(self) -> List[IoFilterManager.QueryIssueResult.HostIssue]: ...
+class FtIssuesOnHost(VmFaultToleranceIssue):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+    @property
+    def errors(self) -> List[vmodl.MethodFault]: ...
+    @errors.setter
+    def errors(self, value: List[vmodl.MethodFault]):
+        self._errors = value
 
 
-        class HostIssue(vmodl.DynamicData):
-            @property
-            def host(self) -> HostSystem: ...
-            @property
-            def issue(self) -> List[vmodl.MethodFault]: ...
+    class HostSelectionType(Enum):
+        user = "user"
+        vc = "vc"
+        drs = "drs"
 
 
-    class IoFilterType(Enum):
-        cache = "cache"
-        replication = "replication"
-        encryption = "encryption"
-        compression = "compression"
-        inspection = "inspection"
-        datastoreIoControl = "datastoreiocontrol"
-        dataProvider = "dataprovider"
-        dataCapture = "datacapture"
+class FullStorageVMotionNotSupported(MigrationFeatureNotSupported): ...
 
 
-    class OperationType(Enum):
-        install = "install"
-        uninstall = "uninstall"
-        upgrade = "upgrade"
+class GatewayConnectFault(HostConnectFault):
+    @property
+    def gatewayType(self) -> str: ...
+    @gatewayType.setter
+    def gatewayType(self, value: str):
+        self._gatewayType = value
+    @property
+    def gatewayId(self) -> str: ...
+    @gatewayId.setter
+    def gatewayId(self, value: str):
+        self._gatewayId = value
+    @property
+    def gatewayInfo(self) -> str: ...
+    @gatewayInfo.setter
+    def gatewayInfo(self, value: str):
+        self._gatewayInfo = value
+    @property
+    def details(self) -> vmodl.LocalizableMessage: ...
+    @details.setter
+    def details(self, value: vmodl.LocalizableMessage):
+        self._details = value
 
 
-class IpPoolManager(ManagedObject):
-    def QueryIpPools(self, dc: Datacenter) -> List[vApp.IpPool]: ...
-    def CreateIpPool(self, dc: Datacenter, pool: vApp.IpPool) -> int: ...
-    def UpdateIpPool(self, dc: Datacenter, pool: vApp.IpPool) -> NoneType: ...
-    def DestroyIpPool(self, dc: Datacenter, id: int, force: bool) -> NoneType: ...
-    def AllocateIpv4Address(self, dc: Datacenter, poolId: int, allocationId: str) -> str: ...
-    def AllocateIpv6Address(self, dc: Datacenter, poolId: int, allocationId: str) -> str: ...
-    def ReleaseIpAllocation(self, dc: Datacenter, poolId: int, allocationId: str) -> NoneType: ...
-    def QueryIPAllocations(self, dc: Datacenter, poolId: int, extensionKey: str) -> List[IpPoolManager.IpAllocation]: ...
+class GatewayHostNotReachable(GatewayToHostConnectFault): ...
 
 
-    class IpAllocation(vmodl.DynamicData):
-        @property
-        def ipAddress(self) -> str: ...
-        @property
-        def allocationId(self) -> str: ...
+class GatewayNotFound(GatewayConnectFault): ...
 
 
-class LicenseAssignmentManager(ManagedObject):
-    def UpdateAssignedLicense(self, entity: str, licenseKey: str, entityDisplayName: str) -> LicenseManager.LicenseInfo: ...
-    def RemoveAssignedLicense(self, entityId: str) -> NoneType: ...
-    def QueryAssignedLicenses(self, entityId: str) -> List[LicenseAssignmentManager.LicenseAssignment]: ...
+class GatewayNotReachable(GatewayConnectFault): ...
 
 
-    class LicenseAssignment(vmodl.DynamicData):
-        @property
-        def entityId(self) -> str: ...
-        @property
-        def scope(self) -> str: ...
-        @property
-        def entityDisplayName(self) -> str: ...
-        @property
-        def assignedLicense(self) -> LicenseManager.LicenseInfo: ...
-        @property
-        def properties(self) -> List[vmodl.KeyAnyValue]: ...
+class GatewayOperationRefused(GatewayConnectFault): ...
 
 
-class LicenseManager(ManagedObject):
+class GatewayToHostAuthFault(GatewayToHostConnectFault):
     @property
-    def source(self) -> LicenseManager.LicenseSource: ...
+    def invalidProperties(self) -> List[str]: ...
+    @invalidProperties.setter
+    def invalidProperties(self, value: List[str]):
+        self._invalidProperties = value
     @property
-    def sourceAvailable(self) -> bool: ...
+    def missingProperties(self) -> List[str]: ...
+    @missingProperties.setter
+    def missingProperties(self, value: List[str]):
+        self._missingProperties = value
+
+
+class GatewayToHostConnectFault(GatewayConnectFault):
     @property
-    def diagnostics(self) -> LicenseManager.DiagnosticInfo: ...
+    def hostname(self) -> str: ...
+    @hostname.setter
+    def hostname(self, value: str):
+        self._hostname = value
     @property
-    def featureInfo(self) -> List[LicenseManager.FeatureInfo]: ...
+    def port(self) -> int: ...
+    @port.setter
+    def port(self, value: int):
+        self._port = value
+
+
+class GatewayToHostTrustVerifyFault(GatewayToHostConnectFault):
     @property
-    def licensedEdition(self) -> str: ...
+    def verificationToken(self) -> str: ...
+    @verificationToken.setter
+    def verificationToken(self, value: str):
+        self._verificationToken = value
     @property
-    def licenses(self) -> List[LicenseManager.LicenseInfo]: ...
+    def propertiesToVerify(self) -> List[vim.KeyValue]: ...
+    @propertiesToVerify.setter
+    def propertiesToVerify(self, value: List[vim.KeyValue]):
+        self._propertiesToVerify = value
+
+
+class GenericDrsFault(VimFault):
     @property
-    def licenseAssignmentManager(self) -> LicenseAssignmentManager: ...
+    def hostFaults(self) -> List[vmodl.MethodFault]: ...
+    @hostFaults.setter
+    def hostFaults(self, value: List[vmodl.MethodFault]):
+        self._hostFaults = value
+
+
+class GenericVmConfigFault(VmConfigFault):
     @property
-    def evaluation(self) -> LicenseManager.EvaluationInfo: ...
-    def QuerySupportedFeatures(self, host: HostSystem) -> List[LicenseManager.FeatureInfo]: ...
-    def QuerySourceAvailability(self, host: HostSystem) -> List[LicenseManager.AvailabilityInfo]: ...
-    def QueryUsage(self, host: HostSystem) -> LicenseManager.LicenseUsageInfo: ...
-    def SetEdition(self, host: HostSystem, featureKey: str) -> NoneType: ...
-    def CheckFeature(self, host: HostSystem, featureKey: str) -> bool: ...
-    def Enable(self, host: HostSystem, featureKey: str) -> bool: ...
-    def Disable(self, host: HostSystem, featureKey: str) -> bool: ...
-    def ConfigureSource(self, host: HostSystem, licenseSource: LicenseManager.LicenseSource) -> NoneType: ...
-    def UpdateLicense(self, licenseKey: str, labels: List[KeyValue]) -> LicenseManager.LicenseInfo: ...
-    def AddLicense(self, licenseKey: str, labels: List[KeyValue]) -> LicenseManager.LicenseInfo: ...
-    def RemoveLicense(self, licenseKey: str) -> NoneType: ...
-    def DecodeLicense(self, licenseKey: str) -> LicenseManager.LicenseInfo: ...
-    def UpdateLabel(self, licenseKey: str, labelKey: str, labelValue: str) -> NoneType: ...
-    def RemoveLabel(self, licenseKey: str, labelKey: str) -> NoneType: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
 
-    class AvailabilityInfo(vmodl.DynamicData):
-        @property
-        def feature(self) -> LicenseManager.FeatureInfo: ...
-        @property
-        def total(self) -> int: ...
-        @property
-        def available(self) -> int: ...
+class GuestAuthenticationChallenge(GuestOperationsFault):
+    @property
+    def serverChallenge(self) -> vim.vm.guest.GuestAuthentication: ...
+    @serverChallenge.setter
+    def serverChallenge(self, value: vim.vm.guest.GuestAuthentication):
+        self._serverChallenge = value
+    @property
+    def sessionID(self) -> long: ...
+    @sessionID.setter
+    def sessionID(self, value: long):
+        self._sessionID = value
 
 
-    class DiagnosticInfo(vmodl.DynamicData):
-        @property
-        def sourceLastChanged(self) -> datetime: ...
-        @property
-        def sourceLost(self) -> str: ...
-        @property
-        def sourceLatency(self) -> float: ...
-        @property
-        def licenseRequests(self) -> str: ...
-        @property
-        def licenseRequestFailures(self) -> str: ...
-        @property
-        def licenseFeatureUnknowns(self) -> str: ...
-        @property
-        def opState(self) -> LicenseManager.LicenseState: ...
-        @property
-        def lastStatusUpdate(self) -> datetime: ...
-        @property
-        def opFailureMessage(self) -> str: ...
+class GuestComponentsOutOfDate(GuestOperationsFault): ...
 
 
-    class EvaluationInfo(vmodl.DynamicData):
-        @property
-        def properties(self) -> List[vmodl.KeyAnyValue]: ...
+class GuestMultipleMappings(GuestOperationsFault): ...
 
 
-    class EvaluationLicense(LicenseManager.LicenseSource):
-        @property
-        def remainingHours(self) -> long: ...
+class GuestOperationsFault(VimFault): ...
 
 
-    class FeatureInfo(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def featureName(self) -> str: ...
-        @property
-        def featureDescription(self) -> str: ...
-        @property
-        def state(self) -> LicenseManager.FeatureInfo.State: ...
-        @property
-        def costUnit(self) -> str: ...
-        @property
-        def sourceRestriction(self) -> str: ...
-        @property
-        def dependentKey(self) -> List[str]: ...
-        @property
-        def edition(self) -> bool: ...
-        @property
-        def expiresOn(self) -> datetime: ...
+class GuestOperationsUnavailable(GuestOperationsFault): ...
 
 
-        class CostUnit(Enum):
-            host = "host"
-            cpuCore = "cpucore"
-            cpuPackage = "cpupackage"
-            server = "server"
-            vm = "vm"
+class GuestPermissionDenied(GuestOperationsFault): ...
 
 
-        class SourceRestriction(Enum):
-            unrestricted = "unrestricted"
-            served = "served"
-            file = "file"
+class GuestProcessNotFound(GuestOperationsFault):
+    @property
+    def pid(self) -> long: ...
+    @pid.setter
+    def pid(self, value: long):
+        self._pid = value
 
 
-    class LicensableResourceInfo(vmodl.DynamicData):
-        @property
-        def resource(self) -> List[vmodl.KeyAnyValue]: ...
+class GuestRegistryFault(GuestOperationsFault):
+    @property
+    def windowsSystemErrorCode(self) -> long: ...
+    @windowsSystemErrorCode.setter
+    def windowsSystemErrorCode(self, value: long):
+        self._windowsSystemErrorCode = value
 
 
-        class ResourceKey(Enum):
-            numCpuPackages = "numcpupackages"
-            numCpuCores = "numcpucores"
-            memorySize = "memorysize"
-            memoryForVms = "memoryforvms"
-            numVmsStarted = "numvmsstarted"
-            numVmsStarting = "numvmsstarting"
+class GuestRegistryKeyAlreadyExists(GuestRegistryKeyFault): ...
 
 
-    class LicenseInfo(vmodl.DynamicData):
-        @property
-        def licenseKey(self) -> str: ...
-        @property
-        def editionKey(self) -> str: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def total(self) -> int: ...
-        @property
-        def used(self) -> int: ...
-        @property
-        def costUnit(self) -> str: ...
-        @property
-        def properties(self) -> List[vmodl.KeyAnyValue]: ...
-        @property
-        def labels(self) -> List[KeyValue]: ...
+class GuestRegistryKeyFault(GuestRegistryFault):
+    @property
+    def keyName(self) -> str: ...
+    @keyName.setter
+    def keyName(self, value: str):
+        self._keyName = value
 
 
-    class LicenseServer(LicenseManager.LicenseSource):
-        @property
-        def licenseServer(self) -> str: ...
+class GuestRegistryKeyHasSubkeys(GuestRegistryKeyFault): ...
 
 
-    class LicenseSource(vmodl.DynamicData): ...
+class GuestRegistryKeyInvalid(GuestRegistryKeyFault): ...
 
 
-    class LicenseUsageInfo(vmodl.DynamicData):
-        @property
-        def source(self) -> LicenseManager.LicenseSource: ...
-        @property
-        def sourceAvailable(self) -> bool: ...
-        @property
-        def reservationInfo(self) -> List[LicenseManager.ReservationInfo]: ...
-        @property
-        def featureInfo(self) -> List[LicenseManager.FeatureInfo]: ...
+class GuestRegistryKeyParentVolatile(GuestRegistryKeyFault): ...
 
 
-    class LocalLicense(LicenseManager.LicenseSource):
-        @property
-        def licenseKeys(self) -> str: ...
+class GuestRegistryValueFault(GuestRegistryFault):
+    @property
+    def keyName(self) -> str: ...
+    @keyName.setter
+    def keyName(self, value: str):
+        self._keyName = value
+    @property
+    def valueName(self) -> str: ...
+    @valueName.setter
+    def valueName(self, value: str):
+        self._valueName = value
 
 
-    class ReservationInfo(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def state(self) -> LicenseManager.ReservationInfo.State: ...
-        @property
-        def required(self) -> int: ...
+class GuestRegistryValueNotFound(GuestRegistryValueFault): ...
 
 
-    class LicenseKey(Enum):
-        esxFull = "esxfull"
-        esxVmtn = "esxvmtn"
-        esxExpress = "esxexpress"
-        san = "san"
-        iscsi = "iscsi"
-        nas = "nas"
-        vsmp = "vsmp"
-        backup = "backup"
-        vc = "vc"
-        vcExpress = "vcexpress"
-        esxHost = "esxhost"
-        gsxHost = "gsxhost"
-        serverHost = "serverhost"
-        drsPower = "drspower"
-        vmotion = "vmotion"
-        drs = "drs"
-        das = "das"
+class HAErrorsAtDest(MigrationFault): ...
 
 
-    class LicenseState(Enum):
-        initializing = "initializing"
-        normal = "normal"
-        marginal = "marginal"
-        fault = "fault"
+class HeterogenousHostsBlockingEVC(EVCConfigFault): ...
 
 
-class LocalizationManager(ManagedObject):
+class HostAccessRestrictedToManagementServer(NotSupported):
     @property
-    def catalog(self) -> List[LocalizationManager.MessageCatalog]: ...
+    def managementServer(self) -> str: ...
+    @managementServer.setter
+    def managementServer(self, value: str):
+        self._managementServer = value
 
 
-    class MessageCatalog(vmodl.DynamicData):
-        @property
-        def moduleName(self) -> str: ...
-        @property
-        def catalogName(self) -> str: ...
-        @property
-        def locale(self) -> str: ...
-        @property
-        def catalogUri(self) -> str: ...
-        @property
-        def lastModified(self) -> datetime: ...
-        @property
-        def md5sum(self) -> str: ...
-        @property
-        def version(self) -> str: ...
+class HostConfigFailed(HostConfigFault):
+    @property
+    def failure(self) -> List[vmodl.MethodFault]: ...
+    @failure.setter
+    def failure(self, value: List[vmodl.MethodFault]):
+        self._failure = value
 
 
-class ManagedEntity(ExtensibleManagedObject):
-    @property
-    def parent(self) -> ManagedEntity: ...
-    @property
-    def customValue(self) -> List[CustomFieldsManager.Value]: ...
-    @property
-    def overallStatus(self) -> ManagedEntity.Status: ...
-    @property
-    def configStatus(self) -> ManagedEntity.Status: ...
-    @property
-    def configIssue(self) -> List[event.Event]: ...
-    @property
-    def effectiveRole(self) -> List[int]: ...
-    @property
-    def permission(self) -> List[AuthorizationManager.Permission]: ...
-    @property
-    def name(self) -> str: ...
-    @property
-    def disabledMethod(self) -> List[ManagedMethod]: ...
-    @property
-    def recentTask(self) -> List[Task]: ...
-    @property
-    def declaredAlarmState(self) -> List[alarm.AlarmState]: ...
-    @property
-    def triggeredAlarmState(self) -> List[alarm.AlarmState]: ...
-    @property
-    def alarmActionsEnabled(self) -> bool: ...
-    @property
-    def tag(self) -> List[Tag]: ...
-    def Reload(self) -> NoneType: ...
-    def Rename(self, newName: str) -> Task: ...
-    def Destroy(self) -> Task: ...
+class HostConfigFault(VimFault): ...
 
 
-    class Status(Enum):
-        gray = "gray"
-        green = "green"
-        yellow = "yellow"
-        red = "red"
+class HostConnectFault(VimFault): ...
 
 
-class Network(ManagedEntity):
+class HostHasComponentFailure(VimFault):
     @property
-    def summary(self) -> Network.Summary: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def host(self) -> List[HostSystem]: ...
+    def componentType(self) -> str: ...
+    @componentType.setter
+    def componentType(self, value: str):
+        self._componentType = value
     @property
-    def vm(self) -> List[VirtualMachine]: ...
-    def DestroyNetwork(self) -> NoneType: ...
+    def componentName(self) -> str: ...
+    @componentName.setter
+    def componentName(self, value: str):
+        self._componentName = value
 
 
-class OpaqueNetwork(Network):
-    @property
-    def capability(self) -> OpaqueNetwork.Capability: ...
-    @property
-    def extraConfig(self) -> List[option.OptionValue]: ...
+    class HostComponentType(Enum):
+        Datastore = "Datastore"
 
 
-class OverheadMemoryManager(ManagedObject):
-    def LookupVmOverheadMemory(self, vm: VirtualMachine, host: HostSystem) -> long: ...
+class HostInDomain(HostConfigFault): ...
 
 
-class OvfManager(ManagedObject):
+class HostIncompatibleForFaultTolerance(VmFaultToleranceIssue):
     @property
-    def ovfImportOption(self) -> List[OvfManager.OvfOptionInfo]: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def ovfExportOption(self) -> List[OvfManager.OvfOptionInfo]: ...
-    def ValidateHost(self, ovfDescriptor: str, host: HostSystem, vhp: OvfManager.ValidateHostParams) -> OvfManager.ValidateHostResult: ...
-    def ParseDescriptor(self, ovfDescriptor: str, pdp: OvfManager.ParseDescriptorParams) -> OvfManager.ParseDescriptorResult: ...
-    def CreateImportSpec(self, ovfDescriptor: str, resourcePool: ResourcePool, datastore: Datastore, cisp: OvfManager.CreateImportSpecParams) -> OvfManager.CreateImportSpecResult: ...
-    def CreateDescriptor(self, obj: ManagedEntity, cdp: OvfManager.CreateDescriptorParams) -> OvfManager.CreateDescriptorResult: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
 
-    class CommonParams(vmodl.DynamicData):
-        @property
-        def locale(self) -> str: ...
-        @property
-        def deploymentOption(self) -> str: ...
-        @property
-        def msgBundle(self) -> List[KeyValue]: ...
-        @property
-        def importOption(self) -> List[str]: ...
+class HostIncompatibleForRecordReplay(VimFault):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+    @property
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
 
-    class CreateDescriptorParams(vmodl.DynamicData):
-        @property
-        def ovfFiles(self) -> List[OvfManager.OvfFile]: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def description(self) -> str: ...
-        @property
-        def includeImageFiles(self) -> bool: ...
-        @property
-        def exportOption(self) -> List[str]: ...
-        @property
-        def snapshot(self) -> vm.Snapshot: ...
+class HostInventoryFull(NotEnoughLicenses):
+    @property
+    def capacity(self) -> int: ...
+    @capacity.setter
+    def capacity(self, value: int):
+        self._capacity = value
 
 
-    class CreateDescriptorResult(vmodl.DynamicData):
-        @property
-        def ovfDescriptor(self) -> str: ...
-        @property
-        def error(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def warning(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def includeImageFiles(self) -> bool: ...
+class HostPowerOpFailed(VimFault): ...
 
 
-    class CreateImportSpecParams(OvfManager.CommonParams):
-        @property
-        def entityName(self) -> str: ...
-        @property
-        def hostSystem(self) -> HostSystem: ...
-        @property
-        def networkMapping(self) -> List[OvfManager.NetworkMapping]: ...
-        @property
-        def ipAllocationPolicy(self) -> str: ...
-        @property
-        def ipProtocol(self) -> str: ...
-        @property
-        def propertyMapping(self) -> List[KeyValue]: ...
-        @property
-        def resourceMapping(self) -> List[OvfManager.ResourceMap]: ...
-        @property
-        def diskProvisioning(self) -> str: ...
-        @property
-        def instantiationOst(self) -> OvfConsumer.OstNode: ...
+class HostSpecificationOperationFailed(VimFault):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-        class DiskProvisioningType(Enum):
-            monolithicSparse = "monolithicsparse"
-            monolithicFlat = "monolithicflat"
-            twoGbMaxExtentSparse = "twogbmaxextentsparse"
-            twoGbMaxExtentFlat = "twogbmaxextentflat"
-            thin = "thin"
-            thick = "thick"
-            seSparse = "sesparse"
-            eagerZeroedThick = "eagerzeroedthick"
-            sparse = "sparse"
-            flat = "flat"
+class HotSnapshotMoveNotSupported(SnapshotCopyNotSupported): ...
 
 
-    class CreateImportSpecResult(vmodl.DynamicData):
-        @property
-        def importSpec(self) -> ImportSpec: ...
-        @property
-        def fileItem(self) -> List[OvfManager.FileItem]: ...
-        @property
-        def warning(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def error(self) -> List[vmodl.MethodFault]: ...
+class HttpFault(VimFault):
+    @property
+    def statusCode(self) -> int: ...
+    @statusCode.setter
+    def statusCode(self, value: int):
+        self._statusCode = value
+    @property
+    def statusMessage(self) -> str: ...
+    @statusMessage.setter
+    def statusMessage(self, value: str):
+        self._statusMessage = value
 
 
-    class DeploymentOption(vmodl.DynamicData):
-        @property
-        def key(self) -> str: ...
-        @property
-        def label(self) -> str: ...
-        @property
-        def description(self) -> str: ...
+class IDEDiskNotSupported(DiskNotSupported): ...
 
 
-    class FileItem(vmodl.DynamicData):
-        @property
-        def deviceId(self) -> str: ...
-        @property
-        def path(self) -> str: ...
-        @property
-        def compressionMethod(self) -> str: ...
-        @property
-        def chunkSize(self) -> long: ...
-        @property
-        def size(self) -> long: ...
-        @property
-        def cimType(self) -> int: ...
-        @property
-        def create(self) -> bool: ...
+class IORMNotSupportedHostOnDatastore(VimFault):
+    @property
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
+    @property
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
+    @property
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
 
 
-    class NetworkInfo(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def description(self) -> str: ...
+class ImportHostAddFailure(DvsFault):
+    @property
+    def hostIp(self) -> List[str]: ...
+    @hostIp.setter
+    def hostIp(self, value: List[str]):
+        self._hostIp = value
 
 
-    class NetworkMapping(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def network(self) -> Network: ...
+class ImportOperationBulkFault(DvsFault):
+    @property
+    def importFaults(self) -> List[ImportOperationBulkFault.FaultOnImport]: ...
+    @importFaults.setter
+    def importFaults(self, value: List[ImportOperationBulkFault.FaultOnImport]):
+        self._importFaults = value
 
 
-    class OvfFile(vmodl.DynamicData):
+    class FaultOnImport(vmodl.DynamicData):
         @property
-        def deviceId(self) -> str: ...
+        def entityType(self) -> str: ...
+        @entityType.setter
+        def entityType(self, value: str):
+            self._entityType = value
         @property
-        def path(self) -> str: ...
-        @property
-        def compressionMethod(self) -> str: ...
-        @property
-        def chunkSize(self) -> long: ...
-        @property
-        def size(self) -> long: ...
-        @property
-        def capacity(self) -> long: ...
+        def key(self) -> str: ...
+        @key.setter
+        def key(self, value: str):
+            self._key = value
         @property
-        def populatedSize(self) -> long: ...
+        def fault(self) -> vmodl.MethodFault: ...
+        @fault.setter
+        def fault(self, value: vmodl.MethodFault):
+            self._fault = value
 
 
-    class OvfOptionInfo(vmodl.DynamicData):
-        @property
-        def option(self) -> str: ...
-        @property
-        def description(self) -> vmodl.LocalizableMessage: ...
+class InUseFeatureManipulationDisallowed(NotEnoughLicenses): ...
 
 
-    class ParseDescriptorParams(OvfManager.CommonParams): ...
+class InaccessibleDatastore(InvalidDatastore):
+    @property
+    def detail(self) -> str: ...
+    @detail.setter
+    def detail(self, value: str):
+        self._detail = value
 
 
-    class ParseDescriptorResult(vmodl.DynamicData):
-        @property
-        def eula(self) -> List[str]: ...
-        @property
-        def network(self) -> List[OvfManager.NetworkInfo]: ...
-        @property
-        def ipAllocationScheme(self) -> List[str]: ...
-        @property
-        def ipProtocols(self) -> List[str]: ...
-        @property
-        def property(self) -> List[vApp.PropertyInfo]: ...
-        @property
-        def productInfo(self) -> vApp.ProductInfo: ...
-        @property
-        def annotation(self) -> str: ...
-        @property
-        def approximateDownloadSize(self) -> long: ...
-        @property
-        def approximateFlatDeploymentSize(self) -> long: ...
-        @property
-        def approximateSparseDeploymentSize(self) -> long: ...
-        @property
-        def defaultEntityName(self) -> str: ...
-        @property
-        def virtualApp(self) -> bool: ...
-        @property
-        def deploymentOption(self) -> List[OvfManager.DeploymentOption]: ...
-        @property
-        def defaultDeploymentOption(self) -> str: ...
-        @property
-        def entityName(self) -> List[KeyValue]: ...
-        @property
-        def annotatedOst(self) -> OvfConsumer.OstNode: ...
-        @property
-        def error(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def warning(self) -> List[vmodl.MethodFault]: ...
+class InaccessibleFTMetadataDatastore(InaccessibleDatastore): ...
 
 
-    class ResourceMap(vmodl.DynamicData):
-        @property
-        def source(self) -> str: ...
-        @property
-        def parent(self) -> ResourcePool: ...
-        @property
-        def resourceSpec(self) -> ResourceConfigSpec: ...
-        @property
-        def datastore(self) -> Datastore: ...
+class InaccessibleVFlashSource(VimFault):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-    class ValidateHostParams(OvfManager.CommonParams): ...
+class IncompatibleDefaultDevice(MigrationFault):
+    @property
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
 
-    class ValidateHostResult(vmodl.DynamicData):
-        @property
-        def downloadSize(self) -> long: ...
-        @property
-        def flatDeploymentSize(self) -> long: ...
-        @property
-        def sparseDeploymentSize(self) -> long: ...
-        @property
-        def error(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def warning(self) -> List[vmodl.MethodFault]: ...
-        @property
-        def supportedDiskProvisioning(self) -> List[str]: ...
+class IncompatibleHostForFtSecondary(VmFaultToleranceIssue):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
+    @property
+    def error(self) -> List[vmodl.MethodFault]: ...
+    @error.setter
+    def error(self, value: List[vmodl.MethodFault]):
+        self._error = value
 
 
-class PerformanceManager(ManagedObject):
+class IncompatibleHostForVmReplication(ReplicationFault):
     @property
-    def description(self) -> PerformanceDescription: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def historicalInterval(self) -> List[HistoricalInterval]: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def perfCounter(self) -> List[PerformanceManager.CounterInfo]: ...
-    def QueryProviderSummary(self, entity: ManagedObject) -> PerformanceManager.ProviderSummary: ...
-    def QueryAvailableMetric(self, entity: ManagedObject, beginTime: datetime, endTime: datetime, intervalId: int) -> List[PerformanceManager.MetricId]: ...
-    def QueryCounter(self, counterId: List[int]) -> List[PerformanceManager.CounterInfo]: ...
-    def QueryCounterByLevel(self, level: int) -> List[PerformanceManager.CounterInfo]: ...
-    def QueryStats(self, querySpec: List[PerformanceManager.QuerySpec]) -> List[PerformanceManager.EntityMetricBase]: ...
-    def QueryCompositeStats(self, querySpec: PerformanceManager.QuerySpec) -> PerformanceManager.CompositeEntityMetric: ...
-    def CreateHistoricalInterval(self, intervalId: HistoricalInterval) -> NoneType: ...
-    def RemoveHistoricalInterval(self, samplePeriod: int) -> NoneType: ...
-    def UpdateHistoricalInterval(self, interval: HistoricalInterval) -> NoneType: ...
-    def UpdateCounterLevelMapping(self, counterLevelMap: List[PerformanceManager.CounterLevelMapping]) -> NoneType: ...
-    def ResetCounterLevelMapping(self, counters: List[int]) -> NoneType: ...
-
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
-    class CompositeEntityMetric(vmodl.DynamicData):
-        @property
-        def entity(self) -> PerformanceManager.EntityMetricBase: ...
-        @property
-        def childEntity(self) -> List[PerformanceManager.EntityMetricBase]: ...
 
-
-    class CounterInfo(vmodl.DynamicData):
-        @property
-        def key(self) -> int: ...
-        @property
-        def nameInfo(self) -> ElementDescription: ...
-        @property
-        def groupInfo(self) -> ElementDescription: ...
-        @property
-        def unitInfo(self) -> ElementDescription: ...
-        @property
-        def rollupType(self) -> PerformanceManager.CounterInfo.RollupType: ...
-        @property
-        def statsType(self) -> PerformanceManager.CounterInfo.StatsType: ...
-        @property
-        def level(self) -> int: ...
-        @property
-        def perDeviceLevel(self) -> int: ...
-        @property
-        def associatedCounterId(self) -> List[int]: ...
+    class IncompatibleReason(Enum):
+        rpo = "rpo"
+        netCompression = "netCompression"
 
 
-        class RollupType(Enum):
-            average = "average"
-            maximum = "maximum"
-            minimum = "minimum"
-            latest = "latest"
-            summation = "summation"
-            none = "none"
-
-
-        class StatsType(Enum):
-            absolute = "absolute"
-            delta = "delta"
-            rate = "rate"
-
-
-        class Unit(Enum):
-            percent = "percent"
-            kiloBytes = "kilobytes"
-            megaBytes = "megabytes"
-            megaHertz = "megahertz"
-            number = "number"
-            microsecond = "microsecond"
-            millisecond = "millisecond"
-            second = "second"
-            kiloBytesPerSecond = "kilobytespersecond"
-            megaBytesPerSecond = "megabytespersecond"
-            watt = "watt"
-            joule = "joule"
-            teraBytes = "terabytes"
-            celsius = "celsius"
-            mgCO2eqPerHour = "mgco2eqperhour"
-            nanosecond = "nanosecond"
+class IncompatibleSetting(InvalidArgument):
+    @property
+    def conflictingProperty(self) -> PropertyPath: ...
+    @conflictingProperty.setter
+    def conflictingProperty(self, value: PropertyPath):
+        self._conflictingProperty = value
 
 
-    class CounterLevelMapping(vmodl.DynamicData):
-        @property
-        def counterId(self) -> int: ...
-        @property
-        def aggregateLevel(self) -> int: ...
-        @property
-        def perDeviceLevel(self) -> int: ...
+class IncorrectFileType(FileFault): ...
 
 
-    class EntityMetric(PerformanceManager.EntityMetricBase):
-        @property
-        def sampleInfo(self) -> List[PerformanceManager.SampleInfo]: ...
-        @property
-        def value(self) -> List[PerformanceManager.MetricSeries]: ...
+class IncorrectHostInformation(NotEnoughLicenses): ...
 
 
-    class EntityMetricBase(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedObject: ...
+class IndependentDiskVMotionNotSupported(MigrationFeatureNotSupported): ...
 
 
-    class EntityMetricCSV(PerformanceManager.EntityMetricBase):
-        @property
-        def sampleInfoCSV(self) -> str: ...
-        @property
-        def value(self) -> List[PerformanceManager.MetricSeriesCSV]: ...
+class InsufficientAgentVmsDeployed(InsufficientResourcesFault):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+    @property
+    def requiredNumAgentVms(self) -> int: ...
+    @requiredNumAgentVms.setter
+    def requiredNumAgentVms(self, value: int):
+        self._requiredNumAgentVms = value
+    @property
+    def currentNumAgentVms(self) -> int: ...
+    @currentNumAgentVms.setter
+    def currentNumAgentVms(self, value: int):
+        self._currentNumAgentVms = value
 
 
-    class IntSeries(PerformanceManager.MetricSeries):
-        @property
-        def value(self) -> List[long]: ...
+class InsufficientCpuResourcesFault(InsufficientResourcesFault):
+    @property
+    def unreserved(self) -> long: ...
+    @unreserved.setter
+    def unreserved(self, value: long):
+        self._unreserved = value
+    @property
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
 
 
-    class MetricId(vmodl.DynamicData):
-        @property
-        def counterId(self) -> int: ...
-        @property
-        def instance(self) -> str: ...
+class InsufficientDisks(VsanDiskFault): ...
 
 
-    class MetricSeries(vmodl.DynamicData):
-        @property
-        def id(self) -> PerformanceManager.MetricId: ...
+class InsufficientFailoverResourcesFault(InsufficientResourcesFault): ...
 
 
-    class MetricSeriesCSV(PerformanceManager.MetricSeries):
-        @property
-        def value(self) -> str: ...
+class InsufficientGraphicsResourcesFault(InsufficientResourcesFault): ...
 
 
-    class ProviderSummary(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedObject: ...
-        @property
-        def currentSupported(self) -> bool: ...
-        @property
-        def summarySupported(self) -> bool: ...
-        @property
-        def refreshRate(self) -> int: ...
+class InsufficientHostCapacityFault(InsufficientResourcesFault):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class QuerySpec(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedObject: ...
-        @property
-        def startTime(self) -> datetime: ...
-        @property
-        def endTime(self) -> datetime: ...
-        @property
-        def maxSample(self) -> int: ...
-        @property
-        def metricId(self) -> List[PerformanceManager.MetricId]: ...
-        @property
-        def intervalId(self) -> int: ...
-        @property
-        def format(self) -> str: ...
+class InsufficientHostCpuCapacityFault(InsufficientHostCapacityFault):
+    @property
+    def unreserved(self) -> long: ...
+    @unreserved.setter
+    def unreserved(self, value: long):
+        self._unreserved = value
+    @property
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
 
 
-    class SampleInfo(vmodl.DynamicData):
-        @property
-        def timestamp(self) -> datetime: ...
-        @property
-        def interval(self) -> int: ...
+class InsufficientHostMemoryCapacityFault(InsufficientHostCapacityFault):
+    @property
+    def unreserved(self) -> long: ...
+    @unreserved.setter
+    def unreserved(self, value: long):
+        self._unreserved = value
+    @property
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
 
 
-class ResourcePlanningManager(ManagedObject):
-    def EstimateDatabaseSize(self, dbSizeParam: ResourcePlanningManager.DatabaseSizeParam) -> ResourcePlanningManager.DatabaseSizeEstimate: ...
+class InsufficientMemoryResourcesFault(InsufficientResourcesFault):
+    @property
+    def unreserved(self) -> long: ...
+    @unreserved.setter
+    def unreserved(self, value: long):
+        self._unreserved = value
+    @property
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
 
 
-    class DatabaseSizeEstimate(vmodl.DynamicData):
-        @property
-        def size(self) -> long: ...
+class InsufficientNetworkCapacity(InsufficientResourcesFault): ...
 
 
-    class DatabaseSizeParam(vmodl.DynamicData):
-        @property
-        def inventoryDesc(self) -> ResourcePlanningManager.InventoryDescription: ...
-        @property
-        def perfStatsDesc(self) -> ResourcePlanningManager.PerfStatsDescription: ...
+class InsufficientNetworkResourcePoolCapacity(InsufficientResourcesFault):
+    @property
+    def dvsName(self) -> str: ...
+    @dvsName.setter
+    def dvsName(self, value: str):
+        self._dvsName = value
+    @property
+    def dvsUuid(self) -> str: ...
+    @dvsUuid.setter
+    def dvsUuid(self, value: str):
+        self._dvsUuid = value
+    @property
+    def resourcePoolKey(self) -> str: ...
+    @resourcePoolKey.setter
+    def resourcePoolKey(self, value: str):
+        self._resourcePoolKey = value
+    @property
+    def available(self) -> long: ...
+    @available.setter
+    def available(self, value: long):
+        self._available = value
+    @property
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
+    @property
+    def device(self) -> List[str]: ...
+    @device.setter
+    def device(self, value: List[str]):
+        self._device = value
 
 
-    class InventoryDescription(vmodl.DynamicData):
-        @property
-        def numHosts(self) -> int: ...
-        @property
-        def numVirtualMachines(self) -> int: ...
-        @property
-        def numResourcePools(self) -> int: ...
-        @property
-        def numClusters(self) -> int: ...
-        @property
-        def numCpuDev(self) -> int: ...
-        @property
-        def numNetDev(self) -> int: ...
-        @property
-        def numDiskDev(self) -> int: ...
-        @property
-        def numvCpuDev(self) -> int: ...
-        @property
-        def numvNetDev(self) -> int: ...
-        @property
-        def numvDiskDev(self) -> int: ...
+class InsufficientPerCpuCapacity(InsufficientHostCapacityFault): ...
 
 
-    class PerfStatsDescription(vmodl.DynamicData):
-        @property
-        def intervals(self) -> List[HistoricalInterval]: ...
+class InsufficientResourcesFault(VimFault): ...
 
 
-class ResourcePool(ManagedEntity):
-    @property
-    def summary(self) -> ResourcePool.Summary: ...
+class InsufficientStandbyCpuResource(InsufficientStandbyResource):
     @property
-    def runtime(self) -> ResourcePool.RuntimeInfo: ...
+    def available(self) -> long: ...
+    @available.setter
+    def available(self, value: long):
+        self._available = value
     @property
-    def owner(self) -> ComputeResource: ...
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
+
+
+class InsufficientStandbyMemoryResource(InsufficientStandbyResource):
     @property
-    def resourcePool(self) -> List[ResourcePool]: ...
+    def available(self) -> long: ...
+    @available.setter
+    def available(self, value: long):
+        self._available = value
     @property
-    def vm(self) -> List[VirtualMachine]: ...
+    def requested(self) -> long: ...
+    @requested.setter
+    def requested(self, value: long):
+        self._requested = value
+
+
+class InsufficientStandbyResource(InsufficientResourcesFault): ...
+
+
+class InsufficientStorageIops(VimFault):
     @property
-    def config(self) -> ResourceConfigSpec: ...
+    def unreservedIops(self) -> long: ...
+    @unreservedIops.setter
+    def unreservedIops(self, value: long):
+        self._unreservedIops = value
     @property
-    def namespace(self) -> str: ...
+    def requestedIops(self) -> long: ...
+    @requestedIops.setter
+    def requestedIops(self, value: long):
+        self._requestedIops = value
     @property
-    def childConfiguration(self) -> List[ResourceConfigSpec]: ...
-    def UpdateConfig(self, name: str, config: ResourceConfigSpec) -> NoneType: ...
-    def MoveInto(self, list: List[ManagedEntity]) -> NoneType: ...
-    def UpdateChildResourceConfiguration(self, spec: List[ResourceConfigSpec]) -> NoneType: ...
-    def CreateResourcePool(self, name: str, spec: ResourceConfigSpec) -> ResourcePool: ...
-    def DestroyChildren(self) -> NoneType: ...
-    def CreateVApp(self, name: str, resSpec: ResourceConfigSpec, configSpec: vApp.VAppConfigSpec, vmFolder: Folder) -> VirtualApp: ...
-    def CreateVm(self, config: vm.ConfigSpec, host: HostSystem) -> Task: ...
-    def RegisterVm(self, path: str, name: str, host: HostSystem) -> Task: ...
-    def ImportVApp(self, spec: ImportSpec, folder: Folder, host: HostSystem) -> HttpNfcLease: ...
-    def QueryResourceConfigOption(self) -> ResourceConfigOption: ...
-    def RefreshRuntime(self) -> NoneType: ...
-
-
-    class ResourceUsage(vmodl.DynamicData):
-        @property
-        def reservationUsed(self) -> long: ...
-        @property
-        def reservationUsedForVm(self) -> long: ...
-        @property
-        def unreservedForPool(self) -> long: ...
-        @property
-        def unreservedForVm(self) -> long: ...
-        @property
-        def overallUsage(self) -> long: ...
-        @property
-        def maxUsage(self) -> long: ...
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
 
 
-class SearchIndex(ManagedObject):
-    def FindByUuid(self, datacenter: Datacenter, uuid: str, vmSearch: bool, instanceUuid: bool) -> ManagedEntity: ...
-    def FindByDatastorePath(self, datacenter: Datacenter, path: str) -> VirtualMachine: ...
-    def FindByDnsName(self, datacenter: Datacenter, dnsName: str, vmSearch: bool) -> ManagedEntity: ...
-    def FindByIp(self, datacenter: Datacenter, ip: str, vmSearch: bool) -> ManagedEntity: ...
-    def FindByInventoryPath(self, inventoryPath: str) -> ManagedEntity: ...
-    def FindChild(self, entity: ManagedEntity, name: str) -> ManagedEntity: ...
-    def FindAllByUuid(self, datacenter: Datacenter, uuid: str, vmSearch: bool, instanceUuid: bool) -> List[ManagedEntity]: ...
-    def FindAllByDnsName(self, datacenter: Datacenter, dnsName: str, vmSearch: bool) -> List[ManagedEntity]: ...
-    def FindAllByIp(self, datacenter: Datacenter, ip: str, vmSearch: bool) -> List[ManagedEntity]: ...
+class InsufficientStorageSpace(InsufficientResourcesFault): ...
 
 
-class ServiceInstance(ManagedObject):
+class InsufficientVFlashResourcesFault(InsufficientResourcesFault):
     @property
-    def serverClock(self) -> datetime: ...
+    def freeSpaceInMB(self) -> long: ...
+    @freeSpaceInMB.setter
+    def freeSpaceInMB(self, value: long):
+        self._freeSpaceInMB = value
     @property
-    def capability(self) -> Capability: ...
+    def freeSpace(self) -> long: ...
+    @freeSpace.setter
+    def freeSpace(self, value: long):
+        self._freeSpace = value
     @property
-    def content(self) -> ServiceInstanceContent: ...
-    def CurrentTime(self) -> datetime: ...
-    def RetrieveContent(self) -> ServiceInstanceContent: ...
-    def ValidateMigration(self, vm: List[VirtualMachine], state: VirtualMachine.PowerState, testType: List[str], pool: ResourcePool, host: HostSystem) -> List[event.Event]: ...
-    def QueryVMotionCompatibility(self, vm: VirtualMachine, host: List[HostSystem], compatibility: List[str]) -> List[ServiceInstance.HostVMotionCompatibility]: ...
-    def RetrieveProductComponents(self) -> List[ServiceInstance.ProductComponentInfo]: ...
+    def requestedSpaceInMB(self) -> long: ...
+    @requestedSpaceInMB.setter
+    def requestedSpaceInMB(self, value: long):
+        self._requestedSpaceInMB = value
+    @property
+    def requestedSpace(self) -> long: ...
+    @requestedSpace.setter
+    def requestedSpace(self, value: long):
+        self._requestedSpace = value
 
 
-    class HostVMotionCompatibility(vmodl.DynamicData):
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def compatibility(self) -> List[str]: ...
+class InvalidAffinitySettingFault(VimFault): ...
 
 
-    class ProductComponentInfo(vmodl.DynamicData):
-        @property
-        def id(self) -> str: ...
-        @property
-        def name(self) -> str: ...
-        @property
-        def version(self) -> str: ...
-        @property
-        def release(self) -> int: ...
+class InvalidBmcRole(VimFault): ...
 
 
-    class VMotionCompatibilityType(Enum):
-        cpu = "cpu"
-        software = "software"
+class InvalidBundle(PlatformConfigFault): ...
 
 
-    class ValidateMigrationTestType(Enum):
-        sourceTests = "sourcetests"
-        compatibilityTests = "compatibilitytests"
-        diskAccessibilityTests = "diskaccessibilitytests"
-        resourceTests = "resourcetests"
+class InvalidCAMCertificate(InvalidCAMServer): ...
 
 
-class ServiceManager(ManagedObject):
+class InvalidCAMServer(ActiveDirectoryFault):
     @property
-    def service(self) -> List[ServiceManager.ServiceInfo]: ...
-    def QueryServiceList(self, serviceName: str, location: List[str]) -> List[ServiceManager.ServiceInfo]: ...
+    def camServer(self) -> str: ...
+    @camServer.setter
+    def camServer(self, value: str):
+        self._camServer = value
 
 
-    class ServiceInfo(vmodl.DynamicData):
-        @property
-        def serviceName(self) -> str: ...
-        @property
-        def location(self) -> List[str]: ...
-        @property
-        def service(self) -> ManagedObject: ...
-        @property
-        def description(self) -> str: ...
+class InvalidClientCertificate(InvalidLogin): ...
 
 
-class SessionManager(ManagedObject):
+class InvalidController(InvalidDeviceSpec):
     @property
-    def sessionList(self) -> List[UserSession]: ...
-    @property
-    def currentSession(self) -> UserSession: ...
+    def controllerKey(self) -> int: ...
+    @controllerKey.setter
+    def controllerKey(self, value: int):
+        self._controllerKey = value
+
+
+class InvalidDasConfigArgument(InvalidArgument):
     @property
-    def message(self) -> str: ...
+    def entry(self) -> str: ...
+    @entry.setter
+    def entry(self, value: str):
+        self._entry = value
     @property
-    def messageLocaleList(self) -> List[str]: ...
+    def clusterName(self) -> str: ...
+    @clusterName.setter
+    def clusterName(self, value: str):
+        self._clusterName = value
+
+
+    class EntryForInvalidArgument(Enum):
+        admissionControl = "admissionControl"
+        userHeartbeatDs = "userHeartbeatDs"
+        vmConfig = "vmConfig"
+
+
+class InvalidDasRestartPriorityForFtVm(InvalidArgument):
     @property
-    def supportedLocaleList(self) -> List[str]: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def defaultLocale(self) -> str: ...
-    def UpdateMessage(self, message: str) -> NoneType: ...
-    def LoginByToken(self, locale: str) -> UserSession: ...
-    def Login(self, userName: str, password: str, locale: str) -> UserSession: ...
-    def LoginBySSPI(self, base64Token: str, locale: str) -> UserSession: ...
-    def Logout(self) -> NoneType: ...
-    def AcquireLocalTicket(self, userName: str) -> SessionManager.LocalTicket: ...
-    def AcquireGenericServiceTicket(self, spec: SessionManager.ServiceRequestSpec) -> SessionManager.GenericServiceTicket: ...
-    def Terminate(self, sessionId: List[str]) -> NoneType: ...
-    def SetLocale(self, locale: str) -> NoneType: ...
-    def LoginExtensionBySubjectName(self, extensionKey: str, locale: str) -> UserSession: ...
-    def LoginExtensionByCertificate(self, extensionKey: str, locale: str) -> UserSession: ...
-    def ImpersonateUser(self, userName: str, locale: str) -> UserSession: ...
-    def SessionIsActive(self, sessionID: str, userName: str) -> bool: ...
-    def AcquireCloneTicket(self) -> str: ...
-    def CloneSession(self, cloneTicket: str) -> UserSession: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class GenericServiceTicket(vmodl.DynamicData):
-        @property
-        def id(self) -> str: ...
-        @property
-        def hostName(self) -> str: ...
-        @property
-        def sslThumbprint(self) -> str: ...
-        @property
-        def certThumbprintList(self) -> List[vm.CertThumbprint]: ...
-        @property
-        def ticketType(self) -> str: ...
+class InvalidDatastore(VimFault):
+    @property
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-        class TicketType(Enum):
-            HttpNfcServiceTicket = "httpnfcserviceticket"
-            HostServiceTicket = "hostserviceticket"
-            VcServiceTicket = "vcserviceticket"
+class InvalidDatastorePath(InvalidDatastore):
+    @property
+    def datastorePath(self) -> str: ...
+    @datastorePath.setter
+    def datastorePath(self, value: str):
+        self._datastorePath = value
 
 
-    class HttpServiceRequestSpec(SessionManager.ServiceRequestSpec):
-        @property
-        def method(self) -> str: ...
-        @property
-        def url(self) -> str: ...
+class InvalidDatastoreState(InvalidState):
+    @property
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
 
 
-        class Method(Enum):
-            httpOptions = "httpoptions"
-            httpGet = "httpget"
-            httpHead = "httphead"
-            httpPost = "httppost"
-            httpPut = "httpput"
-            httpDelete = "httpdelete"
-            httpTrace = "httptrace"
-            httpConnect = "httpconnect"
+class InvalidDeviceBacking(InvalidDeviceSpec): ...
 
 
-    class LocalTicket(vmodl.DynamicData):
-        @property
-        def userName(self) -> str: ...
-        @property
-        def passwordFilePath(self) -> str: ...
+class InvalidDeviceOperation(InvalidDeviceSpec):
+    @property
+    def badOp(self) -> vim.vm.device.VirtualDeviceSpec.Operation | Literal['add', 'remove', 'edit']: ...
+    @badOp.setter
+    def badOp(self, value: vim.vm.device.VirtualDeviceSpec.Operation | Literal['add', 'remove', 'edit']):
+        self._badOp = value
+    @property
+    def badFileOp(self) -> vim.vm.device.VirtualDeviceSpec.FileOperation | Literal['create', 'destroy', 'replace']: ...
+    @badFileOp.setter
+    def badFileOp(self, value: vim.vm.device.VirtualDeviceSpec.FileOperation | Literal['create', 'destroy', 'replace']):
+        self._badFileOp = value
 
 
-    class ServiceRequestSpec(vmodl.DynamicData): ...
+class InvalidDeviceSpec(InvalidVmConfig):
+    @property
+    def deviceIndex(self) -> int: ...
+    @deviceIndex.setter
+    def deviceIndex(self, value: int):
+        self._deviceIndex = value
 
 
-    class VmomiServiceRequestSpec(SessionManager.ServiceRequestSpec):
-        @property
-        def method(self) -> ManagedMethod: ...
+class InvalidDiskFormat(InvalidFormat): ...
 
 
-class SimpleCommand(ManagedObject):
+class InvalidDrsBehaviorForFtVm(InvalidArgument):
     @property
-    def encodingType(self) -> SimpleCommand.Encoding: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def entity(self) -> ServiceManager.ServiceInfo: ...
-    def Execute(self, arguments: List[str]) -> str: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class Encoding(Enum):
-        CSV = "csv"
-        HEX = "hex"
-        STRING = "string"
+class InvalidEditionLicense(NotEnoughLicenses):
+    @property
+    def feature(self) -> str: ...
+    @feature.setter
+    def feature(self, value: str):
+        self._feature = value
 
 
-class SiteInfoManager(ManagedObject):
-    def GetSiteInfo(self) -> SiteInfo: ...
+class InvalidEvent(VimFault): ...
 
 
-class StoragePod(Folder):
-    @property
-    def summary(self) -> StoragePod.Summary: ...
+class InvalidFolder(VimFault):
     @property
-    def podStorageDrsEntry(self) -> StorageResourceManager.PodStorageDrsEntry: ...
+    def target(self) -> vim.ManagedEntity: ...
+    @target.setter
+    def target(self, value: vim.ManagedEntity):
+        self._target = value
 
 
-class StorageQueryManager(ManagedObject):
-    def QueryHostsWithAttachedLun(self, lunUuid: str) -> List[HostSystem]: ...
+class InvalidFormat(VmConfigFault): ...
 
 
-class StorageResourceManager(ManagedObject):
-    def ConfigureDatastoreIORM(self, datastore: Datastore, spec: StorageResourceManager.IORMConfigSpec) -> Task: ...
-    def QueryIORMConfigOption(self, host: HostSystem) -> StorageResourceManager.IORMConfigOption: ...
-    def QueryDatastorePerformanceSummary(self, datastore: Datastore) -> List[StorageResourceManager.StoragePerformanceSummary]: ...
-    def ApplyRecommendationToPod(self, pod: StoragePod, key: str) -> Task: ...
-    def ApplyRecommendation(self, key: List[str]) -> Task: ...
-    def CancelRecommendation(self, key: List[str]) -> NoneType: ...
-    def RefreshRecommendation(self, pod: StoragePod) -> NoneType: ...
-    def RefreshRecommendationsForPod(self, pod: StoragePod) -> Task: ...
-    def ConfigureStorageDrsForPod(self, pod: StoragePod, spec: storageDrs.ConfigSpec, modify: bool) -> Task: ...
-    def ValidateStoragePodConfig(self, pod: StoragePod, spec: storageDrs.ConfigSpec) -> vmodl.MethodFault: ...
-    def RecommendDatastores(self, storageSpec: storageDrs.StoragePlacementSpec) -> storageDrs.StoragePlacementResult: ...
+class InvalidGuestLogin(GuestOperationsFault): ...
 
 
-    class IOAllocationInfo(vmodl.DynamicData):
-        @property
-        def limit(self) -> long: ...
-        @property
-        def shares(self) -> SharesInfo: ...
-        @property
-        def reservation(self) -> int: ...
+class InvalidHostConnectionState(InvalidHostState): ...
 
 
-    class IOAllocationOption(vmodl.DynamicData):
-        @property
-        def limitOption(self) -> option.LongOption: ...
-        @property
-        def sharesOption(self) -> SharesOption: ...
+class InvalidHostName(HostConfigFault): ...
 
 
-    class IORMConfigInfo(vmodl.DynamicData):
-        @property
-        def enabled(self) -> bool: ...
-        @property
-        def congestionThresholdMode(self) -> str: ...
-        @property
-        def congestionThreshold(self) -> int: ...
-        @property
-        def percentOfPeakThroughput(self) -> int: ...
-        @property
-        def statsCollectionEnabled(self) -> bool: ...
-        @property
-        def reservationEnabled(self) -> bool: ...
-        @property
-        def statsAggregationDisabled(self) -> bool: ...
-        @property
-        def reservableIopsThreshold(self) -> int: ...
+class InvalidHostState(InvalidState):
+    @property
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class IORMConfigOption(vmodl.DynamicData):
-        @property
-        def enabledOption(self) -> option.BoolOption: ...
-        @property
-        def congestionThresholdOption(self) -> option.IntOption: ...
-        @property
-        def statsCollectionEnabledOption(self) -> option.BoolOption: ...
-        @property
-        def reservationEnabledOption(self) -> option.BoolOption: ...
+class InvalidIndexArgument(InvalidArgument):
+    @property
+    def key(self) -> str: ...
+    @key.setter
+    def key(self, value: str):
+        self._key = value
 
 
-    class IORMConfigSpec(vmodl.DynamicData):
-        @property
-        def enabled(self) -> bool: ...
-        @property
-        def congestionThresholdMode(self) -> str: ...
-        @property
-        def congestionThreshold(self) -> int: ...
-        @property
-        def percentOfPeakThroughput(self) -> int: ...
-        @property
-        def statsCollectionEnabled(self) -> bool: ...
-        @property
-        def reservationEnabled(self) -> bool: ...
-        @property
-        def statsAggregationDisabled(self) -> bool: ...
-        @property
-        def reservableIopsThreshold(self) -> int: ...
+class InvalidIpfixConfig(DvsFault):
+    @property
+    def property(self) -> PropertyPath: ...
+    @property.setter
+    def property(self, value: PropertyPath):
+        self._property = value
 
 
-    class PodStorageDrsEntry(vmodl.DynamicData):
-        @property
-        def storageDrsConfig(self) -> storageDrs.ConfigInfo: ...
-        @property
-        def recommendation(self) -> List[cluster.Recommendation]: ...
-        @property
-        def drsFault(self) -> List[cluster.DrsFaults]: ...
-        @property
-        def actionHistory(self) -> List[cluster.ActionHistory]: ...
+class InvalidIpmiLoginInfo(VimFault): ...
 
 
-    class StoragePerformanceSummary(vmodl.DynamicData):
-        @property
-        def interval(self) -> int: ...
-        @property
-        def percentile(self) -> List[int]: ...
-        @property
-        def datastoreReadLatency(self) -> List[double]: ...
-        @property
-        def datastoreWriteLatency(self) -> List[double]: ...
-        @property
-        def datastoreVmLatency(self) -> List[double]: ...
-        @property
-        def datastoreReadIops(self) -> List[double]: ...
-        @property
-        def datastoreWriteIops(self) -> List[double]: ...
-        @property
-        def siocActivityDuration(self) -> int: ...
+class InvalidIpmiMacAddress(VimFault):
+    @property
+    def userProvidedMacAddress(self) -> str: ...
+    @userProvidedMacAddress.setter
+    def userProvidedMacAddress(self, value: str):
+        self._userProvidedMacAddress = value
+    @property
+    def observedMacAddress(self) -> str: ...
+    @observedMacAddress.setter
+    def observedMacAddress(self, value: str):
+        self._observedMacAddress = value
 
 
-    class StorageProfileStatistics(vmodl.DynamicData):
-        @property
-        def profileId(self) -> str: ...
-        @property
-        def totalSpaceMB(self) -> long: ...
-        @property
-        def usedSpaceMB(self) -> long: ...
+class InvalidLicense(VimFault):
+    @property
+    def licenseContent(self) -> str: ...
+    @licenseContent.setter
+    def licenseContent(self, value: str):
+        self._licenseContent = value
 
 
-    class CongestionThresholdMode(Enum):
-        automatic = "automatic"
-        manual = "manual"
+class InvalidLocale(VimFault): ...
 
 
-class Task(ExtensibleManagedObject):
-    @property
-    def info(self) -> TaskInfo: ...
-    def Cancel(self) -> NoneType: ...
-    def UpdateProgress(self, percentDone: int) -> NoneType: ...
-    def SetState(self, state: TaskInfo.State, result: object, fault: vmodl.MethodFault) -> NoneType: ...
-    def UpdateDescription(self, description: vmodl.LocalizableMessage) -> NoneType: ...
+class InvalidLogin(VimFault): ...
 
 
-class TaskHistoryCollector(HistoryCollector):
+class InvalidName(VimFault):
+    @property
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def latestPage(self) -> List[TaskInfo]: ...
-    def ReadNext(self, maxCount: int) -> List[TaskInfo]: ...
-    def ReadPrev(self, maxCount: int) -> List[TaskInfo]: ...
+    def entity(self) -> vim.ManagedEntity: ...
+    @entity.setter
+    def entity(self, value: vim.ManagedEntity):
+        self._entity = value
 
 
-class TaskManager(ManagedObject):
+class InvalidNasCredentials(NasConfigFault):
     @property
-    def recentTask(self) -> List[Task]: ...
+    def userName(self) -> str: ...
+    @userName.setter
+    def userName(self, value: str):
+        self._userName = value
+
+
+class InvalidNetworkInType(VAppPropertyFault): ...
+
+
+class InvalidNetworkResource(NasConfigFault):
     @property
-    def description(self) -> TaskDescription: ...
+    def remoteHost(self) -> str: ...
+    @remoteHost.setter
+    def remoteHost(self, value: str):
+        self._remoteHost = value
     @property
-    def maxCollector(self) -> int: ...
-    def CreateCollector(self, filter: TaskFilterSpec) -> TaskHistoryCollector: ...
-    def CreateTask(self, obj: ManagedObject, taskTypeId: str, initiatedBy: str, cancelable: bool, parentTaskKey: str, activationId: str) -> TaskInfo: ...
+    def remotePath(self) -> str: ...
+    @remotePath.setter
+    def remotePath(self, value: str):
+        self._remotePath = value
 
 
-class UserDirectory(ManagedObject):
+class InvalidOperationOnSecondaryVm(VmFaultToleranceIssue):
     @property
-    def domainList(self) -> List[str]: ...
-    def RetrieveUserGroups(self, domain: str, searchStr: str, belongsToGroup: str, belongsToUser: str, exactMatch: bool, findUsers: bool, findGroups: bool) -> List[UserSearchResult]: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
 
 
-class VirtualApp(ResourcePool):
+class InvalidPowerState(InvalidState):
     @property
-    def parentFolder(self) -> Folder: ...
+    def requestedState(self) -> vim.VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended']: ...
+    @requestedState.setter
+    def requestedState(self, value: vim.VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended']):
+        self._requestedState = value
     @property
-    def datastore(self) -> List[Datastore]: ...
+    def existingState(self) -> vim.VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended']: ...
+    @existingState.setter
+    def existingState(self, value: vim.VirtualMachine.PowerState | Literal['poweredOff', 'poweredOn', 'suspended']):
+        self._existingState = value
+
+
+class InvalidPrivilege(VimFault):
     @property
-    def network(self) -> List[Network]: ...
+    def privilege(self) -> str: ...
+    @privilege.setter
+    def privilege(self, value: str):
+        self._privilege = value
+
+
+class InvalidProfileReferenceHost(vmodl.RuntimeFault):
     @property
-    def vAppConfig(self) -> vApp.VAppConfigInfo: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def parentVApp(self) -> ManagedEntity: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def childLink(self) -> List[VirtualApp.LinkInfo]: ...
-    def UpdateVAppConfig(self, spec: vApp.VAppConfigSpec) -> NoneType: ...
-    def UpdateLinkedChildren(self, addChangeSet: List[VirtualApp.LinkInfo], removeSet: List[ManagedEntity]) -> NoneType: ...
-    def Clone(self, name: str, target: ResourcePool, spec: vApp.CloneSpec) -> Task: ...
-    def ExportVApp(self) -> HttpNfcLease: ...
-    def PowerOn(self) -> Task: ...
-    def PowerOff(self, force: bool) -> Task: ...
-    def Suspend(self) -> Task: ...
-    def Unregister(self) -> Task: ...
-
-
-    class LinkInfo(vmodl.DynamicData):
-        @property
-        def key(self) -> ManagedEntity: ...
-        @property
-        def destroyWithParent(self) -> bool: ...
-
+    def profile(self) -> vim.profile.Profile: ...
+    @profile.setter
+    def profile(self, value: vim.profile.Profile):
+        self._profile = value
+    @property
+    def profileName(self) -> str: ...
+    @profileName.setter
+    def profileName(self, value: str):
+        self._profileName = value
 
-    class VAppState(Enum):
-        started = "started"
-        stopped = "stopped"
-        starting = "starting"
-        stopping = "stopping"
-
-
-class VirtualDiskManager(ManagedObject):
-    def CreateVirtualDisk(self, name: str, datacenter: Datacenter, spec: VirtualDiskManager.VirtualDiskSpec) -> Task: ...
-    def DeleteVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def MoveVirtualDisk(self, sourceName: str, sourceDatacenter: Datacenter, destName: str, destDatacenter: Datacenter, force: bool, profile: List[vm.ProfileSpec]) -> Task: ...
-    def CopyVirtualDisk(self, sourceName: str, sourceDatacenter: Datacenter, destName: str, destDatacenter: Datacenter, destSpec: VirtualDiskManager.VirtualDiskSpec, force: bool) -> Task: ...
-    def ExtendVirtualDisk(self, name: str, datacenter: Datacenter, newCapacityKb: long, eagerZero: bool) -> Task: ...
-    def QueryVirtualDiskFragmentation(self, name: str, datacenter: Datacenter) -> int: ...
-    def DefragmentVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def ShrinkVirtualDisk(self, name: str, datacenter: Datacenter, copy: bool) -> Task: ...
-    def InflateVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def EagerZeroVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def ZeroFillVirtualDisk(self, name: str, datacenter: Datacenter) -> Task: ...
-    def SetVirtualDiskUuid(self, name: str, datacenter: Datacenter, uuid: str) -> NoneType: ...
-    def QueryVirtualDiskUuid(self, name: str, datacenter: Datacenter) -> str: ...
-    def QueryVirtualDiskGeometry(self, name: str, datacenter: Datacenter) -> host.DiskDimensions.Chs: ...
-    def ImportUnmanagedSnapshot(self, vdisk: str, datacenter: Datacenter, vvolId: str) -> NoneType: ...
-    def ReleaseManagedSnapshot(self, vdisk: str, datacenter: Datacenter) -> NoneType: ...
 
+class InvalidPropertyType(VAppPropertyFault): ...
 
-    class DeviceBackedVirtualDiskSpec(VirtualDiskManager.VirtualDiskSpec):
-        @property
-        def device(self) -> str: ...
 
+class InvalidPropertyValue(VAppPropertyFault): ...
 
-    class FileBackedVirtualDiskSpec(VirtualDiskManager.VirtualDiskSpec):
-        @property
-        def capacityKb(self) -> long: ...
-        @property
-        def profile(self) -> List[vm.ProfileSpec]: ...
-        @property
-        def crypto(self) -> encryption.CryptoSpec: ...
 
+class InvalidResourcePoolStructureFault(InsufficientResourcesFault): ...
 
-    class SeSparseVirtualDiskSpec(VirtualDiskManager.FileBackedVirtualDiskSpec):
-        @property
-        def grainSizeKb(self) -> int: ...
 
+class InvalidSnapshotFormat(InvalidFormat): ...
 
-    class VirtualDiskSpec(vmodl.DynamicData):
-        @property
-        def diskType(self) -> str: ...
-        @property
-        def adapterType(self) -> str: ...
 
+class InvalidState(VimFault): ...
 
-    class VirtualDiskAdapterType(Enum):
-        ide = "ide"
-        busLogic = "buslogic"
-        lsiLogic = "lsilogic"
-
-
-    class VirtualDiskType(Enum):
-        preallocated = "preallocated"
-        thin = "thin"
-        seSparse = "sesparse"
-        rdm = "rdm"
-        rdmp = "rdmp"
-        raw = "raw"
-        delta = "delta"
-        sparse2Gb = "sparse2gb"
-        thick2Gb = "thick2gb"
-        eagerZeroedThick = "eagerzeroedthick"
-        sparseMonolithic = "sparsemonolithic"
-        flatMonolithic = "flatmonolithic"
-        thick = "thick"
-
-
-class VirtualMachine(ManagedEntity):
-    @property
-    def capability(self) -> vm.Capability: ...
-    @property
-    def config(self) -> vm.ConfigInfo: ...
-    @property
-    def layout(self) -> vm.FileLayout: ...
-    @property
-    def layoutEx(self) -> vm.FileLayoutEx: ...
-    @property
-    def storage(self) -> vm.StorageInfo: ...
-    @property
-    def environmentBrowser(self) -> EnvironmentBrowser: ...
-    @property
-    def resourcePool(self) -> ResourcePool: ...
-    @property
-    def parentVApp(self) -> ManagedEntity: ...
-    @property
-    def resourceConfig(self) -> ResourceConfigSpec: ...
-    @property
-    def runtime(self) -> vm.RuntimeInfo: ...
-    @property
-    def guest(self) -> vm.GuestInfo: ...
-    @property
-    def summary(self) -> vm.Summary: ...
-    @property
-    def datastore(self) -> List[Datastore]: ...
-    @property
-    def network(self) -> List[Network]: ...
-    @property
-    def snapshot(self) -> vm.SnapshotInfo: ...
-    @property
-    def rootSnapshot(self) -> List[vm.Snapshot]: ...
-    @property
-    def guestHeartbeatStatus(self) -> ManagedEntity.Status: ...
-    def RefreshStorageInfo(self) -> NoneType: ...
-    def CreateSnapshot(self, name: str, description: str, memory: bool, quiesce: bool) -> Task: ...
-    def CreateSnapshotEx(self, name: str, description: str, memory: bool, quiesceSpec: vm.GuestQuiesceSpec) -> Task: ...
-    def RevertToCurrentSnapshot(self, host: HostSystem, suppressPowerOn: bool) -> Task: ...
-    def RemoveAllSnapshots(self, consolidate: bool) -> Task: ...
-    def ConsolidateDisks(self) -> Task: ...
-    def EstimateStorageRequirementForConsolidate(self) -> Task: ...
-    def Reconfigure(self, spec: vm.ConfigSpec) -> Task: ...
-    def UpgradeVirtualHardware(self, version: str) -> Task: ...
-    def ExtractOvfEnvironment(self) -> str: ...
-    def PowerOn(self, host: HostSystem) -> Task: ...
-    def PowerOff(self) -> Task: ...
-    def Suspend(self) -> Task: ...
-    def Reset(self) -> Task: ...
-    def ShutdownGuest(self) -> NoneType: ...
-    def RebootGuest(self) -> NoneType: ...
-    def StandbyGuest(self) -> NoneType: ...
-    def Answer(self, questionId: str, answerChoice: str) -> NoneType: ...
-    def Customize(self, spec: vm.customization.Specification) -> Task: ...
-    def CheckCustomizationSpec(self, spec: vm.customization.Specification) -> NoneType: ...
-    def Migrate(self, pool: ResourcePool, host: HostSystem, priority: VirtualMachine.MovePriority, state: VirtualMachine.PowerState) -> Task: ...
-    def Relocate(self, spec: vm.RelocateSpec, priority: VirtualMachine.MovePriority) -> Task: ...
-    def Clone(self, folder: Folder, name: str, spec: vm.CloneSpec) -> Task: ...
-    def InstantClone(self, spec: vm.InstantCloneSpec) -> Task: ...
-    def ExportVm(self) -> HttpNfcLease: ...
-    def MarkAsTemplate(self) -> NoneType: ...
-    def MarkAsVirtualMachine(self, pool: ResourcePool, host: HostSystem) -> NoneType: ...
-    def Unregister(self) -> NoneType: ...
-    def ResetGuestInformation(self) -> NoneType: ...
-    def MountToolsInstaller(self) -> NoneType: ...
-    def UnmountToolsInstaller(self) -> NoneType: ...
-    def UpgradeTools(self, installerOptions: str) -> Task: ...
-    def AcquireMksTicket(self) -> VirtualMachine.MksTicket: ...
-    def QueryConnections(self) -> List[VirtualMachine.Connection]: ...
-    def DropConnections(self, listOfConnections: List[VirtualMachine.Connection]) -> bool: ...
-    def AcquireTicket(self, ticketType: str) -> VirtualMachine.Ticket: ...
-    def SetScreenResolution(self, width: int, height: int) -> NoneType: ...
-    def DefragmentAllDisks(self) -> NoneType: ...
-    def CreateSecondary(self, host: HostSystem) -> Task: ...
-    def CreateSecondaryEx(self, host: HostSystem, spec: vm.FaultToleranceConfigSpec) -> Task: ...
-    def TurnOffFaultTolerance(self) -> Task: ...
-    def MakePrimary(self, vm: VirtualMachine) -> Task: ...
-    def TerminateFaultTolerantVM(self, vm: VirtualMachine) -> Task: ...
-    def DisableSecondary(self, vm: VirtualMachine) -> Task: ...
-    def EnableSecondary(self, vm: VirtualMachine, host: HostSystem) -> Task: ...
-    def SetDisplayTopology(self, displays: List[VirtualMachine.DisplayTopology]) -> NoneType: ...
-    def StartRecording(self, name: str, description: str) -> Task: ...
-    def StopRecording(self) -> Task: ...
-    def StartReplaying(self, replaySnapshot: vm.Snapshot) -> Task: ...
-    def StopReplaying(self) -> Task: ...
-    def PromoteDisks(self, unlink: bool, disks: List[vm.device.VirtualDisk]) -> Task: ...
-    def CreateScreenshot(self) -> Task: ...
-    def PutUsbScanCodes(self, spec: vm.UsbScanCodeSpec) -> int: ...
-    def QueryChangedDiskAreas(self, snapshot: vm.Snapshot, deviceKey: int, startOffset: long, changeId: str) -> VirtualMachine.DiskChangeInfo: ...
-    def QueryUnownedFiles(self) -> List[str]: ...
-    def ReloadFromPath(self, configurationPath: str) -> Task: ...
-    def QueryFaultToleranceCompatibility(self) -> List[vmodl.MethodFault]: ...
-    def QueryFaultToleranceCompatibilityEx(self, forLegacyFt: bool) -> List[vmodl.MethodFault]: ...
-    def Terminate(self) -> NoneType: ...
-    def SendNMI(self) -> NoneType: ...
-    def AttachDisk(self, diskId: vslm.ID, datastore: Datastore, controllerKey: int, unitNumber: int) -> Task: ...
-    def DetachDisk(self, diskId: vslm.ID) -> Task: ...
-    def ApplyEvcMode(self, mask: List[host.FeatureMask], completeMasks: bool) -> Task: ...
-    def CryptoUnlock(self) -> Task: ...
 
+class InvalidVmConfig(VmConfigFault):
+    @property
+    def property(self) -> PropertyPath: ...
+    @property.setter
+    def property(self, value: PropertyPath):
+        self._property = value
 
-    class Connection(vmodl.DynamicData):
-        @property
-        def label(self) -> str: ...
-        @property
-        def client(self) -> str: ...
-        @property
-        def userName(self) -> str: ...
 
+class InvalidVmState(InvalidState):
+    @property
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
 
-    class DiskChangeInfo(vmodl.DynamicData):
-        @property
-        def startOffset(self) -> long: ...
-        @property
-        def length(self) -> long: ...
-        @property
-        def changedArea(self) -> List[VirtualMachine.DiskChangeInfo.DiskChangeExtent]: ...
 
+class InventoryHasStandardAloneHosts(NotEnoughLicenses):
+    @property
+    def hosts(self) -> List[str]: ...
+    @hosts.setter
+    def hosts(self, value: List[str]):
+        self._hosts = value
 
-        class DiskChangeExtent(vmodl.DynamicData):
-            @property
-            def start(self) -> long: ...
-            @property
-            def length(self) -> long: ...
 
+class IpHostnameGeneratorError(CustomizationFault): ...
 
-    class DisplayTopology(vmodl.DynamicData):
-        @property
-        def x(self) -> int: ...
-        @property
-        def y(self) -> int: ...
-        @property
-        def width(self) -> int: ...
-        @property
-        def height(self) -> int: ...
 
+class IscsiFault(VimFault): ...
 
-    class MksConnection(VirtualMachine.Connection): ...
 
+class IscsiFaultInvalidVnic(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class MksTicket(vmodl.DynamicData):
-        @property
-        def ticket(self) -> str: ...
-        @property
-        def cfgFile(self) -> str: ...
-        @property
-        def host(self) -> str: ...
-        @property
-        def port(self) -> int: ...
-        @property
-        def sslThumbprint(self) -> str: ...
 
+class IscsiFaultPnicInUse(IscsiFault):
+    @property
+    def pnicDevice(self) -> str: ...
+    @pnicDevice.setter
+    def pnicDevice(self, value: str):
+        self._pnicDevice = value
 
-    class StorageRequirement(vmodl.DynamicData):
-        @property
-        def datastore(self) -> Datastore: ...
-        @property
-        def freeSpaceRequiredInKb(self) -> long: ...
 
+class IscsiFaultVnicAlreadyBound(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class Ticket(vmodl.DynamicData):
-        @property
-        def ticket(self) -> str: ...
-        @property
-        def cfgFile(self) -> str: ...
-        @property
-        def host(self) -> str: ...
-        @property
-        def port(self) -> int: ...
-        @property
-        def sslThumbprint(self) -> str: ...
-        @property
-        def certThumbprintList(self) -> List[vm.CertThumbprint]: ...
-        @property
-        def url(self) -> str: ...
 
+class IscsiFaultVnicHasActivePaths(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class WipeResult(vmodl.DynamicData):
-        @property
-        def diskId(self) -> int: ...
-        @property
-        def shrinkableDiskSpace(self) -> long: ...
 
+class IscsiFaultVnicHasMultipleUplinks(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class AppHeartbeatStatusType(Enum):
-        appStatusGray = "appstatusgray"
-        appStatusGreen = "appstatusgreen"
-        appStatusRed = "appstatusred"
 
+class IscsiFaultVnicHasNoUplinks(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class FaultToleranceState(Enum):
-        notConfigured = "notconfigured"
-        disabled = "disabled"
-        enabled = "enabled"
-        needSecondary = "needsecondary"
-        starting = "starting"
-        running = "running"
 
+class IscsiFaultVnicHasWrongUplink(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class FaultToleranceType(Enum):
-        unset = "unset"
-        recordReplay = "recordreplay"
-        checkpointing = "checkpointing"
 
+class IscsiFaultVnicInUse(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class MovePriority(Enum):
-        lowPriority = "lowpriority"
-        highPriority = "highpriority"
-        defaultPriority = "defaultpriority"
 
+class IscsiFaultVnicIsLastPath(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class NeedSecondaryReason(Enum):
-        initializing = "initializing"
-        divergence = "divergence"
-        lostConnection = "lostconnection"
-        partialHardwareFailure = "partialhardwarefailure"
-        userAction = "useraction"
-        checkpointError = "checkpointerror"
-        other = "other"
 
+class IscsiFaultVnicNotBound(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-    class RecordReplayState(Enum):
-        recording = "recording"
-        replaying = "replaying"
-        inactive = "inactive"
 
+class IscsiFaultVnicNotFound(IscsiFault):
+    @property
+    def vnicDevice(self) -> str: ...
+    @vnicDevice.setter
+    def vnicDevice(self, value: str):
+        self._vnicDevice = value
 
-class VirtualizationManager(ManagedObject): ...
 
+class KeyNotFound(VimFault):
+    @property
+    def key(self) -> str: ...
+    @key.setter
+    def key(self, value: str):
+        self._key = value
 
-class VsanUpgradeSystem(ManagedObject):
-    def PerformUpgradePreflightCheck(self, cluster: ClusterComputeResource, downgradeFormat: bool) -> VsanUpgradeSystem.PreflightCheckResult: ...
-    def QueryUpgradeStatus(self, cluster: ClusterComputeResource) -> VsanUpgradeSystem.UpgradeStatus: ...
-    def PerformUpgrade(self, cluster: ClusterComputeResource, performObjectUpgrade: bool, downgradeFormat: bool, allowReducedRedundancy: bool, excludeHosts: List[HostSystem]) -> Task: ...
 
+class LargeRDMConversionNotSupported(MigrationFault):
+    @property
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
-    class APIBrokenIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
 
+class LargeRDMNotSupportedOnDatastore(VmConfigFault):
+    @property
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
+    @property
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
+    @property
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
 
-    class AutoClaimEnabledOnHostsIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
 
+class LegacyNetworkInterfaceInUse(CannotAccessNetwork): ...
 
-    class HostsDisconnectedIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
 
+class LicenseAssignmentFailed(vmodl.RuntimeFault):
+    @property
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
 
-    class MissingHostsInClusterIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
 
+class LicenseDowngradeDisallowed(NotEnoughLicenses):
+    @property
+    def edition(self) -> str: ...
+    @edition.setter
+    def edition(self, value: str):
+        self._edition = value
+    @property
+    def entityId(self) -> str: ...
+    @entityId.setter
+    def entityId(self, value: str):
+        self._entityId = value
+    @property
+    def features(self) -> List[vmodl.KeyAnyValue]: ...
+    @features.setter
+    def features(self, value: List[vmodl.KeyAnyValue]):
+        self._features = value
 
-    class NetworkPartitionInfo(vmodl.DynamicData):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
 
+class LicenseEntityNotFound(VimFault):
+    @property
+    def entityId(self) -> str: ...
+    @entityId.setter
+    def entityId(self, value: str):
+        self._entityId = value
 
-    class NetworkPartitionIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def partitions(self) -> List[VsanUpgradeSystem.NetworkPartitionInfo]: ...
 
+class LicenseExpired(NotEnoughLicenses):
+    @property
+    def licenseKey(self) -> str: ...
+    @licenseKey.setter
+    def licenseKey(self, value: str):
+        self._licenseKey = value
 
-    class NotEnoughFreeCapacityIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def reducedRedundancyUpgradePossible(self) -> bool: ...
 
+class LicenseKeyEntityMismatch(NotEnoughLicenses): ...
 
-    class PreflightCheckIssue(vmodl.DynamicData):
-        @property
-        def msg(self) -> str: ...
 
+class LicenseRestricted(NotEnoughLicenses): ...
 
-    class PreflightCheckResult(vmodl.DynamicData):
-        @property
-        def issues(self) -> List[VsanUpgradeSystem.PreflightCheckIssue]: ...
-        @property
-        def diskMappingToRestore(self) -> vsan.host.DiskMapping: ...
 
+class LicenseServerUnavailable(VimFault):
+    @property
+    def licenseServer(self) -> str: ...
+    @licenseServer.setter
+    def licenseServer(self, value: str):
+        self._licenseServer = value
 
-    class RogueHostsInClusterIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def uuids(self) -> List[str]: ...
 
+class LicenseSourceUnavailable(NotEnoughLicenses):
+    @property
+    def licenseSource(self) -> vim.LicenseManager.LicenseSource: ...
+    @licenseSource.setter
+    def licenseSource(self, value: vim.LicenseManager.LicenseSource):
+        self._licenseSource = value
 
-    class UpgradeHistoryDiskGroupOp(VsanUpgradeSystem.UpgradeHistoryItem):
-        @property
-        def operation(self) -> str: ...
-        @property
-        def diskMapping(self) -> vsan.host.DiskMapping: ...
 
+class LimitExceeded(VimFault):
+    @property
+    def property(self) -> PropertyPath: ...
+    @property.setter
+    def property(self, value: PropertyPath):
+        self._property = value
+    @property
+    def limit(self) -> int: ...
+    @limit.setter
+    def limit(self, value: int):
+        self._limit = value
 
-    class UpgradeHistoryItem(vmodl.DynamicData):
-        @property
-        def timestamp(self) -> datetime: ...
-        @property
-        def host(self) -> HostSystem: ...
-        @property
-        def message(self) -> str: ...
-        @property
-        def task(self) -> Task: ...
 
+class LinuxVolumeNotClean(CustomizationFault): ...
 
-    class UpgradeHistoryPreflightFail(VsanUpgradeSystem.UpgradeHistoryItem):
-        @property
-        def preflightResult(self) -> VsanUpgradeSystem.PreflightCheckResult: ...
 
+class LogBundlingFailed(VimFault): ...
 
-    class UpgradeStatus(vmodl.DynamicData):
-        @property
-        def inProgress(self) -> bool: ...
-        @property
-        def history(self) -> List[VsanUpgradeSystem.UpgradeHistoryItem]: ...
-        @property
-        def aborted(self) -> bool: ...
-        @property
-        def completed(self) -> bool: ...
-        @property
-        def progress(self) -> int: ...
 
-
-    class V2ObjectsPresentDuringDowngradeIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def uuids(self) -> List[str]: ...
+class MaintenanceModeFileMove(MigrationFault): ...
 
 
-    class WrongEsxVersionIssue(VsanUpgradeSystem.PreflightCheckIssue):
-        @property
-        def hosts(self) -> List[HostSystem]: ...
+class MemoryFileFormatNotSupportedByDatastore(UnsupportedDatastore):
+    @property
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
+    @property
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
 
 
-    class UpgradeHistoryDiskGroupOpType(Enum):
-        add = "add"
-        remove = "remove"
+class MemoryHotPlugNotSupported(VmConfigFault): ...
 
 
-class AboutInfo(vmodl.DynamicData):
-    @property
-    def name(self) -> str: ...
+class MemorySizeNotRecommended(VirtualHardwareCompatibilityIssue):
     @property
-    def fullName(self) -> str: ...
+    def memorySizeMB(self) -> int: ...
+    @memorySizeMB.setter
+    def memorySizeMB(self, value: int):
+        self._memorySizeMB = value
     @property
-    def vendor(self) -> str: ...
+    def minMemorySizeMB(self) -> int: ...
+    @minMemorySizeMB.setter
+    def minMemorySizeMB(self, value: int):
+        self._minMemorySizeMB = value
     @property
-    def version(self) -> str: ...
-    @property
-    def patchLevel(self) -> str: ...
-    @property
-    def build(self) -> str: ...
-    @property
-    def localeVersion(self) -> str: ...
-    @property
-    def localeBuild(self) -> str: ...
-    @property
-    def osType(self) -> str: ...
+    def maxMemorySizeMB(self) -> int: ...
+    @maxMemorySizeMB.setter
+    def maxMemorySizeMB(self, value: int):
+        self._maxMemorySizeMB = value
+
+
+class MemorySizeNotSupported(VirtualHardwareCompatibilityIssue):
     @property
-    def productLineId(self) -> str: ...
+    def memorySizeMB(self) -> int: ...
+    @memorySizeMB.setter
+    def memorySizeMB(self, value: int):
+        self._memorySizeMB = value
     @property
-    def apiType(self) -> str: ...
+    def minMemorySizeMB(self) -> int: ...
+    @minMemorySizeMB.setter
+    def minMemorySizeMB(self, value: int):
+        self._minMemorySizeMB = value
     @property
-    def apiVersion(self) -> str: ...
+    def maxMemorySizeMB(self) -> int: ...
+    @maxMemorySizeMB.setter
+    def maxMemorySizeMB(self, value: int):
+        self._maxMemorySizeMB = value
+
+
+class MemorySizeNotSupportedByDatastore(VirtualHardwareCompatibilityIssue):
     @property
-    def instanceUuid(self) -> str: ...
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
     @property
-    def licenseProductName(self) -> str: ...
+    def memorySizeMB(self) -> int: ...
+    @memorySizeMB.setter
+    def memorySizeMB(self, value: int):
+        self._memorySizeMB = value
     @property
-    def licenseProductVersion(self) -> str: ...
+    def maxMemorySizeMB(self) -> int: ...
+    @maxMemorySizeMB.setter
+    def maxMemorySizeMB(self, value: int):
+        self._maxMemorySizeMB = value
 
 
-class AuthorizationDescription(vmodl.DynamicData):
-    @property
-    def privilege(self) -> List[ElementDescription]: ...
-    @property
-    def privilegeGroup(self) -> List[ElementDescription]: ...
+class MemorySnapshotOnIndependentDisk(SnapshotFault): ...
 
 
-class BatchResult(vmodl.DynamicData):
-    @property
-    def result(self) -> str: ...
+class MethodAlreadyDisabledFault(vmodl.RuntimeFault):
     @property
-    def hostKey(self) -> str: ...
-    @property
-    def ds(self) -> Datastore: ...
+    def sourceId(self) -> str: ...
+    @sourceId.setter
+    def sourceId(self, value: str):
+        self._sourceId = value
+
+
+class MethodDisabled(vmodl.RuntimeFault):
     @property
-    def fault(self) -> vmodl.MethodFault: ...
+    def source(self) -> str: ...
+    @source.setter
+    def source(self, value: str):
+        self._source = value
 
 
-    class Result(Enum):
-        success = "success"
-        fail = "fail"
+class MigrationDisabled(MigrationFault): ...
 
 
-class BoolPolicy(InheritablePolicy):
-    @property
-    def value(self) -> bool: ...
+class MigrationFault(VimFault): ...
 
 
-class Capability(vmodl.DynamicData):
-    @property
-    def provisioningSupported(self) -> bool: ...
-    @property
-    def multiHostSupported(self) -> bool: ...
-    @property
-    def userShellAccessSupported(self) -> bool: ...
-    @property
-    def supportedEVCMode(self) -> List[EVCMode]: ...
-    @property
-    def supportedEVCGraphicsMode(self) -> List[FeatureEVCMode]: ...
+class MigrationFeatureNotSupported(MigrationFault):
     @property
-    def networkBackupAndRestoreSupported(self) -> bool: ...
+    def atSourceHost(self) -> bool: ...
+    @atSourceHost.setter
+    def atSourceHost(self, value: bool):
+        self._atSourceHost = value
     @property
-    def ftDrsWithoutEvcSupported(self) -> bool: ...
+    def failedHostName(self) -> str: ...
+    @failedHostName.setter
+    def failedHostName(self, value: str):
+        self._failedHostName = value
     @property
-    def hciWorkflowSupported(self) -> bool: ...
-    @property
-    def computePolicyVersion(self) -> int: ...
-    @property
-    def clusterPlacementSupported(self) -> bool: ...
+    def failedHost(self) -> vim.HostSystem: ...
+    @failedHost.setter
+    def failedHost(self, value: vim.HostSystem):
+        self._failedHost = value
+
+
+class MigrationNotReady(MigrationFault):
     @property
-    def lifecycleManagementSupported(self) -> bool: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
+
+
+class MismatchedBundle(VimFault):
     @property
-    def hostSeedingSupported(self) -> bool: ...
+    def bundleUuid(self) -> str: ...
+    @bundleUuid.setter
+    def bundleUuid(self, value: str):
+        self._bundleUuid = value
     @property
-    def scalableSharesSupported(self) -> bool: ...
+    def hostUuid(self) -> str: ...
+    @hostUuid.setter
+    def hostUuid(self, value: str):
+        self._hostUuid = value
     @property
-    def hadcsSupported(self) -> bool: ...
+    def bundleBuildNumber(self) -> int: ...
+    @bundleBuildNumber.setter
+    def bundleBuildNumber(self, value: int):
+        self._bundleBuildNumber = value
     @property
-    def configMgmtSupported(self) -> bool: ...
+    def hostBuildNumber(self) -> int: ...
+    @hostBuildNumber.setter
+    def hostBuildNumber(self, value: int):
+        self._hostBuildNumber = value
 
 
-class CustomizationSpecInfo(vmodl.DynamicData):
+class MismatchedNetworkPolicies(MigrationFault):
     @property
-    def name(self) -> str: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def description(self) -> str: ...
-    @property
-    def type(self) -> str: ...
-    @property
-    def changeVersion(self) -> str: ...
+    def backing(self) -> str: ...
+    @backing.setter
+    def backing(self, value: str):
+        self._backing = value
     @property
-    def lastUpdateTime(self) -> datetime: ...
+    def connected(self) -> bool: ...
+    @connected.setter
+    def connected(self, value: bool):
+        self._connected = value
 
 
-class CustomizationSpecItem(vmodl.DynamicData):
+class MismatchedVMotionNetworkNames(MigrationFault):
     @property
-    def info(self) -> CustomizationSpecInfo: ...
+    def sourceNetwork(self) -> str: ...
+    @sourceNetwork.setter
+    def sourceNetwork(self, value: str):
+        self._sourceNetwork = value
     @property
-    def spec(self) -> vm.customization.Specification: ...
+    def destNetwork(self) -> str: ...
+    @destNetwork.setter
+    def destNetwork(self, value: str):
+        self._destNetwork = value
 
 
-class Description(vmodl.DynamicData):
-    @property
-    def label(self) -> str: ...
-    @property
-    def summary(self) -> str: ...
+class MissingBmcSupport(VimFault): ...
+
+
+class MissingController(InvalidDeviceSpec): ...
+
+
+class MissingIpPool(VAppPropertyFault): ...
+
+
+class MissingLinuxCustResources(CustomizationFault): ...
+
 
+class MissingNetworkIpConfig(VAppPropertyFault): ...
 
-class DesiredSoftwareSpec(vmodl.DynamicData):
+
+class MissingPowerOffConfiguration(VAppConfigFault): ...
+
+
+class MissingPowerOnConfiguration(VAppConfigFault): ...
+
+
+class MissingWindowsCustResources(CustomizationFault): ...
+
+
+class MksConnectionLimitReached(InvalidState):
     @property
-    def baseImageSpec(self) -> DesiredSoftwareSpec.BaseImageSpec: ...
+    def connectionLimit(self) -> int: ...
+    @connectionLimit.setter
+    def connectionLimit(self, value: int):
+        self._connectionLimit = value
+
+
+class MountError(CustomizationFault):
     @property
-    def vendorAddOnSpec(self) -> DesiredSoftwareSpec.VendorAddOnSpec: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def components(self) -> List[DesiredSoftwareSpec.ComponentSpec]: ...
+    def diskIndex(self) -> int: ...
+    @diskIndex.setter
+    def diskIndex(self, value: int):
+        self._diskIndex = value
 
 
-    class BaseImageSpec(vmodl.DynamicData):
-        @property
-        def version(self) -> str: ...
+class MultiWriterNotSupported(DeviceNotSupported): ...
 
 
-    class ComponentSpec(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def version(self) -> str: ...
+class MultipleCertificatesVerifyFault(HostConnectFault):
+    @property
+    def thumbprintData(self) -> List[MultipleCertificatesVerifyFault.ThumbprintData]: ...
+    @thumbprintData.setter
+    def thumbprintData(self, value: List[MultipleCertificatesVerifyFault.ThumbprintData]):
+        self._thumbprintData = value
 
 
-    class VendorAddOnSpec(vmodl.DynamicData):
+    class ThumbprintData(vmodl.DynamicData):
         @property
-        def name(self) -> str: ...
+        def port(self) -> int: ...
+        @port.setter
+        def port(self, value: int):
+            self._port = value
         @property
-        def version(self) -> str: ...
+        def thumbprint(self) -> str: ...
+        @thumbprint.setter
+        def thumbprint(self, value: str):
+            self._thumbprint = value
 
 
-class EVCMode(ElementDescription):
-    @property
-    def guaranteedCPUFeatures(self) -> List[host.CpuIdInfo]: ...
-    @property
-    def featureCapability(self) -> List[host.FeatureCapability]: ...
-    @property
-    def featureMask(self) -> List[host.FeatureMask]: ...
-    @property
-    def featureRequirement(self) -> List[vm.FeatureRequirement]: ...
+class MultipleSnapshotsNotSupported(SnapshotFault): ...
+
+
+class NamespaceFull(VimFault):
     @property
-    def vendor(self) -> str: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def track(self) -> List[str]: ...
+    def currentMaxSize(self) -> long: ...
+    @currentMaxSize.setter
+    def currentMaxSize(self, value: long):
+        self._currentMaxSize = value
     @property
-    def vendorTier(self) -> int: ...
+    def requiredSize(self) -> long: ...
+    @requiredSize.setter
+    def requiredSize(self, value: long):
+        self._requiredSize = value
 
 
-class ElementDescription(Description):
+class NamespaceLimitReached(VimFault):
     @property
-    def key(self) -> str: ...
+    def limit(self) -> int: ...
+    @limit.setter
+    def limit(self, value: int):
+        self._limit = value
 
 
-class EnumDescription(vmodl.DynamicData):
+class NamespaceWriteProtected(VimFault):
     @property
-    def key(self) -> type: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class NasConfigFault(HostConfigFault):
     @property
-    def tags(self) -> List[ElementDescription]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-class ExtendedDescription(Description):
+class NasConnectionLimitReached(NasConfigFault):
     @property
-    def messageCatalogKeyPrefix(self) -> str: ...
+    def remoteHost(self) -> str: ...
+    @remoteHost.setter
+    def remoteHost(self, value: str):
+        self._remoteHost = value
     @property
-    def messageArg(self) -> List[vmodl.KeyAnyValue]: ...
+    def remotePath(self) -> str: ...
+    @remotePath.setter
+    def remotePath(self, value: str):
+        self._remotePath = value
 
 
-class ExtendedElementDescription(ElementDescription):
+class NasSessionCredentialConflict(NasConfigFault):
+    @property
+    def remoteHost(self) -> str: ...
+    @remoteHost.setter
+    def remoteHost(self, value: str):
+        self._remoteHost = value
     @property
-    def messageCatalogKeyPrefix(self) -> str: ...
+    def remotePath(self) -> str: ...
+    @remotePath.setter
+    def remotePath(self, value: str):
+        self._remotePath = value
     @property
-    def messageArg(self) -> List[vmodl.KeyAnyValue]: ...
+    def userName(self) -> str: ...
+    @userName.setter
+    def userName(self, value: str):
+        self._userName = value
 
 
-class Extension(vmodl.DynamicData):
+class NasVolumeNotMounted(NasConfigFault):
     @property
-    def description(self) -> Description: ...
+    def remoteHost(self) -> str: ...
+    @remoteHost.setter
+    def remoteHost(self, value: str):
+        self._remoteHost = value
     @property
-    def key(self) -> str: ...
-    @property
-    def company(self) -> str: ...
+    def remotePath(self) -> str: ...
+    @remotePath.setter
+    def remotePath(self, value: str):
+        self._remotePath = value
+
+
+class NetworkCopyFault(FileFault): ...
+
+
+class NetworkDisruptedAndConfigRolledBack(VimFault):
     @property
-    def type(self) -> str: ...
+    def host(self) -> str: ...
+    @host.setter
+    def host(self, value: str):
+        self._host = value
+
+
+class NetworkInaccessible(NasConfigFault): ...
+
+
+class NetworksMayNotBeTheSame(MigrationFault):
     @property
-    def version(self) -> str: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class NicSettingMismatch(CustomizationFault):
     @property
-    def subjectName(self) -> str: ...
+    def numberOfNicsInSpec(self) -> int: ...
+    @numberOfNicsInSpec.setter
+    def numberOfNicsInSpec(self, value: int):
+        self._numberOfNicsInSpec = value
     @property
-    def server(self) -> List[Extension.ServerInfo]: ...
+    def numberOfNicsInVM(self) -> int: ...
+    @numberOfNicsInVM.setter
+    def numberOfNicsInVM(self, value: int):
+        self._numberOfNicsInVM = value
+
+
+class NoActiveHostInCluster(InvalidState):
     @property
-    def client(self) -> List[Extension.ClientInfo]: ...
+    def computeResource(self) -> vim.ComputeResource: ...
+    @computeResource.setter
+    def computeResource(self, value: vim.ComputeResource):
+        self._computeResource = value
+
+
+class NoAvailableIp(VAppPropertyFault):
     @property
-    def taskList(self) -> List[Extension.TaskTypeInfo]: ...
+    def network(self) -> vim.Network: ...
+    @network.setter
+    def network(self, value: vim.Network):
+        self._network = value
+
+
+class NoClientCertificate(VimFault): ...
+
+
+class NoCompatibleDatastore(VimFault): ...
+
+
+class NoCompatibleHardAffinityHost(VmConfigFault):
     @property
-    def eventList(self) -> List[Extension.EventTypeInfo]: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+class NoCompatibleHost(VimFault):
     @property
-    def faultList(self) -> List[Extension.FaultTypeInfo]: ...
+    def host(self) -> List[vim.HostSystem]: ...
+    @host.setter
+    def host(self, value: List[vim.HostSystem]):
+        self._host = value
     @property
-    def privilegeList(self) -> List[Extension.PrivilegeInfo]: ...
+    def error(self) -> List[vmodl.MethodFault]: ...
+    @error.setter
+    def error(self, value: List[vmodl.MethodFault]):
+        self._error = value
+
+
+class NoCompatibleHostWithAccessToDevice(NoCompatibleHost): ...
+
+
+class NoCompatibleSoftAffinityHost(VmConfigFault):
     @property
-    def resourceList(self) -> List[Extension.ResourceInfo]: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+class NoConnectedDatastore(VimFault): ...
+
+
+class NoDiskFound(VimFault): ...
+
+
+class NoDiskSpace(FileFault):
     @property
-    def lastHeartbeatTime(self) -> datetime: ...
+    def datastore(self) -> str: ...
+    @datastore.setter
+    def datastore(self, value: str):
+        self._datastore = value
+
+
+class NoDisksToCustomize(CustomizationFault): ...
+
+
+class NoGateway(HostConfigFault): ...
+
+
+class NoGuestHeartbeat(MigrationFault): ...
+
+
+class NoHost(HostConnectFault):
     @property
-    def healthInfo(self) -> Extension.HealthInfo: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class NoHostSuitableForFtSecondary(VmFaultToleranceIssue):
     @property
-    def ovfConsumerInfo(self) -> Extension.OvfConsumerInfo: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def extendedProductInfo(self) -> ext.ExtendedProductInfo: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+class NoLicenseServerConfigured(NotEnoughLicenses): ...
+
+
+class NoPeerHostFound(HostPowerOpFailed): ...
+
+
+class NoPermission(SecurityError):
     @property
-    def managedEntityInfo(self) -> List[ext.ManagedEntityInfo]: ...
+    def object(self) -> ManagedObject: ...
+    @object.setter
+    def object(self, value: ManagedObject):
+        self._object = value
     @property
-    def shownInSolutionManager(self) -> bool: ...
+    def privilegeId(self) -> str: ...
+    @privilegeId.setter
+    def privilegeId(self, value: str):
+        self._privilegeId = value
     @property
-    def solutionManagerInfo(self) -> ext.SolutionManagerInfo: ...
+    def missingPrivileges(self) -> List[NoPermission.EntityPrivileges]: ...
+    @missingPrivileges.setter
+    def missingPrivileges(self, value: List[NoPermission.EntityPrivileges]):
+        self._missingPrivileges = value
 
 
-    class ClientInfo(vmodl.DynamicData):
-        @property
-        def version(self) -> str: ...
-        @property
-        def description(self) -> Description: ...
+    class EntityPrivileges(vmodl.DynamicData):
         @property
-        def company(self) -> str: ...
-        @property
-        def type(self) -> str: ...
+        def entity(self) -> ManagedObject: ...
+        @entity.setter
+        def entity(self, value: ManagedObject):
+            self._entity = value
         @property
-        def url(self) -> str: ...
+        def privilegeIds(self) -> List[str]: ...
+        @privilegeIds.setter
+        def privilegeIds(self, value: List[str]):
+            self._privilegeIds = value
 
 
-    class EventTypeInfo(vmodl.DynamicData):
-        @property
-        def eventID(self) -> str: ...
-        @property
-        def eventTypeSchema(self) -> str: ...
+class NoPermissionOnAD(ActiveDirectoryFault): ...
 
 
-    class FaultTypeInfo(vmodl.DynamicData):
-        @property
-        def faultID(self) -> str: ...
+class NoPermissionOnHost(HostConnectFault): ...
 
 
-    class HealthInfo(vmodl.DynamicData):
-        @property
-        def url(self) -> str: ...
+class NoPermissionOnNasVolume(NasConfigFault):
+    @property
+    def userName(self) -> str: ...
+    @userName.setter
+    def userName(self, value: str):
+        self._userName = value
 
 
-    class OvfConsumerInfo(vmodl.DynamicData):
-        @property
-        def callbackUrl(self) -> str: ...
-        @property
-        def sectionType(self) -> List[str]: ...
+class NoSubjectName(VimFault): ...
 
 
-    class PrivilegeInfo(vmodl.DynamicData):
-        @property
-        def privID(self) -> str: ...
-        @property
-        def privGroupName(self) -> str: ...
+class NoVcManagedIpConfigured(VAppPropertyFault): ...
 
 
-    class ResourceInfo(vmodl.DynamicData):
-        @property
-        def locale(self) -> str: ...
-        @property
-        def module(self) -> str: ...
-        @property
-        def data(self) -> List[KeyValue]: ...
+class NoVirtualNic(HostConfigFault): ...
 
 
-    class ServerInfo(vmodl.DynamicData):
-        @property
-        def url(self) -> str: ...
-        @property
-        def description(self) -> Description: ...
-        @property
-        def company(self) -> str: ...
-        @property
-        def type(self) -> str: ...
-        @property
-        def adminEmail(self) -> List[str]: ...
-        @property
-        def serverThumbprint(self) -> str: ...
+class NoVmInVApp(VAppConfigFault): ...
 
 
-    class TaskTypeInfo(vmodl.DynamicData):
-        @property
-        def taskID(self) -> str: ...
+class NonADUserRequired(ActiveDirectoryFault): ...
 
 
-class FaultsByHost(vmodl.DynamicData):
-    @property
-    def host(self) -> HostSystem: ...
+class NonHomeRDMVMotionNotSupported(MigrationFeatureNotSupported):
     @property
-    def faults(self) -> List[vmodl.MethodFault]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
 
-class FaultsByVM(vmodl.DynamicData):
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def faults(self) -> List[vmodl.MethodFault]: ...
+class NonPersistentDisksNotSupported(DeviceNotSupported): ...
 
 
-class FeatureEVCMode(ElementDescription):
-    @property
-    def mask(self) -> List[host.FeatureMask]: ...
+class NonVmwareOuiMacNotSupportedHost(NotSupportedHost):
     @property
-    def capability(self) -> List[host.FeatureCapability]: ...
-    @property
-    def requirement(self) -> List[vm.FeatureRequirement]: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-class ReplicationVmInfo(vmodl.DynamicData):
-    @property
-    def state(self) -> str: ...
-    @property
-    def progressInfo(self) -> HbrManager.ReplicationVmInfo.ProgressInfo: ...
-    @property
-    def imageId(self) -> str: ...
-    @property
-    def lastError(self) -> vmodl.MethodFault: ...
+class NotADirectory(FileFault): ...
 
 
-    class State(Enum):
-        none = "none"
-        paused = "paused"
-        syncing = "syncing"
-        idle = "idle"
-        active = "active"
-        error = "error"
+class NotAFile(FileFault): ...
 
 
-class ProgressInfo(vmodl.DynamicData):
-    @property
-    def progress(self) -> int: ...
-    @property
-    def bytesTransferred(self) -> long: ...
-    @property
-    def bytesToTransfer(self) -> long: ...
-    @property
-    def checksumTotalBytes(self) -> long: ...
-    @property
-    def checksumComparedBytes(self) -> long: ...
+class NotAuthenticated(NoPermission): ...
 
 
-class VmReplicationCapability(vmodl.DynamicData):
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def supportedQuiesceMode(self) -> str: ...
-    @property
-    def compressionSupported(self) -> bool: ...
+class NotEnoughCpus(VirtualHardwareCompatibilityIssue):
     @property
-    def maxSupportedSourceDiskCapacity(self) -> long: ...
+    def numCpuDest(self) -> int: ...
+    @numCpuDest.setter
+    def numCpuDest(self, value: int):
+        self._numCpuDest = value
     @property
-    def minRpo(self) -> long: ...
+    def numCpuVm(self) -> int: ...
+    @numCpuVm.setter
+    def numCpuVm(self, value: int):
+        self._numCpuVm = value
+
+
+class NotEnoughLogicalCpus(NotEnoughCpus):
     @property
-    def fault(self) -> vmodl.MethodFault: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
 
 
-    class QuiesceMode(Enum):
-        application = "application"
-        filesystem = "filesystem"
-        none = "none"
+class NotFound(VimFault): ...
 
 
-class HealthUpdate(vmodl.DynamicData):
+class NotSupportedDeviceForFT(VmFaultToleranceIssue):
     @property
-    def entity(self) -> ManagedEntity: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def healthUpdateInfoId(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def id(self) -> str: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def status(self) -> ManagedEntity.Status: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def remediation(self) -> str: ...
+    def deviceType(self) -> str: ...
+    @deviceType.setter
+    def deviceType(self, value: str):
+        self._deviceType = value
+    @property
+    def deviceLabel(self) -> str: ...
+    @deviceLabel.setter
+    def deviceLabel(self, value: str):
+        self._deviceLabel = value
 
 
-class HealthUpdateInfo(vmodl.DynamicData):
-    @property
-    def id(self) -> str: ...
+    class DeviceType(Enum):
+        virtualVmxnet3 = "virtualVmxnet3"
+        paraVirtualSCSIController = "paraVirtualSCSIController"
+
+
+class NotSupportedHost(HostConnectFault):
     @property
-    def componentType(self) -> str: ...
+    def productName(self) -> str: ...
+    @productName.setter
+    def productName(self, value: str):
+        self._productName = value
     @property
-    def description(self) -> str: ...
+    def productVersion(self) -> str: ...
+    @productVersion.setter
+    def productVersion(self, value: str):
+        self._productVersion = value
 
 
-    class ComponentType(Enum):
-        Memory = "memory"
-        Power = "power"
-        Fan = "fan"
-        Network = "network"
-        Storage = "storage"
+class NotSupportedHostForChecksum(VimFault): ...
 
 
-class HistoricalInterval(vmodl.DynamicData):
-    @property
-    def key(self) -> int: ...
-    @property
-    def samplingPeriod(self) -> int: ...
+class NotSupportedHostForVFlash(NotSupportedHost):
     @property
-    def name(self) -> str: ...
-    @property
-    def length(self) -> int: ...
-    @property
-    def level(self) -> int: ...
-    @property
-    def enabled(self) -> bool: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-class HostServiceTicket(vmodl.DynamicData):
-    @property
-    def host(self) -> str: ...
+class NotSupportedHostForVmcp(NotSupportedHost):
     @property
-    def port(self) -> int: ...
-    @property
-    def sslThumbprint(self) -> str: ...
-    @property
-    def service(self) -> str: ...
-    @property
-    def serviceVersion(self) -> str: ...
-    @property
-    def sessionId(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-class ImportSpec(vmodl.DynamicData):
-    @property
-    def entityConfig(self) -> vApp.EntityConfigInfo: ...
+class NotSupportedHostForVmemFile(NotSupportedHost):
     @property
-    def instantiationOst(self) -> OvfConsumer.OstNode: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-class InheritablePolicy(vmodl.DynamicData):
+class NotSupportedHostForVsan(NotSupportedHost):
     @property
-    def inherited(self) -> bool: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+
 
+class NotSupportedHostInCluster(NotSupportedHost): ...
 
-class IntExpression(NegatableExpression):
+
+class NotSupportedHostInDvs(NotSupportedHost):
     @property
-    def value(self) -> int: ...
+    def switchProductSpec(self) -> vim.dvs.ProductSpec: ...
+    @switchProductSpec.setter
+    def switchProductSpec(self, value: vim.dvs.ProductSpec):
+        self._switchProductSpec = value
 
 
-class IntPolicy(InheritablePolicy):
+class NotSupportedHostInHACluster(NotSupportedHost):
+    @property
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def value(self) -> int: ...
+    def build(self) -> str: ...
+    @build.setter
+    def build(self, value: str):
+        self._build = value
 
 
-class IpAddress(NegatableExpression): ...
+class NotUserConfigurableProperty(VAppPropertyFault): ...
 
 
-class IpRange(IpAddress):
+class NumVirtualCoresPerSocketNotSupported(VirtualHardwareCompatibilityIssue):
     @property
-    def addressPrefix(self) -> str: ...
+    def maxSupportedCoresPerSocketDest(self) -> int: ...
+    @maxSupportedCoresPerSocketDest.setter
+    def maxSupportedCoresPerSocketDest(self, value: int):
+        self._maxSupportedCoresPerSocketDest = value
     @property
-    def prefixLength(self) -> int: ...
+    def numCoresPerSocketVm(self) -> int: ...
+    @numCoresPerSocketVm.setter
+    def numCoresPerSocketVm(self, value: int):
+        self._numCoresPerSocketVm = value
 
 
-class KeyValue(vmodl.DynamicData):
-    @property
-    def key(self) -> str: ...
+class NumVirtualCpusExceedsLimit(InsufficientResourcesFault):
     @property
-    def value(self) -> str: ...
+    def maxSupportedVcpus(self) -> int: ...
+    @maxSupportedVcpus.setter
+    def maxSupportedVcpus(self, value: int):
+        self._maxSupportedVcpus = value
 
 
-class LatencySensitivity(vmodl.DynamicData):
+class NumVirtualCpusIncompatible(VmConfigFault):
     @property
-    def level(self) -> LatencySensitivity.SensitivityLevel: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def sensitivity(self) -> int: ...
-
-
-    class SensitivityLevel(Enum):
-        low = "low"
-        normal = "normal"
-        medium = "medium"
-        high = "high"
-        custom = "custom"
+    def numCpu(self) -> int: ...
+    @numCpu.setter
+    def numCpu(self, value: int):
+        self._numCpu = value
 
 
-class LongPolicy(InheritablePolicy):
+class NumVirtualCpusNotSupported(VirtualHardwareCompatibilityIssue):
     @property
-    def value(self) -> long: ...
+    def maxSupportedVcpusDest(self) -> int: ...
+    @maxSupportedVcpusDest.setter
+    def maxSupportedVcpusDest(self, value: int):
+        self._maxSupportedVcpusDest = value
+    @property
+    def numCpuVm(self) -> int: ...
+    @numCpuVm.setter
+    def numCpuVm(self, value: int):
+        self._numCpuVm = value
 
 
-class MacAddress(NegatableExpression): ...
+class OperationDisabledByGuest(GuestOperationsFault): ...
 
 
-class MacRange(MacAddress):
-    @property
-    def address(self) -> str: ...
-    @property
-    def mask(self) -> str: ...
+class OperationDisallowedOnHost(vmodl.RuntimeFault): ...
 
 
-class MethodDescription(Description):
-    @property
-    def key(self) -> ManagedMethod: ...
+class OperationNotSupportedByGuest(GuestOperationsFault): ...
 
 
-class NegatableExpression(vmodl.DynamicData):
+class OutOfBounds(VimFault):
     @property
-    def negate(self) -> bool: ...
+    def argumentName(self) -> PropertyPath: ...
+    @argumentName.setter
+    def argumentName(self, value: PropertyPath):
+        self._argumentName = value
 
 
-class NumericRange(vmodl.DynamicData):
+class OvfAttribute(OvfInvalidPackage):
     @property
-    def start(self) -> int: ...
+    def elementName(self) -> str: ...
+    @elementName.setter
+    def elementName(self, value: str):
+        self._elementName = value
     @property
-    def end(self) -> int: ...
+    def attributeName(self) -> str: ...
+    @attributeName.setter
+    def attributeName(self, value: str):
+        self._attributeName = value
 
 
-class OstNode(vmodl.DynamicData):
-    @property
-    def id(self) -> str: ...
-    @property
-    def type(self) -> str: ...
-    @property
-    def section(self) -> List[OvfConsumer.OvfSection]: ...
-    @property
-    def child(self) -> List[OvfConsumer.OstNode]: ...
-    @property
-    def entity(self) -> ManagedEntity: ...
+class OvfConnectedDevice(OvfHardwareExport): ...
 
 
-class OvfSection(vmodl.DynamicData):
+class OvfConnectedDeviceFloppy(OvfConnectedDevice):
     @property
-    def lineNumber(self) -> int: ...
-    @property
-    def xml(self) -> str: ...
+    def filename(self) -> str: ...
+    @filename.setter
+    def filename(self, value: str):
+        self._filename = value
 
 
-class PasswordField(vmodl.DynamicData):
+class OvfConnectedDeviceIso(OvfConnectedDevice):
     @property
-    def value(self) -> str: ...
+    def filename(self) -> str: ...
+    @filename.setter
+    def filename(self, value: str):
+        self._filename = value
 
 
-class PerformanceDescription(vmodl.DynamicData):
+class OvfConstraint(OvfInvalidPackage):
     @property
-    def counterType(self) -> List[ElementDescription]: ...
-    @property
-    def statsType(self) -> List[ElementDescription]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-class PosixUserSearchResult(UserSearchResult):
+class OvfConsumerCallbackFault(OvfFault):
     @property
-    def id(self) -> int: ...
+    def extensionKey(self) -> str: ...
+    @extensionKey.setter
+    def extensionKey(self, value: str):
+        self._extensionKey = value
     @property
-    def shellAccess(self) -> bool: ...
+    def extensionName(self) -> str: ...
+    @extensionName.setter
+    def extensionName(self, value: str):
+        self._extensionName = value
 
 
-class PrivilegePolicyDef(vmodl.DynamicData):
+class OvfConsumerCommunicationError(OvfConsumerCallbackFault):
     @property
-    def createPrivilege(self) -> str: ...
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
+
+
+class OvfConsumerFault(OvfConsumerCallbackFault):
     @property
-    def readPrivilege(self) -> str: ...
+    def errorKey(self) -> str: ...
+    @errorKey.setter
+    def errorKey(self, value: str):
+        self._errorKey = value
     @property
-    def updatePrivilege(self) -> str: ...
+    def message(self) -> str: ...
+    @message.setter
+    def message(self, value: str):
+        self._message = value
     @property
-    def deletePrivilege(self) -> str: ...
+    def params(self) -> List[vim.KeyValue]: ...
+    @params.setter
+    def params(self, value: List[vim.KeyValue]):
+        self._params = value
 
 
-class ResourceAllocationInfo(vmodl.DynamicData):
-    @property
-    def reservation(self) -> long: ...
+class OvfConsumerInvalidSection(OvfConsumerCallbackFault):
     @property
-    def expandableReservation(self) -> bool: ...
+    def lineNumber(self) -> int: ...
+    @lineNumber.setter
+    def lineNumber(self, value: int):
+        self._lineNumber = value
     @property
-    def limit(self) -> long: ...
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
+
+
+class OvfConsumerPowerOnFault(InvalidState):
+    @property
+    def extensionKey(self) -> str: ...
+    @extensionKey.setter
+    def extensionKey(self, value: str):
+        self._extensionKey = value
+    @property
+    def extensionName(self) -> str: ...
+    @extensionName.setter
+    def extensionName(self, value: str):
+        self._extensionName = value
     @property
-    def shares(self) -> SharesInfo: ...
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
+
+
+class OvfConsumerUndeclaredSection(OvfConsumerCallbackFault):
     @property
-    def overheadLimit(self) -> long: ...
+    def qualifiedSectionType(self) -> str: ...
+    @qualifiedSectionType.setter
+    def qualifiedSectionType(self, value: str):
+        self._qualifiedSectionType = value
 
 
-class ResourceAllocationOption(vmodl.DynamicData):
+class OvfConsumerUndefinedPrefix(OvfConsumerCallbackFault):
     @property
-    def sharesOption(self) -> SharesOption: ...
+    def prefix(self) -> str: ...
+    @prefix.setter
+    def prefix(self, value: str):
+        self._prefix = value
 
 
-class ResourceConfigOption(vmodl.DynamicData):
+class OvfConsumerValidationFault(VmConfigFault):
+    @property
+    def extensionKey(self) -> str: ...
+    @extensionKey.setter
+    def extensionKey(self, value: str):
+        self._extensionKey = value
     @property
-    def cpuAllocationOption(self) -> ResourceAllocationOption: ...
+    def extensionName(self) -> str: ...
+    @extensionName.setter
+    def extensionName(self, value: str):
+        self._extensionName = value
     @property
-    def memoryAllocationOption(self) -> ResourceAllocationOption: ...
+    def message(self) -> str: ...
+    @message.setter
+    def message(self, value: str):
+        self._message = value
 
 
-class ResourceConfigSpec(vmodl.DynamicData):
+class OvfCpuCompatibility(OvfImport):
     @property
-    def entity(self) -> ManagedEntity: ...
+    def registerName(self) -> str: ...
+    @registerName.setter
+    def registerName(self, value: str):
+        self._registerName = value
     @property
-    def changeVersion(self) -> str: ...
+    def level(self) -> int: ...
+    @level.setter
+    def level(self, value: int):
+        self._level = value
     @property
-    def lastModified(self) -> datetime: ...
+    def registerValue(self) -> str: ...
+    @registerValue.setter
+    def registerValue(self, value: str):
+        self._registerValue = value
     @property
-    def cpuAllocation(self) -> ResourceAllocationInfo: ...
+    def desiredRegisterValue(self) -> str: ...
+    @desiredRegisterValue.setter
+    def desiredRegisterValue(self, value: str):
+        self._desiredRegisterValue = value
+
+
+class OvfCpuCompatibilityCheckNotSupported(OvfImport): ...
+
+
+class OvfDiskMappingNotFound(OvfSystemFault):
     @property
-    def memoryAllocation(self) -> ResourceAllocationInfo: ...
+    def diskName(self) -> str: ...
+    @diskName.setter
+    def diskName(self, value: str):
+        self._diskName = value
     @property
-    def scaleDescendantsShares(self) -> str: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-    class ScaleSharesBehavior(Enum):
-        disabled = "disabled"
-        scaleCpuAndMemoryShares = "scalecpuandmemoryshares"
+class OvfDiskOrderConstraint(OvfConstraint): ...
 
 
-class SDDCBase(vmodl.DynamicData): ...
+class OvfDuplicateElement(OvfElement): ...
 
 
-class SelectionSet(vmodl.DynamicData): ...
+class OvfDuplicatedElementBoundary(OvfElement):
+    @property
+    def boundary(self) -> str: ...
+    @boundary.setter
+    def boundary(self, value: str):
+        self._boundary = value
 
 
-class ServiceInstanceContent(vmodl.DynamicData):
-    @property
-    def rootFolder(self) -> Folder: ...
-    @property
-    def propertyCollector(self) -> vmodl.query.PropertyCollector: ...
-    @property
-    def viewManager(self) -> view.ViewManager: ...
-    @property
-    def about(self) -> AboutInfo: ...
-    @property
-    def setting(self) -> option.OptionManager: ...
-    @property
-    def userDirectory(self) -> UserDirectory: ...
-    @property
-    def sessionManager(self) -> SessionManager: ...
-    @property
-    def authorizationManager(self) -> AuthorizationManager: ...
-    @property
-    def serviceManager(self) -> ServiceManager: ...
-    @property
-    def perfManager(self) -> PerformanceManager: ...
-    @property
-    def scheduledTaskManager(self) -> scheduler.ScheduledTaskManager: ...
-    @property
-    def alarmManager(self) -> alarm.AlarmManager: ...
-    @property
-    def eventManager(self) -> event.EventManager: ...
-    @property
-    def taskManager(self) -> TaskManager: ...
-    @property
-    def extensionManager(self) -> ExtensionManager: ...
+class OvfDuplicatedPropertyIdExport(OvfExport):
     @property
-    def customizationSpecManager(self) -> CustomizationSpecManager: ...
-    @property
-    def guestCustomizationManager(self) -> vm.GuestCustomizationManager: ...
-    @property
-    def customFieldsManager(self) -> CustomFieldsManager: ...
-    @property
-    def accountManager(self) -> host.LocalAccountManager: ...
-    @property
-    def diagnosticManager(self) -> DiagnosticManager: ...
-    @property
-    def licenseManager(self) -> LicenseManager: ...
-    @property
-    def searchIndex(self) -> SearchIndex: ...
-    @property
-    def fileManager(self) -> FileManager: ...
-    @property
-    def datastoreNamespaceManager(self) -> DatastoreNamespaceManager: ...
-    @property
-    def virtualDiskManager(self) -> VirtualDiskManager: ...
-    @property
-    def virtualizationManager(self) -> VirtualizationManager: ...
-    @property
-    def snmpSystem(self) -> host.SnmpSystem: ...
-    @property
-    def vmProvisioningChecker(self) -> vm.check.ProvisioningChecker: ...
-    @property
-    def vmCompatibilityChecker(self) -> vm.check.CompatibilityChecker: ...
-    @property
-    def ovfManager(self) -> OvfManager: ...
-    @property
-    def ipPoolManager(self) -> IpPoolManager: ...
-    @property
-    def dvSwitchManager(self) -> dvs.DistributedVirtualSwitchManager: ...
-    @property
-    def hostProfileManager(self) -> profile.host.ProfileManager: ...
-    @property
-    def clusterProfileManager(self) -> profile.cluster.ProfileManager: ...
-    @property
-    def complianceManager(self) -> profile.ComplianceManager: ...
-    @property
-    def localizationManager(self) -> LocalizationManager: ...
-    @property
-    def storageResourceManager(self) -> StorageResourceManager: ...
-    @property
-    def guestOperationsManager(self) -> vm.guest.GuestOperationsManager: ...
-    @property
-    def overheadMemoryManager(self) -> OverheadMemoryManager: ...
-    @property
-    def certificateManager(self) -> CertificateManager: ...
-    @property
-    def ioFilterManager(self) -> IoFilterManager: ...
-    @property
-    def vStorageObjectManager(self) -> vslm.VStorageObjectManagerBase: ...
-    @property
-    def hostSpecManager(self) -> profile.host.HostSpecificationManager: ...
-    @property
-    def cryptoManager(self) -> encryption.CryptoManager: ...
-    @property
-    def healthUpdateManager(self) -> HealthUpdateManager: ...
-    @property
-    def failoverClusterConfigurator(self) -> vcha.FailoverClusterConfigurator: ...
-    @property
-    def failoverClusterManager(self) -> vcha.FailoverClusterManager: ...
-    @property
-    def tenantManager(self) -> tenant.TenantManager: ...
-    @property
-    def siteInfoManager(self) -> SiteInfoManager: ...
-    @property
-    def storageQueryManager(self) -> StorageQueryManager: ...
+    def fqid(self) -> str: ...
+    @fqid.setter
+    def fqid(self, value: str):
+        self._fqid = value
 
 
-class ServiceLocator(vmodl.DynamicData):
-    @property
-    def instanceUuid(self) -> str: ...
-    @property
-    def url(self) -> str: ...
+class OvfDuplicatedPropertyIdImport(OvfExport): ...
+
+
+class OvfElement(OvfInvalidPackage):
     @property
-    def credential(self) -> ServiceLocator.Credential: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class OvfElementInvalidValue(OvfElement):
     @property
-    def sslThumbprint(self) -> str: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
 
 
-    class Credential(vmodl.DynamicData): ...
+class OvfExport(OvfFault): ...
 
 
-    class NamePassword(ServiceLocator.Credential):
-        @property
-        def username(self) -> str: ...
-        @property
-        def password(self) -> str: ...
+class OvfExportFailed(OvfExport): ...
 
 
-    class SAMLCredential(ServiceLocator.Credential):
-        @property
-        def token(self) -> str: ...
+class OvfFault(VimFault): ...
+
+
+class OvfHardwareCheck(OvfImport): ...
 
 
-class SharesInfo(vmodl.DynamicData):
+class OvfHardwareExport(OvfExport):
     @property
-    def shares(self) -> int: ...
+    def device(self) -> vim.vm.device.VirtualDevice: ...
+    @device.setter
+    def device(self, value: vim.vm.device.VirtualDevice):
+        self._device = value
     @property
-    def level(self) -> SharesInfo.Level: ...
+    def vmPath(self) -> str: ...
+    @vmPath.setter
+    def vmPath(self, value: str):
+        self._vmPath = value
 
 
-    class Level(Enum):
-        low = "low"
-        normal = "normal"
-        high = "high"
-        custom = "custom"
+class OvfHostResourceConstraint(OvfConstraint):
+    @property
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
 
 
-class SharesOption(vmodl.DynamicData):
+class OvfHostValueNotParsed(OvfSystemFault):
     @property
-    def sharesOption(self) -> option.IntOption: ...
+    def property(self) -> str: ...
+    @property.setter
+    def property(self, value: str):
+        self._property = value
     @property
-    def defaultLevel(self) -> SharesInfo.Level: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
 
 
-class SingleIp(IpAddress):
-    @property
-    def address(self) -> str: ...
+class OvfImport(OvfFault): ...
 
 
-class SingleMac(MacAddress):
-    @property
-    def address(self) -> str: ...
+class OvfImportFailed(OvfImport): ...
 
 
-class SiteInfo(vmodl.DynamicData): ...
+class OvfInternalError(OvfSystemFault): ...
 
 
-class StringExpression(NegatableExpression):
+class OvfInvalidPackage(OvfFault):
     @property
-    def value(self) -> str: ...
+    def lineNumber(self) -> int: ...
+    @lineNumber.setter
+    def lineNumber(self, value: int):
+        self._lineNumber = value
 
 
-class StringPolicy(InheritablePolicy):
+class OvfInvalidValue(OvfAttribute):
     @property
     def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
 
 
-class Tag(vmodl.DynamicData):
+class OvfInvalidValueConfiguration(OvfInvalidValue): ...
+
+
+class OvfInvalidValueEmpty(OvfInvalidValue): ...
+
+
+class OvfInvalidValueFormatMalformed(OvfInvalidValue): ...
+
+
+class OvfInvalidValueReference(OvfInvalidValue): ...
+
+
+class OvfInvalidVmName(OvfUnsupportedPackage):
     @property
-    def key(self) -> str: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-class TaskDescription(vmodl.DynamicData):
+class OvfMappedOsId(OvfImport):
     @property
-    def methodInfo(self) -> List[ElementDescription]: ...
+    def ovfId(self) -> int: ...
+    @ovfId.setter
+    def ovfId(self, value: int):
+        self._ovfId = value
     @property
-    def state(self) -> List[ElementDescription]: ...
+    def ovfDescription(self) -> str: ...
+    @ovfDescription.setter
+    def ovfDescription(self, value: str):
+        self._ovfDescription = value
     @property
-    def reason(self) -> List[TypeDescription]: ...
+    def targetDescription(self) -> str: ...
+    @targetDescription.setter
+    def targetDescription(self, value: str):
+        self._targetDescription = value
+
+
+class OvfMissingAttribute(OvfAttribute): ...
+
+
+class OvfMissingElement(OvfElement): ...
 
 
-class TaskFilterSpec(vmodl.DynamicData):
+class OvfMissingElementNormalBoundary(OvfMissingElement):
     @property
-    def entity(self) -> TaskFilterSpec.ByEntity: ...
+    def boundary(self) -> str: ...
+    @boundary.setter
+    def boundary(self, value: str):
+        self._boundary = value
+
+
+class OvfMissingHardware(OvfImport):
     @property
-    def time(self) -> TaskFilterSpec.ByTime: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def userName(self) -> TaskFilterSpec.ByUsername: ...
+    def resourceType(self) -> int: ...
+    @resourceType.setter
+    def resourceType(self, value: int):
+        self._resourceType = value
+
+
+class OvfNetworkMappingNotSupported(OvfImport): ...
+
+
+class OvfNoHostNic(OvfUnsupportedPackage): ...
+
+
+class OvfNoSpaceOnController(OvfUnsupportedElement):
     @property
-    def activationId(self) -> List[str]: ...
+    def parent(self) -> str: ...
+    @parent.setter
+    def parent(self, value: str):
+        self._parent = value
+
+
+class OvfNoSupportedHardwareFamily(OvfUnsupportedPackage):
     @property
-    def state(self) -> List[TaskInfo.State]: ...
+    def version(self) -> str: ...
+    @version.setter
+    def version(self, value: str):
+        self._version = value
+
+
+class OvfProperty(OvfInvalidPackage):
     @property
-    def alarm(self) -> alarm.Alarm: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def scheduledTask(self) -> scheduler.ScheduledTask: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
+
+
+class OvfPropertyExport(OvfExport):
     @property
-    def eventChainId(self) -> List[int]: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def tag(self) -> List[str]: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
+
+
+class OvfPropertyNetwork(OvfProperty): ...
+
+
+class OvfPropertyNetworkExport(OvfExport):
     @property
-    def parentTaskKey(self) -> List[str]: ...
+    def network(self) -> str: ...
+    @network.setter
+    def network(self, value: str):
+        self._network = value
+
+
+class OvfPropertyQualifier(OvfProperty):
     @property
-    def rootTaskKey(self) -> List[str]: ...
+    def qualifier(self) -> str: ...
+    @qualifier.setter
+    def qualifier(self, value: str):
+        self._qualifier = value
 
 
-    class ByEntity(vmodl.DynamicData):
-        @property
-        def entity(self) -> ManagedEntity: ...
-        @property
-        def recursion(self) -> TaskFilterSpec.RecursionOption: ...
+class OvfPropertyQualifierDuplicate(OvfProperty):
+    @property
+    def qualifier(self) -> str: ...
+    @qualifier.setter
+    def qualifier(self, value: str):
+        self._qualifier = value
 
 
-    class ByTime(vmodl.DynamicData):
-        @property
-        def timeType(self) -> TaskFilterSpec.TimeOption: ...
-        @property
-        def beginTime(self) -> datetime: ...
-        @property
-        def endTime(self) -> datetime: ...
+class OvfPropertyQualifierIgnored(OvfProperty):
+    @property
+    def qualifier(self) -> str: ...
+    @qualifier.setter
+    def qualifier(self, value: str):
+        self._qualifier = value
 
 
-    class ByUsername(vmodl.DynamicData):
-        @property
-        def systemUser(self) -> bool: ...
-        @property
-        def userList(self) -> List[str]: ...
+class OvfPropertyType(OvfProperty): ...
 
 
-    class RecursionOption(Enum):
-        self = "self"
-        children = "children"
-        all = "all"
+class OvfPropertyValue(OvfProperty): ...
 
 
-    class TimeOption(Enum):
-        queuedTime = "queuedtime"
-        startedTime = "startedtime"
-        completedTime = "completedtime"
+class OvfSystemFault(OvfFault): ...
 
 
-class TaskInfo(vmodl.DynamicData):
-    @property
-    def key(self) -> str: ...
-    @property
-    def task(self) -> Task: ...
-    @property
-    def description(self) -> vmodl.LocalizableMessage: ...
-    @property
-    def name(self) -> ManagedMethod: ...
-    @property
-    def descriptionId(self) -> str: ...
-    @property
-    def entity(self) -> ManagedEntity: ...
+class OvfToXmlUnsupportedElement(OvfSystemFault):
     @property
-    def entityName(self) -> str: ...
-    @property
-    def locked(self) -> List[ManagedEntity]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class OvfUnableToExportDisk(OvfHardwareExport):
     @property
-    def state(self) -> TaskInfo.State: ...
+    def diskName(self) -> str: ...
+    @diskName.setter
+    def diskName(self, value: str):
+        self._diskName = value
+
+
+class OvfUnexpectedElement(OvfElement): ...
+
+
+class OvfUnknownDevice(OvfSystemFault):
     @property
-    def cancelled(self) -> bool: ...
+    def device(self) -> vim.vm.device.VirtualDevice: ...
+    @device.setter
+    def device(self, value: vim.vm.device.VirtualDevice):
+        self._device = value
     @property
-    def cancelable(self) -> bool: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+class OvfUnknownDeviceBacking(OvfHardwareExport):
     @property
-    def error(self) -> vmodl.MethodFault: ...
+    def backing(self) -> vim.vm.device.VirtualDevice.BackingInfo: ...
+    @backing.setter
+    def backing(self, value: vim.vm.device.VirtualDevice.BackingInfo):
+        self._backing = value
+
+
+class OvfUnknownEntity(OvfSystemFault):
     @property
-    def result(self) -> object: ...
+    def lineNumber(self) -> int: ...
+    @lineNumber.setter
+    def lineNumber(self, value: int):
+        self._lineNumber = value
+
+
+class OvfUnsupportedAttribute(OvfUnsupportedPackage):
     @property
-    def progress(self) -> int: ...
+    def elementName(self) -> str: ...
+    @elementName.setter
+    def elementName(self, value: str):
+        self._elementName = value
     @property
-    def progressDetails(self) -> List[vmodl.KeyAnyValue]: ...
+    def attributeName(self) -> str: ...
+    @attributeName.setter
+    def attributeName(self, value: str):
+        self._attributeName = value
+
+
+class OvfUnsupportedAttributeValue(OvfUnsupportedAttribute):
     @property
-    def reason(self) -> TaskReason: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
+
+
+class OvfUnsupportedDeviceBackingInfo(OvfSystemFault):
     @property
-    def queueTime(self) -> datetime: ...
+    def elementName(self) -> str: ...
+    @elementName.setter
+    def elementName(self, value: str):
+        self._elementName = value
     @property
-    def startTime(self) -> datetime: ...
+    def instanceId(self) -> str: ...
+    @instanceId.setter
+    def instanceId(self, value: str):
+        self._instanceId = value
+    @property
+    def deviceName(self) -> str: ...
+    @deviceName.setter
+    def deviceName(self, value: str):
+        self._deviceName = value
+    @property
+    def backingName(self) -> str: ...
+    @backingName.setter
+    def backingName(self, value: str):
+        self._backingName = value
+
+
+class OvfUnsupportedDeviceBackingOption(OvfSystemFault):
+    @property
+    def elementName(self) -> str: ...
+    @elementName.setter
+    def elementName(self, value: str):
+        self._elementName = value
     @property
-    def completeTime(self) -> datetime: ...
+    def instanceId(self) -> str: ...
+    @instanceId.setter
+    def instanceId(self, value: str):
+        self._instanceId = value
     @property
-    def eventChainId(self) -> int: ...
+    def deviceName(self) -> str: ...
+    @deviceName.setter
+    def deviceName(self, value: str):
+        self._deviceName = value
     @property
-    def changeTag(self) -> str: ...
+    def backingName(self) -> str: ...
+    @backingName.setter
+    def backingName(self, value: str):
+        self._backingName = value
+
+
+class OvfUnsupportedDeviceExport(OvfHardwareExport): ...
+
+
+class OvfUnsupportedDiskProvisioning(OvfImport):
     @property
-    def parentTaskKey(self) -> str: ...
+    def diskProvisioning(self) -> str: ...
+    @diskProvisioning.setter
+    def diskProvisioning(self, value: str):
+        self._diskProvisioning = value
     @property
-    def rootTaskKey(self) -> str: ...
+    def supportedDiskProvisioning(self) -> str: ...
+    @supportedDiskProvisioning.setter
+    def supportedDiskProvisioning(self, value: str):
+        self._supportedDiskProvisioning = value
+
+
+class OvfUnsupportedElement(OvfUnsupportedPackage):
     @property
-    def activationId(self) -> str: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
 
 
-class TaskReason(vmodl.DynamicData): ...
+class OvfUnsupportedElementValue(OvfUnsupportedElement):
+    @property
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
 
 
-class TaskReasonAlarm(TaskReason):
+class OvfUnsupportedPackage(OvfFault):
     @property
-    def alarmName(self) -> str: ...
+    def lineNumber(self) -> int: ...
+    @lineNumber.setter
+    def lineNumber(self, value: int):
+        self._lineNumber = value
+
+
+class OvfUnsupportedSection(OvfUnsupportedElement):
     @property
-    def alarm(self) -> alarm.Alarm: ...
+    def info(self) -> str: ...
+    @info.setter
+    def info(self, value: str):
+        self._info = value
+
+
+class OvfUnsupportedSubType(OvfUnsupportedPackage):
     @property
-    def entityName(self) -> str: ...
+    def elementName(self) -> str: ...
+    @elementName.setter
+    def elementName(self, value: str):
+        self._elementName = value
     @property
-    def entity(self) -> ManagedEntity: ...
+    def instanceId(self) -> str: ...
+    @instanceId.setter
+    def instanceId(self, value: str):
+        self._instanceId = value
+    @property
+    def deviceType(self) -> int: ...
+    @deviceType.setter
+    def deviceType(self, value: int):
+        self._deviceType = value
+    @property
+    def deviceSubType(self) -> str: ...
+    @deviceSubType.setter
+    def deviceSubType(self, value: str):
+        self._deviceSubType = value
 
 
-class TaskReasonSchedule(TaskReason):
+class OvfUnsupportedType(OvfUnsupportedPackage):
     @property
     def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+    @property
+    def instanceId(self) -> str: ...
+    @instanceId.setter
+    def instanceId(self, value: str):
+        self._instanceId = value
     @property
-    def scheduledTask(self) -> scheduler.ScheduledTask: ...
+    def deviceType(self) -> int: ...
+    @deviceType.setter
+    def deviceType(self, value: int):
+        self._deviceType = value
 
 
-class TaskReasonSystem(TaskReason): ...
+class OvfWrongElement(OvfElement): ...
 
 
-class TaskReasonUser(TaskReason):
+class OvfWrongNamespace(OvfInvalidPackage):
     @property
-    def userName(self) -> str: ...
+    def namespaceName(self) -> str: ...
+    @namespaceName.setter
+    def namespaceName(self, value: str):
+        self._namespaceName = value
 
 
-class TypeDescription(Description):
+class OvfXmlFormat(OvfInvalidPackage):
     @property
-    def key(self) -> type: ...
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
 
 
-class UpdateVirtualMachineFilesResult(vmodl.DynamicData):
-    @property
-    def failedVmFile(self) -> List[UpdateVirtualMachineFilesResult.FailedVmFileInfo]: ...
+class PasswordExpired(InvalidLogin): ...
 
 
-    class FailedVmFileInfo(vmodl.DynamicData):
-        @property
-        def vmFile(self) -> str: ...
-        @property
-        def fault(self) -> vmodl.MethodFault: ...
+class PatchAlreadyInstalled(PatchNotApplicable): ...
 
 
-class UserSearchResult(vmodl.DynamicData):
-    @property
-    def principal(self) -> str: ...
+class PatchBinariesNotFound(VimFault):
     @property
-    def fullName(self) -> str: ...
+    def patchID(self) -> str: ...
+    @patchID.setter
+    def patchID(self, value: str):
+        self._patchID = value
     @property
-    def group(self) -> bool: ...
+    def binary(self) -> List[str]: ...
+    @binary.setter
+    def binary(self, value: List[str]):
+        self._binary = value
 
 
-class UserSession(vmodl.DynamicData):
-    @property
-    def key(self) -> str: ...
-    @property
-    def userName(self) -> str: ...
-    @property
-    def fullName(self) -> str: ...
-    @property
-    def loginTime(self) -> datetime: ...
+class PatchInstallFailed(PlatformConfigFault):
     @property
-    def lastActiveTime(self) -> datetime: ...
-    @property
-    def locale(self) -> str: ...
-    @property
-    def messageLocale(self) -> str: ...
-    @property
-    def extensionSession(self) -> bool: ...
-    @property
-    def ipAddress(self) -> str: ...
-    @property
-    def userAgent(self) -> str: ...
-    @property
-    def callCount(self) -> long: ...
+    def rolledBack(self) -> bool: ...
+    @rolledBack.setter
+    def rolledBack(self, value: bool):
+        self._rolledBack = value
 
 
-class VVolVmConfigFileUpdateResult(vmodl.DynamicData):
-    @property
-    def succeededVmConfigFile(self) -> List[KeyValue]: ...
-    @property
-    def failedVmConfigFile(self) -> List[VVolVmConfigFileUpdateResult.FailedVmConfigFileInfo]: ...
+class PatchIntegrityError(PlatformConfigFault): ...
 
 
-    class FailedVmConfigFileInfo(vmodl.DynamicData):
-        @property
-        def targetConfigVVolId(self) -> str: ...
-        @property
-        def dsPath(self) -> str: ...
-        @property
-        def fault(self) -> vmodl.MethodFault: ...
+class PatchMetadataCorrupted(PatchMetadataInvalid): ...
 
 
-class VasaStorageArray(vmodl.DynamicData):
+class PatchMetadataInvalid(VimFault):
     @property
-    def name(self) -> str: ...
+    def patchID(self) -> str: ...
+    @patchID.setter
+    def patchID(self, value: str):
+        self._patchID = value
     @property
-    def uuid(self) -> str: ...
-    @property
-    def vendorId(self) -> str: ...
+    def metaData(self) -> List[str]: ...
+    @metaData.setter
+    def metaData(self, value: List[str]):
+        self._metaData = value
+
+
+class PatchMetadataNotFound(PatchMetadataInvalid): ...
+
+
+class PatchMissingDependencies(PatchNotApplicable):
     @property
-    def modelId(self) -> str: ...
+    def prerequisitePatch(self) -> List[str]: ...
+    @prerequisitePatch.setter
+    def prerequisitePatch(self, value: List[str]):
+        self._prerequisitePatch = value
     @property
-    def discoverySvcInfo(self) -> List[VasaStorageArray.DiscoverySvcInfo]: ...
+    def prerequisiteLib(self) -> List[str]: ...
+    @prerequisiteLib.setter
+    def prerequisiteLib(self, value: List[str]):
+        self._prerequisiteLib = value
 
 
-    class DiscoveryFcTransport(vmodl.DynamicData):
-        @property
-        def nodeWwn(self) -> str: ...
-        @property
-        def portWwn(self) -> str: ...
+class PatchNotApplicable(VimFault):
+    @property
+    def patchID(self) -> str: ...
+    @patchID.setter
+    def patchID(self, value: str):
+        self._patchID = value
 
 
-    class DiscoveryIpTransport(vmodl.DynamicData):
-        @property
-        def ipAddress(self) -> str: ...
-        @property
-        def portNumber(self) -> str: ...
+class PatchSuperseded(PatchNotApplicable):
+    @property
+    def supersede(self) -> List[str]: ...
+    @supersede.setter
+    def supersede(self, value: List[str]):
+        self._supersede = value
 
 
-    class DiscoverySvcInfo(vmodl.DynamicData):
-        @property
-        def portType(self) -> str: ...
-        @property
-        def svcNqn(self) -> str: ...
-        @property
-        def ipInfo(self) -> VasaStorageArray.DiscoveryIpTransport: ...
-        @property
-        def fcInfo(self) -> VasaStorageArray.DiscoveryFcTransport: ...
+class PhysCompatRDMNotSupported(RDMNotSupported): ...
 
 
-class VasaProviderContainerSpec(vmodl.DynamicData):
-    @property
-    def vasaProviderInfo(self) -> List[VimVasaProviderInfo]: ...
+class PlatformConfigFault(HostConfigFault):
     @property
-    def scId(self) -> str: ...
-    @property
-    def deleted(self) -> bool: ...
+    def text(self) -> str: ...
+    @text.setter
+    def text(self, value: str):
+        self._text = value
 
 
-class VimVasaProvider(vmodl.DynamicData):
+class PowerOnFtSecondaryFailed(VmFaultToleranceIssue):
     @property
-    def uid(self) -> str: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def url(self) -> str: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def name(self) -> str: ...
+    def hostSelectionBy(self) -> FtIssuesOnHost.HostSelectionType | Literal['user', 'vc', 'drs']: ...
+    @hostSelectionBy.setter
+    def hostSelectionBy(self, value: FtIssuesOnHost.HostSelectionType | Literal['user', 'vc', 'drs']):
+        self._hostSelectionBy = value
+    @property
+    def hostErrors(self) -> List[vmodl.MethodFault]: ...
+    @hostErrors.setter
+    def hostErrors(self, value: List[vmodl.MethodFault]):
+        self._hostErrors = value
+    @property
+    def rootCause(self) -> vmodl.MethodFault: ...
+    @rootCause.setter
+    def rootCause(self, value: vmodl.MethodFault):
+        self._rootCause = value
+
+
+class PowerOnFtSecondaryTimedout(Timedout):
     @property
-    def selfSignedCertificate(self) -> str: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def vhostConfig(self) -> VimVasaProvider.VirtualHostConfig: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def versionId(self) -> int: ...
+    def timeout(self) -> int: ...
+    @timeout.setter
+    def timeout(self, value: int):
+        self._timeout = value
 
 
-    class StatePerArray(vmodl.DynamicData):
-        @property
-        def priority(self) -> int: ...
-        @property
-        def arrayId(self) -> str: ...
-        @property
-        def active(self) -> bool: ...
+class ProfileUpdateFailed(VimFault):
+    @property
+    def failure(self) -> List[ProfileUpdateFailed.UpdateFailure]: ...
+    @failure.setter
+    def failure(self, value: List[ProfileUpdateFailed.UpdateFailure]):
+        self._failure = value
+    @property
+    def warnings(self) -> List[ProfileUpdateFailed.UpdateFailure]: ...
+    @warnings.setter
+    def warnings(self, value: List[ProfileUpdateFailed.UpdateFailure]):
+        self._warnings = value
 
 
-    class VirtualHostConfig(vmodl.DynamicData):
+    class UpdateFailure(vmodl.DynamicData):
         @property
-        def vhostName(self) -> str: ...
+        def profilePath(self) -> vim.profile.ProfilePropertyPath: ...
+        @profilePath.setter
+        def profilePath(self, value: vim.profile.ProfilePropertyPath):
+            self._profilePath = value
         @property
-        def serviceHost(self) -> str: ...
-        @property
-        def servicePort(self) -> int: ...
+        def errMsg(self) -> vmodl.LocalizableMessage: ...
+        @errMsg.setter
+        def errMsg(self, value: vmodl.LocalizableMessage):
+            self._errMsg = value
 
 
-class VimVasaProviderInfo(vmodl.DynamicData):
+class QuarantineModeFault(VmConfigFault):
     @property
-    def provider(self) -> VimVasaProvider: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def arrayState(self) -> List[VimVasaProvider.StatePerArray]: ...
+    def faultType(self) -> str: ...
+    @faultType.setter
+    def faultType(self, value: str):
+        self._faultType = value
 
 
-class ApplyRecommendationResult(vmodl.DynamicData):
-    @property
-    def vm(self) -> VirtualMachine: ...
+    class FaultType(Enum):
+        NoCompatibleNonQuarantinedHost = "NoCompatibleNonQuarantinedHost"
+        CorrectionDisallowed = "CorrectionDisallowed"
+        CorrectionImpact = "CorrectionImpact"
 
 
-class AutomationConfig(vmodl.DynamicData):
+class QuestionPending(InvalidState):
     @property
-    def spaceLoadBalanceAutomationMode(self) -> str: ...
+    def text(self) -> str: ...
+    @text.setter
+    def text(self, value: str):
+        self._text = value
+
+
+class QuiesceDatastoreIOForHAFailed(ResourceInUse):
     @property
-    def ioLoadBalanceAutomationMode(self) -> str: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def ruleEnforcementAutomationMode(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def policyEnforcementAutomationMode(self) -> str: ...
+    def ds(self) -> vim.Datastore: ...
+    @ds.setter
+    def ds(self, value: vim.Datastore):
+        self._ds = value
     @property
-    def vmEvacuationAutomationMode(self) -> str: ...
+    def dsName(self) -> str: ...
+    @dsName.setter
+    def dsName(self, value: str):
+        self._dsName = value
 
 
-class ConfigInfo(vmodl.DynamicData):
+class RDMConversionNotSupported(MigrationFault):
     @property
-    def podConfig(self) -> storageDrs.PodConfigInfo: ...
-    @property
-    def vmConfig(self) -> List[storageDrs.VmConfigInfo]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
 
-class ConfigSpec(vmodl.DynamicData):
-    @property
-    def podConfigSpec(self) -> storageDrs.PodConfigSpec: ...
+class RDMNotPreserved(MigrationFault):
     @property
-    def vmConfigSpec(self) -> List[storageDrs.VmConfigSpec]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
 
 
-class HbrDiskMigrationAction(cluster.Action):
-    @property
-    def collectionId(self) -> str: ...
-    @property
-    def collectionName(self) -> str: ...
-    @property
-    def diskIds(self) -> List[str]: ...
-    @property
-    def source(self) -> Datastore: ...
-    @property
-    def destination(self) -> Datastore: ...
-    @property
-    def sizeTransferred(self) -> long: ...
-    @property
-    def spaceUtilSrcBefore(self) -> float: ...
-    @property
-    def spaceUtilDstBefore(self) -> float: ...
-    @property
-    def spaceUtilSrcAfter(self) -> float: ...
-    @property
-    def spaceUtilDstAfter(self) -> float: ...
-    @property
-    def ioLatencySrcBefore(self) -> float: ...
-    @property
-    def ioLatencyDstBefore(self) -> float: ...
+class RDMNotSupported(DeviceNotSupported): ...
 
 
-class IoLoadBalanceConfig(vmodl.DynamicData):
+class RDMNotSupportedOnDatastore(VmConfigFault):
     @property
-    def reservablePercentThreshold(self) -> int: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def reservableIopsThreshold(self) -> int: ...
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
     @property
-    def reservableThresholdMode(self) -> str: ...
-    @property
-    def ioLatencyThreshold(self) -> int: ...
-    @property
-    def ioLoadImbalanceThreshold(self) -> int: ...
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
 
 
-class OptionSpec(option.ArrayUpdateSpec):
-    @property
-    def option(self) -> option.OptionValue: ...
+class RDMPointsToInaccessibleDisk(CannotAccessVmDisk): ...
 
 
-class PlacementAffinityRule(vmodl.DynamicData):
-    @property
-    def ruleType(self) -> str: ...
+class RawDiskNotSupported(DeviceNotSupported): ...
+
+
+class ReadHostResourcePoolTreeFailed(HostConnectFault): ...
+
+
+class ReadOnlyDisksWithLegacyDestination(MigrationFault):
     @property
-    def ruleScope(self) -> str: ...
+    def roDiskCount(self) -> int: ...
+    @roDiskCount.setter
+    def roDiskCount(self, value: int):
+        self._roDiskCount = value
     @property
-    def vms(self) -> List[VirtualMachine]: ...
+    def timeoutDanger(self) -> bool: ...
+    @timeoutDanger.setter
+    def timeoutDanger(self, value: bool):
+        self._timeoutDanger = value
+
+
+class RebootRequired(VimFault):
     @property
-    def keys(self) -> List[str]: ...
+    def patch(self) -> str: ...
+    @patch.setter
+    def patch(self, value: str):
+        self._patch = value
 
 
-    class RuleScope(Enum):
-        cluster = "cluster"
-        host = "host"
-        storagePod = "storagepod"
-        datastore = "datastore"
+class RecordReplayDisabled(VimFault): ...
+
+
+class RemoteDeviceNotSupported(DeviceNotSupported): ...
+
 
+class RemoveFailed(VimFault): ...
 
-    class RuleType(Enum):
-        affinity = "affinity"
-        antiAffinity = "antiaffinity"
-        softAffinity = "softaffinity"
-        softAntiAffinity = "softantiaffinity"
 
+class ReplicationConfigFault(ReplicationFault): ...
 
-class PlacementRankResult(vmodl.DynamicData):
+
+class ReplicationDiskConfigFault(ReplicationConfigFault):
     @property
-    def key(self) -> str: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def candidate(self) -> ClusterComputeResource: ...
+    def vmRef(self) -> vim.VirtualMachine: ...
+    @vmRef.setter
+    def vmRef(self, value: vim.VirtualMachine):
+        self._vmRef = value
     @property
-    def reservedSpaceMB(self) -> long: ...
+    def key(self) -> int: ...
+    @key.setter
+    def key(self, value: int):
+        self._key = value
+
+
+    class ReasonForFault(Enum):
+        diskNotFound = "diskNotFound"
+        diskTypeNotSupported = "diskTypeNotSupported"
+        invalidDiskKey = "invalidDiskKey"
+        invalidDiskReplicationId = "invalidDiskReplicationId"
+        duplicateDiskReplicationId = "duplicateDiskReplicationId"
+        invalidPersistentFilePath = "invalidPersistentFilePath"
+        reconfigureDiskReplicationIdNotAllowed = "reconfigureDiskReplicationIdNotAllowed"
+
+
+class ReplicationFault(VimFault): ...
+
+
+class ReplicationIncompatibleWithFT(ReplicationFault): ...
+
+
+class ReplicationInvalidOptions(ReplicationFault):
     @property
-    def usedSpaceMB(self) -> long: ...
+    def options(self) -> str: ...
+    @options.setter
+    def options(self, value: str):
+        self._options = value
     @property
-    def totalSpaceMB(self) -> long: ...
+    def entity(self) -> vim.ManagedEntity: ...
+    @entity.setter
+    def entity(self, value: vim.ManagedEntity):
+        self._entity = value
+
+
+class ReplicationNotSupportedOnHost(ReplicationFault): ...
+
+
+class ReplicationVmConfigFault(ReplicationConfigFault):
     @property
-    def utilization(self) -> double: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def faults(self) -> List[vmodl.MethodFault]: ...
+    def vmRef(self) -> vim.VirtualMachine: ...
+    @vmRef.setter
+    def vmRef(self, value: vim.VirtualMachine):
+        self._vmRef = value
 
 
-class PlacementRankSpec(vmodl.DynamicData):
+class ReplicationVmFault(ReplicationFault):
     @property
-    def specs(self) -> List[cluster.PlacementSpec]: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def clusters(self) -> List[ClusterComputeResource]: ...
+    def state(self) -> str: ...
+    @state.setter
+    def state(self, value: str):
+        self._state = value
     @property
-    def rules(self) -> List[storageDrs.PlacementAffinityRule]: ...
+    def instanceId(self) -> str: ...
+    @instanceId.setter
+    def instanceId(self, value: str):
+        self._instanceId = value
     @property
-    def placementRankByVm(self) -> List[storageDrs.PlacementRankVmSpec]: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
 
 
-class PlacementRankVmSpec(vmodl.DynamicData):
+class ReplicationVmInProgressFault(ReplicationVmFault):
     @property
-    def vmPlacementSpec(self) -> cluster.PlacementSpec: ...
+    def requestedActivity(self) -> str: ...
+    @requestedActivity.setter
+    def requestedActivity(self, value: str):
+        self._requestedActivity = value
     @property
-    def vmClusters(self) -> List[ClusterComputeResource]: ...
+    def inProgressActivity(self) -> str: ...
+    @inProgressActivity.setter
+    def inProgressActivity(self, value: str):
+        self._inProgressActivity = value
 
 
-class PodConfigInfo(vmodl.DynamicData):
-    @property
-    def enabled(self) -> bool: ...
-    @property
-    def ioLoadBalanceEnabled(self) -> bool: ...
-    @property
-    def defaultVmBehavior(self) -> str: ...
-    @property
-    def loadBalanceInterval(self) -> int: ...
+    class Activity(Enum):
+        fullSync = "fullSync"
+        delta = "delta"
+
+
+class ResourceInUse(VimFault):
     @property
-    def defaultIntraVmAffinity(self) -> bool: ...
+    def type(self) -> type: ...
+    @type.setter
+    def type(self, value: type):
+        self._type = value
     @property
-    def spaceLoadBalanceConfig(self) -> storageDrs.SpaceLoadBalanceConfig: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+
+
+class ResourceNotAvailable(VimFault):
     @property
-    def ioLoadBalanceConfig(self) -> storageDrs.IoLoadBalanceConfig: ...
+    def containerType(self) -> type: ...
+    @containerType.setter
+    def containerType(self, value: type):
+        self._containerType = value
     @property
-    def automationOverrides(self) -> storageDrs.AutomationConfig: ...
+    def containerName(self) -> str: ...
+    @containerName.setter
+    def containerName(self, value: str):
+        self._containerName = value
     @property
-    def rule(self) -> List[cluster.RuleInfo]: ...
+    def type(self) -> type: ...
+    @type.setter
+    def type(self, value: type):
+        self._type = value
+
+
+class RestrictedByAdministrator(vmodl.RuntimeFault):
     @property
-    def option(self) -> List[option.OptionValue]: ...
+    def details(self) -> str: ...
+    @details.setter
+    def details(self, value: str):
+        self._details = value
 
 
-    class Behavior(Enum):
-        manual = "manual"
-        automated = "automated"
+class RestrictedVersion(SecurityError): ...
 
 
-class PodConfigSpec(vmodl.DynamicData):
-    @property
-    def enabled(self) -> bool: ...
+class RollbackFailure(DvsFault):
     @property
-    def ioLoadBalanceEnabled(self) -> bool: ...
+    def entityName(self) -> str: ...
+    @entityName.setter
+    def entityName(self, value: str):
+        self._entityName = value
     @property
-    def defaultVmBehavior(self) -> str: ...
+    def entityType(self) -> str: ...
+    @entityType.setter
+    def entityType(self, value: str):
+        self._entityType = value
+
+
+class RuleViolation(VmConfigFault):
     @property
-    def loadBalanceInterval(self) -> int: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def defaultIntraVmAffinity(self) -> bool: ...
+    def rule(self) -> vim.cluster.RuleInfo: ...
+    @rule.setter
+    def rule(self, value: vim.cluster.RuleInfo):
+        self._rule = value
+
+
+class SSLDisabledFault(HostConnectFault): ...
+
+
+class SSLVerifyFault(HostConnectFault):
     @property
-    def spaceLoadBalanceConfig(self) -> storageDrs.SpaceLoadBalanceConfig: ...
+    def selfSigned(self) -> bool: ...
+    @selfSigned.setter
+    def selfSigned(self, value: bool):
+        self._selfSigned = value
     @property
-    def ioLoadBalanceConfig(self) -> storageDrs.IoLoadBalanceConfig: ...
+    def thumbprint(self) -> str: ...
+    @thumbprint.setter
+    def thumbprint(self, value: str):
+        self._thumbprint = value
+
+
+class SSPIChallenge(VimFault):
     @property
-    def automationOverrides(self) -> storageDrs.AutomationConfig: ...
+    def base64Token(self) -> str: ...
+    @base64Token.setter
+    def base64Token(self, value: str):
+        self._base64Token = value
+
+
+class SecondaryVmAlreadyDisabled(VmFaultToleranceIssue):
     @property
-    def rule(self) -> List[cluster.RuleSpec]: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
+
+
+class SecondaryVmAlreadyEnabled(VmFaultToleranceIssue):
     @property
-    def option(self) -> List[storageDrs.OptionSpec]: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
 
 
-class PodSelectionSpec(vmodl.DynamicData):
+class SecondaryVmAlreadyRegistered(VmFaultToleranceIssue):
     @property
-    def initialVmConfig(self) -> List[storageDrs.PodSelectionSpec.VmPodConfig]: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
+
+
+class SecondaryVmNotRegistered(VmFaultToleranceIssue):
     @property
-    def storagePod(self) -> StoragePod: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
 
 
-class DiskLocator(vmodl.DynamicData):
+class SharedBusControllerNotSupported(DeviceNotSupported): ...
+
+
+class ShrinkDiskFault(VimFault):
     @property
     def diskId(self) -> int: ...
-    @property
-    def diskMoveType(self) -> str: ...
-    @property
-    def diskBackingInfo(self) -> vm.device.VirtualDevice.BackingInfo: ...
-    @property
-    def profile(self) -> List[vm.ProfileSpec]: ...
+    @diskId.setter
+    def diskId(self, value: int):
+        self._diskId = value
 
 
-class VmPodConfig(vmodl.DynamicData):
-    @property
-    def storagePod(self) -> StoragePod: ...
-    @property
-    def disk(self) -> List[storageDrs.PodSelectionSpec.DiskLocator]: ...
-    @property
-    def vmConfig(self) -> storageDrs.VmConfigInfo: ...
-    @property
-    def interVmRule(self) -> List[cluster.RuleInfo]: ...
+class SnapshotCloneNotSupported(SnapshotCopyNotSupported): ...
 
 
-class SpaceLoadBalanceConfig(vmodl.DynamicData):
-    @property
-    def spaceThresholdMode(self) -> str: ...
-    @property
-    def spaceUtilizationThreshold(self) -> int: ...
-    @property
-    def freeSpaceThresholdGB(self) -> int: ...
-    @property
-    def minSpaceUtilizationDifference(self) -> int: ...
+class SnapshotCopyNotSupported(MigrationFault): ...
 
 
-    class SpaceThresholdMode(Enum):
-        utilization = "utilization"
-        freeSpace = "freespace"
+class SnapshotDisabled(SnapshotFault): ...
 
 
-class StorageMigrationAction(cluster.Action):
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def relocateSpec(self) -> vm.RelocateSpec: ...
-    @property
-    def source(self) -> Datastore: ...
-    @property
-    def destination(self) -> Datastore: ...
-    @property
-    def sizeTransferred(self) -> long: ...
-    @property
-    def spaceUtilSrcBefore(self) -> float: ...
-    @property
-    def spaceUtilDstBefore(self) -> float: ...
-    @property
-    def spaceUtilSrcAfter(self) -> float: ...
-    @property
-    def spaceUtilDstAfter(self) -> float: ...
-    @property
-    def ioLatencySrcBefore(self) -> float: ...
-    @property
-    def ioLatencyDstBefore(self) -> float: ...
+class SnapshotFault(VimFault): ...
 
 
-class StoragePlacementAction(cluster.Action):
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def relocateSpec(self) -> vm.RelocateSpec: ...
-    @property
-    def destination(self) -> Datastore: ...
-    @property
-    def spaceUtilBefore(self) -> float: ...
-    @property
-    def spaceDemandBefore(self) -> float: ...
-    @property
-    def spaceUtilAfter(self) -> float: ...
-    @property
-    def spaceDemandAfter(self) -> float: ...
+class SnapshotIncompatibleDeviceInVm(SnapshotFault):
     @property
-    def ioLatencyBefore(self) -> float: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
 
 
-class StoragePlacementResult(vmodl.DynamicData):
-    @property
-    def recommendations(self) -> List[cluster.Recommendation]: ...
-    @property
-    def drsFault(self) -> cluster.DrsFaults: ...
-    @property
-    def task(self) -> Task: ...
+class SnapshotLocked(SnapshotFault): ...
 
 
-class StoragePlacementSpec(vmodl.DynamicData):
-    @property
-    def type(self) -> str: ...
-    @property
-    def priority(self) -> VirtualMachine.MovePriority: ...
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def podSelectionSpec(self) -> storageDrs.PodSelectionSpec: ...
-    @property
-    def cloneSpec(self) -> vm.CloneSpec: ...
-    @property
-    def cloneName(self) -> str: ...
-    @property
-    def configSpec(self) -> vm.ConfigSpec: ...
-    @property
-    def relocateSpec(self) -> vm.RelocateSpec: ...
-    @property
-    def resourcePool(self) -> ResourcePool: ...
-    @property
-    def host(self) -> HostSystem: ...
-    @property
-    def folder(self) -> Folder: ...
-    @property
-    def disallowPrerequisiteMoves(self) -> bool: ...
-    @property
-    def resourceLeaseDurationSec(self) -> int: ...
+class SnapshotMoveFromNonHomeNotSupported(SnapshotCopyNotSupported): ...
 
 
-    class PlacementType(Enum):
-        create = "create"
-        reconfigure = "reconfigure"
-        relocate = "relocate"
-        clone = "clone"
+class SnapshotMoveNotSupported(SnapshotCopyNotSupported): ...
 
 
-class VirtualDiskAntiAffinityRuleSpec(cluster.RuleInfo):
-    @property
-    def diskId(self) -> List[int]: ...
+class SnapshotMoveToNonHomeNotSupported(SnapshotCopyNotSupported): ...
 
 
-class VirtualDiskRuleSpec(cluster.RuleInfo):
-    @property
-    def diskRuleType(self) -> str: ...
-    @property
-    def diskId(self) -> List[int]: ...
+class SnapshotNoChange(SnapshotFault): ...
 
 
-class VmConfigInfo(vmodl.DynamicData):
-    @property
-    def vm(self) -> VirtualMachine: ...
-    @property
-    def enabled(self) -> bool: ...
-    @property
-    def behavior(self) -> str: ...
+class SnapshotRevertIssue(MigrationFault):
     @property
-    def intraVmAffinity(self) -> bool: ...
+    def snapshotName(self) -> str: ...
+    @snapshotName.setter
+    def snapshotName(self, value: str):
+        self._snapshotName = value
     @property
-    def intraVmAntiAffinity(self) -> storageDrs.VirtualDiskAntiAffinityRuleSpec: ...
+    def event(self) -> List[vim.event.Event]: ...
+    @event.setter
+    def event(self, value: List[vim.event.Event]):
+        self._event = value
     @property
-    def virtualDiskRules(self) -> List[storageDrs.VirtualDiskRuleSpec]: ...
+    def errors(self) -> bool: ...
+    @errors.setter
+    def errors(self, value: bool):
+        self._errors = value
 
 
-class VmConfigSpec(option.ArrayUpdateSpec):
+class SoftRuleVioCorrectionDisallowed(VmConfigFault):
     @property
-    def info(self) -> storageDrs.VmConfigInfo: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
 
 
-class CloneSpec(vmodl.DynamicData):
-    @property
-    def location(self) -> Datastore: ...
-    @property
-    def host(self) -> HostSystem: ...
-    @property
-    def resourceSpec(self) -> ResourceConfigSpec: ...
+class SoftRuleVioCorrectionImpact(VmConfigFault):
     @property
-    def vmFolder(self) -> Folder: ...
-    @property
-    def networkMapping(self) -> List[vApp.CloneSpec.NetworkMappingPair]: ...
-    @property
-    def property(self) -> List[KeyValue]: ...
-    @property
-    def resourceMapping(self) -> List[vApp.CloneSpec.ResourceMap]: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
+
+
+class SolutionUserRequired(SecurityError): ...
+
+
+class SsdDiskNotAvailable(VimFault):
     @property
-    def provisioning(self) -> str: ...
+    def devicePath(self) -> str: ...
+    @devicePath.setter
+    def devicePath(self, value: str):
+        self._devicePath = value
+
+
+class StorageDrsCannotMoveDiskInMultiWriterMode(VimFault): ...
+
+
+class StorageDrsCannotMoveFTVm(VimFault): ...
+
+
+class StorageDrsCannotMoveIndependentDisk(VimFault): ...
+
 
+class StorageDrsCannotMoveManuallyPlacedSwapFile(VimFault): ...
 
-    class ProvisioningType(Enum):
-        sameAsSource = "sameassource"
-        thin = "thin"
-        thick = "thick"
 
+class StorageDrsCannotMoveManuallyPlacedVm(VimFault): ...
 
-class NetworkMappingPair(vmodl.DynamicData):
+
+class StorageDrsCannotMoveSharedDisk(VimFault): ...
+
+
+class StorageDrsCannotMoveTemplate(VimFault): ...
+
+
+class StorageDrsCannotMoveVmInUserFolder(VimFault): ...
+
+
+class StorageDrsCannotMoveVmWithMountedCDROM(VimFault): ...
+
+
+class StorageDrsCannotMoveVmWithNoFilesInLayout(VimFault): ...
+
+
+class StorageDrsDatacentersCannotShareDatastore(VimFault): ...
+
+
+class StorageDrsDisabledOnVm(VimFault): ...
+
+
+class StorageDrsHbrDiskNotMovable(VimFault):
     @property
-    def source(self) -> Network: ...
+    def nonMovableDiskIds(self) -> str: ...
+    @nonMovableDiskIds.setter
+    def nonMovableDiskIds(self, value: str):
+        self._nonMovableDiskIds = value
+
+
+class StorageDrsHmsMoveInProgress(VimFault): ...
+
+
+class StorageDrsHmsUnreachable(VimFault): ...
+
+
+class StorageDrsIolbDisabledInternally(VimFault): ...
+
+
+class StorageDrsRelocateDisabled(VimFault): ...
+
+
+class StorageDrsStaleHmsCollection(VimFault): ...
+
+
+class StorageDrsUnableToMoveFiles(VimFault): ...
+
+
+class StorageVMotionNotSupported(MigrationFeatureNotSupported): ...
+
+
+class StorageVmotionIncompatible(VirtualHardwareCompatibilityIssue):
     @property
-    def destination(self) -> Network: ...
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
+
+
+class SuspendedRelocateNotSupported(MigrationFault): ...
+
+
+class SwapDatastoreNotWritableOnHost(DatastoreNotWritableOnHost): ...
+
+
+class SwapDatastoreUnset(VimFault): ...
+
+
+class SwapPlacementOverrideNotSupported(InvalidVmConfig): ...
+
+
+class SwitchIpUnset(DvsFault): ...
+
+
+class SwitchNotInUpgradeMode(DvsFault): ...
 
 
-class ResourceMap(vmodl.DynamicData):
+class TaskInProgress(VimFault):
     @property
-    def source(self) -> ManagedEntity: ...
+    def task(self) -> vim.Task: ...
+    @task.setter
+    def task(self, value: vim.Task):
+        self._task = value
+
+
+class ThirdPartyLicenseAssignmentFailed(vmodl.RuntimeFault):
     @property
-    def parent(self) -> ResourcePool: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def resourceSpec(self) -> ResourceConfigSpec: ...
+    def module(self) -> str: ...
+    @module.setter
+    def module(self, value: str):
+        self._module = value
     @property
-    def location(self) -> Datastore: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
+
+
+class Timedout(VimFault): ...
+
+
+class TooManyConcurrentNativeClones(FileFault): ...
+
 
+class TooManyConsecutiveOverrides(VimFault): ...
 
-class EntityConfigInfo(vmodl.DynamicData):
+
+class TooManyDevices(InvalidVmConfig): ...
+
+
+class TooManyDisksOnLegacyHost(MigrationFault):
     @property
-    def key(self) -> ManagedEntity: ...
+    def diskCount(self) -> int: ...
+    @diskCount.setter
+    def diskCount(self, value: int):
+        self._diskCount = value
     @property
-    def tag(self) -> str: ...
+    def timeoutDanger(self) -> bool: ...
+    @timeoutDanger.setter
+    def timeoutDanger(self, value: bool):
+        self._timeoutDanger = value
+
+
+class TooManyGuestLogons(GuestOperationsFault): ...
+
+
+class TooManyHosts(HostConnectFault): ...
+
+
+class TooManyNativeCloneLevels(FileFault): ...
+
+
+class TooManyNativeClonesOnFile(FileFault): ...
+
+
+class TooManySnapshotLevels(SnapshotFault): ...
+
+
+class ToolsAlreadyUpgraded(VmToolsUpgradeFault): ...
+
+
+class ToolsAutoUpgradeNotSupported(VmToolsUpgradeFault): ...
+
+
+class ToolsImageCopyFailed(VmToolsUpgradeFault): ...
+
+
+class ToolsImageNotAvailable(VmToolsUpgradeFault): ...
+
+
+class ToolsImageSignatureCheckFailed(VmToolsUpgradeFault): ...
+
+
+class ToolsInstallationInProgress(MigrationFault): ...
+
+
+class ToolsUnavailable(VimFault): ...
+
+
+class ToolsUpgradeCancelled(VmToolsUpgradeFault): ...
+
+
+class UnSupportedDatastoreForVFlash(UnsupportedDatastore):
     @property
-    def startOrder(self) -> int: ...
+    def datastoreName(self) -> str: ...
+    @datastoreName.setter
+    def datastoreName(self, value: str):
+        self._datastoreName = value
     @property
-    def startDelay(self) -> int: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
+
+
+class UncommittedUndoableDisk(MigrationFault): ...
+
+
+class UnconfiguredPropertyValue(InvalidPropertyValue): ...
+
+
+class UncustomizableGuest(CustomizationFault):
     @property
-    def waitingForGuest(self) -> bool: ...
+    def uncustomizableGuestOS(self) -> str: ...
+    @uncustomizableGuestOS.setter
+    def uncustomizableGuestOS(self, value: str):
+        self._uncustomizableGuestOS = value
+
+
+class UnexpectedCustomizationFault(CustomizationFault): ...
+
+
+class UnrecognizedHost(VimFault):
     @property
-    def startAction(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+
+
+class UnsharedSwapVMotionNotSupported(MigrationFeatureNotSupported): ...
+
+
+class UnsupportedDatastore(VmConfigFault):
     @property
-    def stopDelay(self) -> int: ...
+    def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
+
+
+class UnsupportedGuest(InvalidVmConfig):
     @property
-    def stopAction(self) -> str: ...
+    def unsupportedGuestOS(self) -> str: ...
+    @unsupportedGuestOS.setter
+    def unsupportedGuestOS(self, value: str):
+        self._unsupportedGuestOS = value
+
+
+class UnsupportedVimApiVersion(VimFault):
     @property
-    def destroyWithParent(self) -> bool: ...
+    def version(self) -> str: ...
+    @version.setter
+    def version(self, value: str):
+        self._version = value
 
 
-    class Action(Enum):
-        none = "none"
-        powerOn = "poweron"
-        powerOff = "poweroff"
-        guestShutdown = "guestshutdown"
-        suspend = "suspend"
+class UnsupportedVmxLocation(VmConfigFault): ...
 
 
-class IPAssignmentInfo(vmodl.DynamicData):
-    @property
-    def supportedAllocationScheme(self) -> List[str]: ...
-    @property
-    def ipAllocationPolicy(self) -> str: ...
+class UnusedVirtualDiskBlocksNotScrubbed(DeviceBackingNotSupported): ...
+
+
+class UserNotFound(VimFault):
     @property
-    def supportedIpProtocol(self) -> List[str]: ...
+    def principal(self) -> str: ...
+    @principal.setter
+    def principal(self, value: str):
+        self._principal = value
     @property
-    def ipProtocol(self) -> str: ...
+    def unresolved(self) -> bool: ...
+    @unresolved.setter
+    def unresolved(self, value: bool):
+        self._unresolved = value
 
 
-    class AllocationSchemes(Enum):
-        dhcp = "dhcp"
-        ovfenv = "ovfenv"
+class VAppConfigFault(VimFault): ...
 
 
-    class IpAllocationPolicy(Enum):
-        dhcpPolicy = "dhcppolicy"
-        transientPolicy = "transientpolicy"
-        fixedPolicy = "fixedpolicy"
-        fixedAllocatedPolicy = "fixedallocatedpolicy"
+class VAppNotRunning(VmConfigFault): ...
 
 
-    class Protocols(Enum):
-        IPv4 = "ipv4"
-        IPv6 = "ipv6"
+class VAppOperationInProgress(vmodl.RuntimeFault): ...
 
 
-class IpPool(vmodl.DynamicData):
+class VAppPropertyFault(VmConfigFault):
     @property
-    def id(self) -> int: ...
+    def id(self) -> str: ...
+    @id.setter
+    def id(self, value: str):
+        self._id = value
     @property
-    def name(self) -> str: ...
+    def category(self) -> str: ...
+    @category.setter
+    def category(self, value: str):
+        self._category = value
     @property
-    def ipv4Config(self) -> vApp.IpPool.IpPoolConfigInfo: ...
+    def label(self) -> str: ...
+    @label.setter
+    def label(self, value: str):
+        self._label = value
     @property
-    def ipv6Config(self) -> vApp.IpPool.IpPoolConfigInfo: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def dnsDomain(self) -> str: ...
+    def value(self) -> str: ...
+    @value.setter
+    def value(self, value: str):
+        self._value = value
+
+
+class VAppTaskInProgress(TaskInProgress): ...
+
+
+class VFlashCacheHotConfigNotSupported(VmConfigFault): ...
+
+
+class VFlashModuleNotSupported(VmConfigFault):
     @property
-    def dnsSearchPath(self) -> str: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def hostPrefix(self) -> str: ...
+    def moduleName(self) -> str: ...
+    @moduleName.setter
+    def moduleName(self, value: str):
+        self._moduleName = value
     @property
-    def httpProxy(self) -> str: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def networkAssociation(self) -> List[vApp.IpPool.Association]: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
+
+
+class VFlashModuleVersionIncompatible(VimFault):
     @property
-    def availableIpv4Addresses(self) -> int: ...
+    def moduleName(self) -> str: ...
+    @moduleName.setter
+    def moduleName(self, value: str):
+        self._moduleName = value
     @property
-    def availableIpv6Addresses(self) -> int: ...
+    def vmRequestModuleVersion(self) -> str: ...
+    @vmRequestModuleVersion.setter
+    def vmRequestModuleVersion(self, value: str):
+        self._vmRequestModuleVersion = value
     @property
-    def allocatedIpv4Addresses(self) -> int: ...
+    def hostMinSupportedVerson(self) -> str: ...
+    @hostMinSupportedVerson.setter
+    def hostMinSupportedVerson(self, value: str):
+        self._hostMinSupportedVerson = value
     @property
-    def allocatedIpv6Addresses(self) -> int: ...
+    def hostModuleVersion(self) -> str: ...
+    @hostModuleVersion.setter
+    def hostModuleVersion(self, value: str):
+        self._hostModuleVersion = value
 
 
-class Association(vmodl.DynamicData):
-    @property
-    def network(self) -> Network: ...
-    @property
-    def networkName(self) -> str: ...
+class VMINotSupported(DeviceNotSupported): ...
 
 
-class IpPoolConfigInfo(vmodl.DynamicData):
-    @property
-    def subnetAddress(self) -> str: ...
+class VMOnConflictDVPort(CannotAccessNetwork): ...
+
+
+class VMOnVirtualIntranet(CannotAccessNetwork): ...
+
+
+class VMotionAcrossNetworkNotSupported(MigrationFeatureNotSupported): ...
+
+
+class VMotionInterfaceIssue(MigrationFault):
     @property
-    def netmask(self) -> str: ...
+    def atSourceHost(self) -> bool: ...
+    @atSourceHost.setter
+    def atSourceHost(self, value: bool):
+        self._atSourceHost = value
     @property
-    def gateway(self) -> str: ...
+    def failedHost(self) -> str: ...
+    @failedHost.setter
+    def failedHost(self, value: str):
+        self._failedHost = value
     @property
-    def range(self) -> str: ...
+    def failedHostEntity(self) -> vim.HostSystem: ...
+    @failedHostEntity.setter
+    def failedHostEntity(self, value: vim.HostSystem):
+        self._failedHostEntity = value
+
+
+class VMotionLinkCapacityLow(VMotionInterfaceIssue):
     @property
-    def dns(self) -> List[str]: ...
+    def network(self) -> str: ...
+    @network.setter
+    def network(self, value: str):
+        self._network = value
+
+
+class VMotionLinkDown(VMotionInterfaceIssue):
     @property
-    def dhcpServerAvailable(self) -> bool: ...
+    def network(self) -> str: ...
+    @network.setter
+    def network(self, value: str):
+        self._network = value
+
+
+class VMotionNotConfigured(VMotionInterfaceIssue): ...
+
+
+class VMotionNotLicensed(VMotionInterfaceIssue): ...
+
+
+class VMotionNotSupported(VMotionInterfaceIssue): ...
+
+
+class VMotionProtocolIncompatible(MigrationFault): ...
+
+
+class VimFault(vmodl.MethodFault): ...
+
+
+class VirtualDiskBlocksNotFullyProvisioned(DeviceBackingNotSupported): ...
+
+
+class VirtualDiskModeNotSupported(DeviceNotSupported):
     @property
-    def ipPoolEnabled(self) -> bool: ...
+    def mode(self) -> str: ...
+    @mode.setter
+    def mode(self, value: str):
+        self._mode = value
+
+
+class VirtualEthernetCardNotSupported(DeviceNotSupported): ...
+
 
+class VirtualHardwareCompatibilityIssue(VmConfigFault): ...
 
-class OvfSectionInfo(vmodl.DynamicData):
+
+class VirtualHardwareVersionNotSupported(VirtualHardwareCompatibilityIssue):
     @property
-    def key(self) -> int: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def namespace(self) -> str: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
+
+
+class VmAlreadyExistsInDatacenter(InvalidFolder):
     @property
-    def type(self) -> str: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def atEnvelopeLevel(self) -> bool: ...
+    def hostname(self) -> str: ...
+    @hostname.setter
+    def hostname(self, value: str):
+        self._hostname = value
     @property
-    def contents(self) -> str: ...
+    def vm(self) -> List[vim.VirtualMachine]: ...
+    @vm.setter
+    def vm(self, value: List[vim.VirtualMachine]):
+        self._vm = value
 
 
-class OvfSectionSpec(option.ArrayUpdateSpec):
-    @property
-    def info(self) -> vApp.OvfSectionInfo: ...
+class VmConfigFault(VimFault): ...
 
 
-class ProductInfo(vmodl.DynamicData):
+class VmConfigIncompatibleForFaultTolerance(VmConfigFault):
     @property
-    def key(self) -> int: ...
-    @property
-    def classId(self) -> str: ...
-    @property
-    def instanceId(self) -> str: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
+
+
+class VmConfigIncompatibleForRecordReplay(VmConfigFault):
     @property
-    def name(self) -> str: ...
+    def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
+
+
+class VmFaultToleranceConfigIssue(VmFaultToleranceIssue):
     @property
-    def vendor(self) -> str: ...
+    def reason(self) -> str: ...
+    @reason.setter
+    def reason(self, value: str):
+        self._reason = value
     @property
-    def version(self) -> str: ...
+    def entityName(self) -> str: ...
+    @entityName.setter
+    def entityName(self, value: str):
+        self._entityName = value
+    @property
+    def entity(self) -> vim.ManagedEntity: ...
+    @entity.setter
+    def entity(self, value: vim.ManagedEntity):
+        self._entity = value
+
+
+    class ReasonForIssue(Enum):
+        haNotEnabled = "haNotEnabled"
+        moreThanOneSecondary = "moreThanOneSecondary"
+        recordReplayNotSupported = "recordReplayNotSupported"
+        replayNotSupported = "replayNotSupported"
+        templateVm = "templateVm"
+        multipleVCPU = "multipleVCPU"
+        hostInactive = "hostInactive"
+        ftUnsupportedHardware = "ftUnsupportedHardware"
+        ftUnsupportedProduct = "ftUnsupportedProduct"
+        missingVMotionNic = "missingVMotionNic"
+        missingFTLoggingNic = "missingFTLoggingNic"
+        thinDisk = "thinDisk"
+        verifySSLCertificateFlagNotSet = "verifySSLCertificateFlagNotSet"
+        hasSnapshots = "hasSnapshots"
+        noConfig = "noConfig"
+        ftSecondaryVm = "ftSecondaryVm"
+        hasLocalDisk = "hasLocalDisk"
+        esxAgentVm = "esxAgentVm"
+        video3dEnabled = "video3dEnabled"
+        hasUnsupportedDisk = "hasUnsupportedDisk"
+        insufficientBandwidth = "insufficientBandwidth"
+        hasNestedHVConfiguration = "hasNestedHVConfiguration"
+        hasVFlashConfiguration = "hasVFlashConfiguration"
+        unsupportedProduct = "unsupportedProduct"
+        cpuHvUnsupported = "cpuHvUnsupported"
+        cpuHwmmuUnsupported = "cpuHwmmuUnsupported"
+        cpuHvDisabled = "cpuHvDisabled"
+        hasEFIFirmware = "hasEFIFirmware"
+        tooManyVCPUs = "tooManyVCPUs"
+        tooMuchMemory = "tooMuchMemory"
+        vMotionNotLicensed = "vMotionNotLicensed"
+        ftNotLicensed = "ftNotLicensed"
+        haAgentIssue = "haAgentIssue"
+        unsupportedSPBM = "unsupportedSPBM"
+        hasLinkedCloneDisk = "hasLinkedCloneDisk"
+        unsupportedPMemHAFailOver = "unsupportedPMemHAFailOver"
+        unsupportedEncryptedDisk = "unsupportedEncryptedDisk"
+
+
+class VmFaultToleranceConfigIssueWrapper(VmFaultToleranceIssue):
     @property
-    def fullVersion(self) -> str: ...
+    def entityName(self) -> str: ...
+    @entityName.setter
+    def entityName(self, value: str):
+        self._entityName = value
+    @property
+    def entity(self) -> vim.ManagedEntity: ...
+    @entity.setter
+    def entity(self, value: vim.ManagedEntity):
+        self._entity = value
     @property
-    def vendorUrl(self) -> str: ...
+    def error(self) -> vmodl.MethodFault: ...
+    @error.setter
+    def error(self, value: vmodl.MethodFault):
+        self._error = value
+
+
+class VmFaultToleranceInvalidFileBacking(VmFaultToleranceIssue):
     @property
-    def productUrl(self) -> str: ...
+    def backingType(self) -> str: ...
+    @backingType.setter
+    def backingType(self, value: str):
+        self._backingType = value
     @property
-    def appUrl(self) -> str: ...
+    def backingFilename(self) -> str: ...
+    @backingFilename.setter
+    def backingFilename(self, value: str):
+        self._backingFilename = value
 
 
-class ProductSpec(option.ArrayUpdateSpec):
-    @property
-    def info(self) -> vApp.ProductInfo: ...
+class VmFaultToleranceIssue(VimFault): ...
 
 
-class PropertyInfo(vmodl.DynamicData):
-    @property
-    def key(self) -> int: ...
-    @property
-    def classId(self) -> str: ...
-    @property
-    def instanceId(self) -> str: ...
+class VmFaultToleranceOpIssuesList(VmFaultToleranceIssue):
     @property
-    def id(self) -> str: ...
-    @property
-    def category(self) -> str: ...
+    def errors(self) -> List[vmodl.MethodFault]: ...
+    @errors.setter
+    def errors(self, value: List[vmodl.MethodFault]):
+        self._errors = value
     @property
-    def label(self) -> str: ...
+    def warnings(self) -> List[vmodl.MethodFault]: ...
+    @warnings.setter
+    def warnings(self, value: List[vmodl.MethodFault]):
+        self._warnings = value
+
+
+class VmFaultToleranceTooManyFtVcpusOnHost(InsufficientResourcesFault):
     @property
-    def type(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def typeReference(self) -> str: ...
+    def maxNumFtVcpus(self) -> int: ...
+    @maxNumFtVcpus.setter
+    def maxNumFtVcpus(self, value: int):
+        self._maxNumFtVcpus = value
+
+
+class VmFaultToleranceTooManyVMsOnHost(InsufficientResourcesFault):
     @property
-    def userConfigurable(self) -> bool: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def defaultValue(self) -> str: ...
+    def maxNumFtVms(self) -> int: ...
+    @maxNumFtVms.setter
+    def maxNumFtVms(self, value: int):
+        self._maxNumFtVms = value
+
+
+class VmHostAffinityRuleViolation(VmConfigFault):
     @property
-    def value(self) -> str: ...
+    def vmName(self) -> str: ...
+    @vmName.setter
+    def vmName(self, value: str):
+        self._vmName = value
     @property
-    def description(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
 
 
-class PropertySpec(option.ArrayUpdateSpec):
+class VmLimitLicense(NotEnoughLicenses):
     @property
-    def info(self) -> vApp.PropertyInfo: ...
+    def limit(self) -> int: ...
+    @limit.setter
+    def limit(self, value: int):
+        self._limit = value
 
 
-class VAppConfigInfo(vApp.VmConfigInfo):
-    @property
-    def entityConfig(self) -> List[vApp.EntityConfigInfo]: ...
-    @property
-    def annotation(self) -> str: ...
+class VmMetadataManagerFault(VimFault): ...
+
+
+class VmMonitorIncompatibleForFaultTolerance(VimFault): ...
+
+
+class VmPowerOnDisabled(InvalidState): ...
+
+
+class VmSmpFaultToleranceTooManyVMsOnHost(InsufficientResourcesFault):
     @property
-    def instanceUuid(self) -> str: ...
+    def hostName(self) -> str: ...
+    @hostName.setter
+    def hostName(self, value: str):
+        self._hostName = value
     @property
-    def managedBy(self) -> ext.ManagedByInfo: ...
+    def maxNumSmpFtVms(self) -> int: ...
+    @maxNumSmpFtVms.setter
+    def maxNumSmpFtVms(self, value: int):
+        self._maxNumSmpFtVms = value
+
 
+class VmToolsUpgradeFault(VimFault): ...
 
-class VAppConfigSpec(vApp.VmConfigSpec):
+
+class VmValidateMaxDevice(VimFault):
     @property
-    def entityConfig(self) -> List[vApp.EntityConfigInfo]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
     @property
-    def annotation(self) -> str: ...
+    def max(self) -> int: ...
+    @max.setter
+    def max(self, value: int):
+        self._max = value
     @property
-    def instanceUuid(self) -> str: ...
-    @property
-    def managedBy(self) -> ext.ManagedByInfo: ...
+    def count(self) -> int: ...
+    @count.setter
+    def count(self, value: int):
+        self._count = value
 
 
-class VAppImportSpec(ImportSpec):
+class VmWwnConflict(InvalidVmConfig):
     @property
-    def name(self) -> str: ...
+    def vm(self) -> vim.VirtualMachine: ...
+    @vm.setter
+    def vm(self, value: vim.VirtualMachine):
+        self._vm = value
     @property
-    def vAppConfigSpec(self) -> vApp.VAppConfigSpec: ...
+    def host(self) -> vim.HostSystem: ...
+    @host.setter
+    def host(self, value: vim.HostSystem):
+        self._host = value
     @property
-    def resourcePoolSpec(self) -> ResourceConfigSpec: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def child(self) -> List[ImportSpec]: ...
+    def wwn(self) -> long: ...
+    @wwn.setter
+    def wwn(self, value: long):
+        self._wwn = value
 
 
-class VmConfigInfo(vmodl.DynamicData):
+class VmfsAlreadyMounted(VmfsMountFault): ...
+
+
+class VmfsAmbiguousMount(VmfsMountFault): ...
+
+
+class VmfsMountFault(HostConfigFault):
     @property
-    def product(self) -> List[vApp.ProductInfo]: ...
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
+
+
+class VmotionInterfaceNotEnabled(HostPowerOpFailed): ...
+
+
+class VolumeEditorError(CustomizationFault): ...
+
+
+class VramLimitLicense(NotEnoughLicenses):
     @property
-    def property(self) -> List[vApp.PropertyInfo]: ...
+    def limit(self) -> int: ...
+    @limit.setter
+    def limit(self, value: int):
+        self._limit = value
+
+
+class VsanClusterUuidMismatch(CannotMoveVsanEnabledHost):
     @property
-    def ipAssignment(self) -> vApp.IPAssignmentInfo: ...
+    def hostClusterUuid(self) -> str: ...
+    @hostClusterUuid.setter
+    def hostClusterUuid(self, value: str):
+        self._hostClusterUuid = value
     @property
-    def eula(self) -> List[str]: ...
+    def destinationClusterUuid(self) -> str: ...
+    @destinationClusterUuid.setter
+    def destinationClusterUuid(self, value: str):
+        self._destinationClusterUuid = value
+
+
+class VsanDiskFault(VsanFault):
     @property
-    def ovfSection(self) -> List[vApp.OvfSectionInfo]: ...
+    def device(self) -> str: ...
+    @device.setter
+    def device(self, value: str):
+        self._device = value
+
+
+class VsanFault(VimFault): ...
+
+
+class VsanIncompatibleDiskMapping(VsanDiskFault): ...
+
+
+class VspanDestPortConflict(DvsFault):
     @property
-    def ovfEnvironmentTransport(self) -> List[str]: ...
+    def vspanSessionKey1(self) -> str: ...
+    @vspanSessionKey1.setter
+    def vspanSessionKey1(self, value: str):
+        self._vspanSessionKey1 = value
     @property
-    def installBootRequired(self) -> bool: ...
+    def vspanSessionKey2(self) -> str: ...
+    @vspanSessionKey2.setter
+    def vspanSessionKey2(self, value: str):
+        self._vspanSessionKey2 = value
     @property
-    def installBootStopDelay(self) -> int: ...
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
 
 
-class VmConfigSpec(vmodl.DynamicData):
+class VspanPortConflict(DvsFault):
     @property
-    def product(self) -> List[vApp.ProductSpec]: ...
+    def vspanSessionKey1(self) -> str: ...
+    @vspanSessionKey1.setter
+    def vspanSessionKey1(self, value: str):
+        self._vspanSessionKey1 = value
     @property
-    def property(self) -> List[vApp.PropertySpec]: ...
+    def vspanSessionKey2(self) -> str: ...
+    @vspanSessionKey2.setter
+    def vspanSessionKey2(self, value: str):
+        self._vspanSessionKey2 = value
     @property
-    def ipAssignment(self) -> vApp.IPAssignmentInfo: ...
-    @property
-    def eula(self) -> List[str]: ...
-    @property
-    def ovfSection(self) -> List[vApp.OvfSectionSpec]: ...
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
+
+
+class VspanPortMoveFault(DvsFault):
     @property
-    def ovfEnvironmentTransport(self) -> List[str]: ...
+    def srcPortgroupName(self) -> str: ...
+    @srcPortgroupName.setter
+    def srcPortgroupName(self, value: str):
+        self._srcPortgroupName = value
     @property
-    def installBootRequired(self) -> bool: ...
+    def destPortgroupName(self) -> str: ...
+    @destPortgroupName.setter
+    def destPortgroupName(self, value: str):
+        self._destPortgroupName = value
     @property
-    def installBootStopDelay(self) -> int: ...
-
-
-class CorrelationState(version.version8): ...
-
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
 
-class CorrelationState(version.version8): ...
 
-
-class State(version.version7): ...
-
-
-class QuiesceMode(version.version10): ...
-
-
-class OstNodeType(version.version7): ...
+class VspanPortPromiscChangeFault(DvsFault):
+    @property
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
 
 
-class RuleScope(version.version10): ...
+class VspanPortgroupPromiscChangeFault(DvsFault):
+    @property
+    def portgroupName(self) -> str: ...
+    @portgroupName.setter
+    def portgroupName(self, value: str):
+        self._portgroupName = value
 
 
-class RuleType(version.version10): ...
+class VspanPortgroupTypeChangeFault(DvsFault):
+    @property
+    def portgroupName(self) -> str: ...
+    @portgroupName.setter
+    def portgroupName(self, value: str):
+        self._portgroupName = value
 
 
-class Behavior(version.version7): ...
+class VspanPromiscuousPortNotSupported(DvsFault):
+    @property
+    def vspanSessionKey(self) -> str: ...
+    @vspanSessionKey.setter
+    def vspanSessionKey(self, value: str):
+        self._vspanSessionKey = value
+    @property
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
 
 
-class SpaceThresholdMode(version.version10): ...
+class VspanSameSessionPortConflict(DvsFault):
+    @property
+    def vspanSessionKey(self) -> str: ...
+    @vspanSessionKey.setter
+    def vspanSessionKey(self, value: str):
+        self._vspanSessionKey = value
+    @property
+    def portKey(self) -> str: ...
+    @portKey.setter
+    def portKey(self, value: str):
+        self._portKey = value
 
 
-class PlacementType(version.version7): ...
+class WakeOnLanNotSupported(VirtualHardwareCompatibilityIssue): ...
 
 
-class RuleType(version.version12): ...
+class WakeOnLanNotSupportedByVmotionNIC(HostPowerOpFailed): ...
 
 
-class ProvisioningType(version.version6): ...
+class WillLoseHAProtection(MigrationFault):
+    @property
+    def resolution(self) -> str: ...
+    @resolution.setter
+    def resolution(self, value: str):
+        self._resolution = value
 
 
-class Action(version.version5): ...
+    class Resolution(Enum):
+        svmotion = "svmotion"
+        relocate = "relocate"
 
 
-class AllocationSchemes(version.version5): ...
+class WillModifyConfigCpuRequirements(MigrationFault): ...
 
 
-class IpAllocationPolicy(version.version5): ...
+class WillResetSnapshotDirectory(MigrationFault): ...
 
 
-class Protocols(version.version5): ...
+class WipeDiskFault(VimFault): ...
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/action/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/action/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -4,54 +4,84 @@
 from pyVmomi.VmomiSupport import ManagedMethod
 
 
 class Action(vmodl.DynamicData):
 
 
     class ActionParameter(Enum):
-        targetName = "targetname"
-        alarmName = "alarmname"
-        oldStatus = "oldstatus"
-        newStatus = "newstatus"
-        triggeringSummary = "triggeringsummary"
-        declaringSummary = "declaringsummary"
-        eventDescription = "eventdescription"
+        targetName = "targetName"
+        alarmName = "alarmName"
+        oldStatus = "oldStatus"
+        newStatus = "newStatus"
+        triggeringSummary = "triggeringSummary"
+        declaringSummary = "declaringSummary"
+        eventDescription = "eventDescription"
         target = "target"
         alarm = "alarm"
 
 
 class CreateTaskAction(Action):
     @property
     def taskTypeId(self) -> str: ...
+    @taskTypeId.setter
+    def taskTypeId(self, value: str):
+        self._taskTypeId = value
     @property
     def cancelable(self) -> bool: ...
+    @cancelable.setter
+    def cancelable(self, value: bool):
+        self._cancelable = value
 
 
 class MethodAction(Action):
     @property
     def name(self) -> ManagedMethod: ...
+    @name.setter
+    def name(self, value: ManagedMethod):
+        self._name = value
     @property
     def argument(self) -> List[MethodActionArgument]: ...
+    @argument.setter
+    def argument(self, value: List[MethodActionArgument]):
+        self._argument = value
 
 
 class MethodActionArgument(vmodl.DynamicData):
     @property
     def value(self) -> object: ...
+    @value.setter
+    def value(self, value: object):
+        self._value = value
 
 
 class RunScriptAction(Action):
     @property
     def script(self) -> str: ...
+    @script.setter
+    def script(self, value: str):
+        self._script = value
 
 
 class SendEmailAction(Action):
     @property
     def toList(self) -> str: ...
+    @toList.setter
+    def toList(self, value: str):
+        self._toList = value
     @property
     def ccList(self) -> str: ...
+    @ccList.setter
+    def ccList(self, value: str):
+        self._ccList = value
     @property
     def subject(self) -> str: ...
+    @subject.setter
+    def subject(self, value: str):
+        self._subject = value
     @property
     def body(self) -> str: ...
+    @body.setter
+    def body(self, value: str):
+        self._body = value
 
 
 class SendSNMPAction(Action): ...
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/ext/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/eam/vib/__init__.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 from typing import List
-from pyVmomi import vim, vmodl
+from pyVmomi import vmodl
+from datetime import datetime
 
 
-class ExtendedProductInfo(vmodl.DynamicData):
+class VibInfo(vmodl.DynamicData):
     @property
-    def companyUrl(self) -> str: ...
+    def id(self) -> str: ...
+    @id.setter
+    def id(self, value: str):
+        self._id = value
     @property
-    def productUrl(self) -> str: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def managementUrl(self) -> str: ...
+    def version(self) -> str: ...
+    @version.setter
+    def version(self, value: str):
+        self._version = value
     @property
-    def self(self) -> vim.ManagedEntity: ...
-
-
-class ManagedByInfo(vmodl.DynamicData):
-    @property
-    def extensionKey(self) -> str: ...
-    @property
-    def type(self) -> str: ...
-
-
-class ManagedEntityInfo(vmodl.DynamicData):
+    def vendor(self) -> str: ...
+    @vendor.setter
+    def vendor(self, value: str):
+        self._vendor = value
     @property
-    def type(self) -> str: ...
+    def summary(self) -> str: ...
+    @summary.setter
+    def summary(self, value: str):
+        self._summary = value
     @property
-    def smallIconUrl(self) -> str: ...
+    def softwareTags(self) -> VibInfo.SoftwareTags: ...
+    @softwareTags.setter
+    def softwareTags(self, value: VibInfo.SoftwareTags):
+        self._softwareTags = value
     @property
-    def iconUrl(self) -> str: ...
-    @property
-    def description(self) -> str: ...
-
-
-class SolutionManagerInfo(vmodl.DynamicData):
-    @property
-    def tab(self) -> List[SolutionManagerInfo.TabInfo]: ...
-    @property
-    def smallIconUrl(self) -> str: ...
+    def releaseDate(self) -> datetime: ...
+    @releaseDate.setter
+    def releaseDate(self, value: datetime):
+        self._releaseDate = value
 
 
-    class TabInfo(vmodl.DynamicData):
-        @property
-        def label(self) -> str: ...
+    class SoftwareTags(vmodl.DynamicData):
         @property
-        def url(self) -> str: ...
+        def tags(self) -> List[str]: ...
+        @tags.setter
+        def tags(self, value: List[str]):
+            self._tags = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/profile/host/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/sms/storage/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,559 +1,532 @@
 from typing import List
 from enum import Enum
-from pyVmomi import vim, vmodl
+from pyVmomi import sms, vim, vmodl
 from datetime import datetime
-from pyVmomi.VmomiSupport import ManagedObject, NoneType, PropertyPath, binary, byte
+from pyVmomi.VmomiSupport import long
+from . import replication
 
 
-class HostProfile(vim.profile.Profile):
+class BackingConfig(vmodl.DynamicData):
     @property
-    def validationState(self) -> str: ...
+    def thinProvisionBackingIdentifier(self) -> str: ...
+    @thinProvisionBackingIdentifier.setter
+    def thinProvisionBackingIdentifier(self, value: str):
+        self._thinProvisionBackingIdentifier = value
     @property
-    def validationStateUpdateTime(self) -> datetime: ...
+    def deduplicationBackingIdentifier(self) -> str: ...
+    @deduplicationBackingIdentifier.setter
+    def deduplicationBackingIdentifier(self, value: str):
+        self._deduplicationBackingIdentifier = value
     @property
-    def validationFailureInfo(self) -> HostProfile.ValidationFailureInfo: ...
+    def autoTieringEnabled(self) -> bool: ...
+    @autoTieringEnabled.setter
+    def autoTieringEnabled(self, value: bool):
+        self._autoTieringEnabled = value
     @property
-    def complianceCheckTime(self) -> datetime: ...
+    def deduplicationEfficiency(self) -> long: ...
+    @deduplicationEfficiency.setter
+    def deduplicationEfficiency(self, value: long):
+        self._deduplicationEfficiency = value
     @property
-    def referenceHost(self) -> vim.HostSystem: ...
-    def ResetValidationState(self) -> NoneType: ...
-    def UpdateReferenceHost(self, host: vim.HostSystem) -> NoneType: ...
-    def Update(self, config: HostProfile.ConfigSpec) -> NoneType: ...
-    def Execute(self, host: vim.HostSystem, deferredParam: List[vim.profile.DeferredPolicyOptionParameter]) -> ExecuteResult: ...
+    def performanceOptimizationInterval(self) -> long: ...
+    @performanceOptimizationInterval.setter
+    def performanceOptimizationInterval(self, value: long):
+        self._performanceOptimizationInterval = value
 
 
-    class CompleteConfigSpec(HostProfile.ConfigSpec):
-        @property
-        def applyProfile(self) -> HostApplyProfile: ...
-        @property
-        def customComplyProfile(self) -> vim.profile.ComplianceProfile: ...
-        @property
-        def disabledExpressionListChanged(self) -> bool: ...
-        @property
-        def disabledExpressionList(self) -> List[str]: ...
-        @property
-        def validatorHost(self) -> vim.HostSystem: ...
-        @property
-        def validating(self) -> bool: ...
-        @property
-        def hostConfig(self) -> HostProfile.ConfigInfo: ...
-
-
-    class ConfigInfo(vim.profile.Profile.ConfigInfo):
-        @property
-        def applyProfile(self) -> HostApplyProfile: ...
-        @property
-        def defaultComplyProfile(self) -> vim.profile.ComplianceProfile: ...
-        @property
-        def defaultComplyLocator(self) -> List[vim.profile.ComplianceLocator]: ...
-        @property
-        def customComplyProfile(self) -> vim.profile.ComplianceProfile: ...
-        @property
-        def disabledExpressionList(self) -> List[str]: ...
-        @property
-        def description(self) -> vim.profile.Profile.Description: ...
-
-
-    class ConfigSpec(vim.profile.Profile.CreateSpec): ...
-
-
-    class HostBasedConfigSpec(HostProfile.ConfigSpec):
-        @property
-        def host(self) -> vim.HostSystem: ...
-        @property
-        def useHostProfileEngine(self) -> bool: ...
-
-
-    class SerializedHostProfileSpec(vim.profile.Profile.SerializedCreateSpec):
-        @property
-        def validatorHost(self) -> vim.HostSystem: ...
-        @property
-        def validating(self) -> bool: ...
-
-
-    class ValidationFailureInfo(vmodl.DynamicData):
-        @property
-        def name(self) -> str: ...
-        @property
-        def annotation(self) -> str: ...
-        @property
-        def updateType(self) -> str: ...
-        @property
-        def host(self) -> vim.HostSystem: ...
-        @property
-        def applyProfile(self) -> HostApplyProfile: ...
-        @property
-        def failures(self) -> List[vim.fault.ProfileUpdateFailed.UpdateFailure]: ...
-        @property
-        def faults(self) -> List[vmodl.MethodFault]: ...
-
-
-        class UpdateType(Enum):
-            HostBased = "hostbased"
-            Import = "import"
-            Edit = "edit"
-            Compose = "compose"
-
-
-    class ValidationState(Enum):
-        Ready = "ready"
-        Running = "running"
-        Failed = "failed"
-
-
-class HostSpecificationManager(ManagedObject):
-    def UpdateHostSpecification(self, host: vim.HostSystem, hostSpec: HostSpecification) -> NoneType: ...
-    def UpdateHostSubSpecification(self, host: vim.HostSystem, hostSubSpec: HostSubSpecification) -> NoneType: ...
-    def RetrieveHostSpecification(self, host: vim.HostSystem, fromHost: bool) -> HostSpecification: ...
-    def DeleteHostSubSpecification(self, host: vim.HostSystem, subSpecName: str) -> NoneType: ...
-    def DeleteHostSpecification(self, host: vim.HostSystem) -> NoneType: ...
-    def GetUpdatedHosts(self, startChangeID: str, endChangeID: str) -> List[vim.HostSystem]: ...
-
-
-class ProfileManager(vim.profile.ProfileManager):
-    def ApplyHostConfiguration(self, host: vim.HostSystem, configSpec: ConfigSpec, userInput: List[vim.profile.DeferredPolicyOptionParameter]) -> vim.Task: ...
-    def GenerateConfigTaskList(self, configSpec: ConfigSpec, host: vim.HostSystem) -> ProfileManager.ConfigTaskList: ...
-    def GenerateTaskList(self, configSpec: ConfigSpec, host: vim.HostSystem) -> vim.Task: ...
-    def QueryProfileMetadata(self, profileName: List[type], profile: vim.profile.Profile) -> List[vim.profile.ProfileMetadata]: ...
-    def QueryProfileStructure(self, profile: vim.profile.Profile) -> vim.profile.ProfileStructure: ...
-    def CreateDefaultProfile(self, profileType: type, profileTypeName: str, profile: vim.profile.Profile) -> vim.profile.ApplyProfile: ...
-    def UpdateAnswerFile(self, host: vim.HostSystem, configSpec: ProfileManager.AnswerFileCreateSpec) -> vim.Task: ...
-    def RetrieveAnswerFile(self, host: vim.HostSystem) -> AnswerFile: ...
-    def RetrieveAnswerFileForProfile(self, host: vim.HostSystem, applyProfile: HostApplyProfile) -> AnswerFile: ...
-    def ExportAnswerFile(self, host: vim.HostSystem) -> vim.Task: ...
-    def CheckAnswerFileStatus(self, host: List[vim.HostSystem]) -> vim.Task: ...
-    def QueryAnswerFileStatus(self, host: List[vim.HostSystem]) -> List[AnswerFileStatusResult]: ...
-    def UpdateHostCustomizations(self, hostToConfigSpecMap: List[ProfileManager.HostToConfigSpecMap]) -> vim.Task: ...
-    def RetrieveHostCustomizations(self, hosts: List[vim.HostSystem]) -> List[ProfileManager.StructuredCustomizations]: ...
-    def RetrieveHostCustomizationsForProfile(self, hosts: List[vim.HostSystem], applyProfile: HostApplyProfile) -> List[ProfileManager.StructuredCustomizations]: ...
-    def GenerateHostConfigTaskSpec(self, hostsInfo: List[ProfileManager.StructuredCustomizations]) -> vim.Task: ...
-    def ApplyEntitiesConfiguration(self, applyConfigSpecs: List[ProfileManager.ApplyHostConfigSpec]) -> vim.Task: ...
-    def ValidateComposition(self, source: vim.profile.Profile, targets: List[vim.profile.Profile], toBeMerged: HostApplyProfile, toReplaceWith: HostApplyProfile, toBeDeleted: HostApplyProfile, enableStatusToBeCopied: HostApplyProfile, errorOnly: bool) -> vim.Task: ...
-    def CompositeProfile(self, source: vim.profile.Profile, targets: List[vim.profile.Profile], toBeMerged: HostApplyProfile, toBeReplacedWith: HostApplyProfile, toBeDeleted: HostApplyProfile, enableStatusToBeCopied: HostApplyProfile) -> vim.Task: ...
-
-
-    class AnswerFileCreateSpec(vmodl.DynamicData):
-        @property
-        def validating(self) -> bool: ...
-
-
-    class AnswerFileOptionsCreateSpec(ProfileManager.AnswerFileCreateSpec):
-        @property
-        def userInput(self) -> List[vim.profile.DeferredPolicyOptionParameter]: ...
-
-
-    class AnswerFileSerializedCreateSpec(ProfileManager.AnswerFileCreateSpec):
-        @property
-        def answerFileConfigString(self) -> str: ...
-
-
-    class ApplyHostConfigResult(vmodl.DynamicData):
-        @property
-        def startTime(self) -> datetime: ...
-        @property
-        def completeTime(self) -> datetime: ...
-        @property
-        def host(self) -> vim.HostSystem: ...
-        @property
-        def status(self) -> str: ...
-        @property
-        def errors(self) -> List[vmodl.MethodFault]: ...
-
-
-    class ApplyHostConfigSpec(ExecuteResult):
-        @property
-        def host(self) -> vim.HostSystem: ...
-        @property
-        def taskListRequirement(self) -> List[str]: ...
-        @property
-        def taskDescription(self) -> List[vmodl.LocalizableMessage]: ...
-        @property
-        def rebootStateless(self) -> bool: ...
-        @property
-        def rebootHost(self) -> bool: ...
-        @property
-        def faultData(self) -> vmodl.MethodFault: ...
-
-
-    class CompositionResult(vmodl.DynamicData):
-        @property
-        def errors(self) -> List[vmodl.LocalizableMessage]: ...
-        @property
-        def results(self) -> List[ProfileManager.CompositionResult.ResultElement]: ...
-
-
-        class ResultElement(vmodl.DynamicData):
-            @property
-            def target(self) -> vim.profile.Profile: ...
-            @property
-            def status(self) -> str: ...
-            @property
-            def errors(self) -> List[vmodl.LocalizableMessage]: ...
-
-
-    class CompositionValidationResult(vmodl.DynamicData):
-        @property
-        def results(self) -> List[ProfileManager.CompositionValidationResult.ResultElement]: ...
-        @property
-        def errors(self) -> List[vmodl.LocalizableMessage]: ...
-
-
-    class ConfigTaskList(vmodl.DynamicData):
-        @property
-        def configSpec(self) -> ConfigSpec: ...
-        @property
-        def taskDescription(self) -> List[vmodl.LocalizableMessage]: ...
-        @property
-        def taskListRequirement(self) -> List[str]: ...
-
-
-    class EntityCustomizations(vmodl.DynamicData): ...
-
-
-    class HostToConfigSpecMap(vmodl.DynamicData):
-        @property
-        def host(self) -> vim.HostSystem: ...
-        @property
-        def configSpec(self) -> ProfileManager.AnswerFileCreateSpec: ...
-
-
-    class StructuredCustomizations(ProfileManager.EntityCustomizations):
-        @property
-        def entity(self) -> vim.ManagedEntity: ...
-        @property
-        def customizations(self) -> AnswerFile: ...
-
-
-    class AnswerFileStatus(Enum):
-        valid = "valid"
-        invalid = "invalid"
-        unknown = "unknown"
-
-
-    class TaskListRequirement(Enum):
-        maintenanceModeRequired = "maintenancemoderequired"
-        rebootRequired = "rebootrequired"
-
-
-class ActiveDirectoryProfile(vim.profile.ApplyProfile): ...
-
-
-class AnswerFile(vmodl.DynamicData):
-    @property
-    def userInput(self) -> List[vim.profile.DeferredPolicyOptionParameter]: ...
+class BackingStoragePool(vmodl.DynamicData):
     @property
-    def createdTime(self) -> datetime: ...
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
     @property
-    def modifiedTime(self) -> datetime: ...
-
-
-class AnswerFileStatusResult(vmodl.DynamicData):
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def checkedTime(self) -> datetime: ...
+    def capacityInMB(self) -> long: ...
+    @capacityInMB.setter
+    def capacityInMB(self, value: long):
+        self._capacityInMB = value
     @property
-    def host(self) -> vim.HostSystem: ...
-    @property
-    def status(self) -> str: ...
-    @property
-    def error(self) -> List[AnswerFileStatusResult.AnswerFileStatusError]: ...
+    def usedSpaceInMB(self) -> long: ...
+    @usedSpaceInMB.setter
+    def usedSpaceInMB(self, value: long):
+        self._usedSpaceInMB = value
 
 
-    class AnswerFileStatusError(vmodl.DynamicData):
-        @property
-        def userInputPath(self) -> vim.profile.ProfilePropertyPath: ...
-        @property
-        def errMsg(self) -> vmodl.LocalizableMessage: ...
+    class BackingStoragePoolType(Enum):
+        thinProvisioningPool = "thinProvisioningPool"
+        deduplicationPool = "deduplicationPool"
+        thinAndDeduplicationCombinedPool = "thinAndDeduplicationCombinedPool"
 
 
-class AuthenticationProfile(vim.profile.ApplyProfile):
+class DatastoreBackingPoolMapping(vmodl.DynamicData):
     @property
-    def activeDirectory(self) -> ActiveDirectoryProfile: ...
-
-
-class DateTimeProfile(vim.profile.ApplyProfile): ...
-
-
-class DvsHostVNicProfile(DvsVNicProfile): ...
-
-
-class DvsProfile(vim.profile.ApplyProfile):
+    def datastore(self) -> List[vim.Datastore]: ...
+    @datastore.setter
+    def datastore(self, value: List[vim.Datastore]):
+        self._datastore = value
     @property
-    def key(self) -> str: ...
-    @property
-    def name(self) -> str: ...
-    @property
-    def uplink(self) -> List[PnicUplinkProfile]: ...
-
+    def backingStoragePool(self) -> List[BackingStoragePool]: ...
+    @backingStoragePool.setter
+    def backingStoragePool(self, value: List[BackingStoragePool]):
+        self._backingStoragePool = value
 
-class DvsServiceConsoleVNicProfile(DvsVNicProfile): ...
 
-
-class DvsVNicProfile(vim.profile.ApplyProfile):
+class DatastorePair(vmodl.DynamicData):
     @property
-    def key(self) -> str: ...
+    def datastore1(self) -> vim.Datastore: ...
+    @datastore1.setter
+    def datastore1(self, value: vim.Datastore):
+        self._datastore1 = value
     @property
-    def ipConfig(self) -> IpAddressProfile: ...
+    def datastore2(self) -> vim.Datastore: ...
+    @datastore2.setter
+    def datastore2(self, value: vim.Datastore):
+        self._datastore2 = value
 
 
-class ExecuteResult(vmodl.DynamicData):
-    @property
-    def status(self) -> str: ...
-    @property
-    def configSpec(self) -> ConfigSpec: ...
-    @property
-    def inapplicablePath(self) -> List[PropertyPath]: ...
+class DrsMigrationCapabilityResult(vmodl.DynamicData):
     @property
-    def requireInput(self) -> List[vim.profile.DeferredPolicyOptionParameter]: ...
-    @property
-    def error(self) -> List[ExecuteResult.ExecuteError]: ...
-
-
-    class ExecuteError(vmodl.DynamicData):
-        @property
-        def path(self) -> vim.profile.ProfilePropertyPath: ...
-        @property
-        def message(self) -> vmodl.LocalizableMessage: ...
-
-
-    class Status(Enum):
-        success = "success"
-        needInput = "needinput"
-        error = "error"
-
-
-class FirewallProfile(vim.profile.ApplyProfile):
+    def recommendedDatastorePair(self) -> List[DatastorePair]: ...
+    @recommendedDatastorePair.setter
+    def recommendedDatastorePair(self, value: List[DatastorePair]):
+        self._recommendedDatastorePair = value
     @property
-    def ruleset(self) -> List[FirewallProfile.RulesetProfile]: ...
-
-
-    class RulesetProfile(vim.profile.ApplyProfile):
-        @property
-        def key(self) -> str: ...
+    def nonRecommendedDatastorePair(self) -> List[DatastorePair]: ...
+    @nonRecommendedDatastorePair.setter
+    def nonRecommendedDatastorePair(self, value: List[DatastorePair]):
+        self._nonRecommendedDatastorePair = value
 
 
-class HostApplyProfile(vim.profile.ApplyProfile):
-    @property
-    def memory(self) -> HostMemoryProfile: ...
-    @property
-    def storage(self) -> StorageProfile: ...
-    @property
-    def network(self) -> NetworkProfile: ...
-    @property
-    def datetime(self) -> DateTimeProfile: ...
-    @property
-    def firewall(self) -> FirewallProfile: ...
+class FaultDomainProviderMapping(vmodl.DynamicData):
     @property
-    def security(self) -> SecurityProfile: ...
+    def activeProvider(self) -> sms.provider.Provider: ...
+    @activeProvider.setter
+    def activeProvider(self, value: sms.provider.Provider):
+        self._activeProvider = value
     @property
-    def service(self) -> List[ServiceProfile]: ...
-    @property
-    def option(self) -> List[OptionProfile]: ...
-    @property
-    def userAccount(self) -> List[UserProfile]: ...
-    @property
-    def usergroupAccount(self) -> List[UserGroupProfile]: ...
-    @property
-    def authentication(self) -> AuthenticationProfile: ...
-
+    def faultDomainId(self) -> List[vim.vm.replication.FaultDomainId]: ...
+    @faultDomainId.setter
+    def faultDomainId(self, value: List[vim.vm.replication.FaultDomainId]):
+        self._faultDomainId = value
 
-class HostMemoryProfile(vim.profile.ApplyProfile): ...
 
-
-class HostPortGroupProfile(PortGroupProfile):
+class FcStoragePort(StoragePort):
+    @property
+    def portWwn(self) -> str: ...
+    @portWwn.setter
+    def portWwn(self, value: str):
+        self._portWwn = value
     @property
-    def ipConfig(self) -> IpAddressProfile: ...
+    def nodeWwn(self) -> str: ...
+    @nodeWwn.setter
+    def nodeWwn(self, value: str):
+        self._nodeWwn = value
 
 
-class HostSpecification(vmodl.DynamicData):
-    @property
-    def createdTime(self) -> datetime: ...
-    @property
-    def lastModified(self) -> datetime: ...
+class FcoeStoragePort(StoragePort):
     @property
-    def host(self) -> vim.HostSystem: ...
+    def portWwn(self) -> str: ...
+    @portWwn.setter
+    def portWwn(self, value: str):
+        self._portWwn = value
     @property
-    def subSpecs(self) -> List[HostSubSpecification]: ...
-    @property
-    def changeID(self) -> str: ...
+    def nodeWwn(self) -> str: ...
+    @nodeWwn.setter
+    def nodeWwn(self, value: str):
+        self._nodeWwn = value
 
 
-class HostSubSpecification(vmodl.DynamicData):
-    @property
-    def name(self) -> str: ...
+class FileSystemInfo(vmodl.DynamicData):
     @property
-    def createdTime(self) -> datetime: ...
+    def fileServerName(self) -> str: ...
+    @fileServerName.setter
+    def fileServerName(self, value: str):
+        self._fileServerName = value
     @property
-    def data(self) -> List[byte]: ...
+    def fileSystemPath(self) -> str: ...
+    @fileSystemPath.setter
+    def fileSystemPath(self, value: str):
+        self._fileSystemPath = value
     @property
-    def binaryData(self) -> binary: ...
-
-
-class IpAddressProfile(vim.profile.ApplyProfile): ...
+    def ipAddress(self) -> str: ...
+    @ipAddress.setter
+    def ipAddress(self, value: str):
+        self._ipAddress = value
 
 
-class IpRouteProfile(vim.profile.ApplyProfile):
+class IscsiStoragePort(StoragePort):
     @property
-    def staticRoute(self) -> List[StaticRouteProfile]: ...
+    def identifier(self) -> str: ...
+    @identifier.setter
+    def identifier(self, value: str):
+        self._identifier = value
 
 
-class NasStorageProfile(vim.profile.ApplyProfile):
+class LunHbaAssociation(vmodl.DynamicData):
     @property
-    def key(self) -> str: ...
+    def canonicalName(self) -> str: ...
+    @canonicalName.setter
+    def canonicalName(self, value: str):
+        self._canonicalName = value
+    @property
+    def hba(self) -> List[vim.host.HostBusAdapter]: ...
+    @hba.setter
+    def hba(self, value: List[vim.host.HostBusAdapter]):
+        self._hba = value
 
 
-class NetStackInstanceProfile(vim.profile.ApplyProfile):
-    @property
-    def key(self) -> str: ...
+class NameValuePair(vmodl.DynamicData):
     @property
-    def dnsConfig(self) -> NetworkProfile.DnsConfigProfile: ...
+    def parameterName(self) -> str: ...
+    @parameterName.setter
+    def parameterName(self, value: str):
+        self._parameterName = value
     @property
-    def ipRouteConfig(self) -> IpRouteProfile: ...
-
+    def parameterValue(self) -> str: ...
+    @parameterValue.setter
+    def parameterValue(self, value: str):
+        self._parameterValue = value
 
-class NetworkPolicyProfile(vim.profile.ApplyProfile): ...
 
-
-class NetworkProfile(vim.profile.ApplyProfile):
-    @property
-    def vswitch(self) -> List[VirtualSwitchProfile]: ...
+class StorageAlarm(vmodl.DynamicData):
     @property
-    def vmPortGroup(self) -> List[VmPortGroupProfile]: ...
+    def alarmId(self) -> long: ...
+    @alarmId.setter
+    def alarmId(self, value: long):
+        self._alarmId = value
     @property
-    def hostPortGroup(self) -> List[HostPortGroupProfile]: ...
+    def alarmType(self) -> str: ...
+    @alarmType.setter
+    def alarmType(self, value: str):
+        self._alarmType = value
     @property
-    def serviceConsolePortGroup(self) -> List[ServiceConsolePortGroupProfile]: ...
+    def containerId(self) -> str: ...
+    @containerId.setter
+    def containerId(self, value: str):
+        self._containerId = value
     @property
-    def dnsConfig(self) -> NetworkProfile.DnsConfigProfile: ...
+    def objectId(self) -> str: ...
+    @objectId.setter
+    def objectId(self, value: str):
+        self._objectId = value
     @property
-    def ipRouteConfig(self) -> IpRouteProfile: ...
+    def objectType(self) -> str: ...
+    @objectType.setter
+    def objectType(self, value: str):
+        self._objectType = value
     @property
-    def consoleIpRouteConfig(self) -> IpRouteProfile: ...
+    def status(self) -> str: ...
+    @status.setter
+    def status(self, value: str):
+        self._status = value
+    @property
+    def alarmTimeStamp(self) -> datetime: ...
+    @alarmTimeStamp.setter
+    def alarmTimeStamp(self, value: datetime):
+        self._alarmTimeStamp = value
+    @property
+    def messageId(self) -> str: ...
+    @messageId.setter
+    def messageId(self, value: str):
+        self._messageId = value
+    @property
+    def parameterList(self) -> List[NameValuePair]: ...
+    @parameterList.setter
+    def parameterList(self, value: List[NameValuePair]):
+        self._parameterList = value
+    @property
+    def alarmObject(self) -> object: ...
+    @alarmObject.setter
+    def alarmObject(self, value: object):
+        self._alarmObject = value
+
+
+class StorageArray(vmodl.DynamicData):
     @property
-    def pnic(self) -> List[PhysicalNicProfile]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+    @property
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
+    @property
+    def vendorId(self) -> str: ...
+    @vendorId.setter
+    def vendorId(self, value: str):
+        self._vendorId = value
+    @property
+    def modelId(self) -> str: ...
+    @modelId.setter
+    def modelId(self, value: str):
+        self._modelId = value
+    @property
+    def firmware(self) -> str: ...
+    @firmware.setter
+    def firmware(self, value: str):
+        self._firmware = value
+    @property
+    def alternateName(self) -> List[str]: ...
+    @alternateName.setter
+    def alternateName(self, value: List[str]):
+        self._alternateName = value
+    @property
+    def supportedBlockInterface(self) -> List[str]: ...
+    @supportedBlockInterface.setter
+    def supportedBlockInterface(self, value: List[str]):
+        self._supportedBlockInterface = value
+    @property
+    def supportedFileSystemInterface(self) -> List[str]: ...
+    @supportedFileSystemInterface.setter
+    def supportedFileSystemInterface(self, value: List[str]):
+        self._supportedFileSystemInterface = value
+    @property
+    def supportedProfile(self) -> List[str]: ...
+    @supportedProfile.setter
+    def supportedProfile(self, value: List[str]):
+        self._supportedProfile = value
+    @property
+    def priority(self) -> int: ...
+    @priority.setter
+    def priority(self, value: int):
+        self._priority = value
+    @property
+    def discoverySvc(self) -> List[vim.VasaStorageArray.DiscoverySvcInfo]: ...
+    @discoverySvc.setter
+    def discoverySvc(self, value: List[vim.VasaStorageArray.DiscoverySvcInfo]):
+        self._discoverySvc = value
+
+
+    class BlockDeviceInterface(Enum):
+        fc = "fc"
+        iscsi = "iscsi"
+        fcoe = "fcoe"
+        otherBlock = "otherBlock"
+
+
+    class FileSystemInterface(Enum):
+        nfs = "nfs"
+        otherFileSystem = "otherFileSystem"
+
+
+    class VasaProfile(Enum):
+        blockDevice = "blockDevice"
+        fileSystem = "fileSystem"
+        capability = "capability"
+        policy = "policy"
+        object = "object"
+        statistics = "statistics"
+        storageDrsBlockDevice = "storageDrsBlockDevice"
+        storageDrsFileSystem = "storageDrsFileSystem"
+
+
+class StorageCapability(vmodl.DynamicData):
+    @property
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
     @property
-    def dvswitch(self) -> List[DvsProfile]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
+    @property
+    def description(self) -> str: ...
+    @description.setter
+    def description(self, value: str):
+        self._description = value
+
+
+class StorageContainer(vmodl.DynamicData):
+    @property
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
     @property
-    def dvsServiceConsoleNic(self) -> List[DvsServiceConsoleVNicProfile]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def dvsHostNic(self) -> List[DvsHostVNicProfile]: ...
+    def maxVvolSizeInMB(self) -> long: ...
+    @maxVvolSizeInMB.setter
+    def maxVvolSizeInMB(self, value: long):
+        self._maxVvolSizeInMB = value
     @property
-    def nsxHostNic(self) -> List[NsxHostVNicProfile]: ...
+    def providerId(self) -> List[str]: ...
+    @providerId.setter
+    def providerId(self, value: List[str]):
+        self._providerId = value
     @property
-    def netStackInstance(self) -> List[NetStackInstanceProfile]: ...
+    def arrayId(self) -> List[str]: ...
+    @arrayId.setter
+    def arrayId(self, value: List[str]):
+        self._arrayId = value
     @property
-    def opaqueSwitch(self) -> OpaqueSwitchProfile: ...
+    def vvolContainerType(self) -> str: ...
+    @vvolContainerType.setter
+    def vvolContainerType(self, value: str):
+        self._vvolContainerType = value
 
 
-    class DnsConfigProfile(vim.profile.ApplyProfile): ...
+    class VvolContainerTypeEnum(Enum):
+        NFS = "NFS"
+        NFS4x = "NFS4x"
+        SCSI = "SCSI"
+        NVMe = "NVMe"
 
 
-class NsxHostVNicProfile(vim.profile.ApplyProfile):
+class StorageContainerResult(vmodl.DynamicData):
     @property
-    def key(self) -> str: ...
+    def storageContainer(self) -> List[StorageContainer]: ...
+    @storageContainer.setter
+    def storageContainer(self, value: List[StorageContainer]):
+        self._storageContainer = value
     @property
-    def ipConfig(self) -> IpAddressProfile: ...
-
+    def providerInfo(self) -> List[sms.provider.ProviderInfo]: ...
+    @providerInfo.setter
+    def providerInfo(self, value: List[sms.provider.ProviderInfo]):
+        self._providerInfo = value
 
-class OpaqueSwitchProfile(vim.profile.ApplyProfile): ...
 
-
-class OptionProfile(vim.profile.ApplyProfile):
+class StorageContainerSpec(vmodl.DynamicData):
     @property
-    def key(self) -> str: ...
+    def containerId(self) -> List[str]: ...
+    @containerId.setter
+    def containerId(self, value: List[str]):
+        self._containerId = value
 
 
-class PermissionProfile(vim.profile.ApplyProfile):
+class StorageFileSystem(vmodl.DynamicData):
     @property
-    def key(self) -> str: ...
-
-
-class PhysicalNicProfile(vim.profile.ApplyProfile):
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
     @property
-    def key(self) -> str: ...
-
-
-class PnicUplinkProfile(vim.profile.ApplyProfile):
-    @property
-    def key(self) -> str: ...
-
-
-class PortGroupProfile(vim.profile.ApplyProfile):
+    def info(self) -> List[FileSystemInfo]: ...
+    @info.setter
+    def info(self, value: List[FileSystemInfo]):
+        self._info = value
     @property
-    def key(self) -> str: ...
+    def nativeSnapshotSupported(self) -> bool: ...
+    @nativeSnapshotSupported.setter
+    def nativeSnapshotSupported(self, value: bool):
+        self._nativeSnapshotSupported = value
     @property
-    def name(self) -> str: ...
+    def thinProvisioningStatus(self) -> str: ...
+    @thinProvisioningStatus.setter
+    def thinProvisioningStatus(self, value: str):
+        self._thinProvisioningStatus = value
     @property
-    def vlan(self) -> PortGroupProfile.VlanProfile: ...
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
     @property
-    def vswitch(self) -> PortGroupProfile.VirtualSwitchSelectionProfile: ...
+    def version(self) -> str: ...
+    @version.setter
+    def version(self, value: str):
+        self._version = value
     @property
-    def networkPolicy(self) -> NetworkPolicyProfile: ...
-
+    def backingConfig(self) -> BackingConfig: ...
+    @backingConfig.setter
+    def backingConfig(self, value: BackingConfig):
+        self._backingConfig = value
 
-    class VirtualSwitchSelectionProfile(vim.profile.ApplyProfile): ...
 
+    class FileSystemInterfaceVersion(Enum):
+        NFSV3_0 = "NFSV3_0"
 
-    class VlanProfile(vim.profile.ApplyProfile): ...
 
-
-class SecurityProfile(vim.profile.ApplyProfile):
+class StorageLun(vmodl.DynamicData):
     @property
-    def permission(self) -> List[PermissionProfile]: ...
-
-
-class ServiceConsolePortGroupProfile(PortGroupProfile):
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
     @property
-    def ipConfig(self) -> IpAddressProfile: ...
-
-
-class ServiceProfile(vim.profile.ApplyProfile):
+    def vSphereLunIdentifier(self) -> str: ...
+    @vSphereLunIdentifier.setter
+    def vSphereLunIdentifier(self, value: str):
+        self._vSphereLunIdentifier = value
     @property
-    def key(self) -> str: ...
-
-
-class StaticRouteProfile(vim.profile.ApplyProfile):
+    def vendorDisplayName(self) -> str: ...
+    @vendorDisplayName.setter
+    def vendorDisplayName(self, value: str):
+        self._vendorDisplayName = value
     @property
-    def key(self) -> str: ...
-
-
-class StorageProfile(vim.profile.ApplyProfile):
+    def capacityInMB(self) -> long: ...
+    @capacityInMB.setter
+    def capacityInMB(self, value: long):
+        self._capacityInMB = value
     @property
-    def nasStorage(self) -> List[NasStorageProfile]: ...
-
-
-class UserGroupProfile(vim.profile.ApplyProfile):
+    def usedSpaceInMB(self) -> long: ...
+    @usedSpaceInMB.setter
+    def usedSpaceInMB(self, value: long):
+        self._usedSpaceInMB = value
     @property
-    def key(self) -> str: ...
-
-
-class UserProfile(vim.profile.ApplyProfile):
+    def lunThinProvisioned(self) -> bool: ...
+    @lunThinProvisioned.setter
+    def lunThinProvisioned(self, value: bool):
+        self._lunThinProvisioned = value
     @property
-    def key(self) -> str: ...
-
-
-class VirtualSwitchProfile(vim.profile.ApplyProfile):
+    def alternateIdentifier(self) -> List[str]: ...
+    @alternateIdentifier.setter
+    def alternateIdentifier(self, value: List[str]):
+        self._alternateIdentifier = value
     @property
-    def key(self) -> str: ...
+    def drsManagementPermitted(self) -> bool: ...
+    @drsManagementPermitted.setter
+    def drsManagementPermitted(self, value: bool):
+        self._drsManagementPermitted = value
     @property
-    def name(self) -> str: ...
+    def thinProvisioningStatus(self) -> str: ...
+    @thinProvisioningStatus.setter
+    def thinProvisioningStatus(self, value: str):
+        self._thinProvisioningStatus = value
     @property
-    def link(self) -> VirtualSwitchProfile.LinkProfile: ...
-    @property
-    def numPorts(self) -> VirtualSwitchProfile.NumPortsProfile: ...
-    @property
-    def networkPolicy(self) -> NetworkPolicyProfile: ...
-
-
-    class LinkProfile(vim.profile.ApplyProfile): ...
+    def backingConfig(self) -> BackingConfig: ...
+    @backingConfig.setter
+    def backingConfig(self, value: BackingConfig):
+        self._backingConfig = value
 
 
-    class NumPortsProfile(vim.profile.ApplyProfile): ...
-
-
-class VmPortGroupProfile(PortGroupProfile): ...
-
-
-class Status(vim.version.version12): ...
+class StoragePort(vmodl.DynamicData):
+    @property
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
+    @property
+    def type(self) -> str: ...
+    @type.setter
+    def type(self, value: str):
+        self._type = value
+    @property
+    def alternateName(self) -> List[str]: ...
+    @alternateName.setter
+    def alternateName(self, value: List[str]):
+        self._alternateName = value
 
 
-class Status(vim.version.version12): ...
+class StorageProcessor(vmodl.DynamicData):
+    @property
+    def uuid(self) -> str: ...
+    @uuid.setter
+    def uuid(self, value: str):
+        self._uuid = value
+    @property
+    def alternateIdentifer(self) -> List[str]: ...
+    @alternateIdentifer.setter
+    def alternateIdentifer(self, value: List[str]):
+        self._alternateIdentifer = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/scheduler/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/pbm/__init__.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,170 @@
 from typing import List
 from enum import Enum
-from pyVmomi import vim, vmodl
-from datetime import datetime
-from pyVmomi.VmomiSupport import ManagedObject, NoneType
+from pyVmomi import vmodl
+from pyVmomi.VmomiSupport import ManagedObject
+from . import auth, capability, compliance, fault, placement, profile, provider, replication
 
 
-class ScheduledTask(vim.ExtensibleManagedObject):
+class ServiceInstance(ManagedObject):
     @property
-    def info(self) -> ScheduledTaskInfo: ...
-    def Remove(self) -> NoneType: ...
-    def Reconfigure(self, spec: ScheduledTaskSpec) -> NoneType: ...
-    def Run(self) -> NoneType: ...
+    def content(self) -> ServiceInstanceContent: ...
+    def RetrieveContent(self) -> ServiceInstanceContent: ...
 
 
-class ScheduledTaskManager(ManagedObject):
+class AboutInfo(vmodl.DynamicData):
     @property
-    def scheduledTask(self) -> List[ScheduledTask]: ...
+    def name(self) -> str: ...
+    @name.setter
+    def name(self, value: str):
+        self._name = value
     @property
-    def description(self) -> ScheduledTaskDescription: ...
-    def Create(self, entity: vim.ManagedEntity, spec: ScheduledTaskSpec) -> ScheduledTask: ...
-    def RetrieveEntityScheduledTask(self, entity: vim.ManagedEntity) -> List[ScheduledTask]: ...
-    def CreateObjectScheduledTask(self, obj: ManagedObject, spec: ScheduledTaskSpec) -> ScheduledTask: ...
-    def RetrieveObjectScheduledTask(self, obj: ManagedObject) -> List[ScheduledTask]: ...
-
-
-class AfterStartupTaskScheduler(TaskScheduler):
+    def version(self) -> str: ...
+    @version.setter
+    def version(self, value: str):
+        self._version = value
     @property
-    def minute(self) -> int: ...
+    def instanceUuid(self) -> str: ...
+    @instanceUuid.setter
+    def instanceUuid(self, value: str):
+        self._instanceUuid = value
 
 
-class DailyTaskScheduler(HourlyTaskScheduler):
+class ExtendedElementDescription(vmodl.DynamicData):
     @property
-    def hour(self) -> int: ...
-
-
-class HourlyTaskScheduler(RecurrentTaskScheduler):
+    def label(self) -> str: ...
+    @label.setter
+    def label(self, value: str):
+        self._label = value
     @property
-    def minute(self) -> int: ...
-
-
-class MonthlyByDayTaskScheduler(MonthlyTaskScheduler):
+    def summary(self) -> str: ...
+    @summary.setter
+    def summary(self, value: str):
+        self._summary = value
     @property
-    def day(self) -> int: ...
-
-
-class MonthlyByWeekdayTaskScheduler(MonthlyTaskScheduler):
+    def key(self) -> str: ...
+    @key.setter
+    def key(self, value: str):
+        self._key = value
     @property
-    def offset(self) -> MonthlyByWeekdayTaskScheduler.WeekOfMonth: ...
+    def messageCatalogKeyPrefix(self) -> str: ...
+    @messageCatalogKeyPrefix.setter
+    def messageCatalogKeyPrefix(self, value: str):
+        self._messageCatalogKeyPrefix = value
     @property
-    def weekday(self) -> MonthlyByWeekdayTaskScheduler.DayOfWeek: ...
-
-
-    class DayOfWeek(Enum):
-        sunday = "sunday"
-        monday = "monday"
-        tuesday = "tuesday"
-        wednesday = "wednesday"
-        thursday = "thursday"
-        friday = "friday"
-        saturday = "saturday"
+    def messageArg(self) -> List[vmodl.KeyAnyValue]: ...
+    @messageArg.setter
+    def messageArg(self, value: List[vmodl.KeyAnyValue]):
+        self._messageArg = value
 
 
-    class WeekOfMonth(Enum):
-        first = "first"
-        second = "second"
-        third = "third"
-        fourth = "fourth"
-        last = "last"
-
-
-class MonthlyTaskScheduler(DailyTaskScheduler): ...
+class LoggingConfiguration(vmodl.DynamicData):
+    @property
+    def component(self) -> str: ...
+    @component.setter
+    def component(self, value: str):
+        self._component = value
+    @property
+    def logLevel(self) -> str: ...
+    @logLevel.setter
+    def logLevel(self, value: str):
+        self._logLevel = value
 
 
-class OnceTaskScheduler(TaskScheduler):
-    @property
-    def runAt(self) -> datetime: ...
+    class Component(Enum):
+        pbm = "pbm"
+        vslm = "vslm"
+        sms = "sms"
+        spbm = "spbm"
+        sps = "sps"
+        httpclient_header = "httpclient_header"
+        httpclient_content = "httpclient_content"
+        vmomi = "vmomi"
 
 
-class RecurrentTaskScheduler(TaskScheduler):
-    @property
-    def interval(self) -> int: ...
+    class LogLevel(Enum):
+        INFO = "INFO"
+        DEBUG = "DEBUG"
+        TRACE = "TRACE"
 
 
-class ScheduledTaskDescription(vmodl.DynamicData):
-    @property
-    def action(self) -> List[vim.TypeDescription]: ...
-    @property
-    def schedulerInfo(self) -> List[ScheduledTaskDescription.SchedulerDetail]: ...
+class ServerObjectRef(vmodl.DynamicData):
     @property
-    def state(self) -> List[vim.ElementDescription]: ...
+    def objectType(self) -> str: ...
+    @objectType.setter
+    def objectType(self, value: str):
+        self._objectType = value
     @property
-    def dayOfWeek(self) -> List[vim.ElementDescription]: ...
+    def key(self) -> str: ...
+    @key.setter
+    def key(self, value: str):
+        self._key = value
     @property
-    def weekOfMonth(self) -> List[vim.ElementDescription]: ...
+    def serverUuid(self) -> str: ...
+    @serverUuid.setter
+    def serverUuid(self, value: str):
+        self._serverUuid = value
 
 
-    class SchedulerDetail(vim.TypeDescription):
-        @property
-        def frequency(self) -> str: ...
+    class ObjectType(Enum):
+        virtualMachine = "virtualMachine"
+        virtualMachineAndDisks = "virtualMachineAndDisks"
+        virtualDiskId = "virtualDiskId"
+        virtualDiskUUID = "virtualDiskUUID"
+        datastore = "datastore"
+        vsanObjectId = "vsanObjectId"
+        fileShareId = "fileShareId"
+        host = "host"
+        cluster = "cluster"
+        unknown = "unknown"
 
 
-class ScheduledTaskInfo(ScheduledTaskSpec):
-    @property
-    def scheduledTask(self) -> ScheduledTask: ...
-    @property
-    def entity(self) -> vim.ManagedEntity: ...
-    @property
-    def lastModifiedTime(self) -> datetime: ...
-    @property
-    def lastModifiedUser(self) -> str: ...
-    @property
-    def nextRunTime(self) -> datetime: ...
-    @property
-    def prevRunTime(self) -> datetime: ...
-    @property
-    def state(self) -> vim.TaskInfo.State: ...
-    @property
-    def error(self) -> vmodl.MethodFault: ...
-    @property
-    def result(self) -> object: ...
-    @property
-    def progress(self) -> int: ...
-    @property
-    def activeTask(self) -> vim.Task: ...
-    @property
-    def taskObject(self) -> ManagedObject: ...
+    class VvolType(Enum):
+        Config = "Config"
+        Data = "Data"
+        Swap = "Swap"
 
 
-class ScheduledTaskSpec(vmodl.DynamicData):
+class ServiceInstanceContent(vmodl.DynamicData):
     @property
-    def name(self) -> str: ...
+    def aboutInfo(self) -> AboutInfo: ...
+    @aboutInfo.setter
+    def aboutInfo(self, value: AboutInfo):
+        self._aboutInfo = value
     @property
-    def description(self) -> str: ...
+    def sessionManager(self) -> auth.SessionManager: ...
+    @sessionManager.setter
+    def sessionManager(self, value: auth.SessionManager):
+        self._sessionManager = value
     @property
-    def enabled(self) -> bool: ...
+    def capabilityMetadataManager(self) -> capability.CapabilityMetadataManager: ...
+    @capabilityMetadataManager.setter
+    def capabilityMetadataManager(self, value: capability.CapabilityMetadataManager):
+        self._capabilityMetadataManager = value
     @property
-    def scheduler(self) -> TaskScheduler: ...
+    def profileManager(self) -> profile.ProfileManager: ...
+    @profileManager.setter
+    def profileManager(self, value: profile.ProfileManager):
+        self._profileManager = value
     @property
-    def action(self) -> vim.action.Action: ...
+    def complianceManager(self) -> compliance.ComplianceManager: ...
+    @complianceManager.setter
+    def complianceManager(self, value: compliance.ComplianceManager):
+        self._complianceManager = value
     @property
-    def notification(self) -> str: ...
+    def placementSolver(self) -> placement.PlacementSolver: ...
+    @placementSolver.setter
+    def placementSolver(self, value: placement.PlacementSolver):
+        self._placementSolver = value
+    @property
+    def replicationManager(self) -> replication.ReplicationManager: ...
+    @replicationManager.setter
+    def replicationManager(self, value: replication.ReplicationManager):
+        self._replicationManager = value
 
 
-class TaskScheduler(vmodl.DynamicData):
-    @property
-    def activeTime(self) -> datetime: ...
-    @property
-    def expireTime(self) -> datetime: ...
+class PbmDebugManager():
 
 
-class WeeklyTaskScheduler(DailyTaskScheduler):
-    @property
-    def sunday(self) -> bool: ...
-    @property
-    def monday(self) -> bool: ...
-    @property
-    def tuesday(self) -> bool: ...
-    @property
-    def wednesday(self) -> bool: ...
-    @property
-    def thursday(self) -> bool: ...
-    @property
-    def friday(self) -> bool: ...
-    @property
-    def saturday(self) -> bool: ...
+    class KeystoreName(Enum):
+        SMS = "SMS"
+        TRUSTED_ROOTS = "TRUSTED_ROOTS"
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/view/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/view/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/vsan/host/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/pbm/capability/__init__.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,179 +1,151 @@
 from typing import List
-from enum import Enum
-from pyVmomi import ScsiDisk, vim, vmodl
-from datetime import datetime
+from pyVmomi import pbm, vmodl
+from pyVmomi.VmomiSupport import ManagedObject
+from . import provider, types
 
 
-class ClusterStatus(vmodl.DynamicData):
-    @property
-    def uuid(self) -> str: ...
-    @property
-    def nodeUuid(self) -> str: ...
-    @property
-    def health(self) -> str: ...
-    @property
-    def nodeState(self) -> ClusterStatus.State: ...
-    @property
-    def memberUuid(self) -> List[str]: ...
+class CapabilityMetadataManager(ManagedObject): ...
 
 
-    class State(vmodl.DynamicData):
-        @property
-        def state(self) -> str: ...
-        @property
-        def completion(self) -> ClusterStatus.State.CompletionEstimate: ...
-
-
-        class CompletionEstimate(vmodl.DynamicData):
-            @property
-            def completeTime(self) -> datetime: ...
-            @property
-            def percentComplete(self) -> int: ...
+class CapabilityInstance(vmodl.DynamicData):
+    @property
+    def id(self) -> CapabilityMetadata.UniqueId: ...
+    @id.setter
+    def id(self, value: CapabilityMetadata.UniqueId):
+        self._id = value
+    @property
+    def constraint(self) -> List[ConstraintInstance]: ...
+    @constraint.setter
+    def constraint(self, value: List[ConstraintInstance]):
+        self._constraint = value
 
 
-class ConfigInfo(vmodl.DynamicData):
+class CapabilityMetadata(vmodl.DynamicData):
     @property
-    def enabled(self) -> bool: ...
+    def id(self) -> CapabilityMetadata.UniqueId: ...
+    @id.setter
+    def id(self, value: CapabilityMetadata.UniqueId):
+        self._id = value
     @property
-    def hostSystem(self) -> vim.HostSystem: ...
+    def summary(self) -> pbm.ExtendedElementDescription: ...
+    @summary.setter
+    def summary(self, value: pbm.ExtendedElementDescription):
+        self._summary = value
     @property
-    def clusterInfo(self) -> ConfigInfo.ClusterInfo: ...
+    def mandatory(self) -> bool: ...
+    @mandatory.setter
+    def mandatory(self, value: bool):
+        self._mandatory = value
     @property
-    def storageInfo(self) -> ConfigInfo.StorageInfo: ...
+    def hint(self) -> bool: ...
+    @hint.setter
+    def hint(self, value: bool):
+        self._hint = value
     @property
-    def networkInfo(self) -> ConfigInfo.NetworkInfo: ...
+    def keyId(self) -> str: ...
+    @keyId.setter
+    def keyId(self, value: str):
+        self._keyId = value
     @property
-    def faultDomainInfo(self) -> ConfigInfo.FaultDomainInfo: ...
+    def allowMultipleConstraints(self) -> bool: ...
+    @allowMultipleConstraints.setter
+    def allowMultipleConstraints(self, value: bool):
+        self._allowMultipleConstraints = value
     @property
-    def vsanEsaEnabled(self) -> bool: ...
-
-
-    class ClusterInfo(vmodl.DynamicData):
-        @property
-        def uuid(self) -> str: ...
-        @property
-        def nodeUuid(self) -> str: ...
+    def propertyMetadata(self) -> List[PropertyMetadata]: ...
+    @propertyMetadata.setter
+    def propertyMetadata(self, value: List[PropertyMetadata]):
+        self._propertyMetadata = value
 
 
-    class FaultDomainInfo(vmodl.DynamicData):
+    class UniqueId(vmodl.DynamicData):
         @property
-        def name(self) -> str: ...
-
-
-    class NetworkInfo(vmodl.DynamicData):
+        def namespace(self) -> str: ...
+        @namespace.setter
+        def namespace(self, value: str):
+            self._namespace = value
         @property
-        def port(self) -> List[ConfigInfo.NetworkInfo.PortConfig]: ...
+        def id(self) -> str: ...
+        @id.setter
+        def id(self, value: str):
+            self._id = value
 
 
-        class PortConfig(vmodl.DynamicData):
-            @property
-            def ipConfig(self) -> IpConfig: ...
-            @property
-            def device(self) -> str: ...
-
-
-    class StorageInfo(vmodl.DynamicData):
-        @property
-        def autoClaimStorage(self) -> bool: ...
-        @property
-        def diskMapping(self) -> List[DiskMapping]: ...
-        @property
-        def diskMapInfo(self) -> List[DiskMapInfo]: ...
-        @property
-        def checksumEnabled(self) -> bool: ...
-
-
-class DecommissionMode(vmodl.DynamicData):
+class ConstraintInstance(vmodl.DynamicData):
     @property
-    def objectAction(self) -> str: ...
-
+    def propertyInstance(self) -> List[PropertyInstance]: ...
+    @propertyInstance.setter
+    def propertyInstance(self, value: List[PropertyInstance]):
+        self._propertyInstance = value
 
-    class ObjectAction(Enum):
-        noAction = "noaction"
-        ensureObjectAccessibility = "ensureobjectaccessibility"
-        evacuateAllData = "evacuatealldata"
 
-
-class DiskMapInfo(vmodl.DynamicData):
-    @property
-    def mapping(self) -> DiskMapping: ...
+class GenericTypeInfo(TypeInfo):
     @property
-    def mounted(self) -> bool: ...
+    def genericTypeName(self) -> str: ...
+    @genericTypeName.setter
+    def genericTypeName(self, value: str):
+        self._genericTypeName = value
 
 
-class DiskMapResult(vmodl.DynamicData):
+class PropertyInstance(vmodl.DynamicData):
     @property
-    def mapping(self) -> DiskMapping: ...
+    def id(self) -> str: ...
+    @id.setter
+    def id(self, value: str):
+        self._id = value
     @property
-    def diskResult(self) -> List[DiskResult]: ...
+    def operator(self) -> str: ...
+    @operator.setter
+    def operator(self, value: str):
+        self._operator = value
     @property
-    def error(self) -> vmodl.MethodFault: ...
+    def value(self) -> object: ...
+    @value.setter
+    def value(self, value: object):
+        self._value = value
 
 
-class DiskMapping(vmodl.DynamicData):
-    @property
-    def ssd(self) -> ScsiDisk: ...
-    @property
-    def nonSsd(self) -> List[ScsiDisk]: ...
-
-
-class DiskResult(vmodl.DynamicData):
-    @property
-    def disk(self) -> ScsiDisk: ...
+class PropertyMetadata(vmodl.DynamicData):
     @property
-    def state(self) -> str: ...
-    @property
-    def vsanUuid(self) -> str: ...
-    @property
-    def error(self) -> vmodl.MethodFault: ...
-    @property
-    def degraded(self) -> bool: ...
-
-
-    class State(Enum):
-        inUse = "inuse"
-        eligible = "eligible"
-        ineligible = "ineligible"
-
-
-class IpConfig(vmodl.DynamicData):
+    def id(self) -> str: ...
+    @id.setter
+    def id(self, value: str):
+        self._id = value
     @property
-    def upstreamIpAddress(self) -> str: ...
+    def summary(self) -> pbm.ExtendedElementDescription: ...
+    @summary.setter
+    def summary(self, value: pbm.ExtendedElementDescription):
+        self._summary = value
     @property
-    def downstreamIpAddress(self) -> str: ...
-
-
-class MembershipInfo(vmodl.DynamicData):
+    def mandatory(self) -> bool: ...
+    @mandatory.setter
+    def mandatory(self, value: bool):
+        self._mandatory = value
     @property
-    def nodeUuid(self) -> str: ...
+    def type(self) -> TypeInfo: ...
+    @type.setter
+    def type(self, value: TypeInfo):
+        self._type = value
     @property
-    def hostname(self) -> str: ...
-
-
-class VsanDiskInfo(vmodl.DynamicData):
+    def defaultValue(self) -> object: ...
+    @defaultValue.setter
+    def defaultValue(self, value: object):
+        self._defaultValue = value
     @property
-    def vsanUuid(self) -> str: ...
+    def allowedValue(self) -> object: ...
+    @allowedValue.setter
+    def allowedValue(self, value: object):
+        self._allowedValue = value
     @property
-    def formatVersion(self) -> int: ...
+    def requirementsTypeHint(self) -> str: ...
+    @requirementsTypeHint.setter
+    def requirementsTypeHint(self, value: str):
+        self._requirementsTypeHint = value
 
 
-class VsanRuntimeInfo(vmodl.DynamicData):
-    @property
-    def membershipList(self) -> List[MembershipInfo]: ...
-    @property
-    def diskIssues(self) -> List[VsanRuntimeInfo.DiskIssue]: ...
+class TypeInfo(vmodl.DynamicData):
     @property
-    def accessGenNo(self) -> int: ...
-
-
-    class DiskIssue(vmodl.DynamicData):
-        @property
-        def diskId(self) -> str: ...
-        @property
-        def issue(self) -> str: ...
-
-
-    class DiskIssueType(Enum):
-        nonExist = "nonexist"
-        stampMismatch = "stampmismatch"
-        unknown = "unknown"
+    def typeName(self) -> str: ...
+    @typeName.setter
+    def typeName(self, value: str):
+        self._typeName = value
```

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/vslm/host/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/pyVmomi/vim/vslm/vcenter/__init__.pyi` & `pyvmomi-8.0.1.0.1/pyVmomi/vim/vslm/vcenter/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -38,25 +38,46 @@
     def DeleteVStorageObjectEx(self, id: vim.vslm.ID, datastore: vim.Datastore) -> vim.Task: ...
     def UpdateVStorageObjectMetadataEx(self, id: vim.vslm.ID, datastore: vim.Datastore, metadata: List[vim.KeyValue], deleteKeys: List[str]) -> vim.Task: ...
 
 
 class RetrieveVStorageObjSpec(vmodl.DynamicData):
     @property
     def id(self) -> vim.vslm.ID: ...
+    @id.setter
+    def id(self, value: vim.vslm.ID):
+        self._id = value
     @property
     def datastore(self) -> vim.Datastore: ...
+    @datastore.setter
+    def datastore(self, value: vim.Datastore):
+        self._datastore = value
 
 
 class VStorageObjectAssociations(vmodl.DynamicData):
     @property
     def id(self) -> vim.vslm.ID: ...
+    @id.setter
+    def id(self, value: vim.vslm.ID):
+        self._id = value
     @property
     def vmDiskAssociations(self) -> List[VStorageObjectAssociations.VmDiskAssociations]: ...
+    @vmDiskAssociations.setter
+    def vmDiskAssociations(self, value: List[VStorageObjectAssociations.VmDiskAssociations]):
+        self._vmDiskAssociations = value
     @property
     def fault(self) -> vmodl.MethodFault: ...
+    @fault.setter
+    def fault(self, value: vmodl.MethodFault):
+        self._fault = value
 
 
     class VmDiskAssociations(vmodl.DynamicData):
         @property
         def vmId(self) -> str: ...
+        @vmId.setter
+        def vmId(self, value: str):
+            self._vmId = value
         @property
-        def diskKey(self) -> int: ...
+        def diskKey(self) -> int: ...
+        @diskKey.setter
+        def diskKey(self, value: int):
+            self._diskKey = value
```

### Comparing `pyvmomi-8.0.1.0/pyvmomi.egg-info/PKG-INFO` & `pyvmomi-8.0.1.0.1/pyvmomi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvmomi
-Version: 8.0.1.0
+Version: 8.0.1.0.1
 Summary: VMware vSphere Python SDK
 Home-page: https://github.com/vmware/pyvmomi
 Author: VMware, Inc.
 Author-email: jhu@vmware.com
 License: License :: OSI Approved :: Apache Software License
 Keywords: pyvmomi,vsphere,vmware,esx
 Platform: Windows
```

### Comparing `pyvmomi-8.0.1.0/pyvmomi.egg-info/SOURCES.txt` & `pyvmomi-8.0.1.0.1/pyvmomi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,17 @@
 pyVmomi/vim/fault/__init__.pyi
 pyVmomi/vim/host/__init__.pyi
 pyVmomi/vim/net/__init__.pyi
 pyVmomi/vim/option/__init__.pyi
 pyVmomi/vim/profile/__init__.pyi
 pyVmomi/vim/profile/cluster/__init__.pyi
 pyVmomi/vim/profile/host/__init__.pyi
+pyVmomi/vim/profile/host/profileEngine/__init__.pyi
 pyVmomi/vim/scheduler/__init__.pyi
+pyVmomi/vim/storageDrs/__init__.pyi
 pyVmomi/vim/tenant/__init__.pyi
 pyVmomi/vim/vcha/__init__.pyi
 pyVmomi/vim/view/__init__.pyi
 pyVmomi/vim/vm/__init__.pyi
 pyVmomi/vim/vm/check/__init__.pyi
 pyVmomi/vim/vm/customization/__init__.pyi
 pyVmomi/vim/vm/device/__init__.pyi
```

### Comparing `pyvmomi-8.0.1.0/setup.py` & `pyvmomi-8.0.1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     required = f.read().splitlines()
 
 with open('test-requirements.txt') as f:
     required_for_tests = f.read().splitlines()
 
 setup(
     name='pyvmomi',
-    version='8.0.1.0',
+    version='8.0.1.0.1',
     description='VMware vSphere Python SDK',
     # NOTE: pypi prefers the use of RST to render docs
     long_description=read('README.rst'),
     url='https://github.com/vmware/pyvmomi',
     author='VMware, Inc.',
     author_email='jhu@vmware.com',
     packages=['pyVmomi', 'pyVim'],
```

### Comparing `pyvmomi-8.0.1.0/tests/__init__.py` & `pyvmomi-8.0.1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_datacenter_explode.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_datacenter_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_datastore_explode.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_datastore_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_host_explode.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_host_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_network_explode.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_network_explode.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_default.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_default.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_objs_match.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_objs_match.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_strip_dynamic.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_strip_dynamic.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/test_json_vm_explode_type_match.expect` & `pyvmomi-8.0.1.0.1/tests/files/test_json_vm_explode_type_match.expect`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/files/unknown_method.xml` & `pyvmomi-8.0.1.0.1/tests/files/unknown_method.xml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/basic_connection.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/basic_connection_bad_password.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/basic_connection_bad_password.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/basic_container_view.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/basic_container_view.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/http_proxy.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/http_proxy.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/iso8601_set_datetime.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/iso8601_set_datetime.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/pbm_check_compatibility.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/pbm_check_compatibility.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/root_folder_parent.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/root_folder_parent.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/smart_connection.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/smart_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/ssl_tunnel_http_failure.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/ssl_tunnel_http_failure.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/sspi_connection.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/sspi_connection.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_datacenter_explode.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datacenter_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_datastore_explode.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_datastore_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_host_explode.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_host_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_network_explode.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_network_explode.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_default.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_default.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_objs.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_objs.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_strip_dynamic.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_json_vm_explode_type.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_json_vm_explode_type.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_simple_request_serializer.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_simple_request_serializer.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/test_vm_config_iso8601.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/test_vm_config_iso8601.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/fixtures/vm_nic_data.yaml` & `pyvmomi-8.0.1.0.1/tests/fixtures/vm_nic_data.yaml`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_connect.py` & `pyvmomi-8.0.1.0.1/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_container_view.py` & `pyvmomi-8.0.1.0.1/tests/test_container_view.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_deserializer.py` & `pyvmomi-8.0.1.0.1/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_iso8601.py` & `pyvmomi-8.0.1.0.1/tests/test_iso8601.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_json.py` & `pyvmomi-8.0.1.0.1/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_managed_object.py` & `pyvmomi-8.0.1.0.1/tests/test_managed_object.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_pbm_check_compatibility.py` & `pyvmomi-8.0.1.0.1/tests/test_pbm_check_compatibility.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_serializer.py` & `pyvmomi-8.0.1.0.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `pyvmomi-8.0.1.0/tests/test_virtual_machine_object.py` & `pyvmomi-8.0.1.0.1/tests/test_virtual_machine_object.py`

 * *Files identical despite different names*

