# Comparing `tmp/cartography-0.8.0.tar.gz` & `tmp/cartography-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cartography-0.8.0.tar", last modified: Mon Aug  5 17:25:25 2019, max compression
+gzip compressed data, was "dist/cartography-0.9.0.tar", last modified: Mon Aug 19 22:00:36 2019, max compression
```

## Comparing `cartography-0.8.0.tar` & `cartography-0.9.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     4087 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      266 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography.egg-info/entry_points.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/
--rw-rw-r--   0 travis    (2000) travis    (2000)      800 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/intel/
--rw-rw-r--   0 travis    (2000) travis    (2000)      622 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/create_indexes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/dns.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/intel/gcp/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36591 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/gcp/compute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10522 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/gcp/crm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6271 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/gcp/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/intel/aws/
--rw-rw-r--   0 travis    (2000) travis    (2000)    36918 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/intel/aws/ec2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18590 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/intel/aws/iam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11252 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/aws/s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4305 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/aws/organizations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11158 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/aws/rds.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5604 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/aws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8037 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/aws/elasticsearch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3874 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/aws/dynamodb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8699 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/aws/route53.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/intel/crxcavator/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/intel/crxcavator/crxcavator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/intel/crxcavator/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/intel/analysis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/intel/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/data/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/data/jobs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/data/jobs/analysis/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2498 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3659 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2057 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/data/jobs/analysis/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/data/jobs/cleanup/
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      263 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      715 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      348 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_s3_details.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2120 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3098 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      587 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      685 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      620 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_account_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      957 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      296 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      346 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/data/jobs/cleanup/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      551 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/data/jobs/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2157 2019-08-05 17:23:33.000000 cartography-0.8.0/cartography/data/indexes.cypher
--rw-rw-r--   0 travis    (2000) travis    (2000)     8239 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      101 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/__main__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/graph/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/graph/job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/graph/context.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/graph/statement.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/graph/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-05 17:25:25.000000 cartography-0.8.0/cartography/driftdetect/
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/driftdetect/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1520 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/driftdetect/storage.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/driftdetect/reporter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2377 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/driftdetect/add_shortcut.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/driftdetect/serializers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9175 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/driftdetect/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/driftdetect/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5392 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/driftdetect/get_states.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/driftdetect/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/driftdetect/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-08-05 17:24:50.000000 cartography-0.8.0/cartography/driftdetect/shortcut.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      807 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/driftdetect/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4125 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/driftdetect/detect_deviations.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5796 2019-08-05 17:24:48.000000 cartography-0.8.0/cartography/sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-05 17:24:49.000000 cartography-0.8.0/cartography/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-05 17:25:25.000000 cartography-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    18556 2019-08-05 17:23:33.000000 cartography-0.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-08-05 17:25:25.000000 cartography-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2019-08-05 17:24:50.000000 cartography-0.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4155 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      266 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography.egg-info/entry_points.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      800 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      622 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/create_indexes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3710 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/dns.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/gcp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36591 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/gcp/compute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10522 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/gcp/crm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6271 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/gcp/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/aws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40016 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/aws/ec2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18590 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/intel/aws/iam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11252 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/s3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4305 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/aws/organizations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11158 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/rds.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5709 2019-08-19 22:00:00.000000 cartography-0.9.0/cartography/intel/aws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8037 2019-08-19 22:00:00.000000 cartography-0.9.0/cartography/intel/aws/elasticsearch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3874 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/dynamodb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8699 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/aws/route53.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/intel/crxcavator/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9294 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/intel/crxcavator/crxcavator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/crxcavator/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1417 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/intel/analysis.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/intel/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/analysis/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2498 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3659 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2057 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/analysis/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/data/jobs/cleanup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      263 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_principals_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_policy_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_key_pairs_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      715 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      329 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1551 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      348 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_s3_details.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2120 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3098 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1478 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1592 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      587 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1039 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      685 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      620 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      680 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      272 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      957 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      296 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_buckets_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_users_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      537 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      346 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/cleanup/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1988 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1790 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1059 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      551 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1096 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/data/jobs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2019-08-19 21:58:38.000000 cartography-0.9.0/cartography/data/indexes.cypher
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8239 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      101 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/__main__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/graph/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/graph/job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1230 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/graph/context.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2923 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/graph/statement.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/graph/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1667 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-08-19 22:00:36.000000 cartography-0.9.0/cartography/driftdetect/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      929 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1554 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/storage.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/reporter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2377 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/add_shortcut.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1028 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9175 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/driftdetect/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5400 2019-08-19 21:59:59.000000 cartography-0.9.0/cartography/driftdetect/get_states.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      371 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/shortcut.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      807 2019-08-19 21:59:57.000000 cartography-0.9.0/cartography/driftdetect/model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3994 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/driftdetect/detect_deviations.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5796 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-08-19 21:59:58.000000 cartography-0.9.0/cartography/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      790 2019-08-19 22:00:36.000000 cartography-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18556 2019-08-19 21:58:38.000000 cartography-0.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2019-08-19 22:00:36.000000 cartography-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2019-08-19 21:59:57.000000 cartography-0.9.0/setup.py
```

### Comparing `cartography-0.8.0/cartography.egg-info/PKG-INFO` & `cartography-0.9.0/cartography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cartography
-Version: 0.8.0
+Version: 0.9.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cartography-0.8.0/cartography.egg-info/SOURCES.txt` & `cartography-0.9.0/cartography.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 cartography/data/jobs/cleanup/__init__.py
 cartography/data/jobs/cleanup/aws_account_cleanup.json
 cartography/data/jobs/cleanup/aws_account_dns_cleanup.json
 cartography/data/jobs/cleanup/aws_dns_cleanup.json
 cartography/data/jobs/cleanup/aws_import_account_access_key_cleanup.json
 cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json
 cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json
