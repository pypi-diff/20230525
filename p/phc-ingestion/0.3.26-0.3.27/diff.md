# Comparing `tmp/phc-ingestion-0.3.26.tar.gz` & `tmp/phc-ingestion-0.3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.3.26.tar", last modified: Fri May 19 13:03:28 2023, max compression
+gzip compressed data, was "phc-ingestion-0.3.27.tar", last modified: Thu May 25 12:52:29 2023, max compression
```

## Comparing `phc-ingestion-0.3.26.tar` & `phc-ingestion-0.3.27.tar`

### file list

```diff
@@ -1,64 +1,37 @@
--rw-r--r--   0        0        0       16 2023-05-19 13:02:59.515446 phc-ingestion-0.3.26/PYPI.md
--rw-r--r--   0        0        0        0 2023-05-19 13:02:59.515446 phc-ingestion-0.3.26/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2023-05-19 13:02:59.515446 phc-ingestion-0.3.26/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-19 13:02:59.515446 phc-ingestion-0.3.26/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2023-05-19 13:02:59.515446 phc-ingestion-0.3.26/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4737 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1325 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      629 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      879 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/gene_to_coords.py
--rw-r--r--   0        0        0      555 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4636 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/json.py
--rw-r--r--   0        0        0    21500 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     4948 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1771 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     5010 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3127 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0     8876 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     3187 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0       46 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     2686 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2018 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     6525 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     2181 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     5430 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     1923 2023-05-19 13:02:59.519446 phc-ingestion-0.3.26/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0      982 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/pyproject.toml
--rw-r--r--   0        0        0    31504 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441.json
--rw-r--r--   0        0        0    31986 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_IHC.json
--rw-r--r--   0        0        0     3696 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_empty_test.json
--rw-r--r--   0        0        0    27666 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_equivocal.json
--rw-r--r--   0        0        0    26976 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_equivocal_status.json
--rw-r--r--   0        0        0    26971 2023-05-19 13:02:59.523446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_high.json
--rw-r--r--   0        0        0    27662 2023-05-19 13:02:59.527446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_msi_foo.json
--rw-r--r--   0        0        0    27090 2023-05-19 13:02:59.527446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_no_phys.json
--rw-r--r--   0        0        0    26970 2023-05-19 13:02:59.527446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_qns.json
--rw-r--r--   0        0        0    26989 2023-05-19 13:02:59.527446 phc-ingestion-0.3.26/tests/caris/resources/TN20-779441_qns_long.json
--rw-r--r--   0        0        0  1537024 2023-05-19 13:02:59.535446 phc-ingestion-0.3.26/tests/caris/resources/carisSample.tar
--rw-r--r--   0        0        0   454560 2023-05-19 13:02:59.535446 phc-ingestion-0.3.26/tests/caris/resources/carisSample.tar.gz
--rw-r--r--   0        0        0    78478 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/caris/test_caris.py
--rw-r--r--   0        0        0      973 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/foundation/data/sample/sample.copynumber.csv
--rw-r--r--   0        0        0      667 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/foundation/data/sample/sample.structural.csv
--rw-r--r--   0        0        0     3038 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/foundation/data/sample/sample.vcf
--rw-r--r--   0        0        0     2524 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/foundation/data/sample.vcf
--rw-r--r--   0        0        0   393383 2023-05-19 13:02:59.539446 phc-ingestion-0.3.26/tests/foundation/data/sample.xml
--rw-r--r--   0        0        0   396026 2023-05-19 13:02:59.543446 phc-ingestion-0.3.26/tests/foundation/data/sample_missing_mrn.xml
--rw-r--r--   0        0        0   396053 2023-05-19 13:02:59.547446 phc-ingestion-0.3.26/tests/foundation/data/sample_namespace.xml
--rw-r--r--   0        0        0   395401 2023-05-19 13:02:59.551446 phc-ingestion-0.3.26/tests/foundation/data/sample_no_biomarkers.xml
--rw-r--r--   0        0        0     3249 2023-05-19 13:02:59.551446 phc-ingestion-0.3.26/tests/foundation/data/sample_scientific_notation/sample_scientific_notation.vcf
--rw-r--r--   0        0        0     2712 2023-05-19 13:02:59.551446 phc-ingestion-0.3.26/tests/foundation/data/sample_scientific_notation.vcf
--rw-r--r--   0        0        0   389679 2023-05-19 13:02:59.555446 phc-ingestion-0.3.26/tests/foundation/data/sample_with_multiple_non_human_content.xml
--rw-r--r--   0        0        0     3038 2023-05-19 13:02:59.555446 phc-ingestion-0.3.26/tests/foundation/data/vcf_expected.vcf
--rw-r--r--   0        0        0     3249 2023-05-19 13:02:59.555446 phc-ingestion-0.3.26/tests/foundation/data/vcf_expected_scientific_notation.vcf
--rw-r--r--   0        0        0    32060 2023-05-19 13:02:59.555446 phc-ingestion-0.3.26/tests/foundation/test_util.py
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.26/PKG-INFO
+-rw-r--r--   0        0        0       16 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/PYPI.md
+-rw-r--r--   0        0        0        0 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4737 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1325 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      629 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      879 2023-05-25 12:52:01.671947 phc-ingestion-0.3.27/ingestion/caris/util/gene_to_coords.py
+-rw-r--r--   0        0        0      555 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4636 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0    21500 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     4948 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0     1771 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     5010 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3127 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0     8876 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     3187 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0       46 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     2686 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2018 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     6525 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     2181 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     5430 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     1923 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2023-05-25 12:52:01.675947 phc-ingestion-0.3.27/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0     1029 2023-05-25 12:52:01.679947 phc-ingestion-0.3.27/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.3.27/PKG-INFO
```

### Comparing `phc-ingestion-0.3.26/ingestion/caris/process.py` & `phc-ingestion-0.3.27/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/cnv.py` & `phc-ingestion-0.3.27/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.3.27/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/ga4gh.py` & `phc-ingestion-0.3.27/ingestion/caris/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/gene_to_coords.py` & `phc-ingestion-0.3.27/ingestion/caris/util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.3.27/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/json.py` & `phc-ingestion-0.3.27/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/metadata.py` & `phc-ingestion-0.3.27/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/structural.py` & `phc-ingestion-0.3.27/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/tsv.py` & `phc-ingestion-0.3.27/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/caris/util/vcf.py` & `phc-ingestion-0.3.27/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/foundation/process.py` & `phc-ingestion-0.3.27/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.3.27/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.3.27/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.3.27/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.3.27/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/process.py` & `phc-ingestion-0.3.27/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.3.27/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.3.27/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.3.27/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.3.27/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.3.27/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.3.27/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.3.27/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.3.26/pyproject.toml` & `phc-ingestion-0.3.27/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.3.26"
+version = "0.3.27"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
@@ -26,14 +26,19 @@
 dev = [
     "black==22.3.0",
     "pytest==7.1.2",
     "pytest-cov==2.10.1",
     "coverage==4.4.2",
 ]
 
+[tool.pdm.build]
+excludes = [
+    "tests/",
+]
+
 [tool.pdm.scripts]
 test = "python3 -m pytest -v --cov-report term-missing --cov=ingestion --log-level=INFO tests/"
 lint = "black --check tests/ ingestion/"
 lint-fix = "black tests/ ingestion/"
 
 [tool.black]
 line-length = 100
```

