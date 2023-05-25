# Comparing `tmp/nci_cidc_cli-0.10.2rc0.tar.gz` & `tmp/nci_cidc_cli-0.10.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-shnc8uzy/nci_cidc_cli-0.10.2rc0.tar", last modified: Thu Apr 27 20:26:32 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-7kznu0r3/nci_cidc_cli-0.10.3.tar", last modified: Thu May 25 14:36:02 2023, max compression
```

## Comparing `nci_cidc_cli-0.10.2rc0.tar` & `nci_cidc_cli-0.10.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/consent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/dbedit/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/cli/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:32.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18457 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57247 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/dbedit/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 20:26:20.000000 nci_cidc_cli-0.10.2rc0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/consent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/nci_cidc_cli/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:36:02.000000 nci_cidc_cli-0.10.3/tests/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/dbedit/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 14:35:54.000000 nci_cidc_cli-0.10.3/tests/util.py
```

### Comparing `nci_cidc_cli-0.10.2rc0/LICENSE` & `nci_cidc_cli-0.10.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/PKG-INFO` & `nci_cidc_cli-0.10.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nci_cidc_cli
-Version: 0.10.2rc0
-Summary: A command-line interface for interacting with the NCI CIDC.
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ## NCI-CIDC-CLI
 
 Command line tool for interfacing with the NCI CIDC API.
 
 ## Setup
 
 ### Installation
@@ -19,21 +11,21 @@
 ```
 
 ### Usage
 
 To display the help message for the CLI, run:
 
 ```bash
-cidc
+nci-cidc
 ```
 
 To authenticate with the CIDC API, run:
 
 ```bash
-cidc login [token]
+nci-cidc login [token]
 ```
 
 ## Development
 
 For local development, install the development dependencies:
 
 ```bash
@@ -43,15 +35,15 @@
 ## Admin functions
 
 Under the (hidden) `admin` are several functions meant for CIDC administators / engineers.
 
 ### CSMS
 
 ```bash
-cidc admin test-csms
+nci-cidc admin test-csms
 ```
 
 A simple API hit for a test of CSMS connection. Hits API endpoint `/admin/test_csms` which in turn gets CSMS's `/docs`.
 This tests that the API is able to successfully make connection with the CSMS, as the `/docs` endpoint requires authorization.
 As the API endpoint is protected, only users with role `cidc-admin` can make this request.
 
 ### dbedit suite
@@ -68,76 +60,76 @@
 ```
 
 #### Configuration
 
 Configuration of the environment ie staging versus production is done as above using:
 
 ```bash
-cidc config get-env
-cidc config set-env ENV
+nci-cidc config get-env
+nci-cidc config set-env ENV
 ```
 
 Configuration of the database username is done via a pair of functions:
 
 ```bash
-cidc admin get-username
-cidc admin set-username USERNAME
+nci-cidc admin get-username
+nci-cidc admin set-username USERNAME
 ```
 
 The password is requested every time you issue a command so as to not store it.
 
 #### Listing data
 
-Under the `list` subcommand of `cidc admin`, you can get descriptions of the data available in the database.
+Under the `list` subcommand of `nci-cidc admin`, you can get descriptions of the data available in the database.
 
-- `cidc admin list clinical TRIAL_ID`
+- `nci-cidc admin list clinical TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `object_url`, `filename`, `num_participants`, `created`, `comment`
 
-- `cidc admin list misc-data TRIAL_ID`
+- `nci-cidc admin list misc-data TRIAL_ID`
 
   - prints a table describing all misc_data files for the given trial
   - with the following columns:
     - `batch_id`, `object_url`, `filename`, `created`, `description`
 
-- `cidc admin list shipments TRIAL_ID`
+- `nci-cidc admin list shipments TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `upload_type`, `manifest_id`, `num_samples`, `created`
 
-- `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
+- `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
   - prints a table listing all samples for the given assay/analysis and trial
   - any of the following values are allowed:
-    - `clinical_data`, same as `cidc admin list clinical TRIAL_ID`
-    - `misc_data`, same as `cidc admin list misc-data TRIAL_ID`
+    - `clinical_data`, same as `nci-cidc admin list clinical TRIAL_ID`
+    - `misc_data`, same as `nci-cidc admin list misc-data TRIAL_ID`
     - analyses: `atacseq_analysis`, `cytof_analysis`, `rna_level1_analysis`, `tcr_analysis`, `wes_analysis`, `wes_analysis_old`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`
     - assays: `atacseq`, `ctdna`, `cytof`, `hande`, `ihc`, `elisa`, `microbiome`, `mif`, `nanostring`, `olink`, `rna`, `tcr`, `wes`
 
 #### Removing data
 
-Under the `remove` subcommand of `cidc admin`, you can remove a wide variety of data from the JSON blobs.
+Under the `remove` subcommand of `nci-cidc admin`, you can remove a wide variety of data from the JSON blobs.
 
-- `cidc admin remove clinical TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
 
   - removes a given clinical data file from a given trial's metadata as well as the file itself from the portal
-  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `cidc admin list clinical TRIAL_ID`
+  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `nci-cidc admin list clinical TRIAL_ID`
     - special value `'*'` for all files for this trial
 
-- `cidc admin remove shipment TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove shipment TRIAL_ID TARGET_ID`
 
   - removes a given shipment from a given trial's metadata
-  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `cidc admin list shipments TRIAL_ID`
+  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `nci-cidc admin list shipments TRIAL_ID`
 
-- `cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
+- `nci-cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
   - removes a given clinical data file from a given trial's metadata as well as the associated files themselves from the portal
-  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `cidc admin remove clinical TRIAL_ID TARGET_ID`
-  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
+  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
+  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
     - It cannot go past where is divisible in the data, but can end early to remove the whole section.
     - Namely:
       - `elisa`: requires only `assay_run_id`
       - `misc_data`, `olink`: require `batch_id` with an optional `filename`
       - `nanostring`: requires `batch_id` and optional `run_id`
       - `rna_level1_analysis`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`: requires only `cimac_id`
       - `wes_analysis`, `wes_analysis_old`: requires only `run_id`
