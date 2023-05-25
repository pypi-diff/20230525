# Comparing `tmp/slurmrestapi-1.0.0.tar.gz` & `tmp/slurmrestapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmrestapi-1.0.0.tar", last modified: Thu May 25 05:37:38 2023, max compression
+gzip compressed data, was "slurmrestapi-1.0.1.tar", last modified: Thu May 25 05:49:31 2023, max compression
```

## Comparing `slurmrestapi-1.0.0.tar` & `slurmrestapi-1.0.1.tar`

### file list

```diff
@@ -1,1277 +1,1277 @@
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/
--rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/PKG-INFO
--rw-r--r--   0 keyemyria   (501) staff       (20)    45550 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/README.md
--rw-r--r--   0 keyemyria   (501) staff       (20)       69 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/setup.cfg
--rw-r--r--   0 keyemyria   (501) staff       (20)     1142 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/setup.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)      737 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    58494 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/api_client.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/apis/
--rw-r--r--   0 keyemyria   (501) staff       (20)      214 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/apis/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    19792 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/path_to_api.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)      239 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)       97 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/openapi.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/openapi_json.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      102 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/openapi_v3.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/openapi_yaml.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_job_submit.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      133 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_node_node_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_partition_partition_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_partitions.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_reservation_reservation_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_37_reservations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_job_submit.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      133 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_node_node_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_partition_partition_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_partitions.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_reservation_reservation_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_38_reservations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_job_submit.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_node_node_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_partition_partition_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_partitions.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_reservation_reservation_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurm_v0_0_39_reservations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_account_account_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_accounts.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      227 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_cluster_cluster_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_clusters.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_qos_qos_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_user_user_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_wckey_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_37_wckeys.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_account_account_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_accounts.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_cluster_cluster_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_clusters.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_qos_qos_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_user_user_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_wckey_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_38_wckeys.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_account_account_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_accounts.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_cluster_cluster_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_clusters.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_job_job_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_jobs.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos_qos_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_user_user_name.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckey_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckeys.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      440 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/tag_to_api.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/apis/tags/
--rw-r--r--   0 keyemyria   (501) staff       (20)      329 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/apis/tags/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      725 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/apis/tags/openapi_api.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15541 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/slurmrestapi/apis/tags/slurm_api.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    16953 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/configuration.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4516 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/exceptions.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/model/
--rw-r--r--   0 keyemyria   (501) staff       (20)      346 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8091 2023-05-25 03:58:36.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4842 2023-05-25 03:58:37.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3365 2023-05-25 03:58:37.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    66470 2023-05-25 03:58:38.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3990 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_association_short_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4936 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13330 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_cluster_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12098 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3363 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_config_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2922 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_coordinator_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    38459 2023-05-25 03:58:40.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2902 2023-05-25 03:58:40.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    77631 2023-05-25 03:58:41.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6431 2023-05-25 03:58:42.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4750 2023-05-25 03:58:42.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    71159 2023-05-25 03:58:42.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    86189 2023-05-25 03:58:43.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4736 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3377 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_account_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3385 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_association_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3375 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_cluster_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3377 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_cluster_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3369 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_qos_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3359 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_user_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_user_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3367 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_wckey_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3373 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_wckey_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4788 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5085 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11167 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4773 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6481 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4796 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8091 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5426 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3949 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4065 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    58207 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3990 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_association_short_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5520 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13330 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_cluster_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2602 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_clusters_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12682 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3947 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_config_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2922 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_coordinator_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    39043 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4068 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1403 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    78159 2023-05-25 03:58:49.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6431 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5334 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    68817 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12957 2023-05-25 03:58:51.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    87986 2023-05-25 03:58:51.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5320 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_account_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3959 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5477 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_cluster_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_cluster_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3941 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3953 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_qos_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3943 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_user_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_user_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3951 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_wckey_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3957 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_wckey_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12259 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4548 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5085 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2525 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3403 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3297 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3336 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11013 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5357 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6678 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5380 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4428 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4464 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4452 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_clusters_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8210 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4541 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4068 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1403 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4352 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13008 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4342 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5304 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7178 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4361 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2511 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2492 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2523 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4371 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3498 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1423 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3738 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3621 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/status.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    35555 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2898 2023-05-25 03:58:56.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    47384 2023-05-25 03:58:56.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5288 2023-05-25 03:58:56.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_resources.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    67909 2023-05-25 03:58:57.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_response_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4597 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5073 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4856 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    28420 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4001 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_node_allocation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4751 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    20676 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_partition.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4866 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4449 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4735 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15343 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_reservation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4912 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2470 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0037_signal.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    41678 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4704 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag_rpcm.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4600 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag_rpcu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2989 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    49048 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5288 2023-05-25 03:59:02.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_resources.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    69047 2023-05-25 03:59:02.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_response_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4597 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5643 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5426 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5027 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4804 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12953 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    28420 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6261 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_node_allocation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5321 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    22153 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_partition.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5436 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4449 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5305 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15343 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_reservation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5482 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2470 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0038_signal.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6827 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1391 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_account_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6306 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1418 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_accounting_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5882 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_acct_gather_energy.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      606 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_acct_gather_energy_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    24341 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3999 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1419 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9797 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_usage.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_usage_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13473 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_cluster_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1419 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_cluster_rec_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3967 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_controller_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1457 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_controller_ping_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2916 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_coord.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_coord_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11118 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_cron_entry.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_cron_entry_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1285 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_csv_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4367 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4064 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4633 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_ext_sensors_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_ext_sensors_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3490 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_float64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1287 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_hostlist.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_hostlist_string.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    48237 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5220 2023-05-25 03:59:09.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_array_response_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      609 2023-05-25 03:59:09.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_array_response_msg_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)   104046 2023-05-25 03:59:10.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_argv.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1420 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      605 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_spank_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2058 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_exclusive.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6453 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)   103642 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1305 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info_gres_detail.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1390 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1355 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_mem_per_cpu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_mem_per_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5033 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1615 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3794 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5456 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4442 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_update_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4338 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6802 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4362 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_licenses_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13004 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    49232 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4313 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    36226 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_partition_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1448 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_partition_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4466 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4397 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7428 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_power_mgmt_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_power_mgmt_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    26386 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1355 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_preempt_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1324 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_string_id_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     2883 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    24067 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1466 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1501 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4504 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     7463 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_rollup_stats.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_rollup_stats_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3649 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_slurm_step_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    32117 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6050 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5938 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4403 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rec_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5629 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rpc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1401 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rpc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     5644 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1410 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    32492 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1376 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_req_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1376 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_req_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1380 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_usage_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1380 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_usage_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_string_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3869 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres_str.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint16_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint32_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17978 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_update_node_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12443 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     3494 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1405 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6396 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     4263 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey_tag.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/models/
--rw-r--r--   0 keyemyria   (501) staff       (20)    17875 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/models/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)     5762 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)      297 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6893 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_json/
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_json/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6952 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_json/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_v3/
--rw-r--r--   0 keyemyria   (501) staff       (20)      303 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_v3/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6928 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_v3/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_yaml/
--rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_yaml/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     6952 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/slurmrestapi/paths/openapi_yaml/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8684 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10620 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10721 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    14449 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15011 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_submit/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10950 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10758 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_node_node_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10966 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_nodes/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13062 2023-05-25 03:59:25.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11046 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partitions/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8682 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_ping/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13108 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11078 2023-05-25 03:59:26.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservations/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9193 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10641 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10742 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    14478 2023-05-25 03:59:22.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15528 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_submit/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11457 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8936 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_licenses/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11267 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_node_node_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11473 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_nodes/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13569 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11553 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partitions/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9191 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_ping/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13615 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11585 2023-05-25 03:59:21.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservations/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9172 2023-05-25 03:59:22.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15008 2023-05-25 03:59:22.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10742 2023-05-25 03:59:22.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17843 2023-05-25 03:59:24.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15507 2023-05-25 03:59:24.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11436 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8953 2023-05-25 03:59:24.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11200 2023-05-25 03:59:22.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11246 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17797 2023-05-25 03:59:24.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11452 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13548 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11532 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9170 2023-05-25 03:59:24.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_ping/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13594 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11564 2023-05-25 03:59:23.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10894 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10804 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8798 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11910 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11786 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8866 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8922 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10894 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10804 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8798 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8829 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8822 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8844 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8689 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10716 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17426 2023-05-25 03:59:41.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8723 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10802 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10788 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8739 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8794 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10825 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10735 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8750 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10816 2023-05-25 03:59:40.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10726 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8766 2023-05-25 03:59:42.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8797 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11444 2023-05-25 03:59:27.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13531 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11525 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15622 2023-05-25 03:59:32.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12426 2023-05-25 03:59:27.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12336 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12438 2023-05-25 03:59:27.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12347 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15741 2023-05-25 03:59:32.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11444 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11354 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9348 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15632 2023-05-25 03:59:27.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9340 2023-05-25 03:59:29.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15965 2023-05-25 03:59:32.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9239 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11248 2023-05-25 03:59:30.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    17976 2023-05-25 03:59:30.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11450 2023-05-25 03:59:30.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15519 2023-05-25 03:59:33.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11352 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13515 2023-05-25 03:59:31.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8793 2023-05-25 03:59:31.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15545 2023-05-25 03:59:33.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11375 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13462 2023-05-25 03:59:31.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11477 2023-05-25 03:59:31.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15589 2023-05-25 03:59:33.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11366 2023-05-25 03:59:28.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11276 2023-05-25 03:59:31.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9316 2023-05-25 03:59:32.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15950 2023-05-25 03:59:27.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11279 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13815 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11809 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15485 2023-05-25 03:59:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12397 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12307 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12409 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    12318 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15581 2023-05-25 03:59:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11279 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11329 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9323 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15443 2023-05-25 03:59:33.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9311 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15829 2023-05-25 03:59:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9210 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11219 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    18824 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11734 2023-05-25 03:59:36.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15395 2023-05-25 03:59:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11203 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13799 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     8793 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15417 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11222 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    13746 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11761 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15436 2023-05-25 03:59:39.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11209 2023-05-25 03:59:35.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    11247 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)     9287 2023-05-25 03:59:37.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    15805 2023-05-25 03:59:34.000000 slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    10667 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/rest.py
--rw-r--r--   0 keyemyria   (501) staff       (20)    97648 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/slurmrestapi/schemas.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/
--rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/PKG-INFO
--rw-r--r--   0 keyemyria   (501) staff       (20)    53810 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/SOURCES.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)        1 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/dependency_links.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)      118 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/requires.txt
--rw-r--r--   0 keyemyria   (501) staff       (20)       18 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/slurmrestapi.egg-info/top_level.txt
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_models/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:47.000000 slurmrestapi-1.0.0/test/test_models/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:37.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:37.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:37.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_account_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-25 03:58:38.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      612 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_association_short_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_cluster_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-25 03:58:39.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_config_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:40.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_coordinator_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:40.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:40.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:41.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:58:42.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:42.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:43.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_account_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      632 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_association_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_cluster_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_cluster_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:58:44.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_qos_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_user_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_user_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_wckey_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_wckey_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:45.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0037_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_account_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-25 03:58:46.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_association.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      612 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_association_short_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_cluster_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:58:47.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_clusters_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_config_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_coordinator_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:58:48.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:49.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:50.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:51.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:51.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_account_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_associations.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      636 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_cluster_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_cluster_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_qos_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_user_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_user_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_wckey_add.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_wckey_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:53.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0038_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_account_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_associations_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_clusters_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_config_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:54.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_qos_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      636 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_response_associations_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_set_config.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_tres_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_tres_update.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_update_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_update_users.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_user_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_dbv0039_wckey_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      525 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_status.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:55.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:56.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:56.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_job_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:57.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_job_resources.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:57.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_job_response_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:58.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_node_allocation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_partition.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:59.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_reservation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0037_signal.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_diag_rpcm.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:00.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_diag_rpcu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:01.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_job_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:02.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_job_resources.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:02.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_job_response_properties.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:03.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_node_allocation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:59:04.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_partition.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_reservation.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0038_signal.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_account.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_account_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_accounting.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:05.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_accounting_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_acct_gather_energy.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_acct_gather_energy_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_usage.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_usage_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_cluster_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_cluster_rec_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_controller_ping.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_controller_ping_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_coord.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_coord_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_cron_entry.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_cron_entry_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:07.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_csv_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_diag.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_error.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_errors.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_ext_sensors_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_ext_sensors_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_float64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_hostlist.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:08.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_hostlist_string.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      534 2023-05-25 03:59:09.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:09.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_array_response_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      614 2023-05-25 03:59:09.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_array_response_msg_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      564 2023-05-25 03:59:10.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_argv.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_spank_env.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_exclusive.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:11.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_exit_code.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_info_gres_detail.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      564 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_info_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_mem_per_cpu.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-25 03:59:12.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_mem_per_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      547 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_res.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_res_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      560 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_res_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_submission.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_submission_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_job_update_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_jobs_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_license.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_licenses.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_licenses_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:13.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_meta.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_node.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_nodes_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_partition_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_partition_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:59:14.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_partitions_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_pings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_power_mgmt_data.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_power_mgmt_data_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      534 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_qos.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_qos_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_qos_preempt_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      585 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_qos_string_id_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      617 2023-05-25 03:59:15.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info_core_spec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_reservations_response.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_rollup_stats.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_rollup_stats_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_slurm_step_id.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg_rpcs_by_type.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:16.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg_rpcs_by_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rec.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rec_ptr.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rpc.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rpc_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_stats_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_nodes.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_req_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_req_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:17.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_usage_max.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_usage_min.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_string_array.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_tres.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_tres_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_tres_str.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_uint16_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_uint32_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_uint64_no_val.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_update_node_msg.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_user.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_user_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_warning.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_warnings.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:18.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_wckey.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_wckey_list.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:19.000000 slurmrestapi-1.0.0/test/test_models/test_v0039_wckey_tag.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/
--rw-r--r--   0 keyemyria   (501) staff       (20)     1995 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/__init__.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      826 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_json/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_json/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_json/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_v3/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_v3/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_v3/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_yaml/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_yaml/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:20.000000 slurmrestapi-1.0.0/test/test_paths/test_openapi_yaml/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      864 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_submit/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_node_node_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_nodes/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partition_partition_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partitions/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_ping/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservations/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      864 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_submit/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_licenses/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_node_node_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_nodes/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partition_partition_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partitions/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_ping/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservations/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      845 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_submit/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_submit/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_licenses/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_licenses/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      857 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_nodes/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_nodes/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partition_partition_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partition_partition_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partitions/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partitions/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_ping/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_ping/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_ping/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:43.000000 slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      838 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      835 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_job_job_id/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      825 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_job_job_id/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_diag/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_diag/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_job_job_id/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_job_job_id/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_jobs/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_jobs/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py
-drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:37:38.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/
--rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/__init__.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py
--rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/PKG-INFO
+-rw-r--r--   0 keyemyria   (501) staff       (20)    54556 2023-05-25 05:41:36.000000 slurmrestapi-1.0.1/README.md
+-rw-r--r--   0 keyemyria   (501) staff       (20)       69 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/setup.cfg
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1142 2023-05-25 05:49:03.000000 slurmrestapi-1.0.1/setup.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      737 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    58494 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/api_client.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi/apis/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      214 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/apis/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    19792 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/path_to_api.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      239 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)       97 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/openapi.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/openapi_json.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      102 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/openapi_v3.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      106 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/openapi_yaml.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_job_submit.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      133 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_node_node_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_partition_partition_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_partitions.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_reservation_reservation_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_37_reservations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_job_submit.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      133 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_node_node_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_partition_partition_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_partitions.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_reservation_reservation_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_38_reservations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_job_submit.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      123 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_node_node_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      153 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_partition_partition_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      127 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_partitions.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      115 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      161 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_reservation_reservation_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      131 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurm_v0_0_39_reservations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_account_account_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_accounts.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      227 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_cluster_cluster_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_clusters.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      117 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_qos_qos_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_user_user_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_wckey_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_37_wckeys.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_account_account_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_accounts.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_cluster_cluster_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_clusters.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_qos_qos_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_user_user_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_wckey_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_38_wckeys.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_account_account_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_accounts.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      230 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      255 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_cluster_cluster_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      215 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_clusters.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      129 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_job_job_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      119 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_jobs.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      200 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      231 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_qos_qos_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      203 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      237 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_user_user_name.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      206 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      229 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckey_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      209 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/paths/slurmdb_v0_0_39_wckeys.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      440 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/tag_to_api.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi/apis/tags/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      329 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/apis/tags/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      725 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/apis/tags/openapi_api.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15541 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/slurmrestapi/apis/tags/slurm_api.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    16953 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/configuration.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4516 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/exceptions.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/model/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      346 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8091 2023-05-25 03:58:36.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4842 2023-05-25 03:58:37.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3365 2023-05-25 03:58:37.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    66470 2023-05-25 03:58:38.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3990 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_association_short_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4936 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13330 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_cluster_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12098 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3363 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_config_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2922 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_coordinator_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    38459 2023-05-25 03:58:40.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2902 2023-05-25 03:58:40.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    77631 2023-05-25 03:58:41.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6431 2023-05-25 03:58:42.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4750 2023-05-25 03:58:42.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    71159 2023-05-25 03:58:42.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    86189 2023-05-25 03:58:43.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4736 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3377 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_account_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3385 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_association_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3375 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_cluster_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3377 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_cluster_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3369 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_qos_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3359 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_user_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3371 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_user_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3367 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_wckey_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3373 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_wckey_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4788 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5085 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11167 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4773 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6481 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4796 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8091 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5426 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3949 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4065 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    58207 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3990 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_association_short_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5520 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13330 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_cluster_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2602 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_clusters_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12682 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3947 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_config_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2922 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_coordinator_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    39043 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4068 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1403 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    78159 2023-05-25 03:58:49.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6431 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5334 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    68817 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12957 2023-05-25 03:58:51.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    87986 2023-05-25 03:58:51.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5320 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_account_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3959 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5477 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_cluster_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3961 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_cluster_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3941 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3953 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_qos_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3943 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_user_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3955 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_user_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3951 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_wckey_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3957 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_wckey_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12259 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4548 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5085 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2525 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3403 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3297 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3336 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11013 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5357 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6678 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5380 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4428 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4464 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4452 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_clusters_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8210 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4541 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4068 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1403 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4352 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13008 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4342 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5304 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7178 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4361 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2511 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2492 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2523 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4371 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3498 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1423 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3738 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3621 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/status.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    35555 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2898 2023-05-25 03:58:56.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    47384 2023-05-25 03:58:56.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5288 2023-05-25 03:58:56.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_resources.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    67909 2023-05-25 03:58:57.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_response_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4597 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5073 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4856 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    28420 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4001 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_node_allocation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4751 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    20676 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_partition.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4866 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4449 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4735 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15343 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_reservation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4912 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2470 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0037_signal.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    41678 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4704 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag_rpcm.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4600 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag_rpcu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2989 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    49048 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5288 2023-05-25 03:59:02.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_resources.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    69047 2023-05-25 03:59:02.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_response_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4597 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5643 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5426 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5027 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4804 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12953 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    28420 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6261 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_node_allocation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5321 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    22153 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_partition.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5436 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4449 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5305 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15343 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_reservation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5482 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2470 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0038_signal.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6827 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1391 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_account_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6306 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1418 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_accounting_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5882 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_acct_gather_energy.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      606 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_acct_gather_energy_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    24341 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3999 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1419 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9797 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_usage.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_usage_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13473 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_cluster_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1419 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_cluster_rec_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3967 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_controller_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1457 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_controller_ping_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2916 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_coord.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_coord_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11118 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_cron_entry.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_cron_entry_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1285 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_csv_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4367 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4064 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4633 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_ext_sensors_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_ext_sensors_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3490 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_float64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1287 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_hostlist.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_hostlist_string.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    48237 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5220 2023-05-25 03:59:09.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_array_response_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      609 2023-05-25 03:59:09.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_array_response_msg_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)   104046 2023-05-25 03:59:10.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_argv.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1420 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      605 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_spank_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2058 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_exclusive.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6453 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)   103642 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1305 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info_gres_detail.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1390 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1355 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      599 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_mem_per_cpu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_mem_per_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5033 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1615 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3794 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5456 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4442 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_update_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4338 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6802 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1385 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4362 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_licenses_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13004 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    49232 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1358 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4313 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    36226 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_partition_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1448 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_partition_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4466 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4397 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7428 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_power_mgmt_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_power_mgmt_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    26386 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1355 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1299 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_preempt_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1324 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_string_id_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     2883 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    24067 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1466 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1501 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4504 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     7463 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_rollup_stats.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_rollup_stats_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3649 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_slurm_step_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    32117 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6050 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5938 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4403 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rec_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5629 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rpc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1401 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rpc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5644 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1410 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    32492 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1376 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_req_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1376 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_req_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1380 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_usage_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1380 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_usage_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1293 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_string_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3869 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      594 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres_str.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint16_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint32_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3465 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17978 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_update_node_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12443 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1364 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     3494 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1405 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6396 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1373 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     4263 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey_tag.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/models/
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17875 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/models/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)     5762 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      297 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6893 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_json/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_json/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6952 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_json/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_v3/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      303 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_v3/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6928 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_v3/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_yaml/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      307 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_yaml/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     6952 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/slurmrestapi/paths/openapi_yaml/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8684 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10620 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10721 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    14449 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15011 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_submit/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10950 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10758 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_node_node_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10966 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_nodes/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13062 2023-05-25 03:59:25.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11046 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partitions/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8682 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_ping/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13108 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11078 2023-05-25 03:59:26.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservations/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9193 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10641 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10742 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    14478 2023-05-25 03:59:22.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15528 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_submit/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11457 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8936 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_licenses/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11267 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_node_node_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11473 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_nodes/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13569 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11553 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partitions/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9191 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_ping/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13615 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11585 2023-05-25 03:59:21.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservations/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9172 2023-05-25 03:59:22.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15008 2023-05-25 03:59:22.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10742 2023-05-25 03:59:22.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17843 2023-05-25 03:59:24.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15507 2023-05-25 03:59:24.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11436 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8953 2023-05-25 03:59:24.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11200 2023-05-25 03:59:22.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11246 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17797 2023-05-25 03:59:24.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11452 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      359 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13548 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11532 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      319 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9170 2023-05-25 03:59:24.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_ping/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      367 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13594 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11564 2023-05-25 03:59:23.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10894 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10804 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8798 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11910 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11786 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8866 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8922 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10894 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10804 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8798 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8829 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8822 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8844 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8689 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10716 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17426 2023-05-25 03:59:41.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8723 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10802 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10788 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8739 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8794 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10825 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10735 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8750 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10816 2023-05-25 03:59:40.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10726 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8766 2023-05-25 03:59:42.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8797 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11444 2023-05-25 03:59:27.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13531 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11525 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15622 2023-05-25 03:59:32.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12426 2023-05-25 03:59:27.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12336 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12438 2023-05-25 03:59:27.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12347 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15741 2023-05-25 03:59:32.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11444 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11354 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9348 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15632 2023-05-25 03:59:27.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9340 2023-05-25 03:59:29.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15965 2023-05-25 03:59:32.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9239 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11248 2023-05-25 03:59:30.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    17976 2023-05-25 03:59:30.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11450 2023-05-25 03:59:30.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15519 2023-05-25 03:59:33.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11352 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13515 2023-05-25 03:59:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8793 2023-05-25 03:59:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15545 2023-05-25 03:59:33.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11375 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13462 2023-05-25 03:59:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11477 2023-05-25 03:59:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15589 2023-05-25 03:59:33.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11366 2023-05-25 03:59:28.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11276 2023-05-25 03:59:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9316 2023-05-25 03:59:32.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15950 2023-05-25 03:59:27.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11279 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13815 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11809 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15485 2023-05-25 03:59:38.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12397 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12307 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12409 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    12318 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15581 2023-05-25 03:59:38.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      355 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11279 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11329 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      331 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9323 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15443 2023-05-25 03:59:33.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9311 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15829 2023-05-25 03:59:38.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9210 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      335 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11219 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    18824 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      321 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11734 2023-05-25 03:59:36.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15395 2023-05-25 03:59:38.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      339 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11203 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13799 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      323 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     8793 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15417 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      343 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11222 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    13746 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      325 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11761 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15436 2023-05-25 03:59:39.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      337 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11209 2023-05-25 03:59:35.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    11247 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      327 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)     9287 2023-05-25 03:59:37.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    15805 2023-05-25 03:59:34.000000 slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    10667 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/rest.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)    97648 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/slurmrestapi/schemas.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/
+-rw-r--r--   0 keyemyria   (501) staff       (20)      298 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/PKG-INFO
+-rw-r--r--   0 keyemyria   (501) staff       (20)    53810 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)        1 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)      118 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/requires.txt
+-rw-r--r--   0 keyemyria   (501) staff       (20)       18 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/slurmrestapi.egg-info/top_level.txt
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:30.000000 slurmrestapi-1.0.1/test/
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_models/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:47.000000 slurmrestapi-1.0.1/test/test_models/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:37.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:37.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:37.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_account_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-25 03:58:38.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      612 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_association_short_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_cluster_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-25 03:58:39.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_config_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:40.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_coordinator_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:40.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:40.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:41.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:58:42.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:42.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:43.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_account_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      632 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_association_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_cluster_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_cluster_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:58:44.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_qos_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_user_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_user_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_wckey_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_wckey_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:45.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0037_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_account_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      570 2023-05-25 03:58:46.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      574 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_association.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      612 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_association_short_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_cluster_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:58:47.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_clusters_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      587 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_config_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      591 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_coordinator_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:58:48.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:49.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:50.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:51.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:51.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_account_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      611 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_associations.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      636 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_cluster_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      616 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_cluster_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_qos_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_user_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:58:52.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_user_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_wckey_add.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_wckey_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:53.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0038_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_account_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_associations_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_clusters_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_config_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:58:54.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_qos_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      636 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_response_associations_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_set_config.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_tres_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_tres_update.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_update_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_update_users.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_user_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_dbv0039_wckey_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      525 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_status.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:55.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:56.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:56.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_job_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:57.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_job_resources.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:57.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_job_response_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:58.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_node_allocation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_partition.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:58:59.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_reservation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0037_signal.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_diag_rpcm.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:00.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_diag_rpcu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:01.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_job_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:02.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_job_resources.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:02.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_job_response_properties.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:03.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_node_allocation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      558 2023-05-25 03:59:04.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_partition.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      566 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_reservation.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0038_signal.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_account.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_account_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      562 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_accounting.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:05.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_accounting_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      588 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_acct_gather_energy.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_acct_gather_energy_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_usage.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_usage_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      563 2023-05-25 03:59:06.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_cluster_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_cluster_rec_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_controller_ping.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_controller_ping_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_coord.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_coord_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_cron_entry.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_cron_entry_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:07.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_csv_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_diag.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_error.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      546 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_errors.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_ext_sensors_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_ext_sensors_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_float64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_hostlist.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      579 2023-05-25 03:59:08.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_hostlist_string.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      534 2023-05-25 03:59:09.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      601 2023-05-25 03:59:09.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_array_response_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      614 2023-05-25 03:59:09.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_array_response_msg_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      564 2023-05-25 03:59:10.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_argv.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_spank_env.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_exclusive.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:11.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_exit_code.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      593 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_info_gres_detail.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      564 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_info_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      573 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_mem_per_cpu.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      577 2023-05-25 03:59:12.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_mem_per_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      547 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_res.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_res_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      560 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_res_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_submission.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      608 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_submission_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      592 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_job_update_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_jobs_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_license.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_licenses.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      571 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_licenses_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:13.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_meta.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_node.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_nodes_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      575 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_partition_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      596 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_partition_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      595 2023-05-25 03:59:14.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_partitions_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_pings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_power_mgmt_data.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_power_mgmt_data_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      534 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_qos.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_qos_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_qos_preempt_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      585 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_qos_string_id_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      600 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      583 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      604 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      617 2023-05-25 03:59:15.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info_core_spec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      603 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_reservations_response.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_rollup_stats.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      580 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_rollup_stats_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_slurm_step_id.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg_rpcs_by_type.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      598 2023-05-25 03:59:16.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg_rpcs_by_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rec.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rec_ptr.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rpc.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      572 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rpc_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_stats_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_nodes.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_req_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      581 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_req_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:17.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_usage_max.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      589 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_usage_min.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      567 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_string_array.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_tres.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_tres_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      551 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_tres_str.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_uint16_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_uint32_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      568 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_uint64_no_val.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      576 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_update_node_msg.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      538 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_user.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_user_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      550 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_warning.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      554 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_warnings.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      542 2023-05-25 03:59:18.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_wckey.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      559 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_wckey_list.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      555 2023-05-25 03:59:19.000000 slurmrestapi-1.0.1/test/test_models/test_v0039_wckey_tag.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/
+-rw-r--r--   0 keyemyria   (501) staff       (20)     1995 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/__init__.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      826 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_json/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_json/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_json/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_v3/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_v3/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_v3/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_yaml/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_yaml/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:20.000000 slurmrestapi-1.0.1/test/test_paths/test_openapi_yaml/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      864 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_submit/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_node_node_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_nodes/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partition_partition_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partitions/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_ping/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservations/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      864 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_submit/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_licenses/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_node_node_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_nodes/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partition_partition_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partitions/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_ping/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservations/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      845 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      833 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_submit/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_submit/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      818 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_licenses/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_licenses/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      857 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_nodes/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_nodes/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      822 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      876 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partitions/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partitions/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_ping/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_ping/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      811 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_ping/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      890 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      850 2023-05-25 03:59:43.000000 slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      838 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      835 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_job_job_id/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      825 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_job_job_id/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      842 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      856 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      849 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      852 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      860 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      875 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      868 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      836 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      839 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      851 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_diag/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_diag/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      831 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      834 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_jobs/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_jobs/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      820 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      817 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      840 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      821 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      854 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      847 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      824 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      829 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      848 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      841 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py
+drwxr-xr-x   0 keyemyria   (501) staff       (20)        0 2023-05-25 05:49:31.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/
+-rw-r--r--   0 keyemyria   (501) staff       (20)        0 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/__init__.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      828 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py
+-rw-r--r--   0 keyemyria   (501) staff       (20)      827 2023-05-25 03:59:44.000000 slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py
```

### Comparing `slurmrestapi-1.0.0/setup.py` & `slurmrestapi-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
     Contact: sales@schedmd.com
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "slurmrestapi"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = [
     "certifi >= 14.5.14",
     "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
+    "python-dateutil ~= 2.8.0",
     "setuptools >= 21.0.0",
     "typing_extensions ~= 4.3.0",
     "urllib3 ~= 1.26.7",
 ]
 
 setup(
     name=NAME,
```

### Comparing `slurmrestapi-1.0.0/slurmrestapi/__init__.py` & `slurmrestapi-1.0.1/slurmrestapi/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/api_client.py` & `slurmrestapi-1.0.1/slurmrestapi/api_client.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/apis/path_to_api.py` & `slurmrestapi-1.0.1/slurmrestapi/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/apis/tags/openapi_api.py` & `slurmrestapi-1.0.1/slurmrestapi/apis/tags/openapi_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/apis/tags/slurm_api.py` & `slurmrestapi-1.0.1/slurmrestapi/apis/tags/slurm_api.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/configuration.py` & `slurmrestapi-1.0.1/slurmrestapi/configuration.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/exceptions.py` & `slurmrestapi-1.0.1/slurmrestapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_account_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_account_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_association.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_association.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_association_short_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_association_short_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_associations_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_cluster_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_cluster_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_config_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_config_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_config_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_coordinator_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_exit_code.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_job_step.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_job_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_qos_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_account_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_association_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_associations.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_associations.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_cluster_add.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_cluster_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_qos_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_tres.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_user_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_user_update.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_user_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_wckey_add.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_response_wckey_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_tres_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_tres_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_user.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_user_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_wckey.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0037_wckey_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0037_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_account_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_account_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_accounting.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_association.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_association.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_association_short_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_association_short_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_associations_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_cluster_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_cluster_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_clusters_properties.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_clusters_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_config_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_config_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_config_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_coordinator_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_errors.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_exit_code.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_job_step.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_job_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_meta.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_qos_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_account_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_associations.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_associations.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_associations_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_cluster_add.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_cluster_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_qos_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_tres.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_user_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_user_update.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_user_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_wckey_add.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_response_wckey_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_set_config.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_tres_update.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_account.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_update_users.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_user.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_user_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_wckey.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0038_wckey_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0038_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_account_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_associations_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_clusters_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_clusters_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_config_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_errors.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_job_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_meta.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_qos_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_response_associations_delete.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_set_config.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_tres_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_tres_update.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_update_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_update_users.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_user_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_warning.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_warnings.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/dbv0039_wckey_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/dbv0039_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/status.py` & `slurmrestapi-1.0.1/slurmrestapi/model/status.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_properties.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_resources.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_resources.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_response_properties.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_submission.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_job_submission_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_jobs_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_node.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_node_allocation.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_node_allocation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_nodes_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_partition.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_partition.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_partitions_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_ping.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_pings.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_reservation.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_reservation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_reservations_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0037_signal.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0037_signal.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag_rpcm.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag_rpcm.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_diag_rpcu.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_diag_rpcu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_errors.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_properties.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_resources.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_resources.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_response_properties.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_submission.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_job_submission_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_jobs_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_license.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_licenses.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_meta.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_node.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_node_allocation.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_node_allocation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_nodes_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_partition.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_partition.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_partitions_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_ping.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_pings.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_reservation.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_reservation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_reservations_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0038_signal.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0038_signal.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_account.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_account_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_account_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_accounting.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_accounting_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_accounting_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_acct_gather_energy.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_acct_gather_energy.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_acct_gather_energy_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_acct_gather_energy_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_id.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_short_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_short_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_usage.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_usage.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_assoc_usage_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_assoc_usage_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_cluster_rec.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_cluster_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_cluster_rec_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_cluster_rec_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_controller_ping.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_controller_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_controller_ping_array.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_controller_ping_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_coord.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_coord.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_coord_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_coord_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_cron_entry.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_cron_entry.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_cron_entry_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_cron_entry_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_csv_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_csv_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_diag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_error.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_errors.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_ext_sensors_data.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_ext_sensors_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_ext_sensors_data_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_ext_sensors_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_float64_no_val.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_float64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_hostlist.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_hostlist.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_hostlist_string.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_hostlist_string.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_array_response_msg.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_array_response_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_array_response_msg_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_array_response_msg_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_argv.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_argv.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_env.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_desc_msg_spank_env.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_desc_msg_spank_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_exclusive.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_exclusive.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_exit_code.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info_gres_detail.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info_gres_detail.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_info_msg.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_info_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_mem_per_cpu.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_mem_per_cpu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_mem_per_node.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_mem_per_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res_nodes.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_res_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_res_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_submission.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_submission_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_job_update_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_job_update_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_jobs_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_license.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_licenses.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_licenses_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_licenses_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_meta.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_node.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_nodes.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_nodes_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_partition_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_partition_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_partition_info_array.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_partition_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_partitions_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_pings.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_power_mgmt_data.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_power_mgmt_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_power_mgmt_data_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_power_mgmt_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_preempt_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_preempt_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_qos_string_id_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_qos_string_id_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_core_spec.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info_array.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservation_info_core_spec.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservation_info_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_reservations_response.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_rollup_stats.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_rollup_stats.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_rollup_stats_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_rollup_stats_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_slurm_step_id.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_slurm_step_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_type.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_msg_rpcs_by_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rec.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rec_ptr.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rec_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rpc.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rpc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_rpc_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_rpc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_user.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_stats_user_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_stats_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_nodes.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_req_max.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_req_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_req_min.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_req_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_usage_max.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_usage_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_step_tres_usage_min.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_step_tres_usage_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_string_array.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_string_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_tres_str.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_tres_str.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint16_no_val.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint16_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint32_no_val.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint32_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_uint64_no_val.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_uint64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_update_node_msg.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_update_node_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_user.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_user_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_warning.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_warnings.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey_list.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/model/v0039_wckey_tag.py` & `slurmrestapi-1.0.1/slurmrestapi/model/v0039_wckey_tag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/models/__init__.py` & `slurmrestapi-1.0.1/slurmrestapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/__init__.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/openapi/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/openapi/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/openapi_json/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/openapi_json/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/openapi_v3/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/openapi_v3/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/openapi_yaml/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/openapi_yaml/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_job_id/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_job_id/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_job_submit/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_job_submit/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_node_node_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_node_node_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_nodes/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_nodes/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partition_partition_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_partitions/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_partitions/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_ping/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_ping/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservation_reservation_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_37_reservations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_37_reservations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_job_id/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_job_id/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_job_submit/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_job_submit/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_licenses/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_licenses/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_node_node_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_node_node_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_nodes/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_nodes/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partition_partition_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_partitions/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_partitions/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_ping/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_ping/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservation_reservation_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_38_reservations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_38_reservations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_job_id/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_job_submit/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_licenses/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_node_node_name/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_nodes/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partition_partition_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_partitions/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_ping/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_ping/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservation_reservation_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurm_v0_0_39_reservations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_account_account_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_accounts/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_accounts/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_association/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_association/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_associations/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_associations/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_cluster_cluster_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_clusters/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_clusters/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_config/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_config/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_qos_qos_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_tres/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_tres/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_user_user_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_users/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_users/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckey_wckey/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_37_wckeys/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_account_account_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_accounts/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_accounts/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_association/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_association/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_associations/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_associations/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_cluster_cluster_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_clusters/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_clusters/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_config/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_config/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_qos_qos_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_tres/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_tres/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_user_user_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_users/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_users/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckey_wckey/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_38_wckeys/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_account_account_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_accounts/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_association/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_associations/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_cluster_cluster_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_clusters/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_config/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_diag/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_job_job_id/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_jobs/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_qos_qos_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_tres/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_user_user_name/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_users/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckey_wckey/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py` & `slurmrestapi-1.0.1/slurmrestapi/paths/slurmdb_v0_0_39_wckeys/post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/rest.py` & `slurmrestapi-1.0.1/slurmrestapi/rest.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi/schemas.py` & `slurmrestapi-1.0.1/slurmrestapi/schemas.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/slurmrestapi.egg-info/SOURCES.txt` & `slurmrestapi-1.0.1/slurmrestapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_account.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_account_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_account_response.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_account_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_association.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_association.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_association_short_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_association_short_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_associations_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_cluster_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_cluster_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_config_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_config_response.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_config_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_coordinator_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_error.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_job.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_exit_code.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_job_step.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_job_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_qos_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_account_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_association_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_association_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_associations.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_associations.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_cluster_add.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_cluster_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_qos_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_tres.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_user_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_user_update.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_user_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_wckey_add.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_response_wckey_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_tres_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_tres_list.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_user.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_user_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_wckey.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0037_wckey_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0037_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_account.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_account_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_account_response.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_account_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_accounting.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_association.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_association.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_association_short_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_association_short_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_associations_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_cluster_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_cluster_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_clusters_properties.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_clusters_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_config_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_config_response.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_config_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_coordinator_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_coordinator_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_error.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_errors.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_job.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_exit_code.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_job_step.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_job_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_meta.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_qos_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_account_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_account_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_associations.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_associations.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_associations_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_cluster_add.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_cluster_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_cluster_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_cluster_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_qos_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_qos_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_tres.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_user_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_user_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_user_update.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_user_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_wckey_add.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_wckey_add.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_response_wckey_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_response_wckey_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_set_config.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_list.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_tres_update.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_account.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_update_users.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_user.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_user_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_wckey.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0038_wckey_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0038_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_account_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_account_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_associations_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_associations_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_clusters_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_clusters_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_config_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_config_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_error.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_errors.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_job_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_meta.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_qos_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_qos_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_response_associations_delete.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_response_associations_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_set_config.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_set_config.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_tres_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_tres_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_tres_update.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_tres_update.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_update_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_update_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_update_users.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_update_users.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_user_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_user_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_warning.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_warnings.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_dbv0039_wckey_info.py` & `slurmrestapi-1.0.1/test/test_models/test_dbv0039_wckey_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_status.py` & `slurmrestapi-1.0.1/test/test_models/test_status.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_error.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_job_properties.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_job_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_job_resources.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_job_resources.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_job_response_properties.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_job_submission.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_job_submission_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_jobs_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_node.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_node_allocation.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_node_allocation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_nodes_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_partition.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_partition.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_partitions_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_ping.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_pings.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_reservation.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_reservation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_reservations_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0037_signal.py` & `slurmrestapi-1.0.1/test/test_models/test_v0037_signal.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_diag_rpcm.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_diag_rpcm.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_diag_rpcu.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_diag_rpcu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_error.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_errors.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_job_properties.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_job_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_job_resources.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_job_resources.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_job_response_properties.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_job_response_properties.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_job_submission.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_job_submission_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_jobs_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_license.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_licenses.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_meta.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_node.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_node_allocation.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_node_allocation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_nodes_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_partition.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_partition.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_partitions_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_ping.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_pings.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_reservation.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_reservation.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_reservations_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0038_signal.py` & `slurmrestapi-1.0.1/test/test_models/test_v0038_signal.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_account.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_account.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_account_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_account_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_accounting.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_accounting.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_accounting_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_accounting_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_acct_gather_energy.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_acct_gather_energy.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_acct_gather_energy_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_acct_gather_energy_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_id.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_short_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_short_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_usage.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_usage.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_assoc_usage_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_assoc_usage_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_cluster_rec.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_cluster_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_cluster_rec_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_cluster_rec_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_controller_ping.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_controller_ping.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_controller_ping_array.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_controller_ping_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_coord.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_coord.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_coord_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_coord_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_cron_entry.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_cron_entry.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_cron_entry_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_cron_entry_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_csv_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_csv_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_diag.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_diag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_error.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_error.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_errors.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_errors.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_ext_sensors_data.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_ext_sensors_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_ext_sensors_data_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_ext_sensors_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_float64_no_val.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_float64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_hostlist.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_hostlist.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_hostlist_string.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_hostlist_string.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_array_response_msg.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_array_response_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_array_response_msg_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_array_response_msg_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_argv.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_argv.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_env.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_desc_msg_spank_env.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_desc_msg_spank_env.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_exclusive.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_exclusive.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_exit_code.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_exit_code.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_info.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_info_gres_detail.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_info_gres_detail.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_info_msg.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_info_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_mem_per_cpu.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_mem_per_cpu.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_mem_per_node.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_mem_per_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_res.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_res.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_res_nodes.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_res_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_res_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_res_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_submission.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_submission.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_submission_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_submission_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_job_update_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_job_update_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_jobs_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_jobs_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_license.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_license.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_licenses.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_licenses.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_licenses_info.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_licenses_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_meta.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_meta.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_node.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_node.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_nodes.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_nodes_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_nodes_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_partition_info.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_partition_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_partition_info_array.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_partition_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_partitions_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_partitions_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_pings.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_pings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_power_mgmt_data.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_power_mgmt_data.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_power_mgmt_data_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_power_mgmt_data_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_qos.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_qos.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_qos_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_qos_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_qos_preempt_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_qos_preempt_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_qos_string_id_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_qos_string_id_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_core_spec.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info_array.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_reservation_info_core_spec.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_reservation_info_core_spec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_reservations_response.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_reservations_response.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_rollup_stats.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_rollup_stats.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_rollup_stats_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_rollup_stats_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_slurm_step_id.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_slurm_step_id.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg_rpcs_by_type.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg_rpcs_by_type.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_msg_rpcs_by_user.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_msg_rpcs_by_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rec.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rec.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rec_ptr.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rec_ptr.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rpc.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rpc.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_rpc_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_rpc_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_user.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_stats_user_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_stats_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_nodes.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_nodes.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_req_max.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_req_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_req_min.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_req_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_usage_max.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_usage_max.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_step_tres_usage_min.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_step_tres_usage_min.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_string_array.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_string_array.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_tres.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_tres.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_tres_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_tres_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_tres_str.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_tres_str.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_uint16_no_val.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_uint16_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_uint32_no_val.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_uint32_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_uint64_no_val.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_uint64_no_val.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_update_node_msg.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_update_node_msg.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_user.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_user.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_user_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_user_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_warning.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_warning.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_warnings.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_warnings.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_wckey.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_wckey.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_wckey_list.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_wckey_list.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_models/test_v0039_wckey_tag.py` & `slurmrestapi-1.0.1/test/test_models/test_v0039_wckey_tag.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/__init__.py` & `slurmrestapi-1.0.1/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_openapi/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_openapi/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_openapi_json/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_openapi_json/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_openapi_v3/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_openapi_v3/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_openapi_yaml/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_openapi_yaml/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_job_id/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_job_id/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_job_submit/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_job_submit/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_node_node_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_node_node_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_nodes/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_nodes/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partition_partition_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partition_partition_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_partitions/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_partitions/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_ping/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_ping/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservation_reservation_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_37_reservations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_37_reservations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_job_id/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_job_id/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_job_submit/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_job_submit/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_licenses/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_licenses/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_node_node_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_node_node_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_nodes/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_nodes/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partition_partition_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partition_partition_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_partitions/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_partitions/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_ping/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_ping/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservation_reservation_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_38_reservations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_38_reservations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_job_id/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_job_submit/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_licenses/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_node_node_name/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_nodes/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partition_partition_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_partitions/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_ping/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_ping/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservation_reservation_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurm_v0_0_39_reservations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_account_account_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_accounts/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_association/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_association/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_associations/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_associations/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_cluster_cluster_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_clusters/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_clusters/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_config/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_config/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_qos_qos_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_tres/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_tres/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_user_user_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_users/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_users/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckey_wckey/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_37_wckeys/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_account_account_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_accounts/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_association/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_association/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_associations/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_associations/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_cluster_cluster_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_clusters/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_clusters/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_config/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_config/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_qos_qos_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_tres/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_tres/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_user_user_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_users/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_users/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckey_wckey/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_38_wckeys/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_account_account_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_accounts/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_association/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_associations/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_cluster_cluster_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_clusters/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_config/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_diag/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_job_job_id/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_jobs/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_qos_qos_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_tres/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_user_user_name/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_users/test_post.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_delete.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckey_wckey/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_get.py`

 * *Files identical despite different names*

### Comparing `slurmrestapi-1.0.0/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py` & `slurmrestapi-1.0.1/test/test_paths/test_slurmdb_v0_0_39_wckeys/test_post.py`

 * *Files identical despite different names*

