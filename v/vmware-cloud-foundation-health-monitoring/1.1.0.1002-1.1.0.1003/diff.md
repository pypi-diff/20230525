# Comparing `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar.gz` & `tmp/vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar", last modified: Tue May 23 23:07:20 2023, max compression
+gzip compressed data, was "vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar", last modified: Thu May 25 19:11:19 2023, max compression
```

## Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002.tar` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.040761 vmware-cloud-foundation-health-monitoring-1.1.0.1002/
--rw-rw-rw-   0        0        0    10980 2023-05-23 23:07:20.056387 vmware-cloud-foundation-health-monitoring-1.1.0.1002/PKG-INFO
--rw-rw-rw-   0        0        0    10173 2023-05-23 16:56:37.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/README.md
--rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/pyproject.toml
--rw-rw-rw-   0        0        0     1046 2023-05-23 23:07:20.056387 vmware-cloud-foundation-health-monitoring-1.1.0.1002/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:19.993891 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/
--rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Dashboards.zip
--rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Notifications.json
--rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Supermetrics.json
--rw-rw-rw-   0        0        0    10147 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Views.zip
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.009512 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/__init__.py
--rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/examples/run_send-data-to-vrops.bat
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/__init__.py
--rw-rw-rw-   0        0        0     3199 2023-05-23 18:12:09.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypt-passwords.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypted_files/
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypted_files/__init__.py
--rw-rw-rw-   0        0        0     1456 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/env.json
--rw-rw-rw-   0        0        0    70917 2023-05-23 18:12:09.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/send-data-to-vrops.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.025137 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/
--rw-rw-rw-   0        0        0     5862 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/FolderUtility.py
--rw-rw-rw-   0        0        0     4438 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/LogUtility.py
--rw-rw-rw-   0        0        0     3042 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/PSUtility.py
--rw-rw-rw-   0        0        0     7362 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/SosRest.py
--rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:07:20.040761 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/
--rw-rw-rw-   0        0        0    10980 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      915 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-23 23:07:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/
+-rw-rw-rw-   0        0        0    10980 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/PKG-INFO
+-rw-rw-rw-   0        0        0    10173 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/pyproject.toml
+-rw-rw-rw-   0        0        0     1053 2023-05-25 19:11:19.281760 vmware-cloud-foundation-health-monitoring-1.1.0.1003/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.172402 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.172402 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.219263 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/
+-rw-rw-rw-   0        0        0   150145 2023-02-28 03:47:12.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Alert_Definitions.xml
+-rw-rw-rw-   0        0        0    28694 2023-02-28 20:06:20.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Dashboards.zip
+-rw-rw-rw-   0        0        0    51491 2023-02-28 03:58:54.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Notifications.json
+-rw-rw-rw-   0        0        0    16701 2023-02-28 03:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Supermetrics.json
+-rw-rw-rw-   0        0        0    10147 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Views.zip
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/__init__.py
+-rwxrwxrwx   0        0        0       55 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/examples/run_send-data-to-vrops.bat
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/__init__.py
+-rw-rw-rw-   0        0        0     3199 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypt-passwords.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.234888 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypted_files/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypted_files/__init__.py
+-rw-rw-rw-   0        0        0     1456 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/env.json
+-rw-rw-rw-   0        0        0    70999 2023-05-25 19:10:32.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/send-data-to-vrops.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.250512 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/
+-rw-rw-rw-   0        0        0     5862 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/FolderUtility.py
+-rw-rw-rw-   0        0        0     4438 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/LogUtility.py
+-rw-rw-rw-   0        0        0     3042 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/PSUtility.py
+-rw-rw-rw-   0        0        0     7362 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/SosRest.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:53:28.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 19:11:19.266141 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/
+-rw-rw-rw-   0        0        0    10980 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-25 19:11:19.000000 vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/top_level.txt
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0.1002
+Version: 1.1.0.1003
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -61,15 +61,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/README.md` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/setup.cfg` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6d77 6172 652d 636c 6f75 642d   = vmware-cloud-
 00000020: 666f 756e 6461 7469 6f6e 2d68 6561 6c74  foundation-healt
 00000030: 682d 6d6f 6e69 746f 7269 6e67 0d0a 7665  h-monitoring..ve
 00000040: 7273 696f 6e20 3d20 312e 312e 302e 3130  rsion = 1.1.0.10
-00000050: 3032 0d0a 6175 7468 6f72 203d 2042 6875  02..author = Bhu
+00000050: 3033 0d0a 6175 7468 6f72 203d 2042 6875  03..author = Bhu
 00000060: 6d69 7472 6120 4e61 6761 720d 0a61 7574  mitra Nagar..aut
 00000070: 686f 725f 656d 6169 6c20 3d20 626e 6167  hor_email = bnag
 00000080: 6172 4076 6d77 6172 652e 636f 6d0d 0a64  ar@vmware.com..d
 00000090: 6573 6372 6970 7469 6f6e 203d 2050 7974  escription = Pyt
 000000a0: 686f 6e20 4d6f 6475 6c65 2066 6f72 2056  hon Module for V
 000000b0: 4d77 6172 6520 436c 6f75 6420 466f 756e  Mware Cloud Foun
 000000c0: 6461 7469 6f6e 2048 6561 6c74 6820 4d6f  dation Health Mo
