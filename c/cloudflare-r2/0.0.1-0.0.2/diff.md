# Comparing `tmp/cloudflare_r2-0.0.1.tar.gz` & `tmp/cloudflare_r2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_r2-0.0.1.tar", max compression
+gzip compressed data, was "cloudflare_r2-0.0.2.tar", max compression
```

## Comparing `cloudflare_r2-0.0.1.tar` & `cloudflare_r2-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1491 2023-05-15 14:17:56.734231 cloudflare_r2-0.0.1/LICENSE
--rw-r--r--   0        0        0      253 2023-05-15 15:11:48.461211 cloudflare_r2-0.0.1/README.md
--rw-r--r--   0        0        0       53 2023-05-15 09:09:00.873115 cloudflare_r2-0.0.1/cloudflare_r2/__init__.py
--rw-r--r--   0        0        0     7533 2023-05-15 15:05:00.205749 cloudflare_r2-0.0.1/cloudflare_r2/main.py
--rw-r--r--   0        0        0     1351 2023-05-15 15:06:37.262154 cloudflare_r2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1050 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-15 14:17:56.734231 cloudflare_r2-0.0.2/LICENSE
+-rw-r--r--   0        0        0      253 2023-05-15 15:11:48.461211 cloudflare_r2-0.0.2/README.md
+-rw-r--r--   0        0        0       73 2023-05-25 06:07:18.337332 cloudflare_r2-0.0.2/cloudflare_r2/__init__.py
+-rw-r--r--   0        0        0     8124 2023-05-25 06:10:00.302571 cloudflare_r2-0.0.2/cloudflare_r2/main.py
+-rw-r--r--   0        0        0     1333 2023-05-25 07:48:32.968616 cloudflare_r2-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.2/PKG-INFO
```

### Comparing `cloudflare_r2-0.0.1/LICENSE` & `cloudflare_r2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_r2-0.0.1/cloudflare_r2/main.py` & `cloudflare_r2-0.0.2/cloudflare_r2/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             aws_access_key_id=self.access_key_id,
             aws_secret_access_key=self.secret_access_key,
             region_name=self.region,
         )
 
     def get_bucket(self, bucket_name: str):
         """Get an R2 bucket instance."""
-        return self.resource.Bucket(bucket_name)
+        return self.resource.Bucket(bucket_name)  # type: ignore
 
 
 class CloudflareR2Bucket(CloudflareR2):
     """
     Helper function that can be assigned to each bucket.
 
     Note [AWS API reference](https://docs.aws.amazon.com/AmazonS3/latest/API) vs. [R2](https://developers.cloudflare.com/r2/data-access/s3-api/api/)
@@ -91,14 +91,29 @@
             dict | None: Returns `None` if not found.
         """  # noqa: E501
         try:
             return self.client.get_object(Bucket=self.name, Key=key, *args, **kwargs)
         except Exception:
             return None
 
+    def put(self, key: str, *args, **kwargs) -> dict | None:
+        """Assumes the key prefix exists in the bucket. See helper
+        for [boto3 put_object](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/put_object.html)
+
+        Args:
+            key (str): Should exist in the bucket.
+
+        Returns:
+            dict | None: Returns `None` if not found.
+        """  # noqa: E501
+        try:
+            return self.client.put_object(Bucket=self.name, Key=key, *args, **kwargs)
+        except Exception:
+            return None
+
     def fetch(self, *args, **kwargs) -> dict:
         """Each bucket contain content prefixes but can only be fetched by batches. Each batch is limited
         to a max of 1000 prefixes. Without arguments included in this call, will default to the first 1000 keys.
 
         See details in [boto3 list-objects-v2 API docs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/list_objects_v2.html#list-objects-v2)
         """  # noqa: E501
         return self.client.list_objects_v2(Bucket=self.name, *args, **kwargs)
```

### Comparing `cloudflare_r2-0.0.1/pyproject.toml` & `cloudflare_r2-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cloudflare-r2"
 description = "Wrapper around commonly used boto3 functions in Cloudflare R2 API."
-version = "0.0.1"
+version = "0.0.2"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-r2"
 documentation = "https://mv3.dev/cloudflare-r2"
 classifiers = [
   "Programming Language :: Python :: 3.11",
@@ -18,15 +18,14 @@
 python = "^3.11"
 python-dotenv = "^1.0"
 boto3 = "^1.26"
 start-cloudflare = "^0.0.1"
 
 [tool.poetry.group.dev.dependencies] # latest as of Jan. 2023
 rich = "^13.3"
-black = "^23.3.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
```

### Comparing `cloudflare_r2-0.0.1/PKG-INFO` & `cloudflare_r2-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cloudflare-r2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper around commonly used boto3 functions in Cloudflare R2 API.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
 Requires-Dist: start-cloudflare (>=0.0.1,<0.0.2)
 Project-URL: Documentation, https://mv3.dev/cloudflare-r2
 Project-URL: Repository, https://github.com/justmars/cloudflare-r2
 Description-Content-Type: text/markdown
```

