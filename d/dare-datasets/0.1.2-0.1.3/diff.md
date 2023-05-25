# Comparing `tmp/dare_datasets-0.1.2.tar.gz` & `tmp/dare_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.2.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.3.tar", max compression
```

## Comparing `dare_datasets-0.1.2.tar` & `dare_datasets-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       67 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/__init__.py
--rw-r--r--   0        0        0     1953 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1427 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      696 2023-05-23 16:47:14.762549 dare_datasets-0.1.2/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0      406 2023-05-23 16:47:14.766549 dare_datasets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 dare_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     2310 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1427 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      528 2023-05-25 11:16:19.907255 dare_datasets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 dare_datasets-0.1.3/PKG-INFO
```

### Comparing `dare_datasets-0.1.2/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.3/dare_datasets/dataset_abc.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,61 +2,74 @@
 
 # Url of the FOLDER of the dataset in Google Drive. The folder must be publicly available.
 GDRIVE_URL = ""
 
 
 class Dataset(ABC):
     """
-    Set of methods that every dataset should implement. Apart from these methods the class can
+    Set of methods that every dataset should implement.
+
+    Apart from these methods the class can
     implement whichever other method is considered needed e.g. different versions of the dataset.
     """
     @abstractmethod
     def __init__(self, cache_dir: str | None = '~/.cache/dare-datasets/') -> None:
+        """
+        Initializer chooses the cache directory where the dataset will be downloaded or retrieved.
+        Note the dataset is not yet downloaded.
+
+        Args:
+            cache_dir: Folder where the dataset will be downloaded or retrieved from.
+        """
         pass
 
     @abstractmethod
     def _init_data(self):
         """
         Loads the dataset from disk. If the dataset is not available on disk, it is downloaded and saved in cache.
         """
         pass
 
     @abstractmethod
     def get_info(self) -> dict[str, str]:
         """
         Returns a dictionary with information about the dataset.
         Necessary:
-            - name: name of dataset
-            - description: description of dataset
-            - url: url of cocalc file
-            - original_url: original url of dataset (can be the paper url)
-            - formats: list of formats the dataset is available eg. ["csv", "json", "xml"]
+            - **name**: name of dataset
+            - **description**: description of dataset
+            - **url**: url of gdrive file
+            - **original_url**: original url of dataset (can be the paper url)
+            - **formats**: list of formats the dataset is available eg. ["csv", "json", "xml"]
 
         """
         pass
 
     @abstractmethod
     def get_raw(self):
         """
         Returns the raw data of the dataset on whichever format we consider default.
         Structure (if not applicable it is not enforced):
+        ```python
             {
                  "train":[],
                  "dev":[],
                  "test":[]
             }
+        ```
         """
         pass
 
     @abstractmethod
     def get_processed(self):
         """
         Returns the processed data of the dataset on whichever format we consider default.
         If many processed versions are available, the one we consider default should be the one returned.
         Structure (if not applicable it is not enforced):
+        ```python
             {
                  "train":[],
                  "dev":[],
                  "test":[]
             }
+        ```
         """
         pass
```

### Comparing `dare_datasets-0.1.2/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.3/dare_datasets/qr2t_benchmark.py`

 * *Files identical despite different names*