```

### Comparing `nci_cidc_cli-0.10.2rc0/README.md` & `nci_cidc_cli-0.10.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nci_cidc_cli
+Version: 0.10.3
+Summary: A command-line interface for interacting with the NCI CIDC.
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## NCI-CIDC-CLI
 
 Command line tool for interfacing with the NCI CIDC API.
 
 ## Setup
 
 ### Installation
@@ -11,21 +19,21 @@
 ```
 
 ### Usage
 
 To display the help message for the CLI, run:
 
 ```bash
-cidc
+nci-cidc
 ```
 
 To authenticate with the CIDC API, run:
 
 ```bash
-cidc login [token]
+nci-cidc login [token]
 ```
 
 ## Development
 
 For local development, install the development dependencies:
 
 ```bash
@@ -35,15 +43,15 @@
 ## Admin functions
 
 Under the (hidden) `admin` are several functions meant for CIDC administators / engineers.
 
 ### CSMS
 
 ```bash
-cidc admin test-csms
+nci-cidc admin test-csms
 ```
 
 A simple API hit for a test of CSMS connection. Hits API endpoint `/admin/test_csms` which in turn gets CSMS's `/docs`.
 This tests that the API is able to successfully make connection with the CSMS, as the `/docs` endpoint requires authorization.
 As the API endpoint is protected, only users with role `cidc-admin` can make this request.
 
 ### dbedit suite
@@ -60,76 +68,76 @@
 ```
 
 #### Configuration
 
 Configuration of the environment ie staging versus production is done as above using:
 
 ```bash
-cidc config get-env
-cidc config set-env ENV
+nci-cidc config get-env
+nci-cidc config set-env ENV
 ```
 
 Configuration of the database username is done via a pair of functions:
 
 ```bash
-cidc admin get-username
-cidc admin set-username USERNAME
+nci-cidc admin get-username
+nci-cidc admin set-username USERNAME
 ```
 
 The password is requested every time you issue a command so as to not store it.
 
 #### Listing data
 
-Under the `list` subcommand of `cidc admin`, you can get descriptions of the data available in the database.
+Under the `list` subcommand of `nci-cidc admin`, you can get descriptions of the data available in the database.
 
-- `cidc admin list clinical TRIAL_ID`
+- `nci-cidc admin list clinical TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `object_url`, `filename`, `num_participants`, `created`, `comment`
 
-- `cidc admin list misc-data TRIAL_ID`
+- `nci-cidc admin list misc-data TRIAL_ID`
 
   - prints a table describing all misc_data files for the given trial
   - with the following columns:
     - `batch_id`, `object_url`, `filename`, `created`, `description`
 
-- `cidc admin list shipments TRIAL_ID`
+- `nci-cidc admin list shipments TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `upload_type`, `manifest_id`, `num_samples`, `created`
 
-- `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
+- `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
   - prints a table listing all samples for the given assay/analysis and trial
   - any of the following values are allowed:
-    - `clinical_data`, same as `cidc admin list clinical TRIAL_ID`
-    - `misc_data`, same as `cidc admin list misc-data TRIAL_ID`
+    - `clinical_data`, same as `nci-cidc admin list clinical TRIAL_ID`
+    - `misc_data`, same as `nci-cidc admin list misc-data TRIAL_ID`
     - analyses: `atacseq_analysis`, `cytof_analysis`, `rna_level1_analysis`, `tcr_analysis`, `wes_analysis`, `wes_analysis_old`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`
     - assays: `atacseq`, `ctdna`, `cytof`, `hande`, `ihc`, `elisa`, `microbiome`, `mif`, `nanostring`, `olink`, `rna`, `tcr`, `wes`
 
 #### Removing data
 
-Under the `remove` subcommand of `cidc admin`, you can remove a wide variety of data from the JSON blobs.
+Under the `remove` subcommand of `nci-cidc admin`, you can remove a wide variety of data from the JSON blobs.
 
-- `cidc admin remove clinical TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
 
   - removes a given clinical data file from a given trial's metadata as well as the file itself from the portal
-  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `cidc admin list clinical TRIAL_ID`
+  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `nci-cidc admin list clinical TRIAL_ID`
     - special value `'*'` for all files for this trial
 
-- `cidc admin remove shipment TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove shipment TRIAL_ID TARGET_ID`
 
   - removes a given shipment from a given trial's metadata
-  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `cidc admin list shipments TRIAL_ID`
+  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `nci-cidc admin list shipments TRIAL_ID`
 
-- `cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
+- `nci-cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
   - removes a given clinical data file from a given trial's metadata as well as the associated files themselves from the portal
-  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `cidc admin remove clinical TRIAL_ID TARGET_ID`
-  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
+  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
+  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
     - It cannot go past where is divisible in the data, but can end early to remove the whole section.
     - Namely:
       - `elisa`: requires only `assay_run_id`
       - `misc_data`, `olink`: require `batch_id` with an optional `filename`
       - `nanostring`: requires `batch_id` and optional `run_id`
       - `rna_level1_analysis`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`: requires only `cimac_id`
       - `wes_analysis`, `wes_analysis_old`: requires only `run_id`
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/api.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             return "\n".join(message_lines)
         else:
             return str(message)
     except:
         return f"API server encountered an error processing your request {response.status_code}"
 
 
