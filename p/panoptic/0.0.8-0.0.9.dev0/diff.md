# Comparing `tmp/panoptic-0.0.8.tar.gz` & `tmp/panoptic-0.0.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panoptic-0.0.8.tar", last modified: Tue May 23 17:02:14 2023, max compression
+gzip compressed data, was "panoptic-0.0.9.dev0.tar", last modified: Thu May 25 08:28:51 2023, max compression
```

## Comparing `panoptic-0.0.8.tar` & `panoptic-0.0.9.dev0.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.898768 panoptic-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 17:02:14.898768 panoptic-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 17:02:02.000000 panoptic-0.0.8/build_commans.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 17:02:02.000000 panoptic-0.0.8/description.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.890768 panoptic-0.0.8/panoptic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/compute/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/compute/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/compute/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/compute/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/core/
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/core/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/core/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/core/image_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/html/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/assets/bootstrap-icons-966620f9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/assets/bootstrap-icons-c6569d46.woff
--rw-r--r--   0 runner    (1001) docker     (123)   246090 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/assets/index-4bdeb548.js
--rw-r--r--   0 runner    (1001) docker     (123)   428783 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/assets/index-4d21f9b4.css
--rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/models/payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.894768 panoptic-0.0.8/panoptic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/scripts/create_db.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-23 17:02:02.000000 panoptic-0.0.8/panoptic/scripts/populate_db.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 17:02:14.890768 panoptic-0.0.8/panoptic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 17:02:14.000000 panoptic-0.0.8/panoptic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-23 17:02:02.000000 panoptic-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 17:02:14.898768 panoptic-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-23 17:02:02.000000 panoptic-0.0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-23 17:02:02.000000 panoptic-0.0.8/thunder-collection_Panoptic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.715440 panoptic-0.0.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 08:28:51.715440 panoptic-0.0.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/build_commans.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/description.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.707440 panoptic-0.0.9.dev0/panoptic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.711440 panoptic-0.0.9.dev0/panoptic/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/compute/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/compute/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/compute/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/compute/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.711440 panoptic-0.0.9.dev0/panoptic/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/core/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/core/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/core/image_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.711440 panoptic-0.0.9.dev0/panoptic/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.711440 panoptic-0.0.9.dev0/panoptic/html/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   121296 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/html/assets/bootstrap-icons-966620f9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164352 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/html/assets/bootstrap-icons-c6569d46.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67646 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/html/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.715440 panoptic-0.0.9.dev0/panoptic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/models/payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.715440 panoptic-0.0.9.dev0/panoptic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/scripts/create_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/scripts/populate_db.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/panoptic/scripts/to_pca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:28:51.707440 panoptic-0.0.9.dev0/panoptic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 08:28:51.000000 panoptic-0.0.9.dev0/panoptic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:28:51.715440 panoptic-0.0.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-05-25 08:28:38.000000 panoptic-0.0.9.dev0/thunder-collection_Panoptic.json
```

### Comparing `panoptic-0.0.8/PKG-INFO` & `panoptic-0.0.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.8
+Version: 0.0.9.dev0
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.8/description.md` & `panoptic-0.0.9.dev0/description.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/api.py` & `panoptic-0.0.9.dev0/panoptic/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from starlette.responses import Response
 from starlette.staticfiles import StaticFiles
 
 from panoptic import core
 from panoptic.core import create_property, add_property_to_image, get_images, create_tag, \
     delete_image_property, \
     update_tag, get_tags, get_properties, delete_property, update_property, delete_tag, delete_tag_parent, add_folder, \
