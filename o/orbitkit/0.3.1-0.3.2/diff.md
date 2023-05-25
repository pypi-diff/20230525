# Comparing `tmp/orbitkit-0.3.1.tar.gz` & `tmp/orbitkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/orbitkit-0.3.1.tar", last modified: Mon May 22 01:06:19 2023, max compression
+gzip compressed data, was "dist/orbitkit-0.3.2.tar", last modified: Wed May 24 09:23:30 2023, max compression
```

## Comparing `orbitkit-0.3.1.tar` & `orbitkit-0.3.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/
--rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.3.1/LICENSE
--rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.3.1/MANIFEST.in
--rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-22 01:06:19.000000 orbitkit-0.3.1/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     2207 2021-10-31 14:45:20.000000 orbitkit-0.3.1/README.md
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/
--rw-r--r--   0 crown      (501) staff       (20)        6 2023-05-20 01:15:42.000000 orbitkit-0.3.1/orbitkit/VERSION
--rw-r--r--   0 crown      (501) staff       (20)      354 2023-05-22 01:04:02.000000 orbitkit-0.3.1/orbitkit/__init__.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/file_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        1 2021-07-15 08:55:40.000000 orbitkit-0.3.1/orbitkit/file_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     2111 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/dispatcher.py
--rw-r--r--   0 crown      (501) staff       (20)      244 2021-10-31 03:25:18.000000 orbitkit-0.3.1/orbitkit/file_extractor/exception.py
--rw-r--r--   0 crown      (501) staff       (20)     1912 2021-10-31 14:48:38.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor.py
--rw-r--r--   0 crown      (501) staff       (20)      224 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_audio.py
--rw-r--r--   0 crown      (501) staff       (20)     1211 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_html.py
--rw-r--r--   0 crown      (501) staff       (20)     2034 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_json.py
--rw-r--r--   0 crown      (501) staff       (20)     1016 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_office.py
--rw-r--r--   0 crown      (501) staff       (20)     2983 2022-05-06 07:35:45.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_pdf.py
--rw-r--r--   0 crown      (501) staff       (20)      868 2021-10-31 14:31:58.000000 orbitkit-0.3.1/orbitkit/file_extractor/extractor_txt.py
--rw-r--r--   0 crown      (501) staff       (20)      277 2021-07-27 10:13:23.000000 orbitkit-0.3.1/orbitkit/file_extractor/util.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/id_srv/
--rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.3.1/orbitkit/id_srv/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.3.1/orbitkit/id_srv/id_gen.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/lark_send/
--rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.3.1/orbitkit/lark_send/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.3.1/orbitkit/lark_send/lark.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/pdf_extractor/
--rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.3.1/orbitkit/pdf_extractor/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py
--rw-r--r--   0 crown      (501) staff       (20)     4888 2023-05-10 06:34:32.000000 orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
--rw-r--r--   0 crown      (501) staff       (20)    11739 2023-05-10 06:34:32.000000 orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit/util/
--rw-r--r--   0 crown      (501) staff       (20)      104 2023-05-10 05:26:36.000000 orbitkit-0.3.1/orbitkit/util/__init__.py
--rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.3.1/orbitkit/util/common.py
--rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.3.1/orbitkit/util/util_aws.py
--rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.3.1/orbitkit/util/util_date.py
--rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.3.1/orbitkit/util/util_str.py
--rw-r--r--   0 crown      (501) staff       (20)    19087 2021-12-26 13:51:52.000000 orbitkit-0.3.1/orbitkit/util/util_type_mapping.py
-drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-22 01:06:19.000000 orbitkit-0.3.1/orbitkit.egg-info/
--rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/PKG-INFO
--rw-r--r--   0 crown      (501) staff       (20)     1159 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/SOURCES.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/dependency_links.txt
--rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/not-zip-safe
--rw-r--r--   0 crown      (501) staff       (20)       89 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/requires.txt
--rw-r--r--   0 crown      (501) staff       (20)        9 2023-05-22 01:06:18.000000 orbitkit-0.3.1/orbitkit.egg-info/top_level.txt
--rw-r--r--   0 crown      (501) staff       (20)       38 2023-05-22 01:06:19.000000 orbitkit-0.3.1/setup.cfg
--rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.3.1/setup.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/
+-rw-r--r--   0 crown      (501) staff       (20)     1073 2020-10-28 02:45:18.000000 orbitkit-0.3.2/LICENSE
+-rw-r--r--   0 crown      (501) staff       (20)      118 2022-01-24 08:00:21.000000 orbitkit-0.3.2/MANIFEST.in
+-rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-24 09:23:30.000000 orbitkit-0.3.2/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     2207 2021-10-31 14:45:20.000000 orbitkit-0.3.2/README.md
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/
+-rw-r--r--   0 crown      (501) staff       (20)        6 2023-05-24 09:22:50.000000 orbitkit-0.3.2/orbitkit/VERSION
+-rw-r--r--   0 crown      (501) staff       (20)      354 2023-05-22 01:04:02.000000 orbitkit-0.3.2/orbitkit/__init__.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/file_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        1 2021-07-15 08:55:40.000000 orbitkit-0.3.2/orbitkit/file_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     2111 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/dispatcher.py
+-rw-r--r--   0 crown      (501) staff       (20)      244 2021-10-31 03:25:18.000000 orbitkit-0.3.2/orbitkit/file_extractor/exception.py
+-rw-r--r--   0 crown      (501) staff       (20)     1912 2021-10-31 14:48:38.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor.py
+-rw-r--r--   0 crown      (501) staff       (20)      224 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_audio.py
+-rw-r--r--   0 crown      (501) staff       (20)     1211 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_html.py
+-rw-r--r--   0 crown      (501) staff       (20)     2034 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_json.py
+-rw-r--r--   0 crown      (501) staff       (20)     1016 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_office.py
+-rw-r--r--   0 crown      (501) staff       (20)     2983 2022-05-06 07:35:45.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_pdf.py
+-rw-r--r--   0 crown      (501) staff       (20)      868 2021-10-31 14:31:58.000000 orbitkit-0.3.2/orbitkit/file_extractor/extractor_txt.py
+-rw-r--r--   0 crown      (501) staff       (20)      277 2021-07-27 10:13:23.000000 orbitkit-0.3.2/orbitkit/file_extractor/util.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/id_srv/
+-rw-r--r--   0 crown      (501) staff       (20)       22 2021-12-26 09:49:52.000000 orbitkit-0.3.2/orbitkit/id_srv/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     1533 2021-12-26 11:07:53.000000 orbitkit-0.3.2/orbitkit/id_srv/id_gen.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/lark_send/
+-rw-r--r--   0 crown      (501) staff       (20)       20 2022-01-05 07:16:58.000000 orbitkit-0.3.2/orbitkit/lark_send/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)     5064 2022-01-05 07:16:58.000000 orbitkit-0.3.2/orbitkit/lark_send/lark.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/pdf_extractor/
+-rw-r--r--   0 crown      (501) staff       (20)        0 2023-05-10 05:20:41.000000 orbitkit-0.3.2/orbitkit/pdf_extractor/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      621 2023-05-10 06:21:50.000000 orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py
+-rw-r--r--   0 crown      (501) staff       (20)     6115 2023-05-24 08:44:38.000000 orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py
+-rw-r--r--   0 crown      (501) staff       (20)    13625 2023-05-24 09:10:22.000000 orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit/util/
+-rw-r--r--   0 crown      (501) staff       (20)      104 2023-05-10 05:26:36.000000 orbitkit-0.3.2/orbitkit/util/__init__.py
+-rw-r--r--   0 crown      (501) staff       (20)      790 2023-05-10 05:20:41.000000 orbitkit-0.3.2/orbitkit/util/common.py
+-rw-r--r--   0 crown      (501) staff       (20)      520 2023-05-10 05:26:36.000000 orbitkit-0.3.2/orbitkit/util/util_aws.py
+-rw-r--r--   0 crown      (501) staff       (20)     1781 2023-05-20 01:15:42.000000 orbitkit-0.3.2/orbitkit/util/util_date.py
+-rw-r--r--   0 crown      (501) staff       (20)      148 2023-05-10 05:19:04.000000 orbitkit-0.3.2/orbitkit/util/util_str.py
+-rw-r--r--   0 crown      (501) staff       (20)    19087 2021-12-26 13:51:52.000000 orbitkit-0.3.2/orbitkit/util/util_type_mapping.py
+drwxr-xr-x   0 crown      (501) staff       (20)        0 2023-05-24 09:23:30.000000 orbitkit-0.3.2/orbitkit.egg-info/
+-rw-r--r--   0 crown      (501) staff       (20)     3828 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/PKG-INFO
+-rw-r--r--   0 crown      (501) staff       (20)     1159 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/SOURCES.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/dependency_links.txt
+-rw-r--r--   0 crown      (501) staff       (20)        1 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/not-zip-safe
+-rw-r--r--   0 crown      (501) staff       (20)       89 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/requires.txt
+-rw-r--r--   0 crown      (501) staff       (20)        9 2023-05-24 09:23:29.000000 orbitkit-0.3.2/orbitkit.egg-info/top_level.txt
+-rw-r--r--   0 crown      (501) staff       (20)       38 2023-05-24 09:23:30.000000 orbitkit-0.3.2/setup.cfg
+-rw-r--r--   0 crown      (501) staff       (20)     1547 2023-05-10 05:35:02.000000 orbitkit-0.3.2/setup.py
```

### Comparing `orbitkit-0.3.1/LICENSE` & `orbitkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/PKG-INFO` & `orbitkit-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.3.1/README.md` & `orbitkit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/dispatcher.py` & `orbitkit-0.3.2/orbitkit/file_extractor/dispatcher.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor_html.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor_html.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor_json.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor_json.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor_office.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor_office.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor_pdf.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor_pdf.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/file_extractor/extractor_txt.py` & `orbitkit-0.3.2/orbitkit/file_extractor/extractor_txt.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/id_srv/id_gen.py` & `orbitkit-0.3.2/orbitkit/id_srv/id_gen.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/lark_send/lark.py` & `orbitkit-0.3.2/orbitkit/lark_send/lark.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_base.py` & `orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_base.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_v1.py` & `orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     @classmethod
     def from_local_file(cls, local_path: str, extend_meta: dict, pages: Optional[List[int]] = None):
         return cls(local_path, extend_meta, pages)
 
     def loop_pages(self, page_layout):
         index = 1