-_USER_AGENT = f"cidc-cli/{__version__}"
+_USER_AGENT = f"nci-cidc-cli/{__version__}"
 
 
 def _with_auth(headers: dict = None, id_token: str = None) -> dict:
     """Add an id token to the given headers"""
     if not id_token:
         id_token = auth.get_id_token()
     return {
@@ -74,19 +74,19 @@
     """
     For a function `api_request` that returns a `Response` object, if that response
     has status code 403, prompt the user to enter a fresh ID token from the portal,
     and retry the request.
     """
 
     urls = {
-        "prod": "https://portal.cimac-network.org/assays/cli-instructions",
-        "staging": "https://stagingportal.cimac-network.org/assays/cli-instructions",
-        "dev-int": "https://cidc-dev.nci.nih.gov/assays/cli-instructions",
+        "prod": "https://cidc.nci.nih.gov/analyses/cli-instructions",
+        "staging": "https://cidc-stage.nci.nih.gov/analyses/cli-instructions",
+        "dev-int": "https://cidc-dev.nci.nih.gov/analyses/cli-instructions",
     }
-    TOKEN_URL = urls[get_env()]
+    TOKEN_URL = urls.get(get_env()) or urls["dev-int"]
 
     @wraps(api_request)
     def wrapped(*args, **kwargs):
         retry = True
         while retry:
             res = api_request(*args, **kwargs)
             # If the error isn't auth-related, break out of the retry loop.
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/auth.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class AuthError(click.ClickException):
     pass
 
 
 def unauthenticated() -> AuthError:
     return AuthError(
         "You are not authenticated. Please login with:\n"
-        "   $ cidc login [YOUR PORTAL TOKEN]"
+        "   $ nci-cidc login [YOUR PORTAL TOKEN]"
     )
 
 
 def validate_token(id_token: str):
     """
     Raises AuthError if id_token is not valid
     """
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/cache.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/cli/cli.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,122 +1,122 @@
 """The second generation CIDC command-line interface."""
 import click
 
 from . import api, auth, gcloud, upload, config, consent, __version__
 from .dbedit.cli import get_username, list_, remove_, set_username
 
-#### $ cidc ####
-@click.group()
+#### $ nci-cidc ####
+@click.group(name="nci-cidc")
 @click.option("-i", "--ignore", default=None, hidden=True)
 def cidc(ignore):
     """The CIDC command-line interface."""
     config.check_env_warning(ignore)
     if not consent.check_consent():
         exit(0)
     gcloud.check_installed()
 
 
-#### $ cidc version ####
+#### $ nci-cidc version ####
 @click.command()
 def version():
     """Echo version and done"""
-    click.echo(f"cidc-cli {__version__}")
+    click.echo(f"nci-cidc-cli {__version__}")
 
 
-#### $ cidc login ####
+#### $ nci-cidc login ####
 @click.command()
 @click.argument("portal_token", required=True, type=str)
 def login(portal_token):
     """Validate and cache the given token"""
     click.echo("Validating token...")
     auth.validate_and_cache_token(portal_token)
     click.echo("You are now logged in.")
 
 
-#### $ cidc config ####
+#### $ nci-cidc config ####
 @click.group("config", hidden=True)
 def config_():
     """Manage CLI configuration."""
 
 
-#### $ cidc config set-env ####
+#### $ nci-cidc config set-env ####
 @click.command()
 @click.argument(
     "environment",
     required=True,
     type=click.Choice(["prod", "staging", "dev-int", "dev"]),
 )
 def set_env(environment):
     """Set the CLI environment."""
     config.set_env(environment)
     click.echo(f"Updated CLI environment to {environment}")
 
 
-#### $ cidc config get-env ####
+#### $ nci-cidc config get-env ####
 @click.command()
 def get_env():
     """Get the current CLI environment."""
     click.echo(config.get_env())
 
 
-#### $ cidc admin ####
+#### $ nci-cidc admin ####
 @click.group("admin", hidden=True)
 def admin_():
     """Manage API admin features."""
 
 
-#### $ cidc admin test-csms ####
+#### $ nci-cidc admin test-csms ####
 @click.command()
 def test_csms():
     """A simple API hit for a test of CSMS connection"""
     api.test_csms()
 
 
-#### $ cidc assays ####
+#### $ nci-cidc assays ####
 @click.group()
 def assays():
     """Manage assay data."""
 
 
-#### $ cidc assays list ####
+#### $ nci-cidc assays list ####
 @click.command("list")
 def list_assays():
     """List all supported assay types."""
     assay_list = api.list_assays()
     for assay in assay_list:
         click.echo(f"* {assay}")
 
 
-#### $ cidc assays upload ####
+#### $ nci-cidc assays upload ####
 @click.command("upload")
 @click.option("--assay", required=True, help="Assay type.")
 @click.option("--xlsx", required=True, help="Path to the assay metadata spreadsheet.")
 def upload_assay(assay, xlsx):
     """
     Upload data for an assay.
     """
     upload.run_upload(assay, xlsx)
 
 
-#### $ cidc analyses ####
+#### $ nci-cidc analyses ####
 @click.group()
 def analyses():
     """Manage analysis data."""
 
 
-#### $ cidc analyses list ####
+#### $ nci-cidc analyses list ####
 @click.command("list")
 def list_analyses():
     """List all supported analysis types."""
     analysis_list = api.list_analyses()
     for analysis in analysis_list:
         click.echo(f"* {analysis}")
 
 
-#### $ cidc analyses upload ####
+#### $ nci-cidc analyses upload ####
 @click.command("upload")
 @click.option("--analysis", required=True, help="Analysis type.")
 @click.option(
     "--xlsx", required=True, help="Path to the analysis metadata spreadsheet."
 )
 def upload_analysis(analysis, xlsx):
     """
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/config.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,16 @@
         print(_STRIKE)
         exit(0)
 
 
 # Environment-specific config
 _current_env = get_env()
 if _current_env == "prod":
-    API_V2_URL = "https://api.cimac-network.org"
+    API_V2_URL = "PROD_PLACEHOLDER"
 elif _current_env == "staging":
-    API_V2_URL = "https://staging-api.cimac-network.org"
+    API_V2_URL = "STAGE_PLACEHOLDER"
 elif _current_env == "dev-int":
     API_V2_URL = "https://nih-nci-cimac-cidc-dpline-dev.uk.r.appspot.com"
 elif _current_env == "dev":
     API_V2_URL = "http://localhost:8000"
 else:
     raise ValueError(f"Unsupported environment: {_current_env}")
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/consent.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/consent.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/cli/dbedit/cli.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,107 +1,107 @@
 from typing import Tuple
 import click
 
 from . import core, remove, list as dblist
 from . import config
 
 
-#### $ cidc admin get-username ####
+#### $ nci-cidc admin get-username ####
 @click.command()
 def get_username():
     """Get the current database username."""
     click.echo(" ".join(["database username:", config.get_username()]))
 
 
-#### $ cidc admin set-username ####
+#### $ nci-cidc admin set-username ####
 @click.command()
 @click.argument("username", required=True, type=str)
 def set_username(username: str):
     """Set the database username."""
     config.set_username(username)
     click.echo(f"Updated database username to {username}")
 
 
-#### $ cidc admin list ####
+#### $ nci-cidc admin list ####
 @click.group("list")
 def list_():
     """Listing different things"""
     pass
 
 
-#### $ cidc admin list supported ####
+#### $ nci-cidc admin list supported ####
 @click.command("supported")
 def list_supported():
     """List assays and analyses that are supported for listing"""
     print(", ".join(sorted(list(dblist.SUPPORTED_ASSAYS_AND_ANALYSES))))
 
 
-#### $ cidc admin list assay ####
+#### $ nci-cidc admin list assay ####
 @click.command("assay")
 @click.argument("trial_id", required=True, type=str)
 @click.argument("assay_or_analysis", required=True, type=str)
 def list_assay(trial_id: str, assay_or_analysis: str):
     """
     List CIMAC IDs for a given assay or analysis for a given trial
-    Same as `cidc admin list analysis`
+    Same as `nci-cidc admin list analysis`
 
     TRIAL_ID is the id of the trial to affect
     ASSAY_OR_ANALYSIS is the assay or analysis to list CIMAC IDs for
     """
     core.connect(dblist)
     dblist.list_data_cimac_ids(trial_id=trial_id, assay_or_analysis=assay_or_analysis)
 
 
-#### $ cidc admin list clinical ####
+#### $ nci-cidc admin list clinical ####
 @click.command("clinical")
 @click.argument("trial_id", required=True, type=str)
 def list_clinical(trial_id: str):
     """
     List clinical files for a given trial
 
     TRIAL_ID is the id of the trial to affect
     """
     core.connect(dblist)
     dblist.list_clinical(trial_id=trial_id)
 
 
-#### $ cidc admin list misc-data ####
+#### $ nci-cidc admin list misc-data ####
 @click.command("misc-data")
 @click.argument("trial_id", required=True, type=str)
 def list_misc_data(trial_id: str):
     """
     List files from misc_data uploads for a given trial
 
     TRIAL_ID is the id of the trial to affect
     """
     core.connect(dblist)
     dblist.list_misc_data(trial_id=trial_id)
 
 
-#### $ cidc admin list shipments ####
+#### $ nci-cidc admin list shipments ####
 @click.command("shipments")
 @click.argument("trial_id", required=True, type=str)
 def list_shipments(trial_id: str):
     """
     List shipments for a given trial
 
     TRIAL_ID is the id of the trial to affect
     """
     core.connect(dblist)
     dblist.list_shipments(trial_id=trial_id)
 
 
-#### $ cidc admin remove ####
+#### $ nci-cidc admin remove ####
 @click.group("remove")
 def remove_():
     """Deleting different things"""
     pass
 
 
-#### $ cidc admin remove assay ####
+#### $ nci-cidc admin remove assay ####
 @click.command("assay")
 @click.argument("trial_id", required=True, type=str)
 @click.argument("assay_or_analysis", required=True, type=str)
 @click.argument("target_id", required=True, nargs=-1)
 def remove_assay(trial_id: str, assay_or_analysis: str, target_id: Tuple[str]):
     """
     Remove a given clinical data file from a given trial's metadata
@@ -117,15 +117,15 @@
     """
     core.connect(remove)
     remove.remove_data(
         trial_id=trial_id, assay_or_analysis=assay_or_analysis, target_id=target_id
     )
 
 
-#### $ cidc admin remove clinical ####
+#### $ nci-cidc admin remove clinical ####
 @click.command("clinical")
 @click.argument("trial_id", required=True, type=str)
 @click.argument("target_id", required=True, type=str)
 def remove_clinical(trial_id: str, target_id: str):
     """
     Remove a given clinical data file from a given trial's metadata
     as well as remove the file itself from the portal.
@@ -135,15 +135,15 @@
         not including {trial_id}/clinical/
         special value * for all files for this trial
     """
     core.connect(remove)
     remove.remove_clinical(trial_id=trial_id, target_id=target_id)
 
 
-#### $ cidc admin remove shipment ####
+#### $ nci-cidc admin remove shipment ####
 @click.command("shipment")
 @click.argument("trial_id", required=True, type=str)
 @click.argument("target_id", required=True, type=str)
 def remove_shipment(trial_id: str, target_id: str):
     """
     Remove a given shipment from a given trial's metadata
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/dbedit/core.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Session = None
 DownloadableFiles, TrialMetadata, UploadJobs, Users = None, None, None, None
 
 
 def connect(list_mod: ModuleType) -> None:
     """
     Set up this module to be able to make sqlalchemy calls
-    uses ENV as set by $ cidc config set-env
+    uses ENV as set by $ nci-cidc config set-env
     defaults to staging unless `prod` is specified ie no `dev` mode
 
     If not already loaded, will ask for your database username
     Asks for database password every time as to not store it
     """
     ENV: str = get_env()
     # TODO: support dev environment running database locally
@@ -36,16 +36,16 @@
     username: Optional[str] = get_username()
     if not username:
         username = input("Username: ")
         set_username(username)
 
     password = getpass.getpass()
     connections = {
-        "prod": "cidc-dfci:us-east1:cidc-postgresql-prod",
-        "staging": "cidc-dfci-staging:us-central1:cidc-postgresql-staging",
+        "prod": "PROD_PLACEHOLDER",
+        "staging": "STAGE_PLACEHOLDER",
         "dev-int": "nih-nci-cimac-cidc-dpline-dev:us-east4:cidc-postgresql-cidc-dev2",
     }
     connection_name = connections[ENV]
 
     # initialize Connector object
     connector = Connector()
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/dbedit/list.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/cli/dbedit/remove.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/dbedit/remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
         if len(target_id) == 1:
             remove_clinical(trial_id=trial_id, target_id=target_id[0])
         else:
             print(
                 "Error: if ASSAY_OR_ANALYSIS == 'clinical_data', only `filename` is accepted"
             )
             print(
-                "You can also directly use the command $ cidc admin remove clinical TRIAL_ID FILE_NAME"
+                "You can also directly use the command $ nci-cidc admin remove clinical TRIAL_ID FILE_NAME"
             )
         return
 
     with Session.begin() as session:
         trial: TrialMetadata = get_trial_if_exists(
             trial_id, with_for_update=True, session=session
         )
```

### Comparing `nci_cidc_cli-0.10.2rc0/cli/gcloud.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/gcloud.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/cli/upload.py` & `nci_cidc_cli-0.10.3/nci_cidc_cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,26 +446,26 @@
                     click.echo()
                     click.secho(status.status_details, fg="red", bold=True)
                     click.echo()
                 else:
                     click.echo("Upload failed. ", nl=False)
                 click.echo(
                     "Please contact a CIDC administrator "
-                    "(cidc@jimmy.harvard.edu) if you need assistance."
+                    "(NCICIDCAdmin@mail.nih.gov) if you need assistance."
                 )
                 click.echo(debug_info_message)
             return
         else:
             # we should never reach this code block
             raise
 
     click.secho("!!!", fg="yellow", bold=True)
     click.echo(
         "Upload timed out. Please contact a CIDC administrator "
-        "(cidc@jimmy.harvard.edu) for assistance."
+        "(NCICIDCAdmin@mail.nih.gov) for assistance."
     )
     click.echo(debug_info_message)
 
 
 def _handle_upload_exc(e: Exception):
     """Handle an exception thrown during an upload attempt."""
     if isinstance(e, KeyboardInterrupt):
```

### Comparing `nci_cidc_cli-0.10.2rc0/nci_cidc_cli.egg-info/PKG-INFO` & `nci_cidc_cli-0.10.3/nci_cidc_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-cli
-Version: 0.10.2rc0
+Version: 0.10.3
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
 
@@ -19,21 +19,21 @@
 ```
 
 ### Usage
 
 To display the help message for the CLI, run:
 
 ```bash
-cidc
+nci-cidc
 ```
 
 To authenticate with the CIDC API, run:
 
 ```bash
-cidc login [token]
+nci-cidc login [token]
 ```
 
 ## Development
 
 For local development, install the development dependencies:
 
 ```bash
@@ -43,15 +43,15 @@
 ## Admin functions
 
 Under the (hidden) `admin` are several functions meant for CIDC administators / engineers.
 
 ### CSMS
 
 ```bash
-cidc admin test-csms
+nci-cidc admin test-csms
 ```
 
 A simple API hit for a test of CSMS connection. Hits API endpoint `/admin/test_csms` which in turn gets CSMS's `/docs`.
 This tests that the API is able to successfully make connection with the CSMS, as the `/docs` endpoint requires authorization.
 As the API endpoint is protected, only users with role `cidc-admin` can make this request.
 
 ### dbedit suite
@@ -68,76 +68,76 @@
 ```
 
 #### Configuration
 
 Configuration of the environment ie staging versus production is done as above using:
 
 ```bash
-cidc config get-env
-cidc config set-env ENV
+nci-cidc config get-env
+nci-cidc config set-env ENV
 ```
 
 Configuration of the database username is done via a pair of functions:
 
 ```bash
-cidc admin get-username
-cidc admin set-username USERNAME
+nci-cidc admin get-username
+nci-cidc admin set-username USERNAME
 ```
 
 The password is requested every time you issue a command so as to not store it.
 
 #### Listing data
 
-Under the `list` subcommand of `cidc admin`, you can get descriptions of the data available in the database.
+Under the `list` subcommand of `nci-cidc admin`, you can get descriptions of the data available in the database.
 
-- `cidc admin list clinical TRIAL_ID`
+- `nci-cidc admin list clinical TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `object_url`, `filename`, `num_participants`, `created`, `comment`
 
-- `cidc admin list misc-data TRIAL_ID`
+- `nci-cidc admin list misc-data TRIAL_ID`
 
   - prints a table describing all misc_data files for the given trial
   - with the following columns:
     - `batch_id`, `object_url`, `filename`, `created`, `description`
 
-- `cidc admin list shipments TRIAL_ID`
+- `nci-cidc admin list shipments TRIAL_ID`
 
   - prints a table describing all shipments for the given trial
   - with the following columns:
     - `upload_type`, `manifest_id`, `num_samples`, `created`
 
-- `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
+- `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`
   - prints a table listing all samples for the given assay/analysis and trial
   - any of the following values are allowed:
-    - `clinical_data`, same as `cidc admin list clinical TRIAL_ID`
-    - `misc_data`, same as `cidc admin list misc-data TRIAL_ID`
+    - `clinical_data`, same as `nci-cidc admin list clinical TRIAL_ID`
+    - `misc_data`, same as `nci-cidc admin list misc-data TRIAL_ID`
     - analyses: `atacseq_analysis`, `cytof_analysis`, `rna_level1_analysis`, `tcr_analysis`, `wes_analysis`, `wes_analysis_old`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`
     - assays: `atacseq`, `ctdna`, `cytof`, `hande`, `ihc`, `elisa`, `microbiome`, `mif`, `nanostring`, `olink`, `rna`, `tcr`, `wes`
 
 #### Removing data
 
-Under the `remove` subcommand of `cidc admin`, you can remove a wide variety of data from the JSON blobs.
+Under the `remove` subcommand of `nci-cidc admin`, you can remove a wide variety of data from the JSON blobs.
 
-- `cidc admin remove clinical TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
 
   - removes a given clinical data file from a given trial's metadata as well as the file itself from the portal
-  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `cidc admin list clinical TRIAL_ID`
+  - `TARGET_ID` is the `filename` of the clinical data to remove, as from `nci-cidc admin list clinical TRIAL_ID`
     - special value `'*'` for all files for this trial
 
-- `cidc admin remove shipment TRIAL_ID TARGET_ID`
+- `nci-cidc admin remove shipment TRIAL_ID TARGET_ID`
 
   - removes a given shipment from a given trial's metadata
-  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `cidc admin list shipments TRIAL_ID`
+  - `TARGET_ID` is the `manifest_id` of the shipment to remove, as from `nci-cidc admin list shipments TRIAL_ID`
 
-- `cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
+- `nci-cidc admin remove assay TRIAL_ID ASSAY_OR_ANALYSIS TARGET_ID`
   - removes a given clinical data file from a given trial's metadata as well as the associated files themselves from the portal
-  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `cidc admin remove clinical TRIAL_ID TARGET_ID`
-  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
+  - for `ASSAY_OR_ANALYSIS=clinical_data`, same as `nci-cidc admin remove clinical TRIAL_ID TARGET_ID`
+  - `TARGET_ID` is a tuple of the ids to find the data to remove, as from `nci-cidc admin list assay TRIAL_ID ASSAY_OR_ANALYSIS`.
     - It cannot go past where is divisible in the data, but can end early to remove the whole section.
     - Namely:
       - `elisa`: requires only `assay_run_id`
       - `misc_data`, `olink`: require `batch_id` with an optional `filename`
       - `nanostring`: requires `batch_id` and optional `run_id`
       - `rna_level1_analysis`, `wes_tumor_only_analysis`, `wes_tumor_only_analysis_old`: requires only `cimac_id`
       - `wes_analysis`, `wes_analysis_old`: requires only `run_id`
```

### Comparing `nci_cidc_cli-0.10.2rc0/setup.py` & `nci_cidc_cli-0.10.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 """
 Setup for the package
 """
 
 from setuptools import setup, find_packages
 
-from cli import __version__
+from nci_cidc_cli import __version__
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="nci_cidc_cli",
     version=__version__,
     packages=find_packages(exclude=("tests")),
-    entry_points={"console_scripts": ["cidc = cli.cli:cidc"]},
+    entry_points={"console_scripts": ["nci-cidc = nci_cidc_cli.cli:cidc"]},
     description="A command-line interface for interacting with the NCI CIDC.",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     python_requires=">=3.6",
 )
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/dbedit/constants.py` & `nci_cidc_cli-0.10.3/tests/dbedit/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_core.py` & `nci_cidc_cli-0.10.3/tests/dbedit/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 from unittest.mock import MagicMock
 
