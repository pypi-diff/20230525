# Comparing `tmp/dagster-pagerduty-1.0.5.tar.gz` & `tmp/dagster_pagerduty-2019.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-pagerduty-1.0.5.tar", last modified: Fri Aug 26 13:45:48 2022, max compression
+gzip compressed data, was "dist/dagster_pagerduty-2019.6.2.tar", last modified: Sun Jun  2 23:36:40 2019, max compression
```

## Comparing `dagster-pagerduty-1.0.5.tar` & `dagster_pagerduty-2019.6.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:48.044566 dagster-pagerduty-1.0.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       69 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      657 2022-08-26 13:45:48.044566 dagster-pagerduty-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      137 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:48.044566 dagster-pagerduty-1.0.5/dagster_pagerduty/
--rw-r--r--   0 root         (0) root         (0)      277 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/dagster_pagerduty/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2782 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/dagster_pagerduty/hooks.py
--rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/dagster_pagerduty/py.typed
--rw-r--r--   0 root         (0) root         (0)     8180 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/dagster_pagerduty/resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/dagster_pagerduty/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:45:48.044566 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/
--rw-r--r--   0 root         (0) root         (0)      657 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       20 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-08-26 13:45:47.000000 dagster-pagerduty-1.0.5/dagster_pagerduty.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      164 2022-08-26 13:45:48.048566 dagster-pagerduty-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1318 2022-08-26 13:33:01.000000 dagster-pagerduty-1.0.5/setup.py
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty/
+-rw-r--r--   0 nate       (501) staff       (20)       56 2019-06-02 23:35:20.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty/version.py
+-rw-r--r--   0 nate       (501) staff       (20)      110 2019-04-27 21:03:42.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)     7295 2019-05-29 02:13:31.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty/resources.py
+-rw-r--r--   0 nate       (501) staff       (20)      587 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/PKG-INFO
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty_tests/
+-rw-r--r--   0 nate       (501) staff       (20)     1652 2019-05-21 23:28:27.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty_tests/test_resources.py
+-rw-r--r--   0 nate       (501) staff       (20)       95 2019-04-27 21:03:42.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty_tests/test_version.py
+-rw-r--r--   0 nate       (501) staff       (20)        0 2019-04-27 21:03:42.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty_tests/__init__.py
+-rw-r--r--   0 nate       (501) staff       (20)     1584 2019-05-29 02:13:31.000000 dagster_pagerduty-2019.6.2/README.md
+-rw-r--r--   0 nate       (501) staff       (20)     1781 2019-05-29 02:13:31.000000 dagster_pagerduty-2019.6.2/setup.py
+-rw-r--r--   0 nate       (501) staff       (20)       38 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/setup.cfg
+drwxr-xr-x   0 nate       (501) staff       (20)        0 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/
+-rw-r--r--   0 nate       (501) staff       (20)      587 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/PKG-INFO
+-rw-r--r--   0 nate       (501) staff       (20)        1 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/not-zip-safe
+-rw-r--r--   0 nate       (501) staff       (20)      470 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/SOURCES.txt
+-rw-r--r--   0 nate       (501) staff       (20)       20 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/requires.txt
+-rw-r--r--   0 nate       (501) staff       (20)       42 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/top_level.txt
+-rw-r--r--   0 nate       (501) staff       (20)        1 2019-06-02 23:36:40.000000 dagster_pagerduty-2019.6.2/dagster_pagerduty.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `dagster-pagerduty-1.0.5/PKG-INFO` & `dagster_pagerduty-2019.6.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-Metadata-Version: 2.1
-Name: dagster-pagerduty
-Version: 1.0.5
+Metadata-Version: 1.1
+Name: dagster_pagerduty
+Version: 2019.6.2
 Summary: Package for pagerduty Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-pagerduty
 Author: Elementl
-Author-email: hello@elementl.com
+Author-email: UNKNOWN
 License: Apache-2.0
+Description: UNKNOWN
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `dagster-pagerduty-1.0.5/dagster_pagerduty/resources.py` & `dagster_pagerduty-2019.6.2/dagster_pagerduty/resources.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-from typing import Dict, Optional, cast
-
 import pypd
 
-from dagster import Field, resource
+from dagster import resource, Dict, Field, String
 
 
 class PagerDutyService:
-    """Integrates with PagerDuty via the pypd library.
+    '''Integrates with PagerDuty via the pypd library.
 
     See:
         https://v2.developer.pagerduty.com/docs/events-api-v2
         https://v2.developer.pagerduty.com/docs/send-an-event-events-api-v2
         https://support.pagerduty.com/docs/services-and-integrations#section-events-api-v2
         https://github.com/PagerDuty/pagerduty-api-python-client
 
     for documentation and more information.
-    """
+    '''
 
-    def __init__(self, routing_key: str):
+    def __init__(self, routing_key):
         self.routing_key = routing_key
 
     def EventV2_create(
         self,
-        summary: str,
-        source: str,
-        severity: str,
-        event_action: str = "trigger",
-        dedup_key: Optional[str] = None,
-        timestamp: Optional[str] = None,
-        component: Optional[str] = None,
-        group: Optional[str] = None,
-        event_class: Optional[str] = None,
-        custom_details: Optional[object] = None,
-    ) -> object:
-        """Events API v2 enables you to add PagerDuty's advanced event and incident management
+        summary,
+        source,
+        severity,
+        event_action='trigger',
+        dedup_key=None,
+        timestamp=None,
+        component=None,
+        group=None,
+        event_class=None,
+        custom_details=None,
+    ):
+        '''Events API v2 enables you to add PagerDuty's advanced event and incident management
         functionality to any system that can make an outbound HTTP connection.
 
         Arguments:
             summary {string} -- A high-level, text summary message of the event. Will be used to
                                 construct an alert's description.
 
                                 Example: "PING OK - Packet loss = 0%, RTA = 1.41 ms" "Host
@@ -117,78 +115,53 @@
                                     "500 Error"
 
             custom_details {Dict[str, str]} -- Additional details about the event and affected
                                                system.
 
                                                Example:
                                                {"ping time": "1500ms", "load avg": 0.75 }
-        """
+        '''
 
         data = {
-            "routing_key": self.routing_key,
-            "event_action": event_action,
-            "payload": {"summary": summary, "source": source, "severity": severity},
+            'routing_key': self.routing_key,
+            'event_action': event_action,
+            'payload': {'summary': summary, 'source': source, 'severity': severity},
         }
 
         if dedup_key is not None:
-            data["dedup_key"] = dedup_key
-
-        payload: Dict[str, object] = cast(Dict[str, object], data["payload"])
+            data['dedup_key'] = dedup_key
 
         if timestamp is not None:
-            payload["timestamp"] = timestamp
+            data['payload']['timestamp'] = timestamp
 
         if component is not None:
-            payload["component"] = component
+            data['payload']['component'] = component
 
         if group is not None:
-            payload["group"] = group
+            data['payload']['group'] = group
 
         if event_class is not None:
-            payload["class"] = event_class
+            data['payload']['class'] = event_class
 
         if custom_details is not None:
-            payload["custom_details"] = custom_details
+            data['payload']['custom_details'] = custom_details
 
         return pypd.EventV2.create(data=data)
 
 
 @resource(
-    {
-        "routing_key": Field(
-            str,
-            description="""The routing key provisions access to your PagerDuty service. You
+    config_field=Field(
+        Dict(
+            {
+                'routing_key': Field(
+                    String,
+                    description='''The routing key provisions access to your PagerDuty service. You
                     will need to include the integration key for your new integration, as a
-                    routing_key in the event payload.""",
+                    routing_key in the event payload.''',
+                )
+            }
         )
-    },
-    description="""This resource is for posting events to PagerDuty.""",
+    ),
+    description='''This resource is for posting events to PagerDuty.''',
 )
 def pagerduty_resource(context):
-    """A resource for posting events (alerts) to PagerDuty.
-
-    Example:
-
-    .. code-block:: python
-
-        @op(required_resource_keys={'pagerduty'})
-        def pagerduty_op(context):
-            context.resources.pagerduty.EventV2_create(
-                summary='alert from dagster'
-                source='localhost',
-                severity='error',
-                event_action='trigger',
-            )
-
-        @job(resource_defs={ 'pagerduty': pagerduty_resource })
-        def pagerduty_test():
-            pagerduty_op()
-
-        pagerduty_test.execute_in_process(
-            run_config={
-                "resources": {
-                    'pagerduty': {'config': {'routing_key': '0123456789abcdef0123456789abcdef'}}
-                }
-            }
-        )
-    """
-    return PagerDutyService(context.resource_config.get("routing_key"))
+    return PagerDutyService(context.resource_config.get('routing_key'))
```