+cartography/data/jobs/cleanup/aws_import_ec2_key_pairs_cleanup.json
 cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json
 cartography/data/jobs/cleanup/aws_import_es_cleanup.json
 cartography/data/jobs/cleanup/aws_import_groups_cleanup.json
 cartography/data/jobs/cleanup/aws_import_groups_membership_cleanup.json
 cartography/data/jobs/cleanup/aws_import_groups_policy_cleanup.json
 cartography/data/jobs/cleanup/aws_import_policies_cleanup.json
 cartography/data/jobs/cleanup/aws_import_principals_cleanup.json
```

### Comparing `cartography-0.8.0/cartography/util.py` & `cartography-0.9.0/cartography/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/create_indexes.py` & `cartography-0.9.0/cartography/intel/create_indexes.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/dns.py` & `cartography-0.9.0/cartography/intel/dns.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/gcp/compute.py` & `cartography-0.9.0/cartography/intel/gcp/compute.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/gcp/crm.py` & `cartography-0.9.0/cartography/intel/gcp/crm.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/gcp/__init__.py` & `cartography-0.9.0/cartography/intel/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/ec2.py` & `cartography-0.9.0/cartography/intel/aws/ec2.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,20 @@
     paginator = client.get_paginator('describe_security_groups')
     security_groups = []
     for page in paginator.paginate():
         security_groups.extend(page['SecurityGroups'])
     return {'SecurityGroups': security_groups}
 
 
+def get_ec2_key_pairs(session, region):
+    client = session.client('ec2', region_name=region, config=_get_botocore_config())
+    result = client.describe_key_pairs()
+    return result
+
+
 def get_ec2_instances(session, region):
     client = session.client('ec2', region_name=region, config=_get_botocore_config())
     paginator = client.get_paginator('describe_instances')
     reservations = []
     for page in paginator.paginate():
         reservations.extend(page['Reservations'])
     return {'Reservations': reservations}
@@ -68,14 +74,43 @@
 
 def get_ec2_vpcs(session, region):
     client = session.client('ec2', region_name=region, config=_get_botocore_config())
     # paginator not supported by boto
     return client.describe_vpcs()
 
 