-from cli.dbedit import core
-from cli.config import set_env
+from nci_cidc_cli.dbedit import core
+from nci_cidc_cli.config import set_env
 
 from .constants import TEST_PASSWORD, TEST_TRIAL_ID, TEST_USER
 
 
 class Mocker:
     def __init__(self, monkeypatch) -> None:
         self.sqlalchemy = MagicMock()
@@ -74,15 +74,15 @@
     mocks.Connector.assert_called_once_with()
     mocks.automap_base.assert_called_once_with()
     mocks.sqlalchemy.create_engine.assert_called_once()
     args, _ = mocks.sqlalchemy.create_engine.call_args
     assert args == ("postgresql+pg8000://",)
 
     mocks.Connector_instance.connect.assert_called_once_with(
-        "cidc-dfci:us-east1:cidc-postgresql-prod",
+        "PROD_PLACEHOLDER",
         "pg8000",
         user=TEST_USER,
         password=TEST_PASSWORD,
         db="cidc-prod",
     )
 
     mocks.sessionmaker.assert_called_once_with(mocks.create_engine_result)
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_list.py` & `nci_cidc_cli-0.10.3/tests/dbedit/test_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 import pandas as pd
 from _pytest.monkeypatch import MonkeyPatch
 from unittest.mock import MagicMock
 