+        sentence_list_page = []
         for element in page_layout:
             # 如果页面的元素是 LTTextContainer 则直接拿数据
             if isinstance(element, LTTextContainer):
                 sentence = element.get_text()
                 # Filter sentence
                 sentence_obj = self._sentence_filter(sentence)
                 if sentence_obj['is_valid_sentence'] is False:
@@ -47,15 +48,15 @@
                     "sentence": sentence,
                     "type": "sentence",
                     "text_location": {
                         "location": [[element.x0, element.y1, element.x1, element.y0]]
                     }
                 }
                 _txt_data.update(self.extend_meta)  # 合并额外信息
-                self.sentence_list.append(_txt_data)
+                sentence_list_page.append(_txt_data)
                 index += 1
 
             # 如果页面的元素是 LTFigure 则拼接字符拿数据
             if isinstance(element, LTFigure):
                 sentence_item = ''
                 x0_list = []
                 y1_list = []
@@ -89,39 +90,67 @@
                         "seq_no": str(index),
                         "sentence": sentence,
                         "type": "sentence",
                         "text_location": {
                             "location": [location]}
                     }
                     _txt_data.update(self.extend_meta)  # 合并额外信息
-                    self.sentence_list.append(_txt_data)
+                    sentence_list_page.append(_txt_data)
                     index += 1
 
             # 如果两个 if 都匹配不上则说明此 element 没有数据
             pass
 
