# Comparing `tmp/tidevice-0.9.8.tar.gz` & `tmp/tidevice-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidevice-0.9.8.tar", last modified: Wed Aug 24 11:09:33 2022, max compression
+gzip compressed data, was "tidevice-0.9.9.tar", last modified: Wed Aug 24 11:44:07 2022, max compression
```

## Comparing `tidevice-0.9.8.tar` & `tidevice-0.9.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.420745 tidevice-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.412745 tidevice-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.416745 tidevice-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1425 2022-08-24 11:09:06.000000 tidevice-0.9.8/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)       64 2022-08-24 11:09:33.000000 tidevice-0.9.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)      437 2022-08-24 11:09:33.000000 tidevice-0.9.8/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (116)     2022 2022-08-24 11:09:06.000000 tidevice-0.9.8/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-08-24 11:09:06.000000 tidevice-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       77 2022-08-24 11:09:06.000000 tidevice-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-08-24 11:09:33.420745 tidevice-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      847 2022-08-24 11:09:06.000000 tidevice-0.9.8/PROTOCOL.md
--rw-r--r--   0 runner    (1001) docker     (116)    13216 2022-08-24 11:09:06.000000 tidevice-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)    11568 2022-08-24 11:09:06.000000 tidevice-0.9.8/README_EN.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.416745 tidevice-0.9.8/assets/
--rw-r--r--   0 runner    (1001) docker     (116)    12630 2022-08-24 11:09:06.000000 tidevice-0.9.8/assets/tidevice-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.416745 tidevice-0.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      120 2022-08-24 11:09:06.000000 tidevice-0.9.8/examples/get_bundle_id_from_ipa.py
--rw-r--r--   0 runner    (1001) docker     (116)      757 2022-08-24 11:09:06.000000 tidevice-0.9.8/examples/read_properties.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      289 2022-08-24 11:09:06.000000 tidevice-0.9.8/release.sh
--rw-r--r--   0 runner    (1001) docker     (116)      375 2022-08-24 11:09:06.000000 tidevice-0.9.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.416745 tidevice-0.9.8/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4012 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/ipa_sign.sh
--rw-r--r--   0 runner    (1001) docker     (116)    17538 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/plistdump-tcp-proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (116)     2979 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/run-usbmuxd-proxy.sh
--rwxr-xr-x   0 runner    (1001) docker     (116)      274 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/simple-capture.sh
--rw-r--r--   0 runner    (1001) docker     (116)     3201 2022-08-24 11:09:06.000000 tidevice-0.9.8/scripts/uitest_screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (116)      836 2022-08-24 11:09:33.424745 tidevice-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      226 2022-08-24 11:09:06.000000 tidevice-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.420745 tidevice-0.9.8/tidevice/
--rw-r--r--   0 runner    (1001) docker     (116)      349 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    30644 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      171 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_compat.py
--rw-r--r--   0 runner    (1001) docker     (116)      768 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_crash.py
--rw-r--r--   0 runner    (1001) docker     (116)    41218 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_device.py
--rw-r--r--   0 runner    (1001) docker     (116)    13829 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_hexdump.py
--rw-r--r--   0 runner    (1001) docker     (116)     6055 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_imagemounter.py
--rw-r--r--   0 runner    (1001) docker     (116)     9935 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_installation.py
--rw-r--r--   0 runner    (1001) docker     (116)    39139 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_instruments.py
--rw-r--r--   0 runner    (1001) docker     (116)     3171 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_ipautil.py
--rw-r--r--   0 runner    (1001) docker     (116)    11838 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_perf.py
--rw-r--r--   0 runner    (1001) docker     (116)    11907 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_proto.py
--rw-r--r--   0 runner    (1001) docker     (116)     2980 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_relay.py
--rw-r--r--   0 runner    (1001) docker     (116)     7591 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_safe_socket.py
--rw-r--r--   0 runner    (1001) docker     (116)     3237 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_ssl.py
--rw-r--r--   0 runner    (1001) docker     (116)    13932 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_sync.py
--rw-r--r--   0 runner    (1001) docker     (116)      609 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_types.py
--rw-r--r--   0 runner    (1001) docker     (116)     5399 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (116)     6799 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      242 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     7803 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/_wdaproxy.py
--rw-r--r--   0 runner    (1001) docker     (116)    18769 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/bplist.py
--rw-r--r--   0 runner    (1001) docker     (116)      592 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    31289 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/plistlib2.py
--rw-r--r--   0 runner    (1001) docker     (116)     3423 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/requests_usbmux.py
--rw-r--r--   0 runner    (1001) docker     (116)     3004 2022-08-24 11:09:06.000000 tidevice-0.9.8/tidevice/struct2.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:09:33.420745 tidevice-0.9.8/tidevice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      600 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1224 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       53 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-24 11:09:26.000000 tidevice-0.9.8/tidevice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (116)      145 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-08-24 11:09:33.000000 tidevice-0.9.8/tidevice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.824830 tidevice-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.816830 tidevice-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.816830 tidevice-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1425 2022-08-24 11:43:46.000000 tidevice-0.9.9/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2022-08-24 11:44:07.000000 tidevice-0.9.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (116)      391 2022-08-24 11:44:07.000000 tidevice-0.9.9/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (116)     2022 2022-08-24 11:43:46.000000 tidevice-0.9.9/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1064 2022-08-24 11:43:46.000000 tidevice-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       77 2022-08-24 11:43:46.000000 tidevice-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      600 2022-08-24 11:44:07.824830 tidevice-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      847 2022-08-24 11:43:46.000000 tidevice-0.9.9/PROTOCOL.md
+-rw-r--r--   0 runner    (1001) docker     (116)    13216 2022-08-24 11:43:46.000000 tidevice-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)    11568 2022-08-24 11:43:46.000000 tidevice-0.9.9/README_EN.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.816830 tidevice-0.9.9/assets/
+-rw-r--r--   0 runner    (1001) docker     (116)    12630 2022-08-24 11:43:46.000000 tidevice-0.9.9/assets/tidevice-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.816830 tidevice-0.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      120 2022-08-24 11:43:46.000000 tidevice-0.9.9/examples/get_bundle_id_from_ipa.py
+-rw-r--r--   0 runner    (1001) docker     (116)      757 2022-08-24 11:43:46.000000 tidevice-0.9.9/examples/read_properties.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)      289 2022-08-24 11:43:46.000000 tidevice-0.9.9/release.sh
+-rw-r--r--   0 runner    (1001) docker     (116)      375 2022-08-24 11:43:46.000000 tidevice-0.9.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.820830 tidevice-0.9.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4012 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/ipa_sign.sh
+-rw-r--r--   0 runner    (1001) docker     (116)    17538 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/plistdump-tcp-proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (116)     2979 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/run-usbmuxd-proxy.sh
+-rwxr-xr-x   0 runner    (1001) docker     (116)      274 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/simple-capture.sh
+-rw-r--r--   0 runner    (1001) docker     (116)     3201 2022-08-24 11:43:46.000000 tidevice-0.9.9/scripts/uitest_screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (116)      836 2022-08-24 11:44:07.824830 tidevice-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      226 2022-08-24 11:43:46.000000 tidevice-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.820830 tidevice-0.9.9/tidevice/
+-rw-r--r--   0 runner    (1001) docker     (116)      349 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30644 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      171 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)      768 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_crash.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41219 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_device.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13829 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_hexdump.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6055 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_imagemounter.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9935 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_installation.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39139 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_instruments.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3171 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_ipautil.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11838 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11907 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2980 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_relay.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7591 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_safe_socket.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3237 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13932 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)      609 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5399 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6799 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      242 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7803 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/_wdaproxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18769 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/bplist.py
+-rw-r--r--   0 runner    (1001) docker     (116)      592 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    31289 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/plistlib2.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3423 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/requests_usbmux.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3004 2022-08-24 11:43:46.000000 tidevice-0.9.9/tidevice/struct2.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-24 11:44:07.824830 tidevice-0.9.9/tidevice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      600 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1224 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-24 11:44:01.000000 tidevice-0.9.9/tidevice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2022-08-24 11:44:07.000000 tidevice-0.9.9/tidevice.egg-info/top_level.txt
```

### Comparing `tidevice-0.9.8/.github/workflows/publish-to-test-pypi.yml` & `tidevice-0.9.9/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/DEVELOP.md` & `tidevice-0.9.9/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/LICENSE` & `tidevice-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/PKG-INFO` & `tidevice-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidevice
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/alibaba/tidevice
 Author: 圣翔
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `tidevice-0.9.8/PROTOCOL.md` & `tidevice-0.9.9/PROTOCOL.md`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/README.md` & `tidevice-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/README_EN.md` & `tidevice-0.9.9/README_EN.md`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/assets/tidevice-logo.png` & `tidevice-0.9.9/assets/tidevice-logo.png`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/examples/read_properties.py` & `tidevice-0.9.9/examples/read_properties.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/scripts/ipa_sign.sh` & `tidevice-0.9.9/scripts/ipa_sign.sh`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/scripts/plistdump-tcp-proxy.py` & `tidevice-0.9.9/scripts/plistdump-tcp-proxy.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/scripts/run-usbmuxd-proxy.sh` & `tidevice-0.9.9/scripts/run-usbmuxd-proxy.sh`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/scripts/uitest_screenrecord.py` & `tidevice-0.9.9/scripts/uitest_screenrecord.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/setup.cfg` & `tidevice-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/__main__.py` & `tidevice-0.9.9/tidevice/__main__.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_crash.py` & `tidevice-0.9.9/tidevice/_crash.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_device.py` & `tidevice-0.9.9/tidevice/_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,16 +278,14 @@
     def _host_id(self):
         return self.pair_record['HostID']
 
     @property
     def _system_BUID(self):
         return self.pair_record['SystemBUID']
 
