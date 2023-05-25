# Comparing `tmp/OBP_security_pillar-0.0.1.tar.gz` & `tmp/OBP_security_pillar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_security_pillar-0.0.1.tar", last modified: Mon Dec 19 06:51:36 2022, max compression
+gzip compressed data, was "OBP_security_pillar-0.0.2.tar", last modified: Thu Jan  5 06:30:37 2023, max compression
```

## Comparing `OBP_security_pillar-0.0.1.tar` & `OBP_security_pillar-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,57 @@
-drwxrwxrwx   0        0        0        0 2022-12-19 06:51:36.733010 OBP_security_pillar-0.0.1/
-drwxrwxrwx   0        0        0        0 2022-12-19 06:51:36.605769 OBP_security_pillar-0.0.1/OBP_security_pillar/
--rw-rw-rw-   0        0        0      877 2022-12-19 06:47:30.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-19 06:51:36.688240 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/
--rw-rw-rw-   0        0        0      733 2022-12-19 06:30:51.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/__init__.py
--rw-rw-rw-   0        0        0     2042 2022-12-16 05:21:27.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
--rw-rw-rw-   0        0        0     1968 2022-12-19 06:05:04.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_instance_public_access_check.py
--rw-rw-rw-   0        0        0     2044 2022-12-19 06:07:05.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_snapshot_encrypted.py
--rw-rw-rw-   0        0        0     2467 2022-12-19 06:28:59.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
--rw-rw-rw-   0        0        0     1893 2022-12-19 06:30:51.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_storage_encrypted.py
-drwxrwxrwx   0        0        0        0 2022-12-19 06:51:36.718802 OBP_security_pillar-0.0.1/OBP_security_pillar/s3/
--rw-rw-rw-   0        0        0      550 2022-12-19 06:47:30.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/s3/__init__.py
--rw-rw-rw-   0        0        0     1308 2022-12-19 06:47:30.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
--rw-rw-rw-   0        0        0     1573 2022-12-19 06:41:51.000000 OBP_security_pillar-0.0.1/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
-drwxrwxrwx   0        0        0        0 2022-12-19 06:51:36.622346 OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/
--rw-rw-rw-   0        0        0      736 2022-12-19 06:51:36.000000 OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2022-12-19 06:51:36.000000 OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-19 06:51:36.000000 OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-12-19 06:51:36.000000 OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      736 2022-12-19 06:51:36.727064 OBP_security_pillar-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      403 2022-12-19 06:35:52.000000 OBP_security_pillar-0.0.1/README.md
--rw-rw-rw-   0        0        0      495 2022-12-19 06:36:31.000000 OBP_security_pillar-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-19 06:51:36.733010 OBP_security_pillar-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.646451 OBP_security_pillar-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.288893 OBP_security_pillar-0.0.2/OBP_security_pillar/
+-rw-rw-rw-   0        0        0     2200 2023-01-05 06:29:36.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.330595 OBP_security_pillar-0.0.2/OBP_security_pillar/auto_scaling/
+-rw-rw-rw-   0        0        0      473 2022-12-22 12:38:56.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/auto_scaling/__init__.py
+-rw-rw-rw-   0        0        0     2128 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/auto_scaling/launch_config_public_ip_disabled.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.357847 OBP_security_pillar-0.0.2/OBP_security_pillar/cloudtrail/
+-rw-rw-rw-   0        0        0      724 2022-12-28 09:39:38.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/cloudtrail/__init__.py
+-rw-rw-rw-   0        0        0     2447 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/cloudtrail/cloudtrail_cloudwatch_logs_enabled.py
+-rw-rw-rw-   0        0        0     3124 2022-12-23 11:44:28.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/cloudtrail/driver.py
+-rw-rw-rw-   0        0        0     1170 2022-12-23 07:00:41.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/compliance.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.374541 OBP_security_pillar-0.0.2/OBP_security_pillar/dynamodb/
+-rw-rw-rw-   0        0        0      493 2022-12-28 11:57:53.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0     2806 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/dynamodb/dynamodb_table_encrypted_kms.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.502678 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/
+-rw-rw-rw-   0        0        0     2147 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/Incoming_ssh_disabled.py
+-rw-rw-rw-   0        0        0     1697 2023-01-05 06:13:49.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ebs_snapshot_public_restorable_check.py
+-rw-rw-rw-   0        0        0     1427 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_ebs_encryption_by_default.py
+-rw-rw-rw-   0        0        0     2050 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_encrypted_volume.py
+-rw-rw-rw-   0        0        0     2291 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_imdsv2_check.py
+-rw-rw-rw-   0        0        0     3876 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_instance_managed_by_ssm.py
+-rw-rw-rw-   0        0        0     2145 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_instance_multiple_eni_check.py
+-rw-rw-rw-   0        0        0     2259 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_instance_profile_attached.py
+-rw-rw-rw-   0        0        0     1995 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/ec2_volume_inuse_check.py
+-rw-rw-rw-   0        0        0     2162 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/instance_in_vpc.py
+-rw-rw-rw-   0        0        0     2275 2023-01-05 06:12:12.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/ec2/vpc_flow_logs_enabled.py
+-rw-rw-rw-   0        0        0     2390 2023-01-04 10:47:02.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/elb_logging_enabled.py
+-rw-rw-rw-   0        0        0     2205 2023-01-04 11:19:43.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/elb_tls_https_listeners_only.py
+-rw-rw-rw-   0        0        0     1906 2023-01-04 10:53:57.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2324 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/lambda_inside_vpc.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.555866 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/
+-rw-rw-rw-   0        0        0      733 2022-12-19 06:30:51.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/__init__.py
+-rw-rw-rw-   0        0        0     2108 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py
+-rw-rw-rw-   0        0        0     2028 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_instance_public_access_check.py
+-rw-rw-rw-   0        0        0     2108 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py
+-rw-rw-rw-   0        0        0     2529 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py
+-rw-rw-rw-   0        0        0     1953 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_storage_encrypted.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.634599 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/
+-rw-rw-rw-   0        0        0     1296 2023-01-05 05:59:15.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/__init__.py
+-rw-rw-rw-   0        0        0     1372 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py
+-rw-rw-rw-   0        0        0     2098 2023-01-04 13:07:26.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_public_read_prohibited.py
+-rw-rw-rw-   0        0        0     2090 2023-01-04 13:08:29.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_public_write_prohibited.py
+-rw-rw-rw-   0        0        0     1331 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_server_side_encryption_enabled.py
+-rw-rw-rw-   0        0        0     2208 2023-01-04 10:45:18.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_ssl_requests_only.py
+-rw-rw-rw-   0        0        0     1634 2023-01-04 10:45:19.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py
+-rw-rw-rw-   0        0        0     1761 2023-01-04 10:45:19.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_default_encryption_kms.py
+-rw-rw-rw-   0        0        0     1761 2023-01-04 11:06:48.000000 OBP_security_pillar-0.0.2/OBP_security_pillar/security_hub_enabled.py
+drwxrwxrwx   0        0        0        0 2023-01-05 06:30:37.315133 OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-01-05 06:30:37.000000 OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2223 2023-01-05 06:30:37.000000 OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-05 06:30:37.000000 OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-01-05 06:30:37.000000 OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      797 2023-01-05 06:30:37.641996 OBP_security_pillar-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2022-12-19 07:07:51.000000 OBP_security_pillar-0.0.2/README.md
+-rw-rw-rw-   0        0        0      495 2023-01-05 06:29:36.000000 OBP_security_pillar-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-01-05 06:30:37.646451 OBP_security_pillar-0.0.2/setup.cfg
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/__init__.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_automatic_minor_version_upgrade_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "RDS instance automatic minor version upgrade enabled"
     description = "Checks if automatic minor version upgrade is enabled for RDS instances."
     resource_type = "RDS Instance"
