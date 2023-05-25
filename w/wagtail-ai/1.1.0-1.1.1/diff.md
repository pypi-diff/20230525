# Comparing `tmp/wagtail-ai-1.1.0.tar.gz` & `tmp/wagtail_ai-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-ai-1.1.0.tar", last modified: Thu Mar 16 09:29:24 2023, max compression
+gzip compressed data, was "wagtail_ai-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtail-ai-1.1.0.tar` & `wagtail_ai-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1113 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0       29 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1067 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/LICENSE
--rw-r--r--   0        0        0     4915 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/README.md
--rw-r--r--   0        0        0      560 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/SECURITY.md
--rw-r--r--   0        0        0     1800 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      497 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/setup.cfg
--rw-r--r--   0        0        0      169 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/wagtail_ai/__init__.py
--rw-r--r--   0        0        0      154 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/wagtail_ai/apps.py
--rw-r--r--   0        0        0        0 2023-03-16 09:28:03.832418 wagtail-ai-1.1.0/wagtail_ai/migrations/__init__.py
--rw-r--r--   0        0        0        0 2023-03-16 09:28:03.836418 wagtail-ai-1.1.0/wagtail_ai/models.py
--rw-r--r--   0        0        0      661 2023-03-16 09:28:03.836418 wagtail-ai-1.1.0/wagtail_ai/openai.py
--rw-r--r--   0        0        0     2337 2023-03-16 09:28:03.836418 wagtail-ai-1.1.0/wagtail_ai/prompts.py
--rw-r--r--   0        0        0      903 2023-03-16 09:28:38.420077 wagtail-ai-1.1.0/wagtail_ai/static/wagtail_ai/main.css
--rw-r--r--   0        0        0     8661 2023-03-16 09:28:38.420077 wagtail-ai-1.1.0/wagtail_ai/static/wagtail_ai/wagtail-ai.js
--rw-r--r--   0        0        0     2872 2023-03-16 09:28:03.836418 wagtail-ai-1.1.0/wagtail_ai/views.py
--rw-r--r--   0        0        0     1537 2023-03-16 09:28:03.836418 wagtail-ai-1.1.0/wagtail_ai/wagtail_hooks.py
--rw-r--r--   0        0        0     6367 1970-01-01 00:00:00.000000 wagtail-ai-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1067 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4915 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/README.md
+-rw-r--r--   0        0        0      560 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/SECURITY.md
+-rw-r--r--   0        0        0     1800 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      497 2023-05-25 15:28:03.433240 wagtail_ai-1.1.1/setup.cfg
+-rw-r--r--   0        0        0      169 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/apps.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/models.py
+-rw-r--r--   0        0        0      661 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/openai.py
+-rw-r--r--   0        0        0     2337 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/prompts.py
+-rw-r--r--   0        0        0      903 2023-05-25 15:28:21.761210 wagtail_ai-1.1.1/wagtail_ai/static/wagtail_ai/main.css
+-rw-r--r--   0        0        0     8670 2023-05-25 15:28:21.761210 wagtail_ai-1.1.1/wagtail_ai/static/wagtail_ai/wagtail-ai.js
+-rw-r--r--   0        0        0     2872 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/views.py
+-rw-r--r--   0        0        0     1655 2023-05-25 15:28:03.437240 wagtail_ai-1.1.1/wagtail_ai/wagtail_hooks.py
+-rw-r--r--   0        0        0     6367 1970-01-01 00:00:00.000000 wagtail_ai-1.1.1/PKG-INFO
```

### Comparing `wagtail-ai-1.1.0/CHANGELOG.md` & `wagtail_ai-1.1.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # AI Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.1.1] - 2023-03-25
+
+### Changed
+
+- The URL used by the rich text editor button is now dynamically populated, fixing the issue where it would break if the admin URL had been changed.
+
 ## [1.1.0] - 2023-03-10
 
 ### Added
 
 - Support for customising prompts using the `WAGTAIL_AI_PROMPTS` setting
 
 ### Changed
