# Comparing `tmp/extract_msg-0.41.1.tar.gz` & `tmp/extract_msg-0.41.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extract_msg-0.41.1.tar", last modified: Wed May 10 17:25:35 2023, max compression
+gzip compressed data, was "extract_msg-0.41.2.tar", last modified: Thu May 25 02:02:16 2023, max compression
```

## Comparing `extract_msg-0.41.1.tar` & `extract_msg-0.41.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.770595 extract_msg-0.41.1/
--rw-rw-rw-   0        0        0    75009 2023-05-10 17:25:32.000000 extract_msg-0.41.1/CHANGELOG.md
--rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.41.1/LICENSE.txt
--rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.41.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12267 2023-05-10 17:25:35.771592 extract_msg-0.41.1/PKG-INFO
--rw-rw-rw-   0        0        0    11460 2023-05-10 17:25:32.000000 extract_msg-0.41.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.682831 extract_msg-0.41.1/extract_msg/
--rw-rw-rw-   0        0        0     2254 2023-05-10 17:25:32.000000 extract_msg-0.41.1/extract_msg/__init__.py
--rw-rw-rw-   0        0        0     3542 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.728706 extract_msg-0.41.1/extract_msg/_rtf/
--rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/_rtf/__init__.py
--rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/_rtf/create_doc.py
--rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/_rtf/inject_rtf.py
--rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/_rtf/token.py
--rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/_rtf/tokenize_rtf.py
--rw-rw-rw-   0        0        0     6954 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/appointment.py
--rw-rw-rw-   0        0        0    13262 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/attachment.py
--rw-rw-rw-   0        0        0    16369 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/attachment_base.py
--rw-rw-rw-   0        0        0     3169 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/calendar.py
--rw-rw-rw-   0        0        0    21050 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/calendar_base.py
--rw-rw-rw-   0        0        0    27572 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/constants.py
--rw-rw-rw-   0        0        0    50103 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/contact.py
--rw-rw-rw-   0        0        0    58138 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/enums.py
--rw-rw-rw-   0        0        0     3377 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.733693 extract_msg-0.41.1/extract_msg/logging-config/
--rw-rw-rw-   0        0        0     2082 2023-05-09 19:47:37.000000 extract_msg-0.41.1/extract_msg/logging-config/logging-nt.json
--rw-rw-rw-   0        0        0     2058 2023-05-09 19:47:37.000000 extract_msg-0.41.1/extract_msg/logging-config/logging-posix.json
--rw-rw-rw-   0        0        0     3588 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_cancellation.py
--rw-rw-rw-   0        0        0     1628 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_exception.py
--rw-rw-rw-   0        0        0     3771 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_forward.py
--rw-rw-rw-   0        0        0     2043 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_related.py
--rw-rw-rw-   0        0        0     6784 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_request.py
--rw-rw-rw-   0        0        0     2415 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/meeting_response.py
--rw-rw-rw-   0        0        0      375 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/message.py
--rw-rw-rw-   0        0        0    58493 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/message_base.py
--rw-rw-rw-   0        0        0      201 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/message_signed.py
--rw-rw-rw-   0        0        0     7201 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/message_signed_base.py
--rw-rw-rw-   0        0        0    39208 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/msg.py
--rw-rw-rw-   0        0        0    12647 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/named.py
--rw-rw-rw-   0        0        0    41608 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/ole_writer.py
--rw-rw-rw-   0        0        0     2578 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/post.py
--rw-rw-rw-   0        0        0     6723 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/prop.py
--rw-rw-rw-   0        0        0     7602 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/properties.py
--rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.41.1/extract_msg/py.typed
--rw-rw-rw-   0        0        0    12677 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/recipient.py
--rw-rw-rw-   0        0        0     8976 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/signed_attachment.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.769599 extract_msg-0.41.1/extract_msg/structures/
--rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/__init__.py
--rw-rw-rw-   0        0        0    11677 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/_helpers.py
--rw-rw-rw-   0        0        0     6676 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/business_card.py
--rw-rw-rw-   0        0        0    19038 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/entry_id.py
--rw-rw-rw-   0        0        0     6161 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/misc_id.py
--rw-rw-rw-   0        0        0     7370 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/recurrence_pattern.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/report_tag.py
--rw-rw-rw-   0        0        0     1391 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/system_time.py
--rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/time_zone_definition.py
--rw-rw-rw-   0        0        0     2440 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/time_zone_struct.py
--rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/structures/tz_rule.py
--rw-rw-rw-   0        0        0    13190 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/task.py
--rw-rw-rw-   0        0        0     4162 2023-05-09 19:54:43.000000 extract_msg-0.41.1/extract_msg/task_request.py
--rw-rw-rw-   0        0        0    55888 2023-05-10 17:25:32.000000 extract_msg-0.41.1/extract_msg/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 17:25:35.708760 extract_msg-0.41.1/extract_msg.egg-info/
--rw-rw-rw-   0        0        0    12267 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      228 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 17:25:35.000000 extract_msg-0.41.1/extract_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      197 2023-05-09 19:54:43.000000 extract_msg-0.41.1/requirements.txt
--rw-rw-rw-   0        0        0      167 2023-05-10 17:25:35.773589 extract_msg-0.41.1/setup.cfg
--rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.41.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.781504 extract_msg-0.41.2/
+-rw-rw-rw-   0        0        0    75234 2023-05-25 02:02:13.000000 extract_msg-0.41.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35147 2023-05-09 19:47:37.000000 extract_msg-0.41.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      165 2023-05-09 19:47:37.000000 extract_msg-0.41.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12267 2023-05-25 02:02:16.781504 extract_msg-0.41.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11460 2023-05-25 02:02:13.000000 extract_msg-0.41.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.695243 extract_msg-0.41.2/extract_msg/
+-rw-rw-rw-   0        0        0     2254 2023-05-25 02:02:13.000000 extract_msg-0.41.2/extract_msg/__init__.py
+-rw-rw-rw-   0        0        0     3542 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.736401 extract_msg-0.41.2/extract_msg/_rtf/
+-rw-rw-rw-   0        0        0      425 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/_rtf/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/_rtf/create_doc.py
+-rw-rw-rw-   0        0        0     6250 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/_rtf/inject_rtf.py
+-rw-rw-rw-   0        0        0      856 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/_rtf/token.py
+-rw-rw-rw-   0        0        0     8932 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/_rtf/tokenize_rtf.py
+-rw-rw-rw-   0        0        0     6954 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/appointment.py
+-rw-rw-rw-   0        0        0    13262 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/attachment.py
+-rw-rw-rw-   0        0        0    16369 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/attachment_base.py
+-rw-rw-rw-   0        0        0     3169 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/calendar.py
+-rw-rw-rw-   0        0        0    21050 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/calendar_base.py
+-rw-rw-rw-   0        0        0    27572 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/constants.py
+-rw-rw-rw-   0        0        0    50103 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/contact.py
+-rw-rw-rw-   0        0        0    58866 2023-05-25 02:02:13.000000 extract_msg-0.41.2/extract_msg/enums.py
+-rw-rw-rw-   0        0        0     3377 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.740772 extract_msg-0.41.2/extract_msg/logging-config/
+-rw-rw-rw-   0        0        0     2082 2023-05-09 19:47:37.000000 extract_msg-0.41.2/extract_msg/logging-config/logging-nt.json
+-rw-rw-rw-   0        0        0     2058 2023-05-09 19:47:37.000000 extract_msg-0.41.2/extract_msg/logging-config/logging-posix.json
+-rw-rw-rw-   0        0        0     3588 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_cancellation.py
+-rw-rw-rw-   0        0        0     1628 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_exception.py
+-rw-rw-rw-   0        0        0     3771 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_forward.py
+-rw-rw-rw-   0        0        0     2043 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_related.py
+-rw-rw-rw-   0        0        0     6784 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_request.py
+-rw-rw-rw-   0        0        0     2415 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/meeting_response.py
+-rw-rw-rw-   0        0        0      375 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/message.py
+-rw-rw-rw-   0        0        0    59032 2023-05-25 02:02:13.000000 extract_msg-0.41.2/extract_msg/message_base.py
+-rw-rw-rw-   0        0        0      201 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/message_signed.py
+-rw-rw-rw-   0        0        0     7201 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/message_signed_base.py
+-rw-rw-rw-   0        0        0    39208 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/msg.py
+-rw-rw-rw-   0        0        0    12647 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/named.py
+-rw-rw-rw-   0        0        0    41608 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/ole_writer.py
+-rw-rw-rw-   0        0        0     2578 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/post.py
+-rw-rw-rw-   0        0        0     6723 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/prop.py
+-rw-rw-rw-   0        0        0     7602 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/properties.py
+-rw-rw-rw-   0        0        0        0 2023-05-09 19:47:37.000000 extract_msg-0.41.2/extract_msg/py.typed
+-rw-rw-rw-   0        0        0    12677 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/recipient.py
+-rw-rw-rw-   0        0        0     8976 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/signed_attachment.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.779507 extract_msg-0.41.2/extract_msg/structures/
+-rw-rw-rw-   0        0        0      336 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/__init__.py
+-rw-rw-rw-   0        0        0    11677 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/_helpers.py
+-rw-rw-rw-   0        0        0     6676 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/business_card.py
+-rw-rw-rw-   0        0        0    19038 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/entry_id.py
+-rw-rw-rw-   0        0        0     6161 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/misc_id.py
+-rw-rw-rw-   0        0        0     7370 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/recurrence_pattern.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/report_tag.py
+-rw-rw-rw-   0        0        0     1391 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/system_time.py
+-rw-rw-rw-   0        0        0     1616 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/time_zone_definition.py
+-rw-rw-rw-   0        0        0     2440 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/time_zone_struct.py
+-rw-rw-rw-   0        0        0     3263 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/structures/tz_rule.py
+-rw-rw-rw-   0        0        0    13190 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/task.py
+-rw-rw-rw-   0        0        0     4162 2023-05-09 19:54:43.000000 extract_msg-0.41.2/extract_msg/task_request.py
+-rw-rw-rw-   0        0        0    55888 2023-05-10 17:25:32.000000 extract_msg-0.41.2/extract_msg/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 02:02:16.717159 extract_msg-0.41.2/extract_msg.egg-info/
+-rw-rw-rw-   0        0        0    12267 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      228 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-25 02:02:16.000000 extract_msg-0.41.2/extract_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      197 2023-05-09 19:54:43.000000 extract_msg-0.41.2/requirements.txt
+-rw-rw-rw-   0        0        0      167 2023-05-25 02:02:16.783499 extract_msg-0.41.2/setup.cfg
+-rw-rw-rw-   0        0        0     1657 2023-05-09 19:47:37.000000 extract_msg-0.41.2/setup.py
```

### Comparing `extract_msg-0.41.1/CHANGELOG.md` & `extract_msg-0.41.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+**v0.41.2**
+* Updated annotations on `MessageBase.save`.
+* Added new enum `BodyTypes`.
+* Added property `MessageBase.detectedBodies` for detecting what bodies have been stored (not generated by the module) in the .msg file.
+
 **v0.41.1**
 * [[TeamMsgExtractor #362](https://github.com/TeamMsgExtractor/msg-extractor/issues/362)] Fixed an issue with the removal of the `--dev` option missing one of the checks (I swear I actually tested it).
 
 **v0.41.0**
 * [[TeamMsgExtractor #357](https://github.com/TeamMsgExtractor/msg-extractor/issues/357)] Fixed an issue where the properties stream being absent would raise an error message that was not clear.
 * [[TeamMsgExtractor #357](https://github.com/TeamMsgExtractor/msg-extractor/issues/357)] Added a way to suppress `StandardViolationError` for poorly created files. This may cause issues you might not expect since this exception is meant to stop the processing for a reason.
 * [[TeamMsgExtractor #223](https://github.com/TeamMsgExtractor/msg-extractor/issues/223)] Finally got around to dealing with signed attachments that are embedded MSG files. `SignedAttachment.data` now returns either `bytes` or `MSGFile`. `SignedAttachment` also now has a `asBytes` property that will return the bytes that created the signed attachment, regardless of if it is an MSG or not, making it unnecessary to call `MSGFile.exportBytes` to get the bytes of the embedded MSG file, which can add a small delay to your code. As `Attachment` is a much more complex class, it does *not* (at least yet) have this property. Also unlike `Attachment`, `SignedAttachment` *will not* throw an exception if the data is an MSG file but is not supported. Instead, it will simply be logged as a exception, but the code will continue. If the data is successfully read as an embedded MSG file, the `AttachmentType` will be `AttachmentType.SIGNED_EMBEDDED`.
```

### Comparing `extract_msg-0.41.1/LICENSE.txt` & `extract_msg-0.41.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/PKG-INFO` & `extract_msg-0.41.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract_msg
-Version: 0.41.1
+Version: 0.41.2
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -261,16 +261,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.1/README.rst` & `extract_msg-0.41.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -246,16 +246,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.1/extract_msg/__init__.py` & `extract_msg-0.41.2/extract_msg/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 __author__ = 'Destiny Peterson & Matthew Walker'
-__date__ = '2023-05-10'
-__version__ = '0.41.1'
+__date__ = '2023-05-24'
+__version__ = '0.41.2'
 
 __all__ = [
     # Modules:
     'constants',
     'enums',
     'exceptions',
```

### Comparing `extract_msg-0.41.1/extract_msg/__main__.py` & `extract_msg-0.41.2/extract_msg/__main__.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/_rtf/create_doc.py` & `extract_msg-0.41.2/extract_msg/_rtf/create_doc.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/_rtf/inject_rtf.py` & `extract_msg-0.41.2/extract_msg/_rtf/inject_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/_rtf/token.py` & `extract_msg-0.41.2/extract_msg/_rtf/token.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/_rtf/tokenize_rtf.py` & `extract_msg-0.41.2/extract_msg/_rtf/tokenize_rtf.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/appointment.py` & `extract_msg-0.41.2/extract_msg/appointment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/attachment.py` & `extract_msg-0.41.2/extract_msg/attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/attachment_base.py` & `extract_msg-0.41.2/extract_msg/attachment_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/calendar.py` & `extract_msg-0.41.2/extract_msg/calendar.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/calendar_base.py` & `extract_msg-0.41.2/extract_msg/calendar_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/constants.py` & `extract_msg-0.41.2/extract_msg/constants.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/contact.py` & `extract_msg-0.41.2/extract_msg/contact.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/enums.py` & `extract_msg-0.41.2/extract_msg/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __all__ = [
     'AddressBookType', 'AppointmentAuxilaryFlag', 'AppointmentColor',
     'AppointmentStateFlag', 'AttachErrorBehavior', 'AttachmentType',
     'BCImageAlignment', 'BCImageSource', 'BCLabelFormat', 'BCTemplateID',
-    'BCTextFormat', 'BusyStatus', 'ClientIntentFlag', 'Color',
+    'BCTextFormat', 'BodyTypes', 'BusyStatus', 'ClientIntentFlag', 'Color',
     'ContactAddressIndex', 'ContactLinkState', 'DeencapType',
     'DirectoryEntryType', 'DisplayType', 'ElectronicAddressProperties',
     'EntryIDType', 'EntryIDTypeHex', 'ErrorCode', 'ErrorCodeType', 'Gender',
     'IconIndex', 'Importance', 'Intelligence', 'MacintoshEncoding',
     'MeetingObjectChange', 'MeetingRecipientType', 'MeetingType',
     'MessageFormat', 'MessageType', 'NamedPropertyType', 'OORBodyFormat',
     'PostalAddressID', 'Priority', 'PropertiesType', 'RecipientRowFlagType',
@@ -260,14 +260,35 @@
     RIGHT_UI = 0b00011100
     RIGHT_UIM = 0b00011101
     RIGHT_UIB = 0b00011110
     RIGHT_UIBM = 0b00011111
 
 
 
+class BodyTypes(enum.IntFlag):
+    """
+    Enum representing the types of bodies found in a message. This does not
+    include bodies generated from other sources, and so is a good detection
+    method for generated bodies (if you check a body and it is not null, but it
+    is not listed in the enum, then it was generated from another body).
+
+    This is an IntFlag enum, so to check if a body was found use the & operator
+    with the body you are checking and ensuring the result isn't BodyTypes.None.
+    You can also convert the result to a bool. For example:
+
+    >>> rtfFound = bool(msg.detectedBodies & BodyTypes.RTF)
+    """
+    NONE = 0b000
+    PLAIN = 0b001
+    RTF = 0b010
+    HTML = 0b100
+    ALL = 0b111
+
+
+
 class BusyStatus(enum.Enum):
     """
     The availability of a use for the event described by the object.
 
     OL_FREE: The user is available.
     OL_TENTATIVE: The user has a tentative event scheduled.
     OL_BUSY: The user is busy.
@@ -463,15 +484,15 @@
     # [MS-OXOCNTC] WrappedEntryId Structure.
     WRAPPED = 'C091ADD3519DCF11A4A900AA0047FAA4'
 
 
 
 class ErrorBehavior(enum.IntFlag):
     """
-    The behavior to follow when handling an error in an MSG file and it's 
+    The behavior to follow when handling an error in an MSG file and it's
     attachments. This is an int flag enum, so the options you want will be ORed
     with each other.
 
     THROW: Throw the exception regardless of type.
     ATTACH_NOT_IMPLEMENTED: Silence the exception for NotImplementedError.
     ATTACH_BROKEN: Silence the exception for broken attachments.
     ATTACH_SUPPRESS_ALL: Silence the exception for NotImplementedError and for broken
@@ -1698,15 +1719,15 @@
     RECUR_CURRENT_TZREG = 0b1
     EFFECTIVE_TZREG = 0b10
 
 
 
 class _EnumDeprecator:
     """
-    Special class for handling deprecated enums in a way that shouldn't break 
+    Special class for handling deprecated enums in a way that shouldn't break
     existing code, including code for checking `is` on a member of the enum.
     """
     def __init__(self, oldClassName : str, newClass : enum.Enum, nameConversion : dict = {}, valueConversion : dict = {}):
         """
         :param oldClassName: The name to use in the deprecation message.
         :param newClass: The new enum class to look for the value in.
         :param nameConversion: A dictionary of old names to new names to
@@ -1728,28 +1749,28 @@
 
     def __getattr__(self, key):
         # Warn about the deprecation
         import warnings
         warnings.warn(self.__warnMessage, DeprecationWarning)
 
         return getattr(self.__new, self.__nameConv.get(key, key))
-    
+
     def __getitem__(self, name):
         # Warn about the deprecation
         import warnings
         warnings.warn(self.__warnMessage, DeprecationWarning)
 
         return self.__new.__getitem__(self.__nameConv.get(name, name))
 
 
 
 
 # Deprecated Enums
 AttachErrorBehavior = _EnumDeprecator(
-    'AttachErrorBehavior', 
+    'AttachErrorBehavior',
     ErrorBehavior,
     {
         'BROKEN': 'ATTACH_SUPPRESS_ALL',
         'NOT_IMPLEMENTED': 'ATTACH_NOT_IMPLEMENTED',
     },
     {
         2: 3
```

### Comparing `extract_msg-0.41.1/extract_msg/exceptions.py` & `extract_msg-0.41.2/extract_msg/exceptions.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/logging-config/logging-nt.json` & `extract_msg-0.41.2/extract_msg/logging-config/logging-nt.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/logging-config/logging-posix.json` & `extract_msg-0.41.2/extract_msg/logging-config/logging-posix.json`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_cancellation.py` & `extract_msg-0.41.2/extract_msg/meeting_cancellation.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_exception.py` & `extract_msg-0.41.2/extract_msg/meeting_exception.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_forward.py` & `extract_msg-0.41.2/extract_msg/meeting_forward.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_related.py` & `extract_msg-0.41.2/extract_msg/meeting_related.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_request.py` & `extract_msg-0.41.2/extract_msg/meeting_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/meeting_response.py` & `extract_msg-0.41.2/extract_msg/meeting_response.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/message_base.py` & `extract_msg-0.41.2/extract_msg/message_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+from __future__ import annotations
+
+
 __all__ = [
     'MessageBase',
 ]
 
 
 import base64
 import datetime
 import email.utils
+import functools
 import html
 import json
 import logging
 import os
 import pathlib
 import re
 import subprocess
@@ -22,15 +26,15 @@
 
 from email.parser import Parser as EmailParser
 from typing import Callable, List, Optional, Union
 
 from . import constants
 from ._rtf.create_doc import createDocument
 from ._rtf.inject_rtf import injectStartRTF
-from .enums import DeencapType, RecipientType
+from .enums import BodyTypes, DeencapType, RecipientType
 from .exceptions import (
         BadHtmlError, DataNotFoundError, DeencapMalformedData,
         DeencapNotEncapsulated, IncompatibleOptionsError, WKError
     )
 from .msg import MSGFile
 from .structures.report_tag import ReportTag
 from .recipient import Recipient
@@ -589,15 +593,15 @@
             logger.debug('RTF has encapsulated HTML, but injection method failed. It is likely dirty. Will use normal RTF injection method.')
 
         # If the normal encapsulated HTML injection fails or it isn't
         # encapsulated, use the internal _rtf module.
         logger.debug('Using _rtf module to inject RTF text header.')
         return createDocument(injectStartRTF(self.rtfBody, injectableHeader))
 
-    def save(self, **kwargs):
+    def save(self, **kwargs) -> MessageBase:
         """
         Saves the message body and attachments found in the message.
 
         The body and attachments are stored in a folder in the current running
         directory unless :param customPath: has been specified. The name of the
         folder will be determined by 3 factors.
            * If :param customFilename: has been set, the value provided for that
@@ -1023,14 +1027,29 @@
             dirName = '{0:02d}-{1:02d}-{2:02d}_{3:02d}{4:02d}'.format(*d) if d else 'UnknownDate'
             dirName += ' ' + (prepareFilename(self.subject) if self.subject else '[No subject]')
             dirName = dirName.strip()
 
             self._defaultFolderName = dirName
             return dirName
 
+    @functools.cached_property
+    def detectedBodies(self) -> BodyTypes:
+        """
+        The types of bodies stored in the .msg file.
+        """
+        bodies = BodyTypes.NONE
+        if self.sExists('__substg1.0_1000'):
+            bodies |= BodyTypes.PLAIN
+        if self.exists('__substg1.0_10090102'):
+            bodies |= BodyTypes.RTF
+        if self.exists('__substg1.0_10130102'):
+            bodies |= BodyTypes.HTML
+
+        return bodies
+
     @property
     def header(self):
         """
         Returns the message header, if it exists. Otherwise it will generate
         one.
         """
         try:
```

### Comparing `extract_msg-0.41.1/extract_msg/message_signed_base.py` & `extract_msg-0.41.2/extract_msg/message_signed_base.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/msg.py` & `extract_msg-0.41.2/extract_msg/msg.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/named.py` & `extract_msg-0.41.2/extract_msg/named.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/ole_writer.py` & `extract_msg-0.41.2/extract_msg/ole_writer.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/post.py` & `extract_msg-0.41.2/extract_msg/post.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/prop.py` & `extract_msg-0.41.2/extract_msg/prop.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/properties.py` & `extract_msg-0.41.2/extract_msg/properties.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/recipient.py` & `extract_msg-0.41.2/extract_msg/recipient.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/signed_attachment.py` & `extract_msg-0.41.2/extract_msg/signed_attachment.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/_helpers.py` & `extract_msg-0.41.2/extract_msg/structures/_helpers.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/business_card.py` & `extract_msg-0.41.2/extract_msg/structures/business_card.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/entry_id.py` & `extract_msg-0.41.2/extract_msg/structures/entry_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/misc_id.py` & `extract_msg-0.41.2/extract_msg/structures/misc_id.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/recurrence_pattern.py` & `extract_msg-0.41.2/extract_msg/structures/recurrence_pattern.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/report_tag.py` & `extract_msg-0.41.2/extract_msg/structures/report_tag.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/system_time.py` & `extract_msg-0.41.2/extract_msg/structures/system_time.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/time_zone_definition.py` & `extract_msg-0.41.2/extract_msg/structures/time_zone_definition.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/time_zone_struct.py` & `extract_msg-0.41.2/extract_msg/structures/time_zone_struct.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/structures/tz_rule.py` & `extract_msg-0.41.2/extract_msg/structures/tz_rule.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/task.py` & `extract_msg-0.41.2/extract_msg/task.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/task_request.py` & `extract_msg-0.41.2/extract_msg/task_request.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg/utils.py` & `extract_msg-0.41.2/extract_msg/utils.py`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/extract_msg.egg-info/PKG-INFO` & `extract_msg-0.41.2/extract_msg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-msg
-Version: 0.41.1
+Version: 0.41.2
 Summary: Extracts emails and attachments saved in Microsoft Outlook's .msg files
 Home-page: https://github.com/TeamMsgExtractor/msg-extractor
 Download-URL: https://github.com/TeamMsgExtractor/msg-extractor/archives/master
 Author: Destiny Peterson & Matthew Walker
 Author-email: arceusthe@gmail.com, mattgwwalker@gmail.com
 License: GPL
 Requires-Python: >=3.8
@@ -261,16 +261,16 @@
 major release to ensure continued support. Because of this, it is recommended to
 install it to a separate environment (like a vitural env) to not interfere with
 your access to the newest major version of extract-msg.
 
 .. |License: GPL v3| image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: LICENSE.txt
 
-.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.1-blue.svg
-   :target: https://pypi.org/project/extract-msg/0.41.1/
+.. |PyPI3| image:: https://img.shields.io/badge/pypi-0.41.2-blue.svg
+   :target: https://pypi.org/project/extract-msg/0.41.2/
 
 .. |PyPI2| image:: https://img.shields.io/badge/python-3.8+-brightgreen.svg
    :target: https://www.python.org/downloads/release/python-3816/
 .. _Matthew Walker: https://github.com/mattgwwalker
 .. _Destiny Peterson (The Elemental of Destruction): https://github.com/TheElementalOfDestruction
 .. _JP Bourget: https://github.com/punkrokk
 .. _Philippe Lagadec: https://github.com/decalage2
```

### Comparing `extract_msg-0.41.1/extract_msg.egg-info/SOURCES.txt` & `extract_msg-0.41.2/extract_msg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `extract_msg-0.41.1/setup.py` & `extract_msg-0.41.2/setup.py`

 * *Files identical despite different names*