+        # 最后返回当页的提取结果
+        return sentence_list_page
+
     def extract(self):
         """入口方法
         可以根据 specific_page 选择是提取单独一页的数据还是全部解析
         """
         start_extract_time = time.perf_counter()
         logger.warning('Start extract pdf...')
 
         page_layouts = extract_pages(self.local_path)
         # 解析单独一页数据
         if self.pages:
             for page_layout in page_layouts:
                 if page_layout.pageid in self.pages:
-                    self.loop_pages(page_layout)
+                    ordered_sentence_list_page = self.loop_pages(page_layout)
+                    # 合并入到总的列表中
+                    self.sentence_list.extend(ordered_sentence_list_page)
         else:
             # 解析所有页面
             for page_layout in page_layouts:
-                self.loop_pages(page_layout)
+                ordered_sentence_list_page = self.loop_pages(page_layout)
+                # 合并入到总的列表中
+                self.sentence_list.extend(ordered_sentence_list_page)
 
         end_extract_time = time.perf_counter() - start_extract_time
         logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
 
         return self.sentence_list
 
+    def extract_iter(self):
+        """入口方法
+        可以根据 specific_page 选择是提取单独一页的数据还是全部解析
+        """
+        start_extract_time = time.perf_counter()
+        logger.warning('Start extract pdf...')
+
+        page_layouts = extract_pages(self.local_path)
+        # 解析单独一页数据
+        if self.pages:
+            for page_layout in page_layouts:
+                if page_layout.pageid in self.pages:
+                    yield self.loop_pages(page_layout)
+        else:
+            # 解析所有页面
+            for page_layout in page_layouts:
+                yield self.loop_pages(page_layout)
+
+        end_extract_time = time.perf_counter() - start_extract_time
+        logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
+
 
 if __name__ == '__main__':
     pass