-from cli.dbedit import list as dbedit_list
+from nci_cidc_cli.dbedit import list as dbedit_list
 from .constants import (
     TEST_CLINICAL_URL_CSV,
     TEST_CLINICAL_URL_XLSX,
     TEST_METADATA_JSON,
     TEST_MISC_DATA_URL1,
     TEST_MISC_DATA_URL2,
     TEST_TRIAL_ID,
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/dbedit/test_remove.py` & `nci_cidc_cli-0.10.3/tests/dbedit/test_remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from deepdiff import DeepDiff
 import pytest
 from _pytest.monkeypatch import MonkeyPatch
 from typing import Dict, List
 from unittest.mock import MagicMock, call
 
-from cli.dbedit import remove as dbedit_remove
+from nci_cidc_cli.dbedit import remove as dbedit_remove
 from .constants import (
     TEST_CLINICAL_URL_CSV,
     TEST_CLINICAL_URL_XLSX,
     TEST_MANIFEST_ID,
     TEST_METADATA_JSON,
     TEST_TRIAL_ID,
 )
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/test_api.py` & `nci_cidc_cli-0.10.3/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import BytesIO, StringIO
 
 import click
 import pytest
 from unittest.mock import MagicMock
 from typing import Union
 
-from cli import api, auth, config, cache, __version__
+from nci_cidc_cli import api, auth, config, cache, __version__
 
 
 def make_json_response(body={}) -> MagicMock:
     response = MagicMock()
     response.json.return_value = body
     response.status_code = 200
     return response
@@ -63,23 +63,23 @@
 
 
 def test_with_auth(monkeypatch):
     """Test the authorization header builder"""
     TOKEN = "tok"
     AUTH_HEADER = {
         "Authorization": f"Bearer {TOKEN}",
-        "User-Agent": f"cidc-cli/{__version__}",
+        "User-Agent": f"nci-cidc-cli/{__version__}",
     }
     OTHER_HEADERS = {"If-Match": "blah blah blah", "Content-Type": "application/json"}
     HEADERS = {**OTHER_HEADERS, **AUTH_HEADER}
 
     assert api._with_auth(id_token=TOKEN) == AUTH_HEADER
     assert api._with_auth(headers=OTHER_HEADERS, id_token=TOKEN) == HEADERS
 
-    monkeypatch.setattr("cli.auth.validate_token", MagicMock())
+    monkeypatch.setattr("nci_cidc_cli.auth.validate_token", MagicMock())
     auth.validate_and_cache_token(TOKEN)
     assert api._with_auth() == AUTH_HEADER
     assert api._with_auth(headers=OTHER_HEADERS) == HEADERS
 
 
 def test_check_auth(monkeypatch):
     """Check that api.check_auth handles errors as expected"""
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/test_auth.py` & `nci_cidc_cli-0.10.3/tests/test_auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
 
-from cli import auth
+from nci_cidc_cli import auth
 
 
 def test_get_user_email(monkeypatch):
     """Check that get_user_email extracts an email from a JWT"""
     # This is a JWT with payload {"email": "test@email.com"}
     TOKEN = "eyJhbGciOiJIUzI1NiJ9.eyJlbWFpbCI6InRlc3RAZW1haWwuY29tIn0.jTck01ns477JzZY-KLMM82OOZcc6ctJA11HKE8sXiq4"
 
@@ -44,9 +44,9 @@
 
     with runner.isolated_filesystem():
         # Invalid tokens shouldn't be cached
         with pytest.raises(auth.AuthError):
             auth.validate_and_cache_token("blah")
 
         # Invalid tokens *can* be read.
-        monkeypatch.setattr("cli.cache.get", lambda key: "blah")
+        monkeypatch.setattr("nci_cidc_cli.cache.get", lambda key: "blah")
         assert auth.get_id_token() == "blah"
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/test_cache.py` & `nci_cidc_cli-0.10.3/tests/test_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from click.testing import CliRunner
 
-from cli import cache
+from nci_cidc_cli import cache
 
 
 def test_cache_hit(runner: CliRunner):
     """Test storing and getting an object from the cache"""
     key = "foo"
     value1 = "bar"
     value2 = "baz"
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/test_cli.py` & `nci_cidc_cli-0.10.3/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from click.testing import CliRunner
 
-from cli import cli, consent, config, __version__
+from nci_cidc_cli import cli, consent, config, __version__
 from functools import wraps
 
 
 def skip_consent(monkeypatch):
-    monkeypatch.setattr("cli.consent.check_consent", lambda: True)
+    monkeypatch.setattr("nci_cidc_cli.consent.check_consent", lambda: True)
 
 
 def skip_gcloud_installation_check(monkeypatch):
-    monkeypatch.setattr("cli.gcloud.check_installed", lambda: True)
+    monkeypatch.setattr("nci_cidc_cli.gcloud.check_installed", lambda: True)
 
 
 def with_default_env(fn):
     """Ensures that a test run icurrent CLI config isn't overwritten by a test run"""
 
     @wraps(fn)
     def wrap(*args, **kwds):
@@ -33,33 +33,33 @@
     Check that the interface is wired up correctly, and that
     usage is printed when commands are supplied without arguments.
     """
     skip_consent(monkeypatch)
     skip_gcloud_installation_check(monkeypatch)
 
     res = runner.invoke(cli.cidc)
-    assert "Usage: cidc" in res.output
+    assert "Usage: nci-cidc" in res.output
 
     res = runner.invoke(cli.cidc, ["version"])
-    assert f"cidc-cli {__version__}" in res.output
+    assert f"nci-cidc-cli {__version__}" in res.output
 
     res = runner.invoke(cli.cidc, ["assays"])
-    assert "Usage: cidc assays" in res.output
+    assert "Usage: nci-cidc assays" in res.output
 
     res = runner.invoke(cli.cidc, ["config"])
-    assert "Usage: cidc config" in res.output
+    assert "Usage: nci-cidc config" in res.output
 
     res = runner.invoke(cli.cidc, ["login", "-h"])
-    assert "Usage: cidc login" in res.output
+    assert "Usage: nci-cidc login" in res.output
 
 
 @with_default_env
 def test_no_gcloud_installation(runner: CliRunner, monkeypatch):
     """
-    Check that running `cidc [subcommand]` without a gcloud installation prompts
+    Check that running `nci-cidc [subcommand]` without a gcloud installation prompts
     the user to install gcloud.
     """
     skip_consent(monkeypatch)
 
     def assert_gcloud_message(res):
         assert "requires an installation of the gcloud SDK" in res.output
 
@@ -69,25 +69,25 @@
 
 
 @with_default_env
 def test_assays_list(runner: CliRunner, monkeypatch):
     """
     Check that assay_list displays supported assays as expected.
     """
-    monkeypatch.setattr("cli.api.list_assays", lambda: ["wes", "pbmc"])
+    monkeypatch.setattr("nci_cidc_cli.api.list_assays", lambda: ["wes", "pbmc"])
     res = runner.invoke(cli.assays, ["list"])
     assert "* wes" in res.output
     assert "* pbmc" in res.output
 
 
 def test_env_config(runner: CliRunner, monkeypatch):
     """
     Test setting and getting the current environment.
     """
-    monkeypatch.setattr("cli.cache._cache_dir", lambda: "workdir")
+    monkeypatch.setattr("nci_cidc_cli.cache._cache_dir", lambda: "workdir")
     with runner.isolated_filesystem():
         # Get default value
         res = runner.invoke(cli.get_env)
         assert "prod" in res.output
 
         # Set to valid value
         res = runner.invoke(cli.set_env, ["dev"])
@@ -98,15 +98,15 @@
         # Try to set to invalid value
         res = runner.invoke(cli.set_env, ["blah"])
         assert "Invalid value" in res.output
 
 
 def test_consent(runner: CliRunner, monkeypatch):
     """Check the consent flow."""
-    monkeypatch.setattr("cli.cache._cache_dir", lambda: "workdir")
+    monkeypatch.setattr("nci_cidc_cli.cache._cache_dir", lambda: "workdir")
     with runner.isolated_filesystem():
         # User has not yet consented, so prompt for consent.
         res = runner.invoke(cli.cidc, ["assays"], input="y")
         assert consent.TERMS in res.output
         assert consent.AGREEMENT in res.output
 
         # User has now consented, so don't prompt.
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/test_upload.py` & `nci_cidc_cli-0.10.3/tests/test_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 from unittest.mock import MagicMock
 
 import pytest
 import click
 from click.testing import CliRunner
 
-from cli import api
-from cli import upload
+from nci_cidc_cli import api
+from nci_cidc_cli import upload
 
 from .util import ExceptionCatchingThread
 
 JOB_ID = -1
 JOB_ETAG = "abcd"
 GCS_BUCKET = "upload-bucket"
 URL_MAPPING = {
@@ -25,15 +25,15 @@
 OPTIONAL_FILES = []
 UPLOAD_TOKEN = "test-upload-token"
 
 
 class UploadMocks:
     def __init__(self, monkeypatch):
         self.gcloud_login = MagicMock()
-        monkeypatch.setattr("cli.gcloud.login", self.gcloud_login)
+        monkeypatch.setattr("nci_cidc_cli.gcloud.login", self.gcloud_login)
 
         self.api_initiate_upload = MagicMock()
         self.api_initiate_upload.return_value = api.UploadInfo(
             JOB_ID,
             JOB_ETAG,
             GCS_BUCKET,
             URL_MAPPING,
@@ -55,15 +55,17 @@
             upload, "_poll_for_upload_completion", self._poll_for_upload_completion
         )
 
         self._open_file_mapping = MagicMock()
         monkeypatch.setattr(upload, "_open_file_mapping", self._open_file_mapping)
 
         self.insert_extra_metadata = MagicMock()
-        monkeypatch.setattr("cli.api.insert_extra_metadata", self.insert_extra_metadata)
+        monkeypatch.setattr(
+            "nci_cidc_cli.api.insert_extra_metadata", self.insert_extra_metadata
+        )
 
     def assert_expected_calls(self, failure=False):
         self.gcloud_login.assert_called_once()
         self.api_initiate_upload.assert_called_once()
         if failure:
             self.upload_failed.assert_called_once_with(
                 JOB_ID, UPLOAD_TOKEN, JOB_ETAG, GCS_FILE_MAP
@@ -249,15 +251,15 @@
     gsutil_command.return_value.args = ["gsutil", "arg1", "arg2"]
     gsutil_command.return_value.poll = lambda: 0
     gsutil_command.return_value.returncode = 0
     gsutil_command.return_value.stderr = MagicMock("stderr")
     gsutil_command.return_value.stderr.readline = lambda: "gsutil progress"
     monkeypatch.setattr("subprocess.Popen", gsutil_command)
 
-    monkeypatch.setattr("cli.auth.get_id_token", lambda: "test-token")
+    monkeypatch.setattr("nci_cidc_cli.auth.get_id_token", lambda: "test-token")
 
     def do_upload():
         run_upload(runner)
 
     with runner.isolated_filesystem():
         t1 = ExceptionCatchingThread(do_upload)
         t2 = ExceptionCatchingThread(do_upload)
```

### Comparing `nci_cidc_cli-0.10.2rc0/tests/util.py` & `nci_cidc_cli-0.10.3/tests/util.py`

 * *Files identical despite different names*