@@ -53,14 +53,14 @@
 00000340: 650d 0a70 6163 6b61 6765 7320 3d20 6669  e..packages = fi
 00000350: 6e64 3a0d 0a70 7974 686f 6e5f 7265 7175  nd:..python_requ
 00000360: 6972 6573 203d 203e 3d33 2e36 0d0a 696e  ires = >=3.6..in
 00000370: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
 00000380: 7461 203d 2054 7275 650d 0a0d 0a5b 6f70  ta = True....[op
 00000390: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
 000003a0: 7461 5d0d 0a2a 203d 202a 2e6a 736f 6e2c  ta]..* = *.json,
-000003b0: 202a 2e62 6174 2c20 2a2e 7a69 700d 0a0d   *.bat, *.zip...
-000003c0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000003d0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000003e0: 3d20 736f 7572 6365 0d0a 0d0a 5b65 6767  = source....[egg
-000003f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000400: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000410: 2030 0d0a 0d0a                            0....
+000003b0: 202a 2e62 6174 2c20 2a2e 7a69 702c 202a   *.bat, *.zip, *
+000003c0: 2e78 6d6c 0d0a 0d0a 5b6f 7074 696f 6e73  .xml....[options
+000003d0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
+000003e0: 0a77 6865 7265 203d 2073 6f75 7263 650d  .where = source.
+000003f0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000400: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000410: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Dashboards.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Dashboards.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Notifications.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Notifications.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Supermetrics.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Supermetrics.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/artifacts/vSAN/Views.zip` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/artifacts/vSAN/Views.zip`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/encrypt-passwords.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/encrypt-passwords.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar
 # Date:   2023-04-01
-# Version: 1.1.0.1002
+# Version: 1.1.0.1003
 # ===================================================================================================================
 #
 # Description:
 # Script to encrypt passwords for SDDC Manager and vRealize Operations credentials. Passwords are encrypted and saved
 # in an encrypted_pwds file and a key file in encrypted_files directory.
 #
 # Example:
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/env.json` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/env.json`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/send-data-to-vrops.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/send-data-to-vrops.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 # ===================================================================================================================
 # Created by:  Bhumitra Nagar - Senior Member of Technical Staff
 # Authors: Bhumitra Nagar, Sowjanya V
 # Date:   2023-05-04
-# Version: 1.1.0.1002
+# Version: 1.1.0.1003
 # ===================================================================================================================
 #
 # Description:
 # The send-data-to-vrops.py script receives the operational health data as JSON from SOS utility and supporting
 # Powershell modules and then sends it to objects in vRealize Operations as custom metrics for use in dashboards
 # to monitor the platform's health.
 #
 # Change Log:
 # ---------------------------------------------------------------------------------------
 #    Version - Description
+# 1.1.0.1003 - docs: readme update and update version and dist files for release
 # 1.1.0.1002 - chore: code cleanup
 # 1.1.0.1001 - bug: [HRM] Date on Backups and Snapshot dashboard shown incorrectly #50
 # 1.1.0.1001 - artifacts_update: Updated views for backup and snapshots to address issue #50
 # 1.1.0.1001 - feat: [HRM] Remove SDDC Manager root password from Python module #38
 # 1.1.0.1000 - feat: [HRM] Update project structure to host module on PyPI
 # ---------------------------------------------------------------------------------------
 # 1.0.0.1002 - bug: [HRM] Exception while sending Backup status data to vROps #48
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/FolderUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/FolderUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/LogUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/LogUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/PSUtility.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/PSUtility.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/main/utils/SosRest.py` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/main/utils/SosRest.py`

 * *Files identical despite different names*

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-cloud-foundation-health-monitoring
-Version: 1.1.0.1002
+Version: 1.1.0.1003
 Summary: Python Module for VMware Cloud Foundation Health Monitoring in vRealize Operations
 Home-page: https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
 Author: Bhumitra Nagar
 Author-email: bnagar@vmware.com
 License: BSD-2-Clause
 Project-URL: Bug Tracker, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/issues
 Project-URL: repository, https://github.com/vmware-samples/validated-solutions-for-cloud-foundation/tree/main/hrm
@@ -61,15 +61,15 @@
 ### PowerShell Editions and Versions
 - PowerShell Core 7.2.0 or later
 - Microsoft Windows PowerShell 5.1
 
 
 ### PowerShell Modules
 
-- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.0.1
+- [PowerShell Module for VMware Cloud Foundation Reporting](https://github.com/vmware/powershell-module-for-vmware-cloud-foundation-reporting) 2.1.0
 
 
 
 ## Implementation 
 
 Follow the [Implementation of Health Reporting and Monitoring for VMware Cloud Foundation](https://docs.vmware.com/en/VMware-Cloud-Foundation/services/vcf-health-reporting-and-monitoring-v1/GUID-AD58BAF1-7DC9-4514-90B7-7E9FA2E9E5FA.html) from [Health Reporting and Monitoring for VMware Cloud Foundation](https://core.vmware.com/health-reporting-and-monitoring-vmware-cloud-foundation)
```

### Comparing `vmware-cloud-foundation-health-monitoring-1.1.0.1002/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt` & `vmware-cloud-foundation-health-monitoring-1.1.0.1003/source/vmware_cloud_foundation_health_monitoring.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.cfg
 source/artifacts/__init__.py
+source/artifacts/vSAN/Alert_Definitions.xml
 source/artifacts/vSAN/Dashboards.zip
 source/artifacts/vSAN/Notifications.json
 source/artifacts/vSAN/Supermetrics.json
 source/artifacts/vSAN/Views.zip
 source/artifacts/vSAN/__init__.py
 source/examples/__init__.py
 source/examples/run_send-data-to-vrops.bat
```