+    risk_level = 'Medium'
+
+
 
     regions = self.session.get_available_regions('rds')
 
     for region in regions:
         try:
             client = self.session.client('rds', region_name=region)
             marker = ''
@@ -48,9 +51,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_instance_public_access_check.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/guard_duty_enabled.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-import logging
-import botocore
 from botocore.exceptions import ClientError
 
+import logging
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def rds_instance_public_access_check(self) -> dict:
+# check the compliance for guard duty enabled
+def guard_duty_enabled(self) -> dict:
     """
     :param self:
     :return:
     """
-    logger.info(" ---Inside rds :: rds_instance_public_access_check()")
+    logger.info(" ---Inside guard_duty :: guard_duty_enabled()")
 
     result = True
     failReason = ''
     offenders = []
-    compliance_type = "RDS instance public access check"
-    description = "Checks whether the Amazon Relational Database Service (RDS) instances are not publicly accessible"
-    resource_type = "RDS Instance"
+    compliance_type = "Guard Duty Enabled"
+    description = "Checks if Amazon GuardDuty is enabled in your AWS account and region"
+    resource_type = "Guard Duty"
+    risk_level = 'Medium'
 
-    regions = self.session.get_available_regions('rds')
+    regions = self.session.get_available_regions('guardduty')
 
     for region in regions:
         try:
-            client = self.session.client('rds', region_name=region)
+            client = self.session.client('guardduty', region_name=region)
+            detectors = []
             marker = ''
             while True:
                 if marker == '' or marker is None:
-                    response = client.describe_db_instances()
+                    response = client.list_detectors()
                 else:
-                    response = client.describe_db_instances(
-                        Marker=marker
+                    response = client.list_detectors(
+                        NextToken=marker
                     )
-
-                for instance in response['DBInstances']:
-                    if instance['PubliclyAccessible']:
-                        result = False
-                        failReason = "RDS instance is publicly accessible"
-                        offenders.append(instance['DBInstanceIdentifier'])
+                detectors.extend(response['DetectorIds'])
 
                 try:
-                    marker = response['Marker']
+                    marker = response['NextToken']
                     if marker == '':
                         break
                 except KeyError:
                     break
 
+            if len(detectors) <= 0:
+                result = False
+                failReason = "Guard duty is not enabled"
+
         except ClientError as e:
             logger.error("Something went wrong with the region {}: {}".format(region, e))
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
-    }
+        'Description': description,
+        'Risk Level': risk_level
+    }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_snapshot_encrypted.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_snapshot_encrypted.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "RDS snapshot encrypted"
     description = "Checks whether Amazon Relational Database Service (Amazon RDS) DB snapshots are encrypted"
     resource_type = "RDS"
+    risk_level = 'Medium'
 
     regions = self.session.get_available_regions('rds')
 
     for region in regions:
         try:
             client = self.session.client('rds', region_name=region)
             marker = ''
@@ -31,15 +32,15 @@
                 if marker == '' or marker is None:
                     response = client.describe_db_snapshots()
                 else:
                     response = client.describe_db_snapshots(
                         Marker=marker
                     )
                 for snapshot in response['DBSnapshots']:
-                    print(snapshot['DBSnapshotIdentifier'])
+                    # print(snapshot['DBSnapshotIdentifier'])
                     encryption = snapshot['Encrypted']
                     if not encryption:
                         result = False
                         failReason = 'DB snapshot is not encrypted'
                         offenders.append(snapshot['DBSnapshotIdentifier'])
 
                 try:
@@ -53,9 +54,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_snapshots_public_prohibited.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "RDS snapshot public prohibited"
     description = "Checks if Amazon Relational Database Service (Amazon RDS) snapshots are public"
     resource_type = "RDS"
+    risk_level = 'High'
+
 
     regions = self.session.get_available_regions('rds')
 
     for region in regions:
         try:
             client = self.session.client('rds', region_name=region)
             marker = ''
@@ -57,9 +59,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/rds/rds_storage_encrypted.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/rds/rds_storage_encrypted.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "RDS Storage Encrypted"
     description = "Checks whether storage encryption is enabled for your RDS DB instances"
     resource_type = "RDS"
+    risk_level = 'High'
 
     regions = self.session.get_available_regions('rds')
 
     for region in regions:
         try:
             client = self.session.client('rds', region_name=region)
             marker = ''
@@ -48,9 +49,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/s3/s3_bucket_logging_enabled.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_logging_enabled.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "S3 bucket logging enabled"
     description = "Checks whether logging is enabled for your S3 buckets"
     resource_type = "S3 Buckets"
+    risk_level = 'Medium'
+
 
     client = self.session.client('s3')
     response = client.list_buckets()
 
     for bucket in response['Buckets']:
         bucket_name = bucket['Name']
 
@@ -40,9 +42,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py` & `OBP_security_pillar-0.0.2/OBP_security_pillar/s3/s3_bucket_versioning_enabled.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
     result = True
     failReason = ''
     offenders = []
     compliance_type = "S3 bucket versioning enabled"
     description = "Checks if bucket versioning is enabled in s3 buckets."
     resource_type = "S3 Buckets"
+    risk_level = 'Low'
+
 
     client = self.session.client('s3')
     response = client.list_buckets()
 
     for bucket in response['Buckets']:
         bucket_name = bucket['Name']
 
@@ -44,9 +46,10 @@
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
-        'Description': description
+        'Description': description,
+        'Risk Level': risk_level
     }
```

### Comparing `OBP_security_pillar-0.0.1/OBP_security_pillar.egg-info/PKG-INFO` & `OBP_security_pillar-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP-security-pillar
-Version: 0.0.1
+Name: OBP_security_pillar
+Version: 0.0.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -16,7 +16,9 @@
 # v0.0.1
 1. Added following compliance checks:
    - RdsAutomaticMinorVersionUpgradeEnabled
    - RdsInstancePublicAccessCheck
    - RdsSnapshotEncrypted
    - RdsSnapshotsPublicProhibited
    - RdsStorageEncrypted
+   - S3BucketLoggingEnabled
+   - S3BucketVersioningEnabled
```

### Comparing `OBP_security_pillar-0.0.1/PKG-INFO` & `OBP_security_pillar-0.0.2/OBP_security_pillar.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: OBP_security_pillar
-Version: 0.0.1
+Name: OBP-security-pillar
+Version: 0.0.2
 Summary: Provides AWS compliance details
 Author-email: "dheeraj.banodha" <dheerajmbanodha@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
@@ -16,7 +16,9 @@
 # v0.0.1
 1. Added following compliance checks:
    - RdsAutomaticMinorVersionUpgradeEnabled
    - RdsInstancePublicAccessCheck
    - RdsSnapshotEncrypted
    - RdsSnapshotsPublicProhibited
    - RdsStorageEncrypted
+   - S3BucketLoggingEnabled
+   - S3BucketVersioningEnabled
```