-    db_utils, make_clusters, get_similar_images
+    db_utils, make_clusters, get_similar_images, get_full_image
 from panoptic.core import db
 from panoptic.models import Property, Images, Tag, Tags, Properties, PropertyPayload, \
     AddImagePropertyPayload, AddTagPayload, DeleteImagePropertyPayload, \
     UpdateTagPayload, UpdatePropertyPayload, Tab, MakeClusterPayload
 
 app = FastAPI()
 app.add_middleware(
@@ -129,15 +129,17 @@
     res = await db.get_folders()
     return res
 
 
 @app.get('/import_status')
 async def get_import_status_route():
     image_import = core.importer
-    res = {'to_import': image_import.total_import, 'imported': image_import.current_import}
+    new_image = core.get_new_images()
+    update = [await get_full_image(i) for i in new_image]
+    res = {'to_import': image_import.total_import, 'imported': image_import.current_computed, 'new_images': update}
     return res
 
 
 class PathRequest(BaseModel):
     path: str
```

### Comparing `panoptic-0.0.8/panoptic/compute/ocr.py` & `panoptic-0.0.9.dev0/panoptic/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/compute/similarity.py` & `panoptic-0.0.9.dev0/panoptic/compute/similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         pickle.dump(tree, f)
     global SIMILARITY_TREE
     SIMILARITY_TREE = tree
 
 def get_similar_images(vector: np.ndarray):
     if not SIMILARITY_TREE:
         raise ValueError("Cannot compute image similarity since KDTree was not computed yet")
-    return SIMILARITY_TREE.query(vector, k=200)
+    return SIMILARITY_TREE.query(vector)
 
 
 def make_clusters(images: list[ImageVector], *, method='kmeans', **kwargs) -> list[list[str]]:
     res = []
     vectors, sha1, ahashs = zip(*[(i.vector, i.sha1, i.ahash) for i in images])
     sha1 = np.asarray(sha1)
     ahashs = np.asarray(ahashs)
```

### Comparing `panoptic-0.0.8/panoptic/compute/transform.py` & `panoptic-0.0.9.dev0/panoptic/compute/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 import numpy as np
 from imagehash import average_hash
 from hashlib import sha1 as sha1hash
 import glob
 from PIL import Image
 from sklearn.decomposition import PCA
 from sklearn.neighbors import KDTree
-from transformers import AutoImageProcessor, MobileNetV2Model
+from transformers import AutoImageProcessor, MobileNetV2Model, CLIPVisionModel, CLIPProcessor
 # from .ocr import full_ocr
 from .utils import load_data
 
 from transformers import logging
 
 logging.set_verbosity_error()
 
-PCA_SIZE = 15
+PCA_SIZE = 10
 USE_PCA_IF_POSSIBLE = True
 
 processor = AutoImageProcessor.from_pretrained("google/mobilenet_v2_1.0_224")
 model = MobileNetV2Model.from_pretrained("google/mobilenet_v2_1.0_224")
+
 pca: None | PCA = None
 tree: None | KDTree = None
 try:
     data = load_data()
 except ValueError:
     data = None
 
@@ -108,42 +109,53 @@
 
 def to_vector(img):
     input1 = processor(images=img, return_tensors="pt")
     output1 = model(**input1)
     pooled_output1 = output1[1].detach().numpy()
     vector = pooled_output1.flatten()
     # if a pca was already trained use it
-    if pca is not None:
+    if get_pca() is not None:
         return to_pca(vector)
     return vector
 
 
 # def to_ocr(image: Image):
 #     return full_ocr(image)
 
+def get_pca():
+    path = os.path.join(os.getenv('PANOPTIC_DATA'), 'pca.pkl')
+    global pca
+    if pca:
+        return pca
+    if not pca and os.path.exists(path):
+        with open(path, 'rb') as f:
+            pca = pickle.load(f)
+        return pca
+    return None
+
 
 def make_clusters(sensibility):
     pass
 
 
 def load_clusters():
     pass
 
 
 def create_pca(vectors: []):
     from sklearn.decomposition import PCA
     global pca
     pca = PCA(PCA_SIZE)
     pca.fit(vectors)
-    return pca
+    save_pca()
 
 
-def to_pca(vectors: []):
+def to_pca(vector: np.ndarray):
     if pca is not None:
-        return pca.transform(vectors)
+        return np.float32(pca.transform([vector])[0])
 
 
 def save_pca():
     with open(os.path.join(os.getenv('PANOPTIC_DATA'), 'pca.pkl'), 'wb') as f:
         pickle.dump(pca, f)
 
 
@@ -153,10 +165,12 @@
     Basically it's: do we have more vectors than 110% the number of dimensions ?
     :param nb_vectors: number of vectors that are going to be used to train pca
     :param vector_sample: one of the vectors
     :return: bool
     """
     if not USE_PCA_IF_POSSIBLE:
         return False
+    if pca is not None:
+        return False
     if nb_vectors > vector_sample.shape[0] + (vector_sample.shape[0] / 10):
         return True
     return False
```

### Comparing `panoptic-0.0.8/panoptic/compute/utils.py` & `panoptic-0.0.9.dev0/panoptic/compute/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,12 @@
 
 class SimilarityTreeWithLabel:
     def __init__(self, images: list[ImageVector]):
         vectors, sha1_list = zip(*[(i.vector, i.sha1) for i in images])
         self.image_labels = sha1_list
         self.tree = KDTree(vectors)
 
-    def query(self, image: np.ndarray, k=200):
-        if k > len(self.image_labels):
-            k = len(self.image_labels)
-        dist, ind = self.tree.query(image.reshape(1, -1), k)
+    def query(self, image: np.ndarray):
+        dist, ind = self.tree.query(image.reshape(1, -1), len(self.image_labels))
         indices = [x for x in ind[0]]
         distances = [x for x in dist[0]]
         return [{'sha1': self.image_labels[i], 'dist': float('%.2f' % (distances[index]))} for index, i in enumerate(indices)]
```

### Comparing `panoptic-0.0.8/panoptic/core/__init__.py` & `panoptic-0.0.9.dev0/panoptic/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import atexit
 import json
 from concurrent.futures import ProcessPoolExecutor
 from typing import List
 
 from fastapi import HTTPException
 
@@ -51,14 +52,31 @@
                                  extension=extension, ahash=ahash)
         if property_id:
             result[sha1].properties[property_id] = PropertyValue(
                 **{'property_id': property_id, 'value': db.decode_if_json(value)})
     return result
 
 
+async def get_full_image(sha1: str) -> Image:
+    """
+    Get all images from database
+    """
+    rows = await db.get_full_image_with_sha1(sha1)
+    result = None
+    for row in rows:
+        sha1, paths, height, width, url, extension, name, property_id, value, ahash = row
+        result = Image(sha1=sha1, paths=json.loads(paths), width=width, height=height, url=url, name=name,
+                       extension=extension, ahash=ahash)
+        if property_id:
+            result.properties[property_id] = PropertyValue(
+                **{'property_id': property_id, 'value': db.decode_if_json(value)})
+        break
+    return result
+
+
 async def make_clusters(sensibility: float, image_list: [str]) -> list[list[str]]:
     """
     Compute clusters and return a list of list of sha1
     """
     # TODO: add parameters to compute clusters only on some images
     images = await db.get_images_with_vectors(image_list)
     return compute.make_clusters(images, method="kmeans", nb_clusters=sensibility)
@@ -83,54 +101,69 @@
         raise HTTPException(status_code=400, detail="Trying to set a value on a non existent property or sha1")
 
 
 async def delete_image_property(property_id: int, sha1: str):
     await db.delete_image_property(property_id, sha1)
 
 
+# TODO: confirm lock efficacity
+add_image_lock = asyncio.Lock()
+
+
 async def add_image_to_db(file_path, name, extension, width, height, sha1_hash, url) -> Image:
-    image = await db.get_image_by_sha1(sha1_hash)
-    # Si sha1_hash existe déjà, on ajoute file_path à la liste de paths
-    if image:
-        if file_path not in image.paths:
-            image.paths.append(file_path)
-            # Mise à jour de la liste de paths
-            await db.update_image_paths(sha1_hash, json.dumps(image.paths))
+    async with add_image_lock:
+        image = await db.get_image_by_sha1(sha1_hash)
+        # Si sha1_hash existe déjà, on ajoute file_path à la liste de paths
+        if image:
+            if file_path not in image.paths:
+                image.paths.append(file_path)
+                # Mise à jour de la liste de paths
+                await db.update_image_paths(sha1_hash, json.dumps(image.paths))
 
-    # Si sha1_hash n'existe pas, on l'ajoute avec la liste de paths contenant file_path
-    else:
-        await db.add_image(sha1_hash, height, width, name, extension, json.dumps([file_path]), url)
-    return await db.get_image_by_sha1(sha1_hash)
+        # Si sha1_hash n'existe pas, on l'ajoute avec la liste de paths contenant file_path
+        else:
+            await db.add_image(sha1_hash, height, width, name, extension, json.dumps([file_path]), url)
+        return await db.get_image_by_sha1(sha1_hash)
 
 
 async def add_folder(folder):
     found = await importer.import_folder(save_callback, folder)
     print(f'found {found} images')
     return folder
 
 
+new_images = []
+
+
+def get_new_images():
+    copy = [i for i in new_images]
+    new_images.clear()
+    return copy
+
+
 async def save_callback(image, folder_id: Folder, name, extension, width, height, sha1_hash, url, file_path):
     await add_image_to_db(folder_id, name, extension, width, height, sha1_hash, url)
-
+    new_images.append(sha1_hash)
     importer.compute_image(get_compute_callback(sha1_hash), image_path=file_path)
 
 
 def get_compute_callback(sha1):
     async def callback(ahash, vector, is_last=False):
         await db.update_image_hashs(sha1, str(ahash), vector)
+
     return callback
 
 
 @importer.set_final_callback
 async def compute_finished_callback():
     images: list[ImageVector] = await db.get_images_with_vectors()
     compute.create_similarity_tree(images)
 
 
-async def create_tag(property_id, value, parent_id, color:str) -> Tag:
+async def create_tag(property_id, value, parent_id, color: str) -> Tag:
     existing_tag = await db.get_tag(property_id, value)
     if existing_tag is not None:
         if await db.tag_in_ancestors(existing_tag.id, parent_id):
             raise HTTPException(status_code=400, detail="Adding a tag that is an ancestor of himself")
         existing_tag.parents = list({*existing_tag.parents, parent_id})
         await db.update_tag(existing_tag)
         tag_id = existing_tag.id
```

### Comparing `panoptic-0.0.8/panoptic/core/db.py` & `panoptic-0.0.9.dev0/panoptic/core/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,25 @@
     image = await cursor.fetchone()
     if image:
         return Image(**auto_dict(image, cursor))
     else:
         return None
 
 
+async def get_full_image_with_sha1(sha1: str):
+    query = """
+            SELECT DISTINCT i.sha1, i.paths, i.height, i.width,  i.url, i.extension, i.name, i_d.property_id, i_d.value, i.ahash
+            FROM images i
+            LEFT JOIN images_properties i_d ON i.sha1 = i_d.sha1
+            WHERE i.sha1 = ?
+            """
+    cursor = await execute_query(query, (sha1,))
+    return await cursor.fetchall()
+
+
 async def get_images():
     query = """
             SELECT DISTINCT i.sha1, i.paths, i.height, i.width,  i.url, i.extension, i.name, i_d.property_id, i_d.value, i.ahash
             FROM images i
             LEFT JOIN images_properties i_d ON i.sha1 = i_d.sha1
             """
     cursor = await execute_query(query)
@@ -250,20 +261,20 @@
 async def get_image_properties_with_tag(tag_id: int) -> list[ImageProperty]:
     query = "SELECT * from images_properties ip where ip.value like ?"
     cursor = await execute_query(query, (f"[%{tag_id}%]",))
     return [ImageProperty(**auto_dict(row, cursor)) for row in await cursor.fetchall()]
 
 
 async def get_images_with_vectors(image_list: list[str] = None):
-    query = "SELECT sha1, vector, ahash from images"
+    query = "SELECT sha1, vector, ahash from images WHERE vector is not null "
     if image_list and len(image_list) > 0:
-        query += " WHERE sha1 in (" + ','.join('?' * len(image_list)) + ')'
+        query += " AND sha1 in (" + ','.join('?' * len(image_list)) + ')'
         cursor = await execute_query(query, tuple(image_list))
     else:
         cursor = await execute_query(query)
     return [ImageVector(**auto_dict(row, cursor)) for row in await cursor.fetchall()]
 
 
 async def get_all_sha1() -> list[str]:
     query = "SELECT sha1 from images ORDER BY sha1"
     cursor = await execute_query(query)
-    return [row for row in await cursor.fetchall()]
+    return [row for row in await cursor.fetchall()]
```

### Comparing `panoptic-0.0.8/panoptic/core/db_utils.py` & `panoptic-0.0.9.dev0/panoptic/core/db_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import aiosqlite
 import numpy as np
 
 ALL_TABLES = ['images', 'images_properties', 'properties', 'tags', 'folders', 'tabs']
 
 aiosqlite.register_adapter(np.array, lambda arr: arr.tobytes())
-aiosqlite.register_converter("array", np.frombuffer)
+aiosqlite.register_converter("array", lambda arr: np.frombuffer(arr, dtype='float32'))
 
 conn: aiosqlite.Connection | None = None
 
 
 async def init():
     global conn
     conn = await aiosqlite.connect("panoptic.db", detect_types=sqlite3.PARSE_DECLTYPES)
```

### Comparing `panoptic-0.0.8/panoptic/core/image_importer.py` & `panoptic-0.0.9.dev0/panoptic/core/image_importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     async def wrap_compute(self, future, callback):
         task = asyncio.wrap_future(future)
         res = await task
         self.current_computed += 1
         await callback(*res)
         # this was the last callback
-        if len(self.compute_tasks) == 1:
+        if self.current_computed == self.total_import:
             await self._final_callback()
 
     def set_final_callback(self, fn: Callable):
         self._final_callback = fn
         return fn
 
 def compute_image(image_path: str = None, image: Image = None):
```

### Comparing `panoptic-0.0.8/panoptic/html/assets/bootstrap-icons-966620f9.woff2` & `panoptic-0.0.9.dev0/panoptic/html/assets/bootstrap-icons-966620f9.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/html/assets/bootstrap-icons-c6569d46.woff` & `panoptic-0.0.9.dev0/panoptic/html/assets/bootstrap-icons-c6569d46.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/html/favicon.ico` & `panoptic-0.0.9.dev0/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/main.py` & `panoptic-0.0.9.dev0/panoptic/main.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/models/models.py` & `panoptic-0.0.9.dev0/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/models/payloads.py` & `panoptic-0.0.9.dev0/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/scripts/create_db.sql` & `panoptic-0.0.9.dev0/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic/scripts/populate_db.sql` & `panoptic-0.0.9.dev0/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.0.8/panoptic.egg-info/PKG-INFO` & `panoptic-0.0.9.dev0/panoptic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panoptic
-Version: 0.0.8
+Version: 0.0.9.dev0
 License: Mozilla
 Description-Content-Type: text/markdown
 
 # Panoptic
```

### Comparing `panoptic-0.0.8/setup.py` & `panoptic-0.0.9.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def parse_requirements(req_file):
     with open(req_file) as fp:
         _requires = fp.read()
     return _requires
 
 
 NAME = "panoptic"
-VERSION = "0.0.8"
+VERSION = "0.0.9.dev"
 # Get dependencies from requirement files
 SETUP_REQUIRES = ['setuptools', 'setuptools-git', 'wheel']
 INSTALL_REQUIRES = parse_requirements('requirements.txt')
 LONG_DESCRIPTION = ""
 
 with open(os.path.join(os.path.dirname(__file__), 'description.md'), 'r') as f:
     LONG_DESCRIPTION = f.read()
```

### Comparing `panoptic-0.0.8/thunder-collection_Panoptic.json` & `panoptic-0.0.9.dev0/thunder-collection_Panoptic.json`

 * *Files identical despite different names*