```

### Comparing `wagtail-ai-1.1.0/LICENSE` & `wagtail_ai-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/README.md` & `wagtail_ai-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/SECURITY.md` & `wagtail_ai-1.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/pyproject.toml` & `wagtail_ai-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/wagtail_ai/openai.py` & `wagtail_ai-1.1.1/wagtail_ai/openai.py`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/wagtail_ai/prompts.py` & `wagtail_ai-1.1.1/wagtail_ai/prompts.py`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/wagtail_ai/static/wagtail_ai/main.css` & `wagtail_ai-1.1.1/wagtail_ai/static/wagtail_ai/main.css`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/wagtail_ai/static/wagtail_ai/wagtail-ai.js` & `wagtail_ai-1.1.1/wagtail_ai/static/wagtail_ai/wagtail-ai.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -192,15 +192,15 @@
                         return u(void 0, void 0, void 0, (function() {
                             var n, r, a, o;
                             return c(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
                                         (n = new FormData).append("text", e), n.append("prompt", t.id), i.label = 1;
                                     case 1:
-                                        return i.trys.push([1, 4, , 5]), [4, fetch("/admin/ai/process/", {
+                                        return i.trys.push([1, 4, , 5]), [4, fetch(window.WAGTAIL_AI_PROCESS_URL, {
                                             method: "POST",
                                             body: n
                                         })];
                                     case 2:
                                         return [4, (r = i.sent()).json()];
                                     case 3:
                                         if (a = i.sent(), r.ok) return [2, a.message];
@@ -209,21 +209,21 @@
                                         throw o = i.sent(), console.log("here"), new h(o.message);
                                     case 5:
                                         return [2]
                                 }
                             }))
                         }))
                     },
-                    b = function(e, t) {
+                    w = function(e, t) {
                         var n = f.RichUtils.insertSoftNewline(f.EditorState.moveSelectionToEnd(e)),
                             r = n.getCurrentContent(),
                             a = f.Modifier.replaceText(r, f.EditorState.moveSelectionToEnd(n).getSelection(), t);
                         return f.EditorState.push(n, a, "insert-characters")
                     },
-                    w = function(e, t) {
+                    b = function(e, t) {
                         var n = e.getCurrentContent(),
                             r = f.Modifier.replaceText(n, function(e) {
                                 var t = e.getBlockMap();
                                 return new f.SelectionState({
                                     anchorKey: t.first().getKey(),
                                     anchorOffset: 0,
                                     focusKey: t.last().getKey(),
@@ -291,19 +291,19 @@
                             return u(t, void 0, void 0, (function() {
                                 var t, n, a;
                                 return c(this, (function(i) {
                                     switch (i.label) {
                                         case 0:
                                             x(null), g(!1), f(!0), i.label = 1;
                                         case 1:
-                                            return i.trys.push([1, 6, , 7]), "append" !== e.method ? [3, 3] : (t = r, [4, _(o, e, b)]);
+                                            return i.trys.push([1, 6, , 7]), "append" !== e.method ? [3, 3] : (t = r, [4, _(o, e, w)]);
                                         case 2:
                                             return t.apply(void 0, [i.sent()]), [3, 5];
                                         case 3:
-                                            return n = r, [4, _(o, e, w)];
+                                            return n = r, [4, _(o, e, b)];
                                         case 4:
                                             n.apply(void 0, [i.sent()]), i.label = 5;
                                         case 5:
                                             return [3, 7];
                                         case 6:
                                             return a = i.sent(), x(a.message), [3, 7];
                                         case 7:
```

### Comparing `wagtail-ai-1.1.0/wagtail_ai/views.py` & `wagtail_ai-1.1.1/wagtail_ai/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-ai-1.1.0/wagtail_ai/wagtail_hooks.py` & `wagtail_ai-1.1.1/wagtail_ai/wagtail_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 
-from django.urls import include, path
+from django.urls import include, path, reverse
 from django.utils.safestring import mark_safe
 from django.views.i18n import JavaScriptCatalog
 from wagtail import hooks
 
 from .prompts import get_prompts
 from .views import process
 
@@ -53,15 +53,17 @@
         ),
     )
 
 
 @hooks.register("insert_editor_js")
 def ai_editor_js():
     prompt_json = json.dumps([prompt.as_dict() for prompt in get_prompts()])
+    process_url = reverse("wagtail_ai:process")
 
     return mark_safe(
         f"""
         <script>
+            window.WAGTAIL_AI_PROCESS_URL = "{process_url}";
             window.WAGTAIL_AI_PROMPTS = {prompt_json};
         </script>
         """
     )
```

### Comparing `wagtail-ai-1.1.0/PKG-INFO` & `wagtail_ai-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-ai
-Version: 1.1.0
+Version: 1.1.1
 Summary: Get a hand writing your content with AI super powers!
 Author-email: Tom Usher <tom@tomusher.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

