# Comparing `tmp/django_plausible_proxy-0.4.0.tar.gz` & `tmp/django_plausible_proxy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_plausible_proxy-0.4.0.tar", max compression
+gzip compressed data, was "django_plausible_proxy-0.5.0.tar", max compression
```

## Comparing `django_plausible_proxy-0.4.0.tar` & `django_plausible_proxy-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-29 16:33:02.467878 django_plausible_proxy-0.4.0/LICENSE
--rw-r--r--   0        0        0     5000 2023-03-30 09:46:16.507159 django_plausible_proxy-0.4.0/README.md
--rw-r--r--   0        0        0      117 2023-03-30 09:58:03.813554 django_plausible_proxy-0.4.0/plausible_proxy/__init__.py
--rw-r--r--   0        0        0      199 2023-03-29 16:33:02.468139 django_plausible_proxy-0.4.0/plausible_proxy/apps.py
--rw-r--r--   0        0        0     5287 2023-03-30 09:46:16.508022 django_plausible_proxy-0.4.0/plausible_proxy/services.py
--rw-r--r--   0        0        0        0 2023-03-29 16:33:02.468288 django_plausible_proxy-0.4.0/plausible_proxy/templatetags/__init__.py
--rw-r--r--   0        0        0     1221 2023-03-29 16:33:02.468368 django_plausible_proxy-0.4.0/plausible_proxy/templatetags/plausible.py
--rw-r--r--   0        0        0      333 2023-03-29 16:33:02.468435 django_plausible_proxy-0.4.0/plausible_proxy/urls.py
--rw-r--r--   0        0        0     1405 2023-03-30 09:46:16.508504 django_plausible_proxy-0.4.0/plausible_proxy/views.py
--rw-r--r--   0        0        0     1181 2023-03-30 09:58:03.812898 django_plausible_proxy-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-03-29 16:33:02.468686 django_plausible_proxy-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      449 2023-03-29 16:33:02.468750 django_plausible_proxy-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1569 2023-03-29 16:45:01.310047 django_plausible_proxy-0.4.0/tests/test_services.py
--rw-r--r--   0        0        0     1393 2023-03-29 16:33:02.468900 django_plausible_proxy-0.4.0/tests/test_templatetags.py
--rw-r--r--   0        0        0      647 2023-03-29 16:33:02.468970 django_plausible_proxy-0.4.0/tests/test_views.py
--rw-r--r--   0        0        0      104 2023-03-29 16:33:02.469030 django_plausible_proxy-0.4.0/tests/urlconf.py
--rw-r--r--   0        0        0     6136 1970-01-01 00:00:00.000000 django_plausible_proxy-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-29 16:33:02.467878 django_plausible_proxy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5420 2023-05-25 14:56:26.029553 django_plausible_proxy-0.5.0/README.md
+-rw-r--r--   0        0        0      117 2023-05-25 15:41:35.846854 django_plausible_proxy-0.5.0/plausible_proxy/__init__.py
+-rw-r--r--   0        0        0      199 2023-03-29 16:33:02.468139 django_plausible_proxy-0.5.0/plausible_proxy/apps.py
+-rw-r--r--   0        0        0     5450 2023-05-25 15:19:41.810973 django_plausible_proxy-0.5.0/plausible_proxy/services.py
+-rw-r--r--   0        0        0        0 2023-03-29 16:33:02.468288 django_plausible_proxy-0.5.0/plausible_proxy/templatetags/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-25 15:41:31.623616 django_plausible_proxy-0.5.0/plausible_proxy/templatetags/plausible.py
+-rw-r--r--   0        0        0      333 2023-03-29 16:33:02.468435 django_plausible_proxy-0.5.0/plausible_proxy/urls.py
+-rw-r--r--   0        0        0     1405 2023-03-30 09:46:16.508504 django_plausible_proxy-0.5.0/plausible_proxy/views.py
+-rw-r--r--   0        0        0     1134 2023-05-25 15:41:35.846344 django_plausible_proxy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-03-29 16:33:02.468686 django_plausible_proxy-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      449 2023-03-29 16:33:02.468750 django_plausible_proxy-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1983 2023-05-25 15:09:55.667435 django_plausible_proxy-0.5.0/tests/test_services.py
+-rw-r--r--   0        0        0     1984 2023-05-25 15:41:31.623824 django_plausible_proxy-0.5.0/tests/test_templatetags.py
+-rw-r--r--   0        0        0      647 2023-03-29 16:33:02.468970 django_plausible_proxy-0.5.0/tests/test_views.py
+-rw-r--r--   0        0        0      104 2023-03-29 16:33:02.469030 django_plausible_proxy-0.5.0/tests/urlconf.py
+-rw-r--r--   0        0        0     6502 1970-01-01 00:00:00.000000 django_plausible_proxy-0.5.0/PKG-INFO
```

### Comparing `django_plausible_proxy-0.4.0/LICENSE` & `django_plausible_proxy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_plausible_proxy-0.4.0/README.md` & `django_plausible_proxy-0.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+![Dev workflow](https://github.com/imankulov/django-plausible-proxy/workflows/dev%20workflow/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plausible-proxy.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible-proxy.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plausible-proxy.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plausible-proxy.svg)
+
+
 # Django Plausible Proxy
 
 Django application to proxy requests and send server-side events to Plausible Analytics. Plays well with self-hosted and the managed cloud service.
 
 ## Proxying
 
 Proxying allows a project owner concerned about missing data seeing a more complete picture. See [Adblockers and using a proxy for analytics](https://plausible.io/docs/proxy/introduction) for the detailed outline of the problem and solution.
```

### Comparing `django_plausible_proxy-0.4.0/plausible_proxy/services.py` & `django_plausible_proxy-0.5.0/plausible_proxy/services.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 def send_custom_event(
     request: HttpRequest,
     name: str,
     domain: Optional[str] = None,
     url: Optional[str] = None,
     referrer: Optional[str] = None,
     screen_width: Optional[int] = None,
+    remote_addr: Optional[str] = None,
     props: Optional[Dict[str, Any]] = None,
 ) -> bool:
     """Send a custom event to Plausible and return successful status.
 
     Ref: https://plausible.io/docs/events-api
 
     Args:
@@ -90,14 +91,16 @@
         name: Name of the event. Can specify `pageview` which is a special type of
             event in Plausible. All other names will be treated as custom events.
         url: URL of the page where the event was triggered. If the URL
             contains UTM parameters, they will be extracted and stored. If URL is not
             set, will be extracted from the request.
         referrer: Referrer for this event.
         screen_width: Width of the screen.
+        remote_addr: Remote address of the user. If not set, will be extracted from
+            the request.
         props: Custom properties for the event. See:
             https://plausible.io/docs/custom-event-goals#using-custom-props
 
     Returns:
         True if request was accepted successfully.
     """
     if url is None:
@@ -117,15 +120,15 @@
 
     try:
         resp = requests.post(
             get_plausible_event_api_endpoint(),
             json=event_data,
             headers={
                 "content-type": "application/json",
-                "x-forwarded-for": get_xff(request),
+                "x-forwarded-for": remote_addr or get_xff(request),
                 "user-agent": get_user_agent(request),
             },
             timeout=REQUEST_TIMEOUT,
         )
         return resp.ok
     except requests.Timeout:
         return False
```

### Comparing `django_plausible_proxy-0.4.0/plausible_proxy/templatetags/plausible.py` & `django_plausible_proxy-0.5.0/plausible_proxy/templatetags/plausible.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django import template
+from django.conf import settings
 from django.forms.utils import flatatt
 from django.urls import reverse
 from django.utils.safestring import mark_safe
 
-from plausible_proxy.services import get_default_domain
-
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
 def plausible(context, domain=None, script="script.js"):
     """Return a script tag referencing the script.js.
 
@@ -21,14 +20,21 @@
             the `<script src="...">`
 
     Returns:
         The script tag to include in the base template. E.g.,
         `<script data-domain="example.com" src="/js/script.js" defer></script>`
     """
     if domain is None:
-        domain = get_default_domain(context["request"])
+        domain = getattr(settings, "PLAUSIBLE_DOMAIN", None)
+    if domain is None:
+        request = context.get("request")
+        if request is None:
+            raise ValueError(
+                "PLAUSIBLE_DOMAIN is not defined and request is not set in context."
+            )
+        domain = request.get_host()
     attrs = {
         "defer": True,
         "data-domain": domain,
         "src": reverse("plausible:script-proxy", args=(script,)),
     }
     return mark_safe(f"<script{flatatt(attrs)}></script>")
```

#### html2text {}

```diff
@@ -1,14 +1,17 @@
-from django import template from django.forms.utils import flatatt from
-django.urls import reverse from django.utils.safestring import mark_safe from
-plausible_proxy.services import get_default_domain register = template.Library
-() @register.simple_tag(takes_context=True) def plausible(context, domain=None,
+from django import template from django.conf import settings from
+django.forms.utils import flatatt from django.urls import reverse from
+django.utils.safestring import mark_safe register = template.Library()
+@register.simple_tag(takes_context=True) def plausible(context, domain=None,
 script="script.js"): """Return a script tag referencing the script.js. Args:
 context: Template context. domain: The value to include in the `
 . If not set, the value is taken from PLAUSIBLE_DOMAIN. If PLAUSIBLE_DOMAIN is
 not defined, the value is taken from the request. script: the script name
 without path or domain name. The value to include in the `
-` """ if domain is None: domain = get_default_domain(context["request"]) attrs
-= { "defer": True, "data-domain": domain, "src": reverse("plausible:script-
-proxy", args=(script,)), } return mark_safe(f"
+` """ if domain is None: domain = getattr(settings, "PLAUSIBLE_DOMAIN", None)
+if domain is None: request = context.get("request") if request is None: raise
+ValueError( "PLAUSIBLE_DOMAIN is not defined and request is not set in
+context." ) domain = request.get_host() attrs = { "defer": True, "data-domain":
+domain, "src": reverse("plausible:script-proxy", args=(script,)), } return
+mark_safe(f"
 flatatt(attrs)}>
 ")
```

### Comparing `django_plausible_proxy-0.4.0/plausible_proxy/views.py` & `django_plausible_proxy-0.5.0/plausible_proxy/views.py`

 * *Files identical despite different names*

### Comparing `django_plausible_proxy-0.4.0/pyproject.toml` & `django_plausible_proxy-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "django-plausible-proxy"
-version = "0.4.0"
+version = "0.5.0"
 homepage = "https://github.com/imankulov/django-plausible-proxy"
 description = "Django module to proxy requests to Plausible Analytics."
 authors = ["Roman Imankulov <roman.imankulov@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "plausible_proxy" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.8"
+python = "^3.8"
 Django = ">=3.2"
 requests = "^2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-xdist = "^2.5.0"
 coverage = "^6.2"
```

### Comparing `django_plausible_proxy-0.4.0/tests/test_services.py` & `django_plausible_proxy-0.5.0/tests/test_services.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,7 +46,18 @@
     assert status is True
 
 
 def test_send_custom_event_successful_without_domain(rf, mock_requests):
     request = rf.get("/register", REMOTE_ADDR="1.2.3.4", SERVER_NAME="example.com")
     status = send_custom_event(request, "Register", props={"Plan": "premium"})
     assert status is True
+
+
+def test_send_custom_events_respects_explicit_remote_addr(rf, mock_requests):
+    request = rf.get("/register", REMOTE_ADDR="1.2.3.4", SERVER_NAME="example.com")
+    status = send_custom_event(
+        request, "Register", domain="example.com", remote_addr="1.2.3.5"
+    )
+    assert status is True
+
+    headers = mock_requests.post.call_args.kwargs["headers"]
+    assert headers["x-forwarded-for"] == "1.2.3.5"
```

### Comparing `django_plausible_proxy-0.4.0/tests/test_templatetags.py` & `django_plausible_proxy-0.5.0/tests/test_templatetags.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,14 +19,31 @@
     context = Context({"request": request})
     assert (
         template.render(context)
         == '<script data-domain="example2.com" src="/js/script.js" defer></script>'
     )
 
 
+def test_plausible_uses_plausible_domain_if_request_not_defined(rf, settings):
+    settings.PLAUSIBLE_DOMAIN = "example2.com"
+    template = Template("{% load plausible %}{% plausible %}")
+    context = Context()
+    assert (
+        template.render(context)
+        == '<script data-domain="example2.com" src="/js/script.js" defer></script>'
+    )
+
+
+def test_plausible_raises_exception_if_domain_not_defined_anywhere(rf, settings):
+    template = Template("{% load plausible %}{% plausible %}")
+    context = Context()
+    with pytest.raises(ValueError):
+        template.render(context)
+
+
 @pytest.mark.skip(
     "Test fails as urlconf and urls.py content is cached. "
     "Still, the test works in isolation"
 )
 def test_plausible_modifies_src_if_script_prefix_defined(rf, settings):
     settings.PLAUSIBLE_SCRIPT_PREFIX = "hello_world/js"
     request = rf.get("/", SERVER_NAME="example.com")
```

### Comparing `django_plausible_proxy-0.4.0/tests/test_views.py` & `django_plausible_proxy-0.5.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_plausible_proxy-0.4.0/PKG-INFO` & `django_plausible_proxy-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: django-plausible-proxy
-Version: 0.4.0
+Version: 0.5.0
 Summary: Django module to proxy requests to Plausible Analytics.
 Home-page: https://github.com/imankulov/django-plausible-proxy
 License: MIT
 Author: Roman Imankulov
 Author-email: roman.imankulov@gmail.com
-Requires-Python: >=3.7.8,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Django (>=3.2)
 Requires-Dist: requests (>=2,<3)
 Description-Content-Type: text/markdown
 
+![Dev workflow](https://github.com/imankulov/django-plausible-proxy/workflows/dev%20workflow/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/django-plausible-proxy.svg)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-plausible-proxy.svg)
+![PyPI - Status](https://img.shields.io/pypi/status/django-plausible-proxy.svg)
+![PyPI - License](https://img.shields.io/pypi/l/django-plausible-proxy.svg)
+
+
 # Django Plausible Proxy
 
 Django application to proxy requests and send server-side events to Plausible Analytics. Plays well with self-hosted and the managed cloud service.
 
 ## Proxying
 
 Proxying allows a project owner concerned about missing data seeing a more complete picture. See [Adblockers and using a proxy for analytics](https://plausible.io/docs/proxy/introduction) for the detailed outline of the problem and solution.
```