```

### Comparing `orbitkit-0.3.1/orbitkit/pdf_extractor/pdf_block_extractor_v2.py` & `orbitkit-0.3.2/orbitkit/pdf_extractor/pdf_block_extractor_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,52 +50,95 @@
         logger.warning('Start extract pdf...')
 
         page_layouts = extract_pages(self.local_path)
         # 解析单独一页数据
         if self.pages:
             for page_layout in page_layouts:
                 if page_layout.pageid in self.pages:
-                    self.loop_pages(page_layout)
+                    ordered_sentence_list_page = self.loop_pages(page_layout)
+                    # 合并入到总的列表中
+                    self.sentence_list.extend(ordered_sentence_list_page)
         else:
             # 解析所有页面
             for page_layout in page_layouts:
-                self.loop_pages(page_layout)
+                ordered_sentence_list_page = self.loop_pages(page_layout)
+                # 合并入到总的列表中
+                self.sentence_list.extend(ordered_sentence_list_page)
 
         end_extract_time = time.perf_counter() - start_extract_time
         logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
 
         return self.sentence_list
 
+    def extract_iter(self):
+        """入口方法
+        可以根据 specific_page 选择是提取单独一页的数据还是全部解析
+        """
+
+        start_extract_time = time.perf_counter()
+        logger.warning('Start extract pdf...')
+
+        page_layouts = extract_pages(self.local_path)
+        # 解析单独一页数据
+        if self.pages:
+            for page_layout in page_layouts:
+                if page_layout.pageid in self.pages:
+                    yield self.loop_pages(page_layout)
+        else:
+            # 解析所有页面
+            for page_layout in page_layouts:
+                yield self.loop_pages(page_layout)
+
+        end_extract_time = time.perf_counter() - start_extract_time
+        logger.warning(f'End extract pdf with cost time {str(end_extract_time * 1000)}')
+
     def loop_pages(self, page_layout):
         """处理单独一页的数据
         1. 通过 pdfplumber 提取表格信息
         2. 通过 pdfminer 提取文本 block 信息
         """
         logger.info(f"Start inspect page {str(page_layout.pageid)}...")
 
         sentence_list_page = []
         # 尝试得到每一页的表格
-        tables = self.pdf_plumber_pages[page_layout.pageid - 1].extract_tables()
+        pdf_plumber_page = self.pdf_plumber_pages[page_layout.pageid - 1]
+        '''
+        https://github.com/jsvine/pdfplumber/issues/193
+        Memory issues on very large PDFs
+        
+        I found that after extracting text, the lru_cache was somehow not being cleared causing the memory to keep filling up and eventually run out of it. After some playing around I found the following code helped me. In the code below, I am clearing the page cache and the lru cache.
+        with pdfplumber.open("path-to-pdf/my.pdf") as pdf:
+            for page in pdf.pages:
+            text = page.extract_text(layout=True)
+            page.flush_cache()
+        
+           # This was the fn where cache is implemented
+           page.get_text_layout.cache_clear()     `
+        PS: I am currently using pdfplumber version 0.71. I hope this helps someone.
+        '''
+        tables = pdf_plumber_page.extract_tables()
+        pdf_plumber_page.flush_cache()
+
         # 过滤无用表格，并构建表格扩展对象
-        tables_obj = self.__filter_extend_tables(tables)
+        tables_obj = self._filter_extend_tables(tables)
 
         # 遍历页面所有的元素开始解析
         index = 1
         for element in page_layout:
             # 如果页面的元素是 LTTextContainer 则直接拿数据
             if isinstance(element, LTTextContainer):
                 sentence = element.get_text()
 
                 # 如果 sentence 为空字符串，则本条数据没有意义
                 if sentence.strip() == '':
                     continue
 
                 # If element in table，则统一处理本页的 table
                 if len(tables_obj) > 0:
-                    is_exist_in_table = self.__element_in_table(element, index, tables_obj)
+                    is_exist_in_table = self._element_in_table(element, index, tables_obj)
                     if is_exist_in_table:
                         index += 1
                         continue
 
                 # Filter sentence
                 sentence_obj = self._sentence_filter(sentence)
                 if sentence_obj['is_valid_sentence'] is False:
@@ -182,49 +225,46 @@
             item_table['location'].append(min(item_table['y0_list']))
 
             # 合并进入 sentence_list_page
             _txt_data = {
                 "id": f"l_{id_srv.get_random_short_id()}",
                 "page": page_layout.pageid,
                 "seq_no": min(item_table['index_set']),
-                "sentence": self.__get_html_table_format(item_table['table']),
+                "sentence": self._get_html_table_format(item_table['table']),
                 "type": "table",
                 "text_location": {
                     "location": [item_table['location']]
                 }
             }
             _txt_data.update(self.extend_meta)  # 合并额外信息
             sentence_list_page.append(_txt_data)
 
         # 最后对新的 sentence_list_page 进行排序
         ordered_sentence_list_page = sorted(sentence_list_page, key=lambda item_sen: item_sen['seq_no'])
         # 重新设置顺序信息
         for ind, item in enumerate(ordered_sentence_list_page):
             item['seq_no'] = ind + 1
 
-        # for itemxxx in ordered_sentence_list_page:
-        #     print(itemxxx)
-
         # 合并入到总的列表中
-        self.sentence_list.extend(ordered_sentence_list_page)
+        return ordered_sentence_list_page
 
-    def __element_in_table(self, element: Union[LTTextContainer], index: int, tables_obj):
+    def _element_in_table(self, element: Union[LTTextContainer], index: int, tables_obj):
         is_exist_in_table = False
         for table_info in tables_obj:
             if element.get_text().strip() in table_info['values_set']:
                 is_exist_in_table = True
                 table_info['index_set'].append(index)
                 table_info['x0_list'].append(element.x0)
                 table_info['y1_list'].append(element.y1)
                 table_info['x1_list'].append(element.x1)
                 table_info['y0_list'].append(element.y0)
                 # break
         return is_exist_in_table
 
-    def __filter_extend_tables(self, tables: List[List[List[Optional[str]]]]):
+    def _filter_extend_tables(self, tables: List[List[List[Optional[str]]]]):
         """对 table 信息进行扩展
         table_info = {
             'x0_list': [],
             'y1_list': [],
             'x1_list': [],
             'y0_list': [],
             'table': [], # 得到去掉 None 信息后的 table
@@ -276,15 +316,15 @@
 
             # 判断 table 中是否有有效数据
             if len(values_set) > 0:
                 tables_obj.append(table_info)
 
         return tables_obj
 
-    def __get_html_table_format(self, table):
+    def _get_html_table_format(self, table):
         tb = PrettyTable()
         for row in table:
             tb.add_row(row)
 
         return tb.get_html_string(header=False)
```

### Comparing `orbitkit-0.3.1/orbitkit/util/common.py` & `orbitkit-0.3.2/orbitkit/util/common.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/util/util_aws.py` & `orbitkit-0.3.2/orbitkit/util/util_aws.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/util/util_date.py` & `orbitkit-0.3.2/orbitkit/util/util_date.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit/util/util_type_mapping.py` & `orbitkit-0.3.2/orbitkit/util/util_type_mapping.py`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/orbitkit.egg-info/PKG-INFO` & `orbitkit-0.3.2/orbitkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbitkit
-Version: 0.3.1
+Version: 0.3.2
 Summary: This project is only for Orbit Tech internal use.
 Home-page: https://github.com/clown-0726/orbitkit
 Author: Lilu Cao
 Author-email: lilu.cao@qq.com
 Maintainer: Lilu Cao
 Maintainer-email: lilu.cao@qq.com
 License: MIT License
```

### Comparing `orbitkit-0.3.1/orbitkit.egg-info/SOURCES.txt` & `orbitkit-0.3.2/orbitkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orbitkit-0.3.1/setup.py` & `orbitkit-0.3.2/setup.py`

 * *Files identical despite different names*

