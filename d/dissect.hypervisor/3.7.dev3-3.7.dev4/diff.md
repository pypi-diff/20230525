# Comparing `tmp/dissect.hypervisor-3.7.dev3.tar.gz` & `tmp/dissect.hypervisor-3.7.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.hypervisor-3.7.dev3.tar", last modified: Mon May 15 12:48:10 2023, max compression
+gzip compressed data, was "dissect.hypervisor-3.7.dev4.tar", last modified: Tue May 16 13:26:24 2023, max compression
```

## Comparing `dissect.hypervisor-3.7.dev3.tar` & `dissect.hypervisor-3.7.dev4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.624962 dissect.hypervisor-3.7.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-15 12:48:10.624962 dissect.hypervisor-3.7.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.596962 dissect.hypervisor-3.7.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.604962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.604962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/c_vma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/c_wim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/vma.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/wim.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/xva.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.608962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/c_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/ovf.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/pvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/vbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/vmx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.608962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_qcow2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/qcow2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.612962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/vma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.612962 dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/vmtar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.604962 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 12:48:10.000000 dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-15 12:47:58.000000 dissect.hypervisor-3.7.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:48:10.624962 dissect.hypervisor-3.7.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.616963 dissect.hypervisor-3.7.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.620962 dissect.hypervisor-3.7.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   325934 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/differencing.avhdx.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   145940 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/dynamic.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   184563 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/dynamic.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/encrypted.vmx
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/encryption.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.620962 dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/expanding.hdd
--rw-r--r--   0 runner    (1001) docker     (123)   115232 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   151327 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/fixed.vhd.gz
--rwxr-xr-x   0 runner    (1001) docker     (123)   162126 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/fixed.vhdx.gz
--rw-r--r--   0 runner    (1001) docker     (123)   110592 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/local.tgz.ve
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.620962 dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/plain.hdd
--rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)    54881 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/sesparse.vmdk.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.624962 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/DiskDescriptor.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
--rw-r--r--   0 runner    (1001) docker     (123)    45092 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/test.VMRS
--rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/test.vgz
--rw-r--r--   0 runner    (1001) docker     (123)    65107 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/test.vma.gz
--rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/data/test.vmcx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:48:10.624962 dissect.hypervisor-3.7.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_hdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_hyperv.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_pvs.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vhdx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vma.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vmdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vmtar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tests/test_vmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-15 12:47:54.000000 dissect.hypervisor-3.7.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.524042 dissect.hypervisor-3.7.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-16 13:26:24.524042 dissect.hypervisor-3.7.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.500042 dissect.hypervisor-3.7.dev4/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.504042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.504042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/c_vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/c_wim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/wim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/xva.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.508042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/c_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/ovf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/vbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/vmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.512042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20218 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/qcow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18069 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.512042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/vma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.512042 dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/vmtar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.504042 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 13:26:24.000000 dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-16 13:26:14.000000 dissect.hypervisor-3.7.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:26:24.524042 dissect.hypervisor-3.7.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.516042 dissect.hypervisor-3.7.dev4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.520042 dissect.hypervisor-3.7.dev4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   325934 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/differencing.avhdx.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   145940 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/dynamic.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   184563 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/dynamic.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/encrypted.vmx
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/encryption.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.520042 dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/expanding.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)   115232 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   151327 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/fixed.vhd.gz
+-rwxr-xr-x   0 runner    (1001) docker     (123)   162126 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/fixed.vhdx.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   110592 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/local.tgz.ve
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.520042 dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/plain.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)   114982 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    54881 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/sesparse.vmdk.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.524042 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/DiskDescriptor.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    45092 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/test.VMRS
+-rw-r--r--   0 runner    (1001) docker     (123)    16897 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/test.vgz
+-rw-r--r--   0 runner    (1001) docker     (123)    65107 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/test.vma.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    81920 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/data/test.vmcx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:24.524042 dissect.hypervisor-3.7.dev4/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_hdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_hyperv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_pvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vhdx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vmdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vmtar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tests/test_vmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-16 13:26:06.000000 dissect.hypervisor-3.7.dev4/tox.ini
```

### Comparing `dissect.hypervisor-3.7.dev3/LICENSE` & `dissect.hypervisor-3.7.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/PKG-INFO` & `dissect.hypervisor-3.7.dev4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.7.dev3
+Version: 3.7.dev4
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 License-File: COPYRIGHT
 
 # dissect.hypervisor
 
 A Dissect module implementing parsers for various hypervisor disk, backup and configuration files. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.hypervisor/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.hypervisor` is available on [PyPI](https://pypi.org/project/dissect.hypervisor/).
 
 ```bash
 pip install dissect.hypervisor
 ```
@@ -44,20 +50,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.hypervisor-3.7.dev3/README.md` & `dissect.hypervisor-3.7.dev4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # dissect.hypervisor
 
 A Dissect module implementing parsers for various hypervisor disk, backup and configuration files. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.hypervisor/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.hypervisor` is available on [PyPI](https://pypi.org/project/dissect.hypervisor/).
 
 ```bash
 pip install dissect.hypervisor
 ```
@@ -28,20 +34,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/c_vma.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/c_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/c_wim.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/c_wim.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/vma.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/backup/xva.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/backup/xva.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/c_hyperv.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/c_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/hyperv.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/ovf.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/ovf.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/pvs.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/vbox.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/descriptor/vmx.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/descriptor/vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_hdd.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_qcow2.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vdi.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vhd.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vhdx.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/c_vmdk.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/c_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/hdd.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/qcow2.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/qcow2.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vdi.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vdi.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vhd.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vhdx.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/disk/vmdk.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/disk/vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/envelope.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/tools/vma.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/tools/vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/envelope.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect/hypervisor/util/vmtar.py` & `dissect.hypervisor-3.7.dev4/dissect/hypervisor/util/vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/PKG-INFO` & `dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.hypervisor
-Version: 3.7.dev3
+Version: 3.7.dev4
 Summary: A Dissect module implementing parsers for various hypervisor disk, backup and configuration files
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.hypervisor
 Project-URL: repository, https://github.com/fox-it/dissect.hypervisor
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,20 @@
 License-File: COPYRIGHT
 
 # dissect.hypervisor
 
 A Dissect module implementing parsers for various hypervisor disk, backup and configuration files. For more information,
 please see [the documentation](https://docs.dissect.tools/en/latest/projects/dissect.hypervisor/index.html).
 
+## Requirements
+
+This project is part of the Dissect framework and requires Python.
+
+Information on the supported Python versions can be found in the Getting Started section of [the documentation](https://docs.dissect.tools/en/latest/index.html#getting-started).
+
 ## Installation
 
 `dissect.hypervisor` is available on [PyPI](https://pypi.org/project/dissect.hypervisor/).
 
 ```bash
 pip install dissect.hypervisor
 ```
@@ -44,20 +50,20 @@
 using the default installed Python version, run:
 
 ```bash
 tox
 ```
 
 For a more elaborate explanation on how to build and test the project, please see [the
-documentation](https://docs.dissect.tools/en/latest/contributing/developing.html#building-testing).
+documentation](https://docs.dissect.tools/en/latest/contributing/tooling.html).
 
 ## Contributing
 
 The Dissect project encourages any contribution to the codebase. To make your contribution fit into the project, please
-refer to [the style guide](https://docs.dissect.tools/en/latest/contributing/style-guide.html).
+refer to [the development guide](https://docs.dissect.tools/en/latest/contributing/developing.html).
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
 (<https://www.nccgroup.com>).
 
 Developed by the Dissect Team (<dissect@fox-it.com>) and made available at <https://github.com/fox-it/dissect>.
```

### Comparing `dissect.hypervisor-3.7.dev3/dissect.hypervisor.egg-info/SOURCES.txt` & `dissect.hypervisor-3.7.dev4/dissect.hypervisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/pyproject.toml` & `dissect.hypervisor-3.7.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/conftest.py` & `dissect.hypervisor-3.7.dev4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/differencing.avhdx.gz` & `dissect.hypervisor-3.7.dev4/tests/data/differencing.avhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/dynamic.vhd.gz` & `dissect.hypervisor-3.7.dev4/tests/data/dynamic.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/dynamic.vhdx.gz` & `dissect.hypervisor-3.7.dev4/tests/data/dynamic.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/encrypted.vmx` & `dissect.hypervisor-3.7.dev4/tests/data/encrypted.vmx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/expanding.hdd/expanding.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/fixed.vhd.gz` & `dissect.hypervisor-3.7.dev4/tests/data/fixed.vhd.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/fixed.vhdx.gz` & `dissect.hypervisor-3.7.dev4/tests/data/fixed.vhdx.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/local.tgz.ve` & `dissect.hypervisor-3.7.dev4/tests/data/local.tgz.ve`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/plain.hdd/plain.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/sesparse.vmdk.gz` & `dissect.hypervisor-3.7.dev4/tests/data/sesparse.vmdk.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/DiskDescriptor.xml` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/DiskDescriptor.xml`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.0.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.1.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.2.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.3.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.4.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz` & `dissect.hypervisor-3.7.dev4/tests/data/split.hdd/split.hdd.5.{5fbaabe3-6958-40ff-92a7-860e329aab41}.hds.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/test.VMRS` & `dissect.hypervisor-3.7.dev4/tests/data/test.VMRS`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/test.vgz` & `dissect.hypervisor-3.7.dev4/tests/data/test.vgz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/test.vma.gz` & `dissect.hypervisor-3.7.dev4/tests/data/test.vma.gz`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/data/test.vmcx` & `dissect.hypervisor-3.7.dev4/tests/data/test.vmcx`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/docs/Makefile` & `dissect.hypervisor-3.7.dev4/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/docs/conf.py` & `dissect.hypervisor-3.7.dev4/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_envelope.py` & `dissect.hypervisor-3.7.dev4/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_hdd.py` & `dissect.hypervisor-3.7.dev4/tests/test_hdd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_hyperv.py` & `dissect.hypervisor-3.7.dev4/tests/test_hyperv.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_pvs.py` & `dissect.hypervisor-3.7.dev4/tests/test_pvs.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vbox.py` & `dissect.hypervisor-3.7.dev4/tests/test_vbox.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vhd.py` & `dissect.hypervisor-3.7.dev4/tests/test_vhd.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vhdx.py` & `dissect.hypervisor-3.7.dev4/tests/test_vhdx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vma.py` & `dissect.hypervisor-3.7.dev4/tests/test_vma.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vmdk.py` & `dissect.hypervisor-3.7.dev4/tests/test_vmdk.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vmtar.py` & `dissect.hypervisor-3.7.dev4/tests/test_vmtar.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tests/test_vmx.py` & `dissect.hypervisor-3.7.dev4/tests/test_vmx.py`

 * *Files identical despite different names*

### Comparing `dissect.hypervisor-3.7.dev3/tox.ini` & `dissect.hypervisor-3.7.dev4/tox.ini`

 * *Files identical despite different names*