-    # 2022-08-24 add retry delay, looks like sometime can recover
-    @retry((ssl.SSLError, socket.timeout), delay=3, jitter=1, tries=3, logger=logging)
     def create_inner_connection(
             self,
             port: int = LOCKDOWN_PORT,  # 0xf27e,
             _ssl: bool = False,
             ssl_dial_only: bool = False) -> PlistSocketProxy:
         device_id = self.info.device_id
         conn = self._usbmux.connect_device_port(device_id, port)
@@ -785,14 +783,16 @@
         if self.major_version() >= 14:
             conn = self.start_service(
                 LockdownService.TestmanagerdLockdownSecure)
         else:
             conn = self.start_service(LockdownService.TestmanagerdLockdown)
         return DTXService(conn)
 
+    # 2022-08-24 add retry delay, looks like sometime can recover
+    @retry((ssl.SSLError, socket.timeout), delay=10, jitter=1, tries=3, logger=logging)
     def connect_instruments(self) -> ServiceInstruments:
         """ start service for instruments """
         if self.major_version() >= 14:
             conn = self.start_service(
                 LockdownService.InstrumentsRemoteServerSecure)
         else:
             conn = self.start_service(LockdownService.InstrumentsRemoteServer)
```

### Comparing `tidevice-0.9.8/tidevice/_hexdump.py` & `tidevice-0.9.9/tidevice/_hexdump.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_imagemounter.py` & `tidevice-0.9.9/tidevice/_imagemounter.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_installation.py` & `tidevice-0.9.9/tidevice/_installation.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_instruments.py` & `tidevice-0.9.9/tidevice/_instruments.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_ipautil.py` & `tidevice-0.9.9/tidevice/_ipautil.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_perf.py` & `tidevice-0.9.9/tidevice/_perf.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_proto.py` & `tidevice-0.9.9/tidevice/_proto.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_relay.py` & `tidevice-0.9.9/tidevice/_relay.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_safe_socket.py` & `tidevice-0.9.9/tidevice/_safe_socket.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_ssl.py` & `tidevice-0.9.9/tidevice/_ssl.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_sync.py` & `tidevice-0.9.9/tidevice/_sync.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_types.py` & `tidevice-0.9.9/tidevice/_types.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_usbmux.py` & `tidevice-0.9.9/tidevice/_usbmux.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_utils.py` & `tidevice-0.9.9/tidevice/_utils.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/_wdaproxy.py` & `tidevice-0.9.9/tidevice/_wdaproxy.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/bplist.py` & `tidevice-0.9.9/tidevice/bplist.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/exceptions.py` & `tidevice-0.9.9/tidevice/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/plistlib2.py` & `tidevice-0.9.9/tidevice/plistlib2.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/requests_usbmux.py` & `tidevice-0.9.9/tidevice/requests_usbmux.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice/struct2.py` & `tidevice-0.9.9/tidevice/struct2.py`

 * *Files identical despite different names*

### Comparing `tidevice-0.9.8/tidevice.egg-info/PKG-INFO` & `tidevice-0.9.9/tidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidevice
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/alibaba/tidevice
 Author: 圣翔
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `tidevice-0.9.8/tidevice.egg-info/SOURCES.txt` & `tidevice-0.9.9/tidevice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

