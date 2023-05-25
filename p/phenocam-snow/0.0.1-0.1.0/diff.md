# Comparing `tmp/phenocam-snow-0.0.1.tar.gz` & `tmp/phenocam-snow-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jason/Development/PhenoCamSnow/dist/.tmp-bg3lqxys/phenocam-snow-0.0.1.tar", last modified: Thu May 25 02:03:07 2023, max compression
+gzip compressed data, was "/home/jason/Development/PhenoCamSnow/dist/.tmp-33s2v83s/phenocam-snow-0.1.0.tar", last modified: Thu May 25 02:08:12 2023, max compression
```

## Comparing `phenocam-snow-0.0.1.tar` & `phenocam-snow-0.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/
--rw-r--r--   0 jason     (1000) jason     (1000)     1068 2023-05-08 01:52:37.000000 phenocam-snow-0.0.1/LICENSE
--rw-r--r--   0 jason     (1000) jason     (1000)     3667 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)     2205 2023-05-25 02:00:35.000000 phenocam-snow-0.0.1/README.md
--rw-r--r--   0 jason     (1000) jason     (1000)     1908 2023-05-08 01:52:37.000000 phenocam-snow-0.0.1/pyproject.toml
--rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/setup.cfg
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow/
--rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-05-08 01:52:37.000000 phenocam-snow-0.0.1/src/phenocam_snow/__init__.py
--rw-r--r--   0 jason     (1000) jason     (1000)     8000 2023-05-08 01:52:37.000000 phenocam-snow-0.0.1/src/phenocam_snow/data.py
--rw-r--r--   0 jason     (1000) jason     (1000)     3312 2023-05-24 21:51:46.000000 phenocam-snow-0.0.1/src/phenocam_snow/model.py
--rw-r--r--   0 jason     (1000) jason     (1000)     5863 2023-05-25 02:00:35.000000 phenocam-snow-0.0.1/src/phenocam_snow/predict.py
--rw-r--r--   0 jason     (1000) jason     (1000)     9600 2023-05-25 02:00:35.000000 phenocam-snow-0.0.1/src/phenocam_snow/train.py
--rw-r--r--   0 jason     (1000) jason     (1000)    12009 2023-05-08 01:52:37.000000 phenocam-snow-0.0.1/src/phenocam_snow/utils.py
-drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/
--rw-r--r--   0 jason     (1000) jason     (1000)     3667 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/PKG-INFO
--rw-r--r--   0 jason     (1000) jason     (1000)      402 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/SOURCES.txt
--rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/dependency_links.txt
--rw-r--r--   0 jason     (1000) jason     (1000)      316 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/requires.txt
--rw-r--r--   0 jason     (1000) jason     (1000)       14 2023-05-25 02:03:07.000000 phenocam-snow-0.0.1/src/phenocam_snow.egg-info/top_level.txt
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/
+-rw-r--r--   0 jason     (1000) jason     (1000)     1068 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/LICENSE
+-rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)     1849 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/README.md
+-rw-r--r--   0 jason     (1000) jason     (1000)     1904 2023-05-25 02:06:22.000000 phenocam-snow-0.1.0/pyproject.toml
+-rw-r--r--   0 jason     (1000) jason     (1000)       38 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/setup.cfg
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow/
+-rw-r--r--   0 jason     (1000) jason     (1000)        0 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/__init__.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     8000 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/data.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     3312 2023-05-24 21:51:46.000000 phenocam-snow-0.1.0/src/phenocam_snow/model.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     6201 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/src/phenocam_snow/predict.py
+-rw-r--r--   0 jason     (1000) jason     (1000)     9616 2023-05-25 02:05:18.000000 phenocam-snow-0.1.0/src/phenocam_snow/train.py
+-rw-r--r--   0 jason     (1000) jason     (1000)    12009 2023-05-08 01:52:37.000000 phenocam-snow-0.1.0/src/phenocam_snow/utils.py
+drwxr-xr-x   0 jason     (1000) jason     (1000)        0 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/
+-rw-r--r--   0 jason     (1000) jason     (1000)     3307 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/PKG-INFO
+-rw-r--r--   0 jason     (1000) jason     (1000)      402 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/SOURCES.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)        1 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/dependency_links.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)      316 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/requires.txt
+-rw-r--r--   0 jason     (1000) jason     (1000)       14 2023-05-25 02:08:12.000000 phenocam-snow-0.1.0/src/phenocam_snow.egg-info/top_level.txt
```

### Comparing `phenocam-snow-0.0.1/LICENSE` & `phenocam-snow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.0.1/PKG-INFO` & `phenocam-snow-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phenocam-snow
-Version: 0.0.1
+Version: 0.1.0
 Summary: Pipeline for building deep learning models to classify PhenoCam images.
 Author-email: Jason Jewik <jason.jewik@cs.ucla.edu>
 Project-URL: Source, https://github.com/jasonjewik/PhenoCamSnowClassifier
 Project-URL: Issue Tracker, https://github.com/jasonjewik/PhenoCamSnowClassifier/issues
 Project-URL: Documentation, https://phenocamsnow.readthedocs.io/en/latest/
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -43,52 +43,38 @@
 
 ```console
 pip install phenocam-snow
 ```
 
 Optional dependencies for development and documentation purposes can be installed by specifying the extras `[dev]` and `[docs]`, repsectively. 
 
