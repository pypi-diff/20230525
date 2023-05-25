# Comparing `tmp/skelly_viewer-2023.5.1018.tar.gz` & `tmp/skelly_viewer-2023.5.1019.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_viewer-2023.5.1018.tar", last modified: Mon May  8 20:24:18 2023, max compression
+gzip compressed data, was "skelly_viewer-2023.5.1019.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_viewer-2023.5.1018.tar` & `skelly_viewer-2023.5.1019.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       66 2023-05-08 20:24:10.153940 skelly_viewer-2023.5.1018/.gitattributes
--rw-r--r--   0        0        0     1087 2023-05-08 20:24:10.153940 skelly_viewer-2023.5.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     2784 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/.gitignore
--rw-r--r--   0        0        0     1067 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/LICENSE
--rw-r--r--   0        0        0      989 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/README.md
--rw-r--r--   0        0        0     1660 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/setup.py
--rw-r--r--   0        0        0     1023 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/__init__.py
--rw-r--r--   0        0        0      351 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/__main__.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/__init__.py
--rw-r--r--   0        0        0     1382 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/default_paths.py
--rw-r--r--   0        0        0      478 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/folder_and_file_names.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/init.py
--rw-r--r--   0        0        0     1406 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/logging_configuration.py
--rw-r--r--   0        0        0     1554 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/experimental/checkable_combo_box.py
--rw-r--r--   0        0        0     1155 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/__init__.py
--rw-r--r--   0        0        0     3418 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skelly_viewer_widget.py
--rw-r--r--   0        0        0     2945 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skellyview_main_window.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/init.py
--rw-r--r--   0        0        0     5825 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/multi_video_display.py
--rw-r--r--   0        0        0     6284 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
--rw-r--r--   0        0        0     2648 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/slider_widget.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
--rw-r--r--   0        0        0      965 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
--rw-r--r--   0        0        0     1896 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
--rw-r--r--   0        0        0     2168 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
--rw-r--r--   0        0        0      134 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/test_test.py
--rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/__init__.py
--rw-r--r--   0        0        0     2329 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/freemocap_data_loader.py
--rw-r--r--   0        0        0      850 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/load_sample_data.py
--rw-r--r--   0        0        0     6077 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/mediapipe_skeleton_builder.py
--rw-r--r--   0        0        0     1805 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/video_handler.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 skelly_viewer-2023.5.1018/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/.gitattributes
+-rw-r--r--   0        0        0     1087 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     2784 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/.gitignore
+-rw-r--r--   0        0        0     1067 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/LICENSE
+-rw-r--r--   0        0        0      989 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/README.md
+-rw-r--r--   0        0        0     1660 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/setup.py
+-rw-r--r--   0        0        0     1023 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/__init__.py
+-rw-r--r--   0        0        0      351 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/config/__init__.py
+-rw-r--r--   0        0        0     1382 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/config/default_paths.py
+-rw-r--r--   0        0        0      478 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/config/folder_and_file_names.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/config/init.py
+-rw-r--r--   0        0        0     1406 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/config/logging_configuration.py
+-rw-r--r--   0        0        0     1554 2023-05-25 18:23:47.622249 skelly_viewer-2023.5.1019/skelly_viewer/experimental/checkable_combo_box.py
+-rw-r--r--   0        0        0     1155 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/__init__.py
+-rw-r--r--   0        0        0     3418 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/skelly_viewer_widget.py
+-rw-r--r--   0        0        0     2945 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/skellyview_main_window.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/init.py
+-rw-r--r--   0        0        0     5789 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/multi_video_display.py
+-rw-r--r--   0        0        0     6284 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
+-rw-r--r--   0        0        0     2648 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/slider_widget.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
+-rw-r--r--   0        0        0      965 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
+-rw-r--r--   0        0        0     1896 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
+-rw-r--r--   0        0        0     2168 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
+-rw-r--r--   0        0        0      134 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/test_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/utilities/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/utilities/freemocap_data_loader.py
+-rw-r--r--   0        0        0      850 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     6077 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/utilities/mediapipe_skeleton_builder.py
+-rw-r--r--   0        0        0     1805 2023-05-25 18:23:47.626249 skelly_viewer-2023.5.1019/skelly_viewer/utilities/video_handler.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 skelly_viewer-2023.5.1019/PKG-INFO
```

### Comparing `skelly_viewer-2023.5.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_viewer-2023.5.1019/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/.gitignore` & `skelly_viewer-2023.5.1019/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/LICENSE` & `skelly_viewer-2023.5.1019/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/README.md` & `skelly_viewer-2023.5.1019/README.md`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/pyproject.toml` & `skelly_viewer-2023.5.1019/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1018"
+current_version = "v2023.05.1019"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/__init__.py` & `skelly_viewer-2023.5.1019/skelly_viewer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_viewer"
-__version__ = "v2023.05.1018"
+__version__ = "v2023.05.1019"
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
```

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/config/default_paths.py` & `skelly_viewer-2023.5.1019/skelly_viewer/config/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/config/logging_configuration.py` & `skelly_viewer-2023.5.1019/skelly_viewer/config/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/experimental/checkable_combo_box.py` & `skelly_viewer-2023.5.1019/skelly_viewer/experimental/checkable_combo_box.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py` & `skelly_viewer-2023.5.1019/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skelly_viewer_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/skelly_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skellyview_main_window.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/skellyview_main_window.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/multi_video_display.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/multi_video_display.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,25 +52,23 @@
     def generate_video_display(self, path_to_video_folder: Union[str, Path]):
         self._video_handler_dictionary = self._create_video_handlers(list(Path(path_to_video_folder).glob('*.mp4')))
         self._image_label_widget_dictionary = self._create_image_label_widgets_for_videos(
             number_of_videos=len(self._video_handler_dictionary))
         self._add_widgets_to_layout()
 
         self.update_worker.video_handlers = list(self._video_handler_dictionary.values())