+def load_ec2_key_pairs(session, data, region, current_aws_account_id, aws_update_tag):
+    ingest_key_pair = """
+    MERGE (keypair:KeyPair:EC2KeyPair{arn: {ARN}, id: {ARN}})
+    ON CREATE SET keypair.firstseen = timestamp()
+    SET keypair.keyname = {KeyName}, keypair.keyfingerprint = {KeyFingerprint}, keypair.region = {Region},
+    keypair.lastupdated = {aws_update_tag}
+    WITH keypair
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (aa)-[r:RESOURCE]->(keypair)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
+    for key_pair in data['KeyPairs']:
+        key_name = key_pair["KeyName"]
+        key_fingerprint = key_pair.get("KeyFingerprint")
+        key_pair_arn = f'arn:aws:ec2:{region}:{current_aws_account_id}:key-pair/{key_name}'
+
+        session.run(
+            ingest_key_pair,
+            ARN=key_pair_arn,
+            KeyName=key_name,
+            KeyFingerprint=key_fingerprint,
+            AWS_ACCOUNT_ID=current_aws_account_id,
+            Region=region,
+            aws_update_tag=aws_update_tag,
+        )
+
+
 def load_ec2_instances(session, data, region, current_aws_account_id, aws_update_tag):
     ingest_reservation = """
     MERGE (reservation:EC2Reservation{reservationid: {ReservationId}})
     ON CREATE SET reservation.firstseen = timestamp()
     SET reservation.ownerid = {OwnerId}, reservation.requesterid = {RequesterId}, reservation.region = {Region},
     reservation.lastupdated = {aws_update_tag}
     WITH reservation
@@ -107,14 +142,30 @@
     WITH instance
     MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
     MERGE (aa)-[r:RESOURCE]->(instance)
     ON CREATE SET r.firstseen = timestamp()
     SET r.lastupdated = {aws_update_tag}
     """
 
+    ingest_key_pair = """
+    MERGE (keypair:KeyPair:EC2KeyPair{arn: {KeyPairARN}, id: {KeyPairARN}})
+    ON CREATE SET keypair.firstseen = timestamp()
+    SET keypair.keyname = {KeyName}, keypair.region = {Region}, keypair.lastupdated = {aws_update_tag}
+    WITH keypair
+    MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
+    MERGE (aa)-[r:RESOURCE]->(keypair)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    with keypair
+    MATCH (instance:EC2Instance{instanceid: {InstanceId}})
+    MERGE (instance)<-[r:SSH_LOGIN_TO]-(keypair)
+    ON CREATE SET r.firstseen = timestamp()
+    SET r.lastupdated = {aws_update_tag}
+    """
+
     ingest_security_groups = """
     MERGE (group:EC2SecurityGroup{id: {GroupId}})
     ON CREATE SET group.firstseen = timestamp(), group.groupid = {GroupId}
     SET group.name = {GroupName}, group.region = {Region}, group.lastupdated = {aws_update_tag}
     WITH group
     MATCH (aa:AWSAccount{id: {AWS_ACCOUNT_ID}})
     MERGE (aa)-[r:RESOURCE]->(group)
@@ -169,14 +220,27 @@
                 LaunchTimeUnix=launch_time_unix,
                 State=instance_state,
                 AWS_ACCOUNT_ID=current_aws_account_id,
                 Region=region,
                 aws_update_tag=aws_update_tag,
             )
 