-## Quickstart
+## Example Usage
 
-The following code snippets show how to perform classification of canadaOBS images into "snow", "no snow", and "too dark". If you wish to use a different site, use the canonical site name as listed on [the PhenoCam website](https://phenocam.nau.edu/webcam/network/table/). 
+The following code snippets show how to train and evaluate a model on classifying images from the canadaojp site into "snow", "no snow", and "too dark".
 
-### Training a model
-
-With new data:
 ```console
-python -m phenocam_snow.train canadaOBS \
+python -m phenocam_snow.train \
+   canadaojp \
+   --model resnet18 \
+   --learning_rate 5e-4 \
+   --weight_decay 0.01 \
    --new \
    --n_train 120 \
    --n_test 30 \
    --classes snow no_snow too_dark
 ```
+This will print out the file path of the best model, which can be substituted into the next command.
 
-With already downloaded and labeled data:
-```console
-python -m phenocam_snow.train \
-   --existing \
-   --train_dir canadaOBS_train \
-   --test_dir canadaOBS_test \
-   --classes snow no_snow too_dark
-```
-
-### Getting predictions
-
-For a local directory of images:
-```console
-python -m phenocam_snow.predict canadaOBS \
-   [path/to/checkpoint_of_best_model.pth] \
-   --directory canadaOBS_test_images
-```
-
-For a single online image:
 ```console
-python -m phenocam_snow.predict canadaOBS \
-   [path/to/checkpoint_of_best_model.pth] \
-   --url https://phenocam.sr.unh.edu/[path/to/image]
+python -m phenocam_snow.predict \
+   canadaojp \
+   [path/to/best_model.ckpt] \
+   resnet18 \
+   --categories snow no_snow too_dark
+   --url https://phenocam.nau.edu/data/latest/canadaojp.jpg
 ```
 
 Advanced usage details can be found in the [documentation](http://phenocamsnow.readthedocs.io/).
 
 ## Citation
 
 If you use PhenoCamSnow for your work, please see [`CITATION.cff`](CITATION.cff) or use the citation prompt provided by GitHub in the sidebar.
```

### Comparing `phenocam-snow-0.0.1/pyproject.toml` & `phenocam-snow-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phenocam-snow"
-version = "0.0.1"
+version = "0.1.0"
 authors = [
     { name = "Jason Jewik", email = "jason.jewik@cs.ucla.edu" }
 ]
 description = "Pipeline for building deep learning models to classify PhenoCam images."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow/data.py` & `phenocam-snow-0.1.0/src/phenocam_snow/data.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow/model.py` & `phenocam-snow-0.1.0/src/phenocam_snow/model.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow/predict.py` & `phenocam-snow-0.1.0/src/phenocam_snow/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 def main():
     parser = ArgumentParser(description="Predicts image category using the given model")
     parser.add_argument(
         "site_name", help="The PhenoCam site for which we are generating predictions."
     )
     parser.add_argument("model_path", help="The path of the model to use.")
+    parser.add_argument("resnet", help="The type of resnet used.")
     parser.add_argument("--categories", nargs="+", help="The image categories to use.")
     parser.add_argument(
         "--url",
         default=None,
         help="Provide this if you want to get a prediction for \
                             a single online image.",
     )
@@ -36,39 +37,40 @@
     args = parser.parse_args()
 
     if args.url and args.directory:
         print("Cannot specify both --url and --directory")
     elif not (args.url or args.directory):
         print("Please specify either --url or --directory")
     else:
-        model = load_model_from_file(args.model_path, len(args.categories))
+        model = load_model_from_file(args.model_path, args.resnet, len(args.categories))
         if args.url:
             run_model_online(model, args.site_name, args.categories, args.url)
         elif args.directory:
             run_model_offline(model, args.site_name, args.categories, args.directory)
 
 
-def classify_online(model, img_url):
+def classify_online(model, categories, img_url):
     """Performs online classification.
 
     :param model: The model to use.
     :type model: PhenoCamResNet
+    :param categories: The categories to use.
+    :type categories: List[str]
     :param img_url: The URL of the image to run classification on.
     :type img_url: str
     :return: A 2-tuple where the first element is the image at `img_url` as a
         NumPy array and the second element is the predicted label.
     """
-    categories = ["too_dark", "no_snow", "snow"]
     try:
         resp = requests.get(img_url, timeout=5, verify=False)
     except:
         print("Request timed out")
     if resp.ok:
         img = Image.open(BytesIO(resp.content))
-        np_img = np.array(img)
+        np_img = np.array(img).T
         x = torch.from_numpy(np_img)
         dm = PhenoCamDataModule(
             "dummy_site_name",
             "dummy_train_dir",
             "dummy_train_anns",
             "dummy_test_dir",
             "dummy_test_anns",
@@ -78,67 +80,73 @@
         pred = categories[torch.argmax(yhat, dim=1)]
         return (np_img, pred)
     else:
         print("Error occurred")
     return None
 
 
-def classify_offline(model, img_path):
+def classify_offline(model, categories, img_path):
     """Performs offline classification.
 
     :param model: The model to use.
     :type model: PhenoCamResNet
+    :param categories: The image categories.
+    :type categories: List[str]
     :param img_path: The file path of the image to classify.
     :type img_path: str
     :return: A 2-tuple where the first element is the image at `img_path` as a
         NumPy array and the second element is the predicted label.
     """
-    categories = ["too_dark", "no_snow", "snow"]
     dm = PhenoCamDataModule(
         "dummy_site_name",
         "dummy_train_dir",
         "dummy_train_anns",
         "dummy_test_dir",
         "dummy_test_anns",
     )
     x = dm.preprocess(read_image(img_path).unsqueeze(0))
     yhat = model(x)
     pred = categories[torch.argmax(yhat, dim=1)]
     return pred
 
 
-def load_model_from_file(model_path):
+def load_model_from_file(model_path, resnet, n_classes):
     """Loads a model from checkpoint file.
 
     :param model_path: The path to the model checkpoint file.
     :type model_path: str
+    :param resnet: The type of Resnet that was used.
+    :type resnet: str
+    :param n_classes: The number of classes.
+    :type n_classes: int
     :return: The loaded model.
     :rtype: PhenoCamResNet
     """
-    model = PhenoCamResNet().load_from_checkpoint(model_path)
+    model = PhenoCamResNet.load_from_checkpoint(
+        model_path, resnet=resnet, n_classes=n_classes
+    )
     model.freeze()
     return model
 
 
-def run_model_offline(model, site_name, img_dir):
+def run_model_offline(model, site_name, categories, img_dir):
     """Gets predicted labels for all images in a directory.
 
     :param model: The model to use.
     :type model: PhenoCamResNet
     :param site_name: The name of the PhenoCam site.
     :type site_name: str
     :param img_dir: The directory containing the images to classify.
     :type img_dir: str
     :return: A pandas DataFrame with predictions.
     :rtype: pd.DataFrame
     """
     ######################
     # 1. Get predictions #
     ######################
-    categories = ["too_dark", "no_snow", "snow"]
     if type(img_dir) is str:
         img_dir = Path(img_dir)
     timestamps, predictions = [], []
     for img_path in img_dir.glob("*.jpg"):
         ts_arr = img_path.stem.split("_")
         ts = "-".join(ts_arr[1:4])
         hms = ts_arr[-1]
```

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow/train.py` & `phenocam-snow-0.1.0/src/phenocam_snow/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     ##################
     # 2. Train model #
     ##################
     dm.setup(stage="fit")
     model = PhenoCamResNet(model, len(classes), learning_rate, weight_decay)
     logger = TensorBoardLogger(save_dir=os.getcwd(), name=f"{site_name}_lightning_logs")
-    callbacks = [EarlyStopping(monitor="val_loss", mode="min")]
+    callbacks = [EarlyStopping(monitor="val_loss", mode="min", min_delta=1e-8)]
     accelerator = "gpu" if torch.cuda.is_available() else None
     trainer = pl.Trainer(
         logger=logger,
         callbacks=callbacks,
         max_epochs=50,
         log_every_n_steps=3,
         accelerator=accelerator,
```

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow/utils.py` & `phenocam-snow-0.1.0/src/phenocam_snow/utils.py`

 * *Files identical despite different names*

### Comparing `phenocam-snow-0.0.1/src/phenocam_snow.egg-info/PKG-INFO` & `phenocam-snow-0.1.0/src/phenocam_snow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: phenocam-snow
-Version: 0.0.1
+Version: 0.1.0
 Summary: Pipeline for building deep learning models to classify PhenoCam images.
 Author-email: Jason Jewik <jason.jewik@cs.ucla.edu>
 Project-URL: Source, https://github.com/jasonjewik/PhenoCamSnowClassifier
 Project-URL: Issue Tracker, https://github.com/jasonjewik/PhenoCamSnowClassifier/issues
 Project-URL: Documentation, https://phenocamsnow.readthedocs.io/en/latest/
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -43,52 +43,38 @@
 
 ```console
 pip install phenocam-snow
 ```
 
 Optional dependencies for development and documentation purposes can be installed by specifying the extras `[dev]` and `[docs]`, repsectively. 
 
-## Quickstart
+## Example Usage
 
-The following code snippets show how to perform classification of canadaOBS images into "snow", "no snow", and "too dark". If you wish to use a different site, use the canonical site name as listed on [the PhenoCam website](https://phenocam.nau.edu/webcam/network/table/). 
+The following code snippets show how to train and evaluate a model on classifying images from the canadaojp site into "snow", "no snow", and "too dark".
 
-### Training a model
-
-With new data:
 ```console
-python -m phenocam_snow.train canadaOBS \
+python -m phenocam_snow.train \
+   canadaojp \
+   --model resnet18 \
+   --learning_rate 5e-4 \
+   --weight_decay 0.01 \
    --new \
    --n_train 120 \
    --n_test 30 \
    --classes snow no_snow too_dark
 ```
+This will print out the file path of the best model, which can be substituted into the next command.
 
-With already downloaded and labeled data:
-```console
-python -m phenocam_snow.train \
-   --existing \
-   --train_dir canadaOBS_train \
-   --test_dir canadaOBS_test \
-   --classes snow no_snow too_dark
-```
-
-### Getting predictions
-
-For a local directory of images:
-```console
-python -m phenocam_snow.predict canadaOBS \
-   [path/to/checkpoint_of_best_model.pth] \
-   --directory canadaOBS_test_images
-```
-
-For a single online image:
 ```console
-python -m phenocam_snow.predict canadaOBS \
-   [path/to/checkpoint_of_best_model.pth] \
-   --url https://phenocam.sr.unh.edu/[path/to/image]
+python -m phenocam_snow.predict \
+   canadaojp \
+   [path/to/best_model.ckpt] \
+   resnet18 \
+   --categories snow no_snow too_dark
+   --url https://phenocam.nau.edu/data/latest/canadaojp.jpg
 ```
 
 Advanced usage details can be found in the [documentation](http://phenocamsnow.readthedocs.io/).
 
 ## Citation
 
 If you use PhenoCamSnow for your work, please see [`CITATION.cff`](CITATION.cff) or use the citation prompt provided by GitHub in the sidebar.
```