-        self.update_worker.updated.connect(self._update_display)
+        self.update_worker.updated.connect(self.update_display)
 
     def start_update_worker(self):
         self.update_worker.start()
 
     def stop_update_worker(self):
         self.update_worker.terminate()
 
-    def _update_display(self, image, video_number):
-        image_label_widget = self._image_label_widget_dictionary[video_number]
-        self._set_pixmap_from_image(image_label_widget, image)
+
 
     def _add_widgets_to_layout(self):
         column_count = 0
         row_count = 0
         for widget in self._image_label_widget_dictionary:
             self.video_display_layout.addWidget(self._image_label_widget_dictionary[widget], row_count, column_count)
 
@@ -78,18 +76,22 @@
             column_count += 1
             if column_count % MAX_COLUMN_COUNT == 0:
                 column_count = 0
                 row_count += 1
 
     def update_display(self, frame_number: int):
         # logger.debug(f"Updating video display to frame#{frame_number}")
-        for video_handler, image_label_widget in zip(self._video_handler_dictionary.values(),
+        try:
+            for video_handler, image_label_widget in zip(self._video_handler_dictionary.values(),
                                                      self._image_label_widget_dictionary.values()):
-            image = video_handler.get_image_for_frame_number(frame_number)
-            self._set_pixmap_from_image(image_label_widget, image)
+                image = video_handler.get_image_for_frame_number(frame_number)
+                self._set_pixmap_from_image(image_label_widget, image)
+
+        except Exception as e:
+            logger.warning(f"Error updating display for video {video_handler.video_path.name}: {e}")
 
     def _set_pixmap_from_image(self,
                                image_label_widget: QLabel,
                                image: np.ndarray):
         q_image = self._convert_image_to_qimage(image)
         pixmap = QPixmap.fromImage(q_image)
```

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/slider_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/slider_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py` & `skelly_viewer-2023.5.1019/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/utilities/freemocap_data_loader.py` & `skelly_viewer-2023.5.1019/skelly_viewer/utilities/freemocap_data_loader.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/utilities/load_sample_data.py` & `skelly_viewer-2023.5.1019/skelly_viewer/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/utilities/mediapipe_skeleton_builder.py` & `skelly_viewer-2023.5.1019/skelly_viewer/utilities/mediapipe_skeleton_builder.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/skelly_viewer/utilities/video_handler.py` & `skelly_viewer-2023.5.1019/skelly_viewer/utilities/video_handler.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.5.1018/PKG-INFO` & `skelly_viewer-2023.5.1019/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_viewer
-Version: 2023.5.1018
+Version: 2023.5.1019
 Summary: View a skelly
 Keywords: basic,template,python,repository
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