+            if instance.get("KeyName"):
+                key_name = instance["KeyName"]
+                key_pair_arn = f'arn:aws:ec2:{region}:{current_aws_account_id}:key-pair/{key_name}'
+                session.run(
+                    ingest_key_pair,
+                    KeyPairARN=key_pair_arn,
+                    KeyName=key_name,
+                    Region=region,
+                    InstanceId=instanceid,
+                    AWS_ACCOUNT_ID=current_aws_account_id,
+                    aws_update_tag=aws_update_tag,
+                )
+
             if instance.get("SecurityGroups"):
                 for group in instance["SecurityGroups"]:
                     session.run(
                         ingest_security_groups,
                         GroupId=group["GroupId"],
                         GroupName=group.get("GroupName", ""),
                         InstanceId=instanceid,
@@ -841,14 +905,18 @@
     run_cleanup_job(
         'aws_import_ec2_security_groupinfo_cleanup.json',
         session,
         common_job_parameters,
     )
 
 
+def cleanup_ec2_key_pairs(session, common_job_parameters):
+    run_cleanup_job('aws_import_ec2_key_pairs_cleanup.json', session, common_job_parameters)
+
+
 def cleanup_ec2_instances(session, common_job_parameters):
     run_cleanup_job('aws_import_ec2_instances_cleanup.json', session, common_job_parameters)
 
 
 def cleanup_ec2_auto_scaling_groups(session, common_job_parameters):
     run_cleanup_job(
         'aws_ingest_ec2_auto_scaling_groups_cleanup.json',
@@ -876,14 +944,22 @@
     for region in regions:
         logger.debug("Syncing EC2 security groups for region '%s' in account '%s'.", region, current_aws_account_id)
         data = get_ec2_security_group_data(boto3_session, region)
         load_ec2_security_groupinfo(session, data, region, current_aws_account_id, aws_update_tag)
     cleanup_ec2_security_groupinfo(session, common_job_parameters)
 
 
+def sync_ec2_key_pairs(session, boto3_session, regions, current_aws_account_id, aws_update_tag, common_job_parameters):
+    for region in regions:
+        logger.debug("Syncing EC2 key pairs for region '%s' in account '%s'.", region, current_aws_account_id)
+        data = get_ec2_key_pairs(boto3_session, region)
+        load_ec2_key_pairs(session, data, region, current_aws_account_id, aws_update_tag)
+    cleanup_ec2_key_pairs(session, common_job_parameters)
+
+
 def sync_ec2_instances(session, boto3_session, regions, current_aws_account_id, aws_update_tag, common_job_parameters):
     for region in regions:
         logger.debug("Syncing EC2 instances for region '%s' in account '%s'.", region, current_aws_account_id)
         data = get_ec2_instances(boto3_session, region)
         load_ec2_instances(session, data, region, current_aws_account_id, aws_update_tag)
     cleanup_ec2_instances(session, common_job_parameters)
```

### Comparing `cartography-0.8.0/cartography/intel/aws/iam.py` & `cartography-0.9.0/cartography/intel/aws/iam.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/s3.py` & `cartography-0.9.0/cartography/intel/aws/s3.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/organizations.py` & `cartography-0.9.0/cartography/intel/aws/organizations.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/rds.py` & `cartography-0.9.0/cartography/intel/aws/rds.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/__init__.py` & `cartography-0.9.0/cartography/intel/aws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     dynamodb.sync_dynamodb_tables(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
 
     # EC2
     # TODO move this to EC2 module
     logger.info("Syncing EC2 for account '%s'.", account_id)
     ec2.sync_vpc(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
     ec2.sync_ec2_security_groupinfo(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
+    ec2.sync_ec2_key_pairs(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
     ec2.sync_ec2_instances(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
     ec2.sync_ec2_auto_scaling_groups(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
     ec2.sync_load_balancers(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
     ec2.sync_vpc_peering(session, boto3_session, regions, sync_tag, account_id, common_job_parameters)
 
     # RDS
     rds.sync_rds_instances(session, boto3_session, regions, account_id, sync_tag, common_job_parameters)
```

### Comparing `cartography-0.8.0/cartography/intel/aws/elasticsearch.py` & `cartography-0.9.0/cartography/intel/aws/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/dynamodb.py` & `cartography-0.9.0/cartography/intel/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/aws/route53.py` & `cartography-0.9.0/cartography/intel/aws/route53.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/intel/crxcavator/crxcavator.py` & `cartography-0.9.0/cartography/intel/crxcavator/crxcavator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,50 +56,49 @@
     :return: List containing extension info for ingestion
     """
     # the JSON returned from the CRXcavator API does not return well formatted objects
     # instead, each object is named after it's key, making enumeration more difficult
     # will build a cleaner object for import into graph
 
     _data_index = 1
-    _row_index = 0
 
     extensions = []
     for extension in extension_json.items():
-        details = extension[_data_index][_row_index]
-        if not details:
-            logger.warning(f'Could not retrieve details for extension {extension}')
-            continue
-        extension_id = details['extension_id']
-        version = details['version']
-        data = details['data']
-        extensions.append({
-            'id': f"{extension_id}|{version}",
-            'extension_id': extension_id,
-            'version': version,
-            'risk_total': data['risk'].get('total'),
-            'risk_metadata': json.dumps(data['risk'].get('metadata')),
-            'address': data['webstore'].get('address'),
-            'email': data['webstore'].get('email'),
-            'icon': data['webstore'].get('icon'),
-            'crxcavator_last_updated': data['webstore'].get('last_updated'),
-            'name': data['webstore'].get('name'),
-            'offered_by': data['webstore'].get('offered_by'),
-            'permissions_warnings': data['webstore'].get('permission_warnings'),
-            'privacy_policy': data['webstore'].get('privacy_policy'),
-            'rating': data['webstore'].get('rating'),
-            'rating_users': data['webstore'].get('rating_users'),
-            'short_description': data['webstore'].get('short_description'),
-            'size': data['webstore'].get('size'),
-            'support_site': data['webstore'].get('support_site'),
-            'users': data['webstore'].get('users'),
-            'website': data['webstore'].get('website'),
-            'type': data['webstore'].get('type'),
-            'price': data['webstore'].get('price'),
-            'report_link': "https://crxcavator.io/report/" + extension_id + "/" + version,
-        })
+        for details in extension[_data_index]:
+            if not details:
+                logger.warning(f'Could not retrieve details for extension {extension}')
+                continue
+            extension_id = details['extension_id']
+            version = details['version']
+            data = details['data']
+            extensions.append({
+                'id': f"{extension_id}|{version}",
+                'extension_id': extension_id,
+                'version': version,
+                'risk_total': data['risk'].get('total'),
+                'risk_metadata': json.dumps(data['risk'].get('metadata')),
+                'address': data['webstore'].get('address'),
+                'email': data['webstore'].get('email'),
+                'icon': data['webstore'].get('icon'),
+                'crxcavator_last_updated': data['webstore'].get('last_updated'),
+                'name': data['webstore'].get('name'),
+                'offered_by': data['webstore'].get('offered_by'),
+                'permissions_warnings': data['webstore'].get('permission_warnings'),
+                'privacy_policy': data['webstore'].get('privacy_policy'),
+                'rating': data['webstore'].get('rating'),
+                'rating_users': data['webstore'].get('rating_users'),
+                'short_description': data['webstore'].get('short_description'),
+                'size': data['webstore'].get('size'),
+                'support_site': data['webstore'].get('support_site'),
+                'users': data['webstore'].get('users'),
+                'website': data['webstore'].get('website'),
+                'type': data['webstore'].get('type'),
+                'price': data['webstore'].get('price'),
+                'report_link': "https://crxcavator.io/report/" + extension_id + "/" + version,
+            })
     return extensions
 
 
 def load_extensions(extensions, session, update_tag):
     """
     Ingests the extension details into Neo4J
     :param extensions: List of extension data to load to Neo4J
```

### Comparing `cartography-0.8.0/cartography/intel/analysis.py` & `cartography-0.9.0/cartography/intel/analysis.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json` & `cartography-0.9.0/cartography/data/jobs/analysis/aws_s3acl_analysis.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json` & `cartography-0.9.0/cartography/data/jobs/analysis/gcp_compute_asset_inet_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json` & `cartography-0.9.0/cartography/data/jobs/analysis/aws_ec2_asset_exposure.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_roles_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_post_ingestion_dns_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/crxcavator_import_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_peering_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_firewall_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_instance_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_ec2_auto_scaling_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_security_groupinfo_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_ec2_instances_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_es_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_organization_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_rds_instances_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_dns_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_account_dns_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_dynamodb_tables_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_groups_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_policies_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_ingest_load_balancers_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_compute_vpc_subnet_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_project_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_s3_acl_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/gcp_crm_folder_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json` & `cartography-0.9.0/cartography/data/jobs/cleanup/aws_import_vpc_cleanup.json`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/data/indexes.cypher` & `cartography-0.9.0/cartography/data/indexes.cypher`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 CREATE INDEX ON :DNSZone(name);
 CREATE INDEX ON :DynamoDBTable(arn);
 CREATE INDEX ON :DynamoDBTable(id);
 CREATE INDEX ON :DynamoDBGlobalSecondaryIndex(id);
 CREATE INDEX ON :EC2Instance(instanceid);
 CREATE INDEX ON :EC2Instance(publicdnsname);
 CREATE INDEX ON :EC2Reservation(reservationid);
+CREATE INDEX ON :EC2KeyPair(id);
 CREATE INDEX ON :EC2SecurityGroup(id);
 CREATE INDEX ON :EC2SecurityGroup(groupid);
 CREATE INDEX ON :EC2Subnet(id);
 CREATE INDEX ON :EC2Subnet(subnetid);
 CREATE INDEX ON :ELBListener(id);
 CREATE INDEX ON :Endpoint(id);
 CREATE INDEX ON :ESDomain(arn);
```

### Comparing `cartography-0.8.0/cartography/cli.py` & `cartography-0.9.0/cartography/cli.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/graph/job.py` & `cartography-0.9.0/cartography/graph/job.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/graph/context.py` & `cartography-0.9.0/cartography/graph/context.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/graph/statement.py` & `cartography-0.9.0/cartography/graph/statement.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/config.py` & `cartography-0.9.0/cartography/config.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/util.py` & `cartography-0.9.0/cartography/driftdetect/util.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/storage.py` & `cartography-0.9.0/cartography/driftdetect/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         :param data: Dictionary in JSON format.
         :type file_path: string
         :param file_path: Filepath to be written to.
         :return:
         """
         with open(file_path, 'w') as json_file:
             json.dump(data, json_file, sort_keys=True, indent=4)
+            json_file.write('\n')
 
     @classmethod
     def walk(cls, drift_detection_directory):
         """
         Enables walking through drift detection.
         :type drift_detection_directory: String.
         :param drift_detection_directory: Path to drift detection directory.
```

### Comparing `cartography-0.8.0/cartography/driftdetect/add_shortcut.py` & `cartography-0.9.0/cartography/driftdetect/add_shortcut.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/serializers.py` & `cartography-0.9.0/cartography/driftdetect/serializers.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/cli.py` & `cartography-0.9.0/cartography/driftdetect/cli.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/get_states.py` & `cartography-0.9.0/cartography/driftdetect/get_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,14 @@
     state.properties = new_results.keys()
     results = []
 
     for record in new_results:
         values = []
         for field in record.values():
             if isinstance(field, list):
-                s = "|".join([str(i) for i in field])
+                s = "|".join(sorted([str(i) for i in field]))
                 values.append(s)
             else:
                 values.append(str(field))
         results.append(values)
 
     state.results = results
```

### Comparing `cartography-0.8.0/cartography/driftdetect/config.py` & `cartography-0.9.0/cartography/driftdetect/config.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/model.py` & `cartography-0.9.0/cartography/driftdetect/model.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/cartography/driftdetect/detect_deviations.py` & `cartography-0.9.0/cartography/driftdetect/detect_deviations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
 
 from marshmallow import ValidationError
 
-from cartography.driftdetect.reporter import report_drift_missing
-from cartography.driftdetect.reporter import report_drift_new
+from cartography.driftdetect.reporter import report_drift
 from cartography.driftdetect.serializers import ShortcutSchema
 from cartography.driftdetect.serializers import StateSchema
 from cartography.driftdetect.storage import FileSystem
 from cartography.driftdetect.util import valid_directory
 
 logger = logging.getLogger(__name__)
 
@@ -37,16 +36,15 @@
                     config.end_state,
                     config.end_state,
                 ),
             ),
         )
         end_state = state_serializer.load(end_state_data)
         new_results, missing_results = perform_drift_detection(start_state, end_state)
-        report_drift_new(new_results)
-        report_drift_missing(missing_results)
+        report_drift(new_results, missing_results, end_state.name, end_state.properties)
     except ValidationError as err:
         msg = "Unable to create DriftStates from files {},{} for \n{} in directory {}.".format(
             config.start_state,
             config.end_state,
             err.messages,
             config.query_directory,
         )
@@ -93,16 +91,16 @@
     :param end_state: The later state chronologically to be compared to.
     :return: list of tuples of differences between states in the form (dictionary, State object)
     """
     differences = []
     for result in end_state.results:
         if result in start_state.results:
             continue
-        drift_info = {}
-        for prop, field in zip(end_state.properties, result):
+        drift = []
+        for field in result:
             value = field.split("|")
             if len(value) > 1:
-                drift_info[prop] = value
+                drift.append(value)
             else:
-                drift_info[prop] = field
-        differences.append((drift_info, end_state))
+                drift.append(field)
+        differences.append(drift)
     return differences
```

### Comparing `cartography-0.8.0/cartography/sync.py` & `cartography-0.9.0/cartography/sync.py`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/PKG-INFO` & `cartography-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: cartography
-Version: 0.8.0
+Version: 0.9.0
 Summary: Explore assets and their relationships across your technical infrastructure.
 Home-page: https://www.github.com/lyft/cartography
 Maintainer: Lyft
 Maintainer-email: security@lyft.com
 License: apache2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cartography-0.8.0/README.md` & `cartography-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cartography-0.8.0/setup.py` & `cartography-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 
 
 setup(
     name='cartography',
     version=__version__,
     description='Explore assets and their relationships across your technical infrastructure.',
     url='https://www.github.com/lyft/cartography',
```

